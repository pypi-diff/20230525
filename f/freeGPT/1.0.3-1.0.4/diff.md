# Comparing `tmp/freeGPT-1.0.3.tar.gz` & `tmp/freeGPT-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-oyiaf5f4\freeGPT-1.0.3.tar", last modified: Thu May 25 14:39:04 2023, max compression
+gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-krt1jqdf\freeGPT-1.0.4.tar", last modified: Thu May 25 14:46:45 2023, max compression
```

## Comparing `freeGPT-1.0.3.tar` & `freeGPT-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 14:39:04.667060 freeGPT-1.0.3/
--rw-rw-rw-   0        0        0    35149 2023-05-25 14:37:43.000000 freeGPT-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       98 2023-05-25 14:37:43.000000 freeGPT-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3265 2023-05-25 14:39:04.667060 freeGPT-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2261 2023-05-25 14:37:43.000000 freeGPT-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 14:39:04.667060 freeGPT-1.0.3/freeGPT/
--rw-rw-rw-   0        0        0      146 2023-05-25 14:37:43.000000 freeGPT-1.0.3/freeGPT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:39:04.667060 freeGPT-1.0.3/freeGPT/gpt3/
--rw-rw-rw-   0        0        0     2042 2023-05-25 14:37:43.000000 freeGPT-1.0.3/freeGPT/gpt3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:39:04.667060 freeGPT-1.0.3/freeGPT/gpt4/
--rw-rw-rw-   0        0        0     2662 2023-05-25 14:37:43.000000 freeGPT-1.0.3/freeGPT/gpt4/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:39:04.667060 freeGPT-1.0.3/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     3265 2023-05-25 14:39:04.000000 freeGPT-1.0.3/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-05-25 14:39:04.000000 freeGPT-1.0.3/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 14:39:04.000000 freeGPT-1.0.3/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-25 14:39:04.000000 freeGPT-1.0.3/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-25 14:39:04.000000 freeGPT-1.0.3/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 14:39:04.667060 freeGPT-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1396 2023-05-25 14:37:43.000000 freeGPT-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:46:45.331867 freeGPT-1.0.4/
+-rw-rw-rw-   0        0        0    35149 2023-05-25 14:45:39.000000 freeGPT-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0       98 2023-05-25 14:45:39.000000 freeGPT-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3275 2023-05-25 14:46:45.331867 freeGPT-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2271 2023-05-25 14:45:39.000000 freeGPT-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 14:46:45.331867 freeGPT-1.0.4/freeGPT/
+-rw-rw-rw-   0        0        0      146 2023-05-25 14:45:39.000000 freeGPT-1.0.4/freeGPT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:46:45.331867 freeGPT-1.0.4/freeGPT/gpt3/
+-rw-rw-rw-   0        0        0     2042 2023-05-25 14:45:39.000000 freeGPT-1.0.4/freeGPT/gpt3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:46:45.331867 freeGPT-1.0.4/freeGPT/gpt4/
+-rw-rw-rw-   0        0        0     2662 2023-05-25 14:45:39.000000 freeGPT-1.0.4/freeGPT/gpt4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 14:46:45.331867 freeGPT-1.0.4/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     3275 2023-05-25 14:46:45.000000 freeGPT-1.0.4/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-05-25 14:46:45.000000 freeGPT-1.0.4/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 14:46:45.000000 freeGPT-1.0.4/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-25 14:46:45.000000 freeGPT-1.0.4/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-25 14:46:45.000000 freeGPT-1.0.4/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 14:46:45.331867 freeGPT-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1396 2023-05-25 14:45:39.000000 freeGPT-1.0.4/setup.py
```

### Comparing `freeGPT-1.0.3/LICENSE` & `freeGPT-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.3/PKG-INFO` & `freeGPT-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.0.3
+Version: 1.0.4
 Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Keywords: artificial-intelligence,machine-learning,ai-models,freegpt,chatgpt,openai,gpt3gpt4gpt,ai
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/freeGPT.svg)](https://badge.fury.io/py/freeGPT)
 [![Downloads](https://static.pepy.tech/personalized-badge/freeGPT?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/freeGPT)
-[![License](https://img.shields.io/badge/License-MIT-bright&green.svg)](LICENSE)
+[![License](https://img.shields.io/badge/License-GPLv3-bright&green.svg)](LICENSE)
 # freeGPT
 A Python package that gives access to GPT3 &amp; GPT4 models for free.
 <br>
 *Get started by doing: `pip install freeGPT`*
 
 ## Source:
 *Models with .web have internet access on.*
@@ -41,15 +41,15 @@
 ### TODO-List:
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
 - [x] Add a internet search model for GPT-3 & GPT-4
-- [ ] Add text to image generation
+- [ ] Add a text to image generation model
 - [ ] Make a discord bot
 
 ## Support me:
 - Join my [Discord Server](https://discord.gg/NcQ26PrNDp) :D
 - Star this repository :D
 
 ## Examples:
```

### Comparing `freeGPT-1.0.3/README.md` & `freeGPT-1.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![PyPI version](https://badge.fury.io/py/freeGPT.svg)](https://badge.fury.io/py/freeGPT)
 [![Downloads](https://static.pepy.tech/personalized-badge/freeGPT?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/freeGPT)
-[![License](https://img.shields.io/badge/License-MIT-bright&green.svg)](LICENSE)
+[![License](https://img.shields.io/badge/License-GPLv3-bright&green.svg)](LICENSE)
 # freeGPT
 A Python package that gives access to GPT3 &amp; GPT4 models for free.
 <br>
 *Get started by doing: `pip install freeGPT`*
 
 ## Source:
 *Models with .web have internet access on.*
@@ -19,15 +19,15 @@
 ### TODO-List:
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
 - [x] Add a internet search model for GPT-3 & GPT-4
-- [ ] Add text to image generation
+- [ ] Add a text to image generation model
 - [ ] Make a discord bot
 
 ## Support me:
 - Join my [Discord Server](https://discord.gg/NcQ26PrNDp) :D
 - Star this repository :D
 
 ## Examples:
```

### Comparing `freeGPT-1.0.3/freeGPT/gpt3/__init__.py` & `freeGPT-1.0.4/freeGPT/gpt3/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.3/freeGPT/gpt4/__init__.py` & `freeGPT-1.0.4/freeGPT/gpt4/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.3/freeGPT.egg-info/PKG-INFO` & `freeGPT-1.0.4/freeGPT.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.0.3
+Version: 1.0.4
 Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Keywords: artificial-intelligence,machine-learning,ai-models,freegpt,chatgpt,openai,gpt3gpt4gpt,ai
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/freeGPT.svg)](https://badge.fury.io/py/freeGPT)
 [![Downloads](https://static.pepy.tech/personalized-badge/freeGPT?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/freeGPT)
-[![License](https://img.shields.io/badge/License-MIT-bright&green.svg)](LICENSE)
+[![License](https://img.shields.io/badge/License-GPLv3-bright&green.svg)](LICENSE)
 # freeGPT
 A Python package that gives access to GPT3 &amp; GPT4 models for free.
 <br>
 *Get started by doing: `pip install freeGPT`*
 
 ## Source:
 *Models with .web have internet access on.*
@@ -41,15 +41,15 @@
 ### TODO-List:
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
 - [x] Add a internet search model for GPT-3 & GPT-4
-- [ ] Add text to image generation
+- [ ] Add a text to image generation model
 - [ ] Make a discord bot
 
 ## Support me:
 - Join my [Discord Server](https://discord.gg/NcQ26PrNDp) :D
 - Star this repository :D
 
 ## Examples:
```

### Comparing `freeGPT-1.0.3/setup.py` & `freeGPT-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.0.3",
+    version="1.0.4",
     description="freeGPT is a Python package that gives free access to GPT3 and GPT4 models.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
     license="GPLv3",
     keywords=[
```

