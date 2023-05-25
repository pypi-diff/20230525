# Comparing `tmp/inspire-utils-3.0.8.tar.gz` & `tmp/inspire-utils-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inspire-utils-3.0.8.tar", last modified: Fri Aug 16 11:08:47 2019, max compression
+gzip compressed data, was "dist/inspire-utils-3.0.9.tar", last modified: Mon Feb 24 14:45:09 2020, max compression
```

## Comparing `inspire-utils-3.0.8.tar` & `inspire-utils-3.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-16 11:08:46.000000 inspire-utils-3.0.8/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-16 11:08:46.000000 inspire-utils-3.0.8/inspire_utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2050 2019-08-16 11:08:03.000000 inspire-utils-3.0.8/inspire_utils/urls.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13398 2019-08-16 11:08:03.000000 inspire-utils-3.0.8/inspire_utils/name.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1787 2019-08-16 11:08:03.000000 inspire-utils-3.0.8/inspire_utils/logging.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3669 2019-08-16 11:08:03.000000 inspire-utils-3.0.8/inspire_utils/record.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2647 2019-08-16 11:08:03.000000 inspire-utils-3.0.8/inspire_utils/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2128 2019-08-16 11:08:03.000000 inspire-utils-3.0.8/inspire_utils/dedupers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1003 2019-08-16 11:08:03.000000 inspire-utils-3.0.8/inspire_utils/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5058 2019-08-16 11:08:03.000000 inspire-utils-3.0.8/inspire_utils/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9153 2019-08-16 11:08:03.000000 inspire-utils-3.0.8/inspire_utils/date.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2531 2019-08-16 11:08:46.000000 inspire-utils-3.0.8/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-16 11:08:46.000000 inspire-utils-3.0.8/inspire_utils.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2531 2019-08-16 11:08:46.000000 inspire-utils-3.0.8/inspire_utils.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-08-16 11:08:46.000000 inspire-utils-3.0.8/inspire_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2019-08-16 11:08:46.000000 inspire-utils-3.0.8/inspire_utils.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-08-16 11:08:46.000000 inspire-utils-3.0.8/inspire_utils.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      465 2019-08-16 11:08:46.000000 inspire-utils-3.0.8/inspire_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      577 2019-08-16 11:08:46.000000 inspire-utils-3.0.8/inspire_utils.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      246 2019-08-16 11:08:46.000000 inspire-utils-3.0.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1309 2019-08-16 11:08:03.000000 inspire-utils-3.0.8/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2999 2019-08-16 11:08:03.000000 inspire-utils-3.0.8/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-24 14:45:09.000000 inspire-utils-3.0.9/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-24 14:45:09.000000 inspire-utils-3.0.9/inspire_utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2050 2020-02-24 14:44:32.000000 inspire-utils-3.0.9/inspire_utils/urls.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13398 2020-02-24 14:44:32.000000 inspire-utils-3.0.9/inspire_utils/name.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1787 2020-02-24 14:44:32.000000 inspire-utils-3.0.9/inspire_utils/logging.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3669 2020-02-24 14:44:32.000000 inspire-utils-3.0.9/inspire_utils/record.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2647 2020-02-24 14:44:32.000000 inspire-utils-3.0.9/inspire_utils/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2128 2020-02-24 14:44:32.000000 inspire-utils-3.0.9/inspire_utils/dedupers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1003 2020-02-24 14:44:32.000000 inspire-utils-3.0.9/inspire_utils/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5058 2020-02-24 14:44:32.000000 inspire-utils-3.0.9/inspire_utils/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9263 2020-02-24 14:44:32.000000 inspire-utils-3.0.9/inspire_utils/date.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2531 2020-02-24 14:45:09.000000 inspire-utils-3.0.9/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-24 14:45:09.000000 inspire-utils-3.0.9/inspire_utils.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2531 2020-02-24 14:45:08.000000 inspire-utils-3.0.9/inspire_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-02-24 14:45:08.000000 inspire-utils-3.0.9/inspire_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2020-02-24 14:45:08.000000 inspire-utils-3.0.9/inspire_utils.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-02-24 14:45:08.000000 inspire-utils-3.0.9/inspire_utils.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      465 2020-02-24 14:45:08.000000 inspire-utils-3.0.9/inspire_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      577 2020-02-24 14:45:08.000000 inspire-utils-3.0.9/inspire_utils.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      246 2020-02-24 14:45:09.000000 inspire-utils-3.0.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1309 2020-02-24 14:44:32.000000 inspire-utils-3.0.9/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2999 2020-02-24 14:44:32.000000 inspire-utils-3.0.9/setup.py
```

### Comparing `inspire-utils-3.0.8/inspire_utils/urls.py` & `inspire-utils-3.0.9/inspire_utils/urls.py`

 * *Files identical despite different names*

### Comparing `inspire-utils-3.0.8/inspire_utils/name.py` & `inspire-utils-3.0.9/inspire_utils/name.py`

 * *Files identical despite different names*

### Comparing `inspire-utils-3.0.8/inspire_utils/logging.py` & `inspire-utils-3.0.9/inspire_utils/logging.py`

 * *Files identical despite different names*

### Comparing `inspire-utils-3.0.8/inspire_utils/record.py` & `inspire-utils-3.0.9/inspire_utils/record.py`

 * *Files identical despite different names*

### Comparing `inspire-utils-3.0.8/inspire_utils/config.py` & `inspire-utils-3.0.9/inspire_utils/config.py`

 * *Files identical despite different names*

### Comparing `inspire-utils-3.0.8/inspire_utils/dedupers.py` & `inspire-utils-3.0.9/inspire_utils/dedupers.py`

 * *Files identical despite different names*

### Comparing `inspire-utils-3.0.8/inspire_utils/__init__.py` & `inspire-utils-3.0.9/inspire_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `inspire-utils-3.0.8/inspire_utils/helpers.py` & `inspire-utils-3.0.9/inspire_utils/helpers.py`

 * *Files identical despite different names*

