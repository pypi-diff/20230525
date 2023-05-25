# Comparing `tmp/freeGPT-1.0.7.tar.gz` & `tmp/freeGPT-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-ws9kv_7k\freeGPT-1.0.7.tar", last modified: Thu May 25 16:52:16 2023, max compression
+gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-fr_ututs\freeGPT-1.0.8.tar", last modified: Thu May 25 17:06:54 2023, max compression
```

## Comparing `freeGPT-1.0.7.tar` & `freeGPT-1.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 16:52:16.110228 freeGPT-1.0.7/
--rw-rw-rw-   0        0        0    35149 2023-05-25 16:49:11.000000 freeGPT-1.0.7/LICENSE
--rw-rw-rw-   0        0        0       98 2023-05-25 16:49:11.000000 freeGPT-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     3273 2023-05-25 16:52:16.110228 freeGPT-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2269 2023-05-25 16:49:11.000000 freeGPT-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 16:52:16.110228 freeGPT-1.0.7/freeGPT/
--rw-rw-rw-   0        0        0       43 2023-05-25 16:49:11.000000 freeGPT-1.0.7/freeGPT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:52:16.110228 freeGPT-1.0.7/freeGPT/gpt3/
--rw-rw-rw-   0        0        0     2042 2023-05-25 16:49:11.000000 freeGPT-1.0.7/freeGPT/gpt3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:52:16.110228 freeGPT-1.0.7/freeGPT/gpt3web/
--rw-rw-rw-   0        0        0     5176 2023-05-25 16:49:11.000000 freeGPT-1.0.7/freeGPT/gpt3web/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:52:16.110228 freeGPT-1.0.7/freeGPT/gpt4/
--rw-rw-rw-   0        0        0     2662 2023-05-25 16:49:11.000000 freeGPT-1.0.7/freeGPT/gpt4/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:52:16.110228 freeGPT-1.0.7/freeGPT/gpt4web/
--rw-rw-rw-   0        0        0     8418 2023-05-25 16:49:11.000000 freeGPT-1.0.7/freeGPT/gpt4web/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:52:16.110228 freeGPT-1.0.7/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     3273 2023-05-25 16:52:16.000000 freeGPT-1.0.7/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-05-25 16:52:16.000000 freeGPT-1.0.7/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 16:52:16.000000 freeGPT-1.0.7/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-25 16:52:16.000000 freeGPT-1.0.7/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-25 16:52:16.000000 freeGPT-1.0.7/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 16:52:16.125857 freeGPT-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1396 2023-05-25 16:49:11.000000 freeGPT-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:06:54.041076 freeGPT-1.0.8/
+-rw-rw-rw-   0        0        0    35149 2023-05-25 17:06:10.000000 freeGPT-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0       98 2023-05-25 17:06:10.000000 freeGPT-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     3273 2023-05-25 17:06:54.041076 freeGPT-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2269 2023-05-25 17:06:10.000000 freeGPT-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 17:06:54.025448 freeGPT-1.0.8/freeGPT/
+-rw-rw-rw-   0        0        0     1336 2023-05-25 17:06:10.000000 freeGPT-1.0.8/freeGPT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:06:54.025448 freeGPT-1.0.8/freeGPT/gpt3/
+-rw-rw-rw-   0        0        0     2042 2023-05-25 17:06:10.000000 freeGPT-1.0.8/freeGPT/gpt3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:06:54.025448 freeGPT-1.0.8/freeGPT/gpt3web/
+-rw-rw-rw-   0        0        0     5176 2023-05-25 17:06:10.000000 freeGPT-1.0.8/freeGPT/gpt3web/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:06:54.025448 freeGPT-1.0.8/freeGPT/gpt4/
+-rw-rw-rw-   0        0        0     2662 2023-05-25 17:06:10.000000 freeGPT-1.0.8/freeGPT/gpt4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:06:54.025448 freeGPT-1.0.8/freeGPT/gpt4web/
+-rw-rw-rw-   0        0        0     8418 2023-05-25 17:06:10.000000 freeGPT-1.0.8/freeGPT/gpt4web/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:06:54.025448 freeGPT-1.0.8/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     3273 2023-05-25 17:06:53.000000 freeGPT-1.0.8/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-05-25 17:06:54.000000 freeGPT-1.0.8/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 17:06:53.000000 freeGPT-1.0.8/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-25 17:06:53.000000 freeGPT-1.0.8/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-25 17:06:53.000000 freeGPT-1.0.8/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 17:06:54.041076 freeGPT-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1396 2023-05-25 17:06:10.000000 freeGPT-1.0.8/setup.py
```

### Comparing `freeGPT-1.0.7/LICENSE` & `freeGPT-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.7/PKG-INFO` & `freeGPT-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.0.7
+Version: 1.0.8
 Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Keywords: artificial-intelligence,machine-learning,ai-models,freegpt,chatgpt,openai,gpt3gpt4gpt,ai
```

### Comparing `freeGPT-1.0.7/README.md` & `freeGPT-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.7/freeGPT/gpt3/__init__.py` & `freeGPT-1.0.8/freeGPT/gpt3/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.7/freeGPT/gpt3web/__init__.py` & `freeGPT-1.0.8/freeGPT/gpt3web/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.7/freeGPT/gpt4/__init__.py` & `freeGPT-1.0.8/freeGPT/gpt4/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.7/freeGPT/gpt4web/__init__.py` & `freeGPT-1.0.8/freeGPT/gpt4web/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.7/freeGPT.egg-info/PKG-INFO` & `freeGPT-1.0.8/freeGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.0.7
+Version: 1.0.8
 Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Keywords: artificial-intelligence,machine-learning,ai-models,freegpt,chatgpt,openai,gpt3gpt4gpt,ai
```

### Comparing `freeGPT-1.0.7/setup.py` & `freeGPT-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.0.7",
+    version="1.0.8",
     description="freeGPT is a Python package that gives free access to GPT3 and GPT4 models.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
     license="GPLv3",
     keywords=[
```

