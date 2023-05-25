# Comparing `tmp/pygsod-0.2.3.tar.gz` & `tmp/pygsod-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygsod-0.2.3.tar", last modified: Wed Mar 29 13:33:53 2023, max compression
+gzip compressed data, was "pygsod-0.2.4.tar", last modified: Thu May 25 08:45:05 2023, max compression
```

## Comparing `pygsod-0.2.3.tar` & `pygsod-0.2.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 13:33:53.946495 pygsod-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-03-29 13:33:40.000000 pygsod-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      968 2023-03-29 13:33:53.946495 pygsod-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6263 2023-03-29 13:33:40.000000 pygsod-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 13:33:53.946495 pygsod-0.2.3/pygsod/
--rw-r--r--   0 runner    (1001) docker     (122)      238 2023-03-29 13:33:40.000000 pygsod-0.2.3/pygsod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-03-29 13:33:40.000000 pygsod-0.2.3/pygsod/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     5716 2023-03-29 13:33:40.000000 pygsod-0.2.3/pygsod/epw_converter.py
--rw-r--r--   0 runner    (1001) docker     (122)     9058 2023-03-29 13:33:40.000000 pygsod-0.2.3/pygsod/gsod.py
--rw-r--r--   0 runner    (1001) docker     (122)     6172 2023-03-29 13:33:40.000000 pygsod-0.2.3/pygsod/isd_lite.py
--rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-03-29 13:33:40.000000 pygsod-0.2.3/pygsod/isdhistory.py
--rw-r--r--   0 runner    (1001) docker     (122)    10402 2023-03-29 13:33:40.000000 pygsod-0.2.3/pygsod/ish_full.py
--rw-r--r--   0 runner    (1001) docker     (122)    18725 2023-03-29 13:33:40.000000 pygsod-0.2.3/pygsod/noaadata.py
--rw-r--r--   0 runner    (1001) docker     (122)    11550 2023-03-29 13:33:40.000000 pygsod-0.2.3/pygsod/output.py
--rw-r--r--   0 runner    (1001) docker     (122)     7935 2023-03-29 13:33:40.000000 pygsod-0.2.3/pygsod/tmy_download.py
--rw-r--r--   0 runner    (1001) docker     (122)     5588 2023-03-29 13:33:40.000000 pygsod-0.2.3/pygsod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 13:33:53.946495 pygsod-0.2.3/pygsod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      968 2023-03-29 13:33:53.000000 pygsod-0.2.3/pygsod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-03-29 13:33:53.000000 pygsod-0.2.3/pygsod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-29 13:33:53.000000 pygsod-0.2.3/pygsod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      158 2023-03-29 13:33:53.000000 pygsod-0.2.3/pygsod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-03-29 13:33:53.000000 pygsod-0.2.3/pygsod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      587 2023-03-29 13:33:40.000000 pygsod-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-03-29 13:33:53.946495 pygsod-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4355 2023-03-29 13:33:40.000000 pygsod-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 13:33:53.946495 pygsod-0.2.3/support/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-29 13:33:40.000000 pygsod-0.2.3/support/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:45:05.795551 pygsod-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-05-25 08:44:52.000000 pygsod-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      968 2023-05-25 08:45:05.795551 pygsod-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6263 2023-05-25 08:44:52.000000 pygsod-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:45:05.795551 pygsod-0.2.4/pygsod/
+-rw-r--r--   0 runner    (1001) docker     (122)      238 2023-05-25 08:44:52.000000 pygsod-0.2.4/pygsod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-05-25 08:44:52.000000 pygsod-0.2.4/pygsod/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5716 2023-05-25 08:44:52.000000 pygsod-0.2.4/pygsod/epw_converter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9058 2023-05-25 08:44:52.000000 pygsod-0.2.4/pygsod/gsod.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6172 2023-05-25 08:44:52.000000 pygsod-0.2.4/pygsod/isd_lite.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-05-25 08:44:52.000000 pygsod-0.2.4/pygsod/isdhistory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10402 2023-05-25 08:44:52.000000 pygsod-0.2.4/pygsod/ish_full.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18725 2023-05-25 08:44:52.000000 pygsod-0.2.4/pygsod/noaadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11550 2023-05-25 08:44:52.000000 pygsod-0.2.4/pygsod/output.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7935 2023-05-25 08:44:52.000000 pygsod-0.2.4/pygsod/tmy_download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5650 2023-05-25 08:44:52.000000 pygsod-0.2.4/pygsod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:45:05.795551 pygsod-0.2.4/pygsod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      968 2023-05-25 08:45:05.000000 pygsod-0.2.4/pygsod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-05-25 08:45:05.000000 pygsod-0.2.4/pygsod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 08:45:05.000000 pygsod-0.2.4/pygsod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2023-05-25 08:45:05.000000 pygsod-0.2.4/pygsod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-25 08:45:05.000000 pygsod-0.2.4/pygsod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      587 2023-05-25 08:44:52.000000 pygsod-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      805 2023-05-25 08:45:05.799551 pygsod-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4355 2023-05-25 08:44:52.000000 pygsod-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:45:05.795551 pygsod-0.2.4/support/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 08:44:52.000000 pygsod-0.2.4/support/__init__.py
```

### Comparing `pygsod-0.2.3/LICENSE` & `pygsod-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pygsod-0.2.3/PKG-INFO` & `pygsod-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygsod
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Wrapper to Download data off NOAA's Global Summary of the day,and load them into pandas
 Home-page: https://effibem.com
 Author: Julien Marrec & EffiBEM
 Author-email: contact@effibem.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/jmarrec/pygsod/issues
 Project-URL: Source Code, https://github.com/jmarrec/pygsod
