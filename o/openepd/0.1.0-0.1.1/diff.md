# Comparing `tmp/openepd-0.1.0.tar.gz` & `tmp/openepd-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openepd-0.1.0.tar", max compression
+gzip compressed data, was "openepd-0.1.1.tar", max compression
```

## Comparing `openepd-0.1.0.tar` & `openepd-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-05-18 14:32:16.267817 openepd-0.1.0/LICENSE
--rw-r--r--   0        0        0     2653 2023-05-24 13:40:51.682840 openepd-0.1.0/README.md
--rw-r--r--   0        0        0     3067 2023-05-24 13:43:19.735107 openepd-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      837 2023-05-24 13:45:45.674029 openepd-0.1.0/src/openepd/__init__.py
--rw-r--r--   0        0        0      855 2023-05-24 13:45:45.670696 openepd-0.1.0/src/openepd/__version__.py
--rw-r--r--   0        0        0      837 2023-05-24 13:45:45.670696 openepd-0.1.0/src/openepd/model/__init__.py
--rw-r--r--   0        0        0     1366 2023-05-24 13:45:45.674029 openepd-0.1.0/src/openepd/model/base.py
--rw-r--r--   0        0        0     2573 2023-05-24 13:45:45.670696 openepd-0.1.0/src/openepd/model/common.py
--rw-r--r--   0        0        0     5731 2023-05-24 13:45:45.670696 openepd-0.1.0/src/openepd/model/epd.py
--rw-r--r--   0        0        0     8887 2023-05-24 13:45:45.670696 openepd-0.1.0/src/openepd/model/lcia.py
--rw-r--r--   0        0        0     3783 2023-05-24 13:45:45.670696 openepd-0.1.0/src/openepd/model/orgs.py
--rw-r--r--   0        0        0     2902 2023-05-24 13:45:45.670696 openepd-0.1.0/src/openepd/model/pcr.py
--rw-r--r--   0        0        0     3586 1970-01-01 00:00:00.000000 openepd-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-25 12:22:07.914512 openepd-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2653 2023-05-25 12:22:07.914512 openepd-0.1.1/README.md
+-rw-r--r--   0        0        0     3051 2023-05-25 12:22:07.914512 openepd-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      837 2023-05-25 12:22:07.914512 openepd-0.1.1/src/openepd/__init__.py
+-rw-r--r--   0        0        0      855 2023-05-25 12:22:07.914512 openepd-0.1.1/src/openepd/__version__.py
+-rw-r--r--   0        0        0      837 2023-05-25 12:22:07.914512 openepd-0.1.1/src/openepd/model/__init__.py
+-rw-r--r--   0        0        0     1366 2023-05-25 12:22:07.914512 openepd-0.1.1/src/openepd/model/base.py
+-rw-r--r--   0        0        0     2573 2023-05-25 12:22:07.914512 openepd-0.1.1/src/openepd/model/common.py
+-rw-r--r--   0        0        0     5731 2023-05-25 12:22:07.914512 openepd-0.1.1/src/openepd/model/epd.py
+-rw-r--r--   0        0        0     8887 2023-05-25 12:22:07.914512 openepd-0.1.1/src/openepd/model/lcia.py
+-rw-r--r--   0        0        0     3783 2023-05-25 12:22:07.914512 openepd-0.1.1/src/openepd/model/orgs.py
+-rw-r--r--   0        0        0     2902 2023-05-25 12:22:07.914512 openepd-0.1.1/src/openepd/model/pcr.py
+-rw-r--r--   0        0        0     3535 1970-01-01 00:00:00.000000 openepd-0.1.1/PKG-INFO
```

### Comparing `openepd-0.1.0/LICENSE` & `openepd-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openepd-0.1.0/README.md` & `openepd-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `openepd-0.1.0/pyproject.toml` & `openepd-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "openepd"
-version = "0.1.0"
+version = "0.1.1"
 license = "Apache-2.0"
 description = "Python library to work with OpenEPD format"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <support@c-change-labs.com>"]
-repository = "https://github.com/cchangelabs/ilcdlib"
+repository = "https://github.com/cchangelabs/openepd"
 keywords = []
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
@@ -24,23 +24,23 @@
 pydantic = ">=1.10"
 email-validator = ">=2.0"
 
 # Optional dependencies
 # lxml = { version = "~=4.9.2", optional = true }
 
 [tool.poetry.dev-dependencies]
-platformdirs = "~=2.6.2"    # Remove this as soon as poetry supports 3.x version
 # Unit tests
 coverage = { version = "=6.5", extras = ["toml"] }
 pytest = "~=7.2"
 pytest-subtests = "~=0.4"
 pytest-cov = "~=4.0"
 teamcity-messages = ">=1.31"
 
 # Dev tools
+#virtualenv = "<=20.23.0" # to avoid conflict with flake plugins
 black = "~=22.3"
 licenseheaders = "~=0.8"
 flake8 = "~=4.0"
 flake8-import-graph = "==0.1.3"
 flake8-docstrings = "~=1.7.0"
 isort = "~=5.11"
 mypy = ">=1.0.1"
@@ -52,15 +52,15 @@
 types-deprecated = ">=1.2.9"
 
 [tool.poetry.extras]
 #xml = ["lxml"]
 
 
 [tool.commitizen]
-version = "0.2.0"
+version = "0.1.1"
 bump_version = "bump: version $current_version → $new_version"
 update_changelog_on_bump = true
 pre_bump_hooks = []
 version_files = [
     "pyproject.toml",
     "src/openepd/__version__.py",
 ]
```

