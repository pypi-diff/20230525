# Comparing `tmp/discord_status_updater-0.1.0.tar.gz` & `tmp/discord_status_updater-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord_status_updater-0.1.0.tar", last modified: Tue May 23 18:31:44 2023, max compression
+gzip compressed data, was "discord_status_updater-0.2.0.tar", last modified: Thu May 25 13:48:44 2023, max compression
```

## Comparing `discord_status_updater-0.1.0.tar` & `discord_status_updater-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-05-23 18:31:44.976442 discord_status_updater-0.1.0/
--rw-r--r--   0 nick      (1000) nick      (1000)     1070 2023-05-23 01:29:45.000000 discord_status_updater-0.1.0/LICENSE.txt
--rw-r--r--   0 nick      (1000) nick      (1000)     3368 2023-05-23 18:31:44.976442 discord_status_updater-0.1.0/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)     2727 2023-05-23 17:10:09.000000 discord_status_updater-0.1.0/README.md
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-05-23 18:31:44.976442 discord_status_updater-0.1.0/discord_status_updater/
--rw-r--r--   0 nick      (1000) nick      (1000)       22 2023-05-23 08:08:11.000000 discord_status_updater-0.1.0/discord_status_updater/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)       57 2023-05-23 09:19:56.000000 discord_status_updater-0.1.0/discord_status_updater/__main__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1528 2023-05-23 00:26:09.000000 discord_status_updater-0.1.0/discord_status_updater/discord_client.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1320 2023-05-23 08:18:08.000000 discord_status_updater-0.1.0/discord_status_updater/discord_status_updater.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1193 2023-05-23 18:14:03.000000 discord_status_updater-0.1.0/discord_status_updater/launcher.py
--rw-r--r--   0 nick      (1000) nick      (1000)      186 2023-05-23 08:54:33.000000 discord_status_updater-0.1.0/discord_status_updater/plugin_base.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-05-23 18:31:44.976442 discord_status_updater-0.1.0/discord_status_updater/plugins/
--rw-r--r--   0 nick      (1000) nick      (1000)       41 2023-05-22 23:26:43.000000 discord_status_updater-0.1.0/discord_status_updater/plugins/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1538 2023-05-23 07:48:48.000000 discord_status_updater-0.1.0/discord_status_updater/plugins/locked.py
--rw-r--r--   0 nick      (1000) nick      (1000)     3970 2023-05-23 10:59:55.000000 discord_status_updater-0.1.0/discord_status_updater/plugins/mpris.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-05-23 18:31:44.976442 discord_status_updater-0.1.0/discord_status_updater.egg-info/
--rw-r--r--   0 nick      (1000) nick      (1000)     3368 2023-05-23 18:31:44.000000 discord_status_updater-0.1.0/discord_status_updater.egg-info/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)      675 2023-05-23 18:31:44.000000 discord_status_updater-0.1.0/discord_status_updater.egg-info/SOURCES.txt
--rw-r--r--   0 nick      (1000) nick      (1000)        1 2023-05-23 18:31:44.000000 discord_status_updater-0.1.0/discord_status_updater.egg-info/dependency_links.txt
--rw-r--r--   0 nick      (1000) nick      (1000)      236 2023-05-23 18:31:44.000000 discord_status_updater-0.1.0/discord_status_updater.egg-info/entry_points.txt
--rw-r--r--   0 nick      (1000) nick      (1000)       29 2023-05-23 18:31:44.000000 discord_status_updater-0.1.0/discord_status_updater.egg-info/requires.txt
--rw-r--r--   0 nick      (1000) nick      (1000)       23 2023-05-23 18:31:44.000000 discord_status_updater-0.1.0/discord_status_updater.egg-info/top_level.txt
--rw-r--r--   0 nick      (1000) nick      (1000)     1111 2023-05-23 18:31:44.976442 discord_status_updater-0.1.0/setup.cfg
--rw-r--r--   0 nick      (1000) nick      (1000)       38 2023-05-22 22:41:34.000000 discord_status_updater-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:48:44.433528 discord_status_updater-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-25 13:48:33.000000 discord_status_updater-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-25 13:48:44.433528 discord_status_updater-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-25 13:48:33.000000 discord_status_updater-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:48:44.433528 discord_status_updater-0.2.0/discord_status_updater/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 13:48:33.000000 discord_status_updater-0.2.0/discord_status_updater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-25 13:48:33.000000 discord_status_updater-0.2.0/discord_status_updater/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-25 13:48:33.000000 discord_status_updater-0.2.0/discord_status_updater/discord_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-25 13:48:33.000000 discord_status_updater-0.2.0/discord_status_updater/discord_status_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-25 13:48:33.000000 discord_status_updater-0.2.0/discord_status_updater/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-25 13:48:33.000000 discord_status_updater-0.2.0/discord_status_updater/plugin_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:48:44.433528 discord_status_updater-0.2.0/discord_status_updater/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 13:48:33.000000 discord_status_updater-0.2.0/discord_status_updater/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-25 13:48:33.000000 discord_status_updater-0.2.0/discord_status_updater/plugins/locked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-25 13:48:33.000000 discord_status_updater-0.2.0/discord_status_updater/plugins/mpris.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:48:44.433528 discord_status_updater-0.2.0/discord_status_updater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-25 13:48:44.000000 discord_status_updater-0.2.0/discord_status_updater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-25 13:48:44.000000 discord_status_updater-0.2.0/discord_status_updater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:48:44.000000 discord_status_updater-0.2.0/discord_status_updater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-25 13:48:44.000000 discord_status_updater-0.2.0/discord_status_updater.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-25 13:48:44.000000 discord_status_updater-0.2.0/discord_status_updater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 13:48:44.000000 discord_status_updater-0.2.0/discord_status_updater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-25 13:48:33.000000 discord_status_updater-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-25 13:48:44.437528 discord_status_updater-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 13:48:33.000000 discord_status_updater-0.2.0/setup.py
```

### Comparing `discord_status_updater-0.1.0/LICENSE.txt` & `discord_status_updater-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discord_status_updater-0.1.0/PKG-INFO` & `discord_status_updater-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord_status_updater
-Version: 0.1.0
+Version: 0.2.0
 Summary: updates Discord status depending on various conditions
 Home-page: https://github.com/Kolcha/DiscordStatusUpdater
 Author: Nick Korotysh
 Author-email: nick.korotysh@gmail.com
 License: MIT
 Keywords: Discord
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `discord_status_updater-0.1.0/README.md` & `discord_status_updater-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `discord_status_updater-0.1.0/discord_status_updater/discord_client.py` & `discord_status_updater-0.2.0/discord_status_updater/discord_client.py`

 * *Files identical despite different names*

### Comparing `discord_status_updater-0.1.0/discord_status_updater/discord_status_updater.py` & `discord_status_updater-0.2.0/discord_status_updater/discord_status_updater.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,19 +25,21 @@
         if not self.__discord.login(*credentials):
             return False
         self.__status = self.__discord.get_status()
         for p in self.plugins:
             cls = p.load()
             inst = cls(self.__config['plugins'][p.name])
             inst.set_status(self.__status)
