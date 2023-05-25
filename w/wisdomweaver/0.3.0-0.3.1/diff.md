# Comparing `tmp/wisdomweaver-0.3.0.tar.gz` & `tmp/wisdomweaver-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wisdomweaver-0.3.0.tar", last modified: Tue May 23 21:49:20 2023, max compression
+gzip compressed data, was "wisdomweaver-0.3.1.tar", last modified: Thu May 25 16:15:04 2023, max compression
```

## Comparing `wisdomweaver-0.3.0.tar` & `wisdomweaver-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-23 21:49:20.496689 wisdomweaver-0.3.0/
--rw-rw-r--   0 martin    (1000) martin    (1000)      588 2023-05-23 16:20:38.000000 wisdomweaver-0.3.0/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)     1998 2023-05-23 21:49:20.496689 wisdomweaver-0.3.0/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      776 2023-05-23 21:34:57.000000 wisdomweaver-0.3.0/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)     1180 2023-05-23 21:48:09.000000 wisdomweaver-0.3.0/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-05-23 21:49:20.496689 wisdomweaver-0.3.0/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)      337 2023-05-23 20:03:42.000000 wisdomweaver-0.3.0/setup.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-23 21:49:20.492689 wisdomweaver-0.3.0/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1238 2023-05-13 10:37:32.000000 wisdomweaver-0.3.0/tests/test_database.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1114 2023-05-13 10:35:01.000000 wisdomweaver-0.3.0/tests/test_document.py
--rwxrwxr-x   0 martin    (1000) martin    (1000)     4334 2023-05-23 21:28:31.000000 wisdomweaver-0.3.0/wisdom
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-23 21:49:20.496689 wisdomweaver-0.3.0/wisdomweaver/
--rw-rw-r--   0 martin    (1000) martin    (1000)      241 2023-05-23 21:48:09.000000 wisdomweaver-0.3.0/wisdomweaver/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)       93 2023-05-23 20:05:48.000000 wisdomweaver-0.3.0/wisdomweaver/__main__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1984 2023-05-23 18:49:00.000000 wisdomweaver-0.3.0/wisdomweaver/database.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4581 2023-05-23 20:14:26.000000 wisdomweaver-0.3.0/wisdomweaver/document.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      108 2023-05-13 09:19:34.000000 wisdomweaver-0.3.0/wisdomweaver/models.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      987 2023-05-13 10:35:01.000000 wisdomweaver-0.3.0/wisdomweaver/postprocessor.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-23 21:49:20.496689 wisdomweaver-0.3.0/wisdomweaver.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1998 2023-05-23 21:49:20.000000 wisdomweaver-0.3.0/wisdomweaver.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      465 2023-05-23 21:49:20.000000 wisdomweaver-0.3.0/wisdomweaver.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-05-23 21:49:20.000000 wisdomweaver-0.3.0/wisdomweaver.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       54 2023-05-23 21:49:20.000000 wisdomweaver-0.3.0/wisdomweaver.egg-info/entry_points.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       54 2023-05-23 21:49:20.000000 wisdomweaver-0.3.0/wisdomweaver.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       13 2023-05-23 21:49:20.000000 wisdomweaver-0.3.0/wisdomweaver.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-25 16:15:04.138795 wisdomweaver-0.3.1/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      588 2023-05-23 16:20:38.000000 wisdomweaver-0.3.1/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1998 2023-05-25 16:15:04.138795 wisdomweaver-0.3.1/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      776 2023-05-23 21:34:57.000000 wisdomweaver-0.3.1/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1269 2023-05-25 16:13:24.000000 wisdomweaver-0.3.1/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-05-25 16:15:04.138795 wisdomweaver-0.3.1/setup.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)      266 2023-05-25 16:14:59.000000 wisdomweaver-0.3.1/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-25 16:15:04.138795 wisdomweaver-0.3.1/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1246 2023-05-25 16:04:31.000000 wisdomweaver-0.3.1/tests/test_database.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1118 2023-05-25 16:04:31.000000 wisdomweaver-0.3.1/tests/test_document.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-25 16:15:04.138795 wisdomweaver-0.3.1/wisdomweaver/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      241 2023-05-23 21:48:09.000000 wisdomweaver-0.3.1/wisdomweaver/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5716 2023-05-25 16:04:31.000000 wisdomweaver-0.3.1/wisdomweaver/__main__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1984 2023-05-23 18:49:00.000000 wisdomweaver-0.3.1/wisdomweaver/database.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4587 2023-05-25 16:04:31.000000 wisdomweaver-0.3.1/wisdomweaver/document.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      108 2023-05-13 09:19:34.000000 wisdomweaver-0.3.1/wisdomweaver/models.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      987 2023-05-13 10:35:01.000000 wisdomweaver-0.3.1/wisdomweaver/postprocessor.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-25 16:15:04.138795 wisdomweaver-0.3.1/wisdomweaver.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1998 2023-05-25 16:15:04.000000 wisdomweaver-0.3.1/wisdomweaver.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      458 2023-05-25 16:15:04.000000 wisdomweaver-0.3.1/wisdomweaver.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-05-25 16:15:04.000000 wisdomweaver-0.3.1/wisdomweaver.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       54 2023-05-25 16:15:04.000000 wisdomweaver-0.3.1/wisdomweaver.egg-info/entry_points.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      126 2023-05-25 16:15:04.000000 wisdomweaver-0.3.1/wisdomweaver.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       13 2023-05-25 16:15:04.000000 wisdomweaver-0.3.1/wisdomweaver.egg-info/top_level.txt
```

### Comparing `wisdomweaver-0.3.0/LICENSE` & `wisdomweaver-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wisdomweaver-0.3.0/PKG-INFO` & `wisdomweaver-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wisdomweaver
-Version: 0.3.0
+Version: 0.3.1
 Summary: Wisdom indexer and generator
 Author-email: Martin Schröder <info@swedishembedded.com>
 License: Copyright (C) 2023 Martin Schröder <info@swedishembedded.com>
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
         You may obtain a copy of the License at
