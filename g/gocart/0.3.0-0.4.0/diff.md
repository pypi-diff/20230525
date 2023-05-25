# Comparing `tmp/gocart-0.3.0.tar.gz` & `tmp/gocart-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gocart-0.3.0.tar", last modified: Thu May 18 20:22:09 2023, max compression
+gzip compressed data, was "gocart-0.4.0.tar", last modified: Wed May 24 12:00:51 2023, max compression
```

## Comparing `gocart-0.3.0.tar` & `gocart-0.4.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-18 20:22:09.842508 gocart-0.3.0/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2071 2023-05-18 20:17:14.000000 gocart-0.3.0/CHANGES.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-05-18 20:17:14.000000 gocart-0.3.0/LICENSE
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-05-18 20:17:14.000000 gocart-0.3.0/MANIFEST.in
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6065 2023-05-18 20:22:09.842508 gocart-0.3.0/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5499 2023-05-18 20:17:14.000000 gocart-0.3.0/README.md
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-18 20:22:09.834508 gocart-0.3.0/gocart/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      189 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/__version__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      738 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/advanced_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     8730 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/cl_utils.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-18 20:22:09.838508 gocart-0.3.0/gocart/commonutils/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      157 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/commonutils/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1920 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/commonutils/flatten_healpix_map.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3054 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/commonutils/generate_skymap_stats.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/commonutils/getpackagepath.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-18 20:22:09.838508 gocart-0.3.0/gocart/convert/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      204 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/convert/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    12423 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/convert/aitoff.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3420 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/convert/ascii.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6489 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/convert/healpix2cart.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3033 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/default_settings.yaml
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-18 20:22:09.838508 gocart-0.3.0/gocart/parsers/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       56 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/parsers/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    14405 2023-05-18 20:17:14.000000 gocart-0.3.0/gocart/parsers/lvk.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-18 20:22:09.806507 gocart-0.3.0/gocart/resources/
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-18 20:22:09.842508 gocart-0.3.0/gocart/resources/plugins/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3124 2023-05-18 20:17:15.000000 gocart-0.3.0/gocart/resources/plugins/gp_template.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-05-18 20:17:15.000000 gocart-0.3.0/gocart/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2770 2023-05-18 20:17:15.000000 gocart-0.3.0/gocart/test_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-05-18 20:17:15.000000 gocart-0.3.0/gocart/utKit.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-18 20:22:09.834508 gocart-0.3.0/gocart.egg-info/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6065 2023-05-18 20:22:09.000000 gocart-0.3.0/gocart.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      788 2023-05-18 20:22:09.000000 gocart-0.3.0/gocart.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-05-18 20:22:09.000000 gocart-0.3.0/gocart.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-05-18 20:22:09.000000 gocart-0.3.0/gocart.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-05-18 20:20:59.000000 gocart-0.3.0/gocart.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      113 2023-05-18 20:22:09.000000 gocart-0.3.0/gocart.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-05-18 20:22:09.000000 gocart-0.3.0/gocart.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-05-18 20:22:09.842508 gocart-0.3.0/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1934 2023-05-18 20:17:15.000000 gocart-0.3.0/setup.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-24 12:00:51.812312 gocart-0.4.0/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2755 2023-05-24 11:56:04.000000 gocart-0.4.0/CHANGES.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2023-05-24 11:56:04.000000 gocart-0.4.0/LICENSE
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      377 2023-05-24 11:56:04.000000 gocart-0.4.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6065 2023-05-24 12:00:51.812312 gocart-0.4.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     5499 2023-05-24 11:56:04.000000 gocart-0.4.0/README.md
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-24 12:00:51.800312 gocart-0.4.0/gocart/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      189 2023-05-24 11:56:04.000000 gocart-0.4.0/gocart/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2023-05-24 11:56:04.000000 gocart-0.4.0/gocart/__version__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      738 2023-05-24 11:56:04.000000 gocart-0.4.0/gocart/advanced_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10395 2023-05-24 11:56:04.000000 gocart-0.4.0/gocart/cl_utils.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-24 12:00:51.800312 gocart-0.4.0/gocart/commonutils/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      157 2023-05-24 11:56:04.000000 gocart-0.4.0/gocart/commonutils/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4198 2023-05-24 11:56:04.000000 gocart-0.4.0/gocart/commonutils/flatten_healpix_map.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3054 2023-05-24 11:56:04.000000 gocart-0.4.0/gocart/commonutils/generate_skymap_stats.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2023-05-24 11:56:04.000000 gocart-0.4.0/gocart/commonutils/getpackagepath.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-24 12:00:51.808312 gocart-0.4.0/gocart/convert/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      204 2023-05-24 11:56:04.000000 gocart-0.4.0/gocart/convert/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    12776 2023-05-24 11:56:04.000000 gocart-0.4.0/gocart/convert/aitoff.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3397 2023-05-24 11:56:04.000000 gocart-0.4.0/gocart/convert/ascii.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6489 2023-05-24 11:56:04.000000 gocart-0.4.0/gocart/convert/healpix2cart.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3096 2023-05-24 11:56:04.000000 gocart-0.4.0/gocart/default_settings.yaml
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-24 12:00:51.808312 gocart-0.4.0/gocart/parsers/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       56 2023-05-24 11:56:04.000000 gocart-0.4.0/gocart/parsers/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    15001 2023-05-24 11:56:04.000000 gocart-0.4.0/gocart/parsers/lvk.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-24 12:00:51.784311 gocart-0.4.0/gocart/resources/
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-24 12:00:51.808312 gocart-0.4.0/gocart/resources/plugins/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3124 2023-05-24 11:56:04.000000 gocart-0.4.0/gocart/resources/plugins/gp_template.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9654 2023-05-24 11:56:04.000000 gocart-0.4.0/gocart/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2770 2023-05-24 11:56:04.000000 gocart-0.4.0/gocart/test_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3387 2023-05-24 11:56:04.000000 gocart-0.4.0/gocart/utKit.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2023-05-24 12:00:51.800312 gocart-0.4.0/gocart.egg-info/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6065 2023-05-24 12:00:51.000000 gocart-0.4.0/gocart.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      788 2023-05-24 12:00:51.000000 gocart-0.4.0/gocart.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-05-24 12:00:51.000000 gocart-0.4.0/gocart.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       48 2023-05-24 12:00:51.000000 gocart-0.4.0/gocart.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2023-05-24 11:59:42.000000 gocart-0.4.0/gocart.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      109 2023-05-24 12:00:51.000000 gocart-0.4.0/gocart.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        7 2023-05-24 12:00:51.000000 gocart-0.4.0/gocart.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2023-05-24 12:00:51.812312 gocart-0.4.0/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1915 2023-05-24 11:56:04.000000 gocart-0.4.0/setup.py
```

### Comparing `gocart-0.3.0/CHANGES.md` & `gocart-0.4.0/CHANGES.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 
 ## Release Notes
 
