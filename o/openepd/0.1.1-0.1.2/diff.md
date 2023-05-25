# Comparing `tmp/openepd-0.1.1.tar.gz` & `tmp/openepd-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openepd-0.1.1.tar", max compression
+gzip compressed data, was "openepd-0.1.2.tar", max compression
```

## Comparing `openepd-0.1.1.tar` & `openepd-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-05-25 12:22:07.914512 openepd-0.1.1/LICENSE
--rw-r--r--   0        0        0     2653 2023-05-25 12:22:07.914512 openepd-0.1.1/README.md
--rw-r--r--   0        0        0     3051 2023-05-25 12:22:07.914512 openepd-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      837 2023-05-25 12:22:07.914512 openepd-0.1.1/src/openepd/__init__.py
--rw-r--r--   0        0        0      855 2023-05-25 12:22:07.914512 openepd-0.1.1/src/openepd/__version__.py
--rw-r--r--   0        0        0      837 2023-05-25 12:22:07.914512 openepd-0.1.1/src/openepd/model/__init__.py
--rw-r--r--   0        0        0     1366 2023-05-25 12:22:07.914512 openepd-0.1.1/src/openepd/model/base.py
--rw-r--r--   0        0        0     2573 2023-05-25 12:22:07.914512 openepd-0.1.1/src/openepd/model/common.py
--rw-r--r--   0        0        0     5731 2023-05-25 12:22:07.914512 openepd-0.1.1/src/openepd/model/epd.py
--rw-r--r--   0        0        0     8887 2023-05-25 12:22:07.914512 openepd-0.1.1/src/openepd/model/lcia.py
--rw-r--r--   0        0        0     3783 2023-05-25 12:22:07.914512 openepd-0.1.1/src/openepd/model/orgs.py
--rw-r--r--   0        0        0     2902 2023-05-25 12:22:07.914512 openepd-0.1.1/src/openepd/model/pcr.py
--rw-r--r--   0        0        0     3535 1970-01-01 00:00:00.000000 openepd-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-25 12:58:08.124950 openepd-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2841 2023-05-25 12:58:08.124950 openepd-0.1.2/README.md
+-rw-r--r--   0        0        0     3051 2023-05-25 12:58:08.124950 openepd-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      837 2023-05-25 12:58:08.124950 openepd-0.1.2/src/openepd/__init__.py
+-rw-r--r--   0        0        0      855 2023-05-25 12:58:08.124950 openepd-0.1.2/src/openepd/__version__.py
+-rw-r--r--   0        0        0      837 2023-05-25 12:58:08.124950 openepd-0.1.2/src/openepd/model/__init__.py
+-rw-r--r--   0        0        0     1366 2023-05-25 12:58:08.124950 openepd-0.1.2/src/openepd/model/base.py
+-rw-r--r--   0        0        0     2573 2023-05-25 12:58:08.124950 openepd-0.1.2/src/openepd/model/common.py
+-rw-r--r--   0        0        0     5740 2023-05-25 12:58:08.124950 openepd-0.1.2/src/openepd/model/epd.py
+-rw-r--r--   0        0        0     8887 2023-05-25 12:58:08.124950 openepd-0.1.2/src/openepd/model/lcia.py
+-rw-r--r--   0        0        0     3783 2023-05-25 12:58:08.124950 openepd-0.1.2/src/openepd/model/org.py
+-rw-r--r--   0        0        0     2913 2023-05-25 12:58:08.128949 openepd-0.1.2/src/openepd/model/pcr.py
+-rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 openepd-0.1.2/PKG-INFO
```

### Comparing `openepd-0.1.1/LICENSE` & `openepd-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openepd-0.1.1/README.md` & `openepd-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 <p align="center">
 <a href="https://pypi.org/project/openepd/"><img src="https://img.shields.io/pypi/l/openepd?style=for-the-badge" title="License: Apache-2"/></a> 
 <a href="https://pypi.org/project/openepd/"><img src="https://img.shields.io/pypi/pyversions/openepd?style=for-the-badge" title="Python Versions"/></a> 
 <a href="https://github.com/psf/black/"><img src="https://img.shields.io/badge/Code%20Style-black-black?style=for-the-badge" title="Code style: black"/></a> 
 <a href="https://pypi.org/project/openepd/"><img src="https://img.shields.io/pypi/v/openepd?style=for-the-badge" title="PyPy Version"/></a> 
 <a href="https://pypi.org/project/openepd/"><img src="https://img.shields.io/pypi/dm/openepd?style=for-the-badge" title="PyPy Downloads"/></a> 
 <br>
