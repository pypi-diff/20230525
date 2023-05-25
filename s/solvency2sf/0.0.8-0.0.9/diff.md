# Comparing `tmp/solvency2sf-0.0.8.tar.gz` & `tmp/solvency2sf-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solvency2sf-0.0.8.tar", last modified: Mon Aug 16 15:17:17 2021, max compression
+gzip compressed data, was "solvency2sf-0.0.9.tar", last modified: Fri Oct 29 08:04:35 2021, max compression
```

## Comparing `solvency2sf-0.0.8.tar` & `solvency2sf-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 15:17:17.729810 solvency2sf-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-08-16 15:17:09.000000 solvency2sf-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1974 2021-08-16 15:17:17.729810 solvency2sf-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2021-08-16 15:17:09.000000 solvency2sf-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-16 15:17:17.729810 solvency2sf-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2021-08-16 15:17:09.000000 solvency2sf-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 15:17:17.725810 solvency2sf-0.0.8/solvency2sf/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-08-16 15:17:09.000000 solvency2sf-0.0.8/solvency2sf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2021-08-16 15:17:09.000000 solvency2sf-0.0.8/solvency2sf/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1926 2021-08-16 15:17:09.000000 solvency2sf-0.0.8/solvency2sf/default.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 15:17:17.725810 solvency2sf-0.0.8/solvency2sf/mcr/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-16 15:17:09.000000 solvency2sf-0.0.8/solvency2sf/mcr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2682 2021-08-16 15:17:09.000000 solvency2sf-0.0.8/solvency2sf/mcr/mcr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1455 2021-08-16 15:17:09.000000 solvency2sf-0.0.8/solvency2sf/operational.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 15:17:17.725810 solvency2sf-0.0.8/solvency2sf/scr_nl/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-16 15:17:09.000000 solvency2sf-0.0.8/solvency2sf/scr_nl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 15:17:17.725810 solvency2sf-0.0.8/solvency2sf/scr_nl/cat/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-16 15:17:09.000000 solvency2sf-0.0.8/solvency2sf/scr_nl/cat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 15:17:17.725810 solvency2sf-0.0.8/solvency2sf/scr_nl/cat/manmade/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-16 15:17:09.000000 solvency2sf-0.0.8/solvency2sf/scr_nl/cat/manmade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7435 2021-08-16 15:17:09.000000 solvency2sf-0.0.8/solvency2sf/scr_nl/cat/manmade/manmade.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 15:17:17.729810 solvency2sf-0.0.8/solvency2sf/scr_nl/cat/natcat_eur/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-16 15:17:09.000000 solvency2sf-0.0.8/solvency2sf/scr_nl/cat/natcat_eur/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11062 2021-08-16 15:17:09.000000 solvency2sf-0.0.8/solvency2sf/scr_nl/cat/natcat_eur/natcat_eur.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 15:17:17.729810 solvency2sf-0.0.8/solvency2sf/scr_nl/premres/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-16 15:17:09.000000 solvency2sf-0.0.8/solvency2sf/scr_nl/premres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3707 2021-08-16 15:17:09.000000 solvency2sf-0.0.8/solvency2sf/scr_nl/premres/premres.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-16 15:17:17.725810 solvency2sf-0.0.8/solvency2sf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1974 2021-08-16 15:17:17.000000 solvency2sf-0.0.8/solvency2sf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      674 2021-08-16 15:17:17.000000 solvency2sf-0.0.8/solvency2sf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-16 15:17:17.000000 solvency2sf-0.0.8/solvency2sf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-08-16 15:17:17.000000 solvency2sf-0.0.8/solvency2sf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-08-16 15:17:17.000000 solvency2sf-0.0.8/solvency2sf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-29 08:04:35.675390 solvency2sf-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-10-29 08:04:25.000000 solvency2sf-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1721 2021-10-29 08:04:35.675390 solvency2sf-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1057 2021-10-29 08:04:25.000000 solvency2sf-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-29 08:04:35.675390 solvency2sf-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1216 2021-10-29 08:04:25.000000 solvency2sf-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-29 08:04:35.675390 solvency2sf-0.0.9/solvency2sf/
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2021-10-29 08:04:25.000000 solvency2sf-0.0.9/solvency2sf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1046 2021-10-29 08:04:25.000000 solvency2sf-0.0.9/solvency2sf/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1926 2021-10-29 08:04:25.000000 solvency2sf-0.0.9/solvency2sf/default.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-29 08:04:35.675390 solvency2sf-0.0.9/solvency2sf/mcr/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-29 08:04:25.000000 solvency2sf-0.0.9/solvency2sf/mcr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3047 2021-10-29 08:04:25.000000 solvency2sf-0.0.9/solvency2sf/mcr/mcr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1455 2021-10-29 08:04:25.000000 solvency2sf-0.0.9/solvency2sf/operational.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-29 08:04:35.675390 solvency2sf-0.0.9/solvency2sf/scr_nl/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-29 08:04:25.000000 solvency2sf-0.0.9/solvency2sf/scr_nl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-29 08:04:35.675390 solvency2sf-0.0.9/solvency2sf/scr_nl/cat/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-29 08:04:25.000000 solvency2sf-0.0.9/solvency2sf/scr_nl/cat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-29 08:04:35.675390 solvency2sf-0.0.9/solvency2sf/scr_nl/cat/manmade/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-29 08:04:25.000000 solvency2sf-0.0.9/solvency2sf/scr_nl/cat/manmade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7435 2021-10-29 08:04:25.000000 solvency2sf-0.0.9/solvency2sf/scr_nl/cat/manmade/manmade.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-29 08:04:35.675390 solvency2sf-0.0.9/solvency2sf/scr_nl/cat/natcat_eur/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-29 08:04:25.000000 solvency2sf-0.0.9/solvency2sf/scr_nl/cat/natcat_eur/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11062 2021-10-29 08:04:25.000000 solvency2sf-0.0.9/solvency2sf/scr_nl/cat/natcat_eur/natcat_eur.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-29 08:04:35.675390 solvency2sf-0.0.9/solvency2sf/scr_nl/premres/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-29 08:04:25.000000 solvency2sf-0.0.9/solvency2sf/scr_nl/premres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3707 2021-10-29 08:04:25.000000 solvency2sf-0.0.9/solvency2sf/scr_nl/premres/premres.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-29 08:04:35.675390 solvency2sf-0.0.9/solvency2sf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1721 2021-10-29 08:04:35.000000 solvency2sf-0.0.9/solvency2sf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      674 2021-10-29 08:04:35.000000 solvency2sf-0.0.9/solvency2sf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-29 08:04:35.000000 solvency2sf-0.0.9/solvency2sf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2021-10-29 08:04:35.000000 solvency2sf-0.0.9/solvency2sf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-10-29 08:04:35.000000 solvency2sf-0.0.9/solvency2sf.egg-info/top_level.txt
```

### Comparing `solvency2sf-0.0.8/LICENSE` & `solvency2sf-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `solvency2sf-0.0.8/PKG-INFO` & `solvency2sf-0.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 Metadata-Version: 2.1
 Name: solvency2sf
-Version: 0.0.8
+Version: 0.0.9
 Summary: Solvency 2 Standard Formula
 Home-page: https://github.com/pdavidsonFIA/solvency2sf
 Author: Peter Davidson
 Author-email: peterjd41@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pdavidsonFIA/solvency2sf/issues
-Description: # solvency2sf
-        Solvency 2 Standard Formula
-        
-        Pandas/numpy implementation of the standard formula for non-life.
-        
-        The calculation logic generally mimics the calculations within the standard formula guidance provided by Lloyd's.
-        https://www.lloyds.com/resources-and-services/capital-and-reserving/capital-guidance/standard-formula-scr
-        
-        The template populated with sample data is saved under /tests
-        
-        Provides:
-        - scr:
-          - non-life
-            - premium and reserve
-            - lapse
-            - catastrophy
-              - natcat euro
-              - man-made
-          - default
-          - bscr
-          - op
-          - scr
-        - mcr
-        
-        Structure:
-        - Each scr sub-module is within its own package.
-        - Any required parameters are typically stored in CSV files in the same package 
-        - Functions often return tuples. The first item will be a numerical result, the subsequent items data frames containing additional breakdown to debug and support QRT completion.
-        
-        Known limitations:
-        - only gross scr calculated in natcat: approach for reinsurance may be very company specific.
-        - not all nat-cat modules included (yet)
-        - default quite simple
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Financial and Insurance Industry
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# solvency2sf
+Solvency 2 Standard Formula
+
+Pandas/numpy implementation of the standard formula for non-life.
+
+The calculation logic generally mimics the calculations within the standard formula guidance provided by Lloyd's.
+https://www.lloyds.com/resources-and-services/capital-and-reserving/capital-guidance/standard-formula-scr
+
+The template populated with sample data is saved under /tests
+
+Provides:
+- scr:
+  - non-life
+    - premium and reserve
+    - lapse
+    - catastrophy
+      - natcat euro
+      - man-made
+  - default
+  - bscr
+  - op
+  - scr
+- mcr
+
+Structure:
+- Each scr sub-module is within its own package.
+- Any required parameters are typically stored in CSV files in the same package 
+- Functions often return tuples. The first item will be a numerical result, the subsequent items data frames containing additional breakdown to debug and support QRT completion.
+
+Known limitations:
+- only gross scr calculated in natcat: approach for reinsurance may be very company specific.
+- not all nat-cat modules included (yet)
+- default quite simple
+
+
```

