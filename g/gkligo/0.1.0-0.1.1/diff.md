# Comparing `tmp/gkligo-0.1.0.tar.gz` & `tmp/gkligo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gkligo-0.1.0.tar", last modified: Tue May 23 23:39:23 2023, max compression
+gzip compressed data, was "gkligo-0.1.1.tar", last modified: Wed May 24 11:11:30 2023, max compression
```

## Comparing `gkligo-0.1.0.tar` & `gkligo-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-23 23:39:23.327611 gkligo-0.1.0/
--rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.1.0/MANIFEST.in
--rw-r--r--   0 kws        (502) staff       (20)     1669 2023-05-23 23:39:23.327029 gkligo-0.1.0/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)      980 2023-04-24 12:55:14.000000 gkligo-0.1.0/README.md
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-23 23:39:23.314180 gkligo-0.1.0/gkligo/
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-28 14:27:19.000000 gkligo-0.1.0/gkligo/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-05-23 22:38:35.000000 gkligo-0.1.0/gkligo/__version__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-23 23:39:23.317675 gkligo-0.1.0/gkligo/scripts/
--rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.1.0/gkligo/scripts/__init__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-23 23:39:23.325653 gkligo-0.1.0/gkligo/scripts/python/
--rw-r--r--   0 kws        (502) staff       (20)       31 2023-04-28 14:27:05.000000 gkligo-0.1.0/gkligo/scripts/python/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       89 2023-04-20 16:53:23.000000 gkligo-0.1.0/gkligo/scripts/python/config_download_example.yaml
--rw-r--r--   0 kws        (502) staff       (20)      426 2023-04-24 12:50:06.000000 gkligo-0.1.0/gkligo/scripts/python/config_reports.yaml
--rw-r--r--   0 kws        (502) staff       (20)      498 2023-04-24 13:37:26.000000 gkligo-0.1.0/gkligo/scripts/python/config_reports_example.yaml
--rwxr-xr-x   0 kws        (502) staff       (20)    13653 2023-05-23 23:09:22.000000 gkligo-0.1.0/gkligo/scripts/python/downloadGWAlerts.py
--rwxr-xr-x   0 kws        (502) staff       (20)     5644 2023-04-24 16:53:21.000000 gkligo-0.1.0/gkligo/scripts/python/generateGWReports.py
--rw-r--r--   0 kws        (502) staff       (20)     1266 2023-05-23 20:34:59.000000 gkligo-0.1.0/gkligo/scripts/python/test.yaml
--rwxr-xr-x   0 kws        (502) staff       (20)     2792 2023-04-27 21:33:22.000000 gkligo-0.1.0/gkligo/scripts/python/testDaemon.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-23 23:39:23.317037 gkligo-0.1.0/gkligo.egg-info/
--rw-r--r--   0 kws        (502) staff       (20)     1669 2023-05-23 23:39:23.000000 gkligo-0.1.0/gkligo.egg-info/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)      610 2023-05-23 23:39:23.000000 gkligo-0.1.0/gkligo.egg-info/SOURCES.txt
--rw-r--r--   0 kws        (502) staff       (20)        1 2023-05-23 23:39:23.000000 gkligo-0.1.0/gkligo.egg-info/dependency_links.txt
--rw-r--r--   0 kws        (502) staff       (20)      147 2023-05-23 23:39:23.000000 gkligo-0.1.0/gkligo.egg-info/entry_points.txt
--rw-r--r--   0 kws        (502) staff       (20)       85 2023-05-23 23:39:23.000000 gkligo-0.1.0/gkligo.egg-info/requires.txt
--rw-r--r--   0 kws        (502) staff       (20)        7 2023-05-23 23:39:23.000000 gkligo-0.1.0/gkligo.egg-info/top_level.txt
--rw-r--r--   0 kws        (502) staff       (20)       38 2023-05-23 23:39:23.327829 gkligo-0.1.0/setup.cfg
--rwxr-xr-x   0 kws        (502) staff       (20)     1308 2023-04-24 13:23:15.000000 gkligo-0.1.0/setup.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-24 11:11:30.652646 gkligo-0.1.1/
+-rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.1.1/MANIFEST.in
+-rw-r--r--   0 kws        (502) staff       (20)     1794 2023-05-24 11:11:30.652206 gkligo-0.1.1/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)     1089 2023-05-24 11:09:44.000000 gkligo-0.1.1/README.md
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-24 11:11:30.642025 gkligo-0.1.1/gkligo/
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-28 14:27:19.000000 gkligo-0.1.1/gkligo/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-05-24 11:06:31.000000 gkligo-0.1.1/gkligo/__version__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-24 11:11:30.644824 gkligo-0.1.1/gkligo/scripts/
+-rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.1.1/gkligo/scripts/__init__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-24 11:11:30.650839 gkligo-0.1.1/gkligo/scripts/python/
+-rw-r--r--   0 kws        (502) staff       (20)       31 2023-04-28 14:27:05.000000 gkligo-0.1.1/gkligo/scripts/python/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       89 2023-04-20 16:53:23.000000 gkligo-0.1.1/gkligo/scripts/python/config_download_example.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      426 2023-04-24 12:50:06.000000 gkligo-0.1.1/gkligo/scripts/python/config_reports.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      498 2023-04-24 13:37:26.000000 gkligo-0.1.1/gkligo/scripts/python/config_reports_example.yaml
+-rwxr-xr-x   0 kws        (502) staff       (20)    11625 2023-05-24 11:05:54.000000 gkligo-0.1.1/gkligo/scripts/python/downloadGWAlerts.py
+-rwxr-xr-x   0 kws        (502) staff       (20)     5644 2023-04-24 16:53:21.000000 gkligo-0.1.1/gkligo/scripts/python/generateGWReports.py
+-rw-r--r--   0 kws        (502) staff       (20)     1266 2023-05-23 20:34:59.000000 gkligo-0.1.1/gkligo/scripts/python/test.yaml
+-rwxr-xr-x   0 kws        (502) staff       (20)     2792 2023-04-27 21:33:22.000000 gkligo-0.1.1/gkligo/scripts/python/testDaemon.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-24 11:11:30.644447 gkligo-0.1.1/gkligo.egg-info/
+-rw-r--r--   0 kws        (502) staff       (20)     1794 2023-05-24 11:11:30.000000 gkligo-0.1.1/gkligo.egg-info/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)      610 2023-05-24 11:11:30.000000 gkligo-0.1.1/gkligo.egg-info/SOURCES.txt
+-rw-r--r--   0 kws        (502) staff       (20)        1 2023-05-24 11:11:30.000000 gkligo-0.1.1/gkligo.egg-info/dependency_links.txt
+-rw-r--r--   0 kws        (502) staff       (20)      147 2023-05-24 11:11:30.000000 gkligo-0.1.1/gkligo.egg-info/entry_points.txt
+-rw-r--r--   0 kws        (502) staff       (20)       85 2023-05-24 11:11:30.000000 gkligo-0.1.1/gkligo.egg-info/requires.txt
+-rw-r--r--   0 kws        (502) staff       (20)        7 2023-05-24 11:11:30.000000 gkligo-0.1.1/gkligo.egg-info/top_level.txt
+-rw-r--r--   0 kws        (502) staff       (20)       38 2023-05-24 11:11:30.652849 gkligo-0.1.1/setup.cfg
+-rwxr-xr-x   0 kws        (502) staff       (20)     1308 2023-04-24 13:23:15.000000 gkligo-0.1.1/setup.py
```

### Comparing `gkligo-0.1.0/PKG-INFO` & `gkligo-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkligo
-Version: 0.1.0
+Version: 0.1.1
 Summary: GW (LIGO) utilities
 Home-page: https://github.com/genghisken/gkligo
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Description: # gkligo
         Code to download GW Alert skymaps from Kafka, and optionally write them
