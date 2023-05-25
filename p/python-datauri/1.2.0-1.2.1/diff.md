# Comparing `tmp/python_datauri-1.2.0.tar.gz` & `tmp/python_datauri-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_datauri-1.2.0.tar", max compression
+gzip compressed data, was "python_datauri-1.2.1.tar", max compression
```

## Comparing `python_datauri-1.2.0.tar` & `python_datauri-1.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1211 2020-07-31 14:49:13.887654 python_datauri-1.2.0/LICENSE
--rw-r--r--   0        0        0     2067 2021-01-19 18:04:00.594309 python_datauri-1.2.0/README.rst
--rw-r--r--   0        0        0     4770 2023-05-24 21:43:12.696296 python_datauri-1.2.0/datauri/__init__.py
--rw-r--r--   0        0        0      134 2020-07-31 14:49:13.888532 python_datauri-1.2.0/datauri/exceptions.py
--rw-r--r--   0        0        0      655 2023-05-24 21:45:50.898950 python_datauri-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2795 1970-01-01 00:00:00.000000 python_datauri-1.2.0/setup.py
--rw-r--r--   0        0        0     2717 1970-01-01 00:00:00.000000 python_datauri-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2020-07-31 14:49:13.887654 python_datauri-1.2.1/LICENSE
+-rw-r--r--   0        0        0     2067 2021-01-19 18:04:00.594309 python_datauri-1.2.1/README.rst
+-rw-r--r--   0        0        0     4770 2023-05-24 21:43:12.696296 python_datauri-1.2.1/datauri/__init__.py
+-rw-r--r--   0        0        0      134 2020-07-31 14:49:13.888532 python_datauri-1.2.1/datauri/exceptions.py
+-rw-r--r--   0        0        0      639 2023-05-25 21:51:57.808504 python_datauri-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2708 1970-01-01 00:00:00.000000 python_datauri-1.2.1/setup.py
+-rw-r--r--   0        0        0     2680 1970-01-01 00:00:00.000000 python_datauri-1.2.1/PKG-INFO
```

### Comparing `python_datauri-1.2.0/LICENSE` & `python_datauri-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_datauri-1.2.0/README.rst` & `python_datauri-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `python_datauri-1.2.0/datauri/__init__.py` & `python_datauri-1.2.1/datauri/__init__.py`

 * *Files identical despite different names*

### Comparing `python_datauri-1.2.0/pyproject.toml` & `python_datauri-1.2.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [tool.poetry]
 name = "python-datauri"
-version = "1.2.0"
+version = "1.2.1"
 description = "A li'l class for data URI manipulation in Python"
 authors = ["Flavio Curella <flavio.curella@gmail.com>"]
 readme = "README.rst"
 packages = [{include = "datauri"}]
 license = "Unlicense"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-six = "^1.16.0"
 
 [tool.poetry.group.dev.dependencies]
 coveralls = "^3.3.1"
 pytest = "^7.3.1"
 pydantic = "^1.10.8"
 
 [build-system]
```

### Comparing `python_datauri-1.2.0/setup.py` & `python_datauri-1.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,24 @@
 
 packages = \
 ['datauri']
 
 package_data = \
 {'': ['*']}
 
-install_requires = \
-['six>=1.16.0,<2.0.0']
-
 setup_kwargs = {
     'name': 'python-datauri',
-    'version': '1.2.0',
+    'version': '1.2.1',
     'description': "A li'l class for data URI manipulation in Python",
     'long_description': "DataURI\n=======\n\n.. image:: https://github.com/fcurella/python-datauri/workflows/Python%20Tests/badge.svg\n    :target: https://github.com/fcurella/python-datauri/actions?query=workflow%3A%22Python+Tests%22\n    :alt: Build status of the master branch on Mac/Linux\n\n.. image:: https://coveralls.io/repos/github/fcurella/python-datauri/badge.svg?branch=master\n    :target: https://coveralls.io/github/fcurella/python-datauri?branch=master\n\nData URI manipulation made easy.\n\nThis isn't very robust, and will reject a number of valid data URIs. However, it meets the most useful case: a mimetype, a charset, and the base64 flag.\n\n\nInstallation\n------------\n\n.. code-block:: bash\n\n  $ pip install python-datauri\n\n\nParsing\n-------\n\n.. code-block:: python\n\n  >>> from datauri import DataURI\n  >>> uri = DataURI('data:text/plain;charset=utf-8;base64,VGhlIHF1aWNrIGJyb3duIGZveCBqdW1wZWQgb3ZlciB0aGUgbGF6eSBkb2cu')\n  >>> uri.mimetype\n  'text/plain'\n  >>> uri.charset\n  'utf-8'\n  >>> uri.is_base64\n  True\n  >>> uri.data\n  b'The quick brown fox jumped over the lazy dog.'\n\nNote that ``DataURI.data`` will always return bytes, (which in Python 2 is the same as a string).\nUse ``DataURI.text`` to get a string.\n\nCreating from a string\n----------------------\n\n.. code-block:: python\n\n  >>> from datauri import DataURI\n  >>> made = DataURI.make('text/plain', charset='us-ascii', base64=True, data='This is a message.')\n  >>> made\n  DataURI('data:text/plain;charset=us-ascii;base64,VGhpcyBpcyBhIG1lc3NhZ2Uu')\n  >>> made.data\n  b'This is a message.'\n\nCreating from a file\n--------------------\n\nThis is really just a convenience method.\n\n.. code-block:: python\n\n  >>> from datauri import DataURI\n  >>> png_uri = DataURI.from_file('somefile.png')\n  >>> png_uri.mimetype\n  'image/png'\n  >>> png_uri.data\n  b'\\x89PNG\\r\\n...'\n\nLicense\n-------\n\nThis code is released under the `Unlicense <http://unlicense.org/>`_.\n\nCredits\n-------\n\nThis is a repackaging of `this Gist <https://gist.github.com/zacharyvoase/5538178>`_\noriginally written by `Zachary Voase <https://github.com/zacharyvoase>`_.\n",
     'author': 'Flavio Curella',
     'author_email': 'flavio.curella@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
-    'install_requires': install_requires,
     'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `python_datauri-1.2.0/PKG-INFO` & `python_datauri-1.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: python-datauri
-Version: 1.2.0
+Version: 1.2.1
 Summary: A li'l class for data URI manipulation in Python
 License: Unlicense
 Author: Flavio Curella
 Author-email: flavio.curella@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: six (>=1.16.0,<2.0.0)
 Description-Content-Type: text/x-rst
 
 DataURI
 =======
 
 .. image:: https://github.com/fcurella/python-datauri/workflows/Python%20Tests/badge.svg
     :target: https://github.com/fcurella/python-datauri/actions?query=workflow%3A%22Python+Tests%22
```