+**0.4.0 - May 24, 2023**
+
+- **FEATURE**: gocart can now run in daemon mode. Use the commands `gocart listen|quit|restart|status`   
+- **ENHANCEMENT**: added an `event_dir_exist` parameter to the filtering criteria. If a previous event alert has passed the filtering criteria, it is now possible to allow all subsequent alerts will pass   
+- **ENHANCEMENT**: redshift range added to the right side of aitoff plots  
+- **REFACTOR**: removed `ligo.skymap` dependency as this is a huge package and was causing upgrades of gocart to take 20-40 mins. Required new code to convert multi-order skymaps to a single-order (I was previously relying on a function in `ligo.skymap` to do this)  
+
 **v0.3.0 - May 18, 2023**  
 
 - **FEATURE**: user can now add their own plugin scripts to run every time an alert is parsed  
 - **ENHANCEMENT**: added a count of alerts read when first connected to kafka (gives users peace of mind that goacrt is working)  
 - **FIXED**: area calulations fixed (I was still sort by prob but should have been sorting by probdensity for mulit-order maps)  
 - **FIXED**: can still read an event ID even if not found in the sky-map header (tried to find the event ID from the map directory path)
```

### Comparing `gocart-0.3.0/LICENSE` & `gocart-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gocart-0.3.0/PKG-INFO` & `gocart-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gocart
-Version: 0.3.0
+Version: 0.4.0
 Summary: Listen for, collect and convert multimessenger skymaps
 Home-page: https://github.com/thespacedoctor/gocart
-Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.3.0.zip
+Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.4.0.zip
 Author: David Young
 Author-email: d.r.young@qub.ac.uk
 License: MIT
 Keywords: astronomy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `gocart-0.3.0/README.md` & `gocart-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `gocart-0.3.0/gocart/advanced_settings.yaml` & `gocart-0.4.0/gocart/advanced_settings.yaml`

 * *Files identical despite different names*

### Comparing `gocart-0.3.0/gocart/cl_utils.py` & `gocart-0.4.0/gocart/cl_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # encoding: utf-8
 """
 Documentation for gocart can be found here: http://gocart.readthedocs.org
 
 Usage:
     gocart init
     gocart [-p] echo <daysAgo> [-s <pathToSettingsFile>]
-    gocart [-p] listen [-s <pathToSettingsFile>]
+    gocart [-p] (listen|quit|restart|status) [-s <pathToSettingsFile>]
 
 
 Options:
     init                                   setup the gocart settings file for the first time
     echo <daysAgo>                         relisten to alerts from N <daysAgo> until now and then exit
     listen                                 reconnect to kafka stream and listen from where you left off (or from now on if connectiong for the first time).
 
@@ -141,62 +141,104 @@
             if not os.path.exists(mockDir):
                 os.makedirs(mockDir)
         if parse_real_events:
             print(f"{verb} Superevents")
             if not os.path.exists(evertDir):
                 os.makedirs(evertDir)
 
-    # CALL FUNCTIONS/OBJECTS
-    if a['listen']:
-        from gcn_kafka import Consumer
-        from confluent_kafka import TopicPartition
-        from gocart.parsers import lvk
+    if a['listen'] or a["quit"] or a["status"] or a["restart"]:
 
-        config = {
-            'group.id': settings["gcn-kafka"]["group_id"],
-            'enable.auto.commit': False,
-            'auto.offset.reset': 'earliest'
-        }
-
-        consumer = Consumer(config=config, client_id=settings['gcn-kafka']['client_id'],
-                            client_secret=settings['gcn-kafka']['client_secret'], domain='gcn.nasa.gov')
-        consumer.subscribe([topic])
-
-        stop = False
-        test = 0
-        more = True
-        while not stop:
-            # IF FISRT TIME CONNECTING THEN SKIP MESSAGES
-            if firstConnect:
-                count = 0
-                index = 1
-                print("Marking previous messages as read, this can take a few minutes")
-                while more:
-                    messages = consumer.consume(num_messages=300, timeout=5)
-                    for message in messages:
-                        count += 1
+        # ADD SOMETHING LIKE THE FOLLOWING TO THE CL USAGE:
+        """
+        Usage:
+            myCommand (start|stop|restart|status)
+
+            Options:
+                start                 start the myCommand daemon
+                stop                  stop the myCommand daemon
+                restart               restart the myCommand daemon
+                status                print the staus of the myCommand daemon
+        """
+
+        from fundamentals import daemonise
+
+        class myDaemon(daemonise):
+            def action(
+                    self,
+                    **kwargs):
+                self.log.info('starting the ``action`` method')
+
+                from gcn_kafka import Consumer
+                from confluent_kafka import TopicPartition
+                from gocart.parsers import lvk
+
+                firstConnect = kwargs["firstConnect"]
+
+                from datetime import datetime, date, time
+                now = datetime.now()
+                now = now.strftime("%Y%m%dt%H%M%S")
+
+                print(f"gocart listen started at {now}")
+
+                config = {
+                    'group.id': settings["gcn-kafka"]["group_id"],
+                    'enable.auto.commit': False,
+                    'auto.offset.reset': 'earliest'
+                }
+
+                consumer = Consumer(config=config, client_id=settings['gcn-kafka']['client_id'],
+                                    client_secret=settings['gcn-kafka']['client_secret'], domain='gcn.nasa.gov')
+                consumer.subscribe([topic])
+
+                stop = False
+                test = 0
+                more = True
+                while not stop:
+                    # IF FISRT TIME CONNECTING THEN SKIP MESSAGES
+                    if firstConnect:
+                        count = 0
+                        index = 1
+                        print("Marking previous messages as read, this can take a few minutes")
+                        while more:
+                            messages = consumer.consume(num_messages=300, timeout=5)
+                            for message in messages:
+                                count += 1
+                                consumer.commit(message)
+                            if index > 1:
+                                # Cursor up one line and clear line
+                                sys.stdout.write("\x1b[1A\x1b[2K")
+                            index += 1
+                            print(f"{count} messages read ...")
+                            if not len(messages):
+                                more = False
+
+                        firstConnect = False
+                        print(f"This is your first time using the listen command. gocart will now listen for all new incoming alerts (skipping the {count} previous alerts currently in this topic). If you stop listening and restart sometime later, gocart will immediately collect all alerts missed while off-line.")
+                    for message in consumer.consume(timeout=1):
+                        parser = lvk(
+                            log=log,
+                            record=message.value(),
+                            settings=settings,
+                            plugins=a["pluginsFlag"]
+                        ).parse()
                         consumer.commit(message)
-                    if index > 1:
-                        # Cursor up one line and clear line
-                        sys.stdout.write("\x1b[1A\x1b[2K")
-                    index += 1
-                    print(f"{count} messages read ...")
-                    if not len(messages):
-                        more = False
-
-                firstConnect = False
-                print(f"This is your first time using the listen command. gocart will now listen for all new incoming alerts (skipping the {count} previous alerts currently in this topic). If you stop listening and restart sometime later, gocart will immediately collect all alerts missed while off-line.")
-            for message in consumer.consume(timeout=1):
-                parser = lvk(
-                    log=log,
-                    record=message.value(),
-                    settings=settings,
-                    plugins=a["pluginsFlag"]
-                ).parse()
-                consumer.commit(message)
+
+                self.log.info('completed the ``action`` method')
+                return None
+
+        d = myDaemon(log=log, name="gocart", firstConnect=firstConnect)
+
+        if a['listen']:
+            d.start()
+        elif a['quit']:
+            d.stop()
+        elif a['restart']:
+            d.restart()
+        elif a['status']:
+            d.status()
 
     if a['echo'] and a['daysAgo']:
         # GET MESSAGES OCCURRING IN LAST N DAYS
         from gcn_kafka import Consumer
         from confluent_kafka import TopicPartition
         from gocart.parsers import lvk
         import datetime
```

### Comparing `gocart-0.3.0/gocart/commonutils/generate_skymap_stats.py` & `gocart-0.4.0/gocart/commonutils/generate_skymap_stats.py`

 * *Files identical despite different names*

### Comparing `gocart-0.3.0/gocart/convert/aitoff.py` & `gocart-0.4.0/gocart/convert/aitoff.py`

 * *Files 3% similar despite different names*

```diff
@@ -288,14 +288,20 @@
                 far /= 365.
                 data += f"FAR: 1 per {far:0.1f} yrs\n"
             else:
                 data += f"FAR: 1 per {far:0.1f} days\n"
 
             if 'DISTMEAN' in self.meta['HEADER']:
                 data += f"Dist: {self.meta['HEADER']['DISTMEAN']:.2f} (±{self.meta['HEADER']['DISTSTD']:.2f}) Mpc\n"
+                ho = 67
+                zlow = (ho * (self.meta['HEADER']['DISTMEAN'] - self.meta['HEADER']['DISTSTD'])) / 3e5
+                zhigh = (ho * (self.meta['HEADER']['DISTMEAN'] + self.meta['HEADER']['DISTSTD'])) / 3e5
+                if zlow < 0:
+                    zlow = 0
+                data += f"Redshift: {zlow:0.2}<z<{zhigh:0.2}\n"
 
             data += "\n"
             if "classification" in self.meta['ALERT']['event']:
                 for k, v in self.meta['ALERT']['event']['classification'].items():
                     data += f"{k}: {v:.2f}\n"
 
             data += "\n"
```

### Comparing `gocart-0.3.0/gocart/convert/ascii.py` & `gocart-0.4.0/gocart/convert/ascii.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     ):
         self.log = log
         log.debug("instansiating a new 'ascii' object")
         self.settings = settings
         self.mapPath = mapPath
         self.nside = nside
 
-        self.hdus, self.table = flatten_healpix_map(
+        self.table = flatten_healpix_map(
             log=log,
             mapPath=self.mapPath,
             nside=self.nside
         )
 
         return None
 
@@ -80,15 +80,15 @@
             - ``ascii`` -- the CSV version of the healpix file (nside=64)
         """
         self.log.debug('starting the ``get`` method')
 
         import astropy_healpix as ah
         from astropy.coordinates import SkyCoord
 
