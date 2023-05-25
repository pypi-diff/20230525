# Comparing `tmp/delu-0.0.16.tar.gz` & `tmp/delu-0.0.17.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delu-0.0.16.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "delu-0.0.17.dev0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `delu-0.0.16.tar` & `delu-0.0.17.dev0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0      439 2023-05-25 21:13:54.610436 delu-0.0.16/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      317 2023-05-25 21:13:54.610581 delu-0.0.16/.github/ISSUE_TEMPLATE/other.md
--rw-r--r--   0        0        0      318 2023-05-25 21:13:54.610662 delu-0.0.16/.github/pull_request_template.md
--rw-r--r--   0        0        0     2277 2023-05-25 21:13:54.610860 delu-0.0.16/.gitignore
--rw-r--r--   0        0        0     1210 2023-05-25 21:13:54.610971 delu-0.0.16/CONTRIBUTING.md
--rw-r--r--   0        0        0     1063 2023-05-25 21:13:54.611135 delu-0.0.16/LICENSE
--rw-r--r--   0        0        0     1304 2023-05-25 21:13:54.611299 delu-0.0.16/Makefile
--rw-r--r--   0        0        0     1977 2023-05-25 21:13:54.611410 delu-0.0.16/README.rst
--rw-r--r--   0        0        0      539 2023-05-25 21:15:59.486661 delu-0.0.16/delu/__init__.py
--rw-r--r--   0        0        0    18605 2023-05-25 21:13:54.611728 delu-0.0.16/delu/_stream.py
--rw-r--r--   0        0        0    13571 2023-05-25 21:13:54.611928 delu-0.0.16/delu/_tensor_ops.py
--rw-r--r--   0        0        0    16980 2023-05-25 21:13:54.612119 delu-0.0.16/delu/_tools.py
--rw-r--r--   0        0        0     5037 2023-05-25 21:13:54.612271 delu-0.0.16/delu/_utilities.py
--rw-r--r--   0        0        0     1156 2023-05-25 21:13:54.612382 delu-0.0.16/delu/_utils.py
--rw-r--r--   0        0        0      775 2023-05-25 21:13:54.612486 delu-0.0.16/delu/cuda.py
--rw-r--r--   0        0        0    13592 2023-05-25 21:13:54.612639 delu-0.0.16/delu/data.py
--rw-r--r--   0        0        0       88 2023-05-25 21:13:54.612732 delu-0.0.16/delu/exceptions.py
--rw-r--r--   0        0        0     3290 2023-05-25 21:13:54.612839 delu-0.0.16/delu/hardware.py
--rw-r--r--   0        0        0      734 2023-05-25 21:13:54.612936 delu-0.0.16/delu/nn.py
--rw-r--r--   0        0        0     4926 2023-05-25 21:13:54.613050 delu-0.0.16/delu/random.py
--rw-r--r--   0        0        0        0 2023-05-25 21:13:54.613130 delu-0.0.16/delu/tests/__init__.py
--rw-r--r--   0        0        0     5913 2023-05-25 21:13:54.613253 delu-0.0.16/delu/tests/test__tensor_ops.py
--rw-r--r--   0        0        0     4708 2023-05-25 21:13:54.613365 delu-0.0.16/delu/tests/test__tools.py
--rw-r--r--   0        0        0     1850 2023-05-25 21:13:54.613468 delu-0.0.16/delu/tests/test__utilities.py
--rw-r--r--   0        0        0      536 2023-05-25 21:13:54.613566 delu-0.0.16/delu/tests/test_cuda.py
--rw-r--r--   0        0        0     2178 2023-05-25 21:13:54.613652 delu-0.0.16/delu/tests/test_data.py
--rw-r--r--   0        0        0      286 2023-05-25 21:13:54.613706 delu-0.0.16/delu/tests/test_nn.py
--rw-r--r--   0        0        0     1777 2023-05-25 21:13:54.613763 delu-0.0.16/delu/tests/test_random.py
--rw-r--r--   0        0        0     5296 2023-05-25 21:13:54.613855 delu-0.0.16/delu/tests/test_stream.py
--rw-r--r--   0        0        0     1165 2023-05-25 21:13:54.613951 delu-0.0.16/delu/tests/util.py
--rw-r--r--   0        0        0      635 2023-05-25 21:13:54.614027 delu-0.0.16/docs/Makefile
--rw-r--r--   0        0        0      106 2023-05-25 21:13:54.614126 delu-0.0.16/docs/_static/furo.css
--rw-r--r--   0        0        0      857 2023-05-25 21:13:54.614191 delu-0.0.16/docs/_static/material_theme.css
--rw-r--r--   0        0        0      364 2023-05-25 21:13:54.614247 delu-0.0.16/docs/_static/rtd_theme.css
--rw-r--r--   0        0        0      288 2023-05-25 21:13:54.614346 delu-0.0.16/docs/_static/versions.json
--rw-r--r--   0        0        0      791 2023-05-25 21:13:54.614447 delu-0.0.16/docs/_templates/class.rst
--rw-r--r--   0        0        0       98 2023-05-25 21:13:54.614519 delu-0.0.16/docs/_templates/class_just_autoclass.rst
--rw-r--r--   0        0        0      143 2023-05-25 21:13:54.614576 delu-0.0.16/docs/_templates/class_nn.rst
--rw-r--r--   0        0        0      163 2023-05-25 21:13:54.614634 delu-0.0.16/docs/_templates/layout.html
--rw-r--r--   0        0        0     5111 2023-05-25 21:13:54.614737 delu-0.0.16/docs/conf.py
--rw-r--r--   0        0        0    15086 2023-05-25 21:13:54.614849 delu-0.0.16/docs/images/favicon.ico
--rw-r--r--   0        0        0    12000 2023-05-25 21:13:54.614967 delu-0.0.16/docs/images/logo.png
--rw-r--r--   0        0        0      310 2023-05-25 21:13:54.615029 delu-0.0.16/docs/images/logo_120x120.svg
--rw-r--r--   0        0        0      306 2023-05-25 21:13:54.615081 delu-0.0.16/docs/images/logo_28x28.svg
--rw-r--r--   0        0        0     1796 2023-05-25 21:13:54.615178 delu-0.0.16/docs/index.rst
--rw-r--r--   0        0        0      732 2023-05-25 21:13:54.615269 delu-0.0.16/docs/learn.rst
--rw-r--r--   0        0        0      794 2023-05-25 21:13:54.615335 delu-0.0.16/docs/make.bat
--rw-r--r--   0        0        0      157 2023-05-25 21:13:54.615431 delu-0.0.16/docs/reference/cuda.rst
--rw-r--r--   0        0        0      452 2023-05-25 21:13:54.615534 delu-0.0.16/docs/reference/data.rst
--rw-r--r--   0        0        0      734 2023-05-25 21:13:54.615615 delu-0.0.16/docs/reference/delu.rst
--rw-r--r--   0        0        0      242 2023-05-25 21:13:54.615744 delu-0.0.16/docs/reference/hardware.rst
--rw-r--r--   0        0        0      164 2023-05-25 21:13:54.615821 delu-0.0.16/docs/reference/nn.rst
--rw-r--r--   0        0        0      197 2023-05-25 21:13:54.615900 delu-0.0.16/docs/reference/random.rst
--rw-r--r--   0        0        0      288 2023-05-25 21:13:54.615990 delu-0.0.16/docs/spelling_wordlist.txt
--rw-r--r--   0        0        0      766 2023-05-25 21:13:54.616095 delu-0.0.16/docs/version.rst
--rw-r--r--   0        0        0     6081 2023-05-25 21:13:54.616219 delu-0.0.16/examples/mnist.py
--rw-r--r--   0        0        0     1571 2023-05-25 21:13:54.616322 delu-0.0.16/pyproject.toml
--rw-r--r--   0        0        0      485 2023-05-25 21:13:54.616454 delu-0.0.16/requirements_dev.txt
--rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 delu-0.0.16/PKG-INFO
+-rw-r--r--   0        0        0      439 2023-05-25 21:13:54.610436 delu-0.0.17.dev0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      317 2023-05-25 21:13:54.610581 delu-0.0.17.dev0/.github/ISSUE_TEMPLATE/other.md
+-rw-r--r--   0        0        0      318 2023-05-25 21:13:54.610662 delu-0.0.17.dev0/.github/pull_request_template.md
+-rw-r--r--   0        0        0     2277 2023-05-25 21:13:54.610860 delu-0.0.17.dev0/.gitignore
+-rw-r--r--   0        0        0     1210 2023-05-25 21:13:54.610971 delu-0.0.17.dev0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1063 2023-05-25 21:13:54.611135 delu-0.0.17.dev0/LICENSE
+-rw-r--r--   0        0        0     1304 2023-05-25 21:13:54.611299 delu-0.0.17.dev0/Makefile
+-rw-r--r--   0        0        0     1977 2023-05-25 21:13:54.611410 delu-0.0.17.dev0/README.rst
+-rw-r--r--   0        0        0      544 2023-05-25 21:13:54.611560 delu-0.0.17.dev0/delu/__init__.py
+-rw-r--r--   0        0        0    18605 2023-05-25 21:13:54.611728 delu-0.0.17.dev0/delu/_stream.py
+-rw-r--r--   0        0        0    13571 2023-05-25 21:13:54.611928 delu-0.0.17.dev0/delu/_tensor_ops.py
+-rw-r--r--   0        0        0    16980 2023-05-25 21:13:54.612119 delu-0.0.17.dev0/delu/_tools.py
+-rw-r--r--   0        0        0     5037 2023-05-25 21:13:54.612271 delu-0.0.17.dev0/delu/_utilities.py
+-rw-r--r--   0        0        0     1156 2023-05-25 21:13:54.612382 delu-0.0.17.dev0/delu/_utils.py
+-rw-r--r--   0        0        0      775 2023-05-25 21:13:54.612486 delu-0.0.17.dev0/delu/cuda.py
+-rw-r--r--   0        0        0    13592 2023-05-25 21:13:54.612639 delu-0.0.17.dev0/delu/data.py
+-rw-r--r--   0        0        0       88 2023-05-25 21:13:54.612732 delu-0.0.17.dev0/delu/exceptions.py
+-rw-r--r--   0        0        0     3290 2023-05-25 21:13:54.612839 delu-0.0.17.dev0/delu/hardware.py
+-rw-r--r--   0        0        0      734 2023-05-25 21:13:54.612936 delu-0.0.17.dev0/delu/nn.py
+-rw-r--r--   0        0        0     4926 2023-05-25 21:13:54.613050 delu-0.0.17.dev0/delu/random.py
+-rw-r--r--   0        0        0        0 2023-05-25 21:13:54.613130 delu-0.0.17.dev0/delu/tests/__init__.py
+-rw-r--r--   0        0        0     5913 2023-05-25 21:13:54.613253 delu-0.0.17.dev0/delu/tests/test__tensor_ops.py
+-rw-r--r--   0        0        0     4708 2023-05-25 21:13:54.613365 delu-0.0.17.dev0/delu/tests/test__tools.py
+-rw-r--r--   0        0        0     1850 2023-05-25 21:13:54.613468 delu-0.0.17.dev0/delu/tests/test__utilities.py
+-rw-r--r--   0        0        0      536 2023-05-25 21:13:54.613566 delu-0.0.17.dev0/delu/tests/test_cuda.py
+-rw-r--r--   0        0        0     2178 2023-05-25 21:13:54.613652 delu-0.0.17.dev0/delu/tests/test_data.py
+-rw-r--r--   0        0        0      286 2023-05-25 21:13:54.613706 delu-0.0.17.dev0/delu/tests/test_nn.py
+-rw-r--r--   0        0        0     1777 2023-05-25 21:13:54.613763 delu-0.0.17.dev0/delu/tests/test_random.py
+-rw-r--r--   0        0        0     5296 2023-05-25 21:13:54.613855 delu-0.0.17.dev0/delu/tests/test_stream.py
+-rw-r--r--   0        0        0     1165 2023-05-25 21:13:54.613951 delu-0.0.17.dev0/delu/tests/util.py
+-rw-r--r--   0        0        0      635 2023-05-25 21:13:54.614027 delu-0.0.17.dev0/docs/Makefile
+-rw-r--r--   0        0        0      106 2023-05-25 21:13:54.614126 delu-0.0.17.dev0/docs/_static/furo.css
+-rw-r--r--   0        0        0      857 2023-05-25 21:13:54.614191 delu-0.0.17.dev0/docs/_static/material_theme.css
+-rw-r--r--   0        0        0      364 2023-05-25 21:13:54.614247 delu-0.0.17.dev0/docs/_static/rtd_theme.css
+-rw-r--r--   0        0        0      288 2023-05-25 21:13:54.614346 delu-0.0.17.dev0/docs/_static/versions.json
+-rw-r--r--   0        0        0      791 2023-05-25 21:13:54.614447 delu-0.0.17.dev0/docs/_templates/class.rst
+-rw-r--r--   0        0        0       98 2023-05-25 21:13:54.614519 delu-0.0.17.dev0/docs/_templates/class_just_autoclass.rst
+-rw-r--r--   0        0        0      143 2023-05-25 21:13:54.614576 delu-0.0.17.dev0/docs/_templates/class_nn.rst
+-rw-r--r--   0        0        0      163 2023-05-25 21:13:54.614634 delu-0.0.17.dev0/docs/_templates/layout.html
+-rw-r--r--   0        0        0     5111 2023-05-25 21:13:54.614737 delu-0.0.17.dev0/docs/conf.py
+-rw-r--r--   0        0        0    15086 2023-05-25 21:13:54.614849 delu-0.0.17.dev0/docs/images/favicon.ico
+-rw-r--r--   0        0        0    12000 2023-05-25 21:13:54.614967 delu-0.0.17.dev0/docs/images/logo.png
+-rw-r--r--   0        0        0      310 2023-05-25 21:13:54.615029 delu-0.0.17.dev0/docs/images/logo_120x120.svg
+-rw-r--r--   0        0        0      306 2023-05-25 21:13:54.615081 delu-0.0.17.dev0/docs/images/logo_28x28.svg
+-rw-r--r--   0        0        0     1796 2023-05-25 21:13:54.615178 delu-0.0.17.dev0/docs/index.rst
+-rw-r--r--   0        0        0      732 2023-05-25 21:13:54.615269 delu-0.0.17.dev0/docs/learn.rst
+-rw-r--r--   0        0        0      794 2023-05-25 21:13:54.615335 delu-0.0.17.dev0/docs/make.bat
+-rw-r--r--   0        0        0      157 2023-05-25 21:13:54.615431 delu-0.0.17.dev0/docs/reference/cuda.rst
+-rw-r--r--   0        0        0      452 2023-05-25 21:13:54.615534 delu-0.0.17.dev0/docs/reference/data.rst
+-rw-r--r--   0        0        0      734 2023-05-25 21:13:54.615615 delu-0.0.17.dev0/docs/reference/delu.rst
+-rw-r--r--   0        0        0      242 2023-05-25 21:13:54.615744 delu-0.0.17.dev0/docs/reference/hardware.rst
+-rw-r--r--   0        0        0      164 2023-05-25 21:13:54.615821 delu-0.0.17.dev0/docs/reference/nn.rst
+-rw-r--r--   0        0        0      197 2023-05-25 21:13:54.615900 delu-0.0.17.dev0/docs/reference/random.rst
+-rw-r--r--   0        0        0      288 2023-05-25 21:13:54.615990 delu-0.0.17.dev0/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0      766 2023-05-25 21:13:54.616095 delu-0.0.17.dev0/docs/version.rst
+-rw-r--r--   0        0        0     6081 2023-05-25 21:13:54.616219 delu-0.0.17.dev0/examples/mnist.py
+-rw-r--r--   0        0        0     1571 2023-05-25 21:13:54.616322 delu-0.0.17.dev0/pyproject.toml
+-rw-r--r--   0        0        0      485 2023-05-25 21:13:54.616454 delu-0.0.17.dev0/requirements_dev.txt
+-rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 delu-0.0.17.dev0/PKG-INFO
```

### Comparing `delu-0.0.16/.gitignore` & `delu-0.0.17.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/CONTRIBUTING.md` & `delu-0.0.17.dev0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/LICENSE` & `delu-0.0.17.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/Makefile` & `delu-0.0.17.dev0/Makefile`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/README.rst` & `delu-0.0.17.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/delu/__init__.py` & `delu-0.0.17.dev0/delu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Deep Learning Utilities for PyTorch users."""
-__version__ = '0.0.16'
+__version__ = '0.0.17.dev0'
 
 from . import cuda  # noqa: F401
 from . import data  # noqa: F401
 from . import hardware  # noqa: F401
 from . import nn  # noqa: F401
 from . import random  # noqa: F401
 from ._stream import Stream  # noqa: F401
```

