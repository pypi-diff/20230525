# Comparing `tmp/corby-0.0.8.tar.gz` & `tmp/corby-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corby-0.0.8.tar", last modified: Thu May 25 09:24:33 2023, max compression
+gzip compressed data, was "corby-0.0.9.tar", last modified: Thu May 25 11:24:59 2023, max compression
```

## Comparing `corby-0.0.8.tar` & `corby-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:24:33.139398 corby-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-25 09:24:14.000000 corby-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-25 09:24:33.139398 corby-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-25 09:24:14.000000 corby-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:24:33.135398 corby-0.0.8/corby/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-25 09:24:14.000000 corby-0.0.8/corby/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-25 09:24:14.000000 corby-0.0.8/corby/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:24:33.139398 corby-0.0.8/corby/generator/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-25 09:24:14.000000 corby-0.0.8/corby/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-25 09:24:14.000000 corby-0.0.8/corby/generator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:24:33.139398 corby-0.0.8/corby/generator/chatbot/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-25 09:24:14.000000 corby-0.0.8/corby/generator/chatbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-25 09:24:14.000000 corby-0.0.8/corby/generator/chatbot/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-25 09:24:14.000000 corby-0.0.8/corby/generator/chatbot/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-25 09:24:14.000000 corby-0.0.8/corby/index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:24:33.135398 corby-0.0.8/corby.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-25 09:24:33.000000 corby-0.0.8/corby.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-25 09:24:33.000000 corby-0.0.8/corby.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:24:33.000000 corby-0.0.8/corby.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-25 09:24:33.000000 corby-0.0.8/corby.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 09:24:33.000000 corby-0.0.8/corby.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 09:24:33.139398 corby-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-25 09:24:14.000000 corby-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:24:59.033194 corby-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-25 11:24:42.000000 corby-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-25 11:24:59.033194 corby-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-25 11:24:42.000000 corby-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:24:59.029194 corby-0.0.9/corby/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-25 11:24:42.000000 corby-0.0.9/corby/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-25 11:24:42.000000 corby-0.0.9/corby/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:24:59.029194 corby-0.0.9/corby/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-25 11:24:42.000000 corby-0.0.9/corby/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-25 11:24:42.000000 corby-0.0.9/corby/generator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:24:59.033194 corby-0.0.9/corby/generator/chatbot/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-25 11:24:42.000000 corby-0.0.9/corby/generator/chatbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-25 11:24:42.000000 corby-0.0.9/corby/generator/chatbot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-25 11:24:42.000000 corby-0.0.9/corby/generator/chatbot/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-25 11:24:42.000000 corby-0.0.9/corby/index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:24:59.029194 corby-0.0.9/corby.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-25 11:24:59.000000 corby-0.0.9/corby.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-25 11:24:59.000000 corby-0.0.9/corby.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:24:59.000000 corby-0.0.9/corby.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-25 11:24:59.000000 corby-0.0.9/corby.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 11:24:59.000000 corby-0.0.9/corby.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:24:59.033194 corby-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-25 11:24:42.000000 corby-0.0.9/setup.py
```

### Comparing `corby-0.0.8/LICENSE` & `corby-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `corby-0.0.8/PKG-INFO` & `corby-0.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,12 @@
-Metadata-Version: 2.1
-Name: corby
-Version: 0.0.8
-Summary: ⚡ Create your LLMs applications from zero to deploy in minutes ⚡
-Author: Jose Hervás Díaz
-Author-email: jhervasdiaz@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 🤖 Corby
 
-⚡ Create your LLMs applications from zero to deploy in minutes ⚡
+⚡ Create your AI applications from zero to deploy in minutes ⚡
 
-![pylint](https://github.com/JoseHervas/corby/actions/workflows/pylint.yml/badge.svg) [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-360/) ![version](https://img.shields.io/badge/version-0.0.7-blue) [![License: GPL-3](https://img.shields.io/badge/License-GPL3-green.svg)](https://opensource.org/licenses/GPL-3)
+![pypi](https://github.com/JoseHervas/corby/actions/workflows/publish.yml/badge.svg) ![pylint](https://github.com/JoseHervas/corby/actions/workflows/pylint.yml/badge.svg) [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-360/) [![Downloads](https://static.pepy.tech/badge/corby)](https://pepy.tech/project/corby) [![License: GPL-3](https://img.shields.io/badge/License-GPL3-green.svg)](https://opensource.org/licenses/GPL-3)
 
 ## 🚀 Quick Install
 
 ```bash
 pip install corby
 alias corby="python -m corby"
 ```
```

