# Comparing `tmp/aioairzone-cloud-0.1.2.tar.gz` & `tmp/aioairzone-cloud-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairzone-cloud-0.1.2.tar", last modified: Tue May 23 16:28:14 2023, max compression
+gzip compressed data, was "aioairzone-cloud-0.1.3.tar", last modified: Wed May 24 08:10:00 2023, max compression
```

## Comparing `aioairzone-cloud-0.1.2.tar` & `aioairzone-cloud-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-23 16:28:14.963386 aioairzone-cloud-0.1.2/
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.2/LICENSE
--rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.2/MANIFEST.in
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-23 16:28:14.963386 aioairzone-cloud-0.1.2/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      746 2023-05-22 17:43:05.000000 aioairzone-cloud-0.1.2/README.md
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-23 16:28:14.963386 aioairzone-cloud-0.1.2/aioairzone_cloud/
--rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.1.2/aioairzone_cloud/__init__.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    16766 2023-05-23 16:26:50.000000 aioairzone-cloud-0.1.2/aioairzone_cloud/cloudapi.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1527 2023-05-23 16:19:08.000000 aioairzone-cloud-0.1.2/aioairzone_cloud/common.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     6167 2023-05-23 06:40:31.000000 aioairzone-cloud-0.1.2/aioairzone_cloud/const.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3040 2023-05-23 16:26:50.000000 aioairzone-cloud-0.1.2/aioairzone_cloud/device.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      806 2023-05-21 08:34:57.000000 aioairzone-cloud-0.1.2/aioairzone_cloud/exceptions.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1184 2023-05-19 11:19:38.000000 aioairzone-cloud-0.1.2/aioairzone_cloud/installation.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-05-22 07:54:27.000000 aioairzone-cloud-0.1.2/aioairzone_cloud/py.typed
--rw-r--r--   0 noltari   (1000) noltari   (1000)      401 2023-05-23 16:26:50.000000 aioairzone-cloud-0.1.2/aioairzone_cloud/system.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3791 2023-05-19 11:19:38.000000 aioairzone-cloud-0.1.2/aioairzone_cloud/webserver.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    18130 2023-05-23 16:26:50.000000 aioairzone-cloud-0.1.2/aioairzone_cloud/zone.py
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-23 16:28:14.963386 aioairzone-cloud-0.1.2/aioairzone_cloud.egg-info/
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-23 16:28:14.000000 aioairzone-cloud-0.1.2/aioairzone_cloud.egg-info/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      619 2023-05-23 16:28:14.000000 aioairzone-cloud-0.1.2/aioairzone_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-23 16:28:14.000000 aioairzone-cloud-0.1.2/aioairzone_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-23 16:28:14.000000 aioairzone-cloud-0.1.2/aioairzone_cloud.egg-info/not-zip-safe
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-23 16:28:14.000000 aioairzone-cloud-0.1.2/aioairzone_cloud.egg-info/requires.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-05-23 16:28:14.000000 aioairzone-cloud-0.1.2/aioairzone_cloud.egg-info/top_level.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1029 2023-05-23 16:27:25.000000 aioairzone-cloud-0.1.2/pyproject.toml
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.2/requirements.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-05-23 16:28:14.963386 aioairzone-cloud-0.1.2/setup.cfg
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-24 08:10:00.448727 aioairzone-cloud-0.1.3/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.3/LICENSE
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.3/MANIFEST.in
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-24 08:10:00.448727 aioairzone-cloud-0.1.3/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      746 2023-05-22 17:43:05.000000 aioairzone-cloud-0.1.3/README.md
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-24 08:10:00.448727 aioairzone-cloud-0.1.3/aioairzone_cloud/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.1.3/aioairzone_cloud/__init__.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    16851 2023-05-24 08:04:48.000000 aioairzone-cloud-0.1.3/aioairzone_cloud/cloudapi.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1527 2023-05-23 16:19:08.000000 aioairzone-cloud-0.1.3/aioairzone_cloud/common.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     6167 2023-05-23 06:40:31.000000 aioairzone-cloud-0.1.3/aioairzone_cloud/const.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3040 2023-05-23 16:26:50.000000 aioairzone-cloud-0.1.3/aioairzone_cloud/device.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      806 2023-05-21 08:34:57.000000 aioairzone-cloud-0.1.3/aioairzone_cloud/exceptions.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1184 2023-05-19 11:19:38.000000 aioairzone-cloud-0.1.3/aioairzone_cloud/installation.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-05-22 07:54:27.000000 aioairzone-cloud-0.1.3/aioairzone_cloud/py.typed
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      401 2023-05-23 16:26:50.000000 aioairzone-cloud-0.1.3/aioairzone_cloud/system.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3791 2023-05-19 11:19:38.000000 aioairzone-cloud-0.1.3/aioairzone_cloud/webserver.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    18130 2023-05-23 16:26:50.000000 aioairzone-cloud-0.1.3/aioairzone_cloud/zone.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-24 08:10:00.448727 aioairzone-cloud-0.1.3/aioairzone_cloud.egg-info/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-24 08:10:00.000000 aioairzone-cloud-0.1.3/aioairzone_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      619 2023-05-24 08:10:00.000000 aioairzone-cloud-0.1.3/aioairzone_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-24 08:10:00.000000 aioairzone-cloud-0.1.3/aioairzone_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-24 08:10:00.000000 aioairzone-cloud-0.1.3/aioairzone_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-24 08:10:00.000000 aioairzone-cloud-0.1.3/aioairzone_cloud.egg-info/requires.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-05-24 08:10:00.000000 aioairzone-cloud-0.1.3/aioairzone_cloud.egg-info/top_level.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1029 2023-05-24 08:08:52.000000 aioairzone-cloud-0.1.3/pyproject.toml
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.3/requirements.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-05-24 08:10:00.448727 aioairzone-cloud-0.1.3/setup.cfg
```

### Comparing `aioairzone-cloud-0.1.2/LICENSE` & `aioairzone-cloud-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.2/PKG-INFO` & `aioairzone-cloud-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.1.2
+Version: 0.1.3
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.1.2/README.md` & `aioairzone-cloud-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.2/aioairzone_cloud/cloudapi.py` & `aioairzone-cloud-0.1.3/aioairzone_cloud/cloudapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,45 +235,47 @@
                 API_EMAIL: self.options.username,
                 API_PASSWORD: self.options.password,
             },
         )
         _LOGGER.debug("login resp: %s", resp)
         if resp.keys() < {API_TOKEN, API_REFRESH_TOKEN}:
             raise LoginError("Invalid API response")