### Comparing `delu-0.0.16/delu/_stream.py` & `delu-0.0.17.dev0/delu/_stream.py`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/delu/_tensor_ops.py` & `delu-0.0.17.dev0/delu/_tensor_ops.py`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/delu/_tools.py` & `delu-0.0.17.dev0/delu/_tools.py`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/delu/_utilities.py` & `delu-0.0.17.dev0/delu/_utilities.py`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/delu/_utils.py` & `delu-0.0.17.dev0/delu/_utils.py`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/delu/cuda.py` & `delu-0.0.17.dev0/delu/cuda.py`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/delu/data.py` & `delu-0.0.17.dev0/delu/data.py`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/delu/hardware.py` & `delu-0.0.17.dev0/delu/hardware.py`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/delu/nn.py` & `delu-0.0.17.dev0/delu/nn.py`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/delu/random.py` & `delu-0.0.17.dev0/delu/random.py`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/delu/tests/test__tensor_ops.py` & `delu-0.0.17.dev0/delu/tests/test__tensor_ops.py`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/delu/tests/test__tools.py` & `delu-0.0.17.dev0/delu/tests/test__tools.py`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/delu/tests/test__utilities.py` & `delu-0.0.17.dev0/delu/tests/test__utilities.py`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/delu/tests/test_cuda.py` & `delu-0.0.17.dev0/delu/tests/test_cuda.py`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/delu/tests/test_data.py` & `delu-0.0.17.dev0/delu/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/delu/tests/test_random.py` & `delu-0.0.17.dev0/delu/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/delu/tests/test_stream.py` & `delu-0.0.17.dev0/delu/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/delu/tests/util.py` & `delu-0.0.17.dev0/delu/tests/util.py`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/docs/Makefile` & `delu-0.0.17.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/docs/_static/material_theme.css` & `delu-0.0.17.dev0/docs/_static/material_theme.css`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/docs/_templates/class.rst` & `delu-0.0.17.dev0/docs/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/docs/conf.py` & `delu-0.0.17.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/docs/images/favicon.ico` & `delu-0.0.17.dev0/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/docs/images/logo.png` & `delu-0.0.17.dev0/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/docs/index.rst` & `delu-0.0.17.dev0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/docs/learn.rst` & `delu-0.0.17.dev0/docs/learn.rst`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/docs/make.bat` & `delu-0.0.17.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/docs/reference/delu.rst` & `delu-0.0.17.dev0/docs/reference/delu.rst`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/docs/version.rst` & `delu-0.0.17.dev0/docs/version.rst`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/examples/mnist.py` & `delu-0.0.17.dev0/examples/mnist.py`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/pyproject.toml` & `delu-0.0.17.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `delu-0.0.16/PKG-INFO` & `delu-0.0.17.dev0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delu
-Version: 0.0.16
+Version: 0.0.17.dev0
 Summary: Deep Learning Utilities for PyTorch users.
 Keywords: artificial intelligence,deep learning,library,python,pytorch,torch
 Author-email: Yura52 <strausmg@gmail.com>
 Requires-Python: >=3.8
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

