# Comparing `tmp/qtwasmserver-0.1.1.tar.gz` & `tmp/qtwasmserver-0.1.2.tar.gz`

## Comparing `qtwasmserver-0.1.1.tar` & `qtwasmserver-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 qtwasmserver-0.1.1/build
--rwxr-xr-x   0        0        0     9805 2020-02-02 00:00:00.000000 qtwasmserver-0.1.1/src/qtwasmserver/qtwasmserver.py
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 qtwasmserver-0.1.1/src/qtwasmserver/setup.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 qtwasmserver-0.1.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 qtwasmserver-0.1.1/LICENSE
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 qtwasmserver-0.1.1/README.md
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 qtwasmserver-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 qtwasmserver-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 qtwasmserver-0.1.2/build
+-rwxr-xr-x   0        0        0     9921 2020-02-02 00:00:00.000000 qtwasmserver-0.1.2/src/qtwasmserver/qtwasmserver.py
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 qtwasmserver-0.1.2/src/qtwasmserver/setup.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 qtwasmserver-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 qtwasmserver-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 qtwasmserver-0.1.2/README.md
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 qtwasmserver-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 qtwasmserver-0.1.2/PKG-INFO
```

### Comparing `qtwasmserver-0.1.1/src/qtwasmserver/qtwasmserver.py` & `qtwasmserver-0.1.2/src/qtwasmserver/qtwasmserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,21 @@
     cert_file,
     cert_key_file,
     compression_mode,
     cross_origin_isolation,
 ):
     handler = select_http_handler_class(compression_mode, address)
     handler.cross_origin_isolation = cross_origin_isolation
-    httpd = ThreadingHTTPServer((address, port), handler)
+
+    try:
+        httpd = ThreadingHTTPServer((address, port), handler)
+    except Exception as e:
+        print(f"\n### Error starting HTTP server: {e}\n")
+        exit(1)
+
     if secure:
         context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
         context.load_cert_chain(cert_file.name, cert_key_file.name)
         httpd.socket = context.wrap_socket(
             httpd.socket,
             server_side=True,
         )
```

### Comparing `qtwasmserver-0.1.1/LICENSE` & `qtwasmserver-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qtwasmserver-0.1.1/README.md` & `qtwasmserver-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `qtwasmserver-0.1.1/pyproject.toml` & `qtwasmserver-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "qtwasmserver"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Morten Sørvig", email="msorvig@gmail.com" },
 ]
 description = "Development Web Server for Qt for Webassembly"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qtwasmserver-0.1.1/PKG-INFO` & `qtwasmserver-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtwasmserver
-Version: 0.1.1
+Version: 0.1.2
 Summary: Development Web Server for Qt for Webassembly
 Project-URL: Homepage, https://github.com/msorvig/qtwasmserver
 Project-URL: Bug Tracker, https://github.com/msorvig/qtwasmserver/issues
 Author-email: Morten Sørvig <msorvig@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

