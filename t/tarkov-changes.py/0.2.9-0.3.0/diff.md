# Comparing `tmp/tarkov-changes.py-0.2.9.tar.gz` & `tmp/tarkov-changes.py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarkov-changes.py-0.2.9.tar", last modified: Thu Aug  4 10:07:12 2022, max compression
+gzip compressed data, was "tarkov-changes.py-0.3.0.tar", last modified: Thu May 25 17:58:20 2023, max compression
```

## Comparing `tarkov-changes.py-0.2.9.tar` & `tarkov-changes.py-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2022-08-04 10:07:12.965224 tarkov-changes.py-0.2.9/
--rw-rw-rw-   0        0        0     1081 2022-07-24 11:26:46.000000 tarkov-changes.py-0.2.9/LICENSE
--rw-rw-rw-   0        0        0     3879 2022-08-04 10:07:12.961688 tarkov-changes.py-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     3547 2022-07-26 08:54:53.000000 tarkov-changes.py-0.2.9/README.rst
--rw-rw-rw-   0        0        0       42 2022-08-04 10:07:12.965224 tarkov-changes.py-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0      990 2022-07-25 20:09:13.000000 tarkov-changes.py-0.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-04 10:07:12.477255 tarkov-changes.py-0.2.9/tarkov_changes.py.egg-info/
--rw-rw-rw-   0        0        0     3879 2022-08-04 10:07:11.000000 tarkov-changes.py-0.2.9/tarkov_changes.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      696 2022-08-04 10:07:12.000000 tarkov-changes.py-0.2.9/tarkov_changes.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-04 10:07:11.000000 tarkov-changes.py-0.2.9/tarkov_changes.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2022-08-04 10:07:11.000000 tarkov-changes.py-0.2.9/tarkov_changes.py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-08-04 10:07:12.629356 tarkov-changes.py-0.2.9/tvc/
--rw-rw-rw-   0        0        0      504 2022-08-04 10:06:12.000000 tarkov-changes.py-0.2.9/tvc/__init__.py
--rw-rw-rw-   0        0        0     2958 2022-08-04 10:06:11.000000 tarkov-changes.py-0.2.9/tvc/ammunition.py
--rw-rw-rw-   0        0        0     1994 2022-08-04 10:06:11.000000 tarkov-changes.py-0.2.9/tvc/armor.py
--rw-rw-rw-   0        0        0     1404 2022-08-04 10:06:12.000000 tarkov-changes.py-0.2.9/tvc/backpack.py
--rw-rw-rw-   0        0        0      895 2022-08-02 09:41:31.000000 tarkov-changes.py-0.2.9/tvc/barter.py
--rw-rw-rw-   0        0        0     6173 2022-08-01 08:40:22.000000 tarkov-changes.py-0.2.9/tvc/client.py
--rw-rw-rw-   0        0        0     8129 2022-07-27 13:41:49.000000 tarkov-changes.py-0.2.9/tvc/enums.py
--rw-rw-rw-   0        0        0     1249 2022-07-26 05:36:07.000000 tarkov-changes.py-0.2.9/tvc/exceptions.py
--rw-rw-rw-   0        0        0     1300 2022-08-04 10:06:10.000000 tarkov-changes.py-0.2.9/tvc/food.py
--rw-rw-rw-   0        0        0     1538 2022-08-04 10:06:10.000000 tarkov-changes.py-0.2.9/tvc/grenade.py
--rw-rw-rw-   0        0        0     2198 2022-08-04 10:06:10.000000 tarkov-changes.py-0.2.9/tvc/headphone.py
--rw-rw-rw-   0        0        0     1123 2022-08-04 10:04:42.000000 tarkov-changes.py-0.2.9/tvc/item.py
--rw-rw-rw-   0        0        0     1847 2022-08-04 10:04:42.000000 tarkov-changes.py-0.2.9/tvc/key.py
--rw-rw-rw-   0        0        0     1234 2022-08-04 10:05:07.000000 tarkov-changes.py-0.2.9/tvc/maps.py
--rw-rw-rw-   0        0        0     1708 2022-08-02 10:37:16.000000 tarkov-changes.py-0.2.9/tvc/mixins.py
--rw-rw-rw-   0        0        0     5678 2022-08-01 08:39:38.000000 tarkov-changes.py-0.2.9/tvc/requester.py
-drwxrwxrwx   0        0        0        0 2022-08-04 10:07:12.958181 tarkov-changes.py-0.2.9/tvc/types/
--rw-rw-rw-   0        0        0      156 2022-07-25 20:10:52.000000 tarkov-changes.py-0.2.9/tvc/types/__init__.py
--rw-rw-rw-   0        0        0      750 2022-07-26 05:11:05.000000 tarkov-changes.py-0.2.9/tvc/types/ammunition.py
--rw-rw-rw-   0        0        0      591 2022-07-26 05:11:05.000000 tarkov-changes.py-0.2.9/tvc/types/armor.py
--rw-rw-rw-   0        0        0      338 2022-07-26 05:11:05.000000 tarkov-changes.py-0.2.9/tvc/types/backpack.py
--rw-rw-rw-   0        0        0      149 2022-08-01 08:39:38.000000 tarkov-changes.py-0.2.9/tvc/types/banned.py
--rw-rw-rw-   0        0        0      276 2022-07-26 05:11:05.000000 tarkov-changes.py-0.2.9/tvc/types/barter.py
--rw-rw-rw-   0        0        0      230 2022-07-26 05:11:05.000000 tarkov-changes.py-0.2.9/tvc/types/cell.py
--rw-rw-rw-   0        0        0      390 2022-08-01 08:33:43.000000 tarkov-changes.py-0.2.9/tvc/types/food.py
--rw-rw-rw-   0        0        0      514 2022-07-26 05:11:05.000000 tarkov-changes.py-0.2.9/tvc/types/grenade.py
--rw-rw-rw-   0        0        0      709 2022-07-26 08:40:18.000000 tarkov-changes.py-0.2.9/tvc/types/headphone.py
--rw-rw-rw-   0        0        0      210 2022-07-25 18:19:21.000000 tarkov-changes.py-0.2.9/tvc/types/item.py
--rw-rw-rw-   0        0        0      353 2022-07-26 05:11:05.000000 tarkov-changes.py-0.2.9/tvc/types/key.py
--rw-rw-rw-   0        0        0      382 2022-07-26 05:53:49.000000 tarkov-changes.py-0.2.9/tvc/types/maps.py
--rw-rw-rw-   0        0        0      361 2022-07-24 11:33:39.000000 tarkov-changes.py-0.2.9/tvc/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:58:20.098542 tarkov-changes.py-0.3.0/
+-rw-rw-rw-   0        0        0     1081 2022-07-24 11:26:46.000000 tarkov-changes.py-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     3856 2023-05-25 17:58:20.096542 tarkov-changes.py-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3547 2022-07-26 08:54:53.000000 tarkov-changes.py-0.3.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-05-25 17:58:20.098542 tarkov-changes.py-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      990 2022-07-25 20:09:13.000000 tarkov-changes.py-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:58:20.068949 tarkov-changes.py-0.3.0/tarkov_changes.py.egg-info/
+-rw-rw-rw-   0        0        0     3856 2023-05-25 17:58:19.000000 tarkov-changes.py-0.3.0/tarkov_changes.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      696 2023-05-25 17:58:20.000000 tarkov-changes.py-0.3.0/tarkov_changes.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 17:58:19.000000 tarkov-changes.py-0.3.0/tarkov_changes.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-25 17:58:19.000000 tarkov-changes.py-0.3.0/tarkov_changes.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 17:58:20.082985 tarkov-changes.py-0.3.0/tvc/
+-rw-rw-rw-   0        0        0      504 2023-05-25 17:57:35.000000 tarkov-changes.py-0.3.0/tvc/__init__.py
+-rw-rw-rw-   0        0        0     2958 2022-08-04 10:06:11.000000 tarkov-changes.py-0.3.0/tvc/ammunition.py
+-rw-rw-rw-   0        0        0     1994 2022-08-04 10:06:11.000000 tarkov-changes.py-0.3.0/tvc/armor.py
+-rw-rw-rw-   0        0        0     1404 2022-08-04 10:06:12.000000 tarkov-changes.py-0.3.0/tvc/backpack.py
+-rw-rw-rw-   0        0        0      895 2022-08-02 09:41:31.000000 tarkov-changes.py-0.3.0/tvc/barter.py
+-rw-rw-rw-   0        0        0     6417 2022-08-04 11:21:33.000000 tarkov-changes.py-0.3.0/tvc/client.py
+-rw-rw-rw-   0        0        0     8129 2022-07-27 13:41:49.000000 tarkov-changes.py-0.3.0/tvc/enums.py
+-rw-rw-rw-   0        0        0     1249 2022-07-26 05:36:07.000000 tarkov-changes.py-0.3.0/tvc/exceptions.py
+-rw-rw-rw-   0        0        0     1300 2022-08-04 10:06:10.000000 tarkov-changes.py-0.3.0/tvc/food.py
+-rw-rw-rw-   0        0        0     1538 2022-08-04 10:06:10.000000 tarkov-changes.py-0.3.0/tvc/grenade.py
+-rw-rw-rw-   0        0        0     2198 2022-08-04 10:06:10.000000 tarkov-changes.py-0.3.0/tvc/headphone.py
+-rw-rw-rw-   0        0        0     1123 2022-08-04 10:04:42.000000 tarkov-changes.py-0.3.0/tvc/item.py
+-rw-rw-rw-   0        0        0     1847 2022-08-04 10:04:42.000000 tarkov-changes.py-0.3.0/tvc/key.py
+-rw-rw-rw-   0        0        0     1750 2023-05-25 17:54:53.000000 tarkov-changes.py-0.3.0/tvc/maps.py
+-rw-rw-rw-   0        0        0     1708 2022-08-02 10:37:16.000000 tarkov-changes.py-0.3.0/tvc/mixins.py
+-rw-rw-rw-   0        0        0     5678 2022-08-01 08:39:38.000000 tarkov-changes.py-0.3.0/tvc/requester.py
+drwxrwxrwx   0        0        0        0 2023-05-25 17:58:20.095542 tarkov-changes.py-0.3.0/tvc/types/
+-rw-rw-rw-   0        0        0      156 2022-07-25 20:10:52.000000 tarkov-changes.py-0.3.0/tvc/types/__init__.py
+-rw-rw-rw-   0        0        0      750 2022-07-26 05:11:05.000000 tarkov-changes.py-0.3.0/tvc/types/ammunition.py
+-rw-rw-rw-   0        0        0      591 2022-07-26 05:11:05.000000 tarkov-changes.py-0.3.0/tvc/types/armor.py
+-rw-rw-rw-   0        0        0      338 2022-07-26 05:11:05.000000 tarkov-changes.py-0.3.0/tvc/types/backpack.py
+-rw-rw-rw-   0        0        0      149 2022-08-01 08:39:38.000000 tarkov-changes.py-0.3.0/tvc/types/banned.py
+-rw-rw-rw-   0        0        0      276 2022-07-26 05:11:05.000000 tarkov-changes.py-0.3.0/tvc/types/barter.py
+-rw-rw-rw-   0        0        0      230 2022-07-26 05:11:05.000000 tarkov-changes.py-0.3.0/tvc/types/cell.py
+-rw-rw-rw-   0        0        0      390 2022-08-01 08:33:43.000000 tarkov-changes.py-0.3.0/tvc/types/food.py
+-rw-rw-rw-   0        0        0      514 2022-07-26 05:11:05.000000 tarkov-changes.py-0.3.0/tvc/types/grenade.py
+-rw-rw-rw-   0        0        0      709 2022-07-26 08:40:18.000000 tarkov-changes.py-0.3.0/tvc/types/headphone.py
+-rw-rw-rw-   0        0        0      210 2022-07-25 18:19:21.000000 tarkov-changes.py-0.3.0/tvc/types/item.py
+-rw-rw-rw-   0        0        0      353 2022-07-26 05:11:05.000000 tarkov-changes.py-0.3.0/tvc/types/key.py
+-rw-rw-rw-   0        0        0      482 2023-05-25 17:51:32.000000 tarkov-changes.py-0.3.0/tvc/types/maps.py
+-rw-rw-rw-   0        0        0      361 2022-07-24 11:33:39.000000 tarkov-changes.py-0.3.0/tvc/utils.py
```

### Comparing `tarkov-changes.py-0.2.9/LICENSE` & `tarkov-changes.py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tarkov-changes.py-0.2.9/PKG-INFO` & `tarkov-changes.py-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: tarkov-changes.py
-Version: 0.2.9
+Version: 0.3.0
 Summary: async API wrapper for Tarkov Changes written in Python.
 Home-page: https://github.com/Hostagen/tarkov-changes.py
 Author: Hostagen
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 tarkov-changes.py
 =======================
 
