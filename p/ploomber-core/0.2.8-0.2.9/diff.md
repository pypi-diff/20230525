# Comparing `tmp/ploomber-core-0.2.8.tar.gz` & `tmp/ploomber-core-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ploomber-core-0.2.8.tar", last modified: Mon Mar 27 17:00:37 2023, max compression
+gzip compressed data, was "ploomber-core-0.2.9.tar", last modified: Wed Mar 29 17:09:13 2023, max compression
```

## Comparing `ploomber-core-0.2.8.tar` & `ploomber-core-0.2.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-03-27 17:00:37.324442 ploomber-core-0.2.8/
--rw-r--r--   0 eduardo    (501) staff       (20)     2755 2023-03-27 17:00:36.000000 ploomber-core-0.2.8/CHANGELOG.md
--rw-r--r--   0 eduardo    (501) staff       (20)    11355 2023-01-12 03:29:51.000000 ploomber-core-0.2.8/LICENSE
--rw-r--r--   0 eduardo    (501) staff       (20)      247 2022-11-25 15:42:29.000000 ploomber-core-0.2.8/MANIFEST.in
--rw-r--r--   0 eduardo    (501) staff       (20)      162 2023-03-27 17:00:37.324487 ploomber-core-0.2.8/PKG-INFO
--rw-r--r--   0 eduardo    (501) staff       (20)      217 2022-12-24 02:33:23.000000 ploomber-core-0.2.8/README.md
--rw-r--r--   0 eduardo    (501) staff       (20)      265 2023-03-19 19:18:04.000000 ploomber-core-0.2.8/pyproject.toml
--rw-r--r--   0 eduardo    (501) staff       (20)      111 2023-03-27 17:00:37.324739 ploomber-core-0.2.8/setup.cfg
--rw-r--r--   0 eduardo    (501) staff       (20)     1025 2023-03-27 16:52:11.000000 ploomber-core-0.2.8/setup.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-03-27 17:00:37.322283 ploomber-core-0.2.8/src/
--rw-r--r--   0 eduardo    (501) staff       (20)      147 2022-12-23 17:04:20.000000 ploomber-core-0.2.8/src/conftest.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-03-27 17:00:37.323115 ploomber-core-0.2.8/src/ploomber_core/
--rw-r--r--   0 eduardo    (501) staff       (20)       22 2023-03-27 17:00:36.000000 ploomber-core-0.2.8/src/ploomber_core/__init__.py
--rw-r--r--   0 eduardo    (501) staff       (20)     4380 2022-12-24 02:33:23.000000 ploomber-core-0.2.8/src/ploomber_core/config.py
--rw-r--r--   0 eduardo    (501) staff       (20)     2770 2023-03-22 23:17:38.000000 ploomber-core-0.2.8/src/ploomber_core/dependencies.py
--rw-r--r--   0 eduardo    (501) staff       (20)     3496 2023-01-13 13:58:43.000000 ploomber-core-0.2.8/src/ploomber_core/deprecated.py
--rw-r--r--   0 eduardo    (501) staff       (20)     2453 2023-03-19 19:18:04.000000 ploomber-core-0.2.8/src/ploomber_core/exceptions.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-03-27 17:00:37.323950 ploomber-core-0.2.8/src/ploomber_core/io/
--rw-r--r--   0 eduardo    (501) staff       (20)        0 2023-02-16 11:36:18.000000 ploomber-core-0.2.8/src/ploomber_core/io/__init__.py
--rw-r--r--   0 eduardo    (501) staff       (20)      417 2023-03-19 19:18:04.000000 ploomber-core-0.2.8/src/ploomber_core/io/pretty_print.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-03-27 17:00:37.324346 ploomber-core-0.2.8/src/ploomber_core/telemetry/
--rw-r--r--   0 eduardo    (501) staff       (20)       81 2022-12-23 17:04:20.000000 ploomber-core-0.2.8/src/ploomber_core/telemetry/__init__.py
--rw-r--r--   0 eduardo    (501) staff       (20)    25954 2023-02-20 21:33:09.000000 ploomber-core-0.2.8/src/ploomber_core/telemetry/telemetry.py
--rw-r--r--   0 eduardo    (501) staff       (20)      628 2022-12-24 02:33:23.000000 ploomber-core-0.2.8/src/ploomber_core/telemetry/validate_inputs.py
--rw-r--r--   0 eduardo    (501) staff       (20)     2741 2023-03-19 19:18:04.000000 ploomber-core-0.2.8/src/ploomber_core/validate.py
--rw-r--r--   0 eduardo    (501) staff       (20)      184 2022-12-29 18:29:43.000000 ploomber-core-0.2.8/src/ploomber_core/warnings.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-03-27 17:00:37.323740 ploomber-core-0.2.8/src/ploomber_core.egg-info/
--rw-r--r--   0 eduardo    (501) staff       (20)      162 2023-03-27 17:00:37.000000 ploomber-core-0.2.8/src/ploomber_core.egg-info/PKG-INFO
--rw-r--r--   0 eduardo    (501) staff       (20)      710 2023-03-27 17:00:37.000000 ploomber-core-0.2.8/src/ploomber_core.egg-info/SOURCES.txt
--rw-r--r--   0 eduardo    (501) staff       (20)        1 2023-03-27 17:00:37.000000 ploomber-core-0.2.8/src/ploomber_core.egg-info/dependency_links.txt
--rw-r--r--   0 eduardo    (501) staff       (20)       61 2023-03-27 17:00:37.000000 ploomber-core-0.2.8/src/ploomber_core.egg-info/requires.txt
--rw-r--r--   0 eduardo    (501) staff       (20)       23 2023-03-27 17:00:37.000000 ploomber-core-0.2.8/src/ploomber_core.egg-info/top_level.txt
+drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-03-29 17:09:13.037640 ploomber-core-0.2.9/
+-rw-r--r--   0 eduardo    (501) staff       (20)     2907 2023-03-29 17:09:11.000000 ploomber-core-0.2.9/CHANGELOG.md
+-rw-r--r--   0 eduardo    (501) staff       (20)    11355 2023-01-12 03:29:51.000000 ploomber-core-0.2.9/LICENSE
+-rw-r--r--   0 eduardo    (501) staff       (20)      247 2022-11-25 15:42:29.000000 ploomber-core-0.2.9/MANIFEST.in
+-rw-r--r--   0 eduardo    (501) staff       (20)      162 2023-03-29 17:09:13.037690 ploomber-core-0.2.9/PKG-INFO
+-rw-r--r--   0 eduardo    (501) staff       (20)      217 2022-12-24 02:33:23.000000 ploomber-core-0.2.9/README.md
+-rw-r--r--   0 eduardo    (501) staff       (20)      265 2023-03-19 19:18:04.000000 ploomber-core-0.2.9/pyproject.toml
+-rw-r--r--   0 eduardo    (501) staff       (20)      111 2023-03-29 17:09:13.037870 ploomber-core-0.2.9/setup.cfg
+-rw-r--r--   0 eduardo    (501) staff       (20)     1025 2023-03-27 16:52:11.000000 ploomber-core-0.2.9/setup.py
+drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-03-29 17:09:13.035439 ploomber-core-0.2.9/src/
+-rw-r--r--   0 eduardo    (501) staff       (20)      147 2022-12-23 17:04:20.000000 ploomber-core-0.2.9/src/conftest.py
+drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-03-29 17:09:13.036258 ploomber-core-0.2.9/src/ploomber_core/
+-rw-r--r--   0 eduardo    (501) staff       (20)       22 2023-03-29 17:09:11.000000 ploomber-core-0.2.9/src/ploomber_core/__init__.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     4380 2022-12-24 02:33:23.000000 ploomber-core-0.2.9/src/ploomber_core/config.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     2770 2023-03-22 23:17:38.000000 ploomber-core-0.2.9/src/ploomber_core/dependencies.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     3496 2023-01-13 13:58:43.000000 ploomber-core-0.2.9/src/ploomber_core/deprecated.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     2453 2023-03-19 19:18:04.000000 ploomber-core-0.2.9/src/ploomber_core/exceptions.py
+drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-03-29 17:09:13.037115 ploomber-core-0.2.9/src/ploomber_core/io/
+-rw-r--r--   0 eduardo    (501) staff       (20)        0 2023-02-16 11:36:18.000000 ploomber-core-0.2.9/src/ploomber_core/io/__init__.py
+-rw-r--r--   0 eduardo    (501) staff       (20)      417 2023-03-19 19:18:04.000000 ploomber-core-0.2.9/src/ploomber_core/io/pretty_print.py
+drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-03-29 17:09:13.037542 ploomber-core-0.2.9/src/ploomber_core/telemetry/
+-rw-r--r--   0 eduardo    (501) staff       (20)       81 2022-12-23 17:04:20.000000 ploomber-core-0.2.9/src/ploomber_core/telemetry/__init__.py
+-rw-r--r--   0 eduardo    (501) staff       (20)    25930 2023-03-29 16:24:19.000000 ploomber-core-0.2.9/src/ploomber_core/telemetry/telemetry.py
+-rw-r--r--   0 eduardo    (501) staff       (20)      628 2022-12-24 02:33:23.000000 ploomber-core-0.2.9/src/ploomber_core/telemetry/validate_inputs.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     2741 2023-03-19 19:18:04.000000 ploomber-core-0.2.9/src/ploomber_core/validate.py
+-rw-r--r--   0 eduardo    (501) staff       (20)      184 2022-12-29 18:29:43.000000 ploomber-core-0.2.9/src/ploomber_core/warnings.py
+drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-03-29 17:09:13.036915 ploomber-core-0.2.9/src/ploomber_core.egg-info/
+-rw-r--r--   0 eduardo    (501) staff       (20)      162 2023-03-29 17:09:12.000000 ploomber-core-0.2.9/src/ploomber_core.egg-info/PKG-INFO
+-rw-r--r--   0 eduardo    (501) staff       (20)      710 2023-03-29 17:09:12.000000 ploomber-core-0.2.9/src/ploomber_core.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardo    (501) staff       (20)        1 2023-03-29 17:09:12.000000 ploomber-core-0.2.9/src/ploomber_core.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardo    (501) staff       (20)       61 2023-03-29 17:09:12.000000 ploomber-core-0.2.9/src/ploomber_core.egg-info/requires.txt
+-rw-r--r--   0 eduardo    (501) staff       (20)       23 2023-03-29 17:09:12.000000 ploomber-core-0.2.9/src/ploomber_core.egg-info/top_level.txt
```

### Comparing `ploomber-core-0.2.8/CHANGELOG.md` & `ploomber-core-0.2.9/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # CHANGELOG
 
