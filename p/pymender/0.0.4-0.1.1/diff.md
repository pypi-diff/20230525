# Comparing `tmp/pymender-0.0.4.tar.gz` & `tmp/pymender-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymender-0.0.4.tar", last modified: Thu May 25 19:46:45 2023, max compression
+gzip compressed data, was "pymender-0.1.1.tar", last modified: Thu May 25 20:27:35 2023, max compression
```

## Comparing `pymender-0.0.4.tar` & `pymender-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:46:45.675695 pymender-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-25 19:46:45.671695 pymender-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-25 19:46:36.000000 pymender-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:46:45.671695 pymender-0.0.4/pymender/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:46:36.000000 pymender-0.0.4/pymender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 19:46:36.000000 pymender-0.0.4/pymender/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-25 19:46:36.000000 pymender-0.0.4/pymender/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:46:45.671695 pymender-0.0.4/pymender/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:46:36.000000 pymender-0.0.4/pymender/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-25 19:46:36.000000 pymender-0.0.4/pymender/commands/fastapi_annotated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:46:45.671695 pymender-0.0.4/pymender/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:46:36.000000 pymender-0.0.4/pymender/commands/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-25 19:46:36.000000 pymender-0.0.4/pymender/commands/tests/test_fastapi_annotated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:46:45.671695 pymender-0.0.4/pymender.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-25 19:46:45.000000 pymender-0.0.4/pymender.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-25 19:46:45.000000 pymender-0.0.4/pymender.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:46:45.000000 pymender-0.0.4/pymender.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 19:46:45.000000 pymender-0.0.4/pymender.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 19:46:45.000000 pymender-0.0.4/pymender.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 19:46:45.000000 pymender-0.0.4/pymender.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-25 19:46:36.000000 pymender-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 19:46:36.000000 pymender-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 19:46:45.675695 pymender-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:35.630068 pymender-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-25 20:27:35.630068 pymender-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-25 20:27:26.000000 pymender-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:35.626067 pymender-0.1.1/pymender/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:26.000000 pymender-0.1.1/pymender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 20:27:26.000000 pymender-0.1.1/pymender/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-25 20:27:26.000000 pymender-0.1.1/pymender/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:35.630068 pymender-0.1.1/pymender/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:26.000000 pymender-0.1.1/pymender/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-25 20:27:26.000000 pymender-0.1.1/pymender/commands/fastapi_annotated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:35.630068 pymender-0.1.1/pymender/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:26.000000 pymender-0.1.1/pymender/commands/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-25 20:27:26.000000 pymender-0.1.1/pymender/commands/tests/test_fastapi_annotated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:35.630068 pymender-0.1.1/pymender.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-25 20:27:35.000000 pymender-0.1.1/pymender.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-25 20:27:35.000000 pymender-0.1.1/pymender.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:27:35.000000 pymender-0.1.1/pymender.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 20:27:35.000000 pymender-0.1.1/pymender.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 20:27:35.000000 pymender-0.1.1/pymender.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 20:27:35.000000 pymender-0.1.1/pymender.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-25 20:27:26.000000 pymender-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 20:27:26.000000 pymender-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 20:27:35.630068 pymender-0.1.1/setup.cfg
```

### Comparing `pymender-0.0.4/pymender/cli.py` & `pymender-0.1.1/pymender/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,19 @@
     context = CodemodContext()
     command_instance = Command(context)
     files = gather_files(args.path)
     
     gitignore_path = Path(args.gitignore) if args.gitignore else Path(repo_root) / ".gitignore"
     if gitignore_path.exists() and (validator := parse_gitignore(gitignore_path)):
         files = [file for file in files if not validator(file)]
-        
+    
+    if not files:
+        print("No files to modify! Check if you need to adjust the .gitignore", file=sys.stderr)
+        return 1
+    
     try:
         result = parallel_exec_transform_with_prettyprint(
             command_instance, files, repo_root=repo_root,
         )
     except KeyboardInterrupt:
         print("Interrupted!", file=sys.stderr)
         return 2
