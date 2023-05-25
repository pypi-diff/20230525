# Comparing `tmp/datamarket-0.3.1.tar.gz` & `tmp/datamarket-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamarket-0.3.1.tar", last modified: Thu May 25 14:26:48 2023, max compression
+gzip compressed data, was "datamarket-0.3.2.tar", last modified: Thu May 25 14:40:59 2023, max compression
```

## Comparing `datamarket-0.3.1.tar` & `datamarket-0.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 14:26:48.424753 datamarket-0.3.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35149 2021-10-07 14:37:41.000000 datamarket-0.3.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1486 2023-05-25 14:26:48.424753 datamarket-0.3.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      934 2023-05-25 14:26:25.000000 datamarket-0.3.1/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-25 14:26:48.424753 datamarket-0.3.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1050 2023-05-25 14:26:25.000000 datamarket-0.3.1/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 14:26:48.420753 datamarket-0.3.1/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 14:26:48.420753 datamarket-0.3.1/src/datamarket/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2021-11-03 08:15:04.000000 datamarket-0.3.1/src/datamarket/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 14:26:48.424753 datamarket-0.3.1/src/datamarket/interfaces/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-03 09:55:33.000000 datamarket-0.3.1/src/datamarket/interfaces/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3104 2023-02-16 08:03:41.000000 datamarket-0.3.1/src/datamarket/interfaces/alchemy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2022-08-08 10:00:49.000000 datamarket-0.3.1/src/datamarket/interfaces/drive.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1344 2023-02-17 11:31:46.000000 datamarket-0.3.1/src/datamarket/interfaces/ftp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2023-04-14 11:21:25.000000 datamarket-0.3.1/src/datamarket/interfaces/proxy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2565 2023-03-14 07:00:34.000000 datamarket-0.3.1/src/datamarket/interfaces/tinybird.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 14:26:48.424753 datamarket-0.3.1/src/datamarket/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 14:09:14.000000 datamarket-0.3.1/src/datamarket/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1738 2023-05-25 14:18:08.000000 datamarket-0.3.1/src/datamarket/utils/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2054 2023-05-25 14:19:10.000000 datamarket-0.3.1/src/datamarket/utils/selenium.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 14:26:48.420753 datamarket-0.3.1/src/datamarket.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1486 2023-05-25 14:26:48.000000 datamarket-0.3.1/src/datamarket.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      553 2023-05-25 14:26:48.000000 datamarket-0.3.1/src/datamarket.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-25 14:26:48.000000 datamarket-0.3.1/src/datamarket.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       70 2023-05-25 14:26:48.000000 datamarket-0.3.1/src/datamarket.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-05-25 14:26:48.000000 datamarket-0.3.1/src/datamarket.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 14:40:59.279490 datamarket-0.3.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    35149 2021-10-07 14:37:41.000000 datamarket-0.3.2/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1486 2023-05-25 14:40:59.279490 datamarket-0.3.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      934 2023-05-25 14:26:25.000000 datamarket-0.3.2/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-25 14:40:59.279490 datamarket-0.3.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1050 2023-05-25 14:40:06.000000 datamarket-0.3.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 14:40:59.279490 datamarket-0.3.2/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 14:40:59.279490 datamarket-0.3.2/src/datamarket/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2021-11-03 08:15:04.000000 datamarket-0.3.2/src/datamarket/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 14:40:59.279490 datamarket-0.3.2/src/datamarket/interfaces/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-03 09:55:33.000000 datamarket-0.3.2/src/datamarket/interfaces/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3104 2023-02-16 08:03:41.000000 datamarket-0.3.2/src/datamarket/interfaces/alchemy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2022-08-08 10:00:49.000000 datamarket-0.3.2/src/datamarket/interfaces/drive.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1344 2023-02-17 11:31:46.000000 datamarket-0.3.2/src/datamarket/interfaces/ftp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2913 2023-04-14 11:21:25.000000 datamarket-0.3.2/src/datamarket/interfaces/proxy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2565 2023-03-14 07:00:34.000000 datamarket-0.3.2/src/datamarket/interfaces/tinybird.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 14:40:59.279490 datamarket-0.3.2/src/datamarket/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 14:09:14.000000 datamarket-0.3.2/src/datamarket/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1738 2023-05-25 14:18:08.000000 datamarket-0.3.2/src/datamarket/utils/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2034 2023-05-25 14:40:06.000000 datamarket-0.3.2/src/datamarket/utils/selenium.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 14:40:59.279490 datamarket-0.3.2/src/datamarket.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1486 2023-05-25 14:40:59.000000 datamarket-0.3.2/src/datamarket.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      553 2023-05-25 14:40:59.000000 datamarket-0.3.2/src/datamarket.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-25 14:40:59.000000 datamarket-0.3.2/src/datamarket.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       70 2023-05-25 14:40:59.000000 datamarket-0.3.2/src/datamarket.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-05-25 14:40:59.000000 datamarket-0.3.2/src/datamarket.egg-info/top_level.txt
```

### Comparing `datamarket-0.3.1/LICENSE` & `datamarket-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.1/PKG-INFO` & `datamarket-0.3.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamarket
-Version: 0.3.1
+Version: 0.3.2
 Summary: Utilities that integrate advance scraping knowledge into just one library.
 Home-page: https://github.com/Data-Market/datamarket
 Author: DataMarket
 Author-email: techsupport@datamarket.es
 Project-URL: Website, https://datamarket.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `datamarket-0.3.1/README.md` & `datamarket-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.1/setup.py` & `datamarket-0.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "stem",
     "pydrive",
     "undetected_chromedriver",
 ]
 
 setuptools.setup(
     name="datamarket",
-    version="0.3.1",
+    version="0.3.2",
     author="DataMarket",
     author_email="techsupport@datamarket.es",
     description="Utilities that integrate advance scraping knowledge into just one library.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Data-Market/datamarket",
     project_urls={
```

### Comparing `datamarket-0.3.1/src/datamarket/interfaces/alchemy.py` & `datamarket-0.3.2/src/datamarket/interfaces/alchemy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.1/src/datamarket/interfaces/drive.py` & `datamarket-0.3.2/src/datamarket/interfaces/drive.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.1/src/datamarket/interfaces/ftp.py` & `datamarket-0.3.2/src/datamarket/interfaces/ftp.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.1/src/datamarket/interfaces/proxy.py` & `datamarket-0.3.2/src/datamarket/interfaces/proxy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.1/src/datamarket/interfaces/tinybird.py` & `datamarket-0.3.2/src/datamarket/interfaces/tinybird.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.1/src/datamarket/utils/main.py` & `datamarket-0.3.2/src/datamarket/utils/main.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.3.1/src/datamarket/utils/selenium.py` & `datamarket-0.3.2/src/datamarket/utils/selenium.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,23 +19,23 @@
     return int(
         run_bash_command("/usr/bin/google-chrome --version")
         .split(" ")[2]
         .split(".")[0]
     )
 
 
-def get_driver(self, chrome_options=None):
+def get_driver(chrome_options=None):
     options = uc.ChromeOptions()
 
     if isinstance(chrome_options, list):
         for option in chrome_options:
             options.add_argument(option)
 
-    self.driver = uc.Chrome(version_main=get_chromedriver_version(),
-                            options=options)
+    return uc.Chrome(version_main=get_chromedriver_version(),
+                     options=options)
 
 
 def wait(driver, css_selector, timeout=30):
     logger.info(f"waiting for {css_selector}...")
     return WebDriverWait(driver, timeout).until(EC.element_to_be_clickable(("css selector", css_selector)))
```

### Comparing `datamarket-0.3.1/src/datamarket.egg-info/PKG-INFO` & `datamarket-0.3.2/src/datamarket.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamarket
-Version: 0.3.1
+Version: 0.3.2
 Summary: Utilities that integrate advance scraping knowledge into just one library.
 Home-page: https://github.com/Data-Market/datamarket
 Author: DataMarket
 Author-email: techsupport@datamarket.es
 Project-URL: Website, https://datamarket.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `datamarket-0.3.1/src/datamarket.egg-info/SOURCES.txt` & `datamarket-0.3.2/src/datamarket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

