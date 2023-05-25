# Comparing `tmp/mediaserver-api-client-4.0.tar.gz` & `tmp/mediaserver-api-client-4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediaserver-api-client-4.0.tar", last modified: Wed Mar  8 14:44:42 2023, max compression
+gzip compressed data, was "mediaserver-api-client-4.2.tar", last modified: Thu May 25 07:28:50 2023, max compression
```

## Comparing `mediaserver-api-client-4.0.tar` & `mediaserver-api-client-4.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 djdev     (1000) djdev     (1000)        0 2023-03-08 14:44:42.943731 mediaserver-api-client-4.0/
--rw-rw-r--   0 djdev     (1000) djdev     (1000)     7651 2018-01-16 07:32:19.000000 mediaserver-api-client-4.0/LICENSE
--rw-r--r--   0 djdev     (1000) djdev     (1000)     7753 2023-03-08 14:44:42.943731 mediaserver-api-client-4.0/PKG-INFO
--rw-r--r--   0 djdev     (1000) djdev     (1000)     6853 2023-03-08 14:36:31.000000 mediaserver-api-client-4.0/README.md
-drwxr-xr-x   0 djdev     (1000) djdev     (1000)        0 2023-03-08 14:44:42.943731 mediaserver-api-client-4.0/mediaserver_api_client.egg-info/
--rw-r--r--   0 djdev     (1000) djdev     (1000)     7753 2023-03-08 14:44:42.000000 mediaserver-api-client-4.0/mediaserver_api_client.egg-info/PKG-INFO
--rw-r--r--   0 djdev     (1000) djdev     (1000)      479 2023-03-08 14:44:42.000000 mediaserver-api-client-4.0/mediaserver_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 djdev     (1000) djdev     (1000)        1 2023-03-08 14:44:42.000000 mediaserver-api-client-4.0/mediaserver_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 djdev     (1000) djdev     (1000)       29 2023-03-08 14:44:42.000000 mediaserver-api-client-4.0/mediaserver_api_client.egg-info/requires.txt
--rw-r--r--   0 djdev     (1000) djdev     (1000)       10 2023-03-08 14:44:42.000000 mediaserver-api-client-4.0/mediaserver_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 djdev     (1000) djdev     (1000)        0 2023-03-08 14:44:42.943731 mediaserver-api-client-4.0/ms_client/
--rw-r--r--   0 djdev     (1000) djdev     (1000)       20 2022-11-02 15:53:11.000000 mediaserver-api-client-4.0/ms_client/__init__.py
--rw-r--r--   0 djdev     (1000) djdev     (1000)    11704 2023-03-08 09:51:31.000000 mediaserver-api-client-4.0/ms_client/client.py
--rw-r--r--   0 djdev     (1000) djdev     (1000)     1399 2023-03-08 09:54:56.000000 mediaserver-api-client-4.0/ms_client/conf.py
-drwxr-xr-x   0 djdev     (1000) djdev     (1000)        0 2023-03-08 14:44:42.943731 mediaserver-api-client-4.0/ms_client/lib/
--rw-r--r--   0 djdev     (1000) djdev     (1000)        0 2019-05-24 10:00:59.000000 mediaserver-api-client-4.0/ms_client/lib/__init__.py
--rw-r--r--   0 djdev     (1000) djdev     (1000)     4651 2023-03-08 09:51:11.000000 mediaserver-api-client-4.0/ms_client/lib/configuration.py
--rw-r--r--   0 djdev     (1000) djdev     (1000)     3291 2023-03-08 09:52:03.000000 mediaserver-api-client-4.0/ms_client/lib/content.py
--rw-r--r--   0 djdev     (1000) djdev     (1000)     8615 2023-03-08 09:59:28.000000 mediaserver-api-client-4.0/ms_client/lib/upload.py
--rw-r--r--   0 djdev     (1000) djdev     (1000)     1770 2023-03-08 09:51:17.000000 mediaserver-api-client-4.0/ms_client/lib/users_csv.py
--rw-r--r--   0 djdev     (1000) djdev     (1000)     1145 2023-03-08 14:44:42.943731 mediaserver-api-client-4.0/setup.cfg
--rwxr-xr-x   0 djdev     (1000) djdev     (1000)       63 2019-05-23 14:56:48.000000 mediaserver-api-client-4.0/setup.py
-drwxr-xr-x   0 djdev     (1000) djdev     (1000)        0 2023-03-08 14:44:42.943731 mediaserver-api-client-4.0/tests/
--rw-r--r--   0 djdev     (1000) djdev     (1000)     1849 2022-11-02 15:43:01.000000 mediaserver-api-client-4.0/tests/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 07:28:50.128059 mediaserver-api-client-4.2/
+-rw-rw-r--   0 root         (0) root         (0)     7651 2018-01-16 07:32:19.000000 mediaserver-api-client-4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7753 2023-05-25 07:28:50.128059 mediaserver-api-client-4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6853 2023-03-08 14:36:31.000000 mediaserver-api-client-4.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 07:28:50.124059 mediaserver-api-client-4.2/mediaserver_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7753 2023-05-25 07:28:50.000000 mediaserver-api-client-4.2/mediaserver_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      479 2023-05-25 07:28:50.000000 mediaserver-api-client-4.2/mediaserver_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 07:28:50.000000 mediaserver-api-client-4.2/mediaserver_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-25 07:28:50.000000 mediaserver-api-client-4.2/mediaserver_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-25 07:28:50.000000 mediaserver-api-client-4.2/mediaserver_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 07:28:50.124059 mediaserver-api-client-4.2/ms_client/
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-09 09:51:44.000000 mediaserver-api-client-4.2/ms_client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12057 2023-05-09 09:19:38.000000 mediaserver-api-client-4.2/ms_client/client.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-04-26 14:30:33.000000 mediaserver-api-client-4.2/ms_client/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 07:28:50.128059 mediaserver-api-client-4.2/ms_client/lib/
+-rw-r--r--   0 root         (0) root         (0)        0 2019-05-24 10:00:59.000000 mediaserver-api-client-4.2/ms_client/lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4651 2023-03-08 09:51:11.000000 mediaserver-api-client-4.2/ms_client/lib/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     3778 2023-05-09 09:28:06.000000 mediaserver-api-client-4.2/ms_client/lib/content.py
+-rw-r--r--   0 root         (0) root         (0)     9332 2023-05-09 09:24:21.000000 mediaserver-api-client-4.2/ms_client/lib/upload.py
+-rw-r--r--   0 root         (0) root         (0)     2036 2023-05-09 09:20:25.000000 mediaserver-api-client-4.2/ms_client/lib/users_csv.py
+-rw-r--r--   0 root         (0) root         (0)     1174 2023-05-25 07:28:50.128059 mediaserver-api-client-4.2/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)       63 2019-05-23 14:56:48.000000 mediaserver-api-client-4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 07:28:50.128059 mediaserver-api-client-4.2/tests/
+-rw-r--r--   0 root         (0) root         (0)      943 2023-05-09 09:12:28.000000 mediaserver-api-client-4.2/tests/test_client.py
```

### Comparing `mediaserver-api-client-4.0/LICENSE` & `mediaserver-api-client-4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mediaserver-api-client-4.0/PKG-INFO` & `mediaserver-api-client-4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediaserver-api-client
-Version: 4.0
+Version: 4.2
 Summary: A python3 reference implementation of an UbiCast MediaServer API client
 Home-page: https://www.ubicast.eu/en/solutions/delivery/
 Download-URL: https://github.com/UbiCastTeam/mediaserver-client
 Author: UbiCast
 Author-email: dev@ubicast.eu
 License: LGPLv3
 Keywords: api,client,mediaserver,nudgis,ubicast
