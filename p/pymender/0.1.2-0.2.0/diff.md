# Comparing `tmp/pymender-0.1.2.tar.gz` & `tmp/pymender-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymender-0.1.2.tar", last modified: Thu May 25 21:29:32 2023, max compression
+gzip compressed data, was "pymender-0.2.0.tar", last modified: Thu May 25 21:35:35 2023, max compression
```

## Comparing `pymender-0.1.2.tar` & `pymender-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:29:32.404159 pymender-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-25 21:29:32.404159 pymender-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-25 21:29:22.000000 pymender-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:29:32.400159 pymender-0.1.2/pymender/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 21:29:22.000000 pymender-0.1.2/pymender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 21:29:22.000000 pymender-0.1.2/pymender/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-25 21:29:22.000000 pymender-0.1.2/pymender/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:29:32.400159 pymender-0.1.2/pymender/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 21:29:22.000000 pymender-0.1.2/pymender/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-25 21:29:22.000000 pymender-0.1.2/pymender/commands/fastapi_annotated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:29:32.404159 pymender-0.1.2/pymender/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 21:29:22.000000 pymender-0.1.2/pymender/commands/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-25 21:29:22.000000 pymender-0.1.2/pymender/commands/tests/test_fastapi_annotated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:29:32.400159 pymender-0.1.2/pymender.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-25 21:29:32.000000 pymender-0.1.2/pymender.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-25 21:29:32.000000 pymender-0.1.2/pymender.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:29:32.000000 pymender-0.1.2/pymender.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 21:29:32.000000 pymender-0.1.2/pymender.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 21:29:32.000000 pymender-0.1.2/pymender.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 21:29:32.000000 pymender-0.1.2/pymender.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-25 21:29:22.000000 pymender-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 21:29:22.000000 pymender-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 21:29:32.404159 pymender-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:35:35.640883 pymender-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-25 21:35:35.640883 pymender-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-25 21:35:25.000000 pymender-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:35:35.640883 pymender-0.2.0/pymender/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 21:35:25.000000 pymender-0.2.0/pymender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 21:35:25.000000 pymender-0.2.0/pymender/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-25 21:35:25.000000 pymender-0.2.0/pymender/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:35:35.640883 pymender-0.2.0/pymender/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 21:35:25.000000 pymender-0.2.0/pymender/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-25 21:35:25.000000 pymender-0.2.0/pymender/commands/fastapi_annotated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:35:35.640883 pymender-0.2.0/pymender/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 21:35:25.000000 pymender-0.2.0/pymender/commands/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-25 21:35:25.000000 pymender-0.2.0/pymender/commands/tests/test_fastapi_annotated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:35:35.640883 pymender-0.2.0/pymender.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-25 21:35:35.000000 pymender-0.2.0/pymender.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-25 21:35:35.000000 pymender-0.2.0/pymender.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:35:35.000000 pymender-0.2.0/pymender.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 21:35:35.000000 pymender-0.2.0/pymender.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 21:35:35.000000 pymender-0.2.0/pymender.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 21:35:35.000000 pymender-0.2.0/pymender.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-25 21:35:25.000000 pymender-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 21:35:25.000000 pymender-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 21:35:35.640883 pymender-0.2.0/setup.cfg
```

### Comparing `pymender-0.1.2/PKG-INFO` & `pymender-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pymender
-Version: 0.1.2
+Version: 0.2.0
 Summary: Mend your Python projects with reproducible refactors
 Author-email: Daniel Hails <pymender@hails.info>
 Project-URL: Homepage, https://github.com/DJRHails/pymender
 Project-URL: Bug Tracker, https://github.com/DJRHails/pymender/issues
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # 👷‍♀️ PyMender
 
 Perform entire codebase refactors in a way that is _reproducible_, _testable_ and _reviewable_. Obeys `.gitignore` by default.
 
 ## Usage
 
 ```bash
-pip install pymender==0.1.2
+pip install pymender==0.2.0
 
 pymender <codemod> <path_to_project>
 ```
 
 ## What codemods are available?
 
 ### ⚡ `FastAPIAnnotated`