```

### Comparing `pygsod-0.2.3/README.md` & `pygsod-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pygsod-0.2.3/pygsod/constants.py` & `pygsod-0.2.4/pygsod/constants.py`

 * *Files identical despite different names*

### Comparing `pygsod-0.2.3/pygsod/epw_converter.py` & `pygsod-0.2.4/pygsod/epw_converter.py`

 * *Files identical despite different names*

### Comparing `pygsod-0.2.3/pygsod/gsod.py` & `pygsod-0.2.4/pygsod/gsod.py`

 * *Files identical despite different names*

### Comparing `pygsod-0.2.3/pygsod/isd_lite.py` & `pygsod-0.2.4/pygsod/isd_lite.py`

 * *Files identical despite different names*

### Comparing `pygsod-0.2.3/pygsod/isdhistory.py` & `pygsod-0.2.4/pygsod/isdhistory.py`

 * *Files identical despite different names*

### Comparing `pygsod-0.2.3/pygsod/ish_full.py` & `pygsod-0.2.4/pygsod/ish_full.py`

 * *Files identical despite different names*

### Comparing `pygsod-0.2.3/pygsod/noaadata.py` & `pygsod-0.2.4/pygsod/noaadata.py`

 * *Files identical despite different names*

### Comparing `pygsod-0.2.3/pygsod/output.py` & `pygsod-0.2.4/pygsod/output.py`

 * *Files identical despite different names*

### Comparing `pygsod-0.2.3/pygsod/tmy_download.py` & `pygsod-0.2.4/pygsod/tmy_download.py`

 * *Files identical despite different names*

### Comparing `pygsod-0.2.3/pygsod/utils.py` & `pygsod-0.2.4/pygsod/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,28 +148,29 @@
 
     Needs:
     -------------------------------
         import sys # For backward compatibility with Python 2.x
         import datetime
 
     """
+    current_year = datetime.date.today().year
     while True:
         year = input(prompt)
 
         # If nothing is provided, get current year
         if year == "":
-            year = datetime.date.today().year
+            year = current_year
         try:
             year = int(year)
         except ValueError:
-            print("Please enter an integer between 2000 and 2020")
+            print(f"Please enter an integer between 2000 and {current_year}")
             continue
 
-        if year < 1950 or year > 2020:
-            print("year needs to be between 2000 and 2020!")
+        if year < 1950 or year > current_year:
+            print(f"year needs to be between 2000 and {current_year}!")
             continue
         else:
             break
     return year
 
 
 def clean_df(df):
```

### Comparing `pygsod-0.2.3/pygsod.egg-info/PKG-INFO` & `pygsod-0.2.4/pygsod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygsod
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Wrapper to Download data off NOAA's Global Summary of the day,and load them into pandas
 Home-page: https://effibem.com
 Author: Julien Marrec & EffiBEM
 Author-email: contact@effibem.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/jmarrec/pygsod/issues
 Project-URL: Source Code, https://github.com/jmarrec/pygsod
```

### Comparing `pygsod-0.2.3/pyproject.toml` & `pygsod-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pygsod-0.2.3/setup.cfg` & `pygsod-0.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pygsod-0.2.3/setup.py` & `pygsod-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 and load them into pandas"""
 
 setup(
     name="pygsod",
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.2.3",
+    version="0.2.4",
     description=("A Wrapper to Download data off " "NOAA's Global Summary of the day," "and load them into pandas"),
     long_description=LONG_DESCRIPTION,  # TODO
     # The project's main homepage.
     # url='https://github.com/pypa/sampleproject',
     # Author details
     author="Julien Marrec & EffiBEM",
     author_email="contact@effibem.com",
```