@@ -16,28 +16,30 @@
         
         * gcn-kafka
         * healpy
         * gkutils
         * docopt
         * pyYAML
         * numpy
-        * ligo.skymap
+        * ligo.skymap (via conda install)
         * astropy
         * mocpy
         
         The command line utilities are:
         * downloadGWAlert (Download the alert from Kafka)
         
         The config_example.yaml file is an example config file. Copy it and rename to config.yaml.
         Get your credentials by following the first part of the [Kafka Notices via GCN](https://emfollow.docs.ligo.org/userguide/tutorial/receiving/gcn.html) tutorial. Leave the topics configuration unchanged.
         
         The code has been daemonised so one of the parameters will be start|restart|stop.
         
         Also included is a script called generateGWReports. This will generate coverage reports (CSV files) from the three database (ATLAS, all sky Pan-STARRS, O4 follwup Pan-STARRS).
         
+        TO DO:
+        * Modify generateGWReports to load the GW meta into the database for convenience.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
```

### Comparing `gkligo-0.1.0/README.md` & `gkligo-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 
 * gcn-kafka
 * healpy
 * gkutils
 * docopt
 * pyYAML
 * numpy
-* ligo.skymap
+* ligo.skymap (via conda install)
 * astropy
 * mocpy
 
 The command line utilities are:
 * downloadGWAlert (Download the alert from Kafka)
 
 The config_example.yaml file is an example config file. Copy it and rename to config.yaml.
 Get your credentials by following the first part of the [Kafka Notices via GCN](https://emfollow.docs.ligo.org/userguide/tutorial/receiving/gcn.html) tutorial. Leave the topics configuration unchanged.
 
 The code has been daemonised so one of the parameters will be start|restart|stop.
 
 Also included is a script called generateGWReports. This will generate coverage reports (CSV files) from the three database (ATLAS, all sky Pan-STARRS, O4 follwup Pan-STARRS).
 
+TO DO:
+* Modify generateGWReports to load the GW meta into the database for convenience.
```

### Comparing `gkligo-0.1.0/gkligo/scripts/python/downloadGWAlerts.py` & `gkligo-0.1.1/gkligo/scripts/python/downloadGWAlerts.py`

 * *Files 16% similar despite different names*

```diff
@@ -120,77 +120,19 @@
     logger.info('MOC file %s written' % outputMOCName)
 
 
 def writeMeta(options, dataDict, logger):
     #import MySQLdb
     from astropy.io import fits
 
-    eventid = dataDict['superevent_id']
-    url = dataDict['urls']['gracedb']
-    far = None
-    instruments = None
-
     mjd = None
     distance = None
     distanceStd = None
-    classification = None
-    properties = None
-    significant = None
-    time = None
-    group = None
-    pipeline = None
-    alertType = dataDict['alert_type']
-    timeCreated = dataDict['time_created']
-
-    try:
-        time = dataDict['event']['time']
-    except KeyError as e:
-        logger.error("Can't find the time info.")
-
-    try:
-        group = dataDict['event']['group']
-    except KeyError as e:
-        logger.error("Can't find the group info.")
-
-    try:
-        pipeline = dataDict['event']['pipeline']
-    except KeyError as e:
-        logger.error("Can't find the pipeline info.")
-
-    try:
-        classification = dataDict['event']['classification']
-    except KeyError as e:
-        logger.error("Can't find the classification info.")
-
-    try:
-        significant = dataDict['event']['significant']
-    except KeyError as e:
-        logger.error("Can't find the significance info.")
-
-    try:
-        properties = dataDict['event']['properties']
-    except KeyError as e:
-        logger.error("Can't find the properties info.")
-
     eventMeta = {}
 
-    try:
-        far = float(dataDict['event']['far'])
-        # years = 1/(far*(24*3600*365.2425))
-    except ValueError as e:
-        logger.error("Can't find the FAR info.")
-    except KeyError as e:
-        logger.error("Can't find the FAR info.")
-
-    try:
-        instruments = dataDict['event']['instruments']
-    except KeyError as e:
-        logger.error("Can't find the instuments info.")
-
-
     # Some info (e.g. distance) only in the FITS file
     h = fits.open(BytesIO(base64.b64decode(dataDict['event']['skymap'])))
     header = h[1].header
 
     try:
         mjd = header['MJD-OBS']
     except KeyError as e:
@@ -206,30 +148,21 @@
     except KeyError as e:
         logger.error("The DISTSTD variable is missing.")
 
     # Do NOT write to the database, which could potentially be locked and crash the
     # daemon. Write another script (e.g the reports script) that does that. Just
     # record the metadata for loading.
 
-    eventMeta = {'ALERT': {'event': {'far': far,
-                                     'instruments': instruments,
-                                     'significant': significant,
-                                     'classification': classification,
-                                     'properties': properties,
-                                     'time': time,
-                                     'group': group,
-                                     'pipeline': pipeline},
-                           'urls': {'gracedb': url},
-                           'superevent_id': eventid},
-                           'alert_type': alertType,
-                           'time_created': timeCreated,
+
+    # Remove the skymap from the dictionary.
+    dataDict['event'].pop('skymap')
+    eventMeta = {'ALERT': dataDict,
                  'HEADER': {'MJD-OBS': mjd,
                             'DISTMEAN': distance,
-                            'DISTSTD': distanceStd},
-                }
+                            'DISTSTD': distanceStd}}
 
     return eventMeta
 
  
 def listen(options):
     """listen.
 
@@ -267,17 +200,18 @@
         # Non zero timeout is required, otherwise consume blocks termination signals.
         for message in consumer.consume(timeout=5):
             dataDict = json.loads(message.value().decode('utf-8'))
             try:
                 superEventId = dataDict['superevent_id']
                 eventType = superEventId[0] # M, T or S
 
-                alertTimeStamp = dataDict['time_created'].replace(' ','T')
-                alertType = dataDict['alert_type']
-                alertName = superEventId + '_' + alertType + '_' + alertTimeStamp
+                alertTimeStamp = dataDict['time_created'].replace(' ','T').replace('Z','').replace(':','').replace('-','')
+                alertType = dataDict['alert_type'].lower()
+                #alertName = superEventId + '_' + alertType + '_' + alertTimeStamp
+                alertName = superEventId + '_' + alertTimeStamp + '_' + alertType
                 logger.info("Alert Received: %s" % alertName) # Future version of this script will log the output.
 
                 # Act on all events unless we only want superevents. Need to think about the logic!
                 if eventType != 'S' and options.superevents:
                     logger.info("Skipping over this event.")
                     # Skip to the next event
                     continue
@@ -285,15 +219,15 @@
                 # Write the event meta into the databases
                 if dataDict['event'] is not None and options.writemeta:
                     meta = writeMeta(options, dataDict, logger)
                     if meta:
                         for k,v in meta.items():
                             logger.info("%s = %s" % (k, str(v)))
                         # Overwrite the superevent info every time a new update arrives.
-                        with open(options.directory + '/' + superEventId + '.yaml', 'w') as yamlFile:
+                        with open(options.directory + '/' + alertName + '.yaml', 'w') as yamlFile:
                             yamlFile.write(yaml.dump(meta))
 
 
                 if dataDict['event'] is not None and options.writeMap:
                     skymap = dataDict['event']['skymap']
                     with open(options.directory + '/' + alertName + '.fits', 'wb') as fitsFile:
                         fitsFile.write(base64.b64decode(skymap))
```

### Comparing `gkligo-0.1.0/gkligo/scripts/python/generateGWReports.py` & `gkligo-0.1.1/gkligo/scripts/python/generateGWReports.py`

 * *Files identical despite different names*

### Comparing `gkligo-0.1.0/gkligo/scripts/python/test.yaml` & `gkligo-0.1.1/gkligo/scripts/python/test.yaml`

 * *Files identical despite different names*

### Comparing `gkligo-0.1.0/gkligo/scripts/python/testDaemon.py` & `gkligo-0.1.1/gkligo/scripts/python/testDaemon.py`

 * *Files identical despite different names*

### Comparing `gkligo-0.1.0/gkligo.egg-info/PKG-INFO` & `gkligo-0.1.1/gkligo.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkligo
-Version: 0.1.0
+Version: 0.1.1
 Summary: GW (LIGO) utilities
 Home-page: https://github.com/genghisken/gkligo
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Description: # gkligo
         Code to download GW Alert skymaps from Kafka, and optionally write them
@@ -16,28 +16,30 @@
         
         * gcn-kafka
         * healpy
         * gkutils
         * docopt
         * pyYAML
         * numpy
-        * ligo.skymap
+        * ligo.skymap (via conda install)
         * astropy
         * mocpy
         
         The command line utilities are:
         * downloadGWAlert (Download the alert from Kafka)
         
         The config_example.yaml file is an example config file. Copy it and rename to config.yaml.
         Get your credentials by following the first part of the [Kafka Notices via GCN](https://emfollow.docs.ligo.org/userguide/tutorial/receiving/gcn.html) tutorial. Leave the topics configuration unchanged.
         
         The code has been daemonised so one of the parameters will be start|restart|stop.
         
         Also included is a script called generateGWReports. This will generate coverage reports (CSV files) from the three database (ATLAS, all sky Pan-STARRS, O4 follwup Pan-STARRS).
         
+        TO DO:
+        * Modify generateGWReports to load the GW meta into the database for convenience.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
```

### Comparing `gkligo-0.1.0/gkligo.egg-info/SOURCES.txt` & `gkligo-0.1.1/gkligo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gkligo-0.1.0/setup.py` & `gkligo-0.1.1/setup.py`

 * *Files identical despite different names*

