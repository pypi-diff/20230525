# Comparing `tmp/pymender-0.1.1.tar.gz` & `tmp/pymender-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymender-0.1.1.tar", last modified: Thu May 25 20:27:35 2023, max compression
+gzip compressed data, was "pymender-0.1.2.tar", last modified: Thu May 25 21:29:32 2023, max compression
```

## Comparing `pymender-0.1.1.tar` & `pymender-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:35.630068 pymender-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-25 20:27:35.630068 pymender-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-25 20:27:26.000000 pymender-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:35.626067 pymender-0.1.1/pymender/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:26.000000 pymender-0.1.1/pymender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 20:27:26.000000 pymender-0.1.1/pymender/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-25 20:27:26.000000 pymender-0.1.1/pymender/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:35.630068 pymender-0.1.1/pymender/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:26.000000 pymender-0.1.1/pymender/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-25 20:27:26.000000 pymender-0.1.1/pymender/commands/fastapi_annotated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:35.630068 pymender-0.1.1/pymender/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:26.000000 pymender-0.1.1/pymender/commands/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-25 20:27:26.000000 pymender-0.1.1/pymender/commands/tests/test_fastapi_annotated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:27:35.630068 pymender-0.1.1/pymender.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-25 20:27:35.000000 pymender-0.1.1/pymender.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-25 20:27:35.000000 pymender-0.1.1/pymender.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:27:35.000000 pymender-0.1.1/pymender.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 20:27:35.000000 pymender-0.1.1/pymender.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 20:27:35.000000 pymender-0.1.1/pymender.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 20:27:35.000000 pymender-0.1.1/pymender.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-25 20:27:26.000000 pymender-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 20:27:26.000000 pymender-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 20:27:35.630068 pymender-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:29:32.404159 pymender-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-25 21:29:32.404159 pymender-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-25 21:29:22.000000 pymender-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:29:32.400159 pymender-0.1.2/pymender/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 21:29:22.000000 pymender-0.1.2/pymender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 21:29:22.000000 pymender-0.1.2/pymender/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-25 21:29:22.000000 pymender-0.1.2/pymender/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:29:32.400159 pymender-0.1.2/pymender/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 21:29:22.000000 pymender-0.1.2/pymender/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-25 21:29:22.000000 pymender-0.1.2/pymender/commands/fastapi_annotated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:29:32.404159 pymender-0.1.2/pymender/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 21:29:22.000000 pymender-0.1.2/pymender/commands/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-25 21:29:22.000000 pymender-0.1.2/pymender/commands/tests/test_fastapi_annotated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:29:32.400159 pymender-0.1.2/pymender.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-25 21:29:32.000000 pymender-0.1.2/pymender.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-25 21:29:32.000000 pymender-0.1.2/pymender.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:29:32.000000 pymender-0.1.2/pymender.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 21:29:32.000000 pymender-0.1.2/pymender.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 21:29:32.000000 pymender-0.1.2/pymender.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 21:29:32.000000 pymender-0.1.2/pymender.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-25 21:29:22.000000 pymender-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 21:29:22.000000 pymender-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 21:29:32.404159 pymender-0.1.2/setup.cfg
```

### Comparing `pymender-0.1.1/PKG-INFO` & `pymender-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: pymender
-Version: 0.1.1
+Version: 0.1.2
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
-pip install pymender==0.1.1
+pip install pymender==0.1.2
 
 pymender <codemod> <path_to_project>
 ```
 
 ## What codemods are available?
 
-### `FastAPIAnnotated`
+### ⚡ `FastAPIAnnotated`
 
 Converts FastAPI endpoints to use the preferred `Annotated[<type>, Depends(<dependency>)]` syntax rather than `: <type> = Depends(<dependency>)`.
 
 **Why?**
 
 - *Default* value of the function parameter is the *actual default* value.
 - *Reuse* of the function is now possible.
 - *Type-safe* usage of the functions, previously 'default' values where not type checked.
 - *Multi-purpose* e.g. `Annotated[str, fastapi.Query(), typer.Argument()]` is now possible.
 
 ```bash
-pymender FastAPIAnnotated .
+pymender FastAPIAnnotated <folder-to-upgrade>
 ```
 
 | Before | After |
 | --- | --- |
 | <pre>@router.get('/example')<br/>def example_function(<br/>    value: int,<br/>    query: str = Query("foo"),<br/>    zar: str = Query(default="bar", alias="z"),<br/>    foo: str = Depends(get_foo),<br/>    *,<br/>    bar: str = Depends(get_bar),<br/>    body: str = Body(...),<br/>) -> str:<br/>    return 'example'</pre> | <pre>@router.get('/example')<br/>def example_function(<br/>    value: int,<br/>    foo: Annotated[str, Depends(get_foo)],<br/>    query: Annotated[str, Query()] = "foo",<br/>    zar: Annotated[str, Query(alias="z")] = "bar",<br/>    *,<br/>    bar: Annotated[str, Depends(get_bar)],<br/>    body: Annotated[str, Body()],<br/>) -> str:<br/>    return 'example'</pre> |
 
 ## Developer Guide
```

### Comparing `pymender-0.1.1/README.md` & `pymender-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # 👷‍♀️ PyMender
 
 Perform entire codebase refactors in a way that is _reproducible_, _testable_ and _reviewable_. Obeys `.gitignore` by default.
 
 ## Usage
 
 ```bash
-pip install pymender==0.1.1
+pip install pymender==0.1.2
 
 pymender <codemod> <path_to_project>
 ```
 
 ## What codemods are available?
 
