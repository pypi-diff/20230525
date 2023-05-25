# Comparing `tmp/photcal-0.0.1.tar.gz` & `tmp/photcal-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photcal-0.0.1.tar", last modified: Wed May 24 17:33:09 2023, max compression
+gzip compressed data, was "photcal-0.0.2.tar", last modified: Thu May 25 16:07:22 2023, max compression
```

## Comparing `photcal-0.0.1.tar` & `photcal-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,9 @@
-drwxrwxr-x   0 tlambert  (1001) tlambert  (1001)        0 2023-05-24 17:33:09.901460 photcal-0.0.1/
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      805 2023-05-24 17:33:09.901460 photcal-0.0.1/PKG-INFO
-drwxrwxr-x   0 tlambert  (1001) tlambert  (1001)        0 2023-05-24 17:33:09.901460 photcal-0.0.1/photcal/
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)        0 2023-05-24 14:01:13.337872 photcal-0.0.1/photcal/__init__.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     4284 2023-05-24 14:07:43.573337 photcal-0.0.1/photcal/photometric_calibration.py
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)       39 2023-05-24 14:10:56.066910 photcal-0.0.1/setup.cfg
--rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     1140 2023-05-24 14:13:53.504807 photcal-0.0.1/setup.py
+drwxrwxr-x   0 tlambert  (1001) tlambert  (1001)        0 2023-05-25 16:07:22.565683 photcal-0.0.2/
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)      805 2023-05-25 16:07:22.565683 photcal-0.0.2/PKG-INFO
+drwxrwxr-x   0 tlambert  (1001) tlambert  (1001)        0 2023-05-25 16:07:22.565683 photcal-0.0.2/photcal/
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)        0 2023-05-24 14:01:13.337872 photcal-0.0.2/photcal/__init__.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     1220 2023-05-25 14:34:45.639945 photcal-0.0.2/photcal/k_constant.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     6110 2023-05-25 16:01:02.344103 photcal-0.0.2/photcal/photometric_calibration.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     9226 2023-05-25 15:57:36.184906 photcal-0.0.2/photcal/test_photometric_calibration.py
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)       39 2023-05-24 14:10:56.066910 photcal-0.0.2/setup.cfg
+-rw-rw-r--   0 tlambert  (1001) tlambert  (1001)     1174 2023-05-25 16:03:58.679097 photcal-0.0.2/setup.py
```

### Comparing `photcal-0.0.1/PKG-INFO` & `photcal-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: photcal
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package for photometrically calibrating images with survey catalogs.
 Home-page: https://github.com/TrystanScottLambert
 Author: Trystan Scott Lambert and Dejene Zwedie
 Author-email: trystanscottlambert@gmail.com
 License: MIT
-Download-URL: https://github.com/TrystanScottLambert/photcal/archive/refs/tags/v0.0.1.tar.gz
+Download-URL: https://github.com/TrystanScottLambert/photcal/archive/refs/tags/v0.0.2.tar.gz
 Description: UNKNOWN
 Keywords: astronomy,photometry,calibration
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `photcal-0.0.1/setup.py` & `photcal-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from distutils.core import setup
 
 setup(
   name = 'photcal',
   packages = ['photcal'],
-  version = '0.0.1',
+  version = '0.0.2',
   license='MIT',
   description = 'Package for photometrically calibrating images with survey catalogs.',
   author = 'Trystan Scott Lambert and Dejene Zwedie',
   author_email = 'trystanscottlambert@gmail.com',
   url = 'https://github.com/TrystanScottLambert',
-  download_url = 'https://github.com/TrystanScottLambert/photcal/archive/refs/tags/v0.0.1.tar.gz',
+  download_url = 'https://github.com/TrystanScottLambert/photcal/archive/refs/tags/v0.0.2.tar.gz',
   keywords = ['astronomy', 'photometry', 'calibration'],
   install_requires=[
     'numpy',
+    'astropy',
+    'matplotlib',
    ],
+
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
     'Programming Language :: Python :: 3.10',
```

