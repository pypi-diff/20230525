# Comparing `tmp/aioairzone-cloud-0.1.3.tar.gz` & `tmp/aioairzone-cloud-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairzone-cloud-0.1.3.tar", last modified: Wed May 24 08:10:00 2023, max compression
+gzip compressed data, was "aioairzone-cloud-0.1.4.tar", last modified: Thu May 25 07:18:51 2023, max compression
```

## Comparing `aioairzone-cloud-0.1.3.tar` & `aioairzone-cloud-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-24 08:10:00.448727 aioairzone-cloud-0.1.3/
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.3/LICENSE
--rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.3/MANIFEST.in
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-24 08:10:00.448727 aioairzone-cloud-0.1.3/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      746 2023-05-22 17:43:05.000000 aioairzone-cloud-0.1.3/README.md
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-24 08:10:00.448727 aioairzone-cloud-0.1.3/aioairzone_cloud/
--rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.1.3/aioairzone_cloud/__init__.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    16851 2023-05-24 08:04:48.000000 aioairzone-cloud-0.1.3/aioairzone_cloud/cloudapi.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1527 2023-05-23 16:19:08.000000 aioairzone-cloud-0.1.3/aioairzone_cloud/common.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     6167 2023-05-23 06:40:31.000000 aioairzone-cloud-0.1.3/aioairzone_cloud/const.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3040 2023-05-23 16:26:50.000000 aioairzone-cloud-0.1.3/aioairzone_cloud/device.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      806 2023-05-21 08:34:57.000000 aioairzone-cloud-0.1.3/aioairzone_cloud/exceptions.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1184 2023-05-19 11:19:38.000000 aioairzone-cloud-0.1.3/aioairzone_cloud/installation.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-05-22 07:54:27.000000 aioairzone-cloud-0.1.3/aioairzone_cloud/py.typed
--rw-r--r--   0 noltari   (1000) noltari   (1000)      401 2023-05-23 16:26:50.000000 aioairzone-cloud-0.1.3/aioairzone_cloud/system.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3791 2023-05-19 11:19:38.000000 aioairzone-cloud-0.1.3/aioairzone_cloud/webserver.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    18130 2023-05-23 16:26:50.000000 aioairzone-cloud-0.1.3/aioairzone_cloud/zone.py
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-24 08:10:00.448727 aioairzone-cloud-0.1.3/aioairzone_cloud.egg-info/
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-24 08:10:00.000000 aioairzone-cloud-0.1.3/aioairzone_cloud.egg-info/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      619 2023-05-24 08:10:00.000000 aioairzone-cloud-0.1.3/aioairzone_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-24 08:10:00.000000 aioairzone-cloud-0.1.3/aioairzone_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-24 08:10:00.000000 aioairzone-cloud-0.1.3/aioairzone_cloud.egg-info/not-zip-safe
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-24 08:10:00.000000 aioairzone-cloud-0.1.3/aioairzone_cloud.egg-info/requires.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-05-24 08:10:00.000000 aioairzone-cloud-0.1.3/aioairzone_cloud.egg-info/top_level.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1029 2023-05-24 08:08:52.000000 aioairzone-cloud-0.1.3/pyproject.toml
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.3/requirements.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-05-24 08:10:00.448727 aioairzone-cloud-0.1.3/setup.cfg
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-25 07:18:51.370510 aioairzone-cloud-0.1.4/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.4/LICENSE
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.4/MANIFEST.in
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-25 07:18:51.370510 aioairzone-cloud-0.1.4/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      746 2023-05-22 17:43:05.000000 aioairzone-cloud-0.1.4/README.md
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-25 07:18:51.370510 aioairzone-cloud-0.1.4/aioairzone_cloud/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/__init__.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      156 2023-05-25 06:19:05.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/aidoo.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    18280 2023-05-24 19:18:04.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/cloudapi.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1527 2023-05-23 16:19:08.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/common.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     6443 2023-05-25 06:30:02.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/const.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2608 2023-05-25 06:22:30.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/device.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      806 2023-05-21 08:34:57.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/exceptions.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    16988 2023-05-25 06:16:28.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/hvac.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1181 2023-05-24 18:32:54.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/installation.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-05-22 07:54:27.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/py.typed
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      975 2023-05-25 06:23:06.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/system.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3844 2023-05-24 19:18:04.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/webserver.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2231 2023-05-25 06:23:06.000000 aioairzone-cloud-0.1.4/aioairzone_cloud/zone.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-25 07:18:51.370510 aioairzone-cloud-0.1.4/aioairzone_cloud.egg-info/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-25 07:18:51.000000 aioairzone-cloud-0.1.4/aioairzone_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      670 2023-05-25 07:18:51.000000 aioairzone-cloud-0.1.4/aioairzone_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-25 07:18:51.000000 aioairzone-cloud-0.1.4/aioairzone_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-25 07:18:51.000000 aioairzone-cloud-0.1.4/aioairzone_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-25 07:18:51.000000 aioairzone-cloud-0.1.4/aioairzone_cloud.egg-info/requires.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-05-25 07:18:51.000000 aioairzone-cloud-0.1.4/aioairzone_cloud.egg-info/top_level.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1029 2023-05-25 07:16:49.000000 aioairzone-cloud-0.1.4/pyproject.toml
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.4/requirements.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-05-25 07:18:51.370510 aioairzone-cloud-0.1.4/setup.cfg
```

### Comparing `aioairzone-cloud-0.1.3/LICENSE` & `aioairzone-cloud-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.3/PKG-INFO` & `aioairzone-cloud-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.1.3/README.md` & `aioairzone-cloud-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.3/aioairzone_cloud/cloudapi.py` & `aioairzone-cloud-0.1.4/aioairzone_cloud/cloudapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 import urllib.parse
 from datetime import datetime
 from typing import Any, cast
 
 from aiohttp import ClientConnectorError, ClientResponseError, ClientSession
 from aiohttp.client_reqrep import ClientResponse
 
