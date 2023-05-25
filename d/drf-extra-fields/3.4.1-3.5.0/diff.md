# Comparing `tmp/drf-extra-fields-3.4.1.tar.gz` & `tmp/drf-extra-fields-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drf-extra-fields-3.4.1.tar", last modified: Thu Oct 13 14:25:44 2022, max compression
+gzip compressed data, was "drf-extra-fields-3.5.0.tar", last modified: Thu May 25 10:44:00 2023, max compression
```

## Comparing `drf-extra-fields-3.4.1.tar` & `drf-extra-fields-3.5.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-10-13 14:25:44.000000 drf-extra-fields-3.4.1/
--rw-r--r--   0 apple      (501) staff       (20)    17794 2022-10-13 14:25:44.000000 drf-extra-fields-3.4.1/PKG-INFO
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-10-13 14:25:44.000000 drf-extra-fields-3.4.1/drf_extra_fields/
--rw-r--r--   0 apple      (501) staff       (20)     2131 2022-10-13 13:18:15.000000 drf-extra-fields-3.4.1/drf_extra_fields/geo_fields.py
--rw-r--r--   0 apple      (501) staff       (20)      115 2020-09-23 14:29:27.000000 drf-extra-fields-3.4.1/drf_extra_fields/compat.py
--rw-r--r--   0 apple      (501) staff       (20)    10934 2022-10-13 13:35:37.000000 drf-extra-fields-3.4.1/drf_extra_fields/fields.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-10-13 14:25:44.000000 drf-extra-fields-3.4.1/drf_extra_fields/runtests/
--rw-r--r--   0 apple      (501) staff       (20)        0 2019-10-24 13:30:17.000000 drf-extra-fields-3.4.1/drf_extra_fields/runtests/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     4308 2020-09-23 14:29:27.000000 drf-extra-fields-3.4.1/drf_extra_fields/runtests/settings.py
--rw-r--r--   0 apple      (501) staff       (20)     3814 2022-10-13 13:18:15.000000 drf-extra-fields-3.4.1/drf_extra_fields/relations.py
--rw-r--r--   0 apple      (501) staff       (20)        0 2019-10-24 13:30:17.000000 drf-extra-fields-3.4.1/drf_extra_fields/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    11324 2019-10-24 13:30:17.000000 drf-extra-fields-3.4.1/LICENSE
--rw-r--r--   0 apple      (501) staff       (20)       43 2020-12-03 19:07:10.000000 drf-extra-fields-3.4.1/requirements.txt
--rw-r--r--   0 apple      (501) staff       (20)       59 2022-03-04 09:31:30.000000 drf-extra-fields-3.4.1/MANIFEST.in
--rw-r--r--   0 apple      (501) staff       (20)    12903 2022-10-13 14:23:55.000000 drf-extra-fields-3.4.1/README.md
--rw-r--r--   0 apple      (501) staff       (20)     1664 2022-10-13 14:23:19.000000 drf-extra-fields-3.4.1/setup.py
--rw-r--r--   0 apple      (501) staff       (20)       38 2022-10-13 14:25:44.000000 drf-extra-fields-3.4.1/setup.cfg
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2022-10-13 14:25:44.000000 drf-extra-fields-3.4.1/drf_extra_fields.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)    17794 2022-10-13 14:25:43.000000 drf-extra-fields-3.4.1/drf_extra_fields.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      474 2022-10-13 14:25:43.000000 drf-extra-fields-3.4.1/drf_extra_fields.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)       73 2022-10-13 14:25:43.000000 drf-extra-fields-3.4.1/drf_extra_fields.egg-info/requires.txt
--rw-r--r--   0 apple      (501) staff       (20)       17 2022-10-13 14:25:43.000000 drf-extra-fields-3.4.1/drf_extra_fields.egg-info/top_level.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2022-10-13 14:25:43.000000 drf-extra-fields-3.4.1/drf_extra_fields.egg-info/dependency_links.txt
+drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-05-25 10:44:00.072485 drf-extra-fields-3.5.0/
+-rw-r--r--   0 furkan    (1000) furkan    (1000)    11324 2023-05-22 10:26:49.000000 drf-extra-fields-3.5.0/LICENSE
+-rw-r--r--   0 furkan    (1000) furkan    (1000)       59 2023-05-22 10:26:49.000000 drf-extra-fields-3.5.0/MANIFEST.in
+-rw-r--r--   0 furkan    (1000) furkan    (1000)    14197 2023-05-25 10:44:00.072485 drf-extra-fields-3.5.0/PKG-INFO
+-rw-r--r--   0 furkan    (1000) furkan    (1000)    13184 2023-05-25 10:42:58.000000 drf-extra-fields-3.5.0/README.md
+drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-05-25 10:44:00.072485 drf-extra-fields-3.5.0/drf_extra_fields/
+-rw-r--r--   0 furkan    (1000) furkan    (1000)        0 2023-05-22 10:26:49.000000 drf-extra-fields-3.5.0/drf_extra_fields/__init__.py
+-rw-r--r--   0 furkan    (1000) furkan    (1000)      115 2023-05-22 10:26:49.000000 drf-extra-fields-3.5.0/drf_extra_fields/compat.py
+-rw-r--r--   0 furkan    (1000) furkan    (1000)    10848 2023-05-24 10:36:09.000000 drf-extra-fields-3.5.0/drf_extra_fields/fields.py
+-rw-r--r--   0 furkan    (1000) furkan    (1000)     2131 2023-05-22 10:26:49.000000 drf-extra-fields-3.5.0/drf_extra_fields/geo_fields.py
+-rw-r--r--   0 furkan    (1000) furkan    (1000)     3814 2023-05-22 10:26:49.000000 drf-extra-fields-3.5.0/drf_extra_fields/relations.py
+drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-05-25 10:44:00.072485 drf-extra-fields-3.5.0/drf_extra_fields/runtests/
+-rw-r--r--   0 furkan    (1000) furkan    (1000)        0 2023-05-22 10:26:49.000000 drf-extra-fields-3.5.0/drf_extra_fields/runtests/__init__.py
+-rw-r--r--   0 furkan    (1000) furkan    (1000)     4308 2023-05-22 10:26:49.000000 drf-extra-fields-3.5.0/drf_extra_fields/runtests/settings.py
+drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-05-25 10:44:00.072485 drf-extra-fields-3.5.0/drf_extra_fields.egg-info/
+-rw-r--r--   0 furkan    (1000) furkan    (1000)    14197 2023-05-25 10:44:00.000000 drf-extra-fields-3.5.0/drf_extra_fields.egg-info/PKG-INFO
+-rw-r--r--   0 furkan    (1000) furkan    (1000)      550 2023-05-25 10:44:00.000000 drf-extra-fields-3.5.0/drf_extra_fields.egg-info/SOURCES.txt
+-rw-r--r--   0 furkan    (1000) furkan    (1000)        1 2023-05-25 10:44:00.000000 drf-extra-fields-3.5.0/drf_extra_fields.egg-info/dependency_links.txt
+-rw-r--r--   0 furkan    (1000) furkan    (1000)       89 2023-05-25 10:44:00.000000 drf-extra-fields-3.5.0/drf_extra_fields.egg-info/requires.txt
+-rw-r--r--   0 furkan    (1000) furkan    (1000)       17 2023-05-25 10:44:00.000000 drf-extra-fields-3.5.0/drf_extra_fields.egg-info/top_level.txt
+-rw-r--r--   0 furkan    (1000) furkan    (1000)       61 2023-05-23 10:44:44.000000 drf-extra-fields-3.5.0/requirements.txt
+-rw-r--r--   0 furkan    (1000) furkan    (1000)       38 2023-05-25 10:44:00.072485 drf-extra-fields-3.5.0/setup.cfg
+-rw-r--r--   0 furkan    (1000) furkan    (1000)     1714 2023-05-25 10:42:58.000000 drf-extra-fields-3.5.0/setup.py
+drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-05-25 10:44:00.072485 drf-extra-fields-3.5.0/tests/
+-rw-r--r--   0 furkan    (1000) furkan    (1000)    33952 2023-05-23 10:44:44.000000 drf-extra-fields-3.5.0/tests/test_fields.py
+-rw-r--r--   0 furkan    (1000) furkan    (1000)     2241 2023-05-22 10:26:49.000000 drf-extra-fields-3.5.0/tests/test_model_serializer.py
+-rw-r--r--   0 furkan    (1000) furkan    (1000)     5169 2023-05-22 10:26:49.000000 drf-extra-fields-3.5.0/tests/test_relations.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `drf-extra-fields-3.4.1/drf_extra_fields/geo_fields.py` & `drf-extra-fields-3.5.0/drf_extra_fields/geo_fields.py`

 * *Files identical despite different names*