### Comparing `corby-0.0.8/corby/generator/base.py` & `corby-0.0.9/corby/generator/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,25 +58,25 @@
             template_url = template_url_answers["template_url"]
             template_name = template_url.split("/")[-1].split(".")[0]
         else:
             template_url = templates[answers["template"]]
             template_name = answers["template"]
 
         return {
-            template_name: template_name,
-            template_url: template_url
+            "template_name": template_name,
+            "template_url": template_url
         }
 
     def clone_template(self, template_url, template_name):
         '''Download a template from github and extract the skeleton'''
 
         # Clone the template
         git.Repo.clone_from(template_url, os.getcwd() + '/' + template_name)
 
         # Extract the skeleton
         shutil.move(
-            os.getcwd() + '/' + template_name + '/skeleton', os.getcwd() + '/' + template_name
+            os.getcwd() + '/' + template_name + '/skeleton', os.getcwd() + '/skeleton'
         )
 
     def cleanup(self, template_name):
         '''Removes the base folder from the template'''
         shutil.rmtree(os.getcwd() + '/' + template_name)
```

### Comparing `corby-0.0.8/corby/generator/chatbot/cli.py` & `corby-0.0.9/corby/generator/chatbot/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,13 +9,15 @@
     def get_templates(self):
         return {
         'basic-langchain-template': 'https://github.com/JoseHervas/basic-langchain-chatbot.git'
     }
 
     def create_cli_chatbot(self, name):
         """Generates a new CLI chatbot"""
+        app_path = os.getcwd() + '/' + name
         selected_template = self.ask_template()
         self.clone_template(selected_template["template_url"], selected_template["template_name"])
+        os.rename(os.getcwd() + '/skeleton', app_path)
         self.cleanup(selected_template["template_name"])
-        self.replace_in_folder(os.getcwd() + '/' + name, {'chatbot_name': name})
+        self.replace_in_folder(app_path, {'chatbot_name': name})
         print("Yeepay 🎉, your chatbot is ready!")
         print("You can find it in the " + name + " folder")
```

### Comparing `corby-0.0.8/corby/generator/chatbot/index.py` & `corby-0.0.9/corby/generator/chatbot/index.py`

 * *Files identical despite different names*

### Comparing `corby-0.0.8/corby/index.py` & `corby-0.0.9/corby/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """Main CLI entrypoint for Corby"""
 
 import argparse
 from string import Template
 from .generator.chatbot.index import create_chatbot
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 # We'll include more features in the future
 available_actions = ['new']
 
 available_entities = ['chatbot', 'notebook']
 
 parser = argparse.ArgumentParser(
```

### Comparing `corby-0.0.8/corby.egg-info/PKG-INFO` & `corby-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: corby
-Version: 0.0.8
+Version: 0.0.9
 Summary: ⚡ Create your LLMs applications from zero to deploy in minutes ⚡
 Author: Jose Hervás Díaz
 Author-email: jhervasdiaz@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🤖 Corby
 
-⚡ Create your LLMs applications from zero to deploy in minutes ⚡
+⚡ Create your AI applications from zero to deploy in minutes ⚡
 
-![pylint](https://github.com/JoseHervas/corby/actions/workflows/pylint.yml/badge.svg) [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-360/) ![version](https://img.shields.io/badge/version-0.0.7-blue) [![License: GPL-3](https://img.shields.io/badge/License-GPL3-green.svg)](https://opensource.org/licenses/GPL-3)
+![pypi](https://github.com/JoseHervas/corby/actions/workflows/publish.yml/badge.svg) ![pylint](https://github.com/JoseHervas/corby/actions/workflows/pylint.yml/badge.svg) [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-360/) [![Downloads](https://static.pepy.tech/badge/corby)](https://pepy.tech/project/corby) [![License: GPL-3](https://img.shields.io/badge/License-GPL3-green.svg)](https://opensource.org/licenses/GPL-3)
 
 ## 🚀 Quick Install
 
 ```bash
 pip install corby
 alias corby="python -m corby"
 ```
```

### Comparing `corby-0.0.8/setup.py` & `corby-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''Pypi setup file for corby'''
 
 from setuptools import setup, find_packages
 
 setup(
     name="corby",
-    version="0.0.8",
+    version="0.0.9",
     description="⚡ Create your LLMs applications from zero to deploy in minutes ⚡",
     # pylint: disable=consider-using-with
     long_description=open("README.md", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     author="Jose Hervás Díaz",
     author_email='jhervasdiaz@gmail.com',
     license='MIT',
```

