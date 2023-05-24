# Comparing `tmp/sensapex-1.22.8.tar.gz` & `tmp/sensapex-1.400.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sensapex-1.22.8.tar", last modified: Tue Nov  1 02:34:49 2022, max compression
+gzip compressed data, was "dist/sensapex-1.400.0.tar", last modified: Wed May 24 22:28:13 2023, max compression
```

## Comparing `sensapex-1.22.8.tar` & `sensapex-1.400.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2022-11-01 02:34:49.000000 sensapex-1.22.8/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1121 2020-09-02 18:19:21.000000 sensapex-1.22.8/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)     7078 2022-11-01 02:34:49.000000 sensapex-1.22.8/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     4833 2022-11-01 02:33:55.000000 sensapex-1.22.8/README.md
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2022-11-01 02:34:49.000000 sensapex-1.22.8/sensapex/
--rw-rw-r--   0 martin    (1000) martin    (1000)      116 2022-11-01 02:33:55.000000 sensapex-1.22.8/sensapex/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     8708 2022-06-15 20:01:28.000000 sensapex-1.22.8/sensapex/accuracy_test.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3433 2022-10-11 22:06:40.000000 sensapex-1.22.8/sensapex/pressure_test.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    35385 2022-10-14 19:58:45.000000 sensapex-1.22.8/sensapex/sensapex.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1783 2021-09-03 22:39:42.000000 sensapex-1.22.8/sensapex/test.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4814 2021-09-03 19:54:37.000000 sensapex-1.22.8/sensapex/utils.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2022-11-01 02:34:49.000000 sensapex-1.22.8/sensapex.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     7078 2022-11-01 02:34:49.000000 sensapex-1.22.8/sensapex.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      359 2022-11-01 02:34:49.000000 sensapex-1.22.8/sensapex.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2022-11-01 02:34:49.000000 sensapex-1.22.8/sensapex.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        6 2022-11-01 02:34:49.000000 sensapex-1.22.8/sensapex.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       15 2022-11-01 02:34:49.000000 sensapex-1.22.8/sensapex.egg-info/top_level.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2022-11-01 02:34:49.000000 sensapex-1.22.8/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)     2907 2022-11-01 02:33:55.000000 sensapex-1.22.8/setup.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2022-11-01 02:34:49.000000 sensapex-1.22.8/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2020-12-07 21:42:29.000000 sensapex-1.22.8/tests/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5171 2020-12-07 21:42:29.000000 sensapex-1.22.8/tests/test_move_request.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-24 22:28:13.000000 sensapex-1.400.0/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1121 2020-09-02 18:19:21.000000 sensapex-1.400.0/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7210 2023-05-24 22:28:13.000000 sensapex-1.400.0/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4932 2023-05-24 22:27:54.000000 sensapex-1.400.0/README.md
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-24 22:28:13.000000 sensapex-1.400.0/sensapex/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      116 2023-05-04 19:40:12.000000 sensapex-1.400.0/sensapex/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8763 2023-05-24 22:26:31.000000 sensapex-1.400.0/sensapex/accuracy_test.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3433 2022-10-11 22:06:40.000000 sensapex-1.400.0/sensapex/pressure_test.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    35388 2023-05-04 19:40:12.000000 sensapex-1.400.0/sensapex/sensapex.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1783 2021-09-03 22:39:42.000000 sensapex-1.400.0/sensapex/test.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4814 2021-09-03 19:54:37.000000 sensapex-1.400.0/sensapex/utils.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-24 22:28:13.000000 sensapex-1.400.0/sensapex.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7210 2023-05-24 22:28:13.000000 sensapex-1.400.0/sensapex.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      359 2023-05-24 22:28:13.000000 sensapex-1.400.0/sensapex.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-05-24 22:28:13.000000 sensapex-1.400.0/sensapex.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        6 2023-05-24 22:28:13.000000 sensapex-1.400.0/sensapex.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       15 2023-05-24 22:28:13.000000 sensapex-1.400.0/sensapex.egg-info/top_level.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-05-24 22:28:13.000000 sensapex-1.400.0/setup.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2936 2023-05-04 19:40:12.000000 sensapex-1.400.0/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-24 22:28:13.000000 sensapex-1.400.0/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2020-12-07 21:42:29.000000 sensapex-1.400.0/tests/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5171 2020-12-07 21:42:29.000000 sensapex-1.400.0/tests/test_move_request.py
```

### Comparing `sensapex-1.22.8/LICENSE` & `sensapex-1.400.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sensapex-1.22.8/PKG-INFO` & `sensapex-1.400.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sensapex
-Version: 1.22.8
+Version: 1.400.0
 Summary: Python wrapper for the Sensapex SDK
 Home-page: https://github.com/sensapex/sensapex-py
 Author: Luke Campagnola
 Author-email: luke.campagnola@gmail.com
 License: MIT
 Description: # Sensapex SDK
         
