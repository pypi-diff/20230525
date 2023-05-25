# Comparing `tmp/module_qc_database_tools-2.0.1.tar.gz` & `tmp/module_qc_database_tools-2.0.2rc1.tar.gz`

## Comparing `module_qc_database_tools-2.0.1.tar` & `module_qc_database_tools-2.0.2rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/.env.template
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/.gitlab-ci.yml
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/tbump.toml
--rwxr-xr-x   0        0        0      982 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/ci/pre-commit-update.sh
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/_version.py
--rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/chip_config_api.py
--rw-r--r--   0        0        0    15874 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/core.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/utils.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/cli/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/cli/__main__.py
--rw-r--r--   0        0        0     5043 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/cli/generate_yarr_config.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/cli/main.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/cli/register_component.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/data/componentConfigs.json
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/src/module_qc_database_tools/data/YARR/chip_template.json
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/tests/test_cli.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/tests/test_config_api.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/tests/test_package.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/tests/test_utils.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/.gitignore
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/README.md
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/.env.template
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/tbump.toml
+-rwxr-xr-x   0        0        0      982 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/ci/pre-commit-update.sh
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/src/module_qc_database_tools/__init__.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/src/module_qc_database_tools/_version.py
+-rw-r--r--   0        0        0    11207 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/src/module_qc_database_tools/chip_config_api.py
+-rw-r--r--   0        0        0    15874 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/src/module_qc_database_tools/core.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/src/module_qc_database_tools/utils.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/src/module_qc_database_tools/cli/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/src/module_qc_database_tools/cli/__main__.py
+-rw-r--r--   0        0        0     5043 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/src/module_qc_database_tools/cli/generate_yarr_config.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/src/module_qc_database_tools/cli/main.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/src/module_qc_database_tools/cli/register_component.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/src/module_qc_database_tools/data/componentConfigs.json
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/src/module_qc_database_tools/data/YARR/chip_template.json
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/tests/test_cli.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/tests/test_config_api.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/tests/test_package.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/tests/test_utils.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/.gitignore
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/README.md
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 module_qc_database_tools-2.0.2rc1/PKG-INFO
```

### Comparing `module_qc_database_tools-2.0.1/.gitlab-ci.yml` & `module_qc_database_tools-2.0.2rc1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.1/.pre-commit-config.yaml` & `module_qc_database_tools-2.0.2rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.1/tbump.toml` & `module_qc_database_tools-2.0.2rc1/tbump.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2232 2e30 2e31 220a 0a23 2045  t = "2.0.1"..# E
-00000020: 7861 6d70 6c65 206f 6620 6120 7365 6d76  xample of a semv
-00000030: 6572 2072 6567 6578 702e 0a23 204d 616b  er regexp..# Mak
-00000040: 6520 7375 7265 2074 6869 7320 6d61 7463  e sure this matc
-00000050: 6865 7320 6375 7272 656e 745f 7665 7273  hes current_vers
-00000060: 696f 6e20 6265 666f 7265 0a23 2075 7369  ion before.# usi
-00000070: 6e67 2074 6275 6d70 0a72 6567 6578 203d  ng tbump.regex =
-00000080: 2027 2727 0a20 2028 3f50 3c6d 616a 6f72   '''.  (?P<major
-00000090: 3e5c 642b 290a 2020 5c2e 0a20 2028 3f50  >\d+).  \..  (?P
-000000a0: 3c6d 696e 6f72 3e5c 642b 290a 2020 5c2e  <minor>\d+).  \.
-000000b0: 0a20 2028 3f50 3c70 6174 6368 3e5c 642b  .  (?P<patch>\d+
-000000c0: 290a 2020 2872 630a 2020 2020 283f 503c  ).  (rc.    (?P<
-000000d0: 6361 6e64 6964 6174 653e 5c64 2b29 0a20  candidate>\d+). 
-000000e0: 2029 3f0a 2020 2727 270a 0a5b 6769 745d   )?.  '''..[git]
-000000f0: 0a23 2054 6865 2063 7572 7265 6e74 2076  .# The current v
-00000100: 6572 7369 6f6e 2077 696c 6c20 6765 7420  ersion will get 
-00000110: 7570 6461 7465 6420 7768 656e 2074 6275  updated when tbu
-00000120: 6d70 2069 7320 7275 6e0a 6d65 7373 6167  mp is run.messag
-00000130: 655f 7465 6d70 6c61 7465 203d 2022 4275  e_template = "Bu
-00000140: 6d70 2076 6572 7369 6f6e 3a20 322e 302e  mp version: 2.0.
-00000150: 3120 e286 9220 7b6e 6577 5f76 6572 7369  1 ... {new_versi
-00000160: 6f6e 7d22 0a74 6167 5f74 656d 706c 6174  on}".tag_templat
-00000170: 6520 3d20 2276 7b6e 6577 5f76 6572 7369  e = "v{new_versi
-00000180: 6f6e 7d22 0a0a 2320 466f 7220 6561 6368  on}"..# For each
-00000190: 2066 696c 6520 746f 2070 6174 6368 2c20   file to patch, 
-000001a0: 6164 6420 6120 5b5b 6669 6c65 5d5d 2063  add a [[file]] c
-000001b0: 6f6e 6669 670a 2320 7365 6374 696f 6e20  onfig.# section 
-000001c0: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
-000001d0: 6174 6820 6f66 2074 6865 2066 696c 652c  ath of the file,
-000001e0: 2072 656c 6174 6976 6520 746f 2074 6865   relative to the
-000001f0: 0a23 2074 6275 6d70 2e74 6f6d 6c20 6c6f  .# tbump.toml lo
-00000200: 6361 7469 6f6e 2e0a 5b5b 6669 6c65 5d5d  cation..[[file]]
-00000210: 0a73 7263 203d 2022 7462 756d 702e 746f  .src = "tbump.to
-00000220: 6d6c 220a 2320 5265 7374 7269 6374 2073  ml".# Restrict s
-00000230: 6561 7263 6820 746f 206d 616b 6520 6974  earch to make it
-00000240: 2065 7870 6c69 6369 7420 7768 7920 7462   explicit why tb
-00000250: 756d 702e 746f 6d6c 0a23 2069 7320 6576  ump.toml.# is ev
-00000260: 656e 2069 6e63 6c75 6465 6420 6173 2061  en included as a
-00000270: 2066 696c 6520 746f 2062 756d 702c 2061   file to bump, a
-00000280: 7320 6974 2077 696c 6c20 6765 740a 2320  s it will get.# 
-00000290: 6974 7320 7665 7273 696f 6e2e 6375 7272  its version.curr
-000002a0: 656e 7420 6174 7472 6962 7574 6520 6275  ent attribute bu
-000002b0: 6d70 6564 2061 6e79 7761 792e 0a73 6561  mped anyway..sea
-000002c0: 7263 6820 3d20 2242 756d 7020 7665 7273  rch = "Bump vers
-000002d0: 696f 6e3a 207b 6375 7272 656e 745f 7665  ion: {current_ve
-000002e0: 7273 696f 6e7d 20e2 8692 2022 0a0a 5b5b  rsion} ... "..[[
-000002f0: 6669 6c65 5d5d 0a73 7263 203d 2022 5245  file]].src = "RE
-00000300: 4144 4d45 2e6d 6422 0a0a 5b5b 6669 656c  ADME.md"..[[fiel
-00000310: 645d 5d0a 2320 7468 6520 6e61 6d65 206f  d]].# the name o
-00000320: 6620 7468 6520 6669 656c 640a 6e61 6d65  f the field.name
-00000330: 203d 2022 6361 6e64 6964 6174 6522 0a23   = "candidate".#
-00000340: 2074 6865 2064 6566 6175 6c74 2076 616c   the default val
-00000350: 7565 2074 6f20 7573 652c 2069 6620 7468  ue to use, if th
-00000360: 6572 6520 6973 206e 6f20 6d61 7463 680a  ere is no match.
-00000370: 6465 6661 756c 7420 3d20 2222 0a         default = "".
+00000010: 7420 3d20 2232 2e30 2e32 7263 3122 0a0a  t = "2.0.2rc1"..
+00000020: 2320 4578 616d 706c 6520 6f66 2061 2073  # Example of a s
+00000030: 656d 7665 7220 7265 6765 7870 2e0a 2320  emver regexp..# 
+00000040: 4d61 6b65 2073 7572 6520 7468 6973 206d  Make sure this m
+00000050: 6174 6368 6573 2063 7572 7265 6e74 5f76  atches current_v
+00000060: 6572 7369 6f6e 2062 6566 6f72 650a 2320  ersion before.# 
+00000070: 7573 696e 6720 7462 756d 700a 7265 6765  using tbump.rege
+00000080: 7820 3d20 2727 270a 2020 283f 503c 6d61  x = '''.  (?P<ma
+00000090: 6a6f 723e 5c64 2b29 0a20 205c 2e0a 2020  jor>\d+).  \..  
+000000a0: 283f 503c 6d69 6e6f 723e 5c64 2b29 0a20  (?P<minor>\d+). 
+000000b0: 205c 2e0a 2020 283f 503c 7061 7463 683e   \..  (?P<patch>
+000000c0: 5c64 2b29 0a20 2028 7263 0a20 2020 2028  \d+).  (rc.    (
+000000d0: 3f50 3c63 616e 6469 6461 7465 3e5c 642b  ?P<candidate>\d+
+000000e0: 290a 2020 293f 0a20 2027 2727 0a0a 5b67  ).  )?.  '''..[g
+000000f0: 6974 5d0a 2320 5468 6520 6375 7272 656e  it].# The curren
+00000100: 7420 7665 7273 696f 6e20 7769 6c6c 2067  t version will g
+00000110: 6574 2075 7064 6174 6564 2077 6865 6e20  et updated when 
+00000120: 7462 756d 7020 6973 2072 756e 0a6d 6573  tbump is run.mes
+00000130: 7361 6765 5f74 656d 706c 6174 6520 3d20  sage_template = 
+00000140: 2242 756d 7020 7665 7273 696f 6e3a 2032  "Bump version: 2
+00000150: 2e30 2e32 7263 3120 e286 9220 7b6e 6577  .0.2rc1 ... {new
+00000160: 5f76 6572 7369 6f6e 7d22 0a74 6167 5f74  _version}".tag_t
+00000170: 656d 706c 6174 6520 3d20 2276 7b6e 6577  emplate = "v{new
+00000180: 5f76 6572 7369 6f6e 7d22 0a0a 2320 466f  _version}"..# Fo
+00000190: 7220 6561 6368 2066 696c 6520 746f 2070  r each file to p
+000001a0: 6174 6368 2c20 6164 6420 6120 5b5b 6669  atch, add a [[fi
+000001b0: 6c65 5d5d 2063 6f6e 6669 670a 2320 7365  le]] config.# se
+000001c0: 6374 696f 6e20 636f 6e74 6169 6e69 6e67  ction containing
+000001d0: 2074 6865 2070 6174 6820 6f66 2074 6865   the path of the
+000001e0: 2066 696c 652c 2072 656c 6174 6976 6520   file, relative 
+000001f0: 746f 2074 6865 0a23 2074 6275 6d70 2e74  to the.# tbump.t
+00000200: 6f6d 6c20 6c6f 6361 7469 6f6e 2e0a 5b5b  oml location..[[
+00000210: 6669 6c65 5d5d 0a73 7263 203d 2022 7462  file]].src = "tb
+00000220: 756d 702e 746f 6d6c 220a 2320 5265 7374  ump.toml".# Rest
+00000230: 7269 6374 2073 6561 7263 6820 746f 206d  rict search to m
+00000240: 616b 6520 6974 2065 7870 6c69 6369 7420  ake it explicit 
+00000250: 7768 7920 7462 756d 702e 746f 6d6c 0a23  why tbump.toml.#
+00000260: 2069 7320 6576 656e 2069 6e63 6c75 6465   is even include
+00000270: 6420 6173 2061 2066 696c 6520 746f 2062  d as a file to b
+00000280: 756d 702c 2061 7320 6974 2077 696c 6c20  ump, as it will 
+00000290: 6765 740a 2320 6974 7320 7665 7273 696f  get.# its versio
+000002a0: 6e2e 6375 7272 656e 7420 6174 7472 6962  n.current attrib
+000002b0: 7574 6520 6275 6d70 6564 2061 6e79 7761  ute bumped anywa
+000002c0: 792e 0a73 6561 7263 6820 3d20 2242 756d  y..search = "Bum
+000002d0: 7020 7665 7273 696f 6e3a 207b 6375 7272  p version: {curr
+000002e0: 656e 745f 7665 7273 696f 6e7d 20e2 8692  ent_version} ...
+000002f0: 2022 0a0a 5b5b 6669 6c65 5d5d 0a73 7263   "..[[file]].src
+00000300: 203d 2022 5245 4144 4d45 2e6d 6422 0a0a   = "README.md"..
+00000310: 5b5b 6669 656c 645d 5d0a 2320 7468 6520  [[field]].# the 
+00000320: 6e61 6d65 206f 6620 7468 6520 6669 656c  name of the fiel
+00000330: 640a 6e61 6d65 203d 2022 6361 6e64 6964  d.name = "candid
+00000340: 6174 6522 0a23 2074 6865 2064 6566 6175  ate".# the defau
+00000350: 6c74 2076 616c 7565 2074 6f20 7573 652c  lt value to use,
+00000360: 2069 6620 7468 6572 6520 6973 206e 6f20   if there is no 
+00000370: 6d61 7463 680a 6465 6661 756c 7420 3d20  match.default = 
+00000380: 2222 0a                                  "".
```

### Comparing `module_qc_database_tools-2.0.1/ci/pre-commit-update.sh` & `module_qc_database_tools-2.0.2rc1/ci/pre-commit-update.sh`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.1/src/module_qc_database_tools/chip_config_api.py` & `module_qc_database_tools-2.0.2rc1/src/module_qc_database_tools/chip_config_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,14 +283,16 @@
     def get_revision_history(self, config_id):
         """
         Gets the revision history for this object.
         """
         config = self.database.fe_configs.find_one({"_id": ObjectId(config_id)})
 
         revision = config.get("current_revision_id")
+        if revision is None:
+            return []
 
         revision_history = [str(revision)]
 
         while True:
             revision_id = self._get_prev_commit(revision_history[-1])
 
             if revision_id is None:
```