@@ -114,9 +113,7 @@
 Update Logs
 -------------
 `Check Here <https://github.com/Hostagen/tarkov-changes.py/releases>`_
 
 View more examples
 ---------------------------------------------------------
 `Click here! <https://github.com/Hostagen/tarkov-changes.py/tree/master/examples>`_
-
-
```

### Comparing `tarkov-changes.py-0.2.9/README.rst` & `tarkov-changes.py-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `tarkov-changes.py-0.2.9/setup.py` & `tarkov-changes.py-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `tarkov-changes.py-0.2.9/tarkov_changes.py.egg-info/PKG-INFO` & `tarkov-changes.py-0.3.0/tarkov_changes.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: tarkov-changes.py
-Version: 0.2.9
+Version: 0.3.0
 Summary: async API wrapper for Tarkov Changes written in Python.
 Home-page: https://github.com/Hostagen/tarkov-changes.py
 Author: Hostagen
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 tarkov-changes.py
 =======================
 
@@ -114,9 +113,7 @@
 Update Logs
 -------------
 `Check Here <https://github.com/Hostagen/tarkov-changes.py/releases>`_
 
 View more examples
 ---------------------------------------------------------
 `Click here! <https://github.com/Hostagen/tarkov-changes.py/tree/master/examples>`_
