# Comparing `tmp/nxbt-naibaoofficial-1.0.0.tar.gz` & `tmp/nxbt-naibaoofficial-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nxbt-naibaoofficial-1.0.0.tar", last modified: Thu May 25 18:09:46 2023, max compression
+gzip compressed data, was "nxbt-naibaoofficial-1.1.0.tar", last modified: Thu May 25 18:30:20 2023, max compression
```

## Comparing `nxbt-naibaoofficial-1.0.0.tar` & `nxbt-naibaoofficial-1.1.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:09:46.109410 nxbt-naibaoofficial-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      244 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    18568 2023-05-25 18:09:46.113410 nxbt-naibaoofficial-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14869 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:09:46.105410 nxbt-naibaoofficial-1.0.0/nxbt/
--rw-r--r--   0 root         (0) root         (0)      384 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31451 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/bluez.py
--rw-r--r--   0 root         (0) root         (0)    12173 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:09:46.109410 nxbt-naibaoofficial-1.0.0/nxbt/controller/
--rw-r--r--   0 root         (0) root         (0)      232 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/controller/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1966 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/controller/controller.py
--rw-r--r--   0 root         (0) root         (0)    16666 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/controller/input.py
--rw-r--r--   0 root         (0) root         (0)    19312 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/controller/protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:09:46.109410 nxbt-naibaoofficial-1.0.0/nxbt/controller/sdp/
--rw-r--r--   0 root         (0) root         (0)     2529 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/controller/sdp/switch-controller.xml
--rw-r--r--   0 root         (0) root         (0)    18941 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/controller/server.py
--rw-r--r--   0 root         (0) root         (0)     2109 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/controller/utils.py
--rw-r--r--   0 root         (0) root         (0)      871 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/logging.py
--rw-r--r--   0 root         (0) root         (0)    30097 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/nxbt.py
--rw-r--r--   0 root         (0) root         (0)    23474 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/tui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:09:46.109410 nxbt-naibaoofficial-1.0.0/nxbt/web/
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/web/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4503 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/web/app.py
--rw-r--r--   0 root         (0) root         (0)     3685 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/web/cert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:09:46.109410 nxbt-naibaoofficial-1.0.0/nxbt/web/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:09:46.109410 nxbt-naibaoofficial-1.0.0/nxbt/web/static/css/
--rw-r--r--   0 root         (0) root         (0)    11574 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/web/static/css/main.css
--rw-r--r--   0 root         (0) root         (0)    26906 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/web/static/favicon.png
--rw-r--r--   0 root         (0) root         (0)     1519 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/web/static/joyconl.svg
--rw-r--r--   0 root         (0) root         (0)     1614 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/web/static/joyconr.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:09:46.109410 nxbt-naibaoofficial-1.0.0/nxbt/web/static/js/
--rw-r--r--   0 root         (0) root         (0)    20830 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/web/static/js/main.js
--rw-r--r--   0 root         (0) root         (0)    61797 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/web/static/js/socket.io.js
--rw-r--r--   0 root         (0) root         (0)     1888 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/web/static/procon-transparent.svg
--rw-r--r--   0 root         (0) root         (0)     2601 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/web/static/procon.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:09:46.109410 nxbt-naibaoofficial-1.0.0/nxbt/web/templates/
--rw-r--r--   0 root         (0) root         (0)    11614 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/nxbt/web/templates/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:09:46.109410 nxbt-naibaoofficial-1.0.0/nxbt_naibaoofficial.egg-info/
--rw-r--r--   0 root         (0) root         (0)    18568 2023-05-25 18:09:46.000000 nxbt-naibaoofficial-1.0.0/nxbt_naibaoofficial.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      960 2023-05-25 18:09:46.000000 nxbt-naibaoofficial-1.0.0/nxbt_naibaoofficial.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 18:09:46.000000 nxbt-naibaoofficial-1.0.0/nxbt_naibaoofficial.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-25 18:09:46.000000 nxbt-naibaoofficial-1.0.0/nxbt_naibaoofficial.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 18:09:46.000000 nxbt-naibaoofficial-1.0.0/nxbt_naibaoofficial.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      167 2023-05-25 18:09:46.000000 nxbt-naibaoofficial-1.0.0/nxbt_naibaoofficial.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-25 18:09:46.000000 nxbt-naibaoofficial-1.0.0/nxbt_naibaoofficial.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1213 2023-05-25 18:09:46.113410 nxbt-naibaoofficial-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      610 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:30:20.724341 nxbt-naibaoofficial-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      244 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    21574 2023-05-25 18:30:20.724341 nxbt-naibaoofficial-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17291 2023-05-25 18:29:28.000000 nxbt-naibaoofficial-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:30:20.724341 nxbt-naibaoofficial-1.1.0/nxbt/
+-rw-r--r--   0 root         (0) root         (0)      384 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31451 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/bluez.py
+-rw-r--r--   0 root         (0) root         (0)    12173 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:30:20.724341 nxbt-naibaoofficial-1.1.0/nxbt/controller/
+-rw-r--r--   0 root         (0) root         (0)      232 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/controller/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/controller/controller.py
+-rw-r--r--   0 root         (0) root         (0)    16666 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/controller/input.py
+-rw-r--r--   0 root         (0) root         (0)    19312 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/controller/protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:30:20.724341 nxbt-naibaoofficial-1.1.0/nxbt/controller/sdp/
+-rw-r--r--   0 root         (0) root         (0)     2529 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/controller/sdp/switch-controller.xml
+-rw-r--r--   0 root         (0) root         (0)    18941 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/controller/server.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/controller/utils.py
+-rw-r--r--   0 root         (0) root         (0)      871 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/logging.py
+-rw-r--r--   0 root         (0) root         (0)    30097 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/nxbt.py
+-rw-r--r--   0 root         (0) root         (0)    23474 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/tui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:30:20.724341 nxbt-naibaoofficial-1.1.0/nxbt/web/
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/web/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4503 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/web/app.py
+-rw-r--r--   0 root         (0) root         (0)     3685 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/web/cert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:30:20.724341 nxbt-naibaoofficial-1.1.0/nxbt/web/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:30:20.724341 nxbt-naibaoofficial-1.1.0/nxbt/web/static/css/
+-rw-r--r--   0 root         (0) root         (0)    11574 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/web/static/css/main.css
+-rw-r--r--   0 root         (0) root         (0)    26906 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/web/static/favicon.png
+-rw-r--r--   0 root         (0) root         (0)     1519 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/web/static/joyconl.svg
+-rw-r--r--   0 root         (0) root         (0)     1614 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/web/static/joyconr.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:30:20.724341 nxbt-naibaoofficial-1.1.0/nxbt/web/static/js/
+-rw-r--r--   0 root         (0) root         (0)    20830 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/web/static/js/main.js
+-rw-r--r--   0 root         (0) root         (0)    61797 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/web/static/js/socket.io.js
+-rw-r--r--   0 root         (0) root         (0)     1888 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/web/static/procon-transparent.svg
+-rw-r--r--   0 root         (0) root         (0)     2601 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/web/static/procon.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:30:20.724341 nxbt-naibaoofficial-1.1.0/nxbt/web/templates/
+-rw-r--r--   0 root         (0) root         (0)    11614 2023-05-25 18:00:20.000000 nxbt-naibaoofficial-1.1.0/nxbt/web/templates/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:30:20.724341 nxbt-naibaoofficial-1.1.0/nxbt_naibaoofficial.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    21574 2023-05-25 18:30:20.000000 nxbt-naibaoofficial-1.1.0/nxbt_naibaoofficial.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      960 2023-05-25 18:30:20.000000 nxbt-naibaoofficial-1.1.0/nxbt_naibaoofficial.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 18:30:20.000000 nxbt-naibaoofficial-1.1.0/nxbt_naibaoofficial.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-25 18:30:20.000000 nxbt-naibaoofficial-1.1.0/nxbt_naibaoofficial.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 18:09:46.000000 nxbt-naibaoofficial-1.1.0/nxbt_naibaoofficial.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      167 2023-05-25 18:30:20.000000 nxbt-naibaoofficial-1.1.0/nxbt_naibaoofficial.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-25 18:30:20.000000 nxbt-naibaoofficial-1.1.0/nxbt_naibaoofficial.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-05-25 18:30:20.728341 nxbt-naibaoofficial-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      610 2023-05-25 18:29:44.000000 nxbt-naibaoofficial-1.1.0/setup.py
```

### Comparing `nxbt-naibaoofficial-1.0.0/LICENSE` & `nxbt-naibaoofficial-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/PKG-INFO` & `nxbt-naibaoofficial-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nxbt-naibaoofficial
-Version: 1.0.0
+Version: 1.1.0
 Summary: nxbt marco enhanced by naibaooffical
 Home-page: https://pypi.python.org/pypi/nxbt
 Author: Reece Walsh
 Author-email: reece@brikwerk.com
 License: MIT
 Project-URL: Code, https://github.com/Brikwerk/nxbt
 Project-URL: Issue tracker, https://github.com/Brikwerk/nxbt/issues