-### `FastAPIAnnotated`
+### ⚡ `FastAPIAnnotated`
 
 Converts FastAPI endpoints to use the preferred `Annotated[<type>, Depends(<dependency>)]` syntax rather than `: <type> = Depends(<dependency>)`.
 
 **Why?**
 
 - *Default* value of the function parameter is the *actual default* value.
 - *Reuse* of the function is now possible.
 - *Type-safe* usage of the functions, previously 'default' values where not type checked.
 - *Multi-purpose* e.g. `Annotated[str, fastapi.Query(), typer.Argument()]` is now possible.
 
 ```bash
-pymender FastAPIAnnotated .
+pymender FastAPIAnnotated <folder-to-upgrade>
 ```
 
 | Before | After |
 | --- | --- |
 | <pre>@router.get('/example')<br/>def example_function(<br/>    value: int,<br/>    query: str = Query("foo"),<br/>    zar: str = Query(default="bar", alias="z"),<br/>    foo: str = Depends(get_foo),<br/>    *,<br/>    bar: str = Depends(get_bar),<br/>    body: str = Body(...),<br/>) -> str:<br/>    return 'example'</pre> | <pre>@router.get('/example')<br/>def example_function(<br/>    value: int,<br/>    foo: Annotated[str, Depends(get_foo)],<br/>    query: Annotated[str, Query()] = "foo",<br/>    zar: Annotated[str, Query(alias="z")] = "bar",<br/>    *,<br/>    bar: Annotated[str, Depends(get_bar)],<br/>    body: Annotated[str, Body()],<br/>) -> str:<br/>    return 'example'</pre> |
 
 ## Developer Guide
@@ -46,8 +46,8 @@
 pytest -vv
 
 ```
 
 ## Thanks to:
 
 - [libCST](https://github.com/Instagram/LibCST) which does a lot of the hardwork for this.
-- [autotyping](https://github.com/JelleZijlstra/autotyping) for showing what was possible.
+- [autotyping](https://github.com/JelleZijlstra/autotyping) for showing what was possible.
```

### Comparing `pymender-0.1.1/pymender/cli.py` & `pymender-0.1.2/pymender/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     parser = argparse.ArgumentParser(
         description="Mends Python code to be more idiomatic."
     )
     parser.add_argument(
         "command",
         metavar="COMMAND",
         choices=command_lookup.keys(),
-        help=f"The codemod to run, choose from: {', '.join(command_lookup.keys())}}",
+        help=f"The codemod to run, choose from: {', '.join(command_lookup.keys())}",
     )
     args, _ = parser.parse_known_args()
     
     Command = command_lookup.get(args.command)
     if not Command:
         print(f"Unknown command {args.command}", file=sys.stderr)
         return 1
```

### Comparing `pymender-0.1.1/pymender/commands/fastapi_annotated.py` & `pymender-0.1.2/pymender/commands/fastapi_annotated.py`

 * *Files identical despite different names*

### Comparing `pymender-0.1.1/pymender/commands/tests/test_fastapi_annotated.py` & `pymender-0.1.2/pymender/commands/tests/test_fastapi_annotated.py`

 * *Files identical despite different names*

### Comparing `pymender-0.1.1/pymender.egg-info/PKG-INFO` & `pymender-0.1.2/pymender.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: pymender
-Version: 0.1.1
+Version: 0.1.2
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
-pip install pymender==0.1.1
+pip install pymender==0.1.2
 
 pymender <codemod> <path_to_project>
 ```
 
 ## What codemods are available?
 
-### `FastAPIAnnotated`
+### ⚡ `FastAPIAnnotated`
 
 Converts FastAPI endpoints to use the preferred `Annotated[<type>, Depends(<dependency>)]` syntax rather than `: <type> = Depends(<dependency>)`.
 
 **Why?**
 
 - *Default* value of the function parameter is the *actual default* value.
 - *Reuse* of the function is now possible.
 - *Type-safe* usage of the functions, previously 'default' values where not type checked.
 - *Multi-purpose* e.g. `Annotated[str, fastapi.Query(), typer.Argument()]` is now possible.
 
 ```bash
-pymender FastAPIAnnotated .
+pymender FastAPIAnnotated <folder-to-upgrade>
 ```
 
 | Before | After |
 | --- | --- |
 | <pre>@router.get('/example')<br/>def example_function(<br/>    value: int,<br/>    query: str = Query("foo"),<br/>    zar: str = Query(default="bar", alias="z"),<br/>    foo: str = Depends(get_foo),<br/>    *,<br/>    bar: str = Depends(get_bar),<br/>    body: str = Body(...),<br/>) -> str:<br/>    return 'example'</pre> | <pre>@router.get('/example')<br/>def example_function(<br/>    value: int,<br/>    foo: Annotated[str, Depends(get_foo)],<br/>    query: Annotated[str, Query()] = "foo",<br/>    zar: Annotated[str, Query(alias="z")] = "bar",<br/>    *,<br/>    bar: Annotated[str, Depends(get_bar)],<br/>    body: Annotated[str, Body()],<br/>) -> str:<br/>    return 'example'</pre> |
 
 ## Developer Guide
```

### Comparing `pymender-0.1.1/pyproject.toml` & `pymender-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pymender"
-version = "0.1.1"
+version = "0.1.2"
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
-current_version = "0.1.1"
+current_version = "0.1.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