-
-
```

### Comparing `tarkov-changes.py-0.2.9/tarkov_changes.py.egg-info/SOURCES.txt` & `tarkov-changes.py-0.3.0/tarkov_changes.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tarkov-changes.py-0.2.9/tvc/ammunition.py` & `tarkov-changes.py-0.3.0/tvc/ammunition.py`

 * *Files identical despite different names*

### Comparing `tarkov-changes.py-0.2.9/tvc/armor.py` & `tarkov-changes.py-0.3.0/tvc/armor.py`

 * *Files identical despite different names*

### Comparing `tarkov-changes.py-0.2.9/tvc/backpack.py` & `tarkov-changes.py-0.3.0/tvc/backpack.py`

 * *Files identical despite different names*

### Comparing `tarkov-changes.py-0.2.9/tvc/barter.py` & `tarkov-changes.py-0.3.0/tvc/barter.py`

 * *Files identical despite different names*

### Comparing `tarkov-changes.py-0.2.9/tvc/client.py` & `tarkov-changes.py-0.3.0/tvc/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         self._armors: Dict[str, Armor] = {}
         self._backpacks: Dict[str, Backpack] = {}
         self._barters: Dict[str, Barter] = {}
         self._foods: Dict[str, Food] = {}
         self._grenades: Dict[str, Grenade] = {}
         self._items: Dict[str, Item] = {}
         self._keys: Dict[str, Key] = {}
