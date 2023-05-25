# Comparing `tmp/swoopyui-1.4.tar.gz` & `tmp/swoopyui-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swoopyui-1.4.tar", last modified: Mon May 22 18:26:14 2023, max compression
+gzip compressed data, was "swoopyui-1.5.tar", last modified: Thu May 25 15:47:22 2023, max compression
```

## Comparing `swoopyui-1.4.tar` & `swoopyui-1.5.tar`

### file list

```diff
@@ -1,42 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:26:14.962065 swoopyui-1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-22 18:26:03.000000 swoopyui-1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-22 18:26:03.000000 swoopyui-1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-22 18:26:14.962065 swoopyui-1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-22 18:26:03.000000 swoopyui-1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 18:26:03.000000 swoopyui-1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 18:26:14.962065 swoopyui-1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-22 18:26:03.000000 swoopyui-1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:26:14.958065 swoopyui-1.4/swoopyui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:26:14.958065 swoopyui-1.4/swoopyui/UIkits/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/UIkits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:26:14.958065 swoopyui-1.4/swoopyui/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   322687 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/assets/swoopyui.zip
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/swoopyui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:26:14.962065 swoopyui-1.4/swoopyui/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/tools/check_if_mac.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/tools/on_action.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/tools/pyinstaller_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/tools/run_swiftUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/tools/run_target.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/tools/unzip_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:26:14.962065 swoopyui-1.4/swoopyui/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/views/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/views/navigationlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/views/navigationstack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/views/navigationview.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/views/scrollview.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/views/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/views/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-22 18:26:03.000000 swoopyui-1.4/swoopyui/views/textfield.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:26:14.958065 swoopyui-1.4/swoopyui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-22 18:26:14.000000 swoopyui-1.4/swoopyui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-22 18:26:14.000000 swoopyui-1.4/swoopyui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 18:26:14.000000 swoopyui-1.4/swoopyui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 18:26:14.000000 swoopyui-1.4/swoopyui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 18:26:14.000000 swoopyui-1.4/swoopyui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:22.640205 swoopyui-1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-25 15:47:10.000000 swoopyui-1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-25 15:47:10.000000 swoopyui-1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-25 15:47:22.640205 swoopyui-1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-25 15:47:10.000000 swoopyui-1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-25 15:47:10.000000 swoopyui-1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:47:22.640205 swoopyui-1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-25 15:47:10.000000 swoopyui-1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:22.636205 swoopyui-1.5/swoopyui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:22.636205 swoopyui-1.5/swoopyui/UIkits/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/UIkits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:22.636205 swoopyui-1.5/swoopyui/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   339523 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/assets/swoopyui.zip
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/swoopyui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:22.636205 swoopyui-1.5/swoopyui/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/tools/check_if_mac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/tools/on_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/tools/pyinstaller_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/tools/run_swiftUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/tools/run_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/tools/unzip_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:22.636205 swoopyui-1.5/swoopyui/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/navigationlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/navigationstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/navigationview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/scrollview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:22.640205 swoopyui-1.5/swoopyui/views/shapes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/shapes/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/spacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-25 15:47:10.000000 swoopyui-1.5/swoopyui/views/textfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:47:22.636205 swoopyui-1.5/swoopyui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-25 15:47:22.000000 swoopyui-1.5/swoopyui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-25 15:47:22.000000 swoopyui-1.5/swoopyui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:47:22.000000 swoopyui-1.5/swoopyui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-25 15:47:22.000000 swoopyui-1.5/swoopyui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 15:47:22.000000 swoopyui-1.5/swoopyui.egg-info/top_level.txt
```

### Comparing `swoopyui-1.4/LICENSE` & `swoopyui-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `swoopyui-1.4/PKG-INFO` & `swoopyui-1.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,12 @@
-Metadata-Version: 2.1
-Name: swoopyui
-Version: 1.4
-Summary: A python library that allow you to build swiftUI apps using python.
-Home-page: https://github.com/SKbarbon/swoopyui
-Author: SKbarbon
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: MacOS :: MacOS X
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # swoopyui
-A simple python library that allow you to build swiftUI apps using python.
+swoopyui is a python library that enable developers to easily build swiftUI apps in python. Its not need any swiftUI experience with no xcode require.
 
 ## How does it work ?
-This library works by running python and swift at the same time!. It start a python localhost at the background and run swiftUI app that show the fron-end by communicating with python back-end host. But you should NOT worry about all of that, becuase the library always making sure that everything stay easy, simple and pythonic.
+It works through two parts: a Python host for managing updates and a Swift client app for the front-end. The client app stays connected to the Python back-end to receive real-time front-end updates. With swoopyui, developers can build SwiftUI apps without worrying about Swift or Xcode, because everything is handled with just Python!.
 
 ## installation
 
 Enter this on terminal to install this package:
 
 ```zsh
 pip install swoopyui --upgrade
