# Comparing `tmp/wrighter-0.1.1.tar.gz` & `tmp/wrighter-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrighter-0.1.1.tar", last modified: Fri Jan 13 20:20:05 2023, max compression
+gzip compressed data, was "wrighter-0.1.2.tar", last modified: Thu May 25 11:43:55 2023, max compression
```

## Comparing `wrighter-0.1.1.tar` & `wrighter-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 20:20:05.788581 wrighter-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-13 20:19:57.000000 wrighter-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-01-13 20:20:05.788581 wrighter-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-01-13 20:19:57.000000 wrighter-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-13 20:20:05.788581 wrighter-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-01-13 20:19:57.000000 wrighter-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 20:20:05.784580 wrighter-0.1.1/wrighter/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-01-13 20:19:57.000000 wrighter-0.1.1/wrighter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-01-13 20:19:57.000000 wrighter-0.1.1/wrighter/async_wrighter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-01-13 20:19:57.000000 wrighter-0.1.1/wrighter/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-01-13 20:19:57.000000 wrighter-0.1.1/wrighter/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7340 2023-01-13 20:19:57.000000 wrighter-0.1.1/wrighter/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-01-13 20:19:57.000000 wrighter-0.1.1/wrighter/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 20:20:05.788581 wrighter-0.1.1/wrighter/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-01-13 20:19:57.000000 wrighter-0.1.1/wrighter/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-01-13 20:19:57.000000 wrighter-0.1.1/wrighter/plugins/async_stealth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-01-13 20:19:57.000000 wrighter-0.1.1/wrighter/plugins/network_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-01-13 20:19:57.000000 wrighter-0.1.1/wrighter/plugins/page_timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-01-13 20:19:57.000000 wrighter-0.1.1/wrighter/plugins/resource_blocker.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-01-13 20:19:57.000000 wrighter-0.1.1/wrighter/plugins/sync_stealth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-01-13 20:19:57.000000 wrighter-0.1.1/wrighter/sync_wrighter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 20:20:05.784580 wrighter-0.1.1/wrighter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-01-13 20:20:05.000000 wrighter-0.1.1/wrighter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-01-13 20:20:05.000000 wrighter-0.1.1/wrighter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 20:20:05.000000 wrighter-0.1.1/wrighter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-13 20:20:05.000000 wrighter-0.1.1/wrighter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-13 20:20:05.000000 wrighter-0.1.1/wrighter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:43:55.626137 wrighter-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-25 11:43:44.000000 wrighter-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-25 11:43:55.626137 wrighter-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-25 11:43:44.000000 wrighter-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-25 11:43:44.000000 wrighter-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:43:55.626137 wrighter-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:43:44.000000 wrighter-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:43:55.626137 wrighter-0.1.2/wrighter/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-25 11:43:44.000000 wrighter-0.1.2/wrighter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-05-25 11:43:44.000000 wrighter-0.1.2/wrighter/async_wrighter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-25 11:43:44.000000 wrighter-0.1.2/wrighter/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-05-25 11:43:44.000000 wrighter-0.1.2/wrighter/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-25 11:43:44.000000 wrighter-0.1.2/wrighter/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-25 11:43:44.000000 wrighter-0.1.2/wrighter/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-25 11:43:44.000000 wrighter-0.1.2/wrighter/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-25 11:43:44.000000 wrighter-0.1.2/wrighter/sync_wrighter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:43:55.626137 wrighter-0.1.2/wrighter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-25 11:43:55.000000 wrighter-0.1.2/wrighter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-25 11:43:55.000000 wrighter-0.1.2/wrighter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:43:55.000000 wrighter-0.1.2/wrighter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-25 11:43:55.000000 wrighter-0.1.2/wrighter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 11:43:55.000000 wrighter-0.1.2/wrighter.egg-info/top_level.txt
```

### Comparing `wrighter-0.1.1/LICENSE` & `wrighter-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wrighter-0.1.1/wrighter/async_wrighter.py` & `wrighter-0.1.2/wrighter/async_wrighter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import asyncio
 import random
 from pathlib import Path
 from typing import Any, Mapping
 
