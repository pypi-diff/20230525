# Comparing `tmp/Sophia-Optimizer-0.1.6.tar.gz` & `tmp/Sophia-Optimizer-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sophia-Optimizer-0.1.6.tar", last modified: Thu May 25 03:28:18 2023, max compression
+gzip compressed data, was "Sophia-Optimizer-0.1.8.tar", last modified: Thu May 25 03:39:35 2023, max compression
```

## Comparing `Sophia-Optimizer-0.1.6.tar` & `Sophia-Optimizer-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:28:18.086351 Sophia-Optimizer-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 03:28:04.000000 Sophia-Optimizer-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-25 03:28:18.086351 Sophia-Optimizer-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13213 2023-05-25 03:28:04.000000 Sophia-Optimizer-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:28:18.086351 Sophia-Optimizer-0.1.6/Sophia/
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-25 03:28:04.000000 Sophia-Optimizer-0.1.6/Sophia/Sophia.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-25 03:28:04.000000 Sophia-Optimizer-0.1.6/Sophia/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:28:18.086351 Sophia-Optimizer-0.1.6/Sophia_Optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-25 03:28:18.000000 Sophia-Optimizer-0.1.6/Sophia_Optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-25 03:28:18.000000 Sophia-Optimizer-0.1.6/Sophia_Optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 03:28:18.000000 Sophia-Optimizer-0.1.6/Sophia_Optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 03:28:18.000000 Sophia-Optimizer-0.1.6/Sophia_Optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 03:28:18.000000 Sophia-Optimizer-0.1.6/Sophia_Optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 03:28:18.086351 Sophia-Optimizer-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-25 03:28:04.000000 Sophia-Optimizer-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:39:35.765355 Sophia-Optimizer-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 03:39:24.000000 Sophia-Optimizer-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-25 03:39:35.765355 Sophia-Optimizer-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13213 2023-05-25 03:39:24.000000 Sophia-Optimizer-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:39:35.765355 Sophia-Optimizer-0.1.8/Sophia/
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-25 03:39:24.000000 Sophia-Optimizer-0.1.8/Sophia/Sophia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-25 03:39:24.000000 Sophia-Optimizer-0.1.8/Sophia/Sophiav2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-25 03:39:24.000000 Sophia-Optimizer-0.1.8/Sophia/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 03:39:35.765355 Sophia-Optimizer-0.1.8/Sophia_Optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-25 03:39:35.000000 Sophia-Optimizer-0.1.8/Sophia_Optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-25 03:39:35.000000 Sophia-Optimizer-0.1.8/Sophia_Optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 03:39:35.000000 Sophia-Optimizer-0.1.8/Sophia_Optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 03:39:35.000000 Sophia-Optimizer-0.1.8/Sophia_Optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 03:39:35.000000 Sophia-Optimizer-0.1.8/Sophia_Optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 03:39:35.765355 Sophia-Optimizer-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-25 03:39:24.000000 Sophia-Optimizer-0.1.8/setup.py
```

### Comparing `Sophia-Optimizer-0.1.6/LICENSE` & `Sophia-Optimizer-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Sophia-Optimizer-0.1.6/PKG-INFO` & `Sophia-Optimizer-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sophia-Optimizer
-Version: 0.1.6
+Version: 0.1.8
 Summary: Sophia Optimizer ULTRA FAST
 Home-page: https://github.com/kyegomez/Sophia
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: APACHE
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Sophia-Optimizer-0.1.6/README.md` & `Sophia-Optimizer-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `Sophia-Optimizer-0.1.6/Sophia/Sophia.py` & `Sophia-Optimizer-0.1.8/Sophia/Sophia.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
                 m, h = state['m'], state['h']
                 beta1, beta2 = group['betas']
                 state['step'] += 1
 
 
                 if group['weight_decay'] != 0:
-                    grad = grad.add(group["weight_decau"], p.data)
+                    grad = grad.add(group["weight_decay"], p.data)
 
                 #update biased first moment estimate
                 m.mul_(beta1).add_(1 - beta1, grad)
 
                 #update hessian estimate
                 if state['step'] % group['k'] == 1:
                     if group['estimator'] == "Hutchinson":
```

### Comparing `Sophia-Optimizer-0.1.6/Sophia_Optimizer.egg-info/PKG-INFO` & `Sophia-Optimizer-0.1.8/Sophia_Optimizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sophia-Optimizer
-Version: 0.1.6
+Version: 0.1.8
 Summary: Sophia Optimizer ULTRA FAST
 Home-page: https://github.com/kyegomez/Sophia
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: APACHE
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Sophia-Optimizer-0.1.6/setup.py` & `Sophia-Optimizer-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'Sophia-Optimizer',
   packages = find_packages(exclude=[]),
-  version = '0.1.6',
+  version = '0.1.8',
   license='APACHE',
   description = 'Sophia Optimizer ULTRA FAST',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/Sophia',
   keywords = [
```

