# Comparing `tmp/jade_config-1.1.1.tar.gz` & `tmp/jade_config-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jade_config-1.1.1.tar", last modified: Tue May 23 16:14:00 2023, max compression
+gzip compressed data, was "jade_config-1.1.2.tar", last modified: Thu May 25 01:24:23 2023, max compression
```

## Comparing `jade_config-1.1.1.tar` & `jade_config-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 16:14:00.589257 jade_config-1.1.1/
--rw-rw-rw-   0        0        0     3456 2023-05-23 16:14:00.588255 jade_config-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2934 2023-05-23 16:13:41.000000 jade_config-1.1.1/README.md
--rw-rw-rw-   0        0        0     1113 2023-05-23 16:13:36.000000 jade_config-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 16:14:00.589257 jade_config-1.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-23 16:14:00.572763 jade_config-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 16:14:00.576763 jade_config-1.1.1/src/jade_config/
--rw-rw-rw-   0        0        0      367 2023-01-04 19:02:56.000000 jade_config-1.1.1/src/jade_config/__init__.py
--rw-rw-rw-   0        0        0      147 2023-01-04 18:30:42.000000 jade_config-1.1.1/src/jade_config/__main__.py
--rw-rw-rw-   0        0        0     2771 2023-05-23 15:57:44.000000 jade_config-1.1.1/src/jade_config/config.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:14:00.587255 jade_config-1.1.1/src/jade_config.egg-info/
--rw-rw-rw-   0        0        0     3456 2023-05-23 16:14:00.000000 jade_config-1.1.1/src/jade_config.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-05-23 16:14:00.000000 jade_config-1.1.1/src/jade_config.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 16:14:00.000000 jade_config-1.1.1/src/jade_config.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-23 16:14:00.000000 jade_config-1.1.1/src/jade_config.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-23 16:14:00.000000 jade_config-1.1.1/src/jade_config.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 01:24:23.301024 jade_config-1.1.2/
+-rw-rw-rw-   0        0        0     3593 2023-05-25 01:24:23.301024 jade_config-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3071 2023-05-25 01:23:46.000000 jade_config-1.1.2/README.md
+-rw-rw-rw-   0        0        0     1113 2023-05-25 01:23:50.000000 jade_config-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-25 01:24:23.302025 jade_config-1.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 01:24:23.278024 jade_config-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 01:24:23.286025 jade_config-1.1.2/src/jade_config/
+-rw-rw-rw-   0        0        0      367 2023-01-04 19:02:56.000000 jade_config-1.1.2/src/jade_config/__init__.py
+-rw-rw-rw-   0        0        0      147 2023-01-04 18:30:42.000000 jade_config-1.1.2/src/jade_config/__main__.py
+-rw-rw-rw-   0        0        0     2751 2023-05-25 01:22:06.000000 jade_config-1.1.2/src/jade_config/config.py
+drwxrwxrwx   0        0        0        0 2023-05-25 01:24:23.300025 jade_config-1.1.2/src/jade_config.egg-info/
+-rw-rw-rw-   0        0        0     3593 2023-05-25 01:24:23.000000 jade_config-1.1.2/src/jade_config.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2023-05-25 01:24:23.000000 jade_config-1.1.2/src/jade_config.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 01:24:23.000000 jade_config-1.1.2/src/jade_config.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-25 01:24:23.000000 jade_config-1.1.2/src/jade_config.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-25 01:24:23.000000 jade_config-1.1.2/src/jade_config.egg-info/top_level.txt
```

### Comparing `jade_config-1.1.1/PKG-INFO` & `jade_config-1.1.2/src/jade_config.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jade_config
-Version: 1.1.1
+Name: jade-config
+Version: 1.1.2
 Summary: A python package to quickly and easily make configs, or other things that your program needs to remember.
 Author-email: nfoert <jadesoftware1@gmail.com>
 Project-URL: Homepage, https://github.com/nfoert/jade_config
 Keywords: jade,jade_config,jade config,config,remember
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -92,10 +92,11 @@
 </ul>
 
 **Warning: The files created by this library can still be read by others, eg. hackers, by using Jade Config, shelve or others. Don't store sensitive data like passwords or API Keys! It's certainly more secure than text files, but be careful!**
 
 ## Changelog
 <hr>
 
+- [1.1.2] [5/24/23] Fixed a bug where if you tried to `getValue()` a key that couldn't be found, It would throw an `UnboundLocalError`.
 - [1.1.1] [5/23/23] Made errors more descriptive, added `removeKey()`, and made the database correctly close after it's done being used.
 - [1.0.1] Patch fixing a small logging confusion
 - [1.0.0] Initial release
```

### Comparing `jade_config-1.1.1/README.md` & `jade_config-1.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -79,10 +79,11 @@
 </ul>
 
 **Warning: The files created by this library can still be read by others, eg. hackers, by using Jade Config, shelve or others. Don't store sensitive data like passwords or API Keys! It's certainly more secure than text files, but be careful!**
 
 ## Changelog
 <hr>
 
+- [1.1.2] [5/24/23] Fixed a bug where if you tried to `getValue()` a key that couldn't be found, It would throw an `UnboundLocalError`.
 - [1.1.1] [5/23/23] Made errors more descriptive, added `removeKey()`, and made the database correctly close after it's done being used.
 - [1.0.1] Patch fixing a small logging confusion
 - [1.0.0] Initial release
```

### Comparing `jade_config-1.1.1/pyproject.toml` & `jade_config-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jade_config"
-version = "1.1.1"
+version = "1.1.2"
 description = "A python package to quickly and easily make configs, or other things that your program needs to remember."
 readme = "README.md"
 authors = [{ name = "nfoert", email = "jadesoftware1@gmail.com" }]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
```

### Comparing `jade_config-1.1.1/src/jade_config/config.py` & `jade_config-1.1.2/src/jade_config/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,16 +63,16 @@
             db = shelve.open(self.name)
             value = db[key]
             db.close()
             self.logAndPrint(f"Got value '{value}' from key '{key}'")
             return value
 
         except:
-            self.logAndPrint(f"Unable to get the value '{value}' from key '{key}'")
-            raise UnableToGetValue(f"Unable to get the value '{value}' from key '{key}'")
+            self.logAndPrint(f"Unable to get the value from key '{key}'")
+            raise UnableToGetValue(f"Unable to get the value from key '{key}'")
         
     def removeKey(self, key):
         '''Removes a key from the file'''
         try:
             db = shelve.open(self.name)
             del db[key]
             db.close()
```

### Comparing `jade_config-1.1.1/src/jade_config.egg-info/PKG-INFO` & `jade_config-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jade-config
-Version: 1.1.1
+Name: jade_config
+Version: 1.1.2
 Summary: A python package to quickly and easily make configs, or other things that your program needs to remember.
 Author-email: nfoert <jadesoftware1@gmail.com>
 Project-URL: Homepage, https://github.com/nfoert/jade_config
 Keywords: jade,jade_config,jade config,config,remember
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -92,10 +92,11 @@
 </ul>
 
 **Warning: The files created by this library can still be read by others, eg. hackers, by using Jade Config, shelve or others. Don't store sensitive data like passwords or API Keys! It's certainly more secure than text files, but be careful!**
 
 ## Changelog
 <hr>
 
+- [1.1.2] [5/24/23] Fixed a bug where if you tried to `getValue()` a key that couldn't be found, It would throw an `UnboundLocalError`.
 - [1.1.1] [5/23/23] Made errors more descriptive, added `removeKey()`, and made the database correctly close after it's done being used.
 - [1.0.1] Patch fixing a small logging confusion
 - [1.0.0] Initial release
```

