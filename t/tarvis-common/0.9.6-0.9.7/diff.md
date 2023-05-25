# Comparing `tmp/tarvis-common-0.9.6.tar.gz` & `tmp/tarvis-common-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarvis-common-0.9.6.tar", last modified: Sun May 14 07:27:57 2023, max compression
+gzip compressed data, was "tarvis-common-0.9.7.tar", last modified: Thu May 25 11:13:13 2023, max compression
```

## Comparing `tarvis-common-0.9.6.tar` & `tarvis-common-0.9.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.307687 tarvis-common-0.9.6/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      378 2023-05-14 07:27:57.307687 tarvis-common-0.9.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 07:27:57.307687 tarvis-common-0.9.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      751 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.299687 tarvis-common-0.9.6/tarvis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.299687 tarvis-common-0.9.6/tarvis/common/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.303687 tarvis-common-0.9.6/tarvis/common/asyncio/
--rw-r--r--   0 root         (0) root         (0)      816 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/tarvis/common/asyncio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.299687 tarvis-common-0.9.6/tarvis/common/cache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.303687 tarvis-common-0.9.6/tarvis/common/cache/local/
--rw-r--r--   0 root         (0) root         (0)     3885 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/tarvis/common/cache/local/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.303687 tarvis-common-0.9.6/tarvis/common/config/
--rw-r--r--   0 root         (0) root         (0)     1698 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/tarvis/common/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.303687 tarvis-common-0.9.6/tarvis/common/environ/
--rw-r--r--   0 root         (0) root         (0)     1987 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/tarvis/common/environ/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.303687 tarvis-common-0.9.6/tarvis/common/logging/
--rw-r--r--   0 root         (0) root         (0)     5793 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/tarvis/common/logging/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.303687 tarvis-common-0.9.6/tarvis/common/monitoring/
--rw-r--r--   0 root         (0) root         (0)     3678 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/tarvis/common/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.303687 tarvis-common-0.9.6/tarvis/common/secrets/
--rw-r--r--   0 root         (0) root         (0)     2551 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/tarvis/common/secrets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.303687 tarvis-common-0.9.6/tarvis/common/time/
--rw-r--r--   0 root         (0) root         (0)     6436 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/tarvis/common/time/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.303687 tarvis-common-0.9.6/tarvis/common/trading/
--rw-r--r--   0 root         (0) root         (0)     8778 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/tarvis/common/trading/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.303687 tarvis-common-0.9.6/tarvis_common.egg-info/
--rw-r--r--   0 root         (0) root         (0)      378 2023-05-14 07:27:57.000000 tarvis-common-0.9.6/tarvis_common.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      564 2023-05-14 07:27:57.000000 tarvis-common-0.9.6/tarvis_common.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 07:27:57.000000 tarvis-common-0.9.6/tarvis_common.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      208 2023-05-14 07:27:57.000000 tarvis-common-0.9.6/tarvis_common.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-14 07:27:57.000000 tarvis-common-0.9.6/tarvis_common.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 07:27:57.307687 tarvis-common-0.9.6/test/
--rw-r--r--   0 root         (0) root         (0)      297 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/test/test_config.py
--rw-r--r--   0 root         (0) root         (0)      191 2023-05-14 07:27:44.000000 tarvis-common-0.9.6/test/test_secrets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 11:13:13.297001 tarvis-common-0.9.7/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-05-25 11:13:02.000000 tarvis-common-0.9.7/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      378 2023-05-25 11:13:13.297001 tarvis-common-0.9.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-25 11:13:02.000000 tarvis-common-0.9.7/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 11:13:13.297001 tarvis-common-0.9.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      751 2023-05-25 11:13:02.000000 tarvis-common-0.9.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 11:13:13.293001 tarvis-common-0.9.7/tarvis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 11:13:13.293001 tarvis-common-0.9.7/tarvis/common/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 11:13:13.293001 tarvis-common-0.9.7/tarvis/common/asyncio/
+-rw-r--r--   0 root         (0) root         (0)      816 2023-05-25 11:13:02.000000 tarvis-common-0.9.7/tarvis/common/asyncio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 11:13:13.293001 tarvis-common-0.9.7/tarvis/common/cache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 11:13:13.293001 tarvis-common-0.9.7/tarvis/common/cache/local/
+-rw-r--r--   0 root         (0) root         (0)     3885 2023-05-25 11:13:02.000000 tarvis-common-0.9.7/tarvis/common/cache/local/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 11:13:13.297001 tarvis-common-0.9.7/tarvis/common/config/
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-05-25 11:13:02.000000 tarvis-common-0.9.7/tarvis/common/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 11:13:13.297001 tarvis-common-0.9.7/tarvis/common/environ/
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-05-25 11:13:02.000000 tarvis-common-0.9.7/tarvis/common/environ/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 11:13:13.297001 tarvis-common-0.9.7/tarvis/common/logging/
+-rw-r--r--   0 root         (0) root         (0)     5793 2023-05-25 11:13:02.000000 tarvis-common-0.9.7/tarvis/common/logging/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 11:13:13.297001 tarvis-common-0.9.7/tarvis/common/monitoring/
+-rw-r--r--   0 root         (0) root         (0)     4398 2023-05-25 11:13:02.000000 tarvis-common-0.9.7/tarvis/common/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 11:13:13.297001 tarvis-common-0.9.7/tarvis/common/secrets/
+-rw-r--r--   0 root         (0) root         (0)     2551 2023-05-25 11:13:02.000000 tarvis-common-0.9.7/tarvis/common/secrets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 11:13:13.297001 tarvis-common-0.9.7/tarvis/common/time/
+-rw-r--r--   0 root         (0) root         (0)     6436 2023-05-25 11:13:02.000000 tarvis-common-0.9.7/tarvis/common/time/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 11:13:13.297001 tarvis-common-0.9.7/tarvis/common/trading/
+-rw-r--r--   0 root         (0) root         (0)     8864 2023-05-25 11:13:02.000000 tarvis-common-0.9.7/tarvis/common/trading/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 11:13:13.297001 tarvis-common-0.9.7/tarvis_common.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      378 2023-05-25 11:13:13.000000 tarvis-common-0.9.7/tarvis_common.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      564 2023-05-25 11:13:13.000000 tarvis-common-0.9.7/tarvis_common.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 11:13:13.000000 tarvis-common-0.9.7/tarvis_common.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      208 2023-05-25 11:13:13.000000 tarvis-common-0.9.7/tarvis_common.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-25 11:13:13.000000 tarvis-common-0.9.7/tarvis_common.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 11:13:13.297001 tarvis-common-0.9.7/test/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-05-25 11:13:02.000000 tarvis-common-0.9.7/test/test_config.py
+-rw-r--r--   0 root         (0) root         (0)      191 2023-05-25 11:13:02.000000 tarvis-common-0.9.7/test/test_secrets.py
```

### Comparing `tarvis-common-0.9.6/LICENSE.txt` & `tarvis-common-0.9.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.6/setup.py` & `tarvis-common-0.9.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = requirements_file.read().splitlines()
 
 with open("README.md") as description_file:
     long_description = description_file.read()
 
 setup(
     name="tarvis-common",
-    version="0.9.6",
+    version="0.9.7",
     author="Tarvis Labs",
     author_email="python@tarvislabs.com",
     url="https://tarvislabs.com/",
     description="Tarvis Common Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `tarvis-common-0.9.6/tarvis/common/asyncio/__init__.py` & `tarvis-common-0.9.7/tarvis/common/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.6/tarvis/common/cache/local/__init__.py` & `tarvis-common-0.9.7/tarvis/common/cache/local/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.6/tarvis/common/config/__init__.py` & `tarvis-common-0.9.7/tarvis/common/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.6/tarvis/common/environ/__init__.py` & `tarvis-common-0.9.7/tarvis/common/environ/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.6/tarvis/common/logging/__init__.py` & `tarvis-common-0.9.7/tarvis/common/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.6/tarvis/common/monitoring/__init__.py` & `tarvis-common-0.9.7/tarvis/common/monitoring/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -47,31 +47,39 @@
             extra={"timeout": self._timeout, **self._extra},
         )
 
 
 class Watchdog:
 
     _POLL_INTERVAL = 0.1
