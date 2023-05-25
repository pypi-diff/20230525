# Comparing `tmp/datamarket-0.2.5.tar.gz` & `tmp/datamarket-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamarket-0.2.5.tar", last modified: Fri Apr 14 11:22:22 2023, max compression
+gzip compressed data, was "datamarket-0.2.6.tar", last modified: Wed May 24 14:24:35 2023, max compression
```

## Comparing `datamarket-0.2.5.tar` & `datamarket-0.2.6.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-14 11:22:22.827882 datamarket-0.2.5/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35149 2021-10-07 14:37:41.000000 datamarket-0.2.5/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1342 2023-04-14 11:22:22.823882 datamarket-0.2.5/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      790 2022-08-18 10:42:29.000000 datamarket-0.2.5/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-14 11:22:22.827882 datamarket-0.2.5/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1019 2023-04-14 11:21:39.000000 datamarket-0.2.5/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-14 11:22:22.823882 datamarket-0.2.5/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-14 11:22:22.823882 datamarket-0.2.5/src/datamarket/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2021-11-03 08:15:04.000000 datamarket-0.2.5/src/datamarket/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-14 11:22:22.823882 datamarket-0.2.5/src/datamarket/interfaces/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-03 09:55:33.000000 datamarket-0.2.5/src/datamarket/interfaces/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3104 2023-02-16 08:03:41.000000 datamarket-0.2.5/src/datamarket/interfaces/alchemy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2022-08-08 10:00:49.000000 datamarket-0.2.5/src/datamarket/interfaces/drive.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1344 2023-02-17 11:31:46.000000 datamarket-0.2.5/src/datamarket/interfaces/ftp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2023-04-14 11:21:25.000000 datamarket-0.2.5/src/datamarket/interfaces/proxy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2565 2023-03-14 07:00:34.000000 datamarket-0.2.5/src/datamarket/interfaces/tinybird.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1898 2023-02-09 08:25:23.000000 datamarket-0.2.5/src/datamarket/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-14 11:22:22.823882 datamarket-0.2.5/src/datamarket.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1342 2023-04-14 11:22:22.000000 datamarket-0.2.5/src/datamarket.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      482 2023-04-14 11:22:22.000000 datamarket-0.2.5/src/datamarket.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-14 11:22:22.000000 datamarket-0.2.5/src/datamarket.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       46 2023-04-14 11:22:22.000000 datamarket-0.2.5/src/datamarket.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-04-14 11:22:22.000000 datamarket-0.2.5/src/datamarket.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 14:24:35.451199 datamarket-0.2.6/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35149 2021-10-07 14:37:41.000000 datamarket-0.2.6/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1342 2023-05-24 14:24:35.451199 datamarket-0.2.6/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      790 2022-08-18 10:42:29.000000 datamarket-0.2.6/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-24 14:24:35.451199 datamarket-0.2.6/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1050 2023-05-24 14:05:34.000000 datamarket-0.2.6/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 14:24:35.439198 datamarket-0.2.6/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 14:24:35.447198 datamarket-0.2.6/src/datamarket/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2021-11-03 08:15:04.000000 datamarket-0.2.6/src/datamarket/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 14:24:35.451199 datamarket-0.2.6/src/datamarket/interfaces/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-03 09:55:33.000000 datamarket-0.2.6/src/datamarket/interfaces/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3104 2023-02-16 08:03:41.000000 datamarket-0.2.6/src/datamarket/interfaces/alchemy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2022-08-08 10:00:49.000000 datamarket-0.2.6/src/datamarket/interfaces/drive.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1344 2023-02-17 11:31:46.000000 datamarket-0.2.6/src/datamarket/interfaces/ftp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2023-04-14 11:21:25.000000 datamarket-0.2.6/src/datamarket/interfaces/proxy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1792 2023-05-24 14:14:30.000000 datamarket-0.2.6/src/datamarket/interfaces/selenium.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2565 2023-03-14 07:00:34.000000 datamarket-0.2.6/src/datamarket/interfaces/tinybird.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1901 2023-05-24 14:14:30.000000 datamarket-0.2.6/src/datamarket/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-24 14:24:35.447198 datamarket-0.2.6/src/datamarket.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1342 2023-05-24 14:24:35.000000 datamarket-0.2.6/src/datamarket.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      520 2023-05-24 14:24:35.000000 datamarket-0.2.6/src/datamarket.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-24 14:24:35.000000 datamarket-0.2.6/src/datamarket.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       70 2023-05-24 14:24:35.000000 datamarket-0.2.6/src/datamarket.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-05-24 14:24:35.000000 datamarket-0.2.6/src/datamarket.egg-info/top_level.txt
```

### Comparing `datamarket-0.2.5/LICENSE` & `datamarket-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `datamarket-0.2.5/PKG-INFO` & `datamarket-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamarket
-Version: 0.2.5
+Version: 0.2.6
 Summary: Utilities that integrate advance scraping knowledge into just one library.
 Home-page: https://github.com/Data-Market/datamarket
 Author: DataMarket
 Author-email: techsupport@datamarket.es
 Project-URL: Website, https://datamarket.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `datamarket-0.2.5/README.md` & `datamarket-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `datamarket-0.2.5/setup.py` & `datamarket-0.2.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 
 requirements = [
     "sqlalchemy",
     "requests[socks]",
     "retry",
     "stem",
     "pydrive",
+    "undetected_chromedriver",
 ]
 
 setuptools.setup(
     name="datamarket",
-    version="0.2.5",
+    version="0.2.6",
     author="DataMarket",
     author_email="techsupport@datamarket.es",
     description="Utilities that integrate advance scraping knowledge into just one library.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Data-Market/datamarket",
     project_urls={
```

### Comparing `datamarket-0.2.5/src/datamarket/interfaces/alchemy.py` & `datamarket-0.2.6/src/datamarket/interfaces/alchemy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.2.5/src/datamarket/interfaces/drive.py` & `datamarket-0.2.6/src/datamarket/interfaces/drive.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.2.5/src/datamarket/interfaces/ftp.py` & `datamarket-0.2.6/src/datamarket/interfaces/ftp.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.2.5/src/datamarket/interfaces/proxy.py` & `datamarket-0.2.6/src/datamarket/interfaces/proxy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.2.5/src/datamarket/interfaces/tinybird.py` & `datamarket-0.2.6/src/datamarket/interfaces/tinybird.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.2.5/src/datamarket/utils.py` & `datamarket-0.2.6/src/datamarket/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,12 +66,12 @@
             return num
 
     except ValueError:
         logger.warning(f"unable to parse {text} as integer")
 
 
 def get_chromedriver_version():
-    return (
+    return int(
         run_bash_command("/usr/bin/google-chrome --version")
         .split(" ")[2]
         .split(".")[0]
     )
```

### Comparing `datamarket-0.2.5/src/datamarket.egg-info/PKG-INFO` & `datamarket-0.2.6/src/datamarket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamarket
-Version: 0.2.5
+Version: 0.2.6
 Summary: Utilities that integrate advance scraping knowledge into just one library.
 Home-page: https://github.com/Data-Market/datamarket
 Author: DataMarket
 Author-email: techsupport@datamarket.es
 Project-URL: Website, https://datamarket.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