-        self.token = resp[API_TOKEN]
         self.refresh_time = datetime.now()
         self.refresh_token = resp[API_REFRESH_TOKEN]
+        self.token = resp[API_TOKEN]
 
     async def logout(self) -> None:
         """Perform Airzone Cloud API logout."""
         try:
             if self.token:
                 await self.api_request(
                     "GET",
                     f"{API_V1}/{API_USER_LOGOUT}",
                 )
         except AirzoneCloudError:
             pass
         finally:
+            self.refresh_time = None
             self.refresh_token = None
             self.token = None
 
     async def token_refresh(self) -> None:
         """Perform Airzone Cloud API token refresh."""
         if self.token and self.refresh_token:
             refresh_token = urllib.parse.quote(self.refresh_token)
             resp = await self.api_request(
                 "GET",
                 f"{API_V1}/{API_AUTH_REFRESH_TOKEN}/{refresh_token}",
             )
             _LOGGER.debug("refresh resp: %s", resp)
             if resp.keys() < {API_TOKEN, API_REFRESH_TOKEN}:
                 raise TokenRefreshError("Invalid API response")
-            self.token = resp[API_TOKEN]
+            self.refresh_time = datetime.now()
             self.refresh_token = resp[API_REFRESH_TOKEN]
+            self.token = resp[API_TOKEN]
 
     def raw_data(self) -> dict[str, Any]:
         """Return raw Airzone Cloud API data."""
         return self._api_raw_data
 
     def data(self) -> dict[str, Any]:
         """Return Airzone Cloud data."""
@@ -484,15 +486,15 @@
         await asyncio.gather(*tasks)
 
     async def update(self) -> None:
         """Update all Airzone Cloud data."""
 
         if (self.refresh_time is not None) and (
             datetime.now() - self.refresh_time
-        ) > TOKEN_REFRESH_PERIOD:
+        ) >= TOKEN_REFRESH_PERIOD:
             try:
                 await self.token_refresh()
             except TokenRefreshError:
                 await self.login()
 
         try:
             await self._update()
```

### Comparing `aioairzone-cloud-0.1.2/aioairzone_cloud/common.py` & `aioairzone-cloud-0.1.3/aioairzone_cloud/common.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.2/aioairzone_cloud/const.py` & `aioairzone-cloud-0.1.3/aioairzone_cloud/const.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.2/aioairzone_cloud/device.py` & `aioairzone-cloud-0.1.3/aioairzone_cloud/device.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.2/aioairzone_cloud/exceptions.py` & `aioairzone-cloud-0.1.3/aioairzone_cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.2/aioairzone_cloud/installation.py` & `aioairzone-cloud-0.1.3/aioairzone_cloud/installation.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.2/aioairzone_cloud/webserver.py` & `aioairzone-cloud-0.1.3/aioairzone_cloud/webserver.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.2/aioairzone_cloud/zone.py` & `aioairzone-cloud-0.1.3/aioairzone_cloud/zone.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.2/aioairzone_cloud.egg-info/PKG-INFO` & `aioairzone-cloud-0.1.3/aioairzone_cloud.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.1.2
+Version: 0.1.3
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.1.2/aioairzone_cloud.egg-info/SOURCES.txt` & `aioairzone-cloud-0.1.3/aioairzone_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.2/pyproject.toml` & `aioairzone-cloud-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aioairzone-cloud"
-version = "0.1.2"
+version = "0.1.3"
 description = "Library to control Airzone Cloud devices"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "Apache-2.0"}
 keywords = ["airzone", "cloud", "hvac", "home"] 
 authors = [
   {name = "Álvaro Fernández Rojas", email = "noltari@gmail.com" }
```