### Comparing `inspire-utils-3.0.8/inspire_utils/date.py` & `inspire-utils-3.0.9/inspire_utils/date.py`

 * *Files 4% similar despite different names*

```diff
@@ -187,16 +187,16 @@
             >>> PartialDate(1686, 6, 30).pprint()
             u'Jun 30, 1686'
 
         """
         if not self.month:
             return dates.format_date(datetime.date(self.year, 1, 1), 'yyyy', locale='en')
         if not self.day:
-            return dates.format_date(datetime.date(self.year, self.month, 1), 'MMM, YYYY', locale='en')
-        return dates.format_date(datetime.date(self.year, self.month, self.day), 'MMM d, YYYY', locale='en')
+            return dates.format_date(datetime.date(self.year, self.month, 1), 'MMM, yyyy', locale='en')
+        return dates.format_date(datetime.date(self.year, self.month, self.day), 'MMM d, yyyy', locale='en')
 
 
 def normalize_date(date, **kwargs):
     """Normalize a date to the be schema-compliant.
 
     This is a convenience wrapper around :ref:`PartialDate`, which should be
     used instead if more features are needed.
@@ -237,25 +237,34 @@
 
     This is a convenience wrapper around :ref:`PartialDate`, which should be
     used instead if more features are needed.
     """
     return PartialDate.loads(date).pprint()
 
 
-def earliest_date(dates, full_date=False):
+def earliest_date(dates):
     """Return the earliest among the schema-compliant dates.
 
     This is a convenience wrapper around :ref:`PartialDate`, which should be
     used instead if more features are needed.
 
     Args:
         dates(list): List of dates from which oldest/earliest one will be returned
-        full_date(bool): Adds month and/or day as "01" if they are missing
     Returns:
         str: Earliest date from provided list
     """
     min_date = min(PartialDate.loads(date) for date in dates)
-    if not min_date.month and full_date:
-        min_date.month = 1
-    if not min_date.day and full_date:
-        min_date.day = 1
     return min_date.dumps()
+
+
+def fill_missing_date_parts(date):
+    """Sets missing day and/or month to 1. Useful to avoid errors when saving to DB."""
+
+    if date is None:
+        return
+
+    date_obj = PartialDate.loads(date)
+    if not date_obj.month:
+        date_obj.month = 1
+    if not date_obj.day:
+        date_obj.day = 1
+    return date_obj.dumps()
```

### Comparing `inspire-utils-3.0.8/PKG-INFO` & `inspire-utils-3.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspire-utils
-Version: 3.0.8
+Version: 3.0.9
 Summary: INSPIRE-specific utils.
 Home-page: https://github.com/inspirehep/inspire-utils
 Author: CERN
 Author-email: admin@inspirehep.net
 License: GPLv3
 Description: ..
             This file is part of INSPIRE.
```

### Comparing `inspire-utils-3.0.8/inspire_utils.egg-info/PKG-INFO` & `inspire-utils-3.0.9/inspire_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspire-utils
-Version: 3.0.8
+Version: 3.0.9
 Summary: INSPIRE-specific utils.
 Home-page: https://github.com/inspirehep/inspire-utils
 Author: CERN
 Author-email: admin@inspirehep.net
 License: GPLv3
 Description: ..
             This file is part of INSPIRE.
```

### Comparing `inspire-utils-3.0.8/inspire_utils.egg-info/requires.txt` & `inspire-utils-3.0.9/inspire_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `inspire-utils-3.0.8/README.rst` & `inspire-utils-3.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `inspire-utils-3.0.8/setup.py` & `inspire-utils-3.0.9/setup.py`

 * *Files identical despite different names*

