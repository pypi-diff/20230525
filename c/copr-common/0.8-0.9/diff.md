# Comparing `tmp/copr-common-0.8.tar.gz` & `tmp/copr-common-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/copr-common-0.8.tar", last modified: Wed Jun 10 19:46:23 2020, max compression
+gzip compressed data, was "dist/copr-common-0.9.tar", last modified: Fri Nov 13 13:33:28 2020, max compression
```

## Comparing `copr-common-0.8.tar` & `copr-common-0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2020-06-10 19:46:23.581407 copr-common-0.8/
--rw-rw-r--   0 twine    (17125) twine    (17125)      528 2020-06-10 19:46:23.581407 copr-common-0.8/PKG-INFO
-drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2020-06-10 19:46:23.577407 copr-common-0.8/copr_common/
--rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-07-17 08:59:09.000000 copr-common-0.8/copr_common/__init__.py
--rw-rw-r--   0 twine    (17125) twine    (17125)     3999 2020-06-10 19:42:40.000000 copr-common-0.8/copr_common/enums.py
--rw-rw-r--   0 twine    (17125) twine    (17125)      864 2019-07-17 08:59:09.000000 copr-common-0.8/copr_common/rpm.py
-drwxrwxr-x   0 twine    (17125) twine    (17125)        0 2020-06-10 19:46:23.580407 copr-common-0.8/copr_common.egg-info/
--rw-rw-r--   0 twine    (17125) twine    (17125)      528 2020-06-10 19:46:23.000000 copr-common-0.8/copr_common.egg-info/PKG-INFO
--rw-rw-r--   0 twine    (17125) twine    (17125)      246 2020-06-10 19:46:23.000000 copr-common-0.8/copr_common.egg-info/SOURCES.txt
--rw-rw-r--   0 twine    (17125) twine    (17125)        1 2020-06-10 19:46:23.000000 copr-common-0.8/copr_common.egg-info/dependency_links.txt
--rw-rw-r--   0 twine    (17125) twine    (17125)        1 2020-06-10 19:46:23.000000 copr-common-0.8/copr_common.egg-info/not-zip-safe
--rw-rw-r--   0 twine    (17125) twine    (17125)       12 2020-06-10 19:46:23.000000 copr-common-0.8/copr_common.egg-info/top_level.txt
--rw-rw-r--   0 twine    (17125) twine    (17125)       38 2020-06-10 19:46:23.581407 copr-common-0.8/setup.cfg
--rw-rw-r--   0 twine    (17125) twine    (17125)      839 2020-06-10 19:42:40.000000 copr-common-0.8/setup.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2020-11-13 13:33:28.393251 copr-common-0.9/
+-rw-r--r--   0 twine    (17125) twine    (17125)      528 2020-11-13 13:33:28.393251 copr-common-0.9/PKG-INFO
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2020-11-13 13:33:28.392251 copr-common-0.9/copr_common/
+-rw-rw-r--   0 twine    (17125) twine    (17125)        0 2019-07-17 08:59:09.000000 copr-common-0.9/copr_common/__init__.py
+-rw-r--r--   0 twine    (17125) twine    (17125)     4227 2020-11-13 13:32:58.000000 copr-common-0.9/copr_common/enums.py
+-rw-rw-r--   0 twine    (17125) twine    (17125)      864 2019-07-17 08:59:09.000000 copr-common-0.9/copr_common/rpm.py
+drwxr-xr-x   0 twine    (17125) twine    (17125)        0 2020-11-13 13:33:28.393251 copr-common-0.9/copr_common.egg-info/
+-rw-rw-r--   0 twine    (17125) twine    (17125)      528 2020-11-13 13:33:28.000000 copr-common-0.9/copr_common.egg-info/PKG-INFO
+-rw-rw-r--   0 twine    (17125) twine    (17125)      246 2020-11-13 13:33:28.000000 copr-common-0.9/copr_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 twine    (17125) twine    (17125)        1 2020-11-13 13:33:28.000000 copr-common-0.9/copr_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 twine    (17125) twine    (17125)        1 2020-06-10 19:46:23.000000 copr-common-0.9/copr_common.egg-info/not-zip-safe
+-rw-rw-r--   0 twine    (17125) twine    (17125)       12 2020-11-13 13:33:28.000000 copr-common-0.9/copr_common.egg-info/top_level.txt
+-rw-r--r--   0 twine    (17125) twine    (17125)       38 2020-11-13 13:33:28.393251 copr-common-0.9/setup.cfg
+-rw-r--r--   0 twine    (17125) twine    (17125)      839 2020-11-13 13:32:58.000000 copr-common-0.9/setup.py
```

### Comparing `copr-common-0.8/PKG-INFO` & `copr-common-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: copr-common
-Version: 0.8
+Version: 0.9
 Summary: Common python code used by Copr.
 Home-page: https://pagure.io/copr/copr
 Author: Dominik Turecek
 Author-email: dturecek@redhat.com
 License: GPLv2+
 Description: COPR is lightweight build system. It allows you to create new project
         in WebUI, and submit new builds and COPR will create yum repository from latest builds.