```

### Comparing `mediaserver-api-client-4.0/README.md` & `mediaserver-api-client-4.2/README.md`

 * *Files identical despite different names*

### Comparing `mediaserver-api-client-4.0/mediaserver_api_client.egg-info/PKG-INFO` & `mediaserver-api-client-4.2/mediaserver_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediaserver-api-client
-Version: 4.0
+Version: 4.2
 Summary: A python3 reference implementation of an UbiCast MediaServer API client
 Home-page: https://www.ubicast.eu/en/solutions/delivery/
 Download-URL: https://github.com/UbiCastTeam/mediaserver-client
 Author: UbiCast
 Author-email: dev@ubicast.eu
 License: LGPLv3
 Keywords: api,client,mediaserver,nudgis,ubicast
```

### Comparing `mediaserver-api-client-4.0/ms_client/client.py` & `mediaserver-api-client-4.2/ms_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,19 +24,21 @@
         super().__init__(message)
 
 
 class MediaServerClient():
     """
     MediaServer API client class
     """
-    DEFAULT_CONF = None  # Can be either a dict, a path (`str` object) or a unix user (`unix:msuser` for example)
-    RequestError = MediaServerRequestError  # A reference to the error class to avoid circular imports in the client lib dir
+    # `DEFAULT_CONF` can be either a dict, a path (`str` object) or a unix user (`unix:msuser` for example).
+    DEFAULT_CONF = None
+    # `RequestError` is a reference to the error class to avoid circular imports in the client lib dir.
+    RequestError = MediaServerRequestError
 
     def __init__(self, local_conf=None, setup_logging=True):
