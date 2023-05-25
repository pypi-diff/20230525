# Comparing `tmp/mypy-boto3-codepipeline-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-codepipeline-1.26.141.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codepipeline-1.26.0.post1.tar", last modified: Tue Nov  1 21:43:14 2022, max compression
+gzip compressed data, was "mypy-boto3-codepipeline-1.26.141.tar", last modified: Thu May 25 19:32:48 2023, max compression
```

## Comparing `mypy-boto3-codepipeline-1.26.0.post1.tar` & `mypy-boto3-codepipeline-1.26.141.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:14.152817 mypy-boto3-codepipeline-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:31:57.000000 mypy-boto3-codepipeline-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    19123 2022-11-01 21:43:14.152817 mypy-boto3-codepipeline-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    17662 2022-11-01 21:31:57.000000 mypy-boto3-codepipeline-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:14.152817 mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/
--rw-r--r--   0 runner    (1001) docker     (121)     1704 2022-11-01 21:31:57.000000 mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1703 2022-11-01 21:31:57.000000 mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      937 2022-11-01 21:31:57.000000 mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    32275 2022-11-01 21:31:57.000000 mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    32223 2022-11-01 21:31:57.000000 mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10004 2022-11-01 21:31:57.000000 mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)    10002 2022-11-01 21:31:57.000000 mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7606 2022-11-01 21:31:57.000000 mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     7598 2022-11-01 21:31:57.000000 mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:31:57.000000 mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    46140 2022-11-01 21:31:58.000000 mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    46079 2022-11-01 21:31:58.000000 mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:31:57.000000 mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:43:14.152817 mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    19123 2022-11-01 21:43:13.000000 mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-11-01 21:43:13.000000 mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:13.000000 mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:43:13.000000 mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:43:13.000000 mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-11-01 21:43:13.000000 mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:43:14.152817 mypy-boto3-codepipeline-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2003 2022-11-01 21:31:57.000000 mypy-boto3-codepipeline-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:32:48.408743 mypy-boto3-codepipeline-1.26.141/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-25 19:31:53.000000 mypy-boto3-codepipeline-1.26.141/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19156 2023-05-25 19:32:48.408743 mypy-boto3-codepipeline-1.26.141/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17647 2023-05-25 19:31:53.000000 mypy-boto3-codepipeline-1.26.141/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:32:48.408743 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-25 19:31:53.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-25 19:31:53.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-25 19:31:53.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32307 2023-05-25 19:31:54.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32255 2023-05-25 19:31:54.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-05-25 19:31:54.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-05-25 19:31:54.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-05-25 19:31:54.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-05-25 19:31:54.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:31:53.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46179 2023-05-25 19:31:55.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46118 2023-05-25 19:31:54.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-25 19:31:53.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:32:48.408743 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19156 2023-05-25 19:32:48.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-25 19:32:48.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:32:48.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:32:48.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 19:32:48.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 19:32:48.000000 mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 19:32:48.408743 mypy-boto3-codepipeline-1.26.141/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-25 19:31:53.000000 mypy-boto3-codepipeline-1.26.141/setup.py
```

### Comparing `mypy-boto3-codepipeline-1.26.0.post1/LICENSE` & `mypy-boto3-codepipeline-1.26.141/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-codepipeline-1.26.0.post1/PKG-INFO` & `mypy-boto3-codepipeline-1.26.141/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codepipeline
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CodePipeline 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.141
+Summary: Type annotations for boto3.CodePipeline 1.26.141 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-codepipeline"></a>
 
 # mypy-boto3-codepipeline
 
 [![PyPI - mypy-boto3-codepipeline](https://img.shields.io/pypi/v/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codepipeline?color=blue)](https://pypistats.org/packages/mypy-boto3-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodePipeline 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[boto3.CodePipeline 1.26.141](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codepipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/).
 
 See how it helps to find and fix potential bugs:
 
@@ -514,42 +515,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-codepipeline-1.26.0.post1/README.md` & `mypy-boto3-codepipeline-1.26.141/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codepipeline"></a>
 
 # mypy-boto3-codepipeline
 
 [![PyPI - mypy-boto3-codepipeline](https://img.shields.io/pypi/v/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codepipeline?color=blue)](https://pypistats.org/packages/mypy-boto3-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodePipeline 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[boto3.CodePipeline 1.26.141](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codepipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/).
 
 See how it helps to find and fix potential bugs:
 
@@ -483,42 +483,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/__init__.py` & `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/__init__.pyi` & `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/client.py` & `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         outputArtifactDetails: ArtifactDetailsTypeDef,
         settings: ActionTypeSettingsTypeDef = ...,
         configurationProperties: Sequence[ActionConfigurationPropertyTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateCustomActionTypeOutputTypeDef:
         """
         Creates a new custom action that can be used in all pipelines associated with
-        the AWS account.
+        the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.create_custom_action_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#create_custom_action_type)
         """
 
     def create_pipeline(
         self, *, pipeline: PipelineDeclarationTypeDef, tags: Sequence[TagTypeDef] = ...
@@ -362,16 +362,15 @@
         self,
         *,
         actionOwnerFilter: ActionOwnerType = ...,
         nextToken: str = ...,
         regionFilter: str = ...
     ) -> ListActionTypesOutputTypeDef:
         """
-        Gets a summary of all AWS CodePipeline action types associated with your
-        account.
+        Gets a summary of all CodePipeline action types associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.list_action_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#list_action_types)
         """
 
     def list_pipeline_executions(
         self, *, pipelineName: str, maxResults: int = ..., nextToken: str = ...
@@ -403,29 +402,30 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#list_tags_for_resource)
         """
 
     def list_webhooks(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListWebhooksOutputTypeDef:
         """
-        Gets a listing of all the webhooks in this AWS Region for this account.
+        Gets a listing of all the webhooks in this Amazon Web Services Region for this
+        account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.list_webhooks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#list_webhooks)
         """
 
     def poll_for_jobs(
         self,
         *,
         actionTypeId: ActionTypeIdTypeDef,
         maxBatchSize: int = ...,
         queryParam: Mapping[str, str] = ...
     ) -> PollForJobsOutputTypeDef:
         """
-        Returns information about any jobs for AWS CodePipeline to act on.
+        Returns information about any jobs for CodePipeline to act on.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.poll_for_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#poll_for_jobs)
         """
 
     def poll_for_third_party_jobs(
         self, *, actionTypeId: ActionTypeIdTypeDef, maxBatchSize: int = ...
@@ -442,15 +442,15 @@
         *,
         pipelineName: str,
         stageName: str,
         actionName: str,
         actionRevision: ActionRevisionTypeDef
     ) -> PutActionRevisionOutputTypeDef:
         """
-        Provides information to AWS CodePipeline about new revisions to a source.
+        Provides information to CodePipeline about new revisions to a source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_action_revision)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#put_action_revision)
         """
 
     def put_approval_result(
         self,
@@ -458,15 +458,15 @@
         pipelineName: str,
         stageName: str,
         actionName: str,
         result: ApprovalResultTypeDef,
         token: str
     ) -> PutApprovalResultOutputTypeDef:
         """
-        Provides the response to a manual approval request to AWS CodePipeline.
+        Provides the response to a manual approval request to CodePipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_approval_result)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#put_approval_result)
         """
 
     def put_job_failure_result(
         self, *, jobId: str, failureDetails: FailureDetailsTypeDef
@@ -582,15 +582,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#tag_resource)
         """
 
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        Removes tags from an AWS resource.
+        Removes tags from an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#untag_resource)
         """
 
     def update_action_type(
         self, *, actionType: ActionTypeDeclarationTypeDef
```

### Comparing `mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/client.pyi` & `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         outputArtifactDetails: ArtifactDetailsTypeDef,
         settings: ActionTypeSettingsTypeDef = ...,
         configurationProperties: Sequence[ActionConfigurationPropertyTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateCustomActionTypeOutputTypeDef:
         """
         Creates a new custom action that can be used in all pipelines associated with
-        the AWS account.
+        the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.create_custom_action_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#create_custom_action_type)
         """
     def create_pipeline(
         self, *, pipeline: PipelineDeclarationTypeDef, tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineOutputTypeDef:
@@ -337,16 +337,15 @@
         self,
         *,
         actionOwnerFilter: ActionOwnerType = ...,
         nextToken: str = ...,
         regionFilter: str = ...
     ) -> ListActionTypesOutputTypeDef:
         """
-        Gets a summary of all AWS CodePipeline action types associated with your
-        account.
+        Gets a summary of all CodePipeline action types associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.list_action_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#list_action_types)
         """
     def list_pipeline_executions(
         self, *, pipelineName: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListPipelineExecutionsOutputTypeDef:
@@ -374,28 +373,29 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#list_tags_for_resource)
         """
     def list_webhooks(
         self, *, NextToken: str = ..., MaxResults: int = ...
     ) -> ListWebhooksOutputTypeDef:
         """
-        Gets a listing of all the webhooks in this AWS Region for this account.
+        Gets a listing of all the webhooks in this Amazon Web Services Region for this
+        account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.list_webhooks)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#list_webhooks)
         """
     def poll_for_jobs(
         self,
         *,
         actionTypeId: ActionTypeIdTypeDef,
         maxBatchSize: int = ...,
         queryParam: Mapping[str, str] = ...
     ) -> PollForJobsOutputTypeDef:
         """
-        Returns information about any jobs for AWS CodePipeline to act on.
+        Returns information about any jobs for CodePipeline to act on.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.poll_for_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#poll_for_jobs)
         """
     def poll_for_third_party_jobs(
         self, *, actionTypeId: ActionTypeIdTypeDef, maxBatchSize: int = ...
     ) -> PollForThirdPartyJobsOutputTypeDef:
@@ -410,30 +410,30 @@
         *,
         pipelineName: str,
         stageName: str,
         actionName: str,
         actionRevision: ActionRevisionTypeDef
     ) -> PutActionRevisionOutputTypeDef:
         """
-        Provides information to AWS CodePipeline about new revisions to a source.
+        Provides information to CodePipeline about new revisions to a source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_action_revision)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#put_action_revision)
         """
     def put_approval_result(
         self,
         *,
         pipelineName: str,
         stageName: str,
         actionName: str,
         result: ApprovalResultTypeDef,
         token: str
     ) -> PutApprovalResultOutputTypeDef:
         """
-        Provides the response to a manual approval request to AWS CodePipeline.
+        Provides the response to a manual approval request to CodePipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_approval_result)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#put_approval_result)
         """
     def put_job_failure_result(
         self, *, jobId: str, failureDetails: FailureDetailsTypeDef
     ) -> EmptyResponseMetadataTypeDef:
@@ -538,15 +538,15 @@
         Adds to or modifies the tags of the given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#tag_resource)
         """
     def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        Removes tags from an AWS resource.
+        Removes tags from an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/client/#untag_resource)
         """
     def update_action_type(
         self, *, actionType: ActionTypeDeclarationTypeDef
     ) -> EmptyResponseMetadataTypeDef:
```

### Comparing `mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/literals.py` & `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,14 +117,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -134,27 +135,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -183,14 +188,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -235,51 +241,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -292,14 +304,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -311,28 +324,33 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -341,14 +359,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -359,55 +378,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -434,26 +461,29 @@
     "list_action_types",
     "list_pipeline_executions",
     "list_pipelines",
     "list_tags_for_resource",
     "list_webhooks",
 ]
 RegionName = Literal[
+    "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/literals.pyi` & `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -132,27 +133,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -181,14 +186,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -233,51 +239,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -290,14 +302,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -309,28 +322,33 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -339,14 +357,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -357,55 +376,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -432,26 +459,29 @@
     "list_action_types",
     "list_pipeline_executions",
     "list_pipelines",
     "list_tags_for_resource",
     "list_webhooks",
 ]
 RegionName = Literal[
+    "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/paginator.py` & `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/paginator.pyi` & `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/type_defs.py` & `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -641,14 +641,15 @@
 
 PipelineMetadataTypeDef = TypedDict(
     "PipelineMetadataTypeDef",
     {
         "pipelineArn": str,
         "created": datetime,
         "updated": datetime,
+        "pollingDisabledAt": datetime,
     },
     total=False,
 )
 
 GetPipelineStateInputRequestTypeDef = TypedDict(
     "GetPipelineStateInputRequestTypeDef",
     {
```

### Comparing `mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline/type_defs.pyi` & `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -630,14 +630,15 @@
 
 PipelineMetadataTypeDef = TypedDict(
     "PipelineMetadataTypeDef",
     {
         "pipelineArn": str,
         "created": datetime,
         "updated": datetime,
+        "pollingDisabledAt": datetime,
     },
     total=False,
 )
 
 GetPipelineStateInputRequestTypeDef = TypedDict(
     "GetPipelineStateInputRequestTypeDef",
     {
```

### Comparing `mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline.egg-info/PKG-INFO` & `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codepipeline
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.CodePipeline 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.141
+Summary: Type annotations for boto3.CodePipeline 1.26.141 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-codepipeline"></a>
 
 # mypy-boto3-codepipeline
 
 [![PyPI - mypy-boto3-codepipeline](https://img.shields.io/pypi/v/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codepipeline?color=blue)](https://pypistats.org/packages/mypy-boto3-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodePipeline 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[boto3.CodePipeline 1.26.141](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codepipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/).
 
 See how it helps to find and fix potential bugs:
 
@@ -514,42 +515,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-codepipeline-1.26.0.post1/mypy_boto3_codepipeline.egg-info/SOURCES.txt` & `mypy-boto3-codepipeline-1.26.141/mypy_boto3_codepipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.26.0.post1/setup.py` & `mypy-boto3-codepipeline-1.26.141/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-codepipeline.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codepipeline",
-    version="1.26.0.post1",
+    version="1.26.141",
     packages=["mypy_boto3_codepipeline"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodePipeline 1.26.0 service generated with mypy-boto3-builder"
-        " 7.11.10"
+        "Type annotations for boto3.CodePipeline 1.26.141 service generated with mypy-boto3-builder"
+        " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 codepipeline type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_codepipeline": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_codepipeline": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```