+## 0.2.9 (2023-03-29)
+
+* [Fix] Do not check if there's internet connection when stats are disabled ([#55](https://github.com/ploomber/core/issues/55))
+
 ## 0.2.8 (2023-03-27)
 
 * [Fix] Adds LICENSE information to `setup.py`
 
 ## 0.2.7 (2023-03-22)
 
 * [Feature] Adds `ploomber_core.dependencies.check_installed` to check if packages are installed
```

### Comparing `ploomber-core-0.2.8/LICENSE` & `ploomber-core-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ploomber-core-0.2.8/setup.py` & `ploomber-core-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `ploomber-core-0.2.8/src/ploomber_core/config.py` & `ploomber-core-0.2.9/src/ploomber_core/config.py`

 * *Files identical despite different names*

### Comparing `ploomber-core-0.2.8/src/ploomber_core/dependencies.py` & `ploomber-core-0.2.9/src/ploomber_core/dependencies.py`

 * *Files identical despite different names*

### Comparing `ploomber-core-0.2.8/src/ploomber_core/deprecated.py` & `ploomber-core-0.2.9/src/ploomber_core/deprecated.py`

 * *Files identical despite different names*

### Comparing `ploomber-core-0.2.8/src/ploomber_core/exceptions.py` & `ploomber-core-0.2.9/src/ploomber_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `ploomber-core-0.2.8/src/ploomber_core/telemetry/telemetry.py` & `ploomber-core-0.2.9/src/ploomber_core/telemetry/telemetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -526,18 +526,17 @@
         if argo:
             metadata["argo"] = argo
 
         if "dag" in metadata:
             metadata["dag"] = parse_dag(metadata["dag"])
 
         os = get_os()
-        online = is_online()
         environment = get_env()
 
-        if telemetry_enabled and online:
+        if telemetry_enabled and is_online():
             (event_id, uid, action, client_time, elapsed_time) = validate_entries(
                 event_id, uid, action, client_time, total_runtime
             )
             props = {
                 "event_id": event_id,
                 "user_id": uid,
                 "action": action,
```

### Comparing `ploomber-core-0.2.8/src/ploomber_core/telemetry/validate_inputs.py` & `ploomber-core-0.2.9/src/ploomber_core/telemetry/validate_inputs.py`

 * *Files identical despite different names*

### Comparing `ploomber-core-0.2.8/src/ploomber_core/validate.py` & `ploomber-core-0.2.9/src/ploomber_core/validate.py`

 * *Files identical despite different names*

### Comparing `ploomber-core-0.2.8/src/ploomber_core.egg-info/SOURCES.txt` & `ploomber-core-0.2.9/src/ploomber_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