+        self._maps: Dict[str, Map] = {}
 
     def start(self) -> None:
         self.loop.run_until_complete(self.load_endpoints())
 
     def get_ammunition(self, name: str) -> Optional[Ammunition]:
         return self._ammunition.get(name)
 
@@ -78,14 +79,15 @@
         ammunition = await self.fetch_ammunition()
         backpacks = await self.fetch_backpack()
         barters = await self.fetch_barter()
         foods = await self.fetch_food()
         grenades = await self.fetch_grenade()
         items = await self.fetch_item()
         keys = await self.fetch_key()
+        maps = await self.fetch_map()
 
         for armor in armors:
             self._armors[armor.name] = armor
 
         for ammo in ammunition:
             self._ammunition[ammo.name] = ammo
 
@@ -103,14 +105,17 @@
 
         for item in items:
             self._items[item.name] = item
 
         for key in keys:
             self._keys[key.name] = key
 
+        for _map in maps:
+            self._maps[_map.name] = _map
+
     async def fetch_ammunition(self, query: str = None) -> List[Ammunition]:
         data = await self.__requester.get_ammunition(query)
         return [Ammunition(d) for d in data]
 
     async def fetch_armor(self, query: str = None) -> List[Armor]:
         data = await self.__requester.get_armor(query)
         return [Armor(d) for d in data]