-        # "local_conf" can be either a dict, a path (`str` object) or a unix user (`unix:msuser` for example)
+        # `local_conf` can be either a dict, a path (`str` object) or a unix user (`unix:msuser` for example)
         # Setup logging
         if setup_logging:
             log_format = '%(asctime)s %(name)s %(levelname)s %(message)s'
             logging.basicConfig(level=logging.INFO, format=log_format)
         # Read conf file
         self.load_conf(local_conf)
         # Configure logging
@@ -88,15 +90,16 @@
                     status_code=getattr(err, 'status_code', None),
                     error_code=getattr(err, 'error_code', None)
                 ) from err
             else:
                 logger.debug(f'MediaServer version is: {self._server_version}')
         return self._server_version
 
-    def request(self, url, method='get', headers=None, params=None, data=None, files=None, parse_json=True, timeout=None, stream=False, ignored_status_codes=None, authenticate=True):
+    def request(self, url, method='get', headers=None, params=None, data=None, files=None, parse_json=True,
+                timeout=None, stream=False, ignored_status_codes=None, authenticate=True):
         self.check_conf()
 
         if ignored_status_codes is None:
             ignored_status_codes = []
 
         if self.conf['USE_SESSION']:
             if self.session is None:
@@ -186,15 +189,17 @@
                     f'API call failed on "{url}": {error_message}',
                     status_code=status_code,
                     error_code=error_code,
                     response=response,
                 )
             elif ignored_status_codes and status_code in ignored_status_codes:
                 # Ignored status codes do not trigger retries nor raise exceptions
