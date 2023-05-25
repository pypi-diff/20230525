# Comparing `tmp/debug_print2-0.1.1.tar.gz` & `tmp/debug_print2-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debug_print2-0.1.1.tar", max compression
+gzip compressed data, was "debug_print2-0.1.2.tar", max compression
```

## Comparing `debug_print2-0.1.1.tar` & `debug_print2-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      605 2023-05-06 03:50:46.757612 debug_print2-0.1.1/README.md
--rw-r--r--   0        0        0      368 2023-05-06 04:02:39.313083 debug_print2-0.1.1/debug_print/__init__.py
--rw-r--r--   0        0        0      367 2023-05-06 04:02:39.308829 debug_print2-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1091 1970-01-01 00:00:00.000000 debug_print2-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      608 2023-05-24 09:28:26.395065 debug_print2-0.1.2/README.md
+-rw-r--r--   0        0        0      475 2023-05-24 09:39:38.807785 debug_print2-0.1.2/debug_print/__init__.py
+-rw-r--r--   0        0        0      367 2023-05-24 09:27:21.803278 debug_print2-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 debug_print2-0.1.2/PKG-INFO
```

### Comparing `debug_print2-0.1.1/README.md` & `debug_print2-0.1.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # debug-print
-Capture the print function and add some output information to it for easy debugging
+Capture the print function and add some output information to it for easy debugging.
 
 ## why？
 Is there such a situation？  
 That you need to temporarily use `print` debugging in third-party packages or source code, 
-but you may forget where to add `print` when thinking or jumping back and forth. 
+but you may forget where to add `print` when thinking or jumping back and forth.  
 Now you only need to install and import `debug_print` to let print output the file name and line number, 
 which is more convenient for debugging.
 
 ## Install：
 ```shell
 pip install debug-print2
 ```
 
 ## Usage:
-Just run the file import at the very beginning.
+Just import the file to run.
 ```python
 import debug_print
+debug_print.patch()
 ```
```

### Comparing `debug_print2-0.1.1/PKG-INFO` & `debug_print2-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: debug-print2
-Version: 0.1.1
+Version: 0.1.2
 Summary: Capture the print function and add some output information to it for easy debugging
 Author: vvanglro
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # debug-print
-Capture the print function and add some output information to it for easy debugging
+Capture the print function and add some output information to it for easy debugging.
 
 ## why？
 Is there such a situation？  
 That you need to temporarily use `print` debugging in third-party packages or source code, 
-but you may forget where to add `print` when thinking or jumping back and forth. 
+but you may forget where to add `print` when thinking or jumping back and forth.  
 Now you only need to install and import `debug_print` to let print output the file name and line number, 
 which is more convenient for debugging.
 
 ## Install：
 ```shell
 pip install debug-print2
 ```
 
 ## Usage:
-Just run the file import at the very beginning.
+Just import the file to run.
 ```python
 import debug_print
+debug_print.patch()
 ```
```