+    _EXIT_CODE = 1
 
     @inject
     def __init__(self, config: dict = Provide["config"]):
         self._running = False
         self._timers = []
         self._lock = Lock()
+
+        self._enabled = True
+        self._poll_interval = self._POLL_INTERVAL
+        self._liveness_file_name = ""
+        self._emergency_stop = True
+
         watchdog_config = config.get("watchdog")
-        if watchdog_config is None:
-            self._enabled = True
-            self._poll_interval = self._POLL_INTERVAL
-            self._liveness_file_name = ""
-        else:
-            self._enabled = watchdog_config.get("enabled", True)
+        if watchdog_config is not None:
+            self._enabled = watchdog_config.get("enabled", self._enabled)
             self._poll_interval = watchdog_config.get(
-                "poll_interval", self._POLL_INTERVAL
+                "poll_interval", self._poll_interval
+            )
+            self._liveness_file_name = watchdog_config.get(
+                "liveness_file_name", self._liveness_file_name
+            )
+            self._emergency_stop = watchdog_config.get(
+                "emergency_stop", self._emergency_stop
             )
-            self._liveness_file_name = watchdog_config.get("liveness_file_name", "")
 
     def add_timer(self, timer: WatchdogTimer):
         with self._lock:
             timer._parent = self
             self._timers.append(timer)
             if self._enabled and (not self._running):
                 new_thread = Thread(target=self._run)