-                logger.info(f'Not raising exception for ignored status code {status_code} on url {url} ignored: {response}')
+                logger.info(
+                    f'Not raising exception for ignored status code {status_code} on url {url} ignored: {response}'
+                )
                 return None
             else:
                 raise MediaServerRequestError(
                     f'HTTP {status_code} error on "{url}": {error_message}',
                     status_code=status_code,
                     error_code=error_code,
                     response=response,
@@ -223,23 +228,32 @@
                 tried += 1
                 try:
                     result = self.request(*args, **kwargs)
                     break
                 except MediaServerRequestError as err:
                     # Retry after errors like timeout or RemoteDisconnected errors
                     if err.status_code in self.conf['RETRY_EXCEPT']:
-                        logger.error(f'Request on "{suffix}" failed, tried {tried} times (no retry for the status code {err.status_code}).')
+                        logger.error(
+                            f'Request on "{suffix}" failed, tried {tried} times '
+                            f'(no retry for the status code {err.status_code}).'
+                        )
                         raise err
                     elif tried > max_retry:
-                        logger.error(f'Request on "{suffix}" failed, tried {tried} times (reached max retry count).')
+                        logger.error(
+                            f'Request on "{suffix}" failed, tried {tried} times '
+                            f'(reached max retry count).'
+                        )
                         raise err
                     else:
                         # Wait longer after every attempt
                         delay = 3 * tried * tried
-                        logger.error(f'Request on "{suffix}" failed, tried {tried} times (max {max_retry}), retrying in {delay}s.')
+                        logger.error(
+                            f'Request on "{suffix}" failed, tried {tried} times '
+                            f'(max {max_retry}), retrying in {delay}s.'
+                        )
                         time.sleep(delay)
                         # Seek to 0 in file objects
                         # (file objects using a value different from 0 as initial position is not supported)
                         if kwargs.get('files'):
                             # Python-requests supports the following files arguments:
                             # files = {'file': open('report.xls', 'rb')}
                             # files = {'file': tuple}
```

### Comparing `mediaserver-api-client-4.0/ms_client/conf.py` & `mediaserver-api-client-4.2/ms_client/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,13 +37,13 @@
 
     # Proxies for API requests
     # To use system proxies: None (proxies should be set in environment)
     # To disable proxies: {'http': '', 'https': ''}
     # To use a proxy: {'http': 'http://10.10.1.10:3128', 'https': 'http://10.10.1.10:1080'}
     'PROXIES': None,
 
-    # Chunk size for uploads
-    'UPLOAD_CHUNK_SIZE': 5242880,
+    # Chunk size for uploads (in bytes)
+    'UPLOAD_CHUNK_SIZE': 26214400,
 
     # Maximum number of files per request
     'UPLOAD_MAX_FILES': 100,
 }
```

### Comparing `mediaserver-api-client-4.0/ms_client/lib/configuration.py` & `mediaserver-api-client-4.2/ms_client/lib/configuration.py`

 * *Files identical despite different names*

### Comparing `mediaserver-api-client-4.0/ms_client/lib/content.py` & `mediaserver-api-client-4.2/ms_client/lib/content.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,87 @@
 """
 MediaServer client content library
 This module is not intended to be used directly, only the client class should be used.
 """
 import logging
-import os
 import zipfile
+from pathlib import Path
 
 logger = logging.getLogger(__name__)
 
 
-def add_media(client, title=None, file_path=None, progress_callback=None, progress_data=None, timeout=3600, max_retry=None, **kwargs):
+def add_media(client, title=None, file_path=None, progress_callback=None,
+              progress_data=None, timeout=3600, max_retry=None, **kwargs):
     if not title and not file_path:
         raise ValueError('You should give a title or a file to create a media.')
-    if file_path is not None and os.path.getsize(file_path) == 0:
-        raise Exception('File is empty: %s' % file_path)
+    if file_path is not None:
+        file_path = Path(file_path)
+        if file_path.stat().st_size == 0:
+            raise ValueError('File is empty: %s' % file_path)
     metadata = kwargs
     metadata['origin'] = client.conf['CLIENT_ID']
     if title:
         metadata['title'] = title
     if file_path:
         upload_retry = max_retry if max_retry is not None else 10
-        metadata['code'] = client.chunked_upload(file_path, progress_callback=progress_callback, progress_data=progress_data, max_retry=upload_retry)
-    response = client.api('medias/add/', method='post', data=metadata, timeout=timeout, max_retry=max_retry)
+        metadata['code'] = client.chunked_upload(
+            file_path,
+            progress_callback=progress_callback,
+            progress_data=progress_data,
+            max_retry=upload_retry
+        )
+    response = client.api(
+        'medias/add/',
+        method='post',
+        data=metadata,
+        timeout=timeout,
+        max_retry=max_retry
+    )
     return response
 
 