@@ -128,14 +128,18 @@
         * Luke Campagnola
         * Ari Salmi
         * Martin Chase
         * Thomas Braun
         
         ### Changelog
         
+        #### 1.400.0
+        * Update to latest driver
+        * Accuracy test for 4-axis devices (ignoring the 4th axis)
+        
         #### 1.022.8
         * Include ACQ4 integration instructions in README
         
         #### 1.022.7
         * Packaging fix to include driver binary.
         * find_library to find libum in default locations.
```

### Comparing `sensapex-1.22.8/README.md` & `sensapex-1.400.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -120,14 +120,18 @@
 * Luke Campagnola
 * Ari Salmi
 * Martin Chase
 * Thomas Braun
 
 ### Changelog
 
+#### 1.400.0
+* Update to latest driver
+* Accuracy test for 4-axis devices (ignoring the 4th axis)
+
 #### 1.022.8
 * Include ACQ4 integration instructions in README
 
 #### 1.022.7
 * Packaging fix to include driver binary.
 * find_library to find libum in default locations.
```

### Comparing `sensapex-1.22.8/sensapex/accuracy_test.py` & `sensapex-1.400.0/sensapex/accuracy_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     # calculate closest point to the line from starting position to target
     target_to_pos = position - target
     target_to_last = last_position_before_move - target
     target_to_last /= np.linalg.norm(target_to_last)
     closest_pos = target + np.dot(target_to_pos, target_to_last) * target_to_last
     dist = position - closest_pos
 
-    for i in range(n_axes):
+    for i in range(min(3, n_axes)):
         pos[i].append((position[i] - start_pos[i]) * 1e-6)
         tgt[i].append((target[i] - start_pos[i]) * 1e-6)
         if moving:
             err[i].append(np.nan)
             # only update linear error when moving
             closest[i].append((closest_pos[i] - start_pos[i]) * 1e-6)
             linear_err[i].append(dist[i] * 1e-6)
@@ -200,15 +200,15 @@
 positions = []
 n_axes = dev.n_axes()
 assert (
     len(start_pos) == n_axes
 ), f"Starting position {start_pos} has length {len(start_pos)}, but device has {n_axes} axes."
 if args.test_pos is None:
     moves = np.random.random(size=(args.iter, n_axes)) * args.distance
-    move_axes = np.array([args.x, args.y, args.z])[:n_axes]
+    move_axes = np.array([args.x, args.y, args.z, False])[:n_axes]
     assert np.any(move_axes), "No axes selected to move (use --x, --y, --z, or --test-pos)"
     moves[:, ~move_axes] = 0
     targets = np.array(start_pos)[np.newaxis, :] + moves
     print(f"Distance to move each axis:\n{moves}")
     print(f"Target positions:\n{targets}")
 else:
     # just move back and forth between start and test position
@@ -223,15 +223,17 @@
 
 if args.retry_threshold is not None:
     ump.set_retry_threshold(args.retry_threshold)
 
 for i in range(args.iter):
     target = targets[i]
     last_position_before_move = dev.get_pos()
-    move_req = dev.goto_pos(target, speed=speeds[i], linear=args.linear, max_acceleration=args.acceleration)
+    move_req = dev.goto_pos(
+        target, speed=speeds[i], linear=args.linear, simultaneous=args.linear, max_acceleration=args.acceleration
+    )
     while not move_req.finished:
         update(moving=True)
         time.sleep(0.002)
     waitstart = time.perf_counter()
     while time.perf_counter() - waitstart < 1.0:
         update(moving=False)
         time.sleep(0.002)
```

### Comparing `sensapex-1.22.8/sensapex/pressure_test.py` & `sensapex-1.400.0/sensapex/pressure_test.py`

 * *Files identical despite different names*

### Comparing `sensapex-1.22.8/sensapex/sensapex.py` & `sensapex-1.400.0/sensapex/sensapex.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
                     self._movement_args(max_acceleration, dest4, speed, simultaneous),
                 )
 
     def _movement_args(self, max_acceleration, pos4, speed, simultaneous) -> List[Union[c_int, c_float]]:
         mode = int(bool(simultaneous))  # whether all axes move simultaneously
         retval: List[Union[c_int, c_float]] = [c_int(self.dev)]
         retval += [c_float(x) for x in pos4]
