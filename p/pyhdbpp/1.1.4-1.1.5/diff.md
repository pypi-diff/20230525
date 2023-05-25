# Comparing `tmp/pyhdbpp-1.1.4.tar.gz` & `tmp/pyhdbpp-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyhdbpp-1.1.4.tar", last modified: Tue Mar 28 12:47:16 2023, max compression
+gzip compressed data, was "dist/pyhdbpp-1.1.5.tar", last modified: Thu May 25 14:08:23 2023, max compression
```

## Comparing `pyhdbpp-1.1.4.tar` & `pyhdbpp-1.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-03-28 12:47:16.000000 pyhdbpp-1.1.4/
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-03-28 12:47:16.000000 pyhdbpp-1.1.4/pyhdbpp/
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-03-28 12:47:16.000000 pyhdbpp-1.1.4/pyhdbpp/mariadb/
--rw-r--r--   0 srubio    (1206) Control   (1200)       36 2023-02-02 12:49:29.000000 pyhdbpp-1.1.4/pyhdbpp/mariadb/__init__.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    16286 2023-03-27 15:57:34.000000 pyhdbpp-1.1.4/pyhdbpp/mariadb/mariadb.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-03-28 12:47:16.000000 pyhdbpp-1.1.4/pyhdbpp/multidb/
--rw-r--r--   0 srubio    (1206) Control   (1200)       35 2023-02-02 12:49:29.000000 pyhdbpp-1.1.4/pyhdbpp/multidb/__init__.py
--rw-r--r--   0 srubio    (1206) Control   (1200)     7197 2023-02-02 12:49:29.000000 pyhdbpp-1.1.4/pyhdbpp/multidb/multidb.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-03-28 12:47:16.000000 pyhdbpp-1.1.4/pyhdbpp/qt/
--rw-r--r--   0 srubio    (1206) Control   (1200)        0 2022-12-02 17:00:04.000000 pyhdbpp-1.1.4/pyhdbpp/qt/__init__.py
--rw-r--r--   0 srubio    (1206) Control   (1200)     1093 2022-12-02 17:00:04.000000 pyhdbpp-1.1.4/pyhdbpp/qt/plot.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-03-28 12:47:16.000000 pyhdbpp-1.1.4/pyhdbpp/timescaledb/
--rw-r--r--   0 srubio    (1206) Control   (1200)       43 2022-11-23 14:08:18.000000 pyhdbpp-1.1.4/pyhdbpp/timescaledb/__init__.py
--rwxr-xr-x   0 srubio    (1206) Control   (1200)    10254 2023-02-02 12:49:29.000000 pyhdbpp-1.1.4/pyhdbpp/timescaledb/timescaledb.py
--rw-r--r--   0 srubio    (1206) Control   (1200)      146 2023-02-02 12:49:29.000000 pyhdbpp-1.1.4/pyhdbpp/__init__.py
--rw-r--r--   0 srubio    (1206) Control   (1200)     5183 2023-02-02 12:49:29.000000 pyhdbpp-1.1.4/pyhdbpp/abstract.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    10558 2023-03-27 15:57:37.000000 pyhdbpp-1.1.4/pyhdbpp/reader.py
--rw-r--r--   0 srubio    (1206) Control   (1200)    12169 2023-03-27 15:26:17.000000 pyhdbpp-1.1.4/pyhdbpp/utils.py
-drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-03-28 12:47:16.000000 pyhdbpp-1.1.4/pyhdbpp.egg-info/
--rw-r--r--   0 srubio    (1206) Control   (1200)      491 2023-03-28 12:47:15.000000 pyhdbpp-1.1.4/pyhdbpp.egg-info/PKG-INFO
--rw-r--r--   0 srubio    (1206) Control   (1200)      518 2023-03-28 12:47:16.000000 pyhdbpp-1.1.4/pyhdbpp.egg-info/SOURCES.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)        1 2023-03-28 12:47:15.000000 pyhdbpp-1.1.4/pyhdbpp.egg-info/dependency_links.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)       54 2023-03-28 12:47:15.000000 pyhdbpp-1.1.4/pyhdbpp.egg-info/entry_points.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)       31 2023-03-28 12:47:15.000000 pyhdbpp-1.1.4/pyhdbpp.egg-info/requires.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)        8 2023-03-28 12:47:15.000000 pyhdbpp-1.1.4/pyhdbpp.egg-info/top_level.txt
--rw-r--r--   0 srubio    (1206) Control   (1200)     7637 2022-05-25 07:34:58.000000 pyhdbpp-1.1.4/LICENSE
--rw-r--r--   0 srubio    (1206) Control   (1200)     2607 2023-03-27 15:27:43.000000 pyhdbpp-1.1.4/README.md
--rw-r--r--   0 srubio    (1206) Control   (1200)      567 2023-03-28 12:47:16.000000 pyhdbpp-1.1.4/setup.cfg
--rw-r--r--   0 srubio    (1206) Control   (1200)      509 2023-02-02 12:49:29.000000 pyhdbpp-1.1.4/setup.py
--rw-r--r--   0 srubio    (1206) Control   (1200)      491 2023-03-28 12:47:16.000000 pyhdbpp-1.1.4/PKG-INFO
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-05-25 14:08:23.000000 pyhdbpp-1.1.5/
+-rw-r--r--   0 srubio    (1206) Control   (1200)     7637 2022-05-25 07:34:58.000000 pyhdbpp-1.1.5/LICENSE
+-rw-r--r--   0 srubio    (1206) Control   (1200)      491 2023-05-25 14:08:23.000000 pyhdbpp-1.1.5/PKG-INFO
+-rw-r--r--   0 srubio    (1206) Control   (1200)     2607 2023-05-23 15:26:17.000000 pyhdbpp-1.1.5/README.md
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-05-25 14:08:23.000000 pyhdbpp-1.1.5/pyhdbpp/
+-rw-r--r--   0 srubio    (1206) Control   (1200)      146 2023-05-23 15:26:17.000000 pyhdbpp-1.1.5/pyhdbpp/__init__.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)     5183 2023-02-02 12:49:29.000000 pyhdbpp-1.1.5/pyhdbpp/abstract.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-05-25 14:08:23.000000 pyhdbpp-1.1.5/pyhdbpp/mariadb/
+-rw-r--r--   0 srubio    (1206) Control   (1200)       36 2023-05-23 15:26:17.000000 pyhdbpp-1.1.5/pyhdbpp/mariadb/__init__.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    16294 2023-05-23 15:26:17.000000 pyhdbpp-1.1.5/pyhdbpp/mariadb/mariadb.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-05-25 14:08:23.000000 pyhdbpp-1.1.5/pyhdbpp/multidb/
+-rw-r--r--   0 srubio    (1206) Control   (1200)       35 2023-05-23 15:26:17.000000 pyhdbpp-1.1.5/pyhdbpp/multidb/__init__.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)     7197 2023-05-23 15:26:17.000000 pyhdbpp-1.1.5/pyhdbpp/multidb/multidb.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-05-25 14:08:23.000000 pyhdbpp-1.1.5/pyhdbpp/qt/
+-rw-r--r--   0 srubio    (1206) Control   (1200)        0 2022-12-02 17:00:04.000000 pyhdbpp-1.1.5/pyhdbpp/qt/__init__.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)     1093 2022-12-02 17:00:04.000000 pyhdbpp-1.1.5/pyhdbpp/qt/plot.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    10409 2023-05-23 15:26:17.000000 pyhdbpp-1.1.5/pyhdbpp/reader.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-05-25 14:08:23.000000 pyhdbpp-1.1.5/pyhdbpp/timescaledb/
+-rw-r--r--   0 srubio    (1206) Control   (1200)       43 2022-11-23 14:08:18.000000 pyhdbpp-1.1.5/pyhdbpp/timescaledb/__init__.py
+-rwxr-xr-x   0 srubio    (1206) Control   (1200)    10254 2023-02-02 12:49:29.000000 pyhdbpp-1.1.5/pyhdbpp/timescaledb/timescaledb.py
+-rw-r--r--   0 srubio    (1206) Control   (1200)    12244 2023-05-23 15:26:17.000000 pyhdbpp-1.1.5/pyhdbpp/utils.py
+drwxr-xr-x   0 srubio    (1206) Control   (1200)        0 2023-05-25 14:08:23.000000 pyhdbpp-1.1.5/pyhdbpp.egg-info/
+-rw-r--r--   0 srubio    (1206) Control   (1200)      491 2023-05-25 14:08:22.000000 pyhdbpp-1.1.5/pyhdbpp.egg-info/PKG-INFO
+-rw-r--r--   0 srubio    (1206) Control   (1200)      518 2023-05-25 14:08:22.000000 pyhdbpp-1.1.5/pyhdbpp.egg-info/SOURCES.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)        1 2023-05-25 14:08:22.000000 pyhdbpp-1.1.5/pyhdbpp.egg-info/dependency_links.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)       54 2023-05-25 14:08:22.000000 pyhdbpp-1.1.5/pyhdbpp.egg-info/entry_points.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)       31 2023-05-25 14:08:22.000000 pyhdbpp-1.1.5/pyhdbpp.egg-info/requires.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)        8 2023-05-25 14:08:22.000000 pyhdbpp-1.1.5/pyhdbpp.egg-info/top_level.txt
+-rw-r--r--   0 srubio    (1206) Control   (1200)      567 2023-05-25 14:08:23.000000 pyhdbpp-1.1.5/setup.cfg
+-rw-r--r--   0 srubio    (1206) Control   (1200)      509 2023-05-23 15:26:17.000000 pyhdbpp-1.1.5/setup.py
```

### Comparing `pyhdbpp-1.1.4/pyhdbpp/mariadb/mariadb.py` & `pyhdbpp-1.1.5/pyhdbpp/mariadb/mariadb.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         """
         if load or not self.attributes:
             self.get_attribute_id_table('*')
             
         if pattern:
             return [a for a in self.attributes if attr_match(pattern,a)]
             
-        return self.attributes.keys()
+        return sorted(self.attributes.keys())
     
     def get_attribute_name(self,attribute):
         """
         get attribute name as it is used in hdb++ (e.g. FQDN)
         """
         attribute = attr_translate(attribute)
         attrs = self.get_attributes(pattern=attribute, load=False)
```

### Comparing `pyhdbpp-1.1.4/pyhdbpp/multidb/multidb.py` & `pyhdbpp-1.1.5/pyhdbpp/multidb/multidb.py`

 * *Files identical despite different names*

### Comparing `pyhdbpp-1.1.4/pyhdbpp/qt/plot.py` & `pyhdbpp-1.1.5/pyhdbpp/qt/plot.py`

 * *Files identical despite different names*

### Comparing `pyhdbpp-1.1.4/pyhdbpp/timescaledb/timescaledb.py` & `pyhdbpp-1.1.5/pyhdbpp/timescaledb/timescaledb.py`

 * *Files identical despite different names*

### Comparing `pyhdbpp-1.1.4/pyhdbpp/abstract.py` & `pyhdbpp-1.1.5/pyhdbpp/abstract.py`

 * *Files identical despite different names*

### Comparing `pyhdbpp-1.1.4/pyhdbpp/reader.py` & `pyhdbpp-1.1.5/pyhdbpp/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,16 @@
     try:
         schema = os.getenv('DEFAULT_READER',None)
         logger.info('get_default_reader(%s)' % (schema))
         if schema:
             logger.info('os://DefaultSchema: %s' % str(schema))
             if'@' not in schema:
                 schema = load_config_from_tango(schema)
-                return reader(apiclass=schema['apiclass'],config=schema['config'])
+                return reader(apiclass=schema['apiclass'],
+                              config=schema['config'])
             else:
                 return reader(config=schema)
 
         import tango
         if tango_host:
             tangodb = tango.Database(*tango_host.split(':'))
         else:
@@ -92,18 +93,14 @@
         
         if os.path.isfile(config):
             config = load_config_from_file(config)
         elif config.startswith('tango:'):
             config = load_config_from_tango(config)
         elif config:
             config = parse_config_string(config)
-            
-    config['database'] = config.get('database',config.get('db_name','hdb'))
-    config['password'] = config.get('password',config.get('passwd',''))
-    #print(config)
     
     if not validate_config(config):
         logger.error(config)
         raise Exception('InvalidConfig')
 
     # config should be a dict at this point
     apiclass = config.get('apiclass',apiclass)
```

### Comparing `pyhdbpp-1.1.4/pyhdbpp/utils.py` & `pyhdbpp-1.1.5/pyhdbpp/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
         if '@' in config.get('config',''):
             config.update(parse_config_string(config['config']))
 
         # fill missing fields
         config['database'] = config.get('database',
                             config.get('db_name',
                            config.get('dbname','hdbpp')))
+        config['user'] = config.get('user','')                            
         config['password'] = config.get('password',
                             config.get('passwd',
                            config.get('token','')))
         config['config'] = config.get('config', '%s:%s@%s:%s/%s' % (
             config.get('user','user'), config.get('password','...'), 
             config.get('host','localshot'),
             config.get('port','3306'), config.get('database','hdbpp')))
```

### Comparing `pyhdbpp-1.1.4/pyhdbpp.egg-info/SOURCES.txt` & `pyhdbpp-1.1.5/pyhdbpp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhdbpp-1.1.4/LICENSE` & `pyhdbpp-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhdbpp-1.1.4/README.md` & `pyhdbpp-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyhdbpp-1.1.4/setup.cfg` & `pyhdbpp-1.1.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyhdbpp
-version = 1.1.4
+version = 1.1.5
 url = https://gitlab.com/tango-controls/hdbpp/libhdbpp-python
 description = HDB++ python3 API for extraction
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = LGPL
 license_file = LICENSE
 classifiers =
```

