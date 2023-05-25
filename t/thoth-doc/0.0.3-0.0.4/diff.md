# Comparing `tmp/thoth_doc-0.0.3.tar.gz` & `tmp/thoth_doc-0.0.4.tar.gz`

## Comparing `thoth_doc-0.0.3.tar` & `thoth_doc-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,17 @@
--rw-r--r--   0        0        0    51725 2020-02-02 00:00:00.000000 thoth_doc-0.0.3/Thoth.svg.png
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 thoth_doc-0.0.3/src/thoth_doc/__init__.py
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 thoth_doc-0.0.3/src/thoth_doc/main.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 thoth_doc-0.0.3/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 thoth_doc-0.0.3/LICENSE
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 thoth_doc-0.0.3/README.md
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 thoth_doc-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 thoth_doc-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    28955 2020-02-02 00:00:00.000000 thoth_doc-0.0.4/Thoth.svg.png
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 thoth_doc-0.0.4/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 thoth_doc-0.0.4/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 thoth_doc-0.0.4/.pytest_cache/README.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 thoth_doc-0.0.4/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 thoth_doc-0.0.4/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 thoth_doc-0.0.4/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 thoth_doc-0.0.4/src/thoth_doc/__init__.py
+-rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 thoth_doc-0.0.4/src/thoth_doc/main.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 thoth_doc-0.0.4/src/thoth_doc/parsers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 thoth_doc-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 thoth_doc-0.0.4/tests/test_parsers.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 thoth_doc-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 thoth_doc-0.0.4/LICENSE
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 thoth_doc-0.0.4/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 thoth_doc-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 thoth_doc-0.0.4/PKG-INFO
```

### Comparing `thoth_doc-0.0.3/src/thoth_doc/main.py` & `thoth_doc-0.0.4/src/thoth_doc/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,37 +84,49 @@
             else:
                 name = ref[1]
             docstring = docstring.replace(ref[0], get_docstring(filepath, name))
     return docstring
 
 
 class DocGenerator:
+    parsers = []
+
     def __init__(self, docs_folder, compiled_docs_folder):
         self.docs_folder = docs_folder
         self.compiled_docs_folder = compiled_docs_folder
 
     def parse_file(self, filepath):
         compiled_markdown = ''
         cwd = os.getcwd()
         base = filepath.replace(self.docs_folder, '')
 
         with open(filepath) as f:
             markdown = f.readlines()
 
         for line in markdown:
-            matches = re.findall(RE_REFERENCE, line)
-            if not matches:
-                compiled_markdown += line
+            skip = False
+            for parser in self.parsers:
+                parsed = parser(line)
+                if parsed is not None:
+                    compiled_markdown += parsed
+                    skip = True
+                    break
+
+            if skip:
                 continue
 
+            matches = re.findall(r'(\[@(.+?)\])', line)
+
             for match in matches:
                 mod, name = match[1].split('#')
                 docstring = get_docstring(mod, name)
                 docstring = remove_whitespaces(docstring)
+                docstring = docstring.replace('\n', '\n\n')
                 line = line.replace(match[0], docstring)
+
             compiled_markdown += line
 
         with open(f'{cwd}/{self.compiled_docs_folder}{base}', 'w') as f:
             f.write(compiled_markdown)
 
     def create_folder_structure(self):
         cwd = os.getcwd()
```

### Comparing `thoth_doc-0.0.3/LICENSE` & `thoth_doc-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `thoth_doc-0.0.3/pyproject.toml` & `thoth_doc-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "thoth_doc"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Lev", email="smj510black@gmail.com" },
 ]
 description = "Dependency-free, lightweight docstring parser"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
+    "Topic :: Documentation",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/mariownyou/thoth-doc"
 "Bug Tracker" = "https://github.com/mariownyou/thoth-doc/issues"
```