@@ -184,7 +189,11 @@
     @property
     def items(self) -> List[Item]:
         return list(self._items.values())
 
     @property
     def keys(self) -> List[Key]:
         return list(self._keys.values())
+
+    @property
+    def maps(self) -> List[Map]:
+        return list(self._maps.values())
```

### Comparing `tarkov-changes.py-0.2.9/tvc/enums.py` & `tarkov-changes.py-0.3.0/tvc/enums.py`

 * *Files identical despite different names*

### Comparing `tarkov-changes.py-0.2.9/tvc/exceptions.py` & `tarkov-changes.py-0.3.0/tvc/exceptions.py`

 * *Files identical despite different names*

### Comparing `tarkov-changes.py-0.2.9/tvc/food.py` & `tarkov-changes.py-0.3.0/tvc/food.py`

 * *Files identical despite different names*

### Comparing `tarkov-changes.py-0.2.9/tvc/grenade.py` & `tarkov-changes.py-0.3.0/tvc/grenade.py`

 * *Files identical despite different names*

### Comparing `tarkov-changes.py-0.2.9/tvc/headphone.py` & `tarkov-changes.py-0.3.0/tvc/headphone.py`

 * *Files identical despite different names*

### Comparing `tarkov-changes.py-0.2.9/tvc/item.py` & `tarkov-changes.py-0.3.0/tvc/item.py`

 * *Files identical despite different names*

### Comparing `tarkov-changes.py-0.2.9/tvc/key.py` & `tarkov-changes.py-0.3.0/tvc/key.py`

 * *Files identical despite different names*

### Comparing `tarkov-changes.py-0.2.9/tvc/maps.py` & `tarkov-changes.py-0.3.0/tvc/maps.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,14 +6,28 @@
     from .types.maps import Map as MapPayload
 
 __all__ = ('Map',)
 
 
 class Map:
 
+    __slots__ = (
+        'name',
+        'enabled',
+        'locked',
+        'internal_name',
+        'avg_player_level',
+        'raid_timer',
+        'max_players',
+        'min_players',
+        'required_player_level_min',
+        'required_player_level_max',
+        'min_player_level_access_key',
+    )
+
     def __init__(self, payload: MapPayload) -> None:
         self.name: str = payload['Name']
         self._update(payload)
 
     def __str__(self) -> str:
         return self.name
 
@@ -33,8 +47,10 @@
         self.enabled: bool = data['Map Enabled']
         self.locked: bool = data['Map Locked']
         self.internal_name: str = data['Map Internal Name']
         self.avg_player_level: int = int(data['Avg. Player Level'])
         self.raid_timer: int = data['Raid Timer']
         self.max_players: int = int(data['Max Players'])
         self.min_players: int = int(data['Min Players'])
-        self.required_player_level: int = int(data['Required Player Level'])
+        self.required_player_level_min: int = int(data['Required Player Level Min'])
+        self.required_player_level_max: int = int(data['Required Player Level Max'])
+        self.min_player_level_access_key: float = int(data['Min. Player Level - Access Keys'])
```

### Comparing `tarkov-changes.py-0.2.9/tvc/mixins.py` & `tarkov-changes.py-0.3.0/tvc/mixins.py`

 * *Files identical despite different names*

### Comparing `tarkov-changes.py-0.2.9/tvc/requester.py` & `tarkov-changes.py-0.3.0/tvc/requester.py`

 * *Files identical despite different names*

### Comparing `tarkov-changes.py-0.2.9/tvc/types/ammunition.py` & `tarkov-changes.py-0.3.0/tvc/types/ammunition.py`

 * *Files identical despite different names*

### Comparing `tarkov-changes.py-0.2.9/tvc/types/armor.py` & `tarkov-changes.py-0.3.0/tvc/types/armor.py`

 * *Files identical despite different names*

### Comparing `tarkov-changes.py-0.2.9/tvc/types/grenade.py` & `tarkov-changes.py-0.3.0/tvc/types/grenade.py`

 * *Files identical despite different names*

### Comparing `tarkov-changes.py-0.2.9/tvc/types/headphone.py` & `tarkov-changes.py-0.3.0/tvc/types/headphone.py`

 * *Files identical despite different names*

