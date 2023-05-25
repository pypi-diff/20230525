# Comparing `tmp/tcia_utils-1.3.2.tar.gz` & `tmp/tcia_utils-1.4.tar.gz`

## Comparing `tcia_utils-1.3.2.tar` & `tcia_utils-1.4.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 tcia_utils-1.3.2/src/tcia_utils/__init__.py
--rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 tcia_utils-1.3.2/src/tcia_utils/datacite.py
--rw-r--r--   0        0        0    51536 2020-02-02 00:00:00.000000 tcia_utils-1.3.2/src/tcia_utils/nbia.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tcia_utils-1.3.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-1.3.2/LICENSE
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 tcia_utils-1.3.2/README.md
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 tcia_utils-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 tcia_utils-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 tcia_utils-1.4/src/tcia_utils/__init__.py
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 tcia_utils-1.4/src/tcia_utils/datacite.py
+-rw-r--r--   0        0        0    51536 2020-02-02 00:00:00.000000 tcia_utils-1.4/src/tcia_utils/nbia.py
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 tcia_utils-1.4/src/tcia_utils/pathdb.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tcia_utils-1.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-1.4/LICENSE
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 tcia_utils-1.4/README.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 tcia_utils-1.4/pyproject.toml
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 tcia_utils-1.4/PKG-INFO
```

### Comparing `tcia_utils-1.3.2/src/tcia_utils/datacite.py` & `tcia_utils-1.4/src/tcia_utils/datacite.py`

 * *Files 11% similar despite different names*

```diff
@@ -130,18 +130,18 @@
                     dt_string = now.strftime("%Y-%m-%d_%H%M")
                     df.to_csv('datacite_' + dt_string + '.csv')
                     _log.info(f"Report saved as datacite_{dt_string}.csv")
                 return df
             else:
                 return data
         else:
-            print("No results found.")
+            _log.info(f'No results found.')
             
     # handle errors
     except requests.exceptions.HTTPError as errh:
-        print(errh)
+        _log.error(f'Error: {errh}')
     except requests.exceptions.ConnectionError as errc:
-        print(errc)
+        _log.error(f'Error: {errc}')
     except requests.exceptions.Timeout as errt:
-        print(errt)
+        _log.error(f'Error: {errt}')
     except requests.exceptions.RequestException as err:
-        print(err)
+        _log.error(f'Error: {err}')
```

### Comparing `tcia_utils-1.3.2/src/tcia_utils/nbia.py` & `tcia_utils-1.4/src/tcia_utils/nbia.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.3.2/.gitignore` & `tcia_utils-1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.3.2/LICENSE` & `tcia_utils-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.3.2/README.md` & `tcia_utils-1.4/README.md`

 * *Files identical despite different names*

### Comparing `tcia_utils-1.3.2/pyproject.toml` & `tcia_utils-1.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tcia_utils"
-version = "1.3.2"
+version = "1.4"
 authors = [
   { name="Justin Kirby", email="justin.kirby@nih.gov" },
 ]
 description = "A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tcia_utils-1.3.2/PKG-INFO` & `tcia_utils-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcia_utils
-Version: 1.3.2
+Version: 1.4
 Summary: A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python.
 Project-URL: Homepage, https://github.com/kirbyju/tcia_utils
 Project-URL: Bug Tracker, https://github.com/kirbyju/tcia_utils/issues
 Author-email: Justin Kirby <justin.kirby@nih.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

