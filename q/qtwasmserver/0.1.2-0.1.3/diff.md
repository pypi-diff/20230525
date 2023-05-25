# Comparing `tmp/qtwasmserver-0.1.2.tar.gz` & `tmp/qtwasmserver-0.1.3.tar.gz`

## Comparing `qtwasmserver-0.1.2.tar` & `qtwasmserver-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 qtwasmserver-0.1.2/build
--rwxr-xr-x   0        0        0     9921 2020-02-02 00:00:00.000000 qtwasmserver-0.1.2/src/qtwasmserver/qtwasmserver.py
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 qtwasmserver-0.1.2/src/qtwasmserver/setup.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 qtwasmserver-0.1.2/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 qtwasmserver-0.1.2/LICENSE
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 qtwasmserver-0.1.2/README.md
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 qtwasmserver-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 qtwasmserver-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 qtwasmserver-0.1.3/build
+-rwxr-xr-x   0        0        0     9921 2020-02-02 00:00:00.000000 qtwasmserver-0.1.3/src/qtwasmserver/qtwasmserver.py
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 qtwasmserver-0.1.3/src/qtwasmserver/setup.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 qtwasmserver-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 qtwasmserver-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 qtwasmserver-0.1.3/README.md
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 qtwasmserver-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 qtwasmserver-0.1.3/PKG-INFO
```

### Comparing `qtwasmserver-0.1.2/src/qtwasmserver/qtwasmserver.py` & `qtwasmserver-0.1.3/src/qtwasmserver/qtwasmserver.py`

 * *Files identical despite different names*

### Comparing `qtwasmserver-0.1.2/LICENSE` & `qtwasmserver-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qtwasmserver-0.1.2/README.md` & `qtwasmserver-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ## Qt for WebAssembly development server. 
 
 This server is intented to be used while developing and testing WebAssembly applications on a
-trusted network. It is not suitable for production use, i.e. distributing applicaitons to end
-users over public networks.
+trusted network. It is not suitable for production use cases like distributing applicaitons
+to end users over public networks.
 
 The server is an upgrade from the python one line server ("python -m http.server"), and offers the
 following features:
 
 * Zero-configuration / minimal configuration.
 
 * Support for binding to multiple addresses in addition to localhost. This is useful
@@ -54,10 +54,10 @@
 The basic flow is:
 
  1. Gereate a certificate authority (CA), and install that on all devices and browsers.
     This is a one time operation. mkcert will use thuis CA to sign certificates.
  2. Generate a certificate for each address you want to use. This is done automatically
     by this server.
 
-The main beneifit of this appraoch is that certificates can be generated locally on demand,
-which can be useful when for instance when moving a development machine between home and office
-networks.
+The beneifit of this appraoch is that certificates can be generated locally, on demand,
+for each server address in use. This can be useful when for instance moving a development
+machine between home and office networks.
```

### Comparing `qtwasmserver-0.1.2/pyproject.toml` & `qtwasmserver-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "qtwasmserver"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Morten Sørvig", email="msorvig@gmail.com" },
 ]
 description = "Development Web Server for Qt for Webassembly"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `qtwasmserver-0.1.2/PKG-INFO` & `qtwasmserver-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtwasmserver
-Version: 0.1.2
+Version: 0.1.3
 Summary: Development Web Server for Qt for Webassembly
 Project-URL: Homepage, https://github.com/msorvig/qtwasmserver
 Project-URL: Bug Tracker, https://github.com/msorvig/qtwasmserver/issues
 Author-email: Morten Sørvig <msorvig@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,16 +14,16 @@
 Requires-Dist: httpcompressionserver>=0.5
 Requires-Dist: netifaces>=0.10
 Description-Content-Type: text/markdown
 
 ## Qt for WebAssembly development server. 
 
 This server is intented to be used while developing and testing WebAssembly applications on a
-trusted network. It is not suitable for production use, i.e. distributing applicaitons to end
-users over public networks.
+trusted network. It is not suitable for production use cases like distributing applicaitons
+to end users over public networks.
 
 The server is an upgrade from the python one line server ("python -m http.server"), and offers the
 following features:
 
 * Zero-configuration / minimal configuration.
 
 * Support for binding to multiple addresses in addition to localhost. This is useful
@@ -71,10 +71,10 @@
 The basic flow is:
 
  1. Gereate a certificate authority (CA), and install that on all devices and browsers.
     This is a one time operation. mkcert will use thuis CA to sign certificates.
  2. Generate a certificate for each address you want to use. This is done automatically
     by this server.
 
-The main beneifit of this appraoch is that certificates can be generated locally on demand,
-which can be useful when for instance when moving a development machine between home and office
-networks.
+The beneifit of this appraoch is that certificates can be generated locally, on demand,
+for each server address in use. This can be useful when for instance moving a development
+machine between home and office networks.
```