-from loguru import logger as log
 from playwright.async_api import (
     Browser,
     BrowserContext,
     BrowserType,
     Page,
     Playwright,
     Route,
@@ -52,20 +51,19 @@
 
         Returns:
             The launched browser or browser context.
         """
         driver = self._get_driver(self.options.browser)
         if self.is_persistent:
             opts = self.options.persistent_context_options
-            browser_context = await driver.launch_persistent_context(**opts)
-            browser_context.on("page", lambda page: self._page_add_plugins(page))
-            for plugin in self._plugins:
-                plugin.add_to_context(browser_context)
+            browser_context = await driver.launch_persistent_context(**opts)  # type:ignore
+            browser_context.on("page", lambda page: self.plugin_manager.page_apply_plugins(page))
+            self.plugin_manager.context_apply_plugins(browser_context)
             return browser_context
-        return await driver.launch(**self.options.browser_launch_options)
+        return await driver.launch(**self.options.browser_launch_options)  # type:ignore
 
     async def __launch_context(self) -> BrowserContext:
         if self.is_persistent:
             return self.browser  # type: ignore
         return await self.new_context()
 
     async def new_context(self):
@@ -76,29 +74,28 @@
             RuntimeError: if you try to launch a new context in peristent mode. (if 'user_data_dir' is set)
         Returns:
             BrowserContext
         """
         if self.is_persistent:
             raise RuntimeError("Cannot create contexts in persistent mode.")
         context = await self.browser.new_context(**self.options.context_options)  # type:ignore
-        context.on("page", lambda page: self._page_add_plugins(page))
-        for plugin in self._plugins:
-            plugin.add_to_context(context)
+        context.on("page", lambda page: self.plugin_manager.page_apply_plugins(page))
+        self.plugin_manager.context_apply_plugins(context)
         return context
 
     async def stop(self):
-        log.info("Stopping Playwright")
+        self.logger.debug("Stopping Playwright")
         await self.context.close()
         await self.browser.close()  # type: ignore
         await self.playwright.stop()  # type: ignore
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         try:
             await self.stop()
-        except Exception as e:
+        except Exception:
             pass
 
     async def sleep(self, lo: float, hi: float | None = None) -> float:
         """
         Sleeps for a random duration within a specified range.
 
         Args:
@@ -110,18 +107,18 @@
 
         Raises:
             ValueError: If `hi` is provided and `lo` is greater than `hi`.
         """
 
         if hi is None:
             await asyncio.sleep(lo)
-            self.log.info(f"Sleeping for {round(lo,2)}s")
+            self.logger.info(f"Sleeping for {round(lo,2)}s")
             return lo
         if lo > hi:
             raise ValueError(f"Minimum sleep time is higher that maximum. {(lo,hi)}")
         t = random.uniform(lo, hi)
-        self.log.info(f"Sleeping for {round(t,2)}s")
+        self.logger.info(f"Sleeping for {round(t,2)}s")
         await asyncio.sleep(t)
         return t
 
 
 __all__ = ["AsyncWrighter"]
```

### Comparing `wrighter-0.1.1/wrighter/constants.py` & `wrighter-0.1.2/wrighter/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     "fetch",
     "eventsource",
     "websocket",
     "manifest",
     "other",
 ]
 