-        tableData = self.table.to_pandas()
+        tableData = self.table
 
         # CREATE RA AND DEC COLUMNS
         ra, dec = ah.healpix_to_lonlat(tableData.index, 64, order='nested')
         tableData["RA"] = ra.deg
         tableData["DEC"] = dec.deg
 
         # ALSO GLON GLAT COLUMNS
```

### Comparing `gocart-0.3.0/gocart/convert/healpix2cart.py` & `gocart-0.4.0/gocart/convert/healpix2cart.py`

 * *Files identical despite different names*

### Comparing `gocart-0.3.0/gocart/default_settings.yaml` & `gocart-0.4.0/gocart/default_settings.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     #     - name: high significance
     #       alert_types: [initial, update, retraction]
     #       ns_lower: 0.99
     #       far_upper: 1.6e-10
     #       dist_upper: 250
     #       hasns_lower: 0.9
     #       hasremnant_lower: 0.5
+    #     - name: live event
+    #       event_dir_exist: True
 
 # KAFKA CLIENT CREDENTIALS - https://gcn.nasa.gov/quickstart
 gcn-kafka:
     client_id: XXXX
     client_secret: XXXX
     group_id: XXXX
```

### Comparing `gocart-0.3.0/gocart/parsers/lvk.py` & `gocart-0.4.0/gocart/parsers/lvk.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,16 +268,18 @@
                 if os.path.isfile(filepath) and d[:3] == "gp_":
                     cmd = f"""/usr/bin/env python {filepath} {alertDir}"""
                     print(f"PLUGIN: {d}")
                     try:
                         p = Popen(cmd, stdout=PIPE, stderr=PIPE, shell=True)
                         stdout, stderr = p.communicate()
                         print(stdout.decode('utf-8'))