```

### Comparing `pymender-0.1.2/README.md` & `pymender-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # 👷‍♀️ PyMender
 
 Perform entire codebase refactors in a way that is _reproducible_, _testable_ and _reviewable_. Obeys `.gitignore` by default.
 
 ## Usage
 
 ```bash
-pip install pymender==0.1.2
+pip install pymender==0.2.0
 
 pymender <codemod> <path_to_project>
 ```
 
 ## What codemods are available?
 
 ### ⚡ `FastAPIAnnotated`
```

### Comparing `pymender-0.1.2/pymender/cli.py` & `pymender-0.2.0/pymender/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 
 def run_command(Command: type[CodemodCommand], repo_root: str = ".") -> int:
     os.environ["LIBCST_PARSER_TYPE"] = "native"
     parser = argparse.ArgumentParser(
         description=Command.DESCRIPTION,
     )
     parser.add_argument(
+        "command",
+        metavar="COMMAND",
+    )
+    parser.add_argument(
         "path",
         metavar="PATH",
         nargs="+",
         help=(
             "Path to codemod. Can be a directory, file, or multiple of either. To "
             + 'instead read from stdin and write to stdout, use "-"'
         ),
@@ -39,18 +43,22 @@
         ),   
     )
     args = parser.parse_args()
 
     context = CodemodContext()
     command_instance = Command(context)
     files = gather_files(args.path)
+    print(f"Found {len(files)} files in {args.path}", file=sys.stderr)
     
     gitignore_path = Path(args.gitignore) if args.gitignore else Path(repo_root) / ".gitignore"
+    
     if gitignore_path.exists() and (validator := parse_gitignore(gitignore_path)):
+        print(f"Filtering files through '{gitignore_path}'...", file=sys.stderr)
         files = [file for file in files if not validator(file)]
+        print(f"Found {len(files)} files after filtering", file=sys.stderr)
     
     if not files:
         print("No files to modify! Check if you need to adjust the .gitignore", file=sys.stderr)
         return 1
     
     try:
         result = parallel_exec_transform_with_prettyprint(
```

### Comparing `pymender-0.1.2/pymender/commands/fastapi_annotated.py` & `pymender-0.2.0/pymender/commands/fastapi_annotated.py`

 * *Files identical despite different names*

### Comparing `pymender-0.1.2/pymender/commands/tests/test_fastapi_annotated.py` & `pymender-0.2.0/pymender/commands/tests/test_fastapi_annotated.py`

 * *Files identical despite different names*

### Comparing `pymender-0.1.2/pymender.egg-info/PKG-INFO` & `pymender-0.2.0/pymender.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pymender
-Version: 0.1.2
+Version: 0.2.0
 Summary: Mend your Python projects with reproducible refactors
 Author-email: Daniel Hails <pymender@hails.info>
 Project-URL: Homepage, https://github.com/DJRHails/pymender
 Project-URL: Bug Tracker, https://github.com/DJRHails/pymender/issues
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # 👷‍♀️ PyMender
 
 Perform entire codebase refactors in a way that is _reproducible_, _testable_ and _reviewable_. Obeys `.gitignore` by default.
 
 ## Usage
 
 ```bash
-pip install pymender==0.1.2
+pip install pymender==0.2.0
 
 pymender <codemod> <path_to_project>
 ```
 
 ## What codemods are available?
 
 ### ⚡ `FastAPIAnnotated`
```

### Comparing `pymender-0.1.2/pyproject.toml` & `pymender-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pymender"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
     { name="Daniel Hails", email="pymender@hails.info" },
 ]
 description = "Mend your Python projects with reproducible refactors"
 requires-python = ">=3.10"
 dynamic = ["dependencies", "readme"]
 
@@ -24,15 +24,15 @@
 find = {}  # Scan the project directory with the default parameters
 
 
 [project.scripts]
 pymender = "pymender.cli:main"
 
 [tool.bumpver]
-current_version = "0.1.2"
+current_version = "0.2.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