-        retval += [c_int(int(x)) for x in speed]
+        retval += [c_float(int(x)) for x in speed]
         retval += [c_int(int(x)) for x in [mode, max_acceleration]]
         assert len(retval) == 11
         return retval
 
     def interrupt(self, reason):
         self.ump.call("um_stop", c_int(self.dev))
         self.interrupt_reason = reason
@@ -383,15 +383,15 @@
         self._debug_dir = "sensapex-debug"
         self._debug_file = None
         self._pcap_proc = None
         self._dev_ids_seen = set()
         self._set_debug_mode(self._debug)
 
         min_version = (1, 21)
-        max_version = (1, 23)
+        max_version = (1, 400)
         version_str = self.sdk_version()
         version = tuple(map(int, version_str.lstrip(b"v").split(b".")))
 
         if version < min_version:
             min_version_str = "v{:d}.{:d}".format(*min_version)
             raise RuntimeError(f"SDK version {min_version_str} or later required (your version is {version_str})")
         if version > max_version:
```

### Comparing `sensapex-1.22.8/sensapex/test.py` & `sensapex-1.400.0/sensapex/test.py`

 * *Files identical despite different names*

### Comparing `sensapex-1.22.8/sensapex/utils.py` & `sensapex-1.400.0/sensapex/utils.py`

 * *Files identical despite different names*

### Comparing `sensapex-1.22.8/sensapex.egg-info/PKG-INFO` & `sensapex-1.400.0/sensapex.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sensapex
-Version: 1.22.8
+Version: 1.400.0
 Summary: Python wrapper for the Sensapex SDK
 Home-page: https://github.com/sensapex/sensapex-py
 Author: Luke Campagnola
 Author-email: luke.campagnola@gmail.com
 License: MIT
 Description: # Sensapex SDK
         
@@ -128,14 +128,18 @@
         * Luke Campagnola
         * Ari Salmi
         * Martin Chase
         * Thomas Braun
         
         ### Changelog
         
+        #### 1.400.0
+        * Update to latest driver
+        * Accuracy test for 4-axis devices (ignoring the 4th axis)
+        
         #### 1.022.8
         * Include ACQ4 integration instructions in README
         
         #### 1.022.7
         * Packaging fix to include driver binary.
         * find_library to find libum in default locations.
```

### Comparing `sensapex-1.22.8/setup.py` & `sensapex-1.400.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,21 +22,21 @@
         install_bin(os.path.join(self.egg_path, "sensapex"))
 
 
 def install_bin(path, force=False):
     """Install libum.dll and umpcli.exe to *path*."""
     if force or platform.system() == "Windows":
         dll_data = download_from_zip(
-            "http://dist.sensapex.com/misc/um-sdk/latest/umsdk-1.022-binaries.zip", ["libum.dll"]
+            "https://github.com/sensapex/umsdk/releases/download/v1.400/umsdk-1.400-binaries.zip", ["umsdk-1.400-binaries/x64/libum.dll"]
         )[0]
         print(f"Install libum.dll to {path}")
         with open(os.path.join(path, "libum.dll"), "wb") as install_target:
             install_target.write(dll_data)
         umpcli_data = download_from_zip(
-            "http://dist.sensapex.com/misc/umpcli/umpcli-0_951-beta.zip", ["umpcli-0_951-beta.exe"]
+            "http://dist.sensapex.com/misc/umpcli/umpcli-0_957-beta.zip", ["umpcli.exe"]
         )[0]
         with open(os.path.join(path, "umpcli.exe"), "wb") as install_target:
             install_target.write(umpcli_data)
 
 
 def download_from_zip(url, files):
     req = urllib.request.urlopen(url)
@@ -73,9 +73,9 @@
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     name="sensapex",
     packages=find_packages(),
     python_requires=">=3.7",
     url="https://github.com/sensapex/sensapex-py",
-    version="1.022.8",  # in lock step with umsdk version. don't forget __version__ and changelog!
+    version="1.400.0",  # in lock step with umsdk version. don't forget __version__ and changelog!
 )
```

### Comparing `sensapex-1.22.8/tests/test_move_request.py` & `sensapex-1.400.0/tests/test_move_request.py`

 * *Files identical despite different names*