+from .aidoo import Aidoo
 from .common import ConnectionOptions
 from .const import (
     API_AUTH_LOGIN,
     API_AUTH_REFRESH_TOKEN,
+    API_AZ_AIDOO,
     API_AZ_SYSTEM,
     API_AZ_ZONE,
     API_CONFIG,
     API_DEVICE_ID,
     API_DEVICE_TYPE,
     API_DEVICES,
     API_EMAIL,
@@ -31,14 +33,15 @@
     API_TYPE,
     API_URL,
     API_USER,
     API_USER_LOGOUT,
     API_V1,
     API_WS,
     API_WS_ID,
+    AZD_AIDOOS,
     AZD_INSTALLATIONS,
     AZD_SYSTEMS,
     AZD_WEBSERVERS,
     AZD_ZONES,
     HEADER_AUTHORIZATION,
     HEADER_BEARER,
     HTTP_CALL_TIMEOUT,
@@ -78,23 +81,24 @@
         """Airzone Cloud API init."""
         self._api_raw_data: dict[str, Any] = {
             RAW_DEVICES_CONFIG: {},
             RAW_DEVICES_STATUS: {},
             RAW_INSTALLATIONS: {},
             RAW_WEBSERVERS: {},
         }
+        self.aidoos: dict[str, Aidoo] = {}
         self.aiohttp_session = aiohttp_session
-        self.installations: list[Installation] = []
+        self.installations: dict[str, Installation] = {}
         self.options = options
         self.refresh_time: datetime | None = None
         self.refresh_token: str | None = None
-        self.systems: list[System] = []
+        self.systems: dict[str, System] = {}
         self.token: str | None = None
-        self.webservers: list[WebServer] = []
-        self.zones: list[Zone] = []
+        self.webservers: dict[str, WebServer] = {}
+        self.zones: dict[str, Zone] = {}
 
     async def api_request(
         self, method: str, path: str, json: Any | None = None
     ) -> dict[str, Any]:
         """Airzone Cloud API request."""
         _LOGGER.debug("aiohttp request: /%s (params=%s)", path, json)
 
@@ -277,133 +281,153 @@
         """Return raw Airzone Cloud API data."""
         return self._api_raw_data
 
     def data(self) -> dict[str, Any]:
         """Return Airzone Cloud data."""
         data: dict[str, Any] = {}
 
-        if self.installations:
+        if len(self.aidoos):
+            aidoos: dict[str, Any] = {}
+            for key, aidoo in self.aidoos.items():
+                aidoos[key] = aidoo.data()
+            data[AZD_AIDOOS] = aidoos
+
+        if len(self.installations):
             installations: dict[str, Any] = {}
-            for installation in self.installations:
-                installations[installation.get_id()] = installation.data()
+            for key, installation in self.installations.items():
+                installations[key] = installation.data()
             data[AZD_INSTALLATIONS] = installations
 
-        if self.systems:
+        if len(self.systems):
             systems: dict[str, Any] = {}
-            for system in self.systems:
-                systems[system.get_id()] = system.data()
+            for key, system in self.systems.items():
+                systems[key] = system.data()
             data[AZD_SYSTEMS] = systems
 
-        if self.webservers:
+        if len(self.webservers):
             webservers: dict[str, Any] = {}
-            for webserver in self.webservers:
-                webservers[webserver.get_id()] = webserver.data()
+            for key, webserver in self.webservers.items():
+                webservers[key] = webserver.data()
             data[AZD_WEBSERVERS] = webservers
 
-        if self.zones:
+        if len(self.zones):
             zones: dict[str, Any] = {}
-            for zone in self.zones:
-                zones[zone.get_id()] = zone.data()
+            for key, zone in self.zones.items():
+                zones[key] = zone.data()
             data[AZD_ZONES] = zones
 
         return data
 
+    def get_aidoo_id(self, aidoo_id: str) -> Aidoo | None:
+        """Return Airzone Cloud Aidoo by ID."""
+        return self.aidoos.get(aidoo_id)
+
     def get_installation_id(self, inst_id: str) -> Installation | None:
         """Return Airzone Cloud Installation by ID."""
-        for inst in self.installations:
-            if inst_id == inst.get_id():
-                return inst
-        return None
+        return self.installations.get(inst_id)
 
     def get_system_id(self, sys_id: str) -> System | None:
         """Return Airzone Cloud System by ID."""
-        for system in self.systems:
-            if sys_id == system.get_id():
-                return system
-        return None
+        return self.systems.get(sys_id)
 
     def get_webserver_id(self, ws_id: str) -> WebServer | None:
         """Return Airzone Cloud WebServer by ID."""
-        for ws in self.webservers:
-            if ws_id == ws.get_id():
-                return ws
-        return None
+        return self.webservers.get(ws_id)
 
     def get_zone_id(self, zone_id: str) -> Zone | None:
         """Return Airzone Cloud Zone by ID."""
-        for zone in self.zones:
-            if zone_id == zone.get_id():
-                return zone
-        return None
+        return self.zones.get(zone_id)
 
     async def list_installations(self) -> list[Installation]:
         """Return Airzone Cloud installations list."""
         inst_list: list[Installation] = []
 
         inst_data = await self.api_get_installations()
         for inst in inst_data[API_INSTALLATIONS]:
-            inst_list.append(Installation(inst))
+            inst_list += [Installation(inst)]
 
         return inst_list
 
     def select_installation(self, inst: Installation) -> None:
         """Select single Airzone Cloud installation."""
-        self.installations = [inst]
+        self.installations = {
+            inst.get_id(): inst,
+        }
         for ws_id in inst.get_webservers():
             if not self.get_webserver_id(ws_id):
-                ws = WebServer(inst.get_id(), ws_id)
-                self.webservers.append(ws)
+                self.webservers[ws_id] = WebServer(inst.get_id(), ws_id)
 
     def set_system_zones_data(self, system: System) -> None:
         """Set slave zones modes from master zone."""
         modes = system.get_modes()
         installation_id = system.get_installation()
         system_id = system.get_id()
         system_num = system.get_system()
-        for zone in self.zones:
-            zone.set_system_id(system_id)
-            is_slave = zone.get_master() is False
+        for zone in self.zones.values():
             if (
-                is_slave
-                and modes
-                and zone.get_installation() == installation_id
-                and zone.get_system() == system_num
+                zone.get_installation() != installation_id
+                or zone.get_system() != system_num
             ):
+                continue
+
+            zone.set_system_id(system_id)
+            if zone.get_master() is False and modes:
                 zone.set_modes(modes)
 
+    async def update_aidoo(self, aidoo: Aidoo) -> None:
+        """Update Airzone Cloud Zone from API."""
+        device_data = await self.api_get_device_status(aidoo)
+        aidoo.update(device_data)
+
+    async def update_aidoos(self) -> None:
+        """Update all Airzone Cloud Aidoos."""
+        tasks = []
+
+        for aidoo in self.aidoos.values():
+            tasks += [self.update_aidoo(aidoo)]
+
+        await asyncio.gather(*tasks)
+
     async def update_installation(self, inst: Installation) -> None:
         """Update Airzone Cloud installation from API."""
         installation_data = await self.api_get_installation(inst)
         for group in installation_data[API_GROUPS]:
             for device_data in group[API_DEVICES]:
                 if API_AZ_ZONE == device_data[API_TYPE]:
                     if not self.get_zone_id(device_data[API_DEVICE_ID]):
                         zone = Zone(inst.get_id(), device_data[API_WS_ID], device_data)
                         if zone:
-                            self.zones.append(zone)
+                            self.zones[zone.get_id()] = zone
                 elif API_AZ_SYSTEM == device_data[API_TYPE]:
                     if not self.get_system_id(device_data[API_DEVICE_ID]):
                         system = System(
                             inst.get_id(), device_data[API_WS_ID], device_data
                         )
                         if system:
-                            self.systems.append(system)
+                            self.systems[system.get_id()] = system
+                elif API_AZ_AIDOO == device_data[API_TYPE]:
+                    if not self.get_aidoo_id(device_data[API_DEVICE_ID]):
+                        aidoo = Aidoo(
+                            inst.get_id(), device_data[API_WS_ID], device_data
+                        )
+                        if aidoo:
+                            self.aidoos[aidoo.get_id()] = aidoo
 
     async def update_installations(self) -> None:
         """Update Airzone Cloud installations from API."""
         installations_data = await self.api_get_installations()
         for installation_data in installations_data[API_INSTALLATIONS]:
             if not self.get_installation_id(installation_data[API_INSTALLATION_ID]):
                 installation = Installation(installation_data)
                 if installation:
-                    self.installations.append(installation)
+                    self.installations[installation.get_id()] = installation
                     for ws_id in installation.get_webservers():
                         if not self.get_webserver_id(ws_id):
                             ws = WebServer(installation.get_id(), ws_id)
-                            self.webservers.append(ws)
+                            self.webservers[ws_id] = ws
 
     async def update_system(self, system: System) -> None:
         """Update Airzone Cloud System from API."""
         device_data = await self.api_get_device_status(system)
         system.update(device_data)
 
     async def update_system_id(self, sys_id: str) -> None:
@@ -412,47 +436,52 @@
         if system:
             await self.update_system(system)
 
     async def update_systems(self) -> None:
         """Update all Airzone Cloud Systems."""
         tasks = []
 
-        for system in self.systems:
+        for system in self.systems.values():
             tasks += [self.update_system(system)]
 
         await asyncio.gather(*tasks)
 
     async def update_webserver(self, ws: WebServer, devices: bool) -> None:
         """Update Airzone Cloud WebServer from API."""
         ws_data = await self.api_get_webserver(ws, devices)
         ws.update(ws_data)
         if devices:
             for device_data in ws_data[API_DEVICES]:
                 if API_AZ_ZONE == device_data[API_DEVICE_TYPE]:
                     if not self.get_zone_id(device_data[API_DEVICE_ID]):
                         zone = Zone(ws.get_installation(), ws.get_id(), device_data)
                         if zone:
-                            self.zones.append(zone)
+                            self.zones[zone.get_id()] = zone
                 elif API_AZ_SYSTEM == device_data[API_DEVICE_TYPE]:
                     if not self.get_system_id(device_data[API_DEVICE_ID]):
                         system = System(ws.get_installation(), ws.get_id(), device_data)
                         if system:
-                            self.systems.append(system)
+                            self.systems[system.get_id()] = system
+                elif API_AZ_AIDOO == device_data[API_DEVICE_TYPE]:
+                    if not self.get_aidoo_id(device_data[API_DEVICE_ID]):
+                        aidoo = Aidoo(ws.get_installation(), ws.get_id(), device_data)
+                        if aidoo:
+                            self.aidoos[aidoo.get_id()] = aidoo
 
     async def update_webserver_id(self, ws_id: str, devices: bool) -> None:
         """Update Airzone Cloud WebServer by ID."""
         ws = self.get_webserver_id(ws_id)
         if ws:
             await self.update_webserver(ws, devices)
 
     async def update_webservers(self, devices: bool) -> None:
         """Update all Airzone Cloud WebServers."""
         tasks = []
 
-        for ws in self.webservers:
+        for ws in self.webservers.values():
             tasks += [self.update_webserver(ws, devices)]
 
         await asyncio.gather(*tasks)
 
     async def update_zone(self, zone: Zone) -> None:
         """Update Airzone Cloud Zone from API."""
         device_data = await self.api_get_device_status(zone)
@@ -464,27 +493,28 @@
         if zone:
             await self.update_zone(zone)
 
     async def update_zones(self) -> None:
         """Update all Airzone Cloud Zones."""
         tasks = []
 
-        for zone in self.zones:
+        for zone in self.zones.values():
             tasks += [self.update_zone(zone)]
 
         await asyncio.gather(*tasks)
 
-        for system in self.systems:
+        for system in self.systems.values():
             self.set_system_zones_data(system)
 
     async def _update(self) -> None:
         tasks = [
             self.update_webservers(False),
             self.update_systems(),
             self.update_zones(),
+            self.update_aidoos(),
         ]
 
         await asyncio.gather(*tasks)
 
     async def update(self) -> None:
         """Update all Airzone Cloud data."""
```

### Comparing `aioairzone-cloud-0.1.3/aioairzone_cloud/common.py` & `aioairzone-cloud-0.1.4/aioairzone_cloud/common.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.3/aioairzone_cloud/const.py` & `aioairzone-cloud-0.1.4/aioairzone_cloud/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,36 +2,41 @@
 
 from datetime import timedelta
 from typing import Final
 
 API_AUTH_LOGIN: Final[str] = "auth/login"
 API_AUTH_REFRESH_TOKEN: Final[str] = "auth/refreshToken"
 API_CELSIUS: Final[str] = "celsius"
+API_CITY: Final[str] = "city"
 API_CONFIG: Final[str] = "config"
 API_CONNECTION_DATE: Final[str] = "connection_date"
 API_DEVICE_ID: Final[str] = "device_id"
 API_DEVICE_TYPE: Final[str] = "device_type"
 API_DEVICES: Final[str] = "devices"
 API_DISCONNECTION_DATE: Final[str] = "disconnection_date"
 API_ECO_CONF: Final[str] = "eco_conf"
 API_EMAIL: Final[str] = "email"
 API_FAH: Final[str] = "fah"
+API_GROUP_ID: Final[str] = "group_id"
 API_GROUPS: Final[str] = "groups"
 API_HUMIDITY: Final[str] = "humidity"
 API_INSTALLATION_ID: Final[str] = "installation_id"
 API_INSTALLATIONS: Final[str] = "installations"
 API_IS_CONNECTED: Final[str] = "isConnected"
 API_LOCAL_TEMP: Final[str] = "local_temp"
+API_LOCATION_ID: Final[str] = "location_id"
 API_META: Final[str] = "meta"
 API_MODE: Final[str] = "mode"
 API_MODE_AVAIL: Final[str] = "mode_available"
 API_NAME: Final[str] = "name"
+API_OLD_ID: Final[str] = "_id"
 API_OPTS: Final[str] = "opts"
 API_PARAMS: Final[str] = "params"
 API_PASSWORD: Final[str] = "password"
+API_PIN: Final[str] = "pin"
 API_POWER: Final[str] = "power"
 API_RANGE_SP_MAX_COOL_AIR: Final[str] = "range_sp_cool_air_max"
 API_RANGE_SP_MAX_DRY_AIR: Final[str] = "range_sp_dry_air_max"
 API_RANGE_SP_MAX_EMERHEAT_AIR: Final[str] = "range_sp_emerheat_air_max"
 API_RANGE_SP_MAX_HOT_AIR: Final[str] = "range_sp_hot_air_max"
 API_RANGE_SP_MAX_STOP_AIR: Final[str] = "range_sp_stop_air_max"
 API_RANGE_SP_MAX_VENT_AIR: Final[str] = "range_sp_vent_air_max"
@@ -59,29 +64,32 @@
 API_SYSTEM_NUMBER: Final[str] = "system_number"
 API_TIMER: Final[str] = "timer"
 API_TOKEN: Final[str] = "token"
 API_TYPE: Final[str] = "type"
 API_UNITS: Final[str] = "units"
 API_URL: Final[str] = "https://m.airzonecloud.com"
 API_USER: Final[str] = "user"
+API_USER_ID: Final[str] = "user_id"
 API_USER_LOGOUT: Final[str] = "user/logout"
 API_USER_MODE_CONF: Final[str] = "usermode_conf"
 API_V1: Final[str] = "api/v1"
 API_WS: Final[str] = "ws"
 API_WS_FW: Final[str] = "ws_fw"
 API_WS_ID: Final[str] = "ws_id"
 API_WS_IDS: Final[str] = "ws_ids"
 API_WS_TYPE: Final[str] = "ws_type"
 API_ZONE_NUMBER: Final[str] = "zone_number"
 
+API_AZ_AIDOO: Final[str] = "aidoo"
 API_AZ_SYSTEM: Final[str] = "az_system"
 API_AZ_ZONE: Final[str] = "az_zone"
 
 API_DEFAULT_TEMP_STEP: Final[float] = 0.5
 
+AZD_AIDOOS: Final[str] = "aidoos"
 AZD_CONNECTED: Final[str] = "connected"
 AZD_CONNECTION_DATE: Final[str] = "connection-date"
 AZD_DISCONNECTION_DATE: Final[str] = "disconnection-date"
 AZD_FIRMWARE: Final[str] = "firmware"
 AZD_HUMIDITY: Final[str] = "humidity"
 AZD_ID: Final[str] = "id"
 AZD_INSTALLATION: Final[str] = "installation"
```

### Comparing `aioairzone-cloud-0.1.3/aioairzone_cloud/device.py` & `aioairzone-cloud-0.1.4/aioairzone_cloud/device.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 """Airzone Cloud API Device."""
 from __future__ import annotations
 
 from typing import Any
 
 from .common import OperationMode
 from .const import (
-    API_CONFIG,
     API_DEVICE_ID,
     API_IS_CONNECTED,
-    API_META,
     API_MODE,
     API_MODE_AVAIL,
-    API_SYSTEM_NUMBER,
     AZD_CONNECTED,
     AZD_ID,
     AZD_INSTALLATION,
     AZD_MODE,
     AZD_MODES,
     AZD_NAME,
-    AZD_SYSTEM,
     AZD_WEBSERVER,
 )
 
 
 class Device:
     """Airzone Cloud Device."""
 
@@ -33,31 +29,25 @@
         """Airzone Cloud Device init."""
         self.id = str(device_data[API_DEVICE_ID])
         self.installation_id = inst_id
         self.mode: OperationMode | None = None
         self.modes: list[OperationMode] = []
         self.webserver_id = ws_id
 
-        if API_CONFIG in device_data:
-            self.system_number = int(device_data[API_CONFIG][API_SYSTEM_NUMBER])
-        else:
-            self.system_number = int(device_data[API_META][API_SYSTEM_NUMBER])
-
         if API_IS_CONNECTED in device_data:
             self.connected = bool(device_data[API_IS_CONNECTED])
 
     def data(self) -> dict[str, Any]:
         """Return Device data."""
         data = {
             AZD_CONNECTED: self.get_connected(),
             AZD_ID: self.get_id(),
             AZD_INSTALLATION: self.get_installation(),
             AZD_MODE: self.get_mode(),
             AZD_NAME: self.get_name(),
-            AZD_SYSTEM: self.get_system(),
             AZD_WEBSERVER: self.get_webserver(),
         }
 
         modes = self.get_modes()
         if modes:
             data[AZD_MODES] = modes
 
@@ -85,27 +75,23 @@
             return self.modes
         return None
 
     def get_name(self) -> str:
         """Return Device name."""
         return self.name
 
-    def get_system(self) -> int:
-        """Return System number."""
-        return self.system_number
-
     def get_webserver(self) -> str:
         """Return WebServer ID."""
         return self.webserver_id
 
     def update(self, data: dict[str, Any]) -> None:
         """Update Device data."""
         if API_IS_CONNECTED in data:
             self.connected = bool(data[API_IS_CONNECTED])
 
         if API_MODE in data:
             self.mode = OperationMode(data[API_MODE])
         if API_MODE_AVAIL in data and len(data[API_MODE_AVAIL]) > 0:
             modes = []
             for mode in data[API_MODE_AVAIL]:
-                modes.append(OperationMode(mode))
+                modes += [OperationMode(mode)]
             self.modes = modes
```

### Comparing `aioairzone-cloud-0.1.3/aioairzone_cloud/exceptions.py` & `aioairzone-cloud-0.1.4/aioairzone_cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.3/aioairzone_cloud/installation.py` & `aioairzone-cloud-0.1.4/aioairzone_cloud/installation.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     def __init__(self, inst_data: dict[str, Any]):
         """Airzone Cloud Installation init."""
         self.id = str(inst_data[API_INSTALLATION_ID])
         self.name = str(inst_data[API_NAME])
         self.webservers: list[str] = []
 
         for ws_id in inst_data[API_WS_IDS]:
-            self.webservers.append(ws_id)
+            self.webservers += [ws_id]
 
     def data(self) -> dict[str, Any]:
         """Return Installation data."""
         data: dict[str, Any] = {
             AZD_ID: self.get_id(),
             AZD_NAME: self.get_name(),
             AZD_WEBSERVERS: self.get_webservers(),
```

### Comparing `aioairzone-cloud-0.1.3/aioairzone_cloud/webserver.py` & `aioairzone-cloud-0.1.4/aioairzone_cloud/webserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,20 @@
         """Update WebServer data."""
         self.connected = bool(data[API_STATUS][API_IS_CONNECTED])
         self.connection_date = str(data[API_STATUS][API_CONNECTION_DATE])
         self.disconnection_date = str(data[API_STATUS][API_DISCONNECTION_DATE])
         self.firmware = str(data[API_CONFIG][API_WS_FW])
         self.type = str(data[API_WS_TYPE])
         self.wifi_channel = int(data[API_CONFIG][API_STAT_CHANNEL])
-        self.wifi_mac = str(data[API_CONFIG][API_STAT_AP_MAC])
         self.wifi_quality = int(data[API_STATUS][API_STAT_QUALITY])
         self.wifi_ssid = str(data[API_CONFIG][API_STAT_SSID])
 
+        if API_STAT_AP_MAC in data[API_CONFIG]:
+            self.wifi_mac = str(data[API_CONFIG][API_STAT_AP_MAC])
+
     def data(self) -> dict[str, Any]:
         """Return WebServer data."""
         return {
             AZD_CONNECTED: self.get_connected(),
             AZD_CONNECTION_DATE: self.get_connection_date(),
             AZD_DISCONNECTION_DATE: self.get_disconnection_date(),
             AZD_FIRMWARE: self.get_firmware(),
```

### Comparing `aioairzone-cloud-0.1.3/aioairzone_cloud/zone.py` & `aioairzone-cloud-0.1.4/aioairzone_cloud/hvac.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-"""Airzone Cloud API Zone."""
+"""Airzone Cloud API HVAC device."""
 from __future__ import annotations
 
 from typing import Any
 
-from aioairzone_cloud.common import OperationMode
-
 from .const import (
     API_CELSIUS,
-    API_CONFIG,
     API_DEFAULT_TEMP_STEP,
     API_HUMIDITY,
     API_LOCAL_TEMP,
-    API_META,
-    API_MODE_AVAIL,
     API_NAME,
     API_POWER,
     API_RANGE_SP_MAX_COOL_AIR,
     API_RANGE_SP_MAX_DRY_AIR,
     API_RANGE_SP_MAX_EMERHEAT_AIR,
     API_RANGE_SP_MAX_HOT_AIR,
     API_RANGE_SP_MAX_STOP_AIR,
@@ -29,19 +24,16 @@
     API_RANGE_SP_MIN_VENT_AIR,
     API_SP_AIR_COOL,
     API_SP_AIR_DRY,
     API_SP_AIR_HEAT,
     API_SP_AIR_STOP,
     API_SP_AIR_VENT,
     API_STEP,
-    API_ZONE_NUMBER,
     AZD_HUMIDITY,
-    AZD_MASTER,
     AZD_POWER,
-    AZD_SYSTEM_ID,
     AZD_TEMP,
     AZD_TEMP_SET,
     AZD_TEMP_SET_COOL_AIR,
     AZD_TEMP_SET_DRY_AIR,
     AZD_TEMP_SET_HOT_AIR,
     AZD_TEMP_SET_MAX,
     AZD_TEMP_SET_MAX_COOL_AIR,
@@ -56,31 +48,28 @@
     AZD_TEMP_SET_MIN_EMERHEAT_AIR,
     AZD_TEMP_SET_MIN_HOT_AIR,
     AZD_TEMP_SET_MIN_STOP_AIR,
     AZD_TEMP_SET_MIN_VENT_AIR,
     AZD_TEMP_SET_STOP_AIR,
     AZD_TEMP_SET_VENT_AIR,
     AZD_TEMP_STEP,
-    AZD_ZONE,
 )
 from .device import Device
 
 
-class Zone(Device):
-    """Airzone Cloud Zone."""
+class HVAC(Device):
+    """Airzone Cloud HVAC device."""
 
     def __init__(self, inst_id: str, ws_id: str, device_data: dict[str, Any]):
-        """Airzone Cloud Zone init."""
+        """Airzone Cloud HVAC device init."""
         super().__init__(inst_id, ws_id, device_data)
 
         self.humidity: int | None = None
-        self.master: bool | None = None
         self.name = str(device_data[API_NAME])
         self.power: bool | None = None
-        self.system_id: str | None = None
         self.temp_set_max_cool_air: float | None = None
         self.temp_set_max_dry_air: float | None = None
         self.temp_set_max_emerheat_air: float | None = None
         self.temp_set_max_hot_air: float | None = None
         self.temp_set_max_stop_air: float | None = None
         self.temp_set_max_vent_air: float | None = None
         self.temp_set_min_cool_air: float | None = None
@@ -93,33 +82,22 @@
         self.temp_set_dry_air: float | None = None
         self.temp_set_hot_air: float | None = None
         self.temp_set_stop_air: float | None = None
         self.temp_set_vent_air: float | None = None
         self.temp: float | None = None
         self.temp_step: float | None = None
 
-        if API_CONFIG in device_data:
-            self.zone_number = int(device_data[API_CONFIG][API_ZONE_NUMBER])
-        else:
-            self.zone_number = int(device_data[API_META][API_ZONE_NUMBER])
-
     def data(self) -> dict[str, Any]:
-        """Return Zone data."""
+        """Return HVAC device data."""
         data = super().data()
 
         data[AZD_HUMIDITY] = self.get_humidity()
-        data[AZD_MASTER] = self.get_master()
         data[AZD_POWER] = self.get_power()
         data[AZD_TEMP] = self.get_temperature()
         data[AZD_TEMP_STEP] = self.get_temp_step()
-        data[AZD_ZONE] = self.get_zone()
-
-        system_id = self.get_system_id()
-        if system_id:
-            data[AZD_SYSTEM_ID] = system_id
 
         temp_set_max = self.get_temp_set_max()
         if temp_set_max:
             data[AZD_TEMP_SET_MAX] = temp_set_max
         temp_set_max_cool_air = self.get_temp_set_max_cool_air()
         if temp_set_max_cool_air:
             data[AZD_TEMP_SET_MAX_COOL_AIR] = temp_set_max_cool_air
@@ -179,37 +157,29 @@
         temp_set_vent_air = self.get_temp_set_vent_air()
         if temp_set_vent_air:
             data[AZD_TEMP_SET_VENT_AIR] = temp_set_vent_air
 
         return data
 
     def get_humidity(self) -> int | None:
-        """Return Zone humidity."""
+        """Return HVAC device humidity."""
         return self.humidity
 
-    def get_master(self) -> bool | None:
-        """Return Zone master/slave."""
-        return self.master
-
     def get_power(self) -> bool | None:
-        """Return Zone power."""
+        """Return HVAC device power."""
         return self.power
 
-    def get_system_id(self) -> str | None:
-        """Return System ID."""
-        return self.system_id
-
     def get_temperature(self) -> float | None:
-        """Return Zone temperature."""
+        """Return HVAC device temperature."""
         if self.temp:
             return round(self.temp, 1)
         return None
 
     def get_temp_set(self) -> float | None:
-        """Return Zone temperature setpoint."""
+        """Return HVAC device temperature setpoint."""
         temp_set: float | None = None
         mode = self.get_mode()
         if mode:
             if mode.is_cool():
                 temp_set = self.get_temp_set_cool_air()
             elif mode.is_dry():
                 temp_set = self.get_temp_set_dry_air()
@@ -218,45 +188,45 @@
             elif mode.is_stop():
                 temp_set = self.get_temp_set_stop_air()
             elif mode.is_vent():
                 temp_set = self.get_temp_set_vent_air()
         return temp_set
 
     def get_temp_set_cool_air(self) -> float | None:
-        """Return Zone setpoint for Cool Air."""
+        """Return HVAC device setpoint for Cool Air."""
         if self.temp_set_cool_air:
             return round(self.temp_set_cool_air, 1)
         return None
 
     def get_temp_set_dry_air(self) -> float | None:
-        """Return Zone setpoint for Dry Air."""
+        """Return HVAC device setpoint for Dry Air."""
         if self.temp_set_dry_air:
             return round(self.temp_set_dry_air, 1)
         return None
 
     def get_temp_set_hot_air(self) -> float | None:
-        """Return Zone setpoint for Heat Air."""
+        """Return HVAC device setpoint for Heat Air."""
         if self.temp_set_hot_air:
             return round(self.temp_set_hot_air, 1)
         return None
 
     def get_temp_set_stop_air(self) -> float | None:
-        """Return Zone setpoint for Stop Air."""
+        """Return HVAC device setpoint for Stop Air."""
         if self.temp_set_stop_air:
             return round(self.temp_set_stop_air, 1)
         return None
 
     def get_temp_set_vent_air(self) -> float | None:
-        """Return Zone setpoint for Ventilation Air."""
+        """Return HVAC device setpoint for Ventilation Air."""
         if self.temp_set_vent_air:
             return round(self.temp_set_vent_air, 1)
         return None
 
     def get_temp_set_max(self) -> float | None:
-        """Return Zone max setpoint."""
+        """Return HVAC device max setpoint."""
         max_temp: float | None = None
         temps = [
             self.get_temp_set_max_cool_air(),
             self.get_temp_set_max_dry_air(),
             self.get_temp_set_max_emerheat_air(),
             self.get_temp_set_max_hot_air(),
             self.get_temp_set_max_stop_air(),
@@ -265,51 +235,51 @@
         for temp in temps:
             if temp is not None:
                 if max_temp is None or temp > max_temp:
                     max_temp = temp
         return max_temp
 
     def get_temp_set_max_cool_air(self) -> float | None:
-        """Return Zone max setpoint for Cool Air."""
+        """Return HVAC device max setpoint for Cool Air."""
         if self.temp_set_max_cool_air:
             return round(self.temp_set_max_cool_air, 1)
         return None
 
     def get_temp_set_max_dry_air(self) -> float | None:
-        """Return Zone max setpoint for Dry Air."""
+        """Return HVAC device max setpoint for Dry Air."""
         if self.temp_set_max_dry_air:
             return round(self.temp_set_max_dry_air, 1)
         return None
 
     def get_temp_set_max_emerheat_air(self) -> float | None:
-        """Return Zone max setpoint for Emergency Heat Air."""
+        """Return HVAC device max setpoint for Emergency Heat Air."""
         if self.temp_set_max_emerheat_air:
             return round(self.temp_set_max_emerheat_air, 1)
         return None
 
     def get_temp_set_max_hot_air(self) -> float | None:
-        """Return Zone max setpoint for Heat Air."""
+        """Return HVAC device max setpoint for Heat Air."""
         if self.temp_set_max_hot_air:
             return round(self.temp_set_max_hot_air, 1)
         return None
 
     def get_temp_set_max_stop_air(self) -> float | None:
-        """Return Zone max setpoint for Stop Air."""
+        """Return HVAC device max setpoint for Stop Air."""
         if self.temp_set_max_stop_air:
             return round(self.temp_set_max_stop_air, 1)
         return None
 
     def get_temp_set_max_vent_air(self) -> float | None:
-        """Return Zone max setpoint for Ventilation Air."""
+        """Return HVAC device max setpoint for Ventilation Air."""
         if self.temp_set_max_vent_air:
             return round(self.temp_set_max_vent_air, 1)
         return None
 
     def get_temp_set_min(self) -> float | None:
-        """Return Zone min setpoint."""
+        """Return HVAC device min setpoint."""
         min_temp: float | None = None
         temps = [
             self.get_temp_set_min_cool_air(),
             self.get_temp_set_min_dry_air(),
             self.get_temp_set_min_emerheat_air(),
             self.get_temp_set_min_hot_air(),
             self.get_temp_set_min_stop_air(),
@@ -318,83 +288,66 @@
         for temp in temps:
             if temp is not None:
                 if min_temp is None or temp < min_temp:
                     min_temp = temp
         return min_temp
 
     def get_temp_set_min_cool_air(self) -> float | None:
-        """Return Zone min setpoint for Cool Air."""
+        """Return HVAC device min setpoint for Cool Air."""
         if self.temp_set_min_cool_air:
             return round(self.temp_set_min_cool_air, 1)
         return None
 
     def get_temp_set_min_dry_air(self) -> float | None:
-        """Return Zone min setpoint for Dry Air."""
+        """Return HVAC device min setpoint for Dry Air."""
         if self.temp_set_min_dry_air:
             return round(self.temp_set_min_dry_air, 1)
         return None
 
     def get_temp_set_min_emerheat_air(self) -> float | None:
-        """Return Zone min setpoint for Emergency Heat Air."""
+        """Return HVAC device min setpoint for Emergency Heat Air."""
         if self.temp_set_min_emerheat_air:
             return round(self.temp_set_min_emerheat_air, 1)
         return None
 
     def get_temp_set_min_hot_air(self) -> float | None:
-        """Return Zone min setpoint for Hot Air."""
+        """Return HVAC device min setpoint for Hot Air."""
         if self.temp_set_min_hot_air:
             return round(self.temp_set_min_hot_air, 1)
         return None
 
     def get_temp_set_min_stop_air(self) -> float | None:
-        """Return Zone min setpoint for Stop Air."""
+        """Return HVAC device min setpoint for Stop Air."""
         if self.temp_set_min_stop_air:
             return round(self.temp_set_min_stop_air, 1)
         return None
 
     def get_temp_set_min_vent_air(self) -> float | None:
-        """Return Zone min setpoint for Ventilation Air."""
+        """Return HVAC device min setpoint for Ventilation Air."""
         if self.temp_set_min_vent_air:
             return round(self.temp_set_min_vent_air, 1)
         return None
 
     def get_temp_step(self) -> float | None:
-        """Return Zone temperature step."""
+        """Return HVAC device temperature step."""
         if self.temp_step:
             return round(self.temp_step, 1)
         return API_DEFAULT_TEMP_STEP
 
-    def get_zone(self) -> int:
-        """Return Zone number."""
-        return self.zone_number
-
-    def set_modes(self, modes: list[OperationMode]) -> None:
-        """Set slave zone modes."""
-        self.modes = modes
-
-    def set_system_id(self, system_id: str) -> None:
-        """Set System ID."""
-        self.system_id = system_id
-
     def update(self, data: dict[str, Any]) -> None:
-        """Update Zone data."""
+        """Update HVAC device data."""
         super().update(data)
 
         if API_HUMIDITY in data:
             self.humidity = int(data[API_HUMIDITY])
 
         if API_LOCAL_TEMP in data:
             if API_CELSIUS in data[API_LOCAL_TEMP]:
                 self.temp = float(data[API_LOCAL_TEMP][API_CELSIUS])
 
-        if API_MODE_AVAIL in data:
-            self.master = len(data[API_MODE_AVAIL]) > 0
-        else:
-            self.master = None
-
         if API_POWER in data:
             self.power = bool(data[API_POWER])
 
         if API_RANGE_SP_MAX_COOL_AIR in data:
             if API_CELSIUS in data[API_RANGE_SP_MAX_COOL_AIR]:
                 self.temp_set_max_cool_air = float(
                     data[API_RANGE_SP_MAX_COOL_AIR][API_CELSIUS]
```

### Comparing `aioairzone-cloud-0.1.3/aioairzone_cloud.egg-info/PKG-INFO` & `aioairzone-cloud-0.1.4/aioairzone_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.1.3/pyproject.toml` & `aioairzone-cloud-0.1.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aioairzone-cloud"
-version = "0.1.3"
+version = "0.1.4"
 description = "Library to control Airzone Cloud devices"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "Apache-2.0"}
 keywords = ["airzone", "cloud", "hvac", "home"] 
 authors = [
   {name = "Álvaro Fernández Rojas", email = "noltari@gmail.com" }
```