-<a href="https://github.com/cchangelabs/openepd/actions/workflows/sanity-check.yml"><img src="https://img.shields.io/github/workflow/status/cchangelabs/cli-rack/Sanity%20Check?style=for-the-badge" title="Build Status"/></a> 
+<a href="https://github.com/cchangelabs/openepd/actions/workflows/sanity-check.yml"><img src="https://img.shields.io/github/actions/workflow/status/cchangelabs/openepd/sanity-check.yml?style=for-the-badge" title="Build Status"/></a> 
 <a href="https://github.com/cchangelabs/openepd/"><img src="https://img.shields.io/github/last-commit/cchangelabs/openepd?style=for-the-badge" title="Last Commit"/></a> 
 <a href="https://github.com/cchangelabs/openepd/releases/"><img src="https://img.shields.io/github/release-date/cchangelabs/openepd?style=for-the-badge" title="Last Release"/></a> 
+<a href="https://github.com/cchangelabs/openepd/releases/"><img src="https://img.shields.io/github/v/release/cchangelabs/openepd?style=for-the-badge" title="Recent Version"></a> 
 </p>
 
 This library is a Python library to work with OpenEPD format.
 
 ## About OpenEPD
 
 [openEPD](https://www.buildingtransparency.org/programs/openepd/) is an open data format for passing digital
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
 # Python Library to work with OpenEPD format
      [https://img.shields.io/pypi/l/openepd?style=for-the-badge] [https://
      img.shields.io/pypi/pyversions/openepd?style=for-the-badge] [https://
  img.shields.io/badge/Code%20Style-black-black?style=for-the-badge] [https://
   img.shields.io/pypi/v/openepd?style=for-the-badge] [https://img.shields.io/
                      pypi/dm/openepd?style=for-the-badge]
-     [https://img.shields.io/github/workflow/status/cchangelabs/cli-rack/
-Sanity%20Check?style=for-the-badge] [https://img.shields.io/github/last-commit/
-   cchangelabs/openepd?style=for-the-badge] [https://img.shields.io/github/
-             release-date/cchangelabs/openepd?style=for-the-badge]
+  [https://img.shields.io/github/actions/workflow/status/cchangelabs/openepd/
+  sanity-check.yml?style=for-the-badge] [https://img.shields.io/github/last-
+commit/cchangelabs/openepd?style=for-the-badge] [https://img.shields.io/github/
+release-date/cchangelabs/openepd?style=for-the-badge] [https://img.shields.io/
+           github/v/release/cchangelabs/openepd?style=for-the-badge]
 This library is a Python library to work with OpenEPD format. ## About OpenEPD
 [openEPD](https://www.buildingtransparency.org/programs/openepd/) is an open
 data format for passing digital third-party verified Environmental Product
 Declarations (EPDs) among Program Operators, EPD Databases, Life Cycle Analysis
 tools, design tools, reporting, and procurement. Unlike print or PDF EPDs,
 openEPD provides a shared and precise format to express and refer to EPDs in
 ways that modern databases can use. openEPD can be used alongside a printable
```

### Comparing `openepd-0.1.1/pyproject.toml` & `openepd-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openepd"
-version = "0.1.1"
+version = "0.1.2"
 license = "Apache-2.0"
 description = "Python library to work with OpenEPD format"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <support@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/openepd"
 keywords = []
 classifiers = [
@@ -52,15 +52,15 @@
 types-deprecated = ">=1.2.9"
 
 [tool.poetry.extras]
 #xml = ["lxml"]
 
 
 [tool.commitizen]
-version = "0.1.1"
+version = "0.1.2"
 bump_version = "bump: version $current_version → $new_version"
 update_changelog_on_bump = true
 pre_bump_hooks = []
 version_files = [
     "pyproject.toml",
     "src/openepd/__version__.py",
 ]
```

### Comparing `openepd-0.1.1/src/openepd/__init__.py` & `openepd-0.1.2/src/openepd/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.1.1/src/openepd/__version__.py` & `openepd-0.1.2/src/openepd/__version__.py`

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
-VERSION = "0.1.1"
+VERSION = "0.1.2"
```

### Comparing `openepd-0.1.1/src/openepd/model/__init__.py` & `openepd-0.1.2/src/openepd/model/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-0.1.1/src/openepd/model/base.py` & `openepd-0.1.2/src/openepd/model/base.py`

 * *Files identical despite different names*

### Comparing `openepd-0.1.1/src/openepd/model/common.py` & `openepd-0.1.2/src/openepd/model/common.py`

 * *Files identical despite different names*

### Comparing `openepd-0.1.1/src/openepd/model/epd.py` & `openepd-0.1.2/src/openepd/model/epd.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from typing import Literal
 
 import pydantic as pyd
 
 from openepd.model.base import BaseOpenEpdSchema
 from openepd.model.common import Amount, ExternallyIdentifiableMixin
 from openepd.model.lcia import ImpactSet, OutputFlowSet, ResourceUseSet
-from openepd.model.orgs import Org, Plant
+from openepd.model.org import Org, Plant
 
 
 class Epd(ExternallyIdentifiableMixin, BaseOpenEpdSchema):
     """Represent an EPD."""
 
     # TODO: Add validator for open-xpd-uuid on this field
     id: str = pyd.Field(
@@ -74,15 +74,15 @@
     manufacturer: Org | None = pyd.Field(
         description="JSON object for declaring Org. Sometimes called the "
         '"Declaration Holder" or "Declaration Owner".'
     )
     plants: list[Plant] = pyd.Field(
         max_items=32,
         description="List of object(s) for one or more plant(s) that this declaration applies to.",
-        default=[],
+        default_factory=list,
     )
     program_operator: Org | None = pyd.Field(description="JSON object for program operator Org")
     program_operator_doc_id: str | None = pyd.Field(
         max_length=200, description="Document identifier from Program Operator.", example="123-456.789/b"
     )
     program_operator_version: str | None = pyd.Field(
         max_length=200, description="Document version number from Program Operator.", example="4.3.0"
```

### Comparing `openepd-0.1.1/src/openepd/model/lcia.py` & `openepd-0.1.2/src/openepd/model/lcia.py`

 * *Files identical despite different names*

### Comparing `openepd-0.1.1/src/openepd/model/orgs.py` & `openepd-0.1.2/src/openepd/model/org.py`

 * *Files identical despite different names*

### Comparing `openepd-0.1.1/src/openepd/model/pcr.py` & `openepd-0.1.2/src/openepd/model/pcr.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import datetime
 from typing import Optional
 
 import pydantic as pyd
 
 from openepd.model.base import BaseOpenEpdSchema
 from openepd.model.common import ExternallyIdentifiableMixin, WithAttachmentsMixin
-from openepd.model.orgs import Org
+from openepd.model.org import Org
 
 
 class Pcr(ExternallyIdentifiableMixin, WithAttachmentsMixin, BaseOpenEpdSchema):
     """Represent a PCR (Product Category Rules)."""
 
     id: str = pyd.Field(
         description="The unique ID for this PCR.  To ensure global uniqueness, should be registered "
@@ -64,10 +64,10 @@
         description="Last day on which the document is valid",
     )
     parent: Optional["Pcr"] = pyd.Field(
         description="The parent PCR, base PCR, `Part A` PCR",
         default=None,
     )
     # TODO: why plural?
-    product_classes: dict[str, str] = pyd.Field(
+    product_classes: dict[str, str | list[str]] = pyd.Field(
         description="List of classifications, including Masterformat and UNSPC", default_factory=dict
     )
```

### Comparing `openepd-0.1.1/PKG-INFO` & `openepd-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openepd
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python library to work with OpenEPD format
 Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: support@c-change-labs.com
@@ -26,17 +26,18 @@
 <p align="center">
 <a href="https://pypi.org/project/openepd/"><img src="https://img.shields.io/pypi/l/openepd?style=for-the-badge" title="License: Apache-2"/></a> 
 <a href="https://pypi.org/project/openepd/"><img src="https://img.shields.io/pypi/pyversions/openepd?style=for-the-badge" title="Python Versions"/></a> 
 <a href="https://github.com/psf/black/"><img src="https://img.shields.io/badge/Code%20Style-black-black?style=for-the-badge" title="Code style: black"/></a> 
 <a href="https://pypi.org/project/openepd/"><img src="https://img.shields.io/pypi/v/openepd?style=for-the-badge" title="PyPy Version"/></a> 
 <a href="https://pypi.org/project/openepd/"><img src="https://img.shields.io/pypi/dm/openepd?style=for-the-badge" title="PyPy Downloads"/></a> 
 <br>
-<a href="https://github.com/cchangelabs/openepd/actions/workflows/sanity-check.yml"><img src="https://img.shields.io/github/workflow/status/cchangelabs/cli-rack/Sanity%20Check?style=for-the-badge" title="Build Status"/></a> 
+<a href="https://github.com/cchangelabs/openepd/actions/workflows/sanity-check.yml"><img src="https://img.shields.io/github/actions/workflow/status/cchangelabs/openepd/sanity-check.yml?style=for-the-badge" title="Build Status"/></a> 
 <a href="https://github.com/cchangelabs/openepd/"><img src="https://img.shields.io/github/last-commit/cchangelabs/openepd?style=for-the-badge" title="Last Commit"/></a> 
 <a href="https://github.com/cchangelabs/openepd/releases/"><img src="https://img.shields.io/github/release-date/cchangelabs/openepd?style=for-the-badge" title="Last Release"/></a> 
+<a href="https://github.com/cchangelabs/openepd/releases/"><img src="https://img.shields.io/github/v/release/cchangelabs/openepd?style=for-the-badge" title="Recent Version"></a> 
 </p>
 
 This library is a Python library to work with OpenEPD format.
 
 ## About OpenEPD
 
 [openEPD](https://www.buildingtransparency.org/programs/openepd/) is an open data format for passing digital
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openepd Version: 0.1.1 Summary: Python library to
+Metadata-Version: 2.1 Name: openepd Version: 0.1.2 Summary: Python library to
 work with OpenEPD format Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0 Author: C-Change Labs Author-email: support@c-change-
 labs.com Maintainer: C-Change Labs Maintainer-email: support@c-change-labs.com
 Requires-Python: >=3.11,<4.0 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
@@ -12,18 +12,19 @@
 cchangelabs/openepd Description-Content-Type: text/markdown # Python Library to
 work with OpenEPD format
      [https://img.shields.io/pypi/l/openepd?style=for-the-badge] [https://
      img.shields.io/pypi/pyversions/openepd?style=for-the-badge] [https://
  img.shields.io/badge/Code%20Style-black-black?style=for-the-badge] [https://
   img.shields.io/pypi/v/openepd?style=for-the-badge] [https://img.shields.io/
                      pypi/dm/openepd?style=for-the-badge]
-     [https://img.shields.io/github/workflow/status/cchangelabs/cli-rack/
-Sanity%20Check?style=for-the-badge] [https://img.shields.io/github/last-commit/
-   cchangelabs/openepd?style=for-the-badge] [https://img.shields.io/github/
-             release-date/cchangelabs/openepd?style=for-the-badge]
+  [https://img.shields.io/github/actions/workflow/status/cchangelabs/openepd/
+  sanity-check.yml?style=for-the-badge] [https://img.shields.io/github/last-
+commit/cchangelabs/openepd?style=for-the-badge] [https://img.shields.io/github/
+release-date/cchangelabs/openepd?style=for-the-badge] [https://img.shields.io/
+           github/v/release/cchangelabs/openepd?style=for-the-badge]
 This library is a Python library to work with OpenEPD format. ## About OpenEPD
 [openEPD](https://www.buildingtransparency.org/programs/openepd/) is an open
 data format for passing digital third-party verified Environmental Product
 Declarations (EPDs) among Program Operators, EPD Databases, Life Cycle Analysis
 tools, design tools, reporting, and procurement. Unlike print or PDF EPDs,
 openEPD provides a shared and precise format to express and refer to EPDs in
 ways that modern databases can use. openEPD can be used alongside a printable
```

