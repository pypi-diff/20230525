# Comparing `tmp/IMDBTraktSyncer-1.2.7.tar.gz` & `tmp/IMDBTraktSyncer-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.2.7.tar", last modified: Wed May 24 22:06:49 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.2.9.tar", last modified: Wed May 24 23:33:14 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.2.7.tar` & `IMDBTraktSyncer-1.2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 22:06:49.255229 IMDBTraktSyncer-1.2.7/
-drwxrwxrwx   0        0        0        0 2023-05-24 22:06:49.222344 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    22282 2023-05-24 22:01:23.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1900 2023-05-23 23:43:19.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4079 2023-05-16 01:53:33.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     3845 2023-05-20 20:45:06.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     7752 2023-05-24 22:03:34.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0     5841 2023-05-23 23:18:31.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0     6981 2023-05-23 22:09:09.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-24 22:06:49.252344 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     8556 2023-05-24 22:06:49.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2023-05-24 22:06:49.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 22:06:49.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-24 22:06:49.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-05-24 22:06:49.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-24 22:06:49.000000 IMDBTraktSyncer-1.2.7/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.2.7/LICENSE
--rw-rw-rw-   0        0        0     8556 2023-05-24 22:06:49.255229 IMDBTraktSyncer-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     7856 2023-05-24 22:06:25.000000 IMDBTraktSyncer-1.2.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-24 22:06:49.255229 IMDBTraktSyncer-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1347 2023-05-24 22:06:09.000000 IMDBTraktSyncer-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 23:33:14.989164 IMDBTraktSyncer-1.2.9/
+drwxrwxrwx   0        0        0        0 2023-05-24 23:33:14.964166 IMDBTraktSyncer-1.2.9/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    22282 2023-05-24 22:01:23.000000 IMDBTraktSyncer-1.2.9/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.2.9/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1900 2023-05-23 23:43:19.000000 IMDBTraktSyncer-1.2.9/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4207 2023-05-24 23:10:07.000000 IMDBTraktSyncer-1.2.9/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     3845 2023-05-20 20:45:06.000000 IMDBTraktSyncer-1.2.9/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     7752 2023-05-24 22:03:34.000000 IMDBTraktSyncer-1.2.9/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0     5841 2023-05-23 23:18:31.000000 IMDBTraktSyncer-1.2.9/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0     6981 2023-05-23 22:09:09.000000 IMDBTraktSyncer-1.2.9/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-24 23:33:14.986179 IMDBTraktSyncer-1.2.9/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     8556 2023-05-24 23:33:14.000000 IMDBTraktSyncer-1.2.9/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2023-05-24 23:33:14.000000 IMDBTraktSyncer-1.2.9/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 23:33:14.000000 IMDBTraktSyncer-1.2.9/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-24 23:33:14.000000 IMDBTraktSyncer-1.2.9/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-05-24 23:33:14.000000 IMDBTraktSyncer-1.2.9/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-24 23:33:14.000000 IMDBTraktSyncer-1.2.9/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0     8556 2023-05-24 23:33:14.988179 IMDBTraktSyncer-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7856 2023-05-24 22:06:25.000000 IMDBTraktSyncer-1.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-24 23:33:14.989164 IMDBTraktSyncer-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1347 2023-05-24 23:32:30.000000 IMDBTraktSyncer-1.2.9/setup.py
```

### Comparing `IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.2.9/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.2.9/IMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.2.9/IMDBTraktSyncer/checkChromedriver.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import feedparser
 import subprocess
 import pkg_resources
 import platform
+import sys
 
 def get_chrome_version():
     system = platform.system()
     if system == 'Windows':
         from winreg import ConnectRegistry, HKEY_CURRENT_USER, OpenKey, QueryValueEx
 
         try:
@@ -34,25 +35,25 @@
             return version
         except:
             return None
 
     return None
 
 def install_chromedriver(version):
-    # Install the chromedriver-py package using pip
-    subprocess.run(['pip', 'install', f'chromedriver-py=={version}'])
+    # Install the chromedriver-py package using the Python interpreter
+    subprocess.run([sys.executable, '-m', 'pip', 'install', '--no-cache-dir' f'chromedriver-py=={version}'])
 
 def install_chromedriver_fallback_method():
     print("Using install chromedriver-py fallback method")
-    # Install the chromedriver-py package using pip
+    # Install the chromedriver-py package using the Python interpreter
     feed = feedparser.parse('https://pypi.org/rss/project/chromedriver-py/releases.xml')
     # Get the second latest release version
     version = feed.entries[1].title.split()[-1]
     # Install the chromedriver-py package using pip
-    subprocess.run(['pip', 'install', f'chromedriver-py=={version}'])
+    subprocess.run([sys.executable, '-m', 'pip', 'install', '--no-cache-dir' f'chromedriver-py=={version}'])
 
 # Check if chromedriver-py is already installed
 try:
     dist = pkg_resources.get_distribution('chromedriver-py')
     installed_version = dist.version.split('.')[0]  # Retrieve only the prefix
     chrome_version = get_chrome_version()
```

### Comparing `IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/errorHandling.py` & `IMDBTraktSyncer-1.2.9/IMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.2.9/IMDBTraktSyncer/imdbData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.2.9/IMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.7/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.2.9/IMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.7/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.2.9/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.2.7
+Version: 1.2.9
 Summary: This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `IMDBTraktSyncer-1.2.7/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.2.9/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.7/LICENSE` & `IMDBTraktSyncer-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.7/PKG-INFO` & `IMDBTraktSyncer-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.2.7
+Version: 1.2.9
 Summary: This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `IMDBTraktSyncer-1.2.7/README.md` & `IMDBTraktSyncer-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.2.7/setup.py` & `IMDBTraktSyncer-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.2.7'
+VERSION = '1.2.9'
 DESCRIPTION = 'This python script syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