```

### Comparing `copr-common-0.8/copr_common/enums.py` & `copr-common-0.9/copr_common/enums.py`

 * *Files 19% similar despite different names*

```diff
@@ -93,28 +93,36 @@
         "importing": 7,  # SRPM is being imported into dist-git
         "forked": 8,     # build(-chroot) was forked
         "waiting": 9,    # build(-chroot) is waiting for something else to finish
         "unknown": 1000, # undefined
     }
 
 
+def _filtered_status_enum(keys):
+    new_values = {}
+    for key, value in StatusEnum.vals.items():
+        if key in keys:
+            new_values[key] = value
+    return new_values
+
+
 class ModuleStatusEnum(StatusEnum):
-    vals = {k: v for k, v in StatusEnum.vals.items()
-            if k in ["canceled", "running", "starting", "pending",
-                      "failed", "succeeded", "waiting", "unknown"]}
+    vals = _filtered_status_enum(["canceled", "running", "starting", "pending",
+                                  "failed", "succeeded", "waiting", "unknown"])
 
 
 class BuildSourceEnum(with_metaclass(EnumType, object)):
     vals = {"unset": 0,
             "link": 1,  # url
             "upload": 2,  # pkg, tmp, url
             "pypi": 5, # package_name, version, python_versions
             "rubygems": 6, # gem_name
             "scm": 8, # type, clone_url, committish, subdirectory, spec, srpm_build_method
             "custom": 9, # user-provided script to build sources
+            "distgit": 10, # distgit_instance, package_name, committish
            }
 
 
 class FailTypeEnum(with_metaclass(EnumType, object)):
     vals = {"unset": 0,
             # General errors mixed with errors for SRPM URL/upload:
             "unknown_error": 1,
```

### Comparing `copr-common-0.8/copr_common/rpm.py` & `copr-common-0.9/copr_common/rpm.py`

 * *Files identical despite different names*

### Comparing `copr-common-0.8/copr_common.egg-info/PKG-INFO` & `copr-common-0.9/copr_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: copr-common
-Version: 0.8
+Version: 0.9
 Summary: Common python code used by Copr.
 Home-page: https://pagure.io/copr/copr
 Author: Dominik Turecek
 Author-email: dturecek@redhat.com
 License: GPLv2+
 Description: COPR is lightweight build system. It allows you to create new project
         in WebUI, and submit new builds and COPR will create yum repository from latest builds.
```

### Comparing `copr-common-0.8/setup.py` & `copr-common-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 __author__ = "Dominik Turecek"
 __author_email__ = "dturecek@redhat.com"
 __url__ = "https://pagure.io/copr/copr"
 
 
 setup(
     name='copr-common',
-    version="0.8",
+    version="0.9",
     description=__description__,
     long_description=long_description,
     author=__author__,
     author_email=__author_email__,
     url=__url__,
     license='GPLv2+',
     packages=['copr_common'],
```

