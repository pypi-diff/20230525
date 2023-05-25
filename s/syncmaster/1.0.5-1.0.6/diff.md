# Comparing `tmp/syncmaster-1.0.5.tar.gz` & `tmp/syncmaster-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncmaster-1.0.5.tar", last modified: Thu May  4 10:44:50 2023, max compression
+gzip compressed data, was "syncmaster-1.0.6.tar", last modified: Thu May 25 09:40:09 2023, max compression
```

## Comparing `syncmaster-1.0.5.tar` & `syncmaster-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-05-04 10:44:50.962335 syncmaster-1.0.5/
--rw-rw-r--   0 conor     (1000) conor     (1000)    11337 2023-01-20 02:50:04.000000 syncmaster-1.0.5/LICENSE
--rw-rw-r--   0 conor     (1000) conor     (1000)      111 2023-01-20 02:50:04.000000 syncmaster-1.0.5/MANIFEST.in
--rw-rw-r--   0 conor     (1000) conor     (1000)     3560 2023-05-04 10:44:50.962335 syncmaster-1.0.5/PKG-INFO
--rw-rw-r--   0 conor     (1000) conor     (1000)     2708 2023-05-03 14:33:34.000000 syncmaster-1.0.5/README.md
--rw-rw-r--   0 conor     (1000) conor     (1000)      929 2023-05-04 10:39:57.000000 syncmaster-1.0.5/settings.ini
--rw-rw-r--   0 conor     (1000) conor     (1000)       38 2023-05-04 10:44:50.962335 syncmaster-1.0.5/setup.cfg
--rw-rw-r--   0 conor     (1000) conor     (1000)     2560 2023-01-20 02:50:04.000000 syncmaster-1.0.5/setup.py
-drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-05-04 10:44:50.962335 syncmaster-1.0.5/syncmaster/
--rw-rw-r--   0 conor     (1000) conor     (1000)      235 2023-05-04 10:40:09.000000 syncmaster-1.0.5/syncmaster/__init__.py
--rw-rw-r--   0 conor     (1000) conor     (1000)     2057 2023-05-04 10:40:09.000000 syncmaster-1.0.5/syncmaster/_modidx.py
--rw-rw-r--   0 conor     (1000) conor     (1000)     2816 2023-05-04 10:40:09.000000 syncmaster-1.0.5/syncmaster/analysis.py
--rw-rw-r--   0 conor     (1000) conor     (1000)     3667 2023-05-04 10:40:09.000000 syncmaster-1.0.5/syncmaster/device.py
-drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-05-04 10:44:50.962335 syncmaster-1.0.5/syncmaster.egg-info/
--rw-rw-r--   0 conor     (1000) conor     (1000)     3560 2023-05-04 10:44:50.000000 syncmaster-1.0.5/syncmaster.egg-info/PKG-INFO
--rw-rw-r--   0 conor     (1000) conor     (1000)      379 2023-05-04 10:44:50.000000 syncmaster-1.0.5/syncmaster.egg-info/SOURCES.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-05-04 10:44:50.000000 syncmaster-1.0.5/syncmaster.egg-info/dependency_links.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)       42 2023-05-04 10:44:50.000000 syncmaster-1.0.5/syncmaster.egg-info/entry_points.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-04-17 10:19:07.000000 syncmaster-1.0.5/syncmaster.egg-info/not-zip-safe
--rw-rw-r--   0 conor     (1000) conor     (1000)       41 2023-05-04 10:44:50.000000 syncmaster-1.0.5/syncmaster.egg-info/requires.txt
--rw-rw-r--   0 conor     (1000) conor     (1000)       11 2023-05-04 10:44:50.000000 syncmaster-1.0.5/syncmaster.egg-info/top_level.txt
+drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-05-25 09:40:09.732720 syncmaster-1.0.6/
+-rw-rw-r--   0 conor     (1000) conor     (1000)    11337 2023-01-20 02:50:04.000000 syncmaster-1.0.6/LICENSE
+-rw-rw-r--   0 conor     (1000) conor     (1000)      111 2023-01-20 02:50:04.000000 syncmaster-1.0.6/MANIFEST.in
+-rw-rw-r--   0 conor     (1000) conor     (1000)     3560 2023-05-25 09:40:09.732720 syncmaster-1.0.6/PKG-INFO
+-rw-rw-r--   0 conor     (1000) conor     (1000)     2708 2023-05-03 14:33:34.000000 syncmaster-1.0.6/README.md
+-rw-rw-r--   0 conor     (1000) conor     (1000)      929 2023-05-25 09:39:05.000000 syncmaster-1.0.6/settings.ini
+-rw-rw-r--   0 conor     (1000) conor     (1000)       38 2023-05-25 09:40:09.732720 syncmaster-1.0.6/setup.cfg
+-rw-rw-r--   0 conor     (1000) conor     (1000)     2560 2023-01-20 02:50:04.000000 syncmaster-1.0.6/setup.py
+drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-05-25 09:40:09.732720 syncmaster-1.0.6/syncmaster/
+-rw-rw-r--   0 conor     (1000) conor     (1000)      235 2023-05-25 09:39:09.000000 syncmaster-1.0.6/syncmaster/__init__.py
+-rw-rw-r--   0 conor     (1000) conor     (1000)     2057 2023-05-25 09:39:09.000000 syncmaster-1.0.6/syncmaster/_modidx.py
+-rw-rw-r--   0 conor     (1000) conor     (1000)     2816 2023-05-25 09:39:09.000000 syncmaster-1.0.6/syncmaster/analysis.py
+-rw-rw-r--   0 conor     (1000) conor     (1000)     3675 2023-05-25 09:39:09.000000 syncmaster-1.0.6/syncmaster/device.py
+drwxrwxr-x   0 conor     (1000) conor     (1000)        0 2023-05-25 09:40:09.732720 syncmaster-1.0.6/syncmaster.egg-info/
+-rw-rw-r--   0 conor     (1000) conor     (1000)     3560 2023-05-25 09:40:09.000000 syncmaster-1.0.6/syncmaster.egg-info/PKG-INFO
+-rw-rw-r--   0 conor     (1000) conor     (1000)      379 2023-05-25 09:40:09.000000 syncmaster-1.0.6/syncmaster.egg-info/SOURCES.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-05-25 09:40:09.000000 syncmaster-1.0.6/syncmaster.egg-info/dependency_links.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)       42 2023-05-25 09:40:09.000000 syncmaster-1.0.6/syncmaster.egg-info/entry_points.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)        1 2023-04-17 10:19:07.000000 syncmaster-1.0.6/syncmaster.egg-info/not-zip-safe
+-rw-rw-r--   0 conor     (1000) conor     (1000)       41 2023-05-25 09:40:09.000000 syncmaster-1.0.6/syncmaster.egg-info/requires.txt
+-rw-rw-r--   0 conor     (1000) conor     (1000)       11 2023-05-25 09:40:09.000000 syncmaster-1.0.6/syncmaster.egg-info/top_level.txt
```

### Comparing `syncmaster-1.0.5/LICENSE` & `syncmaster-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `syncmaster-1.0.5/PKG-INFO` & `syncmaster-1.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncmaster
-Version: 1.0.5
+Version: 1.0.6
 Summary: Device and drivers for generating trigger signals to synchronise recorded signals with behavioural data
 Home-page: https://github.com/conorkeogh/syncmaster
 Author: Conor Keogh
 Author-email: conor.keogh@nds.ox.ac.uk
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `syncmaster-1.0.5/README.md` & `syncmaster-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `syncmaster-1.0.5/settings.ini` & `syncmaster-1.0.6/settings.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = syncmaster
 lib_name = syncmaster
-version = 1.0.5
+version = 1.0.6
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = syncmaster
 nbs_path = nbs
 recursive = True
```

