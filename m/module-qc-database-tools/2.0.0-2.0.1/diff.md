# Comparing `tmp/module_qc_database_tools-2.0.0.tar.gz` & `tmp/module_qc_database_tools-2.0.1.tar.gz`

## Comparing `module_qc_database_tools-2.0.0.tar` & `module_qc_database_tools-2.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/.env.template
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/tbump.toml
--rwxr-xr-x   0        0        0      982 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/ci/pre-commit-update.sh
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/src/module_qc_database_tools/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/src/module_qc_database_tools/_version.py
--rw-r--r--   0        0        0    11136 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/src/module_qc_database_tools/chip_config_api.py
--rw-r--r--   0        0        0    15874 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/src/module_qc_database_tools/core.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/src/module_qc_database_tools/utils.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/src/module_qc_database_tools/cli/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/src/module_qc_database_tools/cli/__main__.py
--rw-r--r--   0        0        0     5043 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/src/module_qc_database_tools/cli/generate_yarr_config.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/src/module_qc_database_tools/cli/main.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/src/module_qc_database_tools/cli/register_component.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/src/module_qc_database_tools/data/componentConfigs.json
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/src/module_qc_database_tools/data/YARR/chip_template.json
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/tests/test_cli.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/tests/test_config_api.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/tests/test_package.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/tests/test_utils.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/.gitignore
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/README.md
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/.env.template
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/tbump.toml
+-rwxr-xr-x   0        0        0      982 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/ci/pre-commit-update.sh
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/_version.py
+-rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/chip_config_api.py
+-rw-r--r--   0        0        0    15874 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/core.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/utils.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/cli/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/cli/__main__.py
+-rw-r--r--   0        0        0     5043 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/cli/generate_yarr_config.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/cli/main.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/cli/register_component.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/data/componentConfigs.json
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/data/YARR/chip_template.json
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/tests/test_cli.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/tests/test_config_api.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/tests/test_package.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/tests/test_utils.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/.gitignore
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/README.md
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/PKG-INFO
```

### Comparing `module_qc_database_tools-2.0.0/.gitlab-ci.yml` & `module_qc_database_tools-2.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.0/.pre-commit-config.yaml` & `module_qc_database_tools-2.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.0/tbump.toml` & `module_qc_database_tools-2.0.1/tbump.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2232 2e30 2e30 220a 0a23 2045  t = "2.0.0"..# E
+00000010: 7420 3d20 2232 2e30 2e31 220a 0a23 2045  t = "2.0.1"..# E
 00000020: 7861 6d70 6c65 206f 6620 6120 7365 6d76  xample of a semv
 00000030: 6572 2072 6567 6578 702e 0a23 204d 616b  er regexp..# Mak
 00000040: 6520 7375 7265 2074 6869 7320 6d61 7463  e sure this matc
 00000050: 6865 7320 6375 7272 656e 745f 7665 7273  hes current_vers
 00000060: 696f 6e20 6265 666f 7265 0a23 2075 7369  ion before.# usi
 00000070: 6e67 2074 6275 6d70 0a72 6567 6578 203d  ng tbump.regex =
 00000080: 2027 2727 0a20 2028 3f50 3c6d 616a 6f72   '''.  (?P<major
@@ -15,15 +15,15 @@
 000000e0: 2029 3f0a 2020 2727 270a 0a5b 6769 745d   )?.  '''..[git]
 000000f0: 0a23 2054 6865 2063 7572 7265 6e74 2076  .# The current v
 00000100: 6572 7369 6f6e 2077 696c 6c20 6765 7420  ersion will get 
 00000110: 7570 6461 7465 6420 7768 656e 2074 6275  updated when tbu
 00000120: 6d70 2069 7320 7275 6e0a 6d65 7373 6167  mp is run.messag
 00000130: 655f 7465 6d70 6c61 7465 203d 2022 4275  e_template = "Bu
 00000140: 6d70 2076 6572 7369 6f6e 3a20 322e 302e  mp version: 2.0.
-00000150: 3020 e286 9220 7b6e 6577 5f76 6572 7369  0 ... {new_versi
+00000150: 3120 e286 9220 7b6e 6577 5f76 6572 7369  1 ... {new_versi
 00000160: 6f6e 7d22 0a74 6167 5f74 656d 706c 6174  on}".tag_templat
 00000170: 6520 3d20 2276 7b6e 6577 5f76 6572 7369  e = "v{new_versi
 00000180: 6f6e 7d22 0a0a 2320 466f 7220 6561 6368  on}"..# For each
 00000190: 2066 696c 6520 746f 2070 6174 6368 2c20   file to patch, 
 000001a0: 6164 6420 6120 5b5b 6669 6c65 5d5d 2063  add a [[file]] c
 000001b0: 6f6e 6669 670a 2320 7365 6374 696f 6e20  onfig.# section 
 000001c0: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