+                        if stderr:
+                            print(f"could not execute the {d} plugin. Failed with error: {stderr.decode('utf-8')}")
                     except Exception as e:
-                        self.log.error(f'cound not execute the {d} plugin. Failed with error: {e}')
+                        self.log.error(f'could not execute the {d} plugin. Failed with error: {e}')
 
         self.log.debug('completed the ``parse`` method')
         return lvk
 
     def filter_alert(
             self,
             alert):
@@ -319,14 +321,22 @@
                 message.append(f"area90 = {alert['EXTRA']['area90']} (> {f['area90_upper']})")
             if "hasns_lower" in f and 'event' in alert['ALERT'] and alert['ALERT']['event'] and 'properties' in alert['ALERT']['event'] and not alert['ALERT']['event']['properties']['HasNS'] >= f["hasns_lower"]:
                 passing = False
                 message.append(f"HasNS = {alert['ALERT']['event']['properties']['HasNS']} (< {f['hasns_lower']})")
             if "hasremnant_lower" in f and 'event' in alert['ALERT'] and alert['ALERT']['event'] and 'properties' in alert['ALERT']['event'] and not alert['ALERT']['event']['properties']['HasRemnant'] >= f["hasremnant_lower"]:
                 passing = False
                 message.append(f"HasRemnant = {alert['ALERT']['event']['properties']['HasRemnant']} (< {f['hasremnant_lower']})")
