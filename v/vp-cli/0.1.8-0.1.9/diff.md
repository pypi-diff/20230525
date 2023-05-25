# Comparing `tmp/vp-cli-0.1.8.tar.gz` & `tmp/vp-cli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vp-cli-0.1.8.tar", last modified: Tue Mar 21 15:45:05 2023, max compression
+gzip compressed data, was "vp-cli-0.1.9.tar", last modified: Tue Mar 21 15:52:25 2023, max compression
```

## Comparing `vp-cli-0.1.8.tar` & `vp-cli-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 collins    (501) staff       (20)        0 2023-03-21 15:45:05.420110 vp-cli-0.1.8/
--rw-r--r--   0 collins    (501) staff       (20)       49 2023-03-13 16:06:22.000000 vp-cli-0.1.8/MANIFEST.in
--rw-r--r--   0 collins    (501) staff       (20)     1998 2023-03-21 15:45:05.419804 vp-cli-0.1.8/PKG-INFO
--rw-r--r--   0 collins    (501) staff       (20)     1423 2022-10-19 21:37:21.000000 vp-cli-0.1.8/README.md
-drwxr-xr-x   0 collins    (501) staff       (20)        0 2023-03-21 15:45:05.414319 vp-cli-0.1.8/cli/
--rw-r--r--   0 collins    (501) staff       (20)        1 2020-05-19 18:47:46.000000 vp-cli-0.1.8/cli/__init__.py
--rw-r--r--   0 collins    (501) staff       (20)     8058 2023-03-21 15:44:34.000000 vp-cli-0.1.8/cli/agent.py
--rw-r--r--   0 collins    (501) staff       (20)    14067 2023-03-16 15:32:12.000000 vp-cli-0.1.8/cli/apiexternal.py
--rw-r--r--   0 collins    (501) staff       (20)     8064 2021-03-11 13:57:06.000000 vp-cli-0.1.8/cli/collector.py
--rw-r--r--   0 collins    (501) staff       (20)      107 2023-03-21 15:44:56.000000 vp-cli-0.1.8/cli/consts.py
--rw-r--r--   0 collins    (501) staff       (20)     1053 2020-07-14 20:06:39.000000 vp-cli-0.1.8/cli/docopt_command.py
--rw-r--r--   0 collins    (501) staff       (20)     4843 2020-07-14 20:06:39.000000 vp-cli-0.1.8/cli/file_event_search.py
--rw-r--r--   0 collins    (501) staff       (20)     3580 2020-10-16 14:31:33.000000 vp-cli-0.1.8/cli/image.py
--rw-r--r--   0 collins    (501) staff       (20)     2165 2023-03-13 15:13:33.000000 vp-cli-0.1.8/cli/inspections.py
--rw-r--r--   0 collins    (501) staff       (20)     7847 2021-03-11 13:57:06.000000 vp-cli-0.1.8/cli/integration.py
--rw-r--r--   0 collins    (501) staff       (20)      284 2020-12-07 01:26:44.000000 vp-cli-0.1.8/cli/logger.ini
--rw-r--r--   0 collins    (501) staff       (20)    14963 2023-03-16 14:57:26.000000 vp-cli-0.1.8/cli/main.py
--rw-r--r--   0 collins    (501) staff       (20)     2985 2020-10-13 16:13:16.000000 vp-cli-0.1.8/cli/reputation.py
-drwxr-xr-x   0 collins    (501) staff       (20)        0 2023-03-21 15:45:05.415582 vp-cli-0.1.8/cli/schemas/
--rw-r--r--   0 collins    (501) staff       (20)     1780 2020-07-14 20:06:39.000000 vp-cli-0.1.8/cli/schemas/reputation_schema_v1.json
--rw-r--r--   0 collins    (501) staff       (20)     9618 2022-10-17 22:18:21.000000 vp-cli-0.1.8/cli/util.py
--rw-r--r--   0 collins    (501) staff       (20)      847 2021-03-11 13:57:06.000000 vp-cli-0.1.8/cli/workspace.py
--rw-r--r--   0 collins    (501) staff       (20)       38 2023-03-21 15:45:05.420190 vp-cli-0.1.8/setup.cfg
--rw-r--r--   0 collins    (501) staff       (20)     2526 2023-03-13 21:20:59.000000 vp-cli-0.1.8/setup.py
-drwxr-xr-x   0 collins    (501) staff       (20)        0 2023-03-21 15:45:05.416428 vp-cli-0.1.8/tests/
--rw-r--r--   0 collins    (501) staff       (20)       36 2020-07-14 20:06:39.000000 vp-cli-0.1.8/tests/test_example.py
--rw-r--r--   0 collins    (501) staff       (20)      216 2023-03-13 15:13:33.000000 vp-cli-0.1.8/tox.ini
-drwxr-xr-x   0 collins    (501) staff       (20)        0 2023-03-21 15:45:05.419423 vp-cli-0.1.8/vp_cli.egg-info/
--rw-r--r--   0 collins    (501) staff       (20)     1998 2023-03-21 15:45:05.000000 vp-cli-0.1.8/vp_cli.egg-info/PKG-INFO
--rw-r--r--   0 collins    (501) staff       (20)      531 2023-03-21 15:45:05.000000 vp-cli-0.1.8/vp_cli.egg-info/SOURCES.txt
--rw-r--r--   0 collins    (501) staff       (20)        1 2023-03-21 15:45:05.000000 vp-cli-0.1.8/vp_cli.egg-info/dependency_links.txt
--rw-r--r--   0 collins    (501) staff       (20)       41 2023-03-21 15:45:05.000000 vp-cli-0.1.8/vp_cli.egg-info/entry_points.txt
--rw-r--r--   0 collins    (501) staff       (20)      868 2023-03-21 15:45:05.000000 vp-cli-0.1.8/vp_cli.egg-info/requires.txt
--rw-r--r--   0 collins    (501) staff       (20)        4 2023-03-21 15:45:05.000000 vp-cli-0.1.8/vp_cli.egg-info/top_level.txt
+drwxr-xr-x   0 collins    (501) staff       (20)        0 2023-03-21 15:52:25.298389 vp-cli-0.1.9/
+-rw-r--r--   0 collins    (501) staff       (20)       49 2023-03-13 16:06:22.000000 vp-cli-0.1.9/MANIFEST.in
+-rw-r--r--   0 collins    (501) staff       (20)     1998 2023-03-21 15:52:25.298025 vp-cli-0.1.9/PKG-INFO
+-rw-r--r--   0 collins    (501) staff       (20)     1423 2022-10-19 21:37:21.000000 vp-cli-0.1.9/README.md
+drwxr-xr-x   0 collins    (501) staff       (20)        0 2023-03-21 15:52:25.293866 vp-cli-0.1.9/cli/
+-rw-r--r--   0 collins    (501) staff       (20)        1 2020-05-19 18:47:46.000000 vp-cli-0.1.9/cli/__init__.py
+-rw-r--r--   0 collins    (501) staff       (20)     8053 2023-03-21 15:52:00.000000 vp-cli-0.1.9/cli/agent.py
+-rw-r--r--   0 collins    (501) staff       (20)    14067 2023-03-16 15:32:12.000000 vp-cli-0.1.9/cli/apiexternal.py
+-rw-r--r--   0 collins    (501) staff       (20)     8064 2021-03-11 13:57:06.000000 vp-cli-0.1.9/cli/collector.py
+-rw-r--r--   0 collins    (501) staff       (20)      107 2023-03-21 15:52:07.000000 vp-cli-0.1.9/cli/consts.py
+-rw-r--r--   0 collins    (501) staff       (20)     1053 2020-07-14 20:06:39.000000 vp-cli-0.1.9/cli/docopt_command.py
+-rw-r--r--   0 collins    (501) staff       (20)     4843 2020-07-14 20:06:39.000000 vp-cli-0.1.9/cli/file_event_search.py
+-rw-r--r--   0 collins    (501) staff       (20)     3580 2020-10-16 14:31:33.000000 vp-cli-0.1.9/cli/image.py
+-rw-r--r--   0 collins    (501) staff       (20)     2165 2023-03-13 15:13:33.000000 vp-cli-0.1.9/cli/inspections.py
+-rw-r--r--   0 collins    (501) staff       (20)     7847 2021-03-11 13:57:06.000000 vp-cli-0.1.9/cli/integration.py
+-rw-r--r--   0 collins    (501) staff       (20)      284 2020-12-07 01:26:44.000000 vp-cli-0.1.9/cli/logger.ini
+-rw-r--r--   0 collins    (501) staff       (20)    14963 2023-03-16 14:57:26.000000 vp-cli-0.1.9/cli/main.py
+-rw-r--r--   0 collins    (501) staff       (20)     2985 2020-10-13 16:13:16.000000 vp-cli-0.1.9/cli/reputation.py
+drwxr-xr-x   0 collins    (501) staff       (20)        0 2023-03-21 15:52:25.294415 vp-cli-0.1.9/cli/schemas/
+-rw-r--r--   0 collins    (501) staff       (20)     1780 2020-07-14 20:06:39.000000 vp-cli-0.1.9/cli/schemas/reputation_schema_v1.json
+-rw-r--r--   0 collins    (501) staff       (20)     9618 2022-10-17 22:18:21.000000 vp-cli-0.1.9/cli/util.py
+-rw-r--r--   0 collins    (501) staff       (20)      847 2021-03-11 13:57:06.000000 vp-cli-0.1.9/cli/workspace.py
+-rw-r--r--   0 collins    (501) staff       (20)       38 2023-03-21 15:52:25.298475 vp-cli-0.1.9/setup.cfg
+-rw-r--r--   0 collins    (501) staff       (20)     2526 2023-03-13 21:20:59.000000 vp-cli-0.1.9/setup.py
+drwxr-xr-x   0 collins    (501) staff       (20)        0 2023-03-21 15:52:25.295088 vp-cli-0.1.9/tests/
+-rw-r--r--   0 collins    (501) staff       (20)       36 2020-07-14 20:06:39.000000 vp-cli-0.1.9/tests/test_example.py
+-rw-r--r--   0 collins    (501) staff       (20)      216 2023-03-13 15:13:33.000000 vp-cli-0.1.9/tox.ini
+drwxr-xr-x   0 collins    (501) staff       (20)        0 2023-03-21 15:52:25.297554 vp-cli-0.1.9/vp_cli.egg-info/
+-rw-r--r--   0 collins    (501) staff       (20)     1998 2023-03-21 15:52:25.000000 vp-cli-0.1.9/vp_cli.egg-info/PKG-INFO
+-rw-r--r--   0 collins    (501) staff       (20)      531 2023-03-21 15:52:25.000000 vp-cli-0.1.9/vp_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 collins    (501) staff       (20)        1 2023-03-21 15:52:25.000000 vp-cli-0.1.9/vp_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 collins    (501) staff       (20)       41 2023-03-21 15:52:25.000000 vp-cli-0.1.9/vp_cli.egg-info/entry_points.txt
+-rw-r--r--   0 collins    (501) staff       (20)      868 2023-03-21 15:52:25.000000 vp-cli-0.1.9/vp_cli.egg-info/requires.txt
+-rw-r--r--   0 collins    (501) staff       (20)        4 2023-03-21 15:52:25.000000 vp-cli-0.1.9/vp_cli.egg-info/top_level.txt
```

### Comparing `vp-cli-0.1.8/PKG-INFO` & `vp-cli-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vp-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: VantagePoint CLI
 Author: VantagePoint
 Author-email: developers@vantagepoint.co
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `vp-cli-0.1.8/README.md` & `vp-cli-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `vp-cli-0.1.8/cli/agent.py` & `vp-cli-0.1.9/cli/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
             log.info("Installing agent...")
             with open("./vp_agent_install.sh", "w") as f:
                 f.write(install_script)
 
             os.chmod("./vp_agent_install.sh", 755)
             process = subprocess.Popen(
-                ["sudo", "./vp_agent_install.sh"],
+                "sudo ./vp_agent_install.sh",
                 shell=True,
                 stdout=subprocess.PIPE,
                 stdin=subprocess.PIPE,
                 env=env,
             )
 
             process.wait()
