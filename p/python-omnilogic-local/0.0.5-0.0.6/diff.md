# Comparing `tmp/python_omnilogic_local-0.0.5.tar.gz` & `tmp/python_omnilogic_local-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_omnilogic_local-0.0.5.tar", max compression
+gzip compressed data, was "python_omnilogic_local-0.0.6.tar", max compression
```

## Comparing `python_omnilogic_local-0.0.5.tar` & `python_omnilogic_local-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,15 @@
--rw-r--r--   0        0        0     1697 2023-05-15 14:54:23.226170 python_omnilogic_local-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-05-15 14:54:23.226170 python_omnilogic_local-0.0.5/pyomnilogic_local/__init__.py
--rwxr-xr-x   0        0        0    30991 2023-05-15 17:41:24.211638 python_omnilogic_local-0.0.5/pyomnilogic_local/api.py
--rwxr-xr-x   0        0        0     1763 2023-05-15 14:54:23.226170 python_omnilogic_local-0.0.5/pyomnilogic_local/cli.py
--rw-r--r--   0        0        0     1674 2023-05-10 23:14:12.231775 python_omnilogic_local-0.0.5/pyomnilogic_local/types.py
--rw-r--r--   0        0        0     1414 2023-05-15 17:40:51.919165 python_omnilogic_local-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2646 1970-01-01 00:00:00.000000 python_omnilogic_local-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1697 2023-05-15 14:54:23.226170 python_omnilogic_local-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 14:54:23.226170 python_omnilogic_local-0.0.6/pyomnilogic_local/__init__.py
+-rwxr-xr-x   0        0        0    16868 2023-05-25 01:43:06.594908 python_omnilogic_local-0.0.6/pyomnilogic_local/api.py
+-rwxr-xr-x   0        0        0     2108 2023-05-25 01:43:06.594908 python_omnilogic_local-0.0.6/pyomnilogic_local/cli.py
+-rw-r--r--   0        0        0        0 2023-05-25 01:42:52.754733 python_omnilogic_local-0.0.6/pyomnilogic_local/models/__init__.py
+-rw-r--r--   0        0        0       51 2023-05-25 01:42:52.754733 python_omnilogic_local-0.0.6/pyomnilogic_local/models/const.py
+-rw-r--r--   0        0        0      407 2023-05-25 01:42:52.754733 python_omnilogic_local-0.0.6/pyomnilogic_local/models/leadmessage.py
+-rw-r--r--   0        0        0     5747 2023-05-25 01:43:01.066838 python_omnilogic_local-0.0.6/pyomnilogic_local/models/mspconfig.py
+-rw-r--r--   0        0        0     7770 2023-05-25 01:43:01.066838 python_omnilogic_local-0.0.6/pyomnilogic_local/models/telemetry.py
+-rw-r--r--   0        0        0      337 2023-05-25 01:42:52.754733 python_omnilogic_local-0.0.6/pyomnilogic_local/models/util.py
+-rw-r--r--   0        0        0     7262 2023-05-25 01:43:06.594908 python_omnilogic_local-0.0.6/pyomnilogic_local/protocol.py
+-rw-r--r--   0        0        0     5160 2023-05-25 01:43:06.594908 python_omnilogic_local-0.0.6/pyomnilogic_local/types.py
+-rw-r--r--   0        0        0      361 2023-05-25 01:42:52.754733 python_omnilogic_local-0.0.6/pyomnilogic_local/util.py
+-rw-r--r--   0        0        0     4902 2023-05-25 01:43:10.350956 python_omnilogic_local-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 python_omnilogic_local-0.0.6/PKG-INFO
```

### Comparing `python_omnilogic_local-0.0.5/README.md` & `python_omnilogic_local-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.0.5/PKG-INFO` & `python_omnilogic_local-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: python-omnilogic-local
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API
 Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0
 Author: cryptk
 Author-email: cryptk@users.noreply.github.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pydantic-xml (>=0.6.1,<0.7.0)
+Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Project-URL: Repository, https://github.com/cryptk/python-omnilogic-local
 Description-Content-Type: text/markdown
 
 # Pyomnilogic Local
 
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.0.5 Summary: A
+Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.0.6 Summary: A
 library for local control of Hayward OmniHub/OmniLogic pool controllers using
 their local API Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0 Author: cryptk Author-email:
-cryptk@users.noreply.github.com Requires-Python: >=3.9,<4.0 Classifier:
+cryptk@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
-Software Development :: Libraries Project-URL: Repository, https://github.com/
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries Requires-Dist: pydantic
+(>=1.10.7,<2.0.0) Requires-Dist: pydantic-xml (>=0.6.1,<0.7.0) Requires-Dist:
+xmltodict (>=0.13.0,<0.14.0) Project-URL: Repository, https://github.com/
 cryptk/python-omnilogic-local Description-Content-Type: text/markdown #
 Pyomnilogic Local
              [PyPI_Version] [Supported Python versions] [License]
 A library implementing the UDP XML Local Control api for Hayward OmniLogic and
 OmniHub pool controllers ## Installation This package is published to pypi at
 https://pypi.org/project/python-omnilogic-local/: `pip install python-
 omnilogic-local` ## Functionality This library is still under development and
```

