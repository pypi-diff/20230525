# Comparing `tmp/openinverter-can-tool-0.0.7.tar.gz` & `tmp/openinverter-can-tool-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openinverter-can-tool-0.0.7.tar", last modified: Mon Apr 24 16:59:17 2023, max compression
+gzip compressed data, was "openinverter-can-tool-0.0.8.tar", last modified: Thu May 25 17:04:25 2023, max compression
```

## Comparing `openinverter-can-tool-0.0.7.tar` & `openinverter-can-tool-0.0.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:59:17.177675 openinverter-can-tool-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-24 16:59:17.177675 openinverter-can-tool-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:59:17.177675 openinverter-can-tool-0.0.7/parameter-databases/
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/parameter-databases/c2000-sine.5.14.R.C2000-foc.json
--rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/parameter-databases/c2000-sine.5.24.R.C2000-foc.json
--rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/parameter-databases/stm32-sine.5.24.R-foc.json
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/parameter-databases/stm32-sine.5.24.R-sine.json
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-24 16:59:17.177675 openinverter-can-tool-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:59:17.173675 openinverter-can-tool-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:59:17.177675 openinverter-can-tool-0.0.7/src/openinverter_can_tool/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15879 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool/fpfloat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool/paramdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:59:17.177675 openinverter-can-tool-0.0.7/src/openinverter_can_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-04-24 16:59:17.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-24 16:59:17.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:59:17.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-24 16:59:17.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-24 16:59:17.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 16:59:17.000000 openinverter-can-tool-0.0.7/src/openinverter_can_tool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:59:17.177675 openinverter-can-tool-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-04-24 16:59:06.000000 openinverter-can-tool-0.0.7/tests/test_paramdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:25.024560 openinverter-can-tool-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-25 17:04:15.000000 openinverter-can-tool-0.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-05-25 17:04:25.024560 openinverter-can-tool-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-05-25 17:04:15.000000 openinverter-can-tool-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:25.020560 openinverter-can-tool-0.0.8/parameter-databases/
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-05-25 17:04:15.000000 openinverter-can-tool-0.0.8/parameter-databases/c2000-sine.5.14.R.C2000-foc.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-05-25 17:04:15.000000 openinverter-can-tool-0.0.8/parameter-databases/c2000-sine.5.24.R.C2000-foc.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-05-25 17:04:15.000000 openinverter-can-tool-0.0.8/parameter-databases/stm32-sine.5.24.R-foc.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-05-25 17:04:15.000000 openinverter-can-tool-0.0.8/parameter-databases/stm32-sine.5.24.R-sine.json
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-25 17:04:15.000000 openinverter-can-tool-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 17:04:25.024560 openinverter-can-tool-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-25 17:04:15.000000 openinverter-can-tool-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:25.020560 openinverter-can-tool-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:25.024560 openinverter-can-tool-0.0.8/src/openinverter_can_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:15.000000 openinverter-can-tool-0.0.8/src/openinverter_can_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-25 17:04:15.000000 openinverter-can-tool-0.0.8/src/openinverter_can_tool/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19133 2023-05-25 17:04:15.000000 openinverter-can-tool-0.0.8/src/openinverter_can_tool/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-25 17:04:15.000000 openinverter-can-tool-0.0.8/src/openinverter_can_tool/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-25 17:04:15.000000 openinverter-can-tool-0.0.8/src/openinverter_can_tool/fpfloat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-05-25 17:04:15.000000 openinverter-can-tool-0.0.8/src/openinverter_can_tool/paramdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:25.024560 openinverter-can-tool-0.0.8/src/openinverter_can_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-05-25 17:04:25.000000 openinverter-can-tool-0.0.8/src/openinverter_can_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-25 17:04:25.000000 openinverter-can-tool-0.0.8/src/openinverter_can_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:04:25.000000 openinverter-can-tool-0.0.8/src/openinverter_can_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-25 17:04:25.000000 openinverter-can-tool-0.0.8/src/openinverter_can_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-25 17:04:25.000000 openinverter-can-tool-0.0.8/src/openinverter_can_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 17:04:25.000000 openinverter-can-tool-0.0.8/src/openinverter_can_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:04:25.024560 openinverter-can-tool-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-05-25 17:04:15.000000 openinverter-can-tool-0.0.8/tests/test_paramdb.py
```

### Comparing `openinverter-can-tool-0.0.7/LICENSE.txt` & `openinverter-can-tool-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openinverter-can-tool-0.0.7/PKG-INFO` & `openinverter-can-tool-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openinverter-can-tool
-Version: 0.0.7
+Version: 0.0.8
 Summary: Tool to configure and operate openinverter systems over CAN
 Home-page: https://github.com/davefiddes/openinverter-can-tool
 Author: David J. Fiddes
 Author-email: D.J@fiddes.net
 Project-URL: Bug Reports, https://github.com/davefiddes/openinverter-can-tool/issues
 Project-URL: Source, https://github.com/davefiddes/openinverter-can-tool
 Keywords: openinverter,canopen