-            inst.on_status_changed = self._on_status_changed
+            inst.on_status_changed(self._on_status_changed)
             self.__plugins.append(inst)
+        [p.start() for p in self.__plugins]
         return True
 
     def stop(self):
+        [p.stop() for p in self.__plugins]
         self.__plugins.clear()
         self.__discord.logout()
 
     def _on_status_changed(self, status):
         self.__status.update(status)
         [p.set_status(self.__status) for p in self.__plugins]
         self.__discord.update_status(self.__status)
```

### Comparing `discord_status_updater-0.1.0/discord_status_updater/launcher.py` & `discord_status_updater-0.2.0/discord_status_updater/launcher.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,36 +15,35 @@
         else:
             pcfg[p.name] = {}
     cfg['plugins'] = pcfg
     return cfg
 
 
 def main() -> int:
+    import asyncio
     import json
     import signal
 
-    import gi.repository.GLib
-
     if not cfg_path.exists():
         with cfg_path.open('w', encoding='utf-8') as f:
             json.dump(default_config(), f, ensure_ascii=False, indent=2)
         cfg_path.chmod(0o600)
         return 1
 
     with open(cfg_path, 'r', encoding='utf-8') as f:
         config = json.load(f)
 
     updater = DiscordStatusUpdater(config)
     if not updater.start():
         return 1
 
-    loop = gi.repository.GLib.MainLoop()
+    loop = asyncio.get_event_loop()
 
     def signal_handler(signum, frame):
         updater.stop()
-        loop.quit()
+        loop.stop()
 
     signal.signal(signal.SIGINT, signal_handler)
     signal.signal(signal.SIGTERM, signal_handler)
 
-    loop.run()
+    loop.run_forever()
     return 0
```

### Comparing `discord_status_updater-0.1.0/discord_status_updater.egg-info/PKG-INFO` & `discord_status_updater-0.2.0/discord_status_updater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-status-updater
-Version: 0.1.0
+Version: 0.2.0
 Summary: updates Discord status depending on various conditions
 Home-page: https://github.com/Kolcha/DiscordStatusUpdater
 Author: Nick Korotysh
 Author-email: nick.korotysh@gmail.com
 License: MIT
 Keywords: Discord
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `discord_status_updater-0.1.0/discord_status_updater.egg-info/SOURCES.txt` & `discord_status_updater-0.2.0/discord_status_updater.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE.txt
 README.md
+requirements.txt
 setup.cfg
 setup.py
 discord_status_updater/__init__.py
 discord_status_updater/__main__.py
 discord_status_updater/discord_client.py
 discord_status_updater/discord_status_updater.py
 discord_status_updater/launcher.py
```

### Comparing `discord_status_updater-0.1.0/setup.cfg` & `discord_status_updater-0.2.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,15 @@
 	Programming Language :: Python :: 3
 	Topic :: Communications :: Chat
 	Topic :: Utilities
 
 [options]
 packages = find:
 python_requires = >=3.8
-install_requires = 
-	pydbus
-	python-magic
-	requests
+install_requires = file: requirements.txt
 
 [options.entry_points]
 console_scripts = 
 	discord-status-updater = discord_status_updater.launcher:main
 discord_status_updater_plugins = 
 	mpris = discord_status_updater.plugins.mpris:PlayerPlugin
 	locked = discord_status_updater.plugins.locked:ScreenLockPlugin
```