@@ -88,15 +92,15 @@
     parser = argparse.ArgumentParser(
         description="Mends Python code to be more idiomatic."
     )
     parser.add_argument(
         "command",
         metavar="COMMAND",
         choices=command_lookup.keys(),
-        help="The codemod to run.",
+        help=f"The codemod to run, choose from: {', '.join(command_lookup.keys())}}",
     )
     args, _ = parser.parse_known_args()
     
     Command = command_lookup.get(args.command)
     if not Command:
         print(f"Unknown command {args.command}", file=sys.stderr)
         return 1
```

### Comparing `pymender-0.0.4/pymender/commands/fastapi_annotated.py` & `pymender-0.1.1/pymender/commands/fastapi_annotated.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,17 +41,14 @@
             return wrap_subscript_elements_with_annotated(param, elements, None)
         case cst.Call(func=cst.Name("Body")) | cst.Call(func=cst.Name("Query")):
             logger.info(f"Found Body annotation")
 
             call = param.default
 
             # Find the default value (either first unnamed argument or default=)
-            # breakpoint()
-
-            # First unnamed argument, that is not Ellipsis
             first_unnamed_arg = next(
                 (arg for arg in call.args if arg.keyword is None),
                 None,
             )
             default_keyword = next(
                 (
                     arg
@@ -67,19 +64,23 @@
                     args=[arg for arg in call.args if arg != default]
                 )
 
             elements = [
                 param.annotation.annotation if param.annotation is not None else None,
                 call,
             ]
+            
+            def should_be_included_as_default(default: cst.BaseExpression) -> bool:
+                return default and not isinstance(default.value, cst.Ellipsis)
+            
             return wrap_subscript_elements_with_annotated(
                 param,
                 elements,
                 default.value
-                if default and not isinstance(default.value, cst.Ellipsis)
+                if should_be_included_as_default(default)
                 else None,
             )
 
         case _:
             return None
```

### Comparing `pymender-0.0.4/pymender/commands/tests/test_fastapi_annotated.py` & `pymender-0.1.1/pymender/commands/tests/test_fastapi_annotated.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,32 +6,34 @@
 
 @router.get('/example')
 def example_function(
     value: int,
     query: str = Query("foo"),
     zar: str = Query(default="bar", alias="z"),
     foo: str = Depends(get_foo),
+    *,
     bar: str = Depends(get_bar),
     body: str = Body(...),
 ) -> str:
     return 'example'
     
 """
 
 EXAMPLE_FUNCTION_WITH_ANNOTATED = """
 from typing import Annotated
 
 @router.get('/example')
 def example_function(
     value: int,
     foo: Annotated[str, Depends(get_foo)],
-    bar: Annotated[str, Depends(get_bar)],
-    body: Annotated[str, Body()],
     query: Annotated[str, Query()] = "foo",
     zar: Annotated[str, Query(alias="z")] = "bar",
+    *,
+    bar: Annotated[str, Depends(get_bar)],
+    body: Annotated[str, Body()],
 ) -> str:
     return 'example'
 
 """
 
 EXAMPLE_ASYNC_FUNCTION = """
 @contacts_enrich_industry_router.post(
```

### Comparing `pymender-0.0.4/pyproject.toml` & `pymender-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 [project]
 name = "pymender"
-version = "0.0.4"
+version = "0.1.1"
+authors = [
+    { name="Daniel Hails", email="pymender@hails.info" },
+]
+description = "Mend your Python projects with reproducible refactors"
+requires-python = ">=3.10"
 dynamic = ["dependencies", "readme"]
 
+[project.urls]
+"Homepage" = "https://github.com/DJRHails/pymender"
+"Bug Tracker" = "https://github.com/DJRHails/pymender/issues"
+
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 readme = {file = ["README.md"], content-type = "text/markdown"}
@@ -15,15 +24,15 @@
 find = {}  # Scan the project directory with the default parameters
 
 
 [project.scripts]
 pymender = "pymender.cli:main"
 
 [tool.bumpver]
-current_version = "0.0.4"
+current_version = "0.1.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

