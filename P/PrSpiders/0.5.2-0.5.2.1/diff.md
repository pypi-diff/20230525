# Comparing `tmp/PrSpiders-0.5.2.tar.gz` & `tmp/PrSpiders-0.5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrSpiders-0.5.2.tar", last modified: Wed May 24 05:19:31 2023, max compression
+gzip compressed data, was "PrSpiders-0.5.2.1.tar", last modified: Wed May 24 08:10:43 2023, max compression
```

## Comparing `PrSpiders-0.5.2.tar` & `PrSpiders-0.5.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 05:19:31.496300 PrSpiders-0.5.2/
--rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.5.2/LICENSE.txt
--rw-rw-rw-   0        0        0     5678 2023-05-24 05:19:31.317298 PrSpiders-0.5.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-24 05:19:30.465300 PrSpiders-0.5.2/PrSpider/
--rw-rw-rw-   0        0        0    10667 2023-05-24 05:19:03.000000 PrSpiders-0.5.2/PrSpider/PrSpiders.py
--rw-rw-rw-   0        0        0       98 2023-05-23 06:27:42.000000 PrSpiders-0.5.2/PrSpider/__init__.py
--rw-rw-rw-   0        0        0     2392 2023-05-24 05:18:39.000000 PrSpiders-0.5.2/PrSpider/log.py
--rw-rw-rw-   0        0        0    11257 2023-05-24 01:36:58.000000 PrSpiders-0.5.2/PrSpider/pxpath.py
--rw-rw-rw-   0        0        0     3193 2023-05-23 07:08:35.000000 PrSpiders-0.5.2/PrSpider/pyconn.py
--rw-rw-rw-   0        0        0     4560 2023-05-23 06:28:17.000000 PrSpiders-0.5.2/PrSpider/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.2/PrSpider/useragent.py
-drwxrwxrwx   0        0        0        0 2023-05-24 05:19:30.523298 PrSpiders-0.5.2/PrSpiders.egg-info/
--rw-rw-rw-   0        0        0     5678 2023-05-24 05:19:29.000000 PrSpiders-0.5.2/PrSpiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      598 2023-05-24 05:19:30.000000 PrSpiders-0.5.2/PrSpiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 05:19:29.000000 PrSpiders-0.5.2/PrSpiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-05-24 05:19:29.000000 PrSpiders-0.5.2/PrSpiders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2023-05-24 05:19:29.000000 PrSpiders-0.5.2/PrSpiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-05-24 05:19:29.000000 PrSpiders-0.5.2/PrSpiders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5166 2023-04-23 08:22:29.000000 PrSpiders-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 05:19:30.536301 PrSpiders-0.5.2/pkg/
--rw-rw-rw-   0        0        0       23 2023-05-24 01:39:05.000000 PrSpiders-0.5.2/pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 05:19:30.714298 PrSpiders-0.5.2/pkg/prspider/
--rw-rw-rw-   0        0        0     1212 2023-04-20 09:13:43.000000 PrSpiders-0.5.2/pkg/prspider/PrSpider_CMD.py
--rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.5.2/pkg/prspider/PrSpider_run.py
--rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.5.2/pkg/prspider/__init__.py
--rw-rw-rw-   0        0        0      833 2023-04-23 03:22:54.000000 PrSpiders-0.5.2/pkg/prspider/start.py
-drwxrwxrwx   0        0        0        0 2023-05-24 05:19:30.950298 PrSpiders-0.5.2/requestXpath/
--rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.5.2/requestXpath/__init__.py
--rw-rw-rw-   0        0        0     8642 2023-04-18 08:44:05.000000 PrSpiders-0.5.2/requestXpath/pxpath.py
--rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.5.2/requestXpath/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.2/requestXpath/useragent.py
--rw-rw-rw-   0        0        0       42 2023-05-24 05:19:31.496300 PrSpiders-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1032 2023-05-24 05:19:27.000000 PrSpiders-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 08:10:43.321666 PrSpiders-0.5.2.1/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.5.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     5680 2023-05-24 08:10:43.312656 PrSpiders-0.5.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-24 08:10:43.162660 PrSpiders-0.5.2.1/PrSpider/
+-rw-rw-rw-   0        0        0    10667 2023-05-24 05:19:03.000000 PrSpiders-0.5.2.1/PrSpider/PrSpiders.py
+-rw-rw-rw-   0        0        0       98 2023-05-23 06:27:42.000000 PrSpiders-0.5.2.1/PrSpider/__init__.py
+-rw-rw-rw-   0        0        0     2392 2023-05-24 05:18:39.000000 PrSpiders-0.5.2.1/PrSpider/log.py
+-rw-rw-rw-   0        0        0    11257 2023-05-24 01:36:58.000000 PrSpiders-0.5.2.1/PrSpider/pxpath.py
+-rw-rw-rw-   0        0        0     3268 2023-05-24 08:10:28.000000 PrSpiders-0.5.2.1/PrSpider/pyconn.py
+-rw-rw-rw-   0        0        0     4560 2023-05-23 06:28:17.000000 PrSpiders-0.5.2.1/PrSpider/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.2.1/PrSpider/useragent.py
+drwxrwxrwx   0        0        0        0 2023-05-24 08:10:43.212659 PrSpiders-0.5.2.1/PrSpiders.egg-info/
+-rw-rw-rw-   0        0        0     5680 2023-05-24 08:10:42.000000 PrSpiders-0.5.2.1/PrSpiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      598 2023-05-24 08:10:42.000000 PrSpiders-0.5.2.1/PrSpiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 08:10:42.000000 PrSpiders-0.5.2.1/PrSpiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-24 08:10:42.000000 PrSpiders-0.5.2.1/PrSpiders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2023-05-24 08:10:42.000000 PrSpiders-0.5.2.1/PrSpiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-05-24 08:10:42.000000 PrSpiders-0.5.2.1/PrSpiders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5166 2023-04-23 08:22:29.000000 PrSpiders-0.5.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 08:10:43.225660 PrSpiders-0.5.2.1/pkg/
+-rw-rw-rw-   0        0        0       23 2023-05-24 01:39:05.000000 PrSpiders-0.5.2.1/pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 08:10:43.261660 PrSpiders-0.5.2.1/pkg/prspider/
+-rw-rw-rw-   0        0        0     1212 2023-04-20 09:13:43.000000 PrSpiders-0.5.2.1/pkg/prspider/PrSpider_CMD.py
+-rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.5.2.1/pkg/prspider/PrSpider_run.py
+-rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.5.2.1/pkg/prspider/__init__.py
+-rw-rw-rw-   0        0        0      833 2023-04-23 03:22:54.000000 PrSpiders-0.5.2.1/pkg/prspider/start.py
+drwxrwxrwx   0        0        0        0 2023-05-24 08:10:43.306660 PrSpiders-0.5.2.1/requestXpath/
+-rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.5.2.1/requestXpath/__init__.py
+-rw-rw-rw-   0        0        0     8642 2023-04-18 08:44:05.000000 PrSpiders-0.5.2.1/requestXpath/pxpath.py
+-rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.5.2.1/requestXpath/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.5.2.1/requestXpath/useragent.py
+-rw-rw-rw-   0        0        0       42 2023-05-24 08:10:43.323659 PrSpiders-0.5.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1034 2023-05-24 08:10:35.000000 PrSpiders-0.5.2.1/setup.py
```

### Comparing `PrSpiders-0.5.2/LICENSE.txt` & `PrSpiders-0.5.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2/PKG-INFO` & `PrSpiders-0.5.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.5.2
+Version: 0.5.2.1
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.5.2/PrSpider/PrSpiders.py` & `PrSpiders-0.5.2.1/PrSpider/PrSpiders.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2/PrSpider/log.py` & `PrSpiders-0.5.2.1/PrSpider/log.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2/PrSpider/pxpath.py` & `PrSpiders-0.5.2.1/PrSpider/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2/PrSpider/pyconn.py` & `PrSpiders-0.5.2.1/PrSpider/pyconn.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,15 +61,18 @@
         insert_id = pyconn.insert_id()
         self.login('数据成功插入: %s' % insert_id)
         pyconn.commit()
         return insert_id
 
     @ErrorTip
     def execute(self, sql):