@@ -41,11 +30,10 @@
 - [The docs](https://github.com/SKbarbon/swoopyui/wiki)
 
 ## ⚠️ help and contribute wanted!!
 Hi, read the docs, be master at this, it will be quick and easy..
 
 I want help with:
 - Supporting iOS, we need to support iOS and iPadOS, so if you can help with this.
-- Find a way to pack this library into `.app`, and fix the problem with most of packing packages.
 - Add a secure connection strategy between the host and client.
 
 Thanks, good luck..
```

### Comparing `swoopyui-1.4/setup.py` & `swoopyui-1.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_des = str(f.read())
 
 setup(
     name='swoopyui',
-    version='1.4',
+    version='1.5',
     author='SKbarbon',
     description='A python library that allow you to build swiftUI apps using python.',
     long_description=long_des,
     long_description_content_type='text/markdown',
     url='https://github.com/SKbarbon/swoopyui',
     install_requires=["flask", "requests"],
     packages=find_packages(),
```

### Comparing `swoopyui-1.4/swoopyui/__init__.py` & `swoopyui-1.5/swoopyui/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,8 +9,12 @@
 from .views.text import Text
 from .views.button import Button
 from .views.navigationview import NavigationView
 from .views.navigationstack import NavigationStack
 from .views.navigationlink import NavigationLink
 from .views.textfield import TextField
 from .views.stack import Stack, VSTACK, HSTACK, ZSTACK
-from .views.scrollview import ScrollView
+from .views.scrollview import ScrollView
+from .views.spacer import Spacer
+from .views.list import List
+
+from .views.shapes.circle import Circle
```

### Comparing `swoopyui-1.4/swoopyui/protocol.py` & `swoopyui-1.5/swoopyui/protocol.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.4/swoopyui/swoopyui.py` & `swoopyui-1.5/swoopyui/swoopyui.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import sys
 
 from .protocol import onClientRequestUpdate
 from .tools.run_target import run_the_target
 from .tools.run_swiftUI import run_swiftUI_app
 from .tools.pyinstaller_check import is_run_on_pyinstaller
 from .view import View
-
-
+     
+     
 def run_swiftUI_on_new_process (PORT, tmp_dir):
     if not os.path.isdir (tmp_dir):
         print("Cannot found the temp dir.")
         os._exit(0)
     run_swiftUI_app(PORT, tmp_dir)
 
 class app:
```

### Comparing `swoopyui-1.4/swoopyui/view.py` & `swoopyui-1.5/swoopyui/view.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.4/swoopyui/views/button.py` & `swoopyui-1.5/swoopyui/views/button.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.4/swoopyui/views/navigationlink.py` & `swoopyui-1.5/swoopyui/views/navigationlink.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.4/swoopyui/views/navigationstack.py` & `swoopyui-1.5/swoopyui/views/navigationstack.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.4/swoopyui/views/navigationview.py` & `swoopyui-1.5/swoopyui/views/navigationview.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.4/swoopyui/views/scrollview.py` & `swoopyui-1.5/swoopyui/views/scrollview.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.4/swoopyui/views/stack.py` & `swoopyui-1.5/swoopyui/views/stack.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.4/swoopyui/views/text.py` & `swoopyui-1.5/swoopyui/views/text.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.4/swoopyui/views/textfield.py` & `swoopyui-1.5/swoopyui/views/textfield.py`

 * *Files identical despite different names*

### Comparing `swoopyui-1.4/swoopyui.egg-info/SOURCES.txt` & `swoopyui-1.5/swoopyui.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 swoopyui/tools/on_action.py
 swoopyui/tools/pyinstaller_check.py
 swoopyui/tools/run_swiftUI.py
 swoopyui/tools/run_target.py
 swoopyui/tools/unzip_assets.py
 swoopyui/views/__init__.py
 swoopyui/views/button.py
+swoopyui/views/list.py
 swoopyui/views/navigationlink.py
 swoopyui/views/navigationstack.py
 swoopyui/views/navigationview.py
 swoopyui/views/scrollview.py
+swoopyui/views/spacer.py
 swoopyui/views/stack.py
 swoopyui/views/text.py
-swoopyui/views/textfield.py
+swoopyui/views/textfield.py
+swoopyui/views/shapes/__init__.py
+swoopyui/views/shapes/circle.py
```