### Comparing `solvency2sf-0.0.8/README.md` & `solvency2sf-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `solvency2sf-0.0.8/setup.py` & `solvency2sf-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt', 'r') as f:
     dependencies = f.read().splitlines()
 
 setuptools.setup(
     name="solvency2sf",
-    version="0.0.8",
+    version="0.0.9",
     author="Peter Davidson",
     author_email="peterjd41@gmail.com",
     description="Solvency 2 Standard Formula",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pdavidsonFIA/solvency2sf",
     project_urls={
```

### Comparing `solvency2sf-0.0.8/solvency2sf/aggregation.py` & `solvency2sf-0.0.9/solvency2sf/aggregation.py`

 * *Files identical despite different names*

### Comparing `solvency2sf-0.0.8/solvency2sf/default.py` & `solvency2sf-0.0.9/solvency2sf/default.py`

 * *Files identical despite different names*

### Comparing `solvency2sf-0.0.8/solvency2sf/mcr/mcr.py` & `solvency2sf-0.0.9/solvency2sf/mcr/mcr.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,15 +69,16 @@
 
 
 def mcr(
         nwp: pd.Series,
         tp_nl_net: pd.Series,
         tp_l: pd.Series,
         car_l: float,
-        scr: float
+        scr: float,
+        debug_output={}
 ):
     """
     This function calculate:
      - MCR
      - MCR NL Linear
      - MCR L Linear
      """
@@ -108,11 +109,21 @@
     mcr_linear = mcr_linear_l + mcr_linear_nl
     mcr_cap = scr * bound_cap
     mcr_floor = scr * bound_floor
     mcr_combined = np.minimum(np.maximum(mcr_linear, mcr_floor), mcr_cap)
     mcr = np.maximum(mcr_combined, amcr)
     early_warning = ewi_l * mcr_linear_l + ewi_nl * mcr_linear_nl
 
-    # TODO: add QRT output
-    # df = pd.concat((mcr, mcr_linear_nl), axis=1)
-    # df.columns = ['mcr', 'mcr_linear_nl']
-    return mcr
+    mcr_debug = {
+            's28_01_01_02': df,
+            's28_01_01_05': pd.DataFrame.from_dict({
+                'mcr_linear': mcr_linear,
+                'scr': scr,
+                'mcr_cap': mcr_cap,
+                'mcr_floor': mcr_floor,
+                'mcr_combined': mcr_combined,
+                'amcr': amcr,
+                'mcr': mcr
+            }, orient='index', columns=['C0070'])
+        }
+    debug_output['mcr'] = mcr_debug
+    return mcr, debug_output
```

### Comparing `solvency2sf-0.0.8/solvency2sf/operational.py` & `solvency2sf-0.0.9/solvency2sf/operational.py`

 * *Files identical despite different names*

### Comparing `solvency2sf-0.0.8/solvency2sf/scr_nl/cat/manmade/manmade.py` & `solvency2sf-0.0.9/solvency2sf/scr_nl/cat/manmade/manmade.py`

 * *Files identical despite different names*

### Comparing `solvency2sf-0.0.8/solvency2sf/scr_nl/cat/natcat_eur/natcat_eur.py` & `solvency2sf-0.0.9/solvency2sf/scr_nl/cat/natcat_eur/natcat_eur.py`

 * *Files identical despite different names*

### Comparing `solvency2sf-0.0.8/solvency2sf/scr_nl/premres/premres.py` & `solvency2sf-0.0.9/solvency2sf/scr_nl/premres/premres.py`

 * *Files identical despite different names*

### Comparing `solvency2sf-0.0.8/solvency2sf.egg-info/PKG-INFO` & `solvency2sf-0.0.9/solvency2sf.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 Metadata-Version: 2.1
 Name: solvency2sf
-Version: 0.0.8
+Version: 0.0.9
 Summary: Solvency 2 Standard Formula
 Home-page: https://github.com/pdavidsonFIA/solvency2sf
 Author: Peter Davidson
 Author-email: peterjd41@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pdavidsonFIA/solvency2sf/issues
-Description: # solvency2sf
-        Solvency 2 Standard Formula
-        
-        Pandas/numpy implementation of the standard formula for non-life.
-        
-        The calculation logic generally mimics the calculations within the standard formula guidance provided by Lloyd's.
-        https://www.lloyds.com/resources-and-services/capital-and-reserving/capital-guidance/standard-formula-scr
-        
-        The template populated with sample data is saved under /tests
-        
-        Provides:
-        - scr:
-          - non-life
-            - premium and reserve
-            - lapse
-            - catastrophy
-              - natcat euro
-              - man-made
-          - default
-          - bscr
-          - op
-          - scr
-        - mcr
-        
-        Structure:
-        - Each scr sub-module is within its own package.
-        - Any required parameters are typically stored in CSV files in the same package 
-        - Functions often return tuples. The first item will be a numerical result, the subsequent items data frames containing additional breakdown to debug and support QRT completion.
-        
-        Known limitations:
-        - only gross scr calculated in natcat: approach for reinsurance may be very company specific.
-        - not all nat-cat modules included (yet)
-        - default quite simple
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Financial and Insurance Industry
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# solvency2sf
+Solvency 2 Standard Formula
+
+Pandas/numpy implementation of the standard formula for non-life.
+
+The calculation logic generally mimics the calculations within the standard formula guidance provided by Lloyd's.
+https://www.lloyds.com/resources-and-services/capital-and-reserving/capital-guidance/standard-formula-scr
+
+The template populated with sample data is saved under /tests
+
+Provides:
+- scr:
+  - non-life
+    - premium and reserve
+    - lapse
+    - catastrophy
+      - natcat euro
+      - man-made
+  - default
+  - bscr
+  - op
+  - scr
+- mcr
+
+Structure:
+- Each scr sub-module is within its own package.
+- Any required parameters are typically stored in CSV files in the same package 
+- Functions often return tuples. The first item will be a numerical result, the subsequent items data frames containing additional breakdown to debug and support QRT completion.
+
+Known limitations:
+- only gross scr calculated in natcat: approach for reinsurance may be very company specific.
+- not all nat-cat modules included (yet)
+- default quite simple
+
+
```

### Comparing `solvency2sf-0.0.8/solvency2sf.egg-info/SOURCES.txt` & `solvency2sf-0.0.9/solvency2sf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