@@ -32,34 +32,37 @@
           <a href="#installation">Installation</a> •
           <a href="#getting-started">Getting Started</a> •
           <a href="#troubleshooting">Troubleshooting</a> •
           <a href="#credits">Credits</a> •
           <a href="#license">License</a>
         </p>
         
-        ![screenshot](https://raw.githubusercontent.com/Brikwerk/nxbt/master/docs/img/nxbt-example.png)
+        ![screenshot](https://raw.githubusercontent.com/Naibaowjk/nxbt/master/docs/img/nxbt-example.png)
+        
+        ## Important
+        **This program is based on Brikwerk's nxbt project for secondary development, in order to respect the original author, I did not modify all the copyright information in the documentation, only the necessary places to make changes to the documentation.**
         
         ## Key Features
         
         - Use your favourite web browser to control a Nintendo Switch with any keyboard or gamepad.
         - Use your terminal to control a Nintendo Switch with a keyboard.
         - Use a macro from your terminal, browser, or Python script
         - Use the NXBT Python API to write programs to control your Nintendo Switch.
-        - Primitive loop support in macros.
         - In-depth command line interface.
         - Support for emulating multiple controllers at once.
         - Support for fast connection or reconnection to a Nintendo Switch.
         - Emulated ontrollers support thread-safe access.
+        - ** Use macro in loop, support automacic go back to game and press 'YB' together.
         
         ## Installation
         
         ### Linux
         
         ```bash
-        sudo pip3 install nxbt
+        sudo pip3 install nxbt-naibaoofficial
         ```
         
         **Please Note:** NXBT needs root privileges to toggle the BlueZ Input plugin. If you're not comfortable running this program as root, you can disable the Input plugin manually, and install NXBT as a regular user.
         
         ### Windows and macOS
         
         See the installation guide [here.](docs/Windows-and-macOS-Installation.md)
@@ -192,14 +195,84 @@
         
         If you want more information on NXBT's CLI arguments:
         
         ```bash
         sudo nxbt -h
         ```
         
+        Here is my version help info
+        ```bash
+        $ sudo nxbt macro -h
+          -h, --help            show this help message and exit
+          -c COMMANDS, --commands COMMANDS
+                                Used in conjunction with the macro command. Specifies a macro string or a file location to load a macro string from.
+          -r, --reconnect       Used in conjunction with the macro or tui command. If specified, nxbt will attmept to reconnect to any previously connected Nintendo Switch.
+          -a ADDRESS, --address ADDRESS
+                                Used in conjunction with the macro or tui command. If specified, nxbt will attmept to reconnect to a specific Bluetooth MAC address of a Nintendo Switch.
+          -d, --debug           Enables debug mode in nxbt.
+          -l, --logfile         Enables logging to a file in the current working directory instead of stderr.
+          -i IP, --ip IP        Specifies the IP to run the webapp at. Defaults to 0.0.0.0
+          -p PORT, --port PORT  Specifies the port to run the webapp at. Defaults to 8000
+          --usessl              Enables or disables SSL use in the webapp
+          --certpath CERTPATH   Specifies the folder location for SSL certificates used in the webapp. Certificates in this folder should be in the form of a 'cert.pem' and 'key.pem' pair.
+          --repeat REPEAT       Setting repeat times for macro. Defaults to 0, '-1' means forever
+          --commandinit COMMANDINIT
+                                Used in conjunction with the macro command init. Specifies a macro string or a file location to load a macro string from. This co mmand will not repeat, u can use for back game to start macro rightly
+        ```
+        
+        Using macro command to auto go back game and start macro loop:
+        ```bash
+        $ sudo nxbt macro -c "macro-02.txt" --commandinit "macro-init.txt" --repeat -1
+        $ cat macro-init
+        ZR 0.1S
+        0.3S
+        DPAD_UP 0.2S
+        1S
+        PLUS 0.2S
+        0.3S
+        DPAD_LEFT 0.1S
+        0.1S
+        A 0.1S
+        0.1S
+        DPAD_DOWN 0.1S
+        0.1S
+        A 0.1S
+        0.1S
+        DPAD_RIGHT 0.1S
+        0.1S
+        A 0.1S
+        0.1S
+        A 0.1S
+        0.6S
+        PLUS 0.05S
+        0.08S
+        PLUS 0.05S
+        0.3S
+        DPAD_LEFT 0.1S
+        0.2S
+        A 0.1S
+        0.2S
+        DPAD_DOWN 0.1S
+        0.2S
+        A 0.1S
+        0.3S
+        B 0.1S
+        0.3S
+        L_STICK@+000+100 0.1S
+        0.3S
+        A 0.1S
+        0.1S
+        A 0.1S
+        0.1S
+        L_STICK@+000-100 0.1S
+        ```
+        
+        ```
+        
+        
         ### Running Macros with the Python API
         
         Macros are supported with the `macro` function in the Python API. All macros are expected as strings (multiline strings are accepted).
         
         Minimal working example:
         
         ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nxbt-naibaoofficial Version: 1.0.0 Summary: nxbt
+Metadata-Version: 2.1 Name: nxbt-naibaoofficial Version: 1.1.0 Summary: nxbt
 marco enhanced by naibaooffical Home-page: https://pypi.python.org/pypi/nxbt
 Author: Reece Walsh Author-email: reece@brikwerk.com License: MIT Project-URL:
 Code, https://github.com/Brikwerk/nxbt Project-URL: Issue tracker, https://
 github.com/Brikwerk/nxbt/issues Description:
                                     ******
                                     [NXBT]
                                      NXBT
@@ -12,50 +12,55 @@
    Issues](https://img.shields.io/github/issues/brikwerk/nxbt.svg)](https://
       github.com/brikwerk/ctqa/issues) [![GitHub Pull Requests](https://
     img.shields.io/github/issues-pr/brikwerk/nxbt.svg)](https://github.com/
   brikwerk/ctqa/pulls) [![License](https://img.shields.io/badge/license-MIT-
                              blue.svg)](/LICENSE)
    Key_Features â¢ Installation â¢ Getting_Started â¢ Troubleshooting â¢
                               Credits â¢ License
-![screenshot](https://raw.githubusercontent.com/Brikwerk/nxbt/master/docs/img/
-nxbt-example.png) ## Key Features - Use your favourite web browser to control a
-Nintendo Switch with any keyboard or gamepad. - Use your terminal to control a
-Nintendo Switch with a keyboard. - Use a macro from your terminal, browser, or
-Python script - Use the NXBT Python API to write programs to control your
-Nintendo Switch. - Primitive loop support in macros. - In-depth command line
+![screenshot](https://raw.githubusercontent.com/Naibaowjk/nxbt/master/docs/img/
+nxbt-example.png) ## Important **This program is based on Brikwerk's nxbt
+project for secondary development, in order to respect the original author, I
+did not modify all the copyright information in the documentation, only the
+necessary places to make changes to the documentation.** ## Key Features - Use
+your favourite web browser to control a Nintendo Switch with any keyboard or
+gamepad. - Use your terminal to control a Nintendo Switch with a keyboard. -
+Use a macro from your terminal, browser, or Python script - Use the NXBT Python
+API to write programs to control your Nintendo Switch. - In-depth command line
 interface. - Support for emulating multiple controllers at once. - Support for
 fast connection or reconnection to a Nintendo Switch. - Emulated ontrollers
-support thread-safe access. ## Installation ### Linux ```bash sudo pip3 install
-nxbt ``` **Please Note:** NXBT needs root privileges to toggle the BlueZ Input
-plugin. If you're not comfortable running this program as root, you can disable
-the Input plugin manually, and install NXBT as a regular user. ### Windows and
-macOS See the installation guide [here.](docs/Windows-and-macOS-
-Installation.md) ## Getting Started **Note:** If you installed NXBT as a non-
-root user, please omit the use of `sudo` from any of the following commands.
-### Running the demo The demo is meant to gauge whether or not NXBT is working.
-To do so, the demo will create a Pro Controller and run through a small loop of
-commands. **NOTE:** If this is your first time connecting to an NXBT emulated
-controller on the specific host computer, you **MUST** have the "Change Grip/
-Order Menu" open on your Nintendo Switch. You can see how to navigate to the
-"Change Grip/Order Menu" [HERE](docs/img/change-grip-order-menu.png). To start
-the demo, run the following command in your terminal: ```bash sudo nxbt demo
-``` If all is working correctly, the controller should connect, navigate to the
-settings, test the stick calibration, and navigate back to the "Change Grip/
-Order Menu". ## Using the Webapp The NXBT webapp provides a web interface that
-allows for quick creation of a Nintendo Switch controller and use of a keyboard
-or gamepad to control the Nintendo Switch. This lets anyone who can access the
-website control a Nintendo Switch with their favourite keyboard or gamepad. The
-webapp server can be started with the following command: ```bash sudo nxbt
-webapp ``` The above command boots NXBT and an accompanying web server that
-allows for controller creation and use over your web browser. The webapp itself
-will be locally accessible at `http://127.0.0.1:8000` or, if you're on the same
-network as the host computer, http://HOST_COMPUTER_IP:8000. It's also possible
-to expose your NXBT webapp to the internet, however, you'll need to configure a
-reverse proxy, which is out of the scope of this readme. You should see a
-webpage similar to the following image:
+support thread-safe access. - ** Use macro in loop, support automacic go back
+to game and press 'YB' together. ## Installation ### Linux ```bash sudo pip3
+install nxbt-naibaoofficial ``` **Please Note:** NXBT needs root privileges to
+toggle the BlueZ Input plugin. If you're not comfortable running this program
+as root, you can disable the Input plugin manually, and install NXBT as a
+regular user. ### Windows and macOS See the installation guide [here.](docs/
+Windows-and-macOS-Installation.md) ## Getting Started **Note:** If you
+installed NXBT as a non-root user, please omit the use of `sudo` from any of
+the following commands. ### Running the demo The demo is meant to gauge whether
+or not NXBT is working. To do so, the demo will create a Pro Controller and run
+through a small loop of commands. **NOTE:** If this is your first time
+connecting to an NXBT emulated controller on the specific host computer, you
+**MUST** have the "Change Grip/Order Menu" open on your Nintendo Switch. You
+can see how to navigate to the "Change Grip/Order Menu" [HERE](docs/img/change-
+grip-order-menu.png). To start the demo, run the following command in your
+terminal: ```bash sudo nxbt demo ``` If all is working correctly, the
+controller should connect, navigate to the settings, test the stick
+calibration, and navigate back to the "Change Grip/Order Menu". ## Using the
+Webapp The NXBT webapp provides a web interface that allows for quick creation
+of a Nintendo Switch controller and use of a keyboard or gamepad to control the
+Nintendo Switch. This lets anyone who can access the website control a Nintendo
+Switch with their favourite keyboard or gamepad. The webapp server can be
+started with the following command: ```bash sudo nxbt webapp ``` The above
+command boots NXBT and an accompanying web server that allows for controller
+creation and use over your web browser. The webapp itself will be locally
+accessible at `http://127.0.0.1:8000` or, if you're on the same network as the
+host computer, http://HOST_COMPUTER_IP:8000. It's also possible to expose your
+NXBT webapp to the internet, however, you'll need to configure a reverse proxy,
+which is out of the scope of this readme. You should see a webpage similar to
+the following image:
                           [NXBT Webapp Start Screen]
 To create and start a Pro Controller, click the Pro controller graphic. If
 creation/boot is successful, the website will switch to a loading screen.
 During this time, you should have the Nintendo Switch you wish to connect to
 powered on and within range of the host computer. **NOTE:** If this is your
 first time connecting to your Nintendo Switch with the specific host computer,
 make sure you're on the "Change Grip/Order Menu". If you're still unable to
@@ -105,37 +110,63 @@
 commands you would like to run. You'll need to be on the "Change Grip/Order
 Menu" for the above command to work. If you've already connected to the Switch
 on the host computer, you can reconnect and run the macro by adding the `-r` or
 `--reconnect` flag: ```bash sudo nxbt macro -c "B 0.1s\n 0.1s" -r ``` Since it
 can be a little cumbersome typing out a large macro in the terminal, the macro
 command also supports reading from text files instead! commands.txt file: ``` B
 0.1s 0.1s ``` ```bash sudo nxbt macro -c "commands.txt" -r ``` If you want more
-information on NXBT's CLI arguments: ```bash sudo nxbt -h ``` ### Running
-Macros with the Python API Macros are supported with the `macro` function in
-the Python API. All macros are expected as strings (multiline strings are
-accepted). Minimal working example: ```python import nxbt macro = """ B 0.1s
-0.1s """ # Start the NXBT service nx = nxbt.Nxbt() # Create a Pro Controller
-and wait for it to connect controller_index = nx.create_controller
-(nxbt.PRO_CONTROLLER) nx.wait_for_connection(controller_index) # Run a macro on
-the Pro Controller nx.macro(controller_index, macro) ``` The above example uses
-a blocking macro call, however, multiple macros can be queued (or other actions
-taken) with the non-blocking syntax. Queued macros are processed in FIFO
-(First-In-First-Out) order. ```python # Run a macro on the Pro Controller but
-don't block. # In this instance, we record the macro ID so we can keep track of
-its status later on. macro_id = nx.macro(controller_index, macro, block=False)
-from time import sleep while macro_id not in nx.state[controller_index]
-["finished_macros"]: print("Macro hasn't finished") sleep(1/10) print("Macro
-has finished") ``` ## Using the API NXBT provides a Python API for use in
-Python applications or code. If you're someone that learns by example, check
-out the `demo.py` file located at the root of this project. For a more in-depth
-look at all the functionality provided by the API, checkout the `nxbt/nxbt.py`
-file. For those looking to get started with a few simple examples: Read on!
-**Creating a Controller and Waiting for it to Connect** ```python import nxbt #
-Start the NXBT service nx = nxbt.Nxbt() # Create a Pro Controller and wait for
-it to connect controller_index = nx.create_controller(nxbt.PRO_CONTROLLER)
+information on NXBT's CLI arguments: ```bash sudo nxbt -h ``` Here is my
+version help info ```bash $ sudo nxbt macro -h -h, --help show this help
+message and exit -c COMMANDS, --commands COMMANDS Used in conjunction with the
+macro command. Specifies a macro string or a file location to load a macro
+string from. -r, --reconnect Used in conjunction with the macro or tui command.
+If specified, nxbt will attmept to reconnect to any previously connected
+Nintendo Switch. -a ADDRESS, --address ADDRESS Used in conjunction with the
+macro or tui command. If specified, nxbt will attmept to reconnect to a
+specific Bluetooth MAC address of a Nintendo Switch. -d, --debug Enables debug
+mode in nxbt. -l, --logfile Enables logging to a file in the current working
+directory instead of stderr. -i IP, --ip IP Specifies the IP to run the webapp
+at. Defaults to 0.0.0.0 -p PORT, --port PORT Specifies the port to run the
+webapp at. Defaults to 8000 --usessl Enables or disables SSL use in the webapp
+--certpath CERTPATH Specifies the folder location for SSL certificates used in
+the webapp. Certificates in this folder should be in the form of a 'cert.pem'
+and 'key.pem' pair. --repeat REPEAT Setting repeat times for macro. Defaults to
+0, '-1' means forever --commandinit COMMANDINIT Used in conjunction with the
+macro command init. Specifies a macro string or a file location to load a macro
+string from. This co mmand will not repeat, u can use for back game to start
+macro rightly ``` Using macro command to auto go back game and start macro
+loop: ```bash $ sudo nxbt macro -c "macro-02.txt" --commandinit "macro-
+init.txt" --repeat -1 $ cat macro-init ZR 0.1S 0.3S DPAD_UP 0.2S 1S PLUS 0.2S
+0.3S DPAD_LEFT 0.1S 0.1S A 0.1S 0.1S DPAD_DOWN 0.1S 0.1S A 0.1S 0.1S DPAD_RIGHT
+0.1S 0.1S A 0.1S 0.1S A 0.1S 0.6S PLUS 0.05S 0.08S PLUS 0.05S 0.3S DPAD_LEFT
+0.1S 0.2S A 0.1S 0.2S DPAD_DOWN 0.1S 0.2S A 0.1S 0.3S B 0.1S 0.3S
+L_STICK@+000+100 0.1S 0.3S A 0.1S 0.1S A 0.1S 0.1S L_STICK@+000-100 0.1S ```
+``` ### Running Macros with the Python API Macros are supported with the
+`macro` function in the Python API. All macros are expected as strings
+(multiline strings are accepted). Minimal working example: ```python import
+nxbt macro = """ B 0.1s 0.1s """ # Start the NXBT service nx = nxbt.Nxbt() #
+Create a Pro Controller and wait for it to connect controller_index =
+nx.create_controller(nxbt.PRO_CONTROLLER) nx.wait_for_connection
+(controller_index) # Run a macro on the Pro Controller nx.macro
+(controller_index, macro) ``` The above example uses a blocking macro call,
+however, multiple macros can be queued (or other actions taken) with the non-
+blocking syntax. Queued macros are processed in FIFO (First-In-First-Out)
+order. ```python # Run a macro on the Pro Controller but don't block. # In this
+instance, we record the macro ID so we can keep track of its status later on.
+macro_id = nx.macro(controller_index, macro, block=False) from time import
+sleep while macro_id not in nx.state[controller_index]["finished_macros"]:
+print("Macro hasn't finished") sleep(1/10) print("Macro has finished") ``` ##
+Using the API NXBT provides a Python API for use in Python applications or
+code. If you're someone that learns by example, check out the `demo.py` file
+located at the root of this project. For a more in-depth look at all the
+functionality provided by the API, checkout the `nxbt/nxbt.py` file. For those
+looking to get started with a few simple examples: Read on! **Creating a
+Controller and Waiting for it to Connect** ```python import nxbt # Start the
+NXBT service nx = nxbt.Nxbt() # Create a Pro Controller and wait for it to
+connect controller_index = nx.create_controller(nxbt.PRO_CONTROLLER)
 nx.wait_for_connection(controller_index) print("Connected") ``` **Pressing a
 Button** ```python # Press the B button # press_buttons defaults to pressing a
 button for 0.1s and releasing for 0.1s nx.press_buttons(controller_idx,
 [nxbt.Buttons.B]) # Pressing the B button for 1.0s instead of 0.1s
 nx.press_buttons(controller_idx, [nxbt.Buttons.B], down=1.0) ``` **Tilting a
 Analog Stick** ```python # Tilt the right stick fully to the left. # tilt_stick
 defaults to tilting the stick for 0.1s and releasing for 0.1s nx.tilt_stick
```

### Comparing `nxbt-naibaoofficial-1.0.0/README.md` & `nxbt-naibaoofficial-1.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -22,34 +22,37 @@
   <a href="#installation">Installation</a> •
   <a href="#getting-started">Getting Started</a> •
   <a href="#troubleshooting">Troubleshooting</a> •
   <a href="#credits">Credits</a> •
   <a href="#license">License</a>
 </p>
 
-![screenshot](https://raw.githubusercontent.com/Brikwerk/nxbt/master/docs/img/nxbt-example.png)
+![screenshot](https://raw.githubusercontent.com/Naibaowjk/nxbt/master/docs/img/nxbt-example.png)
+
+## Important
+**This program is based on Brikwerk's nxbt project for secondary development, in order to respect the original author, I did not modify all the copyright information in the documentation, only the necessary places to make changes to the documentation.**
 
 ## Key Features
 
 - Use your favourite web browser to control a Nintendo Switch with any keyboard or gamepad.
 - Use your terminal to control a Nintendo Switch with a keyboard.
 - Use a macro from your terminal, browser, or Python script
 - Use the NXBT Python API to write programs to control your Nintendo Switch.
-- Primitive loop support in macros.
 - In-depth command line interface.
 - Support for emulating multiple controllers at once.
 - Support for fast connection or reconnection to a Nintendo Switch.
 - Emulated ontrollers support thread-safe access.
+- ** Use macro in loop, support automacic go back to game and press 'YB' together.
 
 ## Installation
 
 ### Linux
 
 ```bash
-sudo pip3 install nxbt
+sudo pip3 install nxbt-naibaoofficial
 ```
 
 **Please Note:** NXBT needs root privileges to toggle the BlueZ Input plugin. If you're not comfortable running this program as root, you can disable the Input plugin manually, and install NXBT as a regular user.
 
 ### Windows and macOS
 
 See the installation guide [here.](docs/Windows-and-macOS-Installation.md)
@@ -182,14 +185,84 @@
 
 If you want more information on NXBT's CLI arguments:
 
 ```bash
 sudo nxbt -h
 ```
 
+Here is my version help info
+```bash
+$ sudo nxbt macro -h
+  -h, --help            show this help message and exit
+  -c COMMANDS, --commands COMMANDS
+                        Used in conjunction with the macro command. Specifies a macro string or a file location to load a macro string from.
+  -r, --reconnect       Used in conjunction with the macro or tui command. If specified, nxbt will attmept to reconnect to any previously connected Nintendo Switch.
+  -a ADDRESS, --address ADDRESS
+                        Used in conjunction with the macro or tui command. If specified, nxbt will attmept to reconnect to a specific Bluetooth MAC address of a Nintendo Switch.
+  -d, --debug           Enables debug mode in nxbt.
+  -l, --logfile         Enables logging to a file in the current working directory instead of stderr.
+  -i IP, --ip IP        Specifies the IP to run the webapp at. Defaults to 0.0.0.0
+  -p PORT, --port PORT  Specifies the port to run the webapp at. Defaults to 8000
+  --usessl              Enables or disables SSL use in the webapp
+  --certpath CERTPATH   Specifies the folder location for SSL certificates used in the webapp. Certificates in this folder should be in the form of a 'cert.pem' and 'key.pem' pair.
+  --repeat REPEAT       Setting repeat times for macro. Defaults to 0, '-1' means forever
+  --commandinit COMMANDINIT
+                        Used in conjunction with the macro command init. Specifies a macro string or a file location to load a macro string from. This co mmand will not repeat, u can use for back game to start macro rightly
+```
+
+Using macro command to auto go back game and start macro loop:
+```bash
+$ sudo nxbt macro -c "macro-02.txt" --commandinit "macro-init.txt" --repeat -1
+$ cat macro-init
+ZR 0.1S
+0.3S
+DPAD_UP 0.2S
+1S
+PLUS 0.2S
+0.3S
+DPAD_LEFT 0.1S
+0.1S
+A 0.1S
+0.1S
+DPAD_DOWN 0.1S
+0.1S
+A 0.1S
+0.1S
+DPAD_RIGHT 0.1S
+0.1S
+A 0.1S
+0.1S
+A 0.1S
+0.6S
+PLUS 0.05S
+0.08S
+PLUS 0.05S
+0.3S
+DPAD_LEFT 0.1S
+0.2S
+A 0.1S
+0.2S
+DPAD_DOWN 0.1S
+0.2S
+A 0.1S
+0.3S
+B 0.1S
+0.3S
+L_STICK@+000+100 0.1S
+0.3S
+A 0.1S
+0.1S
+A 0.1S
+0.1S
+L_STICK@+000-100 0.1S
+```
+
+```
+
+
 ### Running Macros with the Python API
 
 Macros are supported with the `macro` function in the Python API. All macros are expected as strings (multiline strings are accepted).
 
 Minimal working example:
 
 ```python
```

#### html2text {}

```diff
@@ -7,50 +7,55 @@
    Issues](https://img.shields.io/github/issues/brikwerk/nxbt.svg)](https://
       github.com/brikwerk/ctqa/issues) [![GitHub Pull Requests](https://
     img.shields.io/github/issues-pr/brikwerk/nxbt.svg)](https://github.com/
   brikwerk/ctqa/pulls) [![License](https://img.shields.io/badge/license-MIT-
                              blue.svg)](/LICENSE)
    Key_Features â¢ Installation â¢ Getting_Started â¢ Troubleshooting â¢
                               Credits â¢ License
-![screenshot](https://raw.githubusercontent.com/Brikwerk/nxbt/master/docs/img/
-nxbt-example.png) ## Key Features - Use your favourite web browser to control a
-Nintendo Switch with any keyboard or gamepad. - Use your terminal to control a
-Nintendo Switch with a keyboard. - Use a macro from your terminal, browser, or
-Python script - Use the NXBT Python API to write programs to control your
-Nintendo Switch. - Primitive loop support in macros. - In-depth command line
+![screenshot](https://raw.githubusercontent.com/Naibaowjk/nxbt/master/docs/img/
+nxbt-example.png) ## Important **This program is based on Brikwerk's nxbt
+project for secondary development, in order to respect the original author, I
+did not modify all the copyright information in the documentation, only the
+necessary places to make changes to the documentation.** ## Key Features - Use
+your favourite web browser to control a Nintendo Switch with any keyboard or
+gamepad. - Use your terminal to control a Nintendo Switch with a keyboard. -
+Use a macro from your terminal, browser, or Python script - Use the NXBT Python
+API to write programs to control your Nintendo Switch. - In-depth command line
 interface. - Support for emulating multiple controllers at once. - Support for
 fast connection or reconnection to a Nintendo Switch. - Emulated ontrollers
-support thread-safe access. ## Installation ### Linux ```bash sudo pip3 install
-nxbt ``` **Please Note:** NXBT needs root privileges to toggle the BlueZ Input
-plugin. If you're not comfortable running this program as root, you can disable
-the Input plugin manually, and install NXBT as a regular user. ### Windows and
-macOS See the installation guide [here.](docs/Windows-and-macOS-
-Installation.md) ## Getting Started **Note:** If you installed NXBT as a non-
-root user, please omit the use of `sudo` from any of the following commands.
-### Running the demo The demo is meant to gauge whether or not NXBT is working.
-To do so, the demo will create a Pro Controller and run through a small loop of
-commands. **NOTE:** If this is your first time connecting to an NXBT emulated
-controller on the specific host computer, you **MUST** have the "Change Grip/
-Order Menu" open on your Nintendo Switch. You can see how to navigate to the
-"Change Grip/Order Menu" [HERE](docs/img/change-grip-order-menu.png). To start
-the demo, run the following command in your terminal: ```bash sudo nxbt demo
-``` If all is working correctly, the controller should connect, navigate to the
-settings, test the stick calibration, and navigate back to the "Change Grip/
-Order Menu". ## Using the Webapp The NXBT webapp provides a web interface that
-allows for quick creation of a Nintendo Switch controller and use of a keyboard
-or gamepad to control the Nintendo Switch. This lets anyone who can access the
-website control a Nintendo Switch with their favourite keyboard or gamepad. The
-webapp server can be started with the following command: ```bash sudo nxbt
-webapp ``` The above command boots NXBT and an accompanying web server that
-allows for controller creation and use over your web browser. The webapp itself
-will be locally accessible at `http://127.0.0.1:8000` or, if you're on the same
-network as the host computer, http://HOST_COMPUTER_IP:8000. It's also possible
-to expose your NXBT webapp to the internet, however, you'll need to configure a
-reverse proxy, which is out of the scope of this readme. You should see a
-webpage similar to the following image:
+support thread-safe access. - ** Use macro in loop, support automacic go back
+to game and press 'YB' together. ## Installation ### Linux ```bash sudo pip3
+install nxbt-naibaoofficial ``` **Please Note:** NXBT needs root privileges to
+toggle the BlueZ Input plugin. If you're not comfortable running this program
+as root, you can disable the Input plugin manually, and install NXBT as a
+regular user. ### Windows and macOS See the installation guide [here.](docs/
+Windows-and-macOS-Installation.md) ## Getting Started **Note:** If you
+installed NXBT as a non-root user, please omit the use of `sudo` from any of
+the following commands. ### Running the demo The demo is meant to gauge whether
+or not NXBT is working. To do so, the demo will create a Pro Controller and run
+through a small loop of commands. **NOTE:** If this is your first time
+connecting to an NXBT emulated controller on the specific host computer, you
+**MUST** have the "Change Grip/Order Menu" open on your Nintendo Switch. You
+can see how to navigate to the "Change Grip/Order Menu" [HERE](docs/img/change-
+grip-order-menu.png). To start the demo, run the following command in your
+terminal: ```bash sudo nxbt demo ``` If all is working correctly, the
+controller should connect, navigate to the settings, test the stick
+calibration, and navigate back to the "Change Grip/Order Menu". ## Using the
+Webapp The NXBT webapp provides a web interface that allows for quick creation
+of a Nintendo Switch controller and use of a keyboard or gamepad to control the
+Nintendo Switch. This lets anyone who can access the website control a Nintendo
+Switch with their favourite keyboard or gamepad. The webapp server can be
+started with the following command: ```bash sudo nxbt webapp ``` The above
+command boots NXBT and an accompanying web server that allows for controller
+creation and use over your web browser. The webapp itself will be locally
+accessible at `http://127.0.0.1:8000` or, if you're on the same network as the
+host computer, http://HOST_COMPUTER_IP:8000. It's also possible to expose your
+NXBT webapp to the internet, however, you'll need to configure a reverse proxy,
+which is out of the scope of this readme. You should see a webpage similar to
+the following image:
                           [NXBT Webapp Start Screen]
 To create and start a Pro Controller, click the Pro controller graphic. If
 creation/boot is successful, the website will switch to a loading screen.
 During this time, you should have the Nintendo Switch you wish to connect to
 powered on and within range of the host computer. **NOTE:** If this is your
 first time connecting to your Nintendo Switch with the specific host computer,
 make sure you're on the "Change Grip/Order Menu". If you're still unable to
@@ -100,37 +105,63 @@
 commands you would like to run. You'll need to be on the "Change Grip/Order
 Menu" for the above command to work. If you've already connected to the Switch
 on the host computer, you can reconnect and run the macro by adding the `-r` or
 `--reconnect` flag: ```bash sudo nxbt macro -c "B 0.1s\n 0.1s" -r ``` Since it
 can be a little cumbersome typing out a large macro in the terminal, the macro
 command also supports reading from text files instead! commands.txt file: ``` B
 0.1s 0.1s ``` ```bash sudo nxbt macro -c "commands.txt" -r ``` If you want more
-information on NXBT's CLI arguments: ```bash sudo nxbt -h ``` ### Running
-Macros with the Python API Macros are supported with the `macro` function in
-the Python API. All macros are expected as strings (multiline strings are
-accepted). Minimal working example: ```python import nxbt macro = """ B 0.1s
-0.1s """ # Start the NXBT service nx = nxbt.Nxbt() # Create a Pro Controller
-and wait for it to connect controller_index = nx.create_controller
-(nxbt.PRO_CONTROLLER) nx.wait_for_connection(controller_index) # Run a macro on
-the Pro Controller nx.macro(controller_index, macro) ``` The above example uses
-a blocking macro call, however, multiple macros can be queued (or other actions
-taken) with the non-blocking syntax. Queued macros are processed in FIFO
-(First-In-First-Out) order. ```python # Run a macro on the Pro Controller but
-don't block. # In this instance, we record the macro ID so we can keep track of
-its status later on. macro_id = nx.macro(controller_index, macro, block=False)
-from time import sleep while macro_id not in nx.state[controller_index]
-["finished_macros"]: print("Macro hasn't finished") sleep(1/10) print("Macro
-has finished") ``` ## Using the API NXBT provides a Python API for use in
-Python applications or code. If you're someone that learns by example, check
-out the `demo.py` file located at the root of this project. For a more in-depth
-look at all the functionality provided by the API, checkout the `nxbt/nxbt.py`
-file. For those looking to get started with a few simple examples: Read on!
-**Creating a Controller and Waiting for it to Connect** ```python import nxbt #
-Start the NXBT service nx = nxbt.Nxbt() # Create a Pro Controller and wait for
-it to connect controller_index = nx.create_controller(nxbt.PRO_CONTROLLER)
+information on NXBT's CLI arguments: ```bash sudo nxbt -h ``` Here is my
+version help info ```bash $ sudo nxbt macro -h -h, --help show this help
+message and exit -c COMMANDS, --commands COMMANDS Used in conjunction with the
+macro command. Specifies a macro string or a file location to load a macro
+string from. -r, --reconnect Used in conjunction with the macro or tui command.
+If specified, nxbt will attmept to reconnect to any previously connected
+Nintendo Switch. -a ADDRESS, --address ADDRESS Used in conjunction with the
+macro or tui command. If specified, nxbt will attmept to reconnect to a
+specific Bluetooth MAC address of a Nintendo Switch. -d, --debug Enables debug
+mode in nxbt. -l, --logfile Enables logging to a file in the current working
+directory instead of stderr. -i IP, --ip IP Specifies the IP to run the webapp
+at. Defaults to 0.0.0.0 -p PORT, --port PORT Specifies the port to run the
+webapp at. Defaults to 8000 --usessl Enables or disables SSL use in the webapp
+--certpath CERTPATH Specifies the folder location for SSL certificates used in
+the webapp. Certificates in this folder should be in the form of a 'cert.pem'
+and 'key.pem' pair. --repeat REPEAT Setting repeat times for macro. Defaults to
+0, '-1' means forever --commandinit COMMANDINIT Used in conjunction with the
+macro command init. Specifies a macro string or a file location to load a macro
+string from. This co mmand will not repeat, u can use for back game to start
+macro rightly ``` Using macro command to auto go back game and start macro
+loop: ```bash $ sudo nxbt macro -c "macro-02.txt" --commandinit "macro-
+init.txt" --repeat -1 $ cat macro-init ZR 0.1S 0.3S DPAD_UP 0.2S 1S PLUS 0.2S
+0.3S DPAD_LEFT 0.1S 0.1S A 0.1S 0.1S DPAD_DOWN 0.1S 0.1S A 0.1S 0.1S DPAD_RIGHT
+0.1S 0.1S A 0.1S 0.1S A 0.1S 0.6S PLUS 0.05S 0.08S PLUS 0.05S 0.3S DPAD_LEFT
+0.1S 0.2S A 0.1S 0.2S DPAD_DOWN 0.1S 0.2S A 0.1S 0.3S B 0.1S 0.3S
+L_STICK@+000+100 0.1S 0.3S A 0.1S 0.1S A 0.1S 0.1S L_STICK@+000-100 0.1S ```
+``` ### Running Macros with the Python API Macros are supported with the
+`macro` function in the Python API. All macros are expected as strings
+(multiline strings are accepted). Minimal working example: ```python import
+nxbt macro = """ B 0.1s 0.1s """ # Start the NXBT service nx = nxbt.Nxbt() #
+Create a Pro Controller and wait for it to connect controller_index =
+nx.create_controller(nxbt.PRO_CONTROLLER) nx.wait_for_connection
+(controller_index) # Run a macro on the Pro Controller nx.macro
+(controller_index, macro) ``` The above example uses a blocking macro call,
+however, multiple macros can be queued (or other actions taken) with the non-
+blocking syntax. Queued macros are processed in FIFO (First-In-First-Out)
+order. ```python # Run a macro on the Pro Controller but don't block. # In this
+instance, we record the macro ID so we can keep track of its status later on.
+macro_id = nx.macro(controller_index, macro, block=False) from time import
+sleep while macro_id not in nx.state[controller_index]["finished_macros"]:
+print("Macro hasn't finished") sleep(1/10) print("Macro has finished") ``` ##
+Using the API NXBT provides a Python API for use in Python applications or
+code. If you're someone that learns by example, check out the `demo.py` file
+located at the root of this project. For a more in-depth look at all the
+functionality provided by the API, checkout the `nxbt/nxbt.py` file. For those
+looking to get started with a few simple examples: Read on! **Creating a
+Controller and Waiting for it to Connect** ```python import nxbt # Start the
+NXBT service nx = nxbt.Nxbt() # Create a Pro Controller and wait for it to
+connect controller_index = nx.create_controller(nxbt.PRO_CONTROLLER)
 nx.wait_for_connection(controller_index) print("Connected") ``` **Pressing a
 Button** ```python # Press the B button # press_buttons defaults to pressing a
 button for 0.1s and releasing for 0.1s nx.press_buttons(controller_idx,
 [nxbt.Buttons.B]) # Pressing the B button for 1.0s instead of 0.1s
 nx.press_buttons(controller_idx, [nxbt.Buttons.B], down=1.0) ``` **Tilting a
 Analog Stick** ```python # Tilt the right stick fully to the left. # tilt_stick
 defaults to tilting the stick for 0.1s and releasing for 0.1s nx.tilt_stick
```

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt/bluez.py` & `nxbt-naibaoofficial-1.1.0/nxbt/bluez.py`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt/cli.py` & `nxbt-naibaoofficial-1.1.0/nxbt/cli.py`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt/controller/controller.py` & `nxbt-naibaoofficial-1.1.0/nxbt/controller/controller.py`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt/controller/input.py` & `nxbt-naibaoofficial-1.1.0/nxbt/controller/input.py`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt/controller/protocol.py` & `nxbt-naibaoofficial-1.1.0/nxbt/controller/protocol.py`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt/controller/sdp/switch-controller.xml` & `nxbt-naibaoofficial-1.1.0/nxbt/controller/sdp/switch-controller.xml`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt/controller/server.py` & `nxbt-naibaoofficial-1.1.0/nxbt/controller/server.py`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt/controller/utils.py` & `nxbt-naibaoofficial-1.1.0/nxbt/controller/utils.py`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt/logging.py` & `nxbt-naibaoofficial-1.1.0/nxbt/logging.py`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt/nxbt.py` & `nxbt-naibaoofficial-1.1.0/nxbt/nxbt.py`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt/tui.py` & `nxbt-naibaoofficial-1.1.0/nxbt/tui.py`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt/web/app.py` & `nxbt-naibaoofficial-1.1.0/nxbt/web/app.py`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt/web/cert.py` & `nxbt-naibaoofficial-1.1.0/nxbt/web/cert.py`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt/web/static/css/main.css` & `nxbt-naibaoofficial-1.1.0/nxbt/web/static/css/main.css`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt/web/static/favicon.png` & `nxbt-naibaoofficial-1.1.0/nxbt/web/static/favicon.png`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt/web/static/joyconl.svg` & `nxbt-naibaoofficial-1.1.0/nxbt/web/static/joyconl.svg`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt/web/static/joyconr.svg` & `nxbt-naibaoofficial-1.1.0/nxbt/web/static/joyconr.svg`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt/web/static/js/main.js` & `nxbt-naibaoofficial-1.1.0/nxbt/web/static/js/main.js`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt/web/static/js/socket.io.js` & `nxbt-naibaoofficial-1.1.0/nxbt/web/static/js/socket.io.js`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt/web/static/procon-transparent.svg` & `nxbt-naibaoofficial-1.1.0/nxbt/web/static/procon-transparent.svg`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt/web/static/procon.svg` & `nxbt-naibaoofficial-1.1.0/nxbt/web/static/procon.svg`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt/web/templates/index.html` & `nxbt-naibaoofficial-1.1.0/nxbt/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt_naibaoofficial.egg-info/PKG-INFO` & `nxbt-naibaoofficial-1.1.0/nxbt_naibaoofficial.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nxbt-naibaoofficial
-Version: 1.0.0
+Version: 1.1.0
 Summary: nxbt marco enhanced by naibaooffical
 Home-page: https://pypi.python.org/pypi/nxbt
 Author: Reece Walsh
 Author-email: reece@brikwerk.com
 License: MIT
 Project-URL: Code, https://github.com/Brikwerk/nxbt
 Project-URL: Issue tracker, https://github.com/Brikwerk/nxbt/issues
@@ -32,34 +32,37 @@
           <a href="#installation">Installation</a> •
           <a href="#getting-started">Getting Started</a> •
           <a href="#troubleshooting">Troubleshooting</a> •
           <a href="#credits">Credits</a> •
           <a href="#license">License</a>
         </p>
         
-        ![screenshot](https://raw.githubusercontent.com/Brikwerk/nxbt/master/docs/img/nxbt-example.png)
+        ![screenshot](https://raw.githubusercontent.com/Naibaowjk/nxbt/master/docs/img/nxbt-example.png)
+        
+        ## Important
+        **This program is based on Brikwerk's nxbt project for secondary development, in order to respect the original author, I did not modify all the copyright information in the documentation, only the necessary places to make changes to the documentation.**
         
         ## Key Features
         
         - Use your favourite web browser to control a Nintendo Switch with any keyboard or gamepad.
         - Use your terminal to control a Nintendo Switch with a keyboard.
         - Use a macro from your terminal, browser, or Python script
         - Use the NXBT Python API to write programs to control your Nintendo Switch.
-        - Primitive loop support in macros.
         - In-depth command line interface.
         - Support for emulating multiple controllers at once.
         - Support for fast connection or reconnection to a Nintendo Switch.
         - Emulated ontrollers support thread-safe access.
+        - ** Use macro in loop, support automacic go back to game and press 'YB' together.
         
         ## Installation
         
         ### Linux
         
         ```bash
-        sudo pip3 install nxbt
+        sudo pip3 install nxbt-naibaoofficial
         ```
         
         **Please Note:** NXBT needs root privileges to toggle the BlueZ Input plugin. If you're not comfortable running this program as root, you can disable the Input plugin manually, and install NXBT as a regular user.
         
         ### Windows and macOS
         
         See the installation guide [here.](docs/Windows-and-macOS-Installation.md)
@@ -192,14 +195,84 @@
         
         If you want more information on NXBT's CLI arguments:
         
         ```bash
         sudo nxbt -h
         ```
         
+        Here is my version help info
+        ```bash
+        $ sudo nxbt macro -h
+          -h, --help            show this help message and exit
+          -c COMMANDS, --commands COMMANDS
+                                Used in conjunction with the macro command. Specifies a macro string or a file location to load a macro string from.
+          -r, --reconnect       Used in conjunction with the macro or tui command. If specified, nxbt will attmept to reconnect to any previously connected Nintendo Switch.
+          -a ADDRESS, --address ADDRESS
+                                Used in conjunction with the macro or tui command. If specified, nxbt will attmept to reconnect to a specific Bluetooth MAC address of a Nintendo Switch.
+          -d, --debug           Enables debug mode in nxbt.
+          -l, --logfile         Enables logging to a file in the current working directory instead of stderr.
+          -i IP, --ip IP        Specifies the IP to run the webapp at. Defaults to 0.0.0.0
+          -p PORT, --port PORT  Specifies the port to run the webapp at. Defaults to 8000
+          --usessl              Enables or disables SSL use in the webapp
+          --certpath CERTPATH   Specifies the folder location for SSL certificates used in the webapp. Certificates in this folder should be in the form of a 'cert.pem' and 'key.pem' pair.
+          --repeat REPEAT       Setting repeat times for macro. Defaults to 0, '-1' means forever
+          --commandinit COMMANDINIT
+                                Used in conjunction with the macro command init. Specifies a macro string or a file location to load a macro string from. This co mmand will not repeat, u can use for back game to start macro rightly
+        ```
+        
+        Using macro command to auto go back game and start macro loop:
+        ```bash
+        $ sudo nxbt macro -c "macro-02.txt" --commandinit "macro-init.txt" --repeat -1
+        $ cat macro-init
+        ZR 0.1S
+        0.3S
+        DPAD_UP 0.2S
+        1S
+        PLUS 0.2S
+        0.3S
+        DPAD_LEFT 0.1S
+        0.1S
+        A 0.1S
+        0.1S
+        DPAD_DOWN 0.1S
+        0.1S
+        A 0.1S
+        0.1S
+        DPAD_RIGHT 0.1S
+        0.1S
+        A 0.1S
+        0.1S
+        A 0.1S
+        0.6S
+        PLUS 0.05S
+        0.08S
+        PLUS 0.05S
+        0.3S
+        DPAD_LEFT 0.1S
+        0.2S
+        A 0.1S
+        0.2S
+        DPAD_DOWN 0.1S
+        0.2S
+        A 0.1S
+        0.3S
+        B 0.1S
+        0.3S
+        L_STICK@+000+100 0.1S
+        0.3S
+        A 0.1S
+        0.1S
+        A 0.1S
+        0.1S
+        L_STICK@+000-100 0.1S
+        ```
+        
+        ```
+        
+        
         ### Running Macros with the Python API
         
         Macros are supported with the `macro` function in the Python API. All macros are expected as strings (multiline strings are accepted).
         
         Minimal working example:
         
         ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nxbt-naibaoofficial Version: 1.0.0 Summary: nxbt
+Metadata-Version: 2.1 Name: nxbt-naibaoofficial Version: 1.1.0 Summary: nxbt
 marco enhanced by naibaooffical Home-page: https://pypi.python.org/pypi/nxbt
 Author: Reece Walsh Author-email: reece@brikwerk.com License: MIT Project-URL:
 Code, https://github.com/Brikwerk/nxbt Project-URL: Issue tracker, https://
 github.com/Brikwerk/nxbt/issues Description:
                                     ******
                                     [NXBT]
                                      NXBT
@@ -12,50 +12,55 @@
    Issues](https://img.shields.io/github/issues/brikwerk/nxbt.svg)](https://
       github.com/brikwerk/ctqa/issues) [![GitHub Pull Requests](https://
     img.shields.io/github/issues-pr/brikwerk/nxbt.svg)](https://github.com/
   brikwerk/ctqa/pulls) [![License](https://img.shields.io/badge/license-MIT-
                              blue.svg)](/LICENSE)
    Key_Features â¢ Installation â¢ Getting_Started â¢ Troubleshooting â¢
                               Credits â¢ License
-![screenshot](https://raw.githubusercontent.com/Brikwerk/nxbt/master/docs/img/
-nxbt-example.png) ## Key Features - Use your favourite web browser to control a
-Nintendo Switch with any keyboard or gamepad. - Use your terminal to control a
-Nintendo Switch with a keyboard. - Use a macro from your terminal, browser, or
-Python script - Use the NXBT Python API to write programs to control your
-Nintendo Switch. - Primitive loop support in macros. - In-depth command line
+![screenshot](https://raw.githubusercontent.com/Naibaowjk/nxbt/master/docs/img/
+nxbt-example.png) ## Important **This program is based on Brikwerk's nxbt
+project for secondary development, in order to respect the original author, I
+did not modify all the copyright information in the documentation, only the
+necessary places to make changes to the documentation.** ## Key Features - Use
+your favourite web browser to control a Nintendo Switch with any keyboard or
+gamepad. - Use your terminal to control a Nintendo Switch with a keyboard. -
+Use a macro from your terminal, browser, or Python script - Use the NXBT Python
+API to write programs to control your Nintendo Switch. - In-depth command line
 interface. - Support for emulating multiple controllers at once. - Support for
 fast connection or reconnection to a Nintendo Switch. - Emulated ontrollers
-support thread-safe access. ## Installation ### Linux ```bash sudo pip3 install
-nxbt ``` **Please Note:** NXBT needs root privileges to toggle the BlueZ Input
-plugin. If you're not comfortable running this program as root, you can disable
-the Input plugin manually, and install NXBT as a regular user. ### Windows and
-macOS See the installation guide [here.](docs/Windows-and-macOS-
-Installation.md) ## Getting Started **Note:** If you installed NXBT as a non-
-root user, please omit the use of `sudo` from any of the following commands.
-### Running the demo The demo is meant to gauge whether or not NXBT is working.
-To do so, the demo will create a Pro Controller and run through a small loop of
-commands. **NOTE:** If this is your first time connecting to an NXBT emulated
-controller on the specific host computer, you **MUST** have the "Change Grip/
-Order Menu" open on your Nintendo Switch. You can see how to navigate to the
-"Change Grip/Order Menu" [HERE](docs/img/change-grip-order-menu.png). To start
-the demo, run the following command in your terminal: ```bash sudo nxbt demo
-``` If all is working correctly, the controller should connect, navigate to the
-settings, test the stick calibration, and navigate back to the "Change Grip/
-Order Menu". ## Using the Webapp The NXBT webapp provides a web interface that
-allows for quick creation of a Nintendo Switch controller and use of a keyboard
-or gamepad to control the Nintendo Switch. This lets anyone who can access the
-website control a Nintendo Switch with their favourite keyboard or gamepad. The
-webapp server can be started with the following command: ```bash sudo nxbt
-webapp ``` The above command boots NXBT and an accompanying web server that
-allows for controller creation and use over your web browser. The webapp itself
-will be locally accessible at `http://127.0.0.1:8000` or, if you're on the same
-network as the host computer, http://HOST_COMPUTER_IP:8000. It's also possible
-to expose your NXBT webapp to the internet, however, you'll need to configure a
-reverse proxy, which is out of the scope of this readme. You should see a
-webpage similar to the following image:
+support thread-safe access. - ** Use macro in loop, support automacic go back
+to game and press 'YB' together. ## Installation ### Linux ```bash sudo pip3
+install nxbt-naibaoofficial ``` **Please Note:** NXBT needs root privileges to
+toggle the BlueZ Input plugin. If you're not comfortable running this program
+as root, you can disable the Input plugin manually, and install NXBT as a
+regular user. ### Windows and macOS See the installation guide [here.](docs/
+Windows-and-macOS-Installation.md) ## Getting Started **Note:** If you
+installed NXBT as a non-root user, please omit the use of `sudo` from any of
+the following commands. ### Running the demo The demo is meant to gauge whether
+or not NXBT is working. To do so, the demo will create a Pro Controller and run
+through a small loop of commands. **NOTE:** If this is your first time
+connecting to an NXBT emulated controller on the specific host computer, you
+**MUST** have the "Change Grip/Order Menu" open on your Nintendo Switch. You
+can see how to navigate to the "Change Grip/Order Menu" [HERE](docs/img/change-
+grip-order-menu.png). To start the demo, run the following command in your
+terminal: ```bash sudo nxbt demo ``` If all is working correctly, the
+controller should connect, navigate to the settings, test the stick
+calibration, and navigate back to the "Change Grip/Order Menu". ## Using the
+Webapp The NXBT webapp provides a web interface that allows for quick creation
+of a Nintendo Switch controller and use of a keyboard or gamepad to control the
+Nintendo Switch. This lets anyone who can access the website control a Nintendo
+Switch with their favourite keyboard or gamepad. The webapp server can be
+started with the following command: ```bash sudo nxbt webapp ``` The above
+command boots NXBT and an accompanying web server that allows for controller
+creation and use over your web browser. The webapp itself will be locally
+accessible at `http://127.0.0.1:8000` or, if you're on the same network as the
+host computer, http://HOST_COMPUTER_IP:8000. It's also possible to expose your
+NXBT webapp to the internet, however, you'll need to configure a reverse proxy,
+which is out of the scope of this readme. You should see a webpage similar to
+the following image:
                           [NXBT Webapp Start Screen]
 To create and start a Pro Controller, click the Pro controller graphic. If
 creation/boot is successful, the website will switch to a loading screen.
 During this time, you should have the Nintendo Switch you wish to connect to
 powered on and within range of the host computer. **NOTE:** If this is your
 first time connecting to your Nintendo Switch with the specific host computer,
 make sure you're on the "Change Grip/Order Menu". If you're still unable to
@@ -105,37 +110,63 @@
 commands you would like to run. You'll need to be on the "Change Grip/Order
 Menu" for the above command to work. If you've already connected to the Switch
 on the host computer, you can reconnect and run the macro by adding the `-r` or
 `--reconnect` flag: ```bash sudo nxbt macro -c "B 0.1s\n 0.1s" -r ``` Since it
 can be a little cumbersome typing out a large macro in the terminal, the macro
 command also supports reading from text files instead! commands.txt file: ``` B
 0.1s 0.1s ``` ```bash sudo nxbt macro -c "commands.txt" -r ``` If you want more
-information on NXBT's CLI arguments: ```bash sudo nxbt -h ``` ### Running
-Macros with the Python API Macros are supported with the `macro` function in
-the Python API. All macros are expected as strings (multiline strings are
-accepted). Minimal working example: ```python import nxbt macro = """ B 0.1s
-0.1s """ # Start the NXBT service nx = nxbt.Nxbt() # Create a Pro Controller
-and wait for it to connect controller_index = nx.create_controller
-(nxbt.PRO_CONTROLLER) nx.wait_for_connection(controller_index) # Run a macro on
-the Pro Controller nx.macro(controller_index, macro) ``` The above example uses
-a blocking macro call, however, multiple macros can be queued (or other actions
-taken) with the non-blocking syntax. Queued macros are processed in FIFO
-(First-In-First-Out) order. ```python # Run a macro on the Pro Controller but
-don't block. # In this instance, we record the macro ID so we can keep track of
-its status later on. macro_id = nx.macro(controller_index, macro, block=False)
-from time import sleep while macro_id not in nx.state[controller_index]
-["finished_macros"]: print("Macro hasn't finished") sleep(1/10) print("Macro
-has finished") ``` ## Using the API NXBT provides a Python API for use in
-Python applications or code. If you're someone that learns by example, check
-out the `demo.py` file located at the root of this project. For a more in-depth
-look at all the functionality provided by the API, checkout the `nxbt/nxbt.py`
-file. For those looking to get started with a few simple examples: Read on!
-**Creating a Controller and Waiting for it to Connect** ```python import nxbt #
-Start the NXBT service nx = nxbt.Nxbt() # Create a Pro Controller and wait for
-it to connect controller_index = nx.create_controller(nxbt.PRO_CONTROLLER)
+information on NXBT's CLI arguments: ```bash sudo nxbt -h ``` Here is my
+version help info ```bash $ sudo nxbt macro -h -h, --help show this help
+message and exit -c COMMANDS, --commands COMMANDS Used in conjunction with the
+macro command. Specifies a macro string or a file location to load a macro
+string from. -r, --reconnect Used in conjunction with the macro or tui command.
+If specified, nxbt will attmept to reconnect to any previously connected
+Nintendo Switch. -a ADDRESS, --address ADDRESS Used in conjunction with the
+macro or tui command. If specified, nxbt will attmept to reconnect to a
+specific Bluetooth MAC address of a Nintendo Switch. -d, --debug Enables debug
+mode in nxbt. -l, --logfile Enables logging to a file in the current working
+directory instead of stderr. -i IP, --ip IP Specifies the IP to run the webapp
+at. Defaults to 0.0.0.0 -p PORT, --port PORT Specifies the port to run the
+webapp at. Defaults to 8000 --usessl Enables or disables SSL use in the webapp
+--certpath CERTPATH Specifies the folder location for SSL certificates used in
+the webapp. Certificates in this folder should be in the form of a 'cert.pem'
+and 'key.pem' pair. --repeat REPEAT Setting repeat times for macro. Defaults to
+0, '-1' means forever --commandinit COMMANDINIT Used in conjunction with the
+macro command init. Specifies a macro string or a file location to load a macro
+string from. This co mmand will not repeat, u can use for back game to start
+macro rightly ``` Using macro command to auto go back game and start macro
+loop: ```bash $ sudo nxbt macro -c "macro-02.txt" --commandinit "macro-
+init.txt" --repeat -1 $ cat macro-init ZR 0.1S 0.3S DPAD_UP 0.2S 1S PLUS 0.2S
+0.3S DPAD_LEFT 0.1S 0.1S A 0.1S 0.1S DPAD_DOWN 0.1S 0.1S A 0.1S 0.1S DPAD_RIGHT
+0.1S 0.1S A 0.1S 0.1S A 0.1S 0.6S PLUS 0.05S 0.08S PLUS 0.05S 0.3S DPAD_LEFT
+0.1S 0.2S A 0.1S 0.2S DPAD_DOWN 0.1S 0.2S A 0.1S 0.3S B 0.1S 0.3S
+L_STICK@+000+100 0.1S 0.3S A 0.1S 0.1S A 0.1S 0.1S L_STICK@+000-100 0.1S ```
+``` ### Running Macros with the Python API Macros are supported with the
+`macro` function in the Python API. All macros are expected as strings
+(multiline strings are accepted). Minimal working example: ```python import
+nxbt macro = """ B 0.1s 0.1s """ # Start the NXBT service nx = nxbt.Nxbt() #
+Create a Pro Controller and wait for it to connect controller_index =
+nx.create_controller(nxbt.PRO_CONTROLLER) nx.wait_for_connection
+(controller_index) # Run a macro on the Pro Controller nx.macro
+(controller_index, macro) ``` The above example uses a blocking macro call,
+however, multiple macros can be queued (or other actions taken) with the non-
+blocking syntax. Queued macros are processed in FIFO (First-In-First-Out)
+order. ```python # Run a macro on the Pro Controller but don't block. # In this
+instance, we record the macro ID so we can keep track of its status later on.
+macro_id = nx.macro(controller_index, macro, block=False) from time import
+sleep while macro_id not in nx.state[controller_index]["finished_macros"]:
+print("Macro hasn't finished") sleep(1/10) print("Macro has finished") ``` ##
+Using the API NXBT provides a Python API for use in Python applications or
+code. If you're someone that learns by example, check out the `demo.py` file
+located at the root of this project. For a more in-depth look at all the
+functionality provided by the API, checkout the `nxbt/nxbt.py` file. For those
+looking to get started with a few simple examples: Read on! **Creating a
+Controller and Waiting for it to Connect** ```python import nxbt # Start the
+NXBT service nx = nxbt.Nxbt() # Create a Pro Controller and wait for it to
+connect controller_index = nx.create_controller(nxbt.PRO_CONTROLLER)
 nx.wait_for_connection(controller_index) print("Connected") ``` **Pressing a
 Button** ```python # Press the B button # press_buttons defaults to pressing a
 button for 0.1s and releasing for 0.1s nx.press_buttons(controller_idx,
 [nxbt.Buttons.B]) # Pressing the B button for 1.0s instead of 0.1s
 nx.press_buttons(controller_idx, [nxbt.Buttons.B], down=1.0) ``` **Tilting a
 Analog Stick** ```python # Tilt the right stick fully to the left. # tilt_stick
 defaults to tilting the stick for 0.1s and releasing for 0.1s nx.tilt_stick
```

### Comparing `nxbt-naibaoofficial-1.0.0/nxbt_naibaoofficial.egg-info/SOURCES.txt` & `nxbt-naibaoofficial-1.1.0/nxbt_naibaoofficial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/setup.cfg` & `nxbt-naibaoofficial-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nxbt-naibaoofficial-1.0.0/setup.py` & `nxbt-naibaoofficial-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="nxbt-naibaoofficial",
-    version='1.0.0',
+    version='1.1.0',
     description='nxbt marco enhanced by naibaooffical',
     include_package_data=True,
     long_description_content_type="text/markdown",
     install_requires=[
         "dbus-python==1.2.16",
         "Flask==1.1.2",
         "Flask-SocketIO==5.0.1",
```