-def download_metadata_zip(client, media_oid, path, include_annotations=None, include_resources_links=None, force=False, timeout=3600, max_retry=None):
+def download_metadata_zip(client, media_oid, path, include_annotations=None, include_resources_links=None,
+                          force=False, timeout=3600, max_retry=None):
     if not media_oid:
         raise ValueError('You should give an object id to get the zip file.')
     valid_annotations = ('all', 'editorial', 'none')
     if include_annotations and include_annotations not in valid_annotations:
-        raise ValueError('Invalid value given for "include_annotations". Valid values: %s.' % ', '.join(valid_annotations))
+        raise ValueError(f'Invalid value given for "include_annotations". Valid values: {valid_annotations}.')
     valid_resources = ('yes', 'no')
     if include_resources_links and include_resources_links not in valid_resources:
-        raise ValueError('Invalid value given for "include_resources_links". Valid values: %s.' % ', '.join(valid_resources))
-    params = dict(oid=media_oid, annotations=include_annotations or 'none', resources=include_resources_links or 'no')
-    if not force and os.path.isfile(path):
-        size = str(os.path.getsize(path))
-        req = client.api('medias/get/zip/', method='head', params=params, timeout=timeout, max_retry=max_retry)
-        if req.headers.get('Content-Length') == size:
-            logger.info('Skipping download of zip file for %s because the file already exists and has the correct size.', media_oid)
+        raise ValueError(f'Invalid value given for "include_resources_links". Valid values: {valid_resources}.')
+    params = dict(
+        oid=media_oid,
+        annotations=include_annotations or 'none',
+        resources=include_resources_links or 'no'
+    )
+    path = Path(path)
+    if not force and path.is_file():
+        size = path.stat().st_size
+        req = client.api(
+            'medias/get/zip/',
+            method='head',
+            params=params,
+            timeout=timeout,
+            max_retry=max_retry
+        )
+        if req.headers.get('Content-Length') == str(size):
+            logger.info(
+                'Skipping download of zip file for %s because the file already exists and has the correct size.',
+                media_oid
+            )
             return path
-    req = client.api('medias/get/zip/', method='get', params=params, timeout=timeout, max_retry=max_retry, stream=True)
+    req = client.api(
+        'medias/get/zip/',
+        method='get',
+        params=params,
+        timeout=timeout,
+        max_retry=max_retry,
+        stream=True
+    )
     with open(path, 'wb') as fo:
         for chunk in req.iter_content(10000000):  # 10 MB chunks
             fo.write(chunk)
 
     # Check that the file is really a zip file
     zip_file = zipfile.ZipFile(path, 'r')
     if zip_file.testzip():
@@ -55,10 +91,16 @@
 
 def remove_all_content(client, timeout=None, max_retry=None):
     logger.info('Remove all content')
     channels = client.api('channels/tree/')['channels']
     while client.api('channels/tree')['channels']:
         for c in channels:
             c_oid = c['oid']
-            client.api('channels/delete/', method='post', data={'oid': c_oid, 'delete_content': 'yes'}, timeout=timeout, max_retry=max_retry)
-            logger.info('Emptied channel %s' % c_oid)
+            client.api(
+                'channels/delete/',
+                method='post',
+                data={'oid': c_oid, 'delete_content': 'yes'},
+                timeout=timeout,
+                max_retry=max_retry
+            )
+            logger.info('Emptied channel %s', c_oid)
         channels = client.api('channels/tree/')['channels']