-        return self.cursor.execute(sql)
+        pyconn = self.conn
+        cursor = pyconn.cursor()
+        cursor.execute(sql)
+        pyconn.commit()
 
     @ErrorTip
     def fetchone(self, sql):
         cursor = self.conn.cursor()
         cursor.execute(sql)
         return cursor.fetchone()
```

### Comparing `PrSpiders-0.5.2/PrSpider/requestXpath.py` & `PrSpiders-0.5.2.1/PrSpider/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2/PrSpider/useragent.py` & `PrSpiders-0.5.2.1/PrSpider/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2/PrSpiders.egg-info/PKG-INFO` & `PrSpiders-0.5.2.1/PrSpiders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.5.2
+Version: 0.5.2.1
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.5.2/PrSpiders.egg-info/SOURCES.txt` & `PrSpiders-0.5.2.1/PrSpiders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2/README.md` & `PrSpiders-0.5.2.1/README.md`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2/pkg/prspider/PrSpider_CMD.py` & `PrSpiders-0.5.2.1/pkg/prspider/PrSpider_CMD.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2/pkg/prspider/start.py` & `PrSpiders-0.5.2.1/pkg/prspider/start.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2/requestXpath/__init__.py` & `PrSpiders-0.5.2.1/requestXpath/__init__.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2/requestXpath/pxpath.py` & `PrSpiders-0.5.2.1/requestXpath/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2/requestXpath/requestXpath.py` & `PrSpiders-0.5.2.1/requestXpath/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2/requestXpath/useragent.py` & `PrSpiders-0.5.2.1/requestXpath/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.5.2/setup.py` & `PrSpiders-0.5.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!python
 # -*- coding:utf-8 -*-
 from __future__ import print_function
 from setuptools import setup, find_packages
 
-__version__ = "0.5.2"
+__version__ = "0.5.2.1"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PrSpiders",
     version=__version__,
```