-BROWSER_LAUNCH_KEYS = [
+BROWSER_LAUNCH_OPTS_NAMES = [
     "executable_path",
     "channel",
     "args",
     "ignore_default_args",
     "handle_sigint",
     "handle_sigterm",
     "handle_sighup",
@@ -59,15 +59,15 @@
     "downloads_path",
     "slow_mo",
     "traces_dir",
     "chromium_sandbox",
     "firefox_user_prefs",
 ]
 
-CONTEXT_KEYS = [
+CONTEXT_OPTS_NAMES = [
     "viewport",
     "screen",
     "no_viewport",
     "ignore_https_errors",
     "java_script_enabled",
     "bypass_csp",
     "user_agent",
```

### Comparing `wrighter-0.1.1/wrighter/options.py` & `wrighter-0.1.2/wrighter/options.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     StorageState,
     ViewportSize,
 )
 from pydantic import BaseModel, validator
 from stdl import fs
 from stdl.str_u import FG, colored
 
-from wrighter.constants import *
+from wrighter.constants import BROWSER_LAUNCH_OPTS_NAMES, BROWSERS, CONTEXT_OPTS_NAMES, PERMISSIONS
 
 
 class BaseOptions(BaseModel):
     class Config:
         validate_assignment = True
         arbitrary_types_allowed = True
 
@@ -43,15 +43,14 @@
         print(colored(self.__class__.__name__, color=FG.LIGHT_BLUE) + ":")
         for k, v in self.dict(exclude_none=not full).items():
             k = k.replace("_", " ").capitalize()
             print(f"\t{k}: {v}")
 
 
 class WrighterOptions(BaseOptions):
-
     data_dir: str | Path = os.path.abspath(os.getcwd())
     browser: str = "chromium"
     user_data_dir: str | Path | None = None
     force_user_agent: bool = True
     # Browser launch options
     executable_path: str | Path | None = None
     channel: str | None = None
@@ -108,34 +107,36 @@
     @property
     def browser_launch_options(self) -> dict[str, Any]:
         """
         Returns the options for launching a browser.
         These options are documented at:
         https://playwright.dev/python/docs/api/class-browsertype#browser-type-launch
         """
-        return {k: v for k, v in self.dict().items() if k in BROWSER_LAUNCH_KEYS}
+        return {k: v for k, v in self.dict().items() if k in BROWSER_LAUNCH_OPTS_NAMES}
 
     @property
     def context_options(self) -> dict[str, Any]:
         """
         Returns the options for launching a context.
         These options are documented at:
         https://playwright.dev/python/docs/api/class-browser#browser-new-context
         """
-        return {k: v for k, v in self.dict().items() if k in CONTEXT_KEYS}
+        return {k: v for k, v in self.dict().items() if k in CONTEXT_OPTS_NAMES}
 
     @property
     def persistent_context_options(self) -> dict[str, Any]:
         """
         Returns the options for launching a persistent context.
         These options are documented at:
         https://playwright.dev/python/docs/api/class-browsertype#browser-type-launch-persistent-context
         """
         opts = {
-            k: v for k, v in self.dict().items() if k in BROWSER_LAUNCH_KEYS or k in CONTEXT_KEYS
+            k: v
+            for k, v in self.dict().items()
+            if k in BROWSER_LAUNCH_OPTS_NAMES or k in CONTEXT_OPTS_NAMES
         }
         if "storage_state" in opts.keys():
             log.warning(
                 "'storage_state' is ignored when launching a browser with a persitent context",
                 storage_state=opts["storage_state"],
             )
             del opts["storage_state"]
```

### Comparing `wrighter-0.1.1/wrighter/sync_wrighter.py` & `wrighter-0.1.2/wrighter/sync_wrighter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# noqa: F401
 import random
 import time
 from pathlib import Path
 from typing import Any, Mapping
 
 from playwright.sync_api import (
     Browser,
@@ -32,19 +33,19 @@
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         try:
             self.stop()
-        except Exception as e:
+        except Exception:
             pass
 
     def __start_playwright(self) -> Playwright:
-        self.log.info("Starting Playwright")
+        self.logger.debug("Starting Playwright")
         return sync_playwright().start()
 
     def _launch_browser(self) -> Browser | BrowserContext:
         """
         Launches a browser or persistent browser context.
         If the Wrighter instance is persistent (if 'user_data_dir' is set),
         this method launches and returns a persistent browser context.
@@ -53,27 +54,26 @@
         Returns:
             The launched browser or browser context.
         """
         driver = self._get_driver(self.options.browser)
         if self.is_persistent:
             opts = self.options.persistent_context_options
             browser_context = driver.launch_persistent_context(**opts)
-            browser_context.on("page", lambda page: self._page_add_plugins(page))
-            for plugin in self._plugins:
-                plugin.add_to_context(browser_context)
+            browser_context.on("page", lambda page: self.plugin_manager.page_apply_plugins(page))
+            self.plugin_manager.context_apply_plugins(browser_context)
             return browser_context
         return driver.launch(**self.options.browser_launch_options)
 
     def __launch_context(self) -> BrowserContext:
         if self.is_persistent:
             return self.browser  # type: ignore
         return self.new_context()
 
     def stop(self) -> None:
-        self.log.info("Stopping Playwright")
+        self.logger.debug("Stopping Playwright")
         self.context.close()
         self.browser.close()
         self.playwright.stop()
 
     def new_context(self) -> BrowserContext:
         """
         Launches a new context that will apply all configured events to pages opened with it.
@@ -82,17 +82,16 @@
             RuntimeError: if you try to launch a new context in peristent mode. (if 'user_data_dir' is set)
         Returns:
             BrowserContext
         """
         if self.is_persistent:
             raise RuntimeError("Cannot create contexts in persistent mode.")
         context = self.browser.new_context(**self.options.context_options)  # type:ignore
-        context.on("page", lambda page: self._page_add_plugins(page))
-        for plugin in self._plugins:
-            plugin.add_to_context(context)
+        context.on("page", lambda page: self.plugin_manager.page_apply_plugins(page))
+        self.plugin_manager.context_apply_plugins(context)
         return context
 
     def sleep(self, lo: float, hi: float | None = None) -> float:
         """
         Sleeps for a random duration within a specified range.
 
         Args:
@@ -104,18 +103,18 @@
 
         Raises:
             ValueError: If `hi` is provided and `lo` is greater than `hi`.
         """
 
         if hi is None:
             time.sleep(lo)
-            self.log.info(f"Sleeping for {round(lo,2)}s")
+            self.logger.info(f"Sleeping for {round(lo,2)}s")
             return lo
         if lo > hi:
             raise ValueError(f"Minimum sleep time is higher that maximum. {(lo,hi)}")
         t = random.uniform(lo, hi)
-        self.log.info(f"Sleeping for {round(t,2)}s")
+        self.logger.info(f"Sleeping for {round(t,2)}s")
         time.sleep(t)
         return t
 
 
 __all__ = ["SyncWrighter"]
```

