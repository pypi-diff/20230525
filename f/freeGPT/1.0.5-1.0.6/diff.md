# Comparing `tmp/freeGPT-1.0.5.tar.gz` & `tmp/freeGPT-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-b6xhp0fe\freeGPT-1.0.5.tar", last modified: Thu May 25 16:05:45 2023, max compression
+gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-jutjxjvv\freeGPT-1.0.6.tar", last modified: Thu May 25 16:35:34 2023, max compression
```

## Comparing `freeGPT-1.0.5.tar` & `freeGPT-1.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 16:05:45.142194 freeGPT-1.0.5/
--rw-rw-rw-   0        0        0    35149 2023-05-25 15:14:10.000000 freeGPT-1.0.5/LICENSE
--rw-rw-rw-   0        0        0       98 2023-05-25 15:14:10.000000 freeGPT-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3273 2023-05-25 16:05:45.142194 freeGPT-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2269 2023-05-25 15:14:10.000000 freeGPT-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 16:05:45.126568 freeGPT-1.0.5/freeGPT/
--rw-rw-rw-   0        0        0      144 2023-05-25 15:14:10.000000 freeGPT-1.0.5/freeGPT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:05:45.142194 freeGPT-1.0.5/freeGPT/gpt3/
--rw-rw-rw-   0        0        0     2042 2023-05-25 15:14:10.000000 freeGPT-1.0.5/freeGPT/gpt3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:05:45.142194 freeGPT-1.0.5/freeGPT/gpt3web/
--rw-rw-rw-   0        0        0     5176 2023-05-25 15:14:10.000000 freeGPT-1.0.5/freeGPT/gpt3web/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:05:45.142194 freeGPT-1.0.5/freeGPT/gpt4/
--rw-rw-rw-   0        0        0     2662 2023-05-25 15:14:10.000000 freeGPT-1.0.5/freeGPT/gpt4/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:05:45.142194 freeGPT-1.0.5/freeGPT/gpt4web/
--rw-rw-rw-   0        0        0     8418 2023-05-25 15:14:10.000000 freeGPT-1.0.5/freeGPT/gpt4web/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:05:45.142194 freeGPT-1.0.5/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     3273 2023-05-25 16:05:45.000000 freeGPT-1.0.5/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-05-25 16:05:45.000000 freeGPT-1.0.5/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 16:05:45.000000 freeGPT-1.0.5/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-25 16:05:45.000000 freeGPT-1.0.5/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-25 16:05:45.000000 freeGPT-1.0.5/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 16:05:45.142194 freeGPT-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1396 2023-05-25 15:14:10.000000 freeGPT-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:35:34.111502 freeGPT-1.0.6/
+-rw-rw-rw-   0        0        0    35149 2023-05-25 15:14:10.000000 freeGPT-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0       98 2023-05-25 15:14:10.000000 freeGPT-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     3273 2023-05-25 16:35:34.111502 freeGPT-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2269 2023-05-25 15:14:10.000000 freeGPT-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 16:35:34.048962 freeGPT-1.0.6/freeGPT/
+-rw-rw-rw-   0        0        0      142 2023-05-25 16:33:26.000000 freeGPT-1.0.6/freeGPT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:35:34.048962 freeGPT-1.0.6/freeGPT/gpt3/
+-rw-rw-rw-   0        0        0     2042 2023-05-25 15:14:10.000000 freeGPT-1.0.6/freeGPT/gpt3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:35:34.064620 freeGPT-1.0.6/freeGPT/gpt3web/
+-rw-rw-rw-   0        0        0     5176 2023-05-25 15:14:10.000000 freeGPT-1.0.6/freeGPT/gpt3web/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:35:34.080248 freeGPT-1.0.6/freeGPT/gpt4/
+-rw-rw-rw-   0        0        0     2662 2023-05-25 15:14:10.000000 freeGPT-1.0.6/freeGPT/gpt4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:35:34.080248 freeGPT-1.0.6/freeGPT/gpt4web/
+-rw-rw-rw-   0        0        0     8418 2023-05-25 15:14:10.000000 freeGPT-1.0.6/freeGPT/gpt4web/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:35:34.048962 freeGPT-1.0.6/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     3273 2023-05-25 16:35:33.000000 freeGPT-1.0.6/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-05-25 16:35:34.000000 freeGPT-1.0.6/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 16:35:33.000000 freeGPT-1.0.6/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-25 16:35:33.000000 freeGPT-1.0.6/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-25 16:35:33.000000 freeGPT-1.0.6/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 16:35:34.111502 freeGPT-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1396 2023-05-25 16:33:21.000000 freeGPT-1.0.6/setup.py
```

### Comparing `freeGPT-1.0.5/LICENSE` & `freeGPT-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.5/PKG-INFO` & `freeGPT-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.0.5
+Version: 1.0.6
 Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Keywords: artificial-intelligence,machine-learning,ai-models,freegpt,chatgpt,openai,gpt3gpt4gpt,ai
```

### Comparing `freeGPT-1.0.5/README.md` & `freeGPT-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.5/freeGPT/gpt3/__init__.py` & `freeGPT-1.0.6/freeGPT/gpt3/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.5/freeGPT/gpt3web/__init__.py` & `freeGPT-1.0.6/freeGPT/gpt3web/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.5/freeGPT/gpt4/__init__.py` & `freeGPT-1.0.6/freeGPT/gpt4/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.5/freeGPT/gpt4web/__init__.py` & `freeGPT-1.0.6/freeGPT/gpt4web/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.5/freeGPT.egg-info/PKG-INFO` & `freeGPT-1.0.6/freeGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.0.5
+Version: 1.0.6
 Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Keywords: artificial-intelligence,machine-learning,ai-models,freegpt,chatgpt,openai,gpt3gpt4gpt,ai
```

### Comparing `freeGPT-1.0.5/setup.py` & `freeGPT-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.0.5",
+    version="1.0.6",
     description="freeGPT is a Python package that gives free access to GPT3 and GPT4 models.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
     license="GPLv3",
     keywords=[
```

