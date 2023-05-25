# Comparing `tmp/cnaclib-0.1.13.tar.gz` & `tmp/cnaclib-0.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnaclib-0.1.13.tar", last modified: Thu May 25 13:41:54 2023, max compression
+gzip compressed data, was "cnaclib-0.1.14.tar", last modified: Thu May 25 13:44:59 2023, max compression
```

## Comparing `cnaclib-0.1.13.tar` & `cnaclib-0.1.14.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 13:41:54.791852 cnaclib-0.1.13/
--rw-rw-rw-   0        0        0     1073 2023-05-10 09:44:18.000000 cnaclib-0.1.13/LICENSE.txt
--rw-rw-rw-   0        0        0     2912 2023-05-25 13:41:54.790851 cnaclib-0.1.13/PKG-INFO
--rw-rw-rw-   0        0        0     1981 2023-05-22 11:02:16.000000 cnaclib-0.1.13/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 13:41:54.760849 cnaclib-0.1.13/cnaclib/
--rw-rw-rw-   0        0        0       17 2023-05-18 14:22:52.000000 cnaclib-0.1.13/cnaclib/__init__.py
--rw-rw-rw-   0        0        0     7931 2023-05-22 15:45:17.000000 cnaclib-0.1.13/cnaclib/lSix.py
--rw-rw-rw-   0        0        0    21717 2023-05-18 09:49:05.000000 cnaclib-0.1.13/cnaclib/rac.py
--rw-rw-rw-   0        0        0       36 2023-05-22 15:54:04.000000 cnaclib-0.1.13/cnaclib/test.py
--rw-rw-rw-   0        0        0    21837 2023-05-25 10:53:32.000000 cnaclib-0.1.13/cnaclib/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-25 13:41:54.783851 cnaclib-0.1.13/cnaclib.egg-info/
--rw-rw-rw-   0        0        0     2912 2023-05-25 13:41:53.000000 cnaclib-0.1.13/cnaclib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-05-25 13:41:53.000000 cnaclib-0.1.13/cnaclib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 13:41:53.000000 cnaclib-0.1.13/cnaclib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      160 2023-05-25 13:41:53.000000 cnaclib-0.1.13/cnaclib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-25 13:41:53.000000 cnaclib-0.1.13/cnaclib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 13:41:54.793852 cnaclib-0.1.13/setup.cfg
--rw-rw-rw-   0        0        0     1192 2023-05-25 13:41:14.000000 cnaclib-0.1.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 13:44:59.123991 cnaclib-0.1.14/
+-rw-rw-rw-   0        0        0     1073 2023-05-10 09:44:18.000000 cnaclib-0.1.14/LICENSE.txt
+-rw-rw-rw-   0        0        0     2886 2023-05-25 13:44:59.118991 cnaclib-0.1.14/PKG-INFO
+-rw-rw-rw-   0        0        0     1963 2023-05-25 13:44:26.000000 cnaclib-0.1.14/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 13:44:59.088994 cnaclib-0.1.14/cnaclib/
+-rw-rw-rw-   0        0        0       17 2023-05-18 14:22:52.000000 cnaclib-0.1.14/cnaclib/__init__.py
+-rw-rw-rw-   0        0        0     7931 2023-05-22 15:45:17.000000 cnaclib-0.1.14/cnaclib/lSix.py
+-rw-rw-rw-   0        0        0    21717 2023-05-18 09:49:05.000000 cnaclib-0.1.14/cnaclib/rac.py
+-rw-rw-rw-   0        0        0       36 2023-05-22 15:54:04.000000 cnaclib-0.1.14/cnaclib/test.py
+-rw-rw-rw-   0        0        0    21837 2023-05-25 10:53:32.000000 cnaclib-0.1.14/cnaclib/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-25 13:44:59.114992 cnaclib-0.1.14/cnaclib.egg-info/
+-rw-rw-rw-   0        0        0     2886 2023-05-25 13:44:58.000000 cnaclib-0.1.14/cnaclib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-05-25 13:44:58.000000 cnaclib-0.1.14/cnaclib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 13:44:58.000000 cnaclib-0.1.14/cnaclib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      160 2023-05-25 13:44:58.000000 cnaclib-0.1.14/cnaclib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-25 13:44:58.000000 cnaclib-0.1.14/cnaclib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 13:44:59.126991 cnaclib-0.1.14/setup.cfg
+-rw-rw-rw-   0        0        0     1192 2023-05-25 13:44:40.000000 cnaclib-0.1.14/setup.py
```

### Comparing `cnaclib-0.1.13/LICENSE.txt` & `cnaclib-0.1.14/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cnaclib-0.1.13/PKG-INFO` & `cnaclib-0.1.14/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnaclib
-Version: 0.1.13
+Version: 0.1.14
 Summary: Simulateur RAC
 Home-page: UNKNOWN
 Author: BENHAMADA Nadir
 Author-email: aistatendz@gmail.com
 License: UNKNOWN
 Description: # cnaclib : Librairie Python developpee pour les usagers et les employes de la CNAC. 
         
