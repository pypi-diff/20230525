# Comparing `tmp/freeGPT-1.0.4.tar.gz` & `tmp/freeGPT-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-krt1jqdf\freeGPT-1.0.4.tar", last modified: Thu May 25 14:46:45 2023, max compression
+gzip compressed data, was "C:\Users\Ruu3f\Downloads\freeGPT\dist\.tmp-b6xhp0fe\freeGPT-1.0.5.tar", last modified: Thu May 25 16:05:45 2023, max compression
```

## Comparing `freeGPT-1.0.4.tar` & `freeGPT-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 14:46:45.331867 freeGPT-1.0.4/
--rw-rw-rw-   0        0        0    35149 2023-05-25 14:45:39.000000 freeGPT-1.0.4/LICENSE
--rw-rw-rw-   0        0        0       98 2023-05-25 14:45:39.000000 freeGPT-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3275 2023-05-25 14:46:45.331867 freeGPT-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2271 2023-05-25 14:45:39.000000 freeGPT-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 14:46:45.331867 freeGPT-1.0.4/freeGPT/
--rw-rw-rw-   0        0        0      146 2023-05-25 14:45:39.000000 freeGPT-1.0.4/freeGPT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:46:45.331867 freeGPT-1.0.4/freeGPT/gpt3/
--rw-rw-rw-   0        0        0     2042 2023-05-25 14:45:39.000000 freeGPT-1.0.4/freeGPT/gpt3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:46:45.331867 freeGPT-1.0.4/freeGPT/gpt4/
--rw-rw-rw-   0        0        0     2662 2023-05-25 14:45:39.000000 freeGPT-1.0.4/freeGPT/gpt4/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:46:45.331867 freeGPT-1.0.4/freeGPT.egg-info/
--rw-rw-rw-   0        0        0     3275 2023-05-25 14:46:45.000000 freeGPT-1.0.4/freeGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-05-25 14:46:45.000000 freeGPT-1.0.4/freeGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 14:46:45.000000 freeGPT-1.0.4/freeGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-25 14:46:45.000000 freeGPT-1.0.4/freeGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-25 14:46:45.000000 freeGPT-1.0.4/freeGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 14:46:45.331867 freeGPT-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1396 2023-05-25 14:45:39.000000 freeGPT-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:05:45.142194 freeGPT-1.0.5/
+-rw-rw-rw-   0        0        0    35149 2023-05-25 15:14:10.000000 freeGPT-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0       98 2023-05-25 15:14:10.000000 freeGPT-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3273 2023-05-25 16:05:45.142194 freeGPT-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2269 2023-05-25 15:14:10.000000 freeGPT-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 16:05:45.126568 freeGPT-1.0.5/freeGPT/
+-rw-rw-rw-   0        0        0      144 2023-05-25 15:14:10.000000 freeGPT-1.0.5/freeGPT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:05:45.142194 freeGPT-1.0.5/freeGPT/gpt3/
+-rw-rw-rw-   0        0        0     2042 2023-05-25 15:14:10.000000 freeGPT-1.0.5/freeGPT/gpt3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:05:45.142194 freeGPT-1.0.5/freeGPT/gpt3web/
+-rw-rw-rw-   0        0        0     5176 2023-05-25 15:14:10.000000 freeGPT-1.0.5/freeGPT/gpt3web/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:05:45.142194 freeGPT-1.0.5/freeGPT/gpt4/
+-rw-rw-rw-   0        0        0     2662 2023-05-25 15:14:10.000000 freeGPT-1.0.5/freeGPT/gpt4/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:05:45.142194 freeGPT-1.0.5/freeGPT/gpt4web/
+-rw-rw-rw-   0        0        0     8418 2023-05-25 15:14:10.000000 freeGPT-1.0.5/freeGPT/gpt4web/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:05:45.142194 freeGPT-1.0.5/freeGPT.egg-info/
+-rw-rw-rw-   0        0        0     3273 2023-05-25 16:05:45.000000 freeGPT-1.0.5/freeGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-05-25 16:05:45.000000 freeGPT-1.0.5/freeGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 16:05:45.000000 freeGPT-1.0.5/freeGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-05-25 16:05:45.000000 freeGPT-1.0.5/freeGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-25 16:05:45.000000 freeGPT-1.0.5/freeGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 16:05:45.142194 freeGPT-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1396 2023-05-25 15:14:10.000000 freeGPT-1.0.5/setup.py
```

### Comparing `freeGPT-1.0.4/LICENSE` & `freeGPT-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.4/PKG-INFO` & `freeGPT-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.0.4
+Version: 1.0.5
 Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Keywords: artificial-intelligence,machine-learning,ai-models,freegpt,chatgpt,openai,gpt3gpt4gpt,ai