+            if "event_dir_exits" in f:
+                if self.record["superevent_id"][0] == 'M':
+                    eventDir = self.mockDir + self.record["superevent_id"]
+                else:
+                    eventDir = self.eventDir + self.record["superevent_id"]
+                if not os.path.exists(eventDir):
+                    passing = False
+                    message.append(f"The event has never passed the filtering criteria")
 
             filterResults.append(passing)
 
             if passing:
                 print(f"The alert passes the {f['name']} filter")
             else:
                 message = (" and ").join(message)
```

### Comparing `gocart-0.3.0/gocart/resources/plugins/gp_template.py` & `gocart-0.4.0/gocart/resources/plugins/gp_template.py`

 * *Files identical despite different names*

### Comparing `gocart-0.3.0/gocart/setup.cfg` & `gocart-0.4.0/gocart/setup.cfg`

 * *Files identical despite different names*

### Comparing `gocart-0.3.0/gocart/test_settings.yaml` & `gocart-0.4.0/gocart/test_settings.yaml`

 * *Files identical despite different names*

### Comparing `gocart-0.3.0/gocart/utKit.py` & `gocart-0.4.0/gocart/utKit.py`

 * *Files identical despite different names*

### Comparing `gocart-0.3.0/gocart.egg-info/PKG-INFO` & `gocart-0.4.0/gocart.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: gocart
-Version: 0.3.0
+Version: 0.4.0
 Summary: Listen for, collect and convert multimessenger skymaps
 Home-page: https://github.com/thespacedoctor/gocart
-Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.3.0.zip
+Download-URL: https://github.com/thespacedoctor/gocart/archive/v0.4.0.zip
 Author: David Young
 Author-email: d.r.young@qub.ac.uk
 License: MIT
 Keywords: astronomy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `gocart-0.3.0/gocart.egg-info/SOURCES.txt` & `gocart-0.4.0/gocart.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gocart-0.3.0/setup.py` & `gocart-0.4.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,24 +16,24 @@
     'astropy==5.2.0',
     'astropy-healpix',
     'numpy',
     'matplotlib',
     'healpy',
     'pandas',
     'tabulate',
-    'ligo.skymap',
-    'gcn-kafka'
+    'gcn-kafka',
+    'mhealpy'
 ]
 
 # READ THE DOCS SERVERS
 exists = os.path.exists("/home/docs/")
 if exists:
     install_requires = ['fundamentals']
     c_exclude_list = ['healpy', 'astropy',
-                      'numpy', 'sherlock', 'wcsaxes', 'HMpTy', 'ligo-gracedb', 'ligo.skymap', 'astropy==5.1.0', 'gcn-kafka', 'astropy_healpix']
+                      'numpy', 'sherlock', 'wcsaxes', 'HMpTy', 'ligo-gracedb', 'astropy==5.1.0', 'gcn-kafka', 'astropy_healpix']
     for e in c_exclude_list:
         try:
             install_requires.remove(e)
         except:
             pass
 
 setup(name="gocart",
```