```

### Comparing `mediaserver-api-client-4.0/ms_client/lib/upload.py` & `mediaserver-api-client-4.2/ms_client/lib/upload.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 MediaServer client upload library
 This module is not intended to be used directly, only the client class should be used.
 """
 from pathlib import Path
-import hashlib
 import logging
 import math
 import time
 
 logger = logging.getLogger(__name__)
 
 
-def chunked_upload(client, file_path, remote_path=None, progress_callback=None, progress_data=None, check_md5=True, timeout=120, max_retry=10):
+def chunked_upload(client, file_path, remote_path=None, progress_callback=None,
+                   progress_data=None, timeout=300, max_retry=10):
     """
     Function to send a file using the chunked upload.
     """
     max_retry = client.get_max_retry(max_retry)
     url_prefix = 'medias/resource/' if client.get_server_version() < (8, 2) else ''
     file_path = Path(file_path)
 
@@ -25,58 +25,73 @@
     chunks_count = math.ceil(total_size / chunk_size)
 
     # Send chunks
     chunk_index = 0
     start_offset = 0
     end_offset = min(chunk_size, total_size) - 1
     data = {}
-    if check_md5:
-        md5sum = hashlib.md5()
     url = client.get_full_url(url_prefix + 'upload/')
     begin = time.time()
     with open(file_path, 'rb') as fo:
         chunk = fo.read(chunk_size)
         while chunk:
             # Send chunk
             chunk_index += 1
             logger.debug(f'Uploading chunk {chunk_index}/{chunks_count}.')
-            if check_md5:
-                md5sum.update(chunk)
             headers = {'Content-Range': f'bytes {start_offset}-{end_offset}/{total_size}'}
             files = {'file': (file_path.name, chunk)}
             tried = 0
             while True:
                 tried += 1
                 try:
                     # Use client.request to handle retry for offset errors
-                    response = client.request(url, method='post', headers=headers, data=data, files=files, timeout=timeout)
+                    response = client.request(
+                        url,
+                        method='post',
+                        headers=headers,
+                        data=data,
+                        files=files,
+                        timeout=timeout
+                    )
                     break
                 except client.RequestError as err:
                     if err.status_code == 400:
                         try:
                             offset = int(err.response.get('offset'))
                         except (ValueError, TypeError):
                             offset = -1
                         if tried > 1 and offset == end_offset + 1 and 'upload_id' in data:
                             # The chunk sent was already received and due to an other error, the request was retried
                             logger.info(f'Offset issue detected during upload, ignoring error: {err}')
                             break
                         # No need to retry for other 400 errors, the result will be the same
-                        logger.error(f'Chunk upload failed, tried {tried} times (no retry for the status code {err.status_code} in chunk upload).')
+                        logger.error(
+                            f'Chunk upload failed, tried {tried} times '
+                            f'(no retry for the status code {err.status_code} in chunk upload).'
+                        )
                         raise err
                     elif err.status_code in client.conf['RETRY_EXCEPT']:
-                        logger.error(f'Chunk upload failed, tried {tried} times (no retry for the status code {err.status_code}).')
+                        logger.error(
+                            f'Chunk upload failed, tried {tried} times '
+                            f'(no retry for the status code {err.status_code}).'
+                        )
                         raise err
                     elif tried > max_retry:
-                        logger.error(f'Chunk upload failed, tried {tried} times (reached max retry count).')
+                        logger.error(
+                            f'Chunk upload failed, tried {tried} times '
+                            f'(reached max retry count).'
+                        )
                         raise err
                     else:
                         # Wait longer after every attempt
                         delay = 3 * tried * tried
-                        logger.error(f'Chunk upload failed, tried {tried} times (max {max_retry}), retrying in {delay}s.')
+                        logger.error(
+                            f'Chunk upload failed, tried {tried} times '
+                            f'(max {max_retry}), retrying in {delay}s.'
+                        )
                         time.sleep(delay)
 
             # Notify progress callback
             if progress_callback:
                 pdata = progress_data or {}
                 progress_callback(0.9 * end_offset / total_size, **pdata)
 
@@ -87,31 +102,35 @@
             end_offset = min(end_offset + chunk_size, total_size - 1)
             chunk = fo.read(chunk_size)
 
     bandwidth = total_size * 8 / ((time.time() - begin) * 1_000_000)
     logger.info(f'Upload finished, average bandwidth was {bandwidth:2f} Mbits/s.')
 
     # Mark file as completed
-    # This will trigger an md5 sum check and will move the file to its correct location in the server
-    if check_md5:
-        data['md5'] = md5sum.hexdigest()
-    else:
-        data['no_md5'] = 'yes'
+    data['no_md5'] = 'yes'  # The md5 check is deprecated since 2023-04-20 and has been removed in Nudgis v11.3.1
+    data['expected_size'] = str(total_size)
     if remote_path:
         data['path'] = remote_path
-    response = client.api(url_prefix + 'upload/complete/', method='post', data=data, timeout=timeout, max_retry=max_retry)
+    response = client.api(
+        url_prefix + 'upload/complete/',
+        method='post',
+        data=data,
+        timeout=timeout,
+        max_retry=max_retry
+    )
 
     # Notify progress callback
     if progress_callback:
         pdata = progress_data or {}
         progress_callback(1., **pdata)
     return data['upload_id']
 
 
-def hls_upload(client, m3u8_path, remote_dir='', progress_callback=None, progress_data=None, timeout=3600, max_retry=10):
+def hls_upload(client, m3u8_path, remote_dir='', progress_callback=None,
+               progress_data=None, timeout=600, max_retry=10):
     """
     Method to upload an HLS video (m3u8 + ts fragments).
     This method is faster than "chunked_upload" because "chunked_upload" is very slow for a large number of tiny files.
     The directory containing ts files must have the same name as the m3u8 file.
     """
     if client.get_server_version() < (8, 2):
         raise Exception('The MediaServer version does not support HLS upload.')
@@ -134,61 +153,87 @@
     files_size = 0
     total_size = 0
     total_files_count = 1
     ts_fragments = sorted(ts_dir.iterdir(), key=lambda item: item.name)
     begin = time.time()
     for ts_path in ts_fragments:
         if not ts_path.is_file():
-            logger.warning(f'Found an element which is not a file in the ts fragments dir "{ts_path.name}". The element will be ignored.')
+            logger.warning(
+                f'Found an element which is not a file in the ts fragments dir "{ts_path.name}". '
+                'The element will be ignored.'
+            )
             continue
 
         size = ts_path.stat().st_size
         files_size += size
         files_list.append((ts_path, size))
         total_files_count += 1
 
         if files_size > max_size or len(files_list) >= max_files:
             # Send files in list
-            logger.info(f'Uploading {len(files_list)} files ({(files_size / 1_000_000):.2f} MB, only fragments) of "{ts_dir}" in one request.')
+            logger.info(
+                f'Uploading {len(files_list)} files ({(files_size / 1_000_000):.2f} MB, only fragments) '
+                f'of "{ts_dir}" in one request.'
+            )
             total_size += files_size
             data = dict(dir_name=remote_dir, hls_name=ts_dir.name)
 
             # Get files size and content (load in RAM to avoid triggering open file limit)
             files = {}
             for path, size in files_list:
                 data[path.name] = str(size)
                 with open(path, 'rb') as fo:
                     files[path.name] = (path.name, fo.read())
-            response = client.api('upload/hls/', method='post', data=data, files=files, timeout=timeout, max_retry=max_retry)
+            response = client.api(
+                'upload/hls/',
+                method='post',
+                data=data,
+                files=files,
+                timeout=timeout,
+                max_retry=max_retry
+            )
 
             # Notify progress callback
             if progress_callback:
                 pdata = progress_data or {}
                 progress_callback(total_files_count / len(ts_fragments), **pdata)
             files_list = []
             files_size = 0
             if not remote_dir:
                 remote_dir = response['dir_name']
 
     # Send remaining ts fragments and m3u8 file
     size = m3u8_path.stat().st_size
     files_size += size
     files_list.append((m3u8_path, size))
-    logger.info(f'Uploading {len(files_list)} files ({(files_size / 1_000_000):.2f} MB, fragments and the playlist) of "{ts_dir}" in one request.')
+    logger.info(
+        f'Uploading {len(files_list)} files ({(files_size / 1_000_000):.2f} MB, fragments and the playlist) '
+        f'of "{ts_dir}" in one request.'
+    )
     total_size += files_size
     data = dict(dir_name=remote_dir, hls_name=ts_dir.name)
     files = {}
 
     # Get files size and content (load in RAM to avoid triggering open file limit)
     for path, size in files_list:
         data[path.name] = str(size)
         with open(path, 'rb') as fo:
             files[path.name] = (path.name, fo.read())
-    client.api('upload/hls/', method='post', data=data, files=files, timeout=timeout, max_retry=max_retry)
+    client.api(
+        'upload/hls/',
+        method='post',
+        data=data,
+        files=files,
+        timeout=timeout,
+        max_retry=max_retry
+    )
     bandwidth = total_size * 8 / ((time.time() - begin) * 1_000_000)
-    logger.info(f'Upload finished ({total_files_count} files in "{remote_dir}"), average bandwidth: {bandwidth:.2f} Mbits/s')
+    logger.info(
+        f'Upload finished ({total_files_count} files in "{remote_dir}"), '
+        f'average bandwidth: {bandwidth:.2f} Mbits/s'
+    )
 
     # Notify progress callback
     if progress_callback:
         pdata = progress_data or {}
         progress_callback(1., **pdata)
     return remote_dir
```

### Comparing `mediaserver-api-client-4.0/ms_client/lib/users_csv.py` & `mediaserver-api-client-4.2/ms_client/lib/users_csv.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 import time
 
 logger = logging.getLogger(__name__)
 
 
 def import_users_csv(client, csv_path, timeout=None, max_retry=None):
     group_name = f'Users imported from csv on {time.ctime()}'
-    group_id = client.api('groups/add/', method='post', data={'name': group_name}).get('id')
+    group_id = client.api(
+        'groups/add/',
+        method='post',
+        data={'name': group_name}
+    ).get('id')
     logger.info(f'Created group {group_name} with id {group_id}')
     with open(csv_path, 'r') as fo:
         content = fo.read()
     for index, line in enumerate(content.split('\n')):
         # Skip first line (contains header)
         if line and index > 0:
             fields = [field.strip() for field in line.split(';')]
@@ -25,19 +29,31 @@
                 'last_name': fields[1],
                 'company': fields[3],
                 'username': email,
                 'is_active': 'true',
             }
             logger.info(f'Adding user "{email}"')
             try:
-                response = client.api('users/add/', method='post', data=user, timeout=timeout, max_retry=max_retry)
+                response = client.api(
+                    'users/add/',
+                    method='post',
+                    data=user,
+                    timeout=timeout,
+                    max_retry=max_retry
+                )
             except Exception as err:
                 logger.error(f'Error: {err}')
             else:
                 logger.info(f'Success: {response}')
             logger.info(f'Adding user "{email}" to group "{group_name}"')
             try:
-                response = client.api('groups/members/add/', method='post', data={'id': group_id, 'user_email': email}, timeout=timeout, max_retry=max_retry)
+                response = client.api(
+                    'groups/members/add/',
+                    method='post',
+                    data={'id': group_id, 'user_email': email},
+                    timeout=timeout,
+                    max_retry=max_retry
+                )
             except Exception as err:
                 logger.error(f'Error: {err}')
             else:
                 logger.info(f'Success: {response}')
```

### Comparing `mediaserver-api-client-4.0/setup.cfg` & `mediaserver-api-client-4.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -25,25 +25,28 @@
 	Programming Language :: Python :: 3.11
 	Topic :: Multimedia :: Video
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 include_package_data = True
 install_requires = 
-	requests >= 2.28
+	requests >= 2.30
 packages = 
 	ms_client
 	ms_client.lib
 setup_requires = 
 	setuptools >= 30.3.0
 	wheel
 
 [options.extras_require]
 dev = 
 	flake8
+	pytest
+	pytest-cov
+	vulture
 
 [bdist_wheel]
 universal = 1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

