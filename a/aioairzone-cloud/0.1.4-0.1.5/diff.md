# Comparing `tmp/aioairzone-cloud-0.1.4.tar.gz` & `tmp/aioairzone-cloud-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairzone-cloud-0.1.4.tar", last modified: Thu May 25 07:18:51 2023, max compression
+gzip compressed data, was "aioairzone-cloud-0.1.5.tar", last modified: Thu May 25 07:24:43 2023, max compression
```

## Comparing `aioairzone-cloud-0.1.4.tar` & `aioairzone-cloud-0.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-25 07:18:51.370510 aioairzone-cloud-0.1.4/
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.4/LICENSE
--rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.4/MANIFEST.in
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-25 07:18:51.370510 aioairzone-cloud-0.1.4/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      746 2023-05-22 17:43:05.000000 aioairzone-cloud-0.1.4/README.md
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-25 07:18:51.370510 aioairzone-cloud-0.1.4/aioairzone_cloud/
--rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/__init__.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      156 2023-05-25 06:19:05.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/aidoo.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    18280 2023-05-24 19:18:04.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/cloudapi.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1527 2023-05-23 16:19:08.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/common.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     6443 2023-05-25 06:30:02.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/const.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2608 2023-05-25 06:22:30.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/device.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      806 2023-05-21 08:34:57.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/exceptions.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    16988 2023-05-25 06:16:28.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/hvac.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1181 2023-05-24 18:32:54.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/installation.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-05-22 07:54:27.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/py.typed
--rw-r--r--   0 noltari   (1000) noltari   (1000)      975 2023-05-25 06:23:06.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/system.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3844 2023-05-24 19:18:04.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/webserver.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2231 2023-05-25 06:23:06.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/zone.py
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-25 07:18:51.370510 aioairzone-cloud-0.1.4/aioairzone_cloud.egg-info/
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-25 07:18:51.000000 aioairzone-cloud-0.1.4/aioairzone_cloud.egg-info/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      670 2023-05-25 07:18:51.000000 aioairzone-cloud-0.1.4/aioairzone_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-25 07:18:51.000000 aioairzone-cloud-0.1.4/aioairzone_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-25 07:18:51.000000 aioairzone-cloud-0.1.4/aioairzone_cloud.egg-info/not-zip-safe
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-25 07:18:51.000000 aioairzone-cloud-0.1.4/aioairzone_cloud.egg-info/requires.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-05-25 07:18:51.000000 aioairzone-cloud-0.1.4/aioairzone_cloud.egg-info/top_level.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1029 2023-05-25 07:16:49.000000 aioairzone-cloud-0.1.4/pyproject.toml
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.4/requirements.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-05-25 07:18:51.370510 aioairzone-cloud-0.1.4/setup.cfg
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-25 07:24:43.447688 aioairzone-cloud-0.1.5/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.5/LICENSE
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.5/MANIFEST.in
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-25 07:24:43.451688 aioairzone-cloud-0.1.5/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      746 2023-05-22 17:43:05.000000 aioairzone-cloud-0.1.5/README.md
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-25 07:24:43.447688 aioairzone-cloud-0.1.5/aioairzone_cloud/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.1.5/aioairzone_cloud/__init__.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      156 2023-05-25 06:19:05.000000 aioairzone-cloud-0.1.5/aioairzone_cloud/aidoo.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    18280 2023-05-24 19:18:04.000000 aioairzone-cloud-0.1.5/aioairzone_cloud/cloudapi.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1527 2023-05-23 16:19:08.000000 aioairzone-cloud-0.1.5/aioairzone_cloud/common.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     6443 2023-05-25 06:30:02.000000 aioairzone-cloud-0.1.5/aioairzone_cloud/const.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2608 2023-05-25 06:22:30.000000 aioairzone-cloud-0.1.5/aioairzone_cloud/device.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      806 2023-05-21 08:34:57.000000 aioairzone-cloud-0.1.5/aioairzone_cloud/exceptions.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    16988 2023-05-25 06:16:28.000000 aioairzone-cloud-0.1.5/aioairzone_cloud/hvac.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1181 2023-05-24 18:32:54.000000 aioairzone-cloud-0.1.5/aioairzone_cloud/installation.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-05-22 07:54:27.000000 aioairzone-cloud-0.1.5/aioairzone_cloud/py.typed
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      976 2023-05-25 07:22:40.000000 aioairzone-cloud-0.1.5/aioairzone_cloud/system.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3844 2023-05-24 19:18:04.000000 aioairzone-cloud-0.1.5/aioairzone_cloud/webserver.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2231 2023-05-25 06:23:06.000000 aioairzone-cloud-0.1.5/aioairzone_cloud/zone.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-25 07:24:43.447688 aioairzone-cloud-0.1.5/aioairzone_cloud.egg-info/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-25 07:24:43.000000 aioairzone-cloud-0.1.5/aioairzone_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      670 2023-05-25 07:24:43.000000 aioairzone-cloud-0.1.5/aioairzone_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-25 07:24:43.000000 aioairzone-cloud-0.1.5/aioairzone_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-25 07:24:43.000000 aioairzone-cloud-0.1.5/aioairzone_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-25 07:24:43.000000 aioairzone-cloud-0.1.5/aioairzone_cloud.egg-info/requires.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-05-25 07:24:43.000000 aioairzone-cloud-0.1.5/aioairzone_cloud.egg-info/top_level.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1029 2023-05-25 07:24:11.000000 aioairzone-cloud-0.1.5/pyproject.toml
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.5/requirements.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-05-25 07:24:43.451688 aioairzone-cloud-0.1.5/setup.cfg
```

### Comparing `aioairzone-cloud-0.1.4/LICENSE` & `aioairzone-cloud-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.4/PKG-INFO` & `aioairzone-cloud-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.1.4
+Version: 0.1.5
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.1.4/README.md` & `aioairzone-cloud-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.4/aioairzone_cloud/cloudapi.py` & `aioairzone-cloud-0.1.5/aioairzone_cloud/cloudapi.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.4/aioairzone_cloud/common.py` & `aioairzone-cloud-0.1.5/aioairzone_cloud/common.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.4/aioairzone_cloud/const.py` & `aioairzone-cloud-0.1.5/aioairzone_cloud/const.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.4/aioairzone_cloud/device.py` & `aioairzone-cloud-0.1.5/aioairzone_cloud/device.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.4/aioairzone_cloud/exceptions.py` & `aioairzone-cloud-0.1.5/aioairzone_cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.4/aioairzone_cloud/hvac.py` & `aioairzone-cloud-0.1.5/aioairzone_cloud/hvac.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.4/aioairzone_cloud/installation.py` & `aioairzone-cloud-0.1.5/aioairzone_cloud/installation.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.4/aioairzone_cloud/system.py` & `aioairzone-cloud-0.1.5/aioairzone_cloud/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 class System(Device):
     """Airzone Cloud System device."""
 
     def __init__(self, inst_id: str, ws_id: str, device_data: dict[str, Any]):
         """Airzone Cloud System device init."""
         super().__init__(inst_id, ws_id, device_data)
 