### Comparing `syncmaster-1.0.5/setup.py` & `syncmaster-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `syncmaster-1.0.5/syncmaster/_modidx.py` & `syncmaster-1.0.6/syncmaster/_modidx.py`

 * *Files identical despite different names*

### Comparing `syncmaster-1.0.5/syncmaster/analysis.py` & `syncmaster-1.0.6/syncmaster/analysis.py`

 * *Files identical despite different names*

### Comparing `syncmaster-1.0.5/syncmaster/device.py` & `syncmaster-1.0.6/syncmaster/device.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,27 +86,27 @@
             raise Exception("Device not found")
             #print("Device not found")
 
     ''' Send required messages over serial '''
 
     def start(self):
         ''' Send start signal '''
-        self.sendMessage(self.STARTMARKER)
+        self.sendMessage(self.STARTPULSE)
 
     def end(self):
         ''' Send end signal '''
-        self.sendMessage(self.ENDMARKER)
+        self.sendMessage(self.ENDPULSE)
 
     def event1(self):
         ''' Send event 1 signal '''
-        self.sendMessage(self.EVENT1)
+        self.sendMessage(self.EVENT1PULSE)
 
     def event2(self):
         ''' Send event 2 signal '''
-        self.sendMessage(self.EVENT2)
+        self.sendMessage(self.EVENT2PULSE)
         
     def event(self, eventID):
         ''' Create event marker '''
         self.sendMessage(eventID)
 
     # Send message via serial port
     def sendMessage(self, message):
```

### Comparing `syncmaster-1.0.5/syncmaster.egg-info/PKG-INFO` & `syncmaster-1.0.6/syncmaster.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncmaster
-Version: 1.0.5
+Version: 1.0.6
 Summary: Device and drivers for generating trigger signals to synchronise recorded signals with behavioural data
 Home-page: https://github.com/conorkeogh/syncmaster
 Author: Conor Keogh
 Author-email: conor.keogh@nds.ox.ac.uk
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

