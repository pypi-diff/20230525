# Comparing `tmp/atcom-0.4.1.tar.gz` & `tmp/atcom-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/atcom-0.4.1.tar", last modified: Thu Mar 24 21:20:55 2022, max compression
+gzip compressed data, was "atcom-0.4.3.tar", last modified: Thu May 25 14:00:40 2023, max compression
```

## Comparing `atcom-0.4.1.tar` & `atcom-0.4.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-24 21:20:55.000000 atcom-0.4.1/
--rw-r--r--   0 root         (0) root         (0)     3336 2022-03-24 21:20:55.000000 atcom-0.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2118 2021-04-13 13:25:32.000000 atcom-0.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-24 21:20:55.000000 atcom-0.4.1/atcom/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-20 16:34:55.000000 atcom-0.4.1/atcom/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2022-03-24 21:15:49.000000 atcom-0.4.1/atcom/__version__.py
--rwxr-xr-x   0 root         (0) root         (0)     7289 2022-03-24 21:13:53.000000 atcom-0.4.1/atcom/cli.py
--rw-r--r--   0 root         (0) root         (0)     2869 2022-03-24 21:14:02.000000 atcom-0.4.1/atcom/modems.py
--rw-r--r--   0 root         (0) root         (0)     2633 2022-03-24 20:50:06.000000 atcom-0.4.1/atcom/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-24 21:20:55.000000 atcom-0.4.1/atcom.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3336 2022-03-24 21:20:55.000000 atcom-0.4.1/atcom.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      277 2022-03-24 21:20:55.000000 atcom-0.4.1/atcom.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-24 21:20:55.000000 atcom-0.4.1/atcom.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2022-03-24 21:20:55.000000 atcom-0.4.1/atcom.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       22 2022-03-24 21:20:55.000000 atcom-0.4.1/atcom.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2022-03-24 21:20:55.000000 atcom-0.4.1/atcom.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-03-24 21:20:55.000000 atcom-0.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3070 2021-04-13 13:25:32.000000 atcom-0.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:00:40.336826 atcom-0.4.3/
+-rw-r--r--   0 root         (0) root         (0)     3547 2023-05-25 14:00:40.336826 atcom-0.4.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2289 2023-05-25 11:18:00.000000 atcom-0.4.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:00:40.332826 atcom-0.4.3/atcom/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 11:18:00.000000 atcom-0.4.3/atcom/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-25 13:28:20.000000 atcom-0.4.3/atcom/__version__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7392 2023-05-25 11:18:00.000000 atcom-0.4.3/atcom/cli.py
+-rw-r--r--   0 root         (0) root         (0)     2869 2023-05-25 11:18:00.000000 atcom-0.4.3/atcom/modems.py
+-rw-r--r--   0 root         (0) root         (0)     2883 2023-05-25 13:26:55.000000 atcom-0.4.3/atcom/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:00:40.336826 atcom-0.4.3/atcom.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3547 2023-05-25 14:00:40.000000 atcom-0.4.3/atcom.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      277 2023-05-25 14:00:40.000000 atcom-0.4.3/atcom.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 14:00:40.000000 atcom-0.4.3/atcom.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-25 14:00:40.000000 atcom-0.4.3/atcom.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-25 14:00:40.000000 atcom-0.4.3/atcom.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-25 14:00:40.000000 atcom-0.4.3/atcom.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 14:00:40.336826 atcom-0.4.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3070 2023-05-25 11:18:00.000000 atcom-0.4.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `atcom-0.4.1/PKG-INFO` & `atcom-0.4.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atcom
-Version: 0.4.1
+Version: 0.4.3
 Summary: A tool which makes AT communication easier.
 Home-page: https://github.com/sixfab/atcom
 Author: Bugra Isguzar
 Author-email: bugra@sixfab.com
 License: MIT
 Description: 
         # ATCom
@@ -27,14 +27,19 @@
         ```
         ​
         ## Usage
         ​
         ```bash
         $ atcom [OPTIONS] AT_COMMAND
         ```
+        
+        > ### Warning: 
+        > If you need to send `"` or `'` character, you should use escape character `\` before it.
+        > ### Example: 
+        > ```atcom AT+CGDCONT=1,\"IP\",\"internet\"```
         ​
         ### Examples
         ​
         Running **atcom** without *--port* parameter, scans for available ports, and selects a valid modem port if available.
         ​
         ```bash
         $ atcom AT
```

### Comparing `atcom-0.4.1/README.md` & `atcom-0.4.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,19 @@
 ```
 ​
 ## Usage
 ​
 ```bash
 $ atcom [OPTIONS] AT_COMMAND
 ```
+
+> ### Warning: 
+> If you need to send `"` or `'` character, you should use escape character `\` before it.
+> ### Example: 
+> ```atcom AT+CGDCONT=1,\"IP\",\"internet\"```
 ​
 ### Examples
 ​
 Running **atcom** without *--port* parameter, scans for available ports, and selects a valid modem port if available.
 ​
 ```bash
 $ atcom AT
```