```

### Comparing `wisdomweaver-0.3.0/README.md` & `wisdomweaver-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `wisdomweaver-0.3.0/pyproject.toml` & `wisdomweaver-0.3.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,60 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wisdomweaver"
-version = "0.3.0"
+version = "0.3.1"
 description = "Wisdom indexer and generator"
 readme = "README.md"
 authors = [{ name = "Martin Schröder", email = "info@swedishembedded.com" }]
 license = { file = "LICENSE" }
 classifiers = [
-    "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
+	"License :: OSI Approved :: Apache Software License",
+	"Programming Language :: Python",
+	"Programming Language :: Python :: 3",
 ]
 keywords = ["llm", "languagemodel", "indexing"]
 dependencies = [
-    "html2text",
+	"torch",
+	"pypdf",
+	"nltk",
+	"sentence_transformers",
+	"qdrant_client",
+	"openai",
+	"guidance",
+	"xformers",
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
-dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
+dev = [
+	"black",
+	"bumpversion",
+	"isort",
+	"pip-tools",
+	"pytest"
+]
 
 [project.urls]
 Homepage = "https://github.com/swedishembedded/wisdomweaver"
 
 [project.scripts]
 wisdom = "wisdomweaver.__main__:main"
 
 [tool.bumpver]
-current_version = "0.3.0"
+current_version = "0.3.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
-    'current_version = "{version}"',
-    'version = "{version}"',
+	'current_version = "{version}"',
+	'version = "{version}"',
 ]
 "wisdomweaver/__init__.py" = [
 	'__version__ = "{version}"',
 ]
```

### Comparing `wisdomweaver-0.3.0/tests/test_database.py` & `wisdomweaver-0.3.1/tests/test_database.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import textwrap
 
 sys.path.append("../")
 
-from database import Database  # noqa: E402
-from document import Document  # noqa: E402
+from wisdomweaver import Database  # noqa: E402
+from wisdomweaver import Document  # noqa: E402
 
 TEST_DATABASE = ".database-test"
 COLLECTION = "test-database"
 
 
 def test_database_can_return_similar_sentences():
     db = Database(TEST_DATABASE)
```

### Comparing `wisdomweaver-0.3.0/tests/test_document.py` & `wisdomweaver-0.3.1/tests/test_document.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Tests for the automator API
 """
 import sys
 import textwrap
 
 sys.path.append("../")
 
-from document import Document  # noqa: E402
+from wisdomweaver import Document  # noqa: E402
 
 
 def test_document_split_paragraphs_on_newlines():
     """
     Verify that splitting paragraphs works as i
     """
     text = """
```

### Comparing `wisdomweaver-0.3.0/wisdomweaver/database.py` & `wisdomweaver-0.3.1/wisdomweaver/database.py`

 * *Files identical despite different names*

### Comparing `wisdomweaver-0.3.0/wisdomweaver/document.py` & `wisdomweaver-0.3.1/wisdomweaver/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,22 +98,22 @@
         if path.suffix == ".pdf":
             with open(str(path), "rb") as file:
                 reader = pypdf.PdfReader(file)
                 pages = []
                 for page_num in range(len(reader.pages)):
                     pages.extend(reader.pages[page_num].extract_text())
                 self.add_text("\n".join(pages))
-        if path.suffix == ".rst":
+        elif path.suffix == ".rst":
             with open(str(path), "r") as file:
                 self.load_rst(str(file.read()))
-        if path.suffix == ".adoc":
+        elif path.suffix == ".adoc":
             with open(str(path), "r") as file:
                 self.add_text(str(file.read()))
         else:
-            raise Exception("Unknown file suffix %s" % (path.suffix))
+            raise Exception("Unknown file suffix '%s'" % (path.suffix))
 
     @property
     def paragraphs(self):
         """
         Returns paragraphs of the previously loaded document
         """
         return self.paragraph_list
```

### Comparing `wisdomweaver-0.3.0/wisdomweaver/postprocessor.py` & `wisdomweaver-0.3.1/wisdomweaver/postprocessor.py`

 * *Files identical despite different names*

### Comparing `wisdomweaver-0.3.0/wisdomweaver.egg-info/PKG-INFO` & `wisdomweaver-0.3.1/wisdomweaver.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wisdomweaver
-Version: 0.3.0
+Version: 0.3.1
 Summary: Wisdom indexer and generator
 Author-email: Martin Schröder <info@swedishembedded.com>
 License: Copyright (C) 2023 Martin Schröder <info@swedishembedded.com>
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
         You may obtain a copy of the License at
```