-        self.name = f"System {self.get_system()}"
-
         if API_CONFIG in device_data:
             sub_data = device_data[API_CONFIG]
         else:
             sub_data = device_data[API_META]
 
         self.system_number = int(sub_data[API_SYSTEM_NUMBER])
 
+        self.name = f"System {self.system_number}"
+
     def data(self) -> dict[str, Any]:
         """Return System device data."""
         data = super().data()
 
         data[AZD_SYSTEM] = self.get_system()
 
         return data
```

### Comparing `aioairzone-cloud-0.1.4/aioairzone_cloud/webserver.py` & `aioairzone-cloud-0.1.5/aioairzone_cloud/webserver.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.4/aioairzone_cloud/zone.py` & `aioairzone-cloud-0.1.5/aioairzone_cloud/zone.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.4/aioairzone_cloud.egg-info/PKG-INFO` & `aioairzone-cloud-0.1.5/aioairzone_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.1.4
+Version: 0.1.5
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.1.4/aioairzone_cloud.egg-info/SOURCES.txt` & `aioairzone-cloud-0.1.5/aioairzone_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.4/pyproject.toml` & `aioairzone-cloud-0.1.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aioairzone-cloud"
-version = "0.1.4"
+version = "0.1.5"
 description = "Library to control Airzone Cloud devices"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "Apache-2.0"}
 keywords = ["airzone", "cloud", "hvac", "home"] 
 authors = [
   {name = "Álvaro Fernández Rojas", email = "noltari@gmail.com" }
```