### Comparing `openepd-0.1.0/src/openepd/__init__.py` & `openepd-0.1.1/src/openepd/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.1.0/src/openepd/__version__.py` & `openepd-0.1.1/src/openepd/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "0.2.0"
+VERSION = "0.1.1"
```

### Comparing `openepd-0.1.0/src/openepd/model/__init__.py` & `openepd-0.1.1/src/openepd/model/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.1.0/src/openepd/model/base.py` & `openepd-0.1.1/src/openepd/model/base.py`

 * *Files identical despite different names*

### Comparing `openepd-0.1.0/src/openepd/model/common.py` & `openepd-0.1.1/src/openepd/model/common.py`

 * *Files identical despite different names*

### Comparing `openepd-0.1.0/src/openepd/model/epd.py` & `openepd-0.1.1/src/openepd/model/epd.py`

 * *Files identical despite different names*

### Comparing `openepd-0.1.0/src/openepd/model/lcia.py` & `openepd-0.1.1/src/openepd/model/lcia.py`

 * *Files identical despite different names*

### Comparing `openepd-0.1.0/src/openepd/model/orgs.py` & `openepd-0.1.1/src/openepd/model/orgs.py`

 * *Files identical despite different names*

### Comparing `openepd-0.1.0/src/openepd/model/pcr.py` & `openepd-0.1.1/src/openepd/model/pcr.py`

 * *Files identical despite different names*

### Comparing `openepd-0.1.0/PKG-INFO` & `openepd-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: openepd
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library to work with OpenEPD format
-Home-page: https://github.com/cchangelabs/ilcdlib
+Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: support@c-change-labs.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: email-validator (>=2.0)
 Requires-Dist: pydantic (>=1.10)
-Project-URL: Repository, https://github.com/cchangelabs/ilcdlib
+Project-URL: Repository, https://github.com/cchangelabs/openepd
 Description-Content-Type: text/markdown
 
 # Python Library to work with OpenEPD format
 
 <p align="center">
 <a href="https://pypi.org/project/openepd/"><img src="https://img.shields.io/pypi/l/openepd?style=for-the-badge" title="License: Apache-2"/></a> 
 <a href="https://pypi.org/project/openepd/"><img src="https://img.shields.io/pypi/pyversions/openepd?style=for-the-badge" title="Python Versions"/></a>
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: openepd Version: 0.1.0 Summary: Python library to
-work with OpenEPD format Home-page: https://github.com/cchangelabs/ilcdlib
+Metadata-Version: 2.1 Name: openepd Version: 0.1.1 Summary: Python library to
+work with OpenEPD format Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0 Author: C-Change Labs Author-email: support@c-change-
 labs.com Maintainer: C-Change Labs Maintainer-email: support@c-change-labs.com
 Requires-Python: >=3.11,<4.0 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: email-validator (>=2.0) Requires-Dist: pydantic (>=1.10)
-Project-URL: Repository, https://github.com/cchangelabs/ilcdlib Description-
-Content-Type: text/markdown # Python Library to work with OpenEPD format
+Language :: Python :: 3.11 Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Requires-Dist: email-validator (>=2.0) Requires-
+Dist: pydantic (>=1.10) Project-URL: Repository, https://github.com/
+cchangelabs/openepd Description-Content-Type: text/markdown # Python Library to
+work with OpenEPD format
      [https://img.shields.io/pypi/l/openepd?style=for-the-badge] [https://
      img.shields.io/pypi/pyversions/openepd?style=for-the-badge] [https://
  img.shields.io/badge/Code%20Style-black-black?style=for-the-badge] [https://
   img.shields.io/pypi/v/openepd?style=for-the-badge] [https://img.shields.io/
                      pypi/dm/openepd?style=for-the-badge]
      [https://img.shields.io/github/workflow/status/cchangelabs/cli-rack/
 Sanity%20Check?style=for-the-badge] [https://img.shields.io/github/last-commit/
```