@@ -47,15 +47,15 @@
   * Save parameters to flash
   * Revert parameters to their default values
   * Reset
 * Scan a CAN bus for possible nodes
 * Runs on Linux, Windows and MacOS with python 3.7+
 * Works with any CAN adapter supported by [python-can](https://pypi.org/project/python-can/)
 * Supports [stm32-sine](https://github.com/jsphuebner/stm32-sine) 5.24.R or later
-* Automatic parameter database download requires stm32-sine 5.25.R or later
+* Automatic parameter database download and caching (requires stm32-sine development branch - likely 5.27.R or later)
 
 ## Installation
 
 The most recent release may be installed using pip:
 
 ```text
     pip install openinverter_can_tool
@@ -72,21 +72,21 @@
 ### Linux
 
 Linux users may reduce the potential of package conflicts by installing python dependencies from their package manager. This should be done before running `pip`.
 
 #### Fedora
 
 ```text
-    sudo dnf install python3-setuptools python3-pip python3-click python3-can
+    sudo dnf install python3-setuptools python3-pip python3-click python3-can python3-appdirs
 ```
 
 #### Ubuntu/Debian
 
 ```text
-    sudo apt install python3-setuptools python3-pip python3-click python3-can
+    sudo apt install python3-setuptools python3-pip python3-click python3-can python3-appsdirs
 ```
 
 ## Configuration
 
 Before the tool can be used the CAN interface adapter needs to be configured. To do this create `~/.canrc` on Linux or `%USERPROFILE%/can.conf` on Windows. Details on interfaces supported and the configuration file format can be found in the [python-can](https://python-can.readthedocs.io/en/stable/installation.html) documentation.
 
 An example configuration file for a [SocketCAN](https://python-can.readthedocs.io/en/stable/interfaces/socketcan.html) compatible adapter on Linux would look like:
@@ -138,14 +138,15 @@
       -c, --context TEXT   Which python-can configuration context to use
       -n, --node INTEGER   The CAN SDO node ID to communicate with  [default: 1]
       -t, --timeout FLOAT  Response timeout in seconds  [default: 1.0]
       --version            Show the version and exit.
       --help               Show this message and exit.
 
     Commands:
+      cache       Parameter database cache management commands
       cmd         Execute a command on a device
       dumpall     Dump the values of all available parameters and values
       listparams  List all available parameters and values
       load        Load all parameters from json IN_FILE
       log         Log the value of PARAMS from the device periodically in CSV...
       read        Read the value of PARAM from the device
       save        Save all parameters in json to OUT_FILE
@@ -157,20 +158,29 @@
 To read a specific parameter from 5.24.R firmware:
 
 ```text
     $ oic -d parameter-databases/stm32-sine.5.24.R-foc.json read brakeregen
     brakeregen: -13 [%]
 ```
 
-To write a new value to a parameter with 5.25.R or later firmware with automatic database download:
+To write a new value to a parameter with 5.27.R or later firmware with automatic database download:
 
 ```text
     oic write brakeregen -30.5
 ```
 
+Values may be changed using symbolic names:
+
+```text
+    oic write potmode DualChannel
+    oic write pinswap PWMOutput13,PWMOutput23
+```
+
+The list of allowed values for a given parameter can be found using the `listparams` command.
+
 ## Development
 
 If you want to be able to change the code while using it, clone it then install
 it in development mode:
 
 ```text
     git clone https://github.com/davefiddes/openinverter_can_tool.git
```

### Comparing `openinverter-can-tool-0.0.7/README.md` & `openinverter-can-tool-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   * Save parameters to flash
   * Revert parameters to their default values
   * Reset
 * Scan a CAN bus for possible nodes
 * Runs on Linux, Windows and MacOS with python 3.7+
 * Works with any CAN adapter supported by [python-can](https://pypi.org/project/python-can/)
 * Supports [stm32-sine](https://github.com/jsphuebner/stm32-sine) 5.24.R or later
-* Automatic parameter database download requires stm32-sine 5.25.R or later
+* Automatic parameter database download and caching (requires stm32-sine development branch - likely 5.27.R or later)
 
 ## Installation
 
 The most recent release may be installed using pip:
 
 ```text
     pip install openinverter_can_tool
@@ -46,21 +46,21 @@
 ### Linux
 
 Linux users may reduce the potential of package conflicts by installing python dependencies from their package manager. This should be done before running `pip`.
 
 #### Fedora
 
 ```text
-    sudo dnf install python3-setuptools python3-pip python3-click python3-can
+    sudo dnf install python3-setuptools python3-pip python3-click python3-can python3-appdirs
 ```
 
 #### Ubuntu/Debian
 
 ```text
-    sudo apt install python3-setuptools python3-pip python3-click python3-can
+    sudo apt install python3-setuptools python3-pip python3-click python3-can python3-appsdirs
 ```
 
 ## Configuration
 
 Before the tool can be used the CAN interface adapter needs to be configured. To do this create `~/.canrc` on Linux or `%USERPROFILE%/can.conf` on Windows. Details on interfaces supported and the configuration file format can be found in the [python-can](https://python-can.readthedocs.io/en/stable/installation.html) documentation.
 
 An example configuration file for a [SocketCAN](https://python-can.readthedocs.io/en/stable/interfaces/socketcan.html) compatible adapter on Linux would look like:
@@ -112,14 +112,15 @@
       -c, --context TEXT   Which python-can configuration context to use
       -n, --node INTEGER   The CAN SDO node ID to communicate with  [default: 1]
       -t, --timeout FLOAT  Response timeout in seconds  [default: 1.0]
       --version            Show the version and exit.
       --help               Show this message and exit.
 
     Commands:
+      cache       Parameter database cache management commands
       cmd         Execute a command on a device
       dumpall     Dump the values of all available parameters and values
       listparams  List all available parameters and values
       load        Load all parameters from json IN_FILE
       log         Log the value of PARAMS from the device periodically in CSV...
       read        Read the value of PARAM from the device
       save        Save all parameters in json to OUT_FILE
@@ -131,20 +132,29 @@
 To read a specific parameter from 5.24.R firmware:
 
 ```text
     $ oic -d parameter-databases/stm32-sine.5.24.R-foc.json read brakeregen
     brakeregen: -13 [%]
 ```
 
-To write a new value to a parameter with 5.25.R or later firmware with automatic database download:
+To write a new value to a parameter with 5.27.R or later firmware with automatic database download:
 
 ```text
     oic write brakeregen -30.5
 ```
 
+Values may be changed using symbolic names:
+
+```text
+    oic write potmode DualChannel
+    oic write pinswap PWMOutput13,PWMOutput23
+```
+
+The list of allowed values for a given parameter can be found using the `listparams` command.
+
 ## Development
 
 If you want to be able to change the code while using it, clone it then install
 it in development mode:
 
 ```text
     git clone https://github.com/davefiddes/openinverter_can_tool.git
```

### Comparing `openinverter-can-tool-0.0.7/parameter-databases/c2000-sine.5.14.R.C2000-foc.json` & `openinverter-can-tool-0.0.8/parameter-databases/c2000-sine.5.14.R.C2000-foc.json`

 * *Files identical despite different names*

### Comparing `openinverter-can-tool-0.0.7/parameter-databases/c2000-sine.5.24.R.C2000-foc.json` & `openinverter-can-tool-0.0.8/parameter-databases/c2000-sine.5.24.R.C2000-foc.json`

 * *Files identical despite different names*

### Comparing `openinverter-can-tool-0.0.7/parameter-databases/stm32-sine.5.24.R-foc.json` & `openinverter-can-tool-0.0.8/parameter-databases/stm32-sine.5.24.R-foc.json`

 * *Files identical despite different names*

### Comparing `openinverter-can-tool-0.0.7/parameter-databases/stm32-sine.5.24.R-sine.json` & `openinverter-can-tool-0.0.8/parameter-databases/stm32-sine.5.24.R-sine.json`

 * *Files identical despite different names*

### Comparing `openinverter-can-tool-0.0.7/setup.py` & `openinverter-can-tool-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Strip the build status as this only makes sense on github
 long_description = re.sub(r'\[!\[Build status.*\)\n\n', '', long_description)
 
 setup(
     name="openinverter-can-tool",
-    version="0.0.7",
+    version="0.0.8",
     description="Tool to configure and operate openinverter systems over CAN",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/davefiddes/openinverter-can-tool",
     author="David J. Fiddes",
     author_email="D.J@fiddes.net",
 
@@ -46,15 +46,15 @@
 
     keywords="openinverter, canopen",
 
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     python_requires=">=3.7, <4",
 
-    install_requires=["click", "canopen"],
+    install_requires=["click", "canopen", "appdirs"],
     extras_require={
         "dev": ["check-manifest", "flake8"],
         "test": ["coverage", "pytest"],
     },
 
     # No data files are expected within the package
     package_data={},
```

### Comparing `openinverter-can-tool-0.0.7/src/openinverter_can_tool/cli.py` & `openinverter-can-tool-0.0.8/src/openinverter_can_tool/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """
 openinverter CAN Tools main program
 """
 
 import functools
-from typing import Optional
+from typing import Optional, Union
 import json
 import csv
 import time
 import datetime
+import glob
+import os
 import click
 import can
 import canopen
-from .paramdb import import_database, import_remote_database
+import appdirs
+from .paramdb import import_database, import_cached_database
 from .fpfloat import fixed_to_float, fixed_from_float
 from . import constants as oi
 
 
 class CliSettings:
     """Simple class to store the common settings used for all commands"""
 
@@ -24,17 +27,17 @@
             database_path: str,
             context: str,
             node_number: int,
             timeout: float) -> None:
         self.database_path = database_path
         self.context = context
         self.node_number = node_number
-        self.network = Optional[canopen.Network]
+        self.network: Optional[canopen.Network] = None
         self.database = canopen.objectdictionary.ObjectDictionary()
-        self.node = Optional[canopen.Node]
+        self.node: Optional[canopen.Node] = None
         self.timeout = timeout
 
 
 pass_cli_settings = click.make_pass_decorator(CliSettings)
 
 
 def db_action(func):
@@ -47,23 +50,26 @@
 
         # Assume that the first argument exists and is a CliSettings
         cli_settings: CliSettings = args[0]
 
         if cli_settings.database_path:
             device_db = import_database(cli_settings.database_path)
         else:
+            network = None
             try:
                 # Fire up the CAN network just to grab the node parameter
                 # database from the device
                 network = canopen.Network()
                 network.connect(context=cli_settings.context)
                 network.check()
 
-                device_db = import_remote_database(
-                    network, cli_settings.node_number)
+                device_db = import_cached_database(
+                    network,
+                    cli_settings.node_number,
+                    appdirs.user_cache_dir(oi.APPNAME, oi.APPAUTHOR))
             finally:
                 if network:
                     network.disconnect()
 
         cli_settings.database = device_db
 
         # Call the command handler function
@@ -81,14 +87,15 @@
 
         # Assume that the first argument exists and is a CliSettings
         cli_settings: CliSettings = args[0]
 
         # Ensure we always have something to return
         return_value = None
 
+        network = None
         try:
             # Start with creating a network representing one CAN bus
             network = canopen.Network()
 
             # Connect to the CAN bus
             network.connect(context=cli_settings.context)
 
@@ -147,25 +154,29 @@
 @click.option("-t", "--timeout",
               default=1.0,
               show_default=True,
               type=click.FLOAT,
               help="Response timeout in seconds")
 @click.version_option()
 @click.pass_context
-def cli(ctx, database, context, node, timeout):
+def cli(ctx: click.Context,
+        database: str,
+        context: str,
+        node: int,
+        timeout: float) -> None:
     """openinverter CAN Tool allows querying and setting configuration of
     inverter parameters over a CAN connection"""
 
     ctx.obj = CliSettings(database, context, node, timeout)
 
 
 @cli.command()
 @pass_cli_settings
 @db_action
-def listparams(cli_settings: CliSettings):
+def listparams(cli_settings: CliSettings) -> None:
     """List all available parameters and values"""
     for item in cli_settings.database.names.values():
         print(
             f"{item.name} [{item.unit}]", end="")
 
         if item.isparam:
             print(
@@ -174,15 +185,15 @@
                 f"default: {fixed_to_float(item.default):g}")
         else:
             print(" - read-only value")
 
 
 def print_param(
         variable: canopen.objectdictionary.Variable,
-        value: float) -> str:
+        value: float) -> None:
     """Print out the value of a parameter or outputs the enumeration value or
     bits in a bitfield"""
 
     click.echo(f"{variable.name:20}: ", nl=False)
 
     if variable.value_descriptions:
         if value in variable.value_descriptions:
@@ -206,28 +217,28 @@
             f"{value:g} [{variable.unit}]")
 
 
 @cli.command()
 @pass_cli_settings
 @db_action
 @can_action
-def dumpall(cli_settings: CliSettings):
+def dumpall(cli_settings: CliSettings) -> None:
     """Dump the values of all available parameters and values"""
 
     node = cli_settings.node
     for item in cli_settings.database.names.values():
         print_param(item, fixed_to_float(node.sdo[item.name].raw))
 
 
 @cli.command()
 @click.argument("param", required=True)
 @pass_cli_settings
 @db_action
 @can_action
-def read(cli_settings: CliSettings, param: str):
+def read(cli_settings: CliSettings, param: str) -> None:
     """Read the value of PARAM from the device"""
 
     if param in cli_settings.database.names:
         node = cli_settings.node
         print_param(
             cli_settings.database.names[param],
             fixed_to_float(node.sdo[param].raw))
@@ -250,15 +261,15 @@
 @pass_cli_settings
 @db_action
 @can_action
 def log(cli_settings: CliSettings,
         params: tuple,
         out_file: click.File,
         step: int,
-        timestamp: bool):
+        timestamp: bool) -> None:
     """Log the value of PARAMS from the device periodically in CSV
     format. Multiple parameters may be specified separated by a space.
     OUT_FILE may be a filename or - to output to stdout."""
 
     # Validate the list of supplied parameters
     query_list = []
     for param in params:
@@ -292,15 +303,15 @@
 
 
 @cli.command()
 @click.argument("out_file", type=click.File("w"))
 @pass_cli_settings
 @db_action
 @can_action
-def save(cli_settings: CliSettings, out_file: click.File):
+def save(cli_settings: CliSettings, out_file: click.File) -> None:
     """Save all parameters in json to OUT_FILE"""
 
     doc = {}
     count = 0
     node = cli_settings.node
     for item in cli_settings.database.names.values():
         if item.isparam:
@@ -308,61 +319,126 @@
             count += 1
 
     json.dump(doc, out_file, indent=4)
 
     click.echo(f"Saved {count} parameters")
 
 
-def write_impl(cli_settings: CliSettings, param: str, value: float):
+def set_enum_value(
+        node: canopen.Node,
+        param: canopen.objectdictionary.Variable,
+        value: str) -> None:
+    """Set a enumeration parameter over SDO by looking up its symbolic value"""
+
+    result = None
+    for key, description in param.value_descriptions.items():
+        if description.lower() == value.lower():
+            result = key
+
+    if result is not None:
+        node.sdo[param.name].raw = fixed_from_float(result)
+    else:
+        click.echo(f"Unable to find value: '{value}' for parameter: "
+                   f"{param.name}. Valid values are "
+                   f"{param.value_descriptions}")
+
+
+def set_bitfield_value(
+        node: canopen.Node,
+        param: canopen.objectdictionary.Variable,
+        value: str) -> None:
+    """Set a bitfield parameter over SDO by looking up its symbolic values. The
+      value should be a comma separated list"""
+
+    result = 0
+    for bit_name in value.split(','):
+        bit_name = bit_name.strip()
+        for key, description in param.bit_definitions.items():
+            if description.lower() == bit_name.lower():
+                result |= key
+
+    node.sdo[param.name].raw = fixed_from_float(result)
+
+
+def set_float_value(
+        node: canopen.Node,
+        param: canopen.objectdictionary.Variable,
+        value: float) -> None:
+    """Set a parameter with a floating point value over SDO"""
+
+    fixed_value = fixed_from_float(value)
+
+    if fixed_value < param.min:
+        click.echo(f"Value {value:g} is smaller than the minimum "
+                   f"value {fixed_to_float(param.min):g} allowed "
+                   f"for {param.name}")
+    elif fixed_value > param.max:
+        click.echo(f"Value {value:g} is larger than the maximum value "
+                   f"{fixed_to_float(param.max):g} allowed for "
+                   f"{param.name}")
+    else:
+        node.sdo[param.name].raw = fixed_value
+
+
+def write_impl(
+        cli_settings: CliSettings,
+        param: str,
+        value: Union[float, str]) -> None:
     """Implementation of the single parameter write command. Separated from
     the command so the logic can be shared with loading all parameters from
     json."""
 
     if param in cli_settings.database.names:
         param_item = cli_settings.database.names[param]
 
         # Check if we are a modifiable parameter
         if param_item.isparam:
-            fixed_value = fixed_from_float(value)
-
-            if fixed_value < param_item.min:
-                click.echo(f"Value {value:g} is smaller than the minimum "
-                           f"value {fixed_to_float(param_item.min):g} allowed "
-                           f"for {param}")
-            elif fixed_value > param_item.max:
-                click.echo(f"Value {value:g} is larger than the maximum value "
-                           f"{fixed_to_float(param_item.max):g} allowed for "
-                           f"{param}")
+            if isinstance(value, float):
+                set_float_value(cli_settings.node, param_item, value)
             else:
-                cli_settings.node.sdo[param].raw = fixed_value
+                # Assume the value is a float to start with
+                try:
+                    set_float_value(
+                        cli_settings.node,
+                        param_item,
+                        float(value))
+                except ValueError:
+                    if param_item.value_descriptions:
+                        set_enum_value(cli_settings.node, param_item, value)
+                    elif param_item.bit_definitions:
+                        set_bitfield_value(
+                            cli_settings.node, param_item, value)
+                    else:
+                        click.echo(f"Invalid value: '{value}' for parameter: "
+                                   f"{param}")
         else:
             click.echo(f"{param} is a spot value parameter. "
                        "Spot values are read-only.")
     else:
         click.echo(f"Unknown parameter: {param}")
 
 
 @cli.command(context_settings=dict(ignore_unknown_options=True))
 @click.argument("param")
-@click.argument("value", type=float)
+@click.argument("value")
 @pass_cli_settings
 @db_action
 @can_action
-def write(cli_settings: CliSettings, param: str, value: float):
+def write(cli_settings: CliSettings, param: str, value: str) -> None:
     """Write the value to the parameter PARAM on the device"""
 
     write_impl(cli_settings, param, value)
 
 
 @cli.command()
 @click.argument("in_file", type=click.File("r"))
 @pass_cli_settings
 @db_action
 @can_action
-def load(cli_settings: CliSettings, in_file: click.File):
+def load(cli_settings: CliSettings, in_file: click.File) -> None:
     """Load all parameters from json IN_FILE"""
 
     doc = json.load(in_file)
     count = 0
     for param_name in doc:
         value = doc[param_name]
 
@@ -376,15 +452,15 @@
 
     click.echo(f"Loaded {count} parameters")
 
 
 @cli.command()
 @pass_cli_settings
 @can_action
-def serialno(cli_settings: CliSettings):
+def serialno(cli_settings: CliSettings) -> None:
     """Read the device serial number. This is required to load firmware over
     CAN"""
 
     # Fetch the serial number in 3 parts reversing from little-endian on the
     # wire into a reversed array where the LSB is first and MSB is last. This
     # is odd but mirrors the behaviour of the STM32 terminal "serial" command
     # for consistency.
@@ -396,15 +472,15 @@
     # Print out the serial number array
     serialno_str = "".join(format(x, "02x") for x in serialno_data)
     click.echo(f"Serial Number: {serialno_str}")
 
 
 @cli.group()
 @pass_cli_settings
-def cmd(cli_settings: CliSettings):
+def cmd(cli_settings: CliSettings) -> None:
     """Execute a command on a device"""
     # We have to have cli_settings to allow the command hierarchy to work but
     # it is unused here so just pretend to use it
     _ = cli_settings
 
 
 def send_command(
@@ -422,47 +498,47 @@
     cli_settings.node.sdo["command"].raw = arg
     click.echo("Command sent successfully")
 
 
 @cmd.command("save")
 @pass_cli_settings
 @can_action
-def cmd_save(cli_settings: CliSettings):
+def cmd_save(cli_settings: CliSettings) -> None:
     """Save device parameters and CAN map to flash"""
     send_command(cli_settings, oi.SAVE_COMMAND_SUBINDEX)
 
 
 @cmd.command("load")
 @pass_cli_settings
 @can_action
-def cmd_load(cli_settings: CliSettings):
+def cmd_load(cli_settings: CliSettings) -> None:
     """Load device parameters and CAN map from flash"""
     send_command(cli_settings, oi.LOAD_COMMAND_SUBINDEX)
 
 
 @cmd.command("reset")
 @pass_cli_settings
 @can_action
-def cmd_reset(cli_settings: CliSettings):
+def cmd_reset(cli_settings: CliSettings) -> None:
     """Reset the device"""
     send_command(cli_settings, oi.RESET_COMMAND_SUBINDEX)
 
 
 @cmd.command("defaults")
 @pass_cli_settings
 @can_action
-def cmd_defaults(cli_settings: CliSettings):
+def cmd_defaults(cli_settings: CliSettings) -> None:
     """Reset the device parameters to their built-in defaults"""
     send_command(cli_settings, oi.DEFAULTS_COMMAND_SUBINDEX)
 
 
 @cmd.command("stop")
 @pass_cli_settings
 @can_action
-def cmd_stop(cli_settings: CliSettings):
+def cmd_stop(cli_settings: CliSettings) -> None:
     """Stop the device from operating"""
     send_command(cli_settings, oi.STOP_COMMAND_SUBINDEX)
 
 
 @cmd.command("start")
 @click.option("--mode",
               type=click.Choice(["Normal",
@@ -472,15 +548,15 @@
                                  "ACHeat",
                                  "Sine"],
                                 case_sensitive=False),
               default="Normal",
               show_default=True)
 @pass_cli_settings
 @can_action
-def cmd_start(cli_settings: CliSettings, mode):
+def cmd_start(cli_settings: CliSettings, mode: str) -> None:
     """Start the device in the specified mode"""
     mode_list = {
         "Normal": oi.START_MODE_NORMAL,
         "Manual": oi.START_MODE_MANUAL,
         "Boost": oi.START_MODE_BOOST,
         "Buck": oi.START_MODE_BUCK,
         "Sine": oi.START_MODE_SINE,
@@ -489,15 +565,15 @@
 
     send_command(cli_settings, oi.START_COMMAND_SUBINDEX, mode_list[mode])
 
 
 @cli.command()
 @pass_cli_settings
 @can_action
-def scan(cli_settings: CliSettings):
+def scan(cli_settings: CliSettings) -> None:
     """Scan the CAN bus for available nodes"""
 
     # Maximum number of devices we are going to scan for
     limit = 20
 
     # Actively scan the bus for SDO nodes which might indicate something we
     # can talk to
@@ -511,7 +587,31 @@
     node_list = [id for id in cli_settings.network.scanner.nodes if id < limit]
 
     if node_list:
         for node_id in node_list:
             click.echo(f"Found possible openinverter node: {node_id}")
     else:
         click.echo("No nodes found")
+
+
+@cli.group()
+@pass_cli_settings
+def cache(cli_settings: CliSettings) -> None:
+    """Parameter database cache management commands"""
+    # We have to have cli_settings to allow the command hierarchy to work but
+    # it is unused here so just pretend to use it
+    _ = cli_settings
+
+
+@cache.command("clean")
+@pass_cli_settings
+def cmd_clean(cli_settings: CliSettings) -> None:
+    """Remove all entries from the parameter database cache"""
+
+    # cli_settings is unused
+    _ = cli_settings
+
+    for file in glob.glob(
+            os.path.join(
+                appdirs.user_cache_dir(oi.APPNAME, oi.APPAUTHOR), "*.json")):
+        click.echo(f"Removing {file}")
+        os.remove(file)
```

### Comparing `openinverter-can-tool-0.0.7/src/openinverter_can_tool/constants.py` & `openinverter-can-tool-0.0.8/src/openinverter_can_tool/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """Useful constants"""
 
 # CANopen SDO indexes used by openinverter systems
 
 # Index for unique serial numbers
 SERIALNO_INDEX = 0x5000
 
+# Parameter database checksum
+PARAM_DB_CHECKSUM_SUBINDEX = 3
+
 # Index for long segmented strings
 STRINGS_INDEX = 0x5001
 
 # CANopen SDO subindex for JSON parameter databases. Used with STRINGS_INDEX
 PARAM_DB_SUBINDEX = 0
 
 # Index for sending commands - somewhat abusing the SDO protocol
@@ -27,7 +30,11 @@
 START_MODE_BOOST = 3
 START_MODE_BUCK = 4
 START_MODE_SINE = 5
 START_MODE_ACHEAT = 6
 
 # SDO abort error codes - Not defined by canopen for some reason
 SDO_ABORT_OBJECT_NOT_AVAILABLE = 0x06020000
+
+# Names for common directories
+APPNAME = "openinverter_can_tool"
+APPAUTHOR = "openinverter"
```

### Comparing `openinverter-can-tool-0.0.7/src/openinverter_can_tool/paramdb.py` & `openinverter-can-tool-0.0.8/src/openinverter_can_tool/paramdb.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """
 openinverter parameter database functions
 """
 
 
 import json
 from typing import Tuple, Dict
-from canopen import objectdictionary, Network
+import os.path
+import canopen
 from canopen.sdo import SdoClient
 from .fpfloat import fixed_from_float
 from . import constants as oi
 
 
 def index_from_id(param_identifier: int) -> Tuple[int, int]:
     """Generate an index, subindex tuple from an openinverter parameter id"""
     index = 0x2100 | (param_identifier >> 8)
     subindex = param_identifier & 0xFF
     return (index, subindex)
 
 
-def is_power_of_two(num):
+def is_power_of_two(num: int) -> bool:
     """Use some clever bitwise anding and arithmetic to determine wether a
     number is a power of two"""
     return (num != 0) and (num & (num - 1) == 0)
 
 
 def is_bitfield(values: Dict[int, str]) -> bool:
     """Try to figure out if the dictionary of values is a bitfield or an
@@ -38,42 +39,42 @@
     if len(values) <= 3:
         return False
     else:
         return True
 
 
 def import_database_json(
-        paramdb_json: dict) -> objectdictionary.ObjectDictionary:
+        paramdb_json: dict) -> canopen.objectdictionary.ObjectDictionary:
     """Import an openinverter parameter database JSON.
 
     :param paramdb_json:
         A dictionary containing an openinverter parameter database
 
     :returns:
         The Object Dictionary.
     :rtype: canopen.ObjectDictionary
     """
 
-    dictionary = objectdictionary.ObjectDictionary()
+    dictionary = canopen.objectdictionary.ObjectDictionary()
     for param_name in paramdb_json:
         param = paramdb_json[param_name]
 
         # Ignore parameters without unique IDs
         if "id" not in param:
             continue
 
         (index, subindex) = index_from_id(int(param["id"]))
-        var = objectdictionary.Variable(param_name, index, subindex)
+        var = canopen.objectdictionary.Variable(param_name, index, subindex)
 
         # All openinverter params are 32-bit fixed float values
         # we will convert to float on presentation as required
         # but work with them as integers to keep the canopen
         # library happy
         var.factor = 32
-        var.data_type = objectdictionary.INTEGER32
+        var.data_type = canopen.objectdictionary.INTEGER32
 
         # Common attributes for parameters and values
         # "isparam" and "category" are not normal member variables in the
         # objectdictionary.Variable class. We add them here.
         var.unit = param["unit"]
         var.isparam = param["isparam"]
 
@@ -109,15 +110,15 @@
             var.default = fixed_from_float(float(param["default"]))
 
         dictionary.add_object(var)
 
     return dictionary
 
 
-def import_database(paramdb: str) -> objectdictionary.ObjectDictionary:
+def import_database(paramdb: str) -> canopen.objectdictionary.ObjectDictionary:
     """Import an openinverter parameter database file.
 
     :param paramdb:
         A path to an openinverter parameter database file
 
     :returns:
         The Object Dictionary.
@@ -127,16 +128,16 @@
     with open(paramdb, encoding="utf-8") as file:
         doc = json.load(file)
 
     return import_database_json(doc)
 
 
 def import_remote_database(
-        network: Network,
-        node_id: int) -> objectdictionary.ObjectDictionary:
+        network: canopen.Network,
+        node_id: int) -> canopen.objectdictionary.ObjectDictionary:
     """Import an openinverter parameter database from a remote node.
 
     :param network:
         The configured and started canopen.Network to use to communicate with
         the node.
 
     :param node_id:
@@ -144,22 +145,90 @@
 
     :returns:
         The Object Dictionary.
     :rtype: canopen.ObjectDictionary
     """
 
     # Create temporary SDO client and attach to the network
-    sdo_client = SdoClient(0x600 + node_id, 0x580 + node_id,
-                           objectdictionary.ObjectDictionary())
+    sdo_client = SdoClient(0x600 + node_id,
+                           0x580 + node_id,
+                           canopen.objectdictionary.ObjectDictionary())
     sdo_client.network = network
     network.subscribe(0x580 + node_id, sdo_client.on_response)
 
     # Create file like object to load the JSON from the remote
     # openinverter node
     try:
         with sdo_client.open(oi.STRINGS_INDEX, oi.PARAM_DB_SUBINDEX,
                              "rt", encoding="utf-8") as param_db:
             dictionary = import_database_json(json.load(param_db))
     finally:
         network.unsubscribe(0x580 + node_id)
 
     return dictionary
+
+
+def import_cached_database(
+        network: canopen.Network,
+        node_id: int,
+        cache_location: str
+) -> canopen.objectdictionary.ObjectDictionary:
+    """Import an openinverter parameter database from a remote node and cache
+    it for quicker access in future.
+
+    :param network:
+        The configured and started canopen.Network to use to communicate with
+        the node.
+
+    :param node_id:
+        The openinverter node we wish to obtain the parameter database from.
+
+    :param cache_location:
+        A directory containing the parameter database cache.
+
+    :returns:
+        The Object Dictionary.
+
+    :rtype: canopen.ObjectDictionary
+    """
+
+    # Create temporary SDO client and attach to the network
+    temp_dictionary = canopen.objectdictionary.ObjectDictionary()
+    sdo_client = SdoClient(0x600 + node_id, 0x580 + node_id, temp_dictionary)
+    sdo_client.network = network
+    network.subscribe(0x580 + node_id, sdo_client.on_response)
+
+    try:
+        checksum_var = canopen.objectdictionary.Variable(
+            "checksum",
+            oi.SERIALNO_INDEX,
+            oi.PARAM_DB_CHECKSUM_SUBINDEX)
+        checksum_var.data_type = canopen.objectdictionary.UNSIGNED32
+        temp_dictionary.add_object(checksum_var)
+        checksum = sdo_client["checksum"].raw
+
+        if not os.path.exists(cache_location):
+            os.mkdir(cache_location)
+
+        cache_file = os.path.join(
+            cache_location, f"{node_id}-{checksum}.json")
+
+        if os.path.exists(cache_file):
+            dictionary = import_database(cache_file)
+        else:
+            # Create file like object to load the JSON from the remote
+            # openinverter node
+            with sdo_client.open(oi.STRINGS_INDEX,
+                                 oi.PARAM_DB_SUBINDEX,
+                                 "rt", encoding="utf-8") as param_db:
+                param_db_str = param_db.read()
+
+            dictionary = import_database_json(json.loads(param_db_str))
+
+            # Only save the database in the cache when we have successfully
+            # imported it
+            with open(cache_file, "wt", encoding="utf-8") as param_db_file:
+                param_db_file.write(param_db_str)
+    finally:
+        network.unsubscribe(0x580 + node_id)
+
+    return dictionary
```

### Comparing `openinverter-can-tool-0.0.7/src/openinverter_can_tool.egg-info/PKG-INFO` & `openinverter-can-tool-0.0.8/src/openinverter_can_tool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openinverter-can-tool
-Version: 0.0.7
+Version: 0.0.8
 Summary: Tool to configure and operate openinverter systems over CAN
 Home-page: https://github.com/davefiddes/openinverter-can-tool
 Author: David J. Fiddes
 Author-email: D.J@fiddes.net
 Project-URL: Bug Reports, https://github.com/davefiddes/openinverter-can-tool/issues
 Project-URL: Source, https://github.com/davefiddes/openinverter-can-tool
 Keywords: openinverter,canopen
@@ -47,15 +47,15 @@
   * Save parameters to flash
   * Revert parameters to their default values
   * Reset
 * Scan a CAN bus for possible nodes
 * Runs on Linux, Windows and MacOS with python 3.7+
 * Works with any CAN adapter supported by [python-can](https://pypi.org/project/python-can/)
 * Supports [stm32-sine](https://github.com/jsphuebner/stm32-sine) 5.24.R or later
-* Automatic parameter database download requires stm32-sine 5.25.R or later
+* Automatic parameter database download and caching (requires stm32-sine development branch - likely 5.27.R or later)
 
 ## Installation
 
 The most recent release may be installed using pip:
 
 ```text
     pip install openinverter_can_tool
@@ -72,21 +72,21 @@
 ### Linux
 
 Linux users may reduce the potential of package conflicts by installing python dependencies from their package manager. This should be done before running `pip`.
 
 #### Fedora
 
 ```text
-    sudo dnf install python3-setuptools python3-pip python3-click python3-can
+    sudo dnf install python3-setuptools python3-pip python3-click python3-can python3-appdirs
 ```
 
 #### Ubuntu/Debian
 
 ```text
-    sudo apt install python3-setuptools python3-pip python3-click python3-can
+    sudo apt install python3-setuptools python3-pip python3-click python3-can python3-appsdirs
 ```
 
 ## Configuration
 
 Before the tool can be used the CAN interface adapter needs to be configured. To do this create `~/.canrc` on Linux or `%USERPROFILE%/can.conf` on Windows. Details on interfaces supported and the configuration file format can be found in the [python-can](https://python-can.readthedocs.io/en/stable/installation.html) documentation.
 
 An example configuration file for a [SocketCAN](https://python-can.readthedocs.io/en/stable/interfaces/socketcan.html) compatible adapter on Linux would look like:
@@ -138,14 +138,15 @@
       -c, --context TEXT   Which python-can configuration context to use
       -n, --node INTEGER   The CAN SDO node ID to communicate with  [default: 1]
       -t, --timeout FLOAT  Response timeout in seconds  [default: 1.0]
       --version            Show the version and exit.
       --help               Show this message and exit.
 
     Commands:
+      cache       Parameter database cache management commands
       cmd         Execute a command on a device
       dumpall     Dump the values of all available parameters and values
       listparams  List all available parameters and values
       load        Load all parameters from json IN_FILE
       log         Log the value of PARAMS from the device periodically in CSV...
       read        Read the value of PARAM from the device
       save        Save all parameters in json to OUT_FILE
@@ -157,20 +158,29 @@
 To read a specific parameter from 5.24.R firmware:
 
 ```text
     $ oic -d parameter-databases/stm32-sine.5.24.R-foc.json read brakeregen
     brakeregen: -13 [%]
 ```
 
-To write a new value to a parameter with 5.25.R or later firmware with automatic database download:
+To write a new value to a parameter with 5.27.R or later firmware with automatic database download:
 
 ```text
     oic write brakeregen -30.5
 ```
 
+Values may be changed using symbolic names:
+
+```text
+    oic write potmode DualChannel
+    oic write pinswap PWMOutput13,PWMOutput23
+```
+
+The list of allowed values for a given parameter can be found using the `listparams` command.
+
 ## Development
 
 If you want to be able to change the code while using it, clone it then install
 it in development mode:
 
 ```text
     git clone https://github.com/davefiddes/openinverter_can_tool.git
```

### Comparing `openinverter-can-tool-0.0.7/src/openinverter_can_tool.egg-info/SOURCES.txt` & `openinverter-can-tool-0.0.8/src/openinverter_can_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openinverter-can-tool-0.0.7/tests/test_paramdb.py` & `openinverter-can-tool-0.0.8/tests/test_paramdb.py`

 * *Files identical despite different names*