```

### Comparing `vp-cli-0.1.8/cli/apiexternal.py` & `vp-cli-0.1.9/cli/apiexternal.py`

 * *Files identical despite different names*

### Comparing `vp-cli-0.1.8/cli/collector.py` & `vp-cli-0.1.9/cli/collector.py`

 * *Files identical despite different names*

### Comparing `vp-cli-0.1.8/cli/docopt_command.py` & `vp-cli-0.1.9/cli/docopt_command.py`

 * *Files identical despite different names*

### Comparing `vp-cli-0.1.8/cli/file_event_search.py` & `vp-cli-0.1.9/cli/file_event_search.py`

 * *Files identical despite different names*

### Comparing `vp-cli-0.1.8/cli/image.py` & `vp-cli-0.1.9/cli/image.py`

 * *Files identical despite different names*

### Comparing `vp-cli-0.1.8/cli/inspections.py` & `vp-cli-0.1.9/cli/inspections.py`

 * *Files identical despite different names*

### Comparing `vp-cli-0.1.8/cli/integration.py` & `vp-cli-0.1.9/cli/integration.py`

 * *Files identical despite different names*

### Comparing `vp-cli-0.1.8/cli/main.py` & `vp-cli-0.1.9/cli/main.py`

 * *Files identical despite different names*

### Comparing `vp-cli-0.1.8/cli/reputation.py` & `vp-cli-0.1.9/cli/reputation.py`

 * *Files identical despite different names*

### Comparing `vp-cli-0.1.8/cli/schemas/reputation_schema_v1.json` & `vp-cli-0.1.9/cli/schemas/reputation_schema_v1.json`

 * *Files identical despite different names*

### Comparing `vp-cli-0.1.8/cli/util.py` & `vp-cli-0.1.9/cli/util.py`

 * *Files identical despite different names*

### Comparing `vp-cli-0.1.8/cli/workspace.py` & `vp-cli-0.1.9/cli/workspace.py`

 * *Files identical despite different names*

### Comparing `vp-cli-0.1.8/setup.py` & `vp-cli-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `vp-cli-0.1.8/vp_cli.egg-info/PKG-INFO` & `vp-cli-0.1.9/vp_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vp-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: VantagePoint CLI
 Author: VantagePoint
 Author-email: developers@vantagepoint.co
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `vp-cli-0.1.8/vp_cli.egg-info/SOURCES.txt` & `vp-cli-0.1.9/vp_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vp-cli-0.1.8/vp_cli.egg-info/requires.txt` & `vp-cli-0.1.9/vp_cli.egg-info/requires.txt`

 * *Files identical despite different names*