### Comparing `module_qc_database_tools-2.0.1/src/module_qc_database_tools/core.py` & `module_qc_database_tools-2.0.2rc1/src/module_qc_database_tools/core.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.1/src/module_qc_database_tools/utils.py` & `module_qc_database_tools-2.0.2rc1/src/module_qc_database_tools/utils.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.1/src/module_qc_database_tools/cli/generate_yarr_config.py` & `module_qc_database_tools-2.0.2rc1/src/module_qc_database_tools/cli/generate_yarr_config.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.1/src/module_qc_database_tools/cli/main.py` & `module_qc_database_tools-2.0.2rc1/src/module_qc_database_tools/cli/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.1/src/module_qc_database_tools/cli/register_component.py` & `module_qc_database_tools-2.0.2rc1/src/module_qc_database_tools/cli/register_component.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.1/src/module_qc_database_tools/data/componentConfigs.json` & `module_qc_database_tools-2.0.2rc1/src/module_qc_database_tools/data/componentConfigs.json`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.1/tests/test_cli.py` & `module_qc_database_tools-2.0.2rc1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.1/tests/test_config_api.py` & `module_qc_database_tools-2.0.2rc1/tests/test_config_api.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.1/.gitignore` & `module_qc_database_tools-2.0.2rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.1/README.md` & `module_qc_database_tools-2.0.2rc1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Module QC Database Tools v2.0.1
+# Module QC Database Tools v2.0.2rc1
 
 The package to regisiter ITkPixV1.1 modules, and generate YARR configs from ITk
 production database using `itkdb` API.
 
 ## Set-Up and First-time Installation
 
 A minimum of python version 3.7+ is required.
```

### Comparing `module_qc_database_tools-2.0.1/pyproject.toml` & `module_qc_database_tools-2.0.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.0.1/PKG-INFO` & `module_qc_database_tools-2.0.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-qc-database-tools
-Version: 2.0.1
+Version: 2.0.2rc1
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
 
-# Module QC Database Tools v2.0.1
+# Module QC Database Tools v2.0.2rc1
 
 The package to regisiter ITkPixV1.1 modules, and generate YARR configs from ITk
 production database using `itkdb` API.
 
 ## Set-Up and First-time Installation
 
 A minimum of python version 3.7+ is required.
```