### Comparing `atcom-0.4.1/atcom/cli.py` & `atcom-0.4.3/atcom/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 		Function for getting modem response
 		"""
 		if self.serial.isOpen():
 			response =""
 			timer = millis()
 			
 			while True:
-				delay(100)
+				delay(2)
 				if millis() - timer < timeout: 
 					while self.serial.inWaiting():
 						try: 
 							response += self.serial.read(self.serial.inWaiting()).decode('utf-8')
 						except:
 							raise RuntimeError("An error occured while reading from serial port")
 
@@ -141,16 +141,16 @@
 
 	logger = Logger(verbose)
 	configs = {}
 
 
 	if not at_command:
 		print("Error: AT_COMMAND missing\n")
-		print("Usage: t.py [OPTIONS] AT_COMMAND")
-		print("Try 't.py --help' for help.")
+		print("Usage: atcom [OPTIONS] AT_COMMAND")
+		print("Try 'atcom --help' for help.")
 		return
 
 	try:
 		config_file_path = config or "./configs.yml"
 
 		configs = open(config_file_path, "r").read()
 		configs = yaml.load(configs, Loader=yaml.FullLoader)
@@ -159,25 +159,29 @@
 		logger.info("Configs file not found, reading properties from args")
 
 	else:
 		logger.info("Found configs file, loading properties")
 
 	properties = (
 		{"id": "port", "name": "Port", "required": True},
+		{"id": "baudrate", "name": "Baudrate", "required": False},
 		{"id": "rts_cts", "name": "RTS-CTS", "required": False},
 		{"id": "dsr_dtr", "name": "DSR_DTR", "required": False},
 		{"id": "timeout", "name": "Timeout", "required": False}
 	)
 
 
 	for _property in properties:
 		if not locals().get(_property["id"], None):
 			continue
 	
-		logger.info("{} property specified as argument, overriding config file".format(_property["name"]))
+		logger.info("{} property specified as argument, overriding config file: {}"
+		.format(_property["name"], locals().get(_property["id"]))
+		)
+
 		configs[_property["id"]] = locals().get(_property["id"])
 
 	if not configs.get("port"):
 		logger.info("Port not specified, scanning available ports")
 	
 		detected = decide_port()
 		port_to_connect = detected[0]
```

### Comparing `atcom-0.4.1/atcom/modems.py` & `atcom-0.4.3/atcom/modems.py`

 * *Files identical despite different names*

### Comparing `atcom-0.4.1/atcom/utils.py` & `atcom-0.4.3/atcom/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -35,14 +35,18 @@
                 _port_details["model"] = line[9:].replace("'", "")
             elif line.startswith("ID_MODEL_FROM_DATABASE="):
                 _port_details["model_from_database"] = line[23:].replace("'", "")
             elif line.startswith("ID_MODEL_ID="):
                 _port_details["product_id"] = line[12:].replace("'", "")
             elif line.startswith("ID_USB_INTERFACE_NUM="):
                 _port_details["interface"] = "if"+line[21:].replace("'", "")
+            elif line.startswith("ID_USB_VENDOR_ID="):
+                _port_details["ID_USB_VENDOR_ID"] = line[17:].replace("'", "")
+            elif line.startswith("ID_USB_MODEL_ID="):
+                _port_details["ID_USB_MODEL_ID"] = line[16:].replace("'", "")
 
         if "bus" not in _port_details["port"]:
             available_ports.append(_port_details)
 
     return available_ports
 
 
@@ -64,13 +68,13 @@
         return (None, None)
     else:
         ports = get_available_ports()
         for port in ports:
             if  modem.com_ifs in port.values() and \
                 modem.vid in port.values() and \
                 modem.pid in port.values():
-                
+
                 port_name = port.get("port")
                 modem.desc_vendor = port.get("vendor")
                 modem.desc_product = port.get("model", port.get("model_from_database"))
                 return (port_name, modem)
         return (None, None)
```

### Comparing `atcom-0.4.1/atcom.egg-info/PKG-INFO` & `atcom-0.4.3/atcom.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atcom
-Version: 0.4.1
+Version: 0.4.3
 Summary: A tool which makes AT communication easier.
 Home-page: https://github.com/sixfab/atcom
 Author: Bugra Isguzar
 Author-email: bugra@sixfab.com
 License: MIT
 Description: 
         # ATCom
@@ -27,14 +27,19 @@
         ```
         ​
         ## Usage
         ​
         ```bash
         $ atcom [OPTIONS] AT_COMMAND
         ```
+        
+        > ### Warning: 
+        > If you need to send `"` or `'` character, you should use escape character `\` before it.
+        > ### Example: 
+        > ```atcom AT+CGDCONT=1,\"IP\",\"internet\"```
         ​
         ### Examples
         ​
         Running **atcom** without *--port* parameter, scans for available ports, and selects a valid modem port if available.
         ​
         ```bash
         $ atcom AT
```

### Comparing `atcom-0.4.1/setup.py` & `atcom-0.4.3/setup.py`

 * *Files identical despite different names*