@@ -96,14 +104,21 @@
                         all_alive = True
                         for timer in self._timers:
                             # noinspection PyProtectedMember
                             timer._tick(now)
                             all_alive &= not timer.alarmed
                         if all_alive:
                             self._add_liveness_indicator()
+                        elif self._emergency_stop:
+                            # Do not attempt to do anything except die. A problem
+                            # relating to logging or cleanup may be the source of the
+                            # problem, so attempting to do any of those things may
+                            # prevent the emergency stop.
+                            # noinspection PyUnresolvedReferences, PyProtectedMember
+                            os._exit(self._EXIT_CODE)
                     else:
                         self._running = False
                         break
                 native_time.sleep(self._poll_interval)
         except Exception as watchdog_exception:
             logging.critical(
                 f"Unhandled exception: {watchdog_exception}", exc_info=True
```

### Comparing `tarvis-common-0.9.6/tarvis/common/secrets/__init__.py` & `tarvis-common-0.9.7/tarvis/common/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.6/tarvis/common/time/__init__.py` & `tarvis-common-0.9.7/tarvis/common/time/__init__.py`

 * *Files identical despite different names*

### Comparing `tarvis-common-0.9.6/tarvis/common/trading/__init__.py` & `tarvis-common-0.9.7/tarvis/common/trading/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,25 +26,27 @@
 class BasicTradingIndicator:
     def __init__(
         self,
         time: float,
         direction: MarketPosition,
         price: float = None,
         leverage: float = 1,
+        averaging_factor: float = 1,
         take_profit: float = 0,
         meta_data: dict = None,
     ):
         if leverage <= 0:
             raise ValueError("leverage must be greater than 0.")
         if (take_profit < 0) or (take_profit > 1):
             raise ValueError("take_profit must be between 0 and 1 inclusive.")
         self.time = time
         self.direction = direction
         self.price = price
         self.leverage = leverage
+        self.averaging_factor = averaging_factor
         self.take_profit = take_profit
         self.meta_data = meta_data
 
     def __eq__(self, other):
         if other is self:
             return True
         if isinstance(other, BasicTradingIndicator):
```

### Comparing `tarvis-common-0.9.6/tarvis_common.egg-info/SOURCES.txt` & `tarvis-common-0.9.7/tarvis_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

