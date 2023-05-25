# Comparing `tmp/fetchify-1.1.2.tar.gz` & `tmp/fetchify-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fetchify-1.1.2.tar", last modified: Thu May 25 02:30:03 2023, max compression
+gzip compressed data, was "fetchify-1.1.3.tar", last modified: Thu May 25 06:41:44 2023, max compression
```

## Comparing `fetchify-1.1.2.tar` & `fetchify-1.1.3.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 02:30:03.364882 fetchify-1.1.2/
--rw-rw-rw-   0        0        0      594 2023-05-25 02:30:03.363899 fetchify-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-05-19 11:17:31.000000 fetchify-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 02:30:03.361890 fetchify-1.1.2/fetchify.egg-info/
--rw-rw-rw-   0        0        0      594 2023-05-25 02:30:02.000000 fetchify-1.1.2/fetchify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-05-25 02:30:03.000000 fetchify-1.1.2/fetchify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 02:30:02.000000 fetchify-1.1.2/fetchify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-25 02:30:02.000000 fetchify-1.1.2/fetchify.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-25 02:30:02.000000 fetchify-1.1.2/fetchify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1321 2023-05-25 02:29:23.000000 fetchify-1.1.2/fetchify.py
--rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 fetchify-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 02:30:03.364882 fetchify-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      904 2023-05-25 02:29:33.000000 fetchify-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 06:41:44.710009 fetchify-1.1.3/
+-rw-rw-rw-   0        0        0      594 2023-05-25 06:41:44.710009 fetchify-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-05-25 06:31:58.000000 fetchify-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 06:41:44.710009 fetchify-1.1.3/fetchify.egg-info/
+-rw-rw-rw-   0        0        0      594 2023-05-25 06:41:44.000000 fetchify-1.1.3/fetchify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-05-25 06:41:44.000000 fetchify-1.1.3/fetchify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 06:41:44.000000 fetchify-1.1.3/fetchify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-25 06:41:44.000000 fetchify-1.1.3/fetchify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1408 2023-05-25 06:41:28.000000 fetchify-1.1.3/fetchify.py
+-rw-rw-rw-   0        0        0       86 2023-05-25 06:34:41.000000 fetchify-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 06:41:44.710009 fetchify-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      876 2023-05-25 06:35:02.000000 fetchify-1.1.3/setup.py
```

### Comparing `fetchify-1.1.2/PKG-INFO` & `fetchify-1.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fetchify
-Version: 1.1.2
+Version: 1.1.3
 Summary: Library to access Code Files from Cloud
 Home-page: https://techinfoak.wixsite.com/tech-info
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `fetchify-1.1.2/fetchify.egg-info/PKG-INFO` & `fetchify-1.1.3/fetchify.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fetchify
-Version: 1.1.2
+Version: 1.1.3
 Summary: Library to access Code Files from Cloud
 Home-page: https://techinfoak.wixsite.com/tech-info
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `fetchify-1.1.2/fetchify.py` & `fetchify-1.1.3/fetchify.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 """This a library that mean't to access files from github repo without opening it again and again"""
 
 import requests
 
-url1 = "https://raw.githubusercontent.com/Anupam1707/Python_Programmes/main/"
-url2 = "https://raw.githubusercontent.com/Anupam1707/weather-app-py/main/"
-url3 = "https://raw.githubusercontent.com/Anupam1707/ai/main/"
-url4 = "https://raw.githubusercontent.com/Anupam1707/datasense/main/"
-url5 = "https://raw.githubusercontent.com/Anupam1707/SecuriPy/main/"
+py = "https://raw.githubusercontent.com/Anupam1707/Python_Programmes/main/"
+we = "https://raw.githubusercontent.com/Anupam1707/weather-app-py/main/"
+aiu = "https://raw.githubusercontent.com/Anupam1707/ai/main/"
+ds = "https://raw.githubusercontent.com/Anupam1707/datasense/main/"
+spy = "https://raw.githubusercontent.com/Anupam1707/SecuriPy/main/"
 
 def python(filename):
     """To access files from the Repository 'Python'"""
-    page = requests.get(url1 + filename)
+    page = requests.get(py + filename)
     return page.text
 
 def weather(filename):
     """To access files from the Repository 'weather'"""
-    page = requests.get(url2 + filename)
+    page = requests.get(we + filename)
     return page.text
 
 def ai(filename):
     """To access files from the Repository 'ai'"""
-    page = requests.get(url3 + filename)
+    page = requests.get(aiu + filename)
     return page.text
 
 def sense(filename):
-    """To access files from the Repository 'food'"""
-    page = requests.get(url4 + filename)
+    """To access files from the Repository 'datasense'"""
+    page = requests.get(ds + filename)
     return page.text
 
 def secure(filename):
     """To access files from the Repository 'SecuriPy'"""
-    page = request.get(url + filename)
+    page = request.get(spy + filename)
     return page.text
 
 def save(file, name):
     with open(f"{name}", "w", encoding = "utf-8", newline = "") as f:
-        f.writelines(file)
+        f.writelines(file)
+
+def image(filename, url):
+    page = requests.get(url+filename)
+    return page.content
+
```

### Comparing `fetchify-1.1.2/setup.py` & `fetchify-1.1.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fetchify",
-    version="1.1.2",
+    version="1.1.3",
     author="Anupam Kanoongo",
     author_email="programmer.tiak@gmail.com",
     description="Library to access Code Files from Cloud",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://techinfoak.wixsite.com/tech-info",
     project_urls={
-        "Our Website": "https://techinfoak.wixsite.com/tech-info",
-        "Our YT Handle": "https://youtube.com/@techinfoak"
+            "Our Website": "https://techinfoak.wixsite.com/tech-info",
+            "Our YT Handle": "https://youtube.com/@techinfoak"
     },
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=['requests'],
     py_modules=["fetchify"],
     python_requires=">=3.6"
 )
```

