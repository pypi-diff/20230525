# Comparing `tmp/dirigera-0.1.7.tar.gz` & `tmp/dirigera-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirigera-0.1.7.tar", last modified: Wed May 24 15:14:53 2023, max compression
+gzip compressed data, was "dirigera-0.1.8.tar", last modified: Thu May 25 18:02:22 2023, max compression
```

## Comparing `dirigera-0.1.7.tar` & `dirigera-0.1.8.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:14:53.422249 dirigera-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-24 15:14:44.000000 dirigera-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-05-24 15:14:53.422249 dirigera-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-05-24 15:14:44.000000 dirigera-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-24 15:14:44.000000 dirigera-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:14:53.422249 dirigera-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:14:44.000000 dirigera-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:14:53.418249 dirigera-0.1.7/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:14:53.418249 dirigera-0.1.7/src/dirigera/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:14:53.422249 dirigera-0.1.7/src/dirigera/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/devices/blinds.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/devices/environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/devices/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/devices/open_close_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/devices/outlet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:14:53.422249 dirigera-0.1.7/src/dirigera/hub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/hub/abstract_smart_home_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-24 15:14:44.000000 dirigera-0.1.7/src/dirigera/hub/hub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:14:53.418249 dirigera-0.1.7/src/dirigera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-05-24 15:14:53.000000 dirigera-0.1.7/src/dirigera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-24 15:14:53.000000 dirigera-0.1.7/src/dirigera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:14:53.000000 dirigera-0.1.7/src/dirigera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 15:14:53.000000 dirigera-0.1.7/src/dirigera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-24 15:14:53.000000 dirigera-0.1.7/src/dirigera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 15:14:53.000000 dirigera-0.1.7/src/dirigera.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:14:53.422249 dirigera-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-24 15:14:44.000000 dirigera-0.1.7/tests/test_blinds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-24 15:14:44.000000 dirigera-0.1.7/tests/test_environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11554 2023-05-24 15:14:44.000000 dirigera-0.1.7/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-24 15:14:44.000000 dirigera-0.1.7/tests/test_open_close_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-24 15:14:44.000000 dirigera-0.1.7/tests/test_outlet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:02:22.677058 dirigera-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-25 18:02:10.000000 dirigera-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-25 18:02:22.677058 dirigera-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-05-25 18:02:10.000000 dirigera-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-25 18:02:10.000000 dirigera-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 18:02:22.677058 dirigera-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 18:02:10.000000 dirigera-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:02:22.673058 dirigera-0.1.8/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:02:22.673058 dirigera-0.1.8/src/dirigera/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:02:22.677058 dirigera-0.1.8/src/dirigera/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/devices/blinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/devices/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/devices/environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/devices/open_close_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/devices/outlet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:02:22.677058 dirigera-0.1.8/src/dirigera/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/hub/abstract_smart_home_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-05-25 18:02:10.000000 dirigera-0.1.8/src/dirigera/hub/hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:02:22.673058 dirigera-0.1.8/src/dirigera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-25 18:02:22.000000 dirigera-0.1.8/src/dirigera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-25 18:02:22.000000 dirigera-0.1.8/src/dirigera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 18:02:22.000000 dirigera-0.1.8/src/dirigera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-25 18:02:22.000000 dirigera-0.1.8/src/dirigera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-25 18:02:22.000000 dirigera-0.1.8/src/dirigera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 18:02:22.000000 dirigera-0.1.8/src/dirigera.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 18:02:22.677058 dirigera-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-25 18:02:10.000000 dirigera-0.1.8/tests/test_blinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-25 18:02:10.000000 dirigera-0.1.8/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-25 18:02:10.000000 dirigera-0.1.8/tests/test_environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11554 2023-05-25 18:02:10.000000 dirigera-0.1.8/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-25 18:02:10.000000 dirigera-0.1.8/tests/test_open_close_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-25 18:02:10.000000 dirigera-0.1.8/tests/test_outlet.py
```

### Comparing `dirigera-0.1.7/LICENSE` & `dirigera-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.7/PKG-INFO` & `dirigera-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 0.1.7
+Version: 0.1.8
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,14 +46,15 @@
 [![Downloads](https://static.pepy.tech/badge/dirigera/month)](https://pepy.tech/project/dirigera)
 ![Downloads](https://img.shields.io/pypi/pyversions/dirigera)
 
 This repository provides an unofficial Python client for controlling the IKEA Dirigera Smart Home Hub. Current features:
  - [light control](#controlling-lights)
  - [outlet control](#controlling-outlets)
  - [blinds control](#controlling-blinds)
+ - [remote controllers](#remote-controllers) (tested with STYRBAR)
  - [environment sensor](#environment-sensor) (tested with VINDSTYRKA)
  - [event listener](#event-listener) for hub events
 
 Support for other features will be added in the future and your input in form of issues and PRs is greatly appreciated.
 
 ## Installation
 
@@ -197,14 +198,42 @@
 
 ```python
 blind.set_name(name="kitchen blind 1")
 
 blind.set_target_level(target_level=90)
 ```
 
+## [Remote Controllers](./src/dirigera/devices/controller.py)
+
+Currently only tested with the STYRBAR remote.
+
+To get information about the available controllers, you can use the `get_controllers()` method:
+
+```python
+controllers = dirigera_hub.get_controllers()
+```
+
+The controller object has the following attributes:
+
+```python
+device_id: str
+is_reachable: bool
+custom_name: str
+is_on: bool
+battery_percentage: int
+room_id: str
+room_name: str
+can_receive: List[str]  # list of all available commands ["customName"]
+```
+
+Available methods for controller are:
+
+```python
+controller.set_name(name="kitchen remote 1")
+```
 
 ## [Environment Sensor](./src/dirigera/devices/environment_sensor.py)
 Currently only tested with the VINDSTYRKA sensor. If you have other sensors please send me the json and I will add support or create a PR.
 
 
 To get the environment sensors use:
 ```python
```

### Comparing `dirigera-0.1.7/README.md` & `dirigera-0.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 [![Downloads](https://static.pepy.tech/badge/dirigera/month)](https://pepy.tech/project/dirigera)
 ![Downloads](https://img.shields.io/pypi/pyversions/dirigera)
 
 This repository provides an unofficial Python client for controlling the IKEA Dirigera Smart Home Hub. Current features:
  - [light control](#controlling-lights)
  - [outlet control](#controlling-outlets)
  - [blinds control](#controlling-blinds)
+ - [remote controllers](#remote-controllers) (tested with STYRBAR)
  - [environment sensor](#environment-sensor) (tested with VINDSTYRKA)
  - [event listener](#event-listener) for hub events
 
 Support for other features will be added in the future and your input in form of issues and PRs is greatly appreciated.
 
 ## Installation
 
@@ -155,14 +156,42 @@
 
 ```python
 blind.set_name(name="kitchen blind 1")
 
 blind.set_target_level(target_level=90)
 ```
 
+## [Remote Controllers](./src/dirigera/devices/controller.py)
+
+Currently only tested with the STYRBAR remote.
+
+To get information about the available controllers, you can use the `get_controllers()` method:
+
+```python
+controllers = dirigera_hub.get_controllers()
+```
+
+The controller object has the following attributes:
+
+```python
+device_id: str
+is_reachable: bool
+custom_name: str
+is_on: bool
+battery_percentage: int
+room_id: str
+room_name: str
+can_receive: List[str]  # list of all available commands ["customName"]
+```
+
+Available methods for controller are:
+
+```python
+controller.set_name(name="kitchen remote 1")
+```
 
 ## [Environment Sensor](./src/dirigera/devices/environment_sensor.py)
 Currently only tested with the VINDSTYRKA sensor. If you have other sensors please send me the json and I will add support or create a PR.
 
 
 To get the environment sensors use:
 ```python
```

### Comparing `dirigera-0.1.7/pyproject.toml` & `dirigera-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
    "setuptools",
    "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dirigera"
-version = "0.1.7"
+version = "0.1.8"
 description = "An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub"
 readme = "README.md"
 authors = [{ name = "Leggin", email = "legginsun@gmail.com" }]
 license = { file = "LICENSE" }
 keywords = ["python", "iot", "smarthome", "hub", "lighting", "ikea", "tradfri", "dirigera"]
 dependencies = [
     "requests >= 2.22.0",
```

### Comparing `dirigera-0.1.7/src/dirigera/devices/blinds.py` & `dirigera-0.1.8/src/dirigera/devices/blinds.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.7/src/dirigera/devices/device.py` & `dirigera-0.1.8/src/dirigera/devices/device.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.7/src/dirigera/devices/environment_sensor.py` & `dirigera-0.1.8/src/dirigera/devices/environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.7/src/dirigera/devices/light.py` & `dirigera-0.1.8/src/dirigera/devices/light.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.7/src/dirigera/devices/open_close_sensor.py` & `dirigera-0.1.8/src/dirigera/devices/open_close_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.7/src/dirigera/devices/outlet.py` & `dirigera-0.1.8/src/dirigera/devices/outlet.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.7/src/dirigera/hub/abstract_smart_home_hub.py` & `dirigera-0.1.8/src/dirigera/hub/abstract_smart_home_hub.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.7/src/dirigera/hub/auth.py` & `dirigera-0.1.8/src/dirigera/hub/auth.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.7/src/dirigera/hub/hub.py` & `dirigera-0.1.8/src/dirigera/hub/hub.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import requests
 import websocket
 from urllib3.exceptions import InsecureRequestWarning
 
 from .abstract_smart_home_hub import AbstractSmartHomeHub
 from ..devices.light import Light, dict_to_light
 from ..devices.blinds import Blind, dict_to_blind
+from ..devices.controller import Controller, dict_to_controller
 from ..devices.outlet import Outlet, dict_to_outlet
 from ..devices.environment_sensor import EnvironmentSensor, dict_to_environment_sensor
 from ..devices.open_close_sensor import OpenCloseSensor, dict_to_open_close_sensor
 
 requests.packages.urllib3.disable_warnings(  # pylint: disable=no-member
     category=InsecureRequestWarning
 )
@@ -146,7 +147,31 @@
         Fetches all blinds and returns first result that matches this name
         """
         blinds = self.get_blinds()
         blinds = list(filter(lambda x: x.custom_name == blind_name, blinds))
         if len(blinds) == 0:
             raise AssertionError(f"No blind found with name {blind_name}")
         return blinds[0]
+
+    def get_controllers(self) -> List[Controller]:
+        """
+        Fetches all controllers registered in the Hub
+        """
+        devices = self.get("/devices")
+        controllers = list(
+            filter(lambda x: x["type"] == "controller", devices)
+        )
+        return [
+            dict_to_controller(controller, self) for controller in controllers
+        ]
+
+    def get_controller_by_name(self, controller_name: str) -> Controller:
+        """
+        Fetches all controllers and returns first result that matches this name
+        """
+        controllers = self.get_controllers()
+        controllers = list(
+            filter(lambda x: x.custom_name == controller_name, controllers)
+        )
+        if len(controllers) == 0:
+            raise AssertionError(f"No controller found with name {controller_name}")
+        return controllers[0]
```

### Comparing `dirigera-0.1.7/src/dirigera.egg-info/PKG-INFO` & `dirigera-0.1.8/src/dirigera.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 0.1.7
+Version: 0.1.8
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,14 +46,15 @@
 [![Downloads](https://static.pepy.tech/badge/dirigera/month)](https://pepy.tech/project/dirigera)
 ![Downloads](https://img.shields.io/pypi/pyversions/dirigera)
 
 This repository provides an unofficial Python client for controlling the IKEA Dirigera Smart Home Hub. Current features:
  - [light control](#controlling-lights)
  - [outlet control](#controlling-outlets)
  - [blinds control](#controlling-blinds)
+ - [remote controllers](#remote-controllers) (tested with STYRBAR)
  - [environment sensor](#environment-sensor) (tested with VINDSTYRKA)
  - [event listener](#event-listener) for hub events
 
 Support for other features will be added in the future and your input in form of issues and PRs is greatly appreciated.
 
 ## Installation
 
@@ -197,14 +198,42 @@
 
 ```python
 blind.set_name(name="kitchen blind 1")
 
 blind.set_target_level(target_level=90)
 ```
 
+## [Remote Controllers](./src/dirigera/devices/controller.py)
+
+Currently only tested with the STYRBAR remote.
+
+To get information about the available controllers, you can use the `get_controllers()` method:
+
+```python
+controllers = dirigera_hub.get_controllers()
+```
+
+The controller object has the following attributes:
+
+```python
+device_id: str
+is_reachable: bool
+custom_name: str
+is_on: bool
+battery_percentage: int
+room_id: str
+room_name: str
+can_receive: List[str]  # list of all available commands ["customName"]
+```
+
+Available methods for controller are:
+
+```python
+controller.set_name(name="kitchen remote 1")
+```
 
 ## [Environment Sensor](./src/dirigera/devices/environment_sensor.py)
 Currently only tested with the VINDSTYRKA sensor. If you have other sensors please send me the json and I will add support or create a PR.
 
 
 To get the environment sensors use:
 ```python
```

### Comparing `dirigera-0.1.7/src/dirigera.egg-info/SOURCES.txt` & `dirigera-0.1.8/src/dirigera.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 src/dirigera.egg-info/SOURCES.txt
 src/dirigera.egg-info/dependency_links.txt
 src/dirigera.egg-info/entry_points.txt
 src/dirigera.egg-info/requires.txt
 src/dirigera.egg-info/top_level.txt
 src/dirigera/devices/__init__.py
 src/dirigera/devices/blinds.py
+src/dirigera/devices/controller.py
 src/dirigera/devices/device.py
 src/dirigera/devices/environment_sensor.py
 src/dirigera/devices/light.py
 src/dirigera/devices/open_close_sensor.py
 src/dirigera/devices/outlet.py
 src/dirigera/hub/__init__.py
 src/dirigera/hub/abstract_smart_home_hub.py
 src/dirigera/hub/auth.py
 src/dirigera/hub/hub.py
 tests/test_blinds.py
+tests/test_controller.py
 tests/test_environment_sensor.py
 tests/test_light.py
 tests/test_open_close_sensor.py
 tests/test_outlet.py
```

### Comparing `dirigera-0.1.7/tests/test_blinds.py` & `dirigera-0.1.8/tests/test_blinds.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.7/tests/test_environment_sensor.py` & `dirigera-0.1.8/tests/test_environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.7/tests/test_light.py` & `dirigera-0.1.8/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.7/tests/test_open_close_sensor.py` & `dirigera-0.1.8/tests/test_open_close_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-0.1.7/tests/test_outlet.py` & `dirigera-0.1.8/tests/test_outlet.py`

 * *Files identical despite different names*