```

### Comparing `module_qc_database_tools-2.0.0/ci/pre-commit-update.sh` & `module_qc_database_tools-2.0.1/ci/pre-commit-update.sh`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.0/src/module_qc_database_tools/chip_config_api.py` & `module_qc_database_tools-2.0.1/src/module_qc_database_tools/chip_config_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
 
         return str(revision_id)
 
     def _get_prev_commit(self, revision_id):
         revision = self.database.fe_config_revision.find_one(
             {"_id": ObjectId(revision_id)}
         )
-        return str(revision.get("parent_revision_id"))
+        return str(revision.get("parent_revision_id")) if revision else None
 
     def get_revision_id(self, config_id, tag="HEAD"):
         """
         Get the revision id for the config id and tag.
         """
         config = self.database.fe_configs.find_one({"_id": ObjectId(config_id)})
         revision_id = str(config.get("current_revision_id"))
@@ -289,15 +289,15 @@
         revision = config.get("current_revision_id")
 
         revision_history = [str(revision)]
 
         while True:
             revision_id = self._get_prev_commit(revision_history[-1])
 
-            if revision_id == "None":
+            if revision_id is None:
                 break
 
             revision_history += [revision_id]
 
         return revision_history
 
     def get_log(self, config_id, depth=10):
```

### Comparing `module_qc_database_tools-2.0.0/src/module_qc_database_tools/core.py` & `module_qc_database_tools-2.0.1/src/module_qc_database_tools/core.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.0/src/module_qc_database_tools/utils.py` & `module_qc_database_tools-2.0.1/src/module_qc_database_tools/utils.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.0/src/module_qc_database_tools/cli/generate_yarr_config.py` & `module_qc_database_tools-2.0.1/src/module_qc_database_tools/cli/generate_yarr_config.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.0/src/module_qc_database_tools/cli/main.py` & `module_qc_database_tools-2.0.1/src/module_qc_database_tools/cli/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.0/src/module_qc_database_tools/cli/register_component.py` & `module_qc_database_tools-2.0.1/src/module_qc_database_tools/cli/register_component.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.0/src/module_qc_database_tools/data/componentConfigs.json` & `module_qc_database_tools-2.0.1/src/module_qc_database_tools/data/componentConfigs.json`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.0/tests/test_cli.py` & `module_qc_database_tools-2.0.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.0/tests/test_config_api.py` & `module_qc_database_tools-2.0.1/tests/test_config_api.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.0/.gitignore` & `module_qc_database_tools-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.0/README.md` & `module_qc_database_tools-2.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Module QC Database Tools v2.0.0
+# Module QC Database Tools v2.0.1
 
 The package to regisiter ITkPixV1.1 modules, and generate YARR configs from ITk
 production database using `itkdb` API.
 
 ## Set-Up and First-time Installation
 
 A minimum of python version 3.7+ is required.
```

### Comparing `module_qc_database_tools-2.0.0/pyproject.toml` & `module_qc_database_tools-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.0/PKG-INFO` & `module_qc_database_tools-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-qc-database-tools
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python wrapper to interface with LocalDB and Production DB for common tasks for pixel modules.
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools
 Author-email: Jay Chan <jay.chan@cern.ch>
 Maintainer-email: Giordon Stark <kratsg@gmail.com>, Elisabetta Pianori <elisabetta.pianori@cern.ch>, Lingxin Meng <lingxin.meng@cern.ch>
 Classifier: Development Status :: 1 - Planning
@@ -29,15 +29,15 @@
 Requires-Dist: jsondiff
 Requires-Dist: pandas
 Requires-Dist: pymongo
 Requires-Dist: rich
 Requires-Dist: typer
 Description-Content-Type: text/markdown
 
-# Module QC Database Tools v2.0.0
+# Module QC Database Tools v2.0.1
 
 The package to regisiter ITkPixV1.1 modules, and generate YARR configs from ITk
 production database using `itkdb` API.
 
 ## Set-Up and First-time Installation
 
 A minimum of python version 3.7+ is required.
```