@@ -31,15 +31,14 @@
         ### Dependencies
         
         cnaclib requires 
         
         ```
         certifi >=2023.5.7
         charset-normalizer >=3.1.0
-        cnaclib >=0.1.10
         idna >=3.4
         numpy >=1.24.3
         pandas >=2.0.1
         python-dateutil >=2.8.2
         pytz >=2023.3
         six >=1.16.0
         tzdata >=2023.3
```

### Comparing `cnaclib-0.1.13/README.md` & `cnaclib-0.1.14/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 ### Dependencies
 
 cnaclib requires 
 
 ```
 certifi >=2023.5.7
 charset-normalizer >=3.1.0
-cnaclib >=0.1.10
 idna >=3.4
 numpy >=1.24.3
 pandas >=2.0.1
 python-dateutil >=2.8.2
 pytz >=2023.3
 six >=1.16.0
 tzdata >=2023.3
```

### Comparing `cnaclib-0.1.13/cnaclib/lSix.py` & `cnaclib-0.1.14/cnaclib/lSix.py`

 * *Files identical despite different names*

### Comparing `cnaclib-0.1.13/cnaclib/rac.py` & `cnaclib-0.1.14/cnaclib/rac.py`

 * *Files identical despite different names*

### Comparing `cnaclib-0.1.13/cnaclib/tools.py` & `cnaclib-0.1.14/cnaclib/tools.py`

 * *Files identical despite different names*

### Comparing `cnaclib-0.1.13/cnaclib.egg-info/PKG-INFO` & `cnaclib-0.1.14/cnaclib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnaclib
-Version: 0.1.13
+Version: 0.1.14
 Summary: Simulateur RAC
 Home-page: UNKNOWN
 Author: BENHAMADA Nadir
 Author-email: aistatendz@gmail.com
 License: UNKNOWN
 Description: # cnaclib : Librairie Python developpee pour les usagers et les employes de la CNAC. 
         
@@ -31,15 +31,14 @@
         ### Dependencies
         
         cnaclib requires 
         
         ```
         certifi >=2023.5.7
         charset-normalizer >=3.1.0
-        cnaclib >=0.1.10
         idna >=3.4
         numpy >=1.24.3
         pandas >=2.0.1
         python-dateutil >=2.8.2
         pytz >=2023.3
         six >=1.16.0
         tzdata >=2023.3
```

### Comparing `cnaclib-0.1.13/setup.py` & `cnaclib-0.1.14/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 chemin = Path(__file__).parent
 long_description = (chemin / "README.md").read_text()
 
 
 setuptools.setup(
     name = 'cnaclib',
-    version = '0.1.13',
+    version = '0.1.14',
     author= 'BENHAMADA Nadir',
     author_email='aistatendz@gmail.com',
     description='Simulateur RAC',
     packages=setuptools.find_packages(),
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=["certifi >=2023.5.7",
```