@@ -30,17 +30,17 @@
 
 ## Source:
 *Models with .web have internet access on.*
 <br>
 | Models            | Websites                                 |
 | ----------------- | -----------------------------------------|
 | gpt3              | [theb.ai](https://theb.ai)               |
-| gpt3.web          | [you.com](https://you.com)               |
+| gpt3web           | [you.com](https://you.com)               |
 | gpt4              | [usesless.com](https://ai.usesless.com)  |
-| gpt4.web          | [forefront.ai](https://chat.forefront.ai)|
+| gpt4web           | [forefront.ai](https://chat.forefront.ai)|
 
 ### TODO-List:
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
@@ -53,24 +53,24 @@
 - Star this repository :D
 
 ## Examples:
 
 #### GPT-3:
 
 ```python
-from freeGPT import gpt3 # If you want to use web just replace `gpt3` with `gpt3.web as gpt3` and no other changes needed.
+from freeGPT import gpt3 # If you want to use web just replace `gpt3` with `gpt3web as gpt3` and no other changes needed.
 
 prompt = input("👦 > ")
 resp = gpt3.Completion.create(prompt=prompt)
 print(f"🤖 > {resp.text}")
 ```
 #### GPT-4:
 
 ```python
-from freeGPT import gpt4  # If you want to use web just replace `gpt4` with `gpt4.web as gpt4` and no other changes needed.
+from freeGPT import gpt4  # If you want to use web just replace `gpt4` with `gpt4web as gpt4` and no other changes needed.
 
 token = gpt4.Account.create(logging=True) # Don't forget to remove this if you want to use web.
 prompt = input("👦 > ")
 resp = gpt4.Completion.create(prompt=prompt, token=token) # Don't forget to remove the token parameter here if you want to use web.
 print(f"🤖 > {resp.text}")
 ```
```

### Comparing `freeGPT-1.0.4/README.md` & `freeGPT-1.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 ## Source:
 *Models with .web have internet access on.*
 <br>
 | Models            | Websites                                 |
 | ----------------- | -----------------------------------------|
 | gpt3              | [theb.ai](https://theb.ai)               |
-| gpt3.web          | [you.com](https://you.com)               |
+| gpt3web           | [you.com](https://you.com)               |
 | gpt4              | [usesless.com](https://ai.usesless.com)  |
-| gpt4.web          | [forefront.ai](https://chat.forefront.ai)|
+| gpt4web           | [forefront.ai](https://chat.forefront.ai)|
 
 ### TODO-List:
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
@@ -31,24 +31,24 @@
 - Star this repository :D
 
 ## Examples:
 
 #### GPT-3:
 
 ```python
-from freeGPT import gpt3 # If you want to use web just replace `gpt3` with `gpt3.web as gpt3` and no other changes needed.
+from freeGPT import gpt3 # If you want to use web just replace `gpt3` with `gpt3web as gpt3` and no other changes needed.
 
 prompt = input("👦 > ")
 resp = gpt3.Completion.create(prompt=prompt)
 print(f"🤖 > {resp.text}")
 ```
 #### GPT-4:
 
 ```python
-from freeGPT import gpt4  # If you want to use web just replace `gpt4` with `gpt4.web as gpt4` and no other changes needed.
+from freeGPT import gpt4  # If you want to use web just replace `gpt4` with `gpt4web as gpt4` and no other changes needed.
 
 token = gpt4.Account.create(logging=True) # Don't forget to remove this if you want to use web.
 prompt = input("👦 > ")
 resp = gpt4.Completion.create(prompt=prompt, token=token) # Don't forget to remove the token parameter here if you want to use web.
 print(f"🤖 > {resp.text}")
 ```
```

### Comparing `freeGPT-1.0.4/freeGPT/gpt3/__init__.py` & `freeGPT-1.0.5/freeGPT/gpt3/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.4/freeGPT/gpt4/__init__.py` & `freeGPT-1.0.5/freeGPT/gpt4/__init__.py`

 * *Files identical despite different names*

### Comparing `freeGPT-1.0.4/freeGPT.egg-info/PKG-INFO` & `freeGPT-1.0.5/freeGPT.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeGPT
-Version: 1.0.4
+Version: 1.0.5
 Summary: freeGPT is a Python package that gives free access to GPT3 and GPT4 models.
 Home-page: https://github.com/Ruu3f/freeGPT
 Author: Ruu3f
 License: GPLv3
 Project-URL: Source, https://github.com/Ruu3f/freeGPT
 Project-URL: Issues, https://github.com/Ruu3f/freeGPT/issues
 Keywords: artificial-intelligence,machine-learning,ai-models,freegpt,chatgpt,openai,gpt3gpt4gpt,ai
@@ -30,17 +30,17 @@
 
 ## Source:
 *Models with .web have internet access on.*
 <br>
 | Models            | Websites                                 |
 | ----------------- | -----------------------------------------|
 | gpt3              | [theb.ai](https://theb.ai)               |
-| gpt3.web          | [you.com](https://you.com)               |
+| gpt3web           | [you.com](https://you.com)               |
 | gpt4              | [usesless.com](https://ai.usesless.com)  |
-| gpt4.web          | [forefront.ai](https://chat.forefront.ai)|
+| gpt4web           | [forefront.ai](https://chat.forefront.ai)|
 
 ### TODO-List:
 - [x] Add GPT-4.
 - [x] Make the library well-documented.
 - [x] Make the over-all library easier to use.
 - [x] Make the over-all library easier to understand.
 - [x] Replace you.com with theb.ai for less failed responses.
@@ -53,24 +53,24 @@
 - Star this repository :D
 
 ## Examples:
 
 #### GPT-3:
 
 ```python
-from freeGPT import gpt3 # If you want to use web just replace `gpt3` with `gpt3.web as gpt3` and no other changes needed.
+from freeGPT import gpt3 # If you want to use web just replace `gpt3` with `gpt3web as gpt3` and no other changes needed.
 
 prompt = input("👦 > ")
 resp = gpt3.Completion.create(prompt=prompt)
 print(f"🤖 > {resp.text}")
 ```
 #### GPT-4:
 
 ```python
-from freeGPT import gpt4  # If you want to use web just replace `gpt4` with `gpt4.web as gpt4` and no other changes needed.
+from freeGPT import gpt4  # If you want to use web just replace `gpt4` with `gpt4web as gpt4` and no other changes needed.
 
 token = gpt4.Account.create(logging=True) # Don't forget to remove this if you want to use web.
 prompt = input("👦 > ")
 resp = gpt4.Completion.create(prompt=prompt, token=token) # Don't forget to remove the token parameter here if you want to use web.
 print(f"🤖 > {resp.text}")
 ```
```

### Comparing `freeGPT-1.0.4/setup.py` & `freeGPT-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="freeGPT",
-    version="1.0.4",
+    version="1.0.5",
     description="freeGPT is a Python package that gives free access to GPT3 and GPT4 models.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ruu3f/freeGPT",
     author="Ruu3f",
     license="GPLv3",
     keywords=[
```