### Comparing `drf-extra-fields-3.4.1/drf_extra_fields/fields.py` & `drf-extra-fields-3.5.0/drf_extra_fields/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import base64
 import binascii
-import imghdr
+import filetype
 import io
 import uuid
 
 from django.core.exceptions import ValidationError
 from django.core.files.uploadedfile import SimpleUploadedFile
 from django.utils.translation import gettext_lazy as _
 from rest_framework.fields import (
@@ -124,38 +124,34 @@
     A django-rest-framework field for handling image-uploads through raw post data.
     It uses base64 for en-/decoding the contents of the file.
     """
     ALLOWED_TYPES = (
         "jpeg",
         "jpg",
         "png",
-        "gif"
+        "gif",
+        "webp"
     )
     INVALID_FILE_MESSAGE = _("Please upload a valid image.")
     INVALID_TYPE_MESSAGE = _("The type of the image couldn't be determined.")
 
     def get_file_extension(self, filename, decoded_file):
-        try:
-            from PIL import Image
-        except ImportError:
-            raise ImportError("Pillow is not installed.")
-        extension = imghdr.what(filename, decoded_file)
-
-        # Try with PIL as fallback if format not detected due
-        # to bug in imghdr https://bugs.python.org/issue16512
+        extension = filetype.guess_extension(decoded_file)
         if extension is None:
             try:
+                # Try with PIL as fallback if format not detected
+                # with `filetype` module
+                from PIL import Image
                 image = Image.open(io.BytesIO(decoded_file))
-            except OSError:
+            except (ImportError, OSError):
                 raise ValidationError(self.INVALID_FILE_MESSAGE)
+            else:
+                extension = image.format.lower()
 
-            extension = image.format.lower()
-
-        extension = "jpg" if extension == "jpeg" else extension
-        return extension
+        return "jpg" if extension == "jpeg" else extension
 
 
 class HybridImageField(Base64ImageField):
     """
     A django-rest-framework field for handling image-uploads through
     raw post data, with a fallback to multipart form data.
     """
```

### Comparing `drf-extra-fields-3.4.1/drf_extra_fields/runtests/settings.py` & `drf-extra-fields-3.5.0/drf_extra_fields/runtests/settings.py`

 * *Files identical despite different names*

### Comparing `drf-extra-fields-3.4.1/drf_extra_fields/relations.py` & `drf-extra-fields-3.5.0/drf_extra_fields/relations.py`

 * *Files identical despite different names*

### Comparing `drf-extra-fields-3.4.1/LICENSE` & `drf-extra-fields-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-extra-fields-3.4.1/README.md` & `drf-extra-fields-3.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,20 @@
 [![Build Status](https://github.com/Hipo/drf-extra-fields/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/Hipo/drf-extra-fields/actions)
 [![codecov](https://codecov.io/gh/Hipo/drf-extra-fields/branch/master/graph/badge.svg)](https://codecov.io/gh/Hipo/drf-extra-fields)
 [![PyPI Version](https://img.shields.io/pypi/v/drf-extra-fields.svg)](https://pypi.org/project/drf-extra-fields)
 [![Python Versions](https://img.shields.io/pypi/pyversions/drf-extra-fields.svg)](https://pypi.org/project/drf-extra-fields)
 
 Latest Changes
 ==============
-- **v3.4.1**
-  - Modernize the code for `Python 3.7`.
+- **v3.5.0**
+  - Development environment fixes & improvements.
+  - Since `Python 3.6` support is ended, the codebase is refactored/modernized for `Python 3.7`.
+  - `WebP` is added to default `ALLOWED_TYPES` of the `Base64ImageField`.
+  - Deprecated `imghdr` library is replaced with `filetype`.
+  - Unintended `Pillow` dependency is removed.
 - **v3.4.0**
   - :warning: **BACKWARD INCOMPATIBLE** :warning:
     - Support for `Django 3.0` and `Django 3.1` is ended.
   - `Django 4.0` is now supported.
 - **v3.3.0**
   - :warning: **BACKWARD INCOMPATIBLE** :warning:
     - Support for `Python 3.6` is ended.
@@ -460,15 +464,15 @@
 $ pip install tox  # if not already installed
 $ tox
 ```
 
 Or, if you prefer using Docker (recommended):
 
 ```bash
-source tools/run_development.sh
+tools/run_development.sh
 tox
 ```
 
 **README**
 - Make sure that you add the documentation for the field added to README.md
```

### Comparing `drf-extra-fields-3.4.1/setup.py` & `drf-extra-fields-3.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     requirements = requirements_txt.read().strip().splitlines()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='drf-extra-fields',
-    version='3.4.1',
+    version='3.5.0',
     packages=['drf_extra_fields',
               'drf_extra_fields.runtests'],
     include_package_data=True,
     extras_require={
         "Base64ImageField": ["Pillow >= 6.2.1"],
     },
     license='Apache-2.0',
@@ -37,11 +37,12 @@
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     ],
 )
```

