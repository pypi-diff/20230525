# Comparing `tmp/verifit-3.0.1.tar.gz` & `tmp/verifit-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verifit-3.0.1.tar", last modified: Wed Apr 26 08:32:43 2023, max compression
+gzip compressed data, was "verifit-3.0.2.tar", last modified: Thu May 25 13:39:37 2023, max compression
```

## Comparing `verifit-3.0.1.tar` & `verifit-3.0.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2023-04-26 08:32:43.075963 verifit-3.0.1/
--rw-r--r--   0 sorel      (501) staff       (20)     1067 2022-08-11 12:38:58.000000 verifit-3.0.1/LICENSE
--rw-r--r--   0 sorel      (501) staff       (20)       67 2023-03-06 16:27:14.000000 verifit-3.0.1/MANIFEST.in
--rw-r--r--   0 sorel      (501) staff       (20)    11465 2023-04-26 08:32:43.075783 verifit-3.0.1/PKG-INFO
--rw-r--r--   0 sorel      (501) staff       (20)     9668 2023-04-26 08:27:28.000000 verifit-3.0.1/Readme.md
--rw-r--r--   0 sorel      (501) staff       (20)     1020 2023-04-26 08:32:32.000000 verifit-3.0.1/pyproject.toml
--rw-r--r--   0 sorel      (501) staff       (20)      114 2023-04-26 07:14:27.000000 verifit-3.0.1/requirements.txt
--rw-r--r--   0 sorel      (501) staff       (20)       38 2023-04-26 08:32:43.076004 verifit-3.0.1/setup.cfg
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2023-04-26 08:32:43.071468 verifit-3.0.1/src/
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2023-04-26 08:32:43.074898 verifit-3.0.1/src/verifit/
--rw-r--r--   0 sorel      (501) staff       (20)      204 2023-04-26 08:31:59.000000 verifit-3.0.1/src/verifit/__init__.py
--rw-r--r--   0 sorel      (501) staff       (20)     1405 2023-03-31 17:39:37.000000 verifit-3.0.1/src/verifit/cache.py
--rw-r--r--   0 sorel      (501) staff       (20)      698 2023-03-31 17:39:37.000000 verifit-3.0.1/src/verifit/config.py
--rw-r--r--   0 sorel      (501) staff       (20)      295 2023-03-14 17:26:30.000000 verifit-3.0.1/src/verifit/date_diff.py
--rw-r--r--   0 sorel      (501) staff       (20)      441 2023-03-15 15:10:31.000000 verifit-3.0.1/src/verifit/json_web_token.py
--rw-r--r--   0 sorel      (501) staff       (20)     2674 2023-04-26 08:00:17.000000 verifit-3.0.1/src/verifit/login.py
--rw-r--r--   0 sorel      (501) staff       (20)      407 2023-04-03 13:23:28.000000 verifit-3.0.1/src/verifit/memoize.py
--rw-r--r--   0 sorel      (501) staff       (20)      310 2023-03-27 10:54:45.000000 verifit-3.0.1/src/verifit/prop.py
--rw-r--r--   0 sorel      (501) staff       (20)     2059 2023-04-01 15:01:48.000000 verifit-3.0.1/src/verifit/retrieve.py
--rw-r--r--   0 sorel      (501) staff       (20)     2068 2023-03-24 18:38:29.000000 verifit-3.0.1/src/verifit/web_sockets.py
-drwxr-xr-x   0 sorel      (501) staff       (20)        0 2023-04-26 08:32:43.075592 verifit-3.0.1/verifit.egg-info/
--rw-r--r--   0 sorel      (501) staff       (20)    11465 2023-04-26 08:32:43.000000 verifit-3.0.1/verifit.egg-info/PKG-INFO
--rw-r--r--   0 sorel      (501) staff       (20)      452 2023-04-26 08:32:43.000000 verifit-3.0.1/verifit.egg-info/SOURCES.txt
--rw-r--r--   0 sorel      (501) staff       (20)        1 2023-04-26 08:32:43.000000 verifit-3.0.1/verifit.egg-info/dependency_links.txt
--rw-r--r--   0 sorel      (501) staff       (20)       87 2023-04-26 08:32:43.000000 verifit-3.0.1/verifit.egg-info/requires.txt
--rw-r--r--   0 sorel      (501) staff       (20)        8 2023-04-26 08:32:43.000000 verifit-3.0.1/verifit.egg-info/top_level.txt
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2023-05-25 13:39:37.349845 verifit-3.0.2/
+-rw-r--r--   0 sorel      (501) staff       (20)     1067 2023-05-25 10:42:33.000000 verifit-3.0.2/LICENSE
+-rw-r--r--   0 sorel      (501) staff       (20)       67 2023-05-25 10:42:33.000000 verifit-3.0.2/MANIFEST.in
+-rw-r--r--   0 sorel      (501) staff       (20)    13505 2023-05-25 13:39:37.349630 verifit-3.0.2/PKG-INFO
+-rw-r--r--   0 sorel      (501) staff       (20)    11708 2023-05-25 13:30:18.000000 verifit-3.0.2/Readme.md
+-rw-r--r--   0 sorel      (501) staff       (20)     1020 2023-05-25 13:32:06.000000 verifit-3.0.2/pyproject.toml
+-rw-r--r--   0 sorel      (501) staff       (20)      114 2023-05-25 10:42:33.000000 verifit-3.0.2/requirements.txt
+-rw-r--r--   0 sorel      (501) staff       (20)       38 2023-05-25 13:39:37.349889 verifit-3.0.2/setup.cfg
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2023-05-25 13:39:37.346028 verifit-3.0.2/src/
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2023-05-25 13:39:37.348558 verifit-3.0.2/src/verifit/
+-rw-r--r--   0 sorel      (501) staff       (20)      204 2023-05-25 10:42:33.000000 verifit-3.0.2/src/verifit/__init__.py
+-rw-r--r--   0 sorel      (501) staff       (20)     1405 2023-05-25 10:42:33.000000 verifit-3.0.2/src/verifit/cache.py
+-rw-r--r--   0 sorel      (501) staff       (20)      698 2023-05-25 10:42:33.000000 verifit-3.0.2/src/verifit/config.py
+-rw-r--r--   0 sorel      (501) staff       (20)      295 2023-05-25 10:42:33.000000 verifit-3.0.2/src/verifit/date_diff.py
+-rw-r--r--   0 sorel      (501) staff       (20)      373 2023-05-25 13:20:47.000000 verifit-3.0.2/src/verifit/driver.py
+-rw-r--r--   0 sorel      (501) staff       (20)      441 2023-05-25 10:42:33.000000 verifit-3.0.2/src/verifit/json_web_token.py
+-rw-r--r--   0 sorel      (501) staff       (20)     2674 2023-05-25 10:42:33.000000 verifit-3.0.2/src/verifit/login.py
+-rw-r--r--   0 sorel      (501) staff       (20)      407 2023-05-25 10:42:33.000000 verifit-3.0.2/src/verifit/memoize.py
+-rw-r--r--   0 sorel      (501) staff       (20)      310 2023-05-25 10:42:33.000000 verifit-3.0.2/src/verifit/prop.py
+-rw-r--r--   0 sorel      (501) staff       (20)     2059 2023-05-25 10:42:33.000000 verifit-3.0.2/src/verifit/retrieve.py
+-rw-r--r--   0 sorel      (501) staff       (20)     2068 2023-05-25 10:42:33.000000 verifit-3.0.2/src/verifit/web_sockets.py
+drwxr-xr-x   0 sorel      (501) staff       (20)        0 2023-05-25 13:39:37.349397 verifit-3.0.2/verifit.egg-info/
+-rw-r--r--   0 sorel      (501) staff       (20)    13505 2023-05-25 13:39:37.000000 verifit-3.0.2/verifit.egg-info/PKG-INFO
+-rw-r--r--   0 sorel      (501) staff       (20)      474 2023-05-25 13:39:37.000000 verifit-3.0.2/verifit.egg-info/SOURCES.txt
+-rw-r--r--   0 sorel      (501) staff       (20)        1 2023-05-25 13:39:37.000000 verifit-3.0.2/verifit.egg-info/dependency_links.txt
+-rw-r--r--   0 sorel      (501) staff       (20)       87 2023-05-25 13:39:37.000000 verifit-3.0.2/verifit.egg-info/requires.txt
+-rw-r--r--   0 sorel      (501) staff       (20)        8 2023-05-25 13:39:37.000000 verifit-3.0.2/verifit.egg-info/top_level.txt
```

### Comparing `verifit-3.0.1/LICENSE` & `verifit-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `verifit-3.0.1/PKG-INFO` & `verifit-3.0.2/Readme.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,7 @@
-Metadata-Version: 2.1
-Name: verifit
-Version: 3.0.1
-Summary: Verify It: Automatic Testing helper tools & sample tests
-Author-email: Sorel Mitra <sorelmitra@yahoo.com>
-License: MIT License
-        
-        Copyright (c) 2022 sorelmitra
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/sorelmitra/verifit
-Keywords: automatic testing,acceptance testing,bdd,Gherkin,black box testing
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # About
 
 This is a Python library aimed at developers, that simplifies setting up and using automatic system testing for several types of projects.
 
 I've named it `verifit` as a contraction of `Verify It!`, i.e. "Make sure your system works fine!"
 
 
@@ -113,32 +76,64 @@
 
 ### 2.2. Sample Tests
 
 The sample tests use dummy online services or commands in order to show how to test various types of applications, and how to use our lib: 
 
 1. `post_service/post/test_post.py`. Tests simple APIs using HTTP and GraphQL servers.
 
-2. `shopping_service/login/test_login.py`. Here we test log in to a server.
+2. `post_service/drivers/test_post_via_drivers.py`. The same as `test_post.py`, but showcasing using different drivers.
+
+   If you need to run your tests through multiple channels, then it's best if you keep your tests unified, and add a couple of layers to help directing the tests through the right channel.
+
+    Assume you need to 'Post' items via two channels, 'foo', and 'bar'.  The layers would be:
+    
+    1. Test declaration
+    	- Does the actual testing, 'Posting' an item and verifying the result
+    	- Does not call directly to 'foo' or 'bar'
+    	- Calls to a Domain-Specific Language, aka DSL
+    2. DSL implementation
+    	- Based on the 'driver' parameter, it calls either to 'foo' or 'bar'
+    3. Drivers implementation
+    	- Each driver 'Posts' items in the way it knows
+    	- There is one driver implementation for each channel, i.e., 'foo' and 'bar'
+        - If 'bar' cannot 'Post' an item, then the corresponding driver is missing 
+
+    The files:
+
+    - `drivers.py` contains the list of our particular drivers
+    - The test itself is straightforward, as it imports the DSL, calls it, and verifies the result.  Note that the test is skipped for the 'bar' driver, because in our example, we are pretending that the 'bar' channel has no way to 'Post an item.
+    - `dsl_post.py`: The DSL uses the driver lib to call to the right driver from a driver map it provides.  In our case, the 'foo' driver is omitted from the map, because we know it cannot create an 'Item'.
+    - `driver_foo.py`: The 'foo' driver to 'Post' an item.  The 'bar' driver to 'Post' an item does not exist, as it cannot perform this action.
+
+    To run this test via the 'bar' driver, do this:
+
+    ```
+    DRIVER=bar pytest . -k 'post'
+    ```
+   
+    By default, `DRIVER` is `foo`.
+
+3. `shopping_service/login/test_login.py`. Here we test log in to a server.
 
-3. `shopping_service/login/test_products.py`. This one does the following:
+4. `shopping_service/login/test_products.py`. This one does the following:
 
    - Log in from cache.  This returns the cached token if it is valid, or logs in and caches the token before returning it.
    - Call to a private endpoint, passing in an authorization header with a cached access token.
 
-4. `shopping_service/login/test_carts.py`. It shows Gherkin features and BDD.
+5. `shopping_service/login/test_carts.py`. It shows Gherkin features and BDD.
 
-5. `echo_service/test_echo_service.py`.  Shows how to simplify testing WebSockets using our library.
+6. `echo_service/test_echo_service.py`.  Shows how to simplify testing WebSockets using our library.
 
     **Note**: As of _2023-04-26_, the online server that we were using for this sample test stopped accepting the API key that they provide.  As a result, we've marked this test as skipped.
 
-6. `date_service/test_date.py`.  Shows how to test CLI programs using this lib: it runs the shell command `date` with some arguments, and verifies the resulting output.
+7. `date_service/test_date.py`.  Shows how to test CLI programs using this lib: it runs the shell command `date` with some arguments, and verifies the resulting output.
 
-7. `self_check/test_self.py`.  Tests the lib itself.
+8. `self_check/test_self.py`.  Tests the lib itself.
 
-8. `kitchen_service/test_kitchen_service.py`.  Showcase doing a Web UI test using Cypress.IO and their kitchen sink sample page.
+9. `kitchen_service/test_kitchen_service.py`.  Showcase doing a Web UI test using Cypress.IO and their kitchen sink sample page.
 
 To prepare for running the sample tests that are included with this project, do this:
 
 ```shell
 cd tests
 pip install -r requirements.txt
 ```
@@ -174,14 +169,18 @@
 - No global variables, not even a singleton - memoize takes care of this.
 
 ## Helpers
 
 - `cache.py`.  Implements a simple cache, that is being stored in a file named `.<env>-cache.json` from the `tests` directory.
 - `config.py`.  Loads configuration via the `dotenv` package, and returns a unique store for getting/setting values across tests.
 - `date_diff.py`.  Simple date diff.
+- `driver.py`.  The driver lib is pretty simple:
+    - It gets the current driver from the environment
+    - It calls the corresponding function from a driver name / function dict
+    - It also offers a helper function to skip a test for a particular driver
 - `json_web_token.py`.  Decoding and extracting data from a JWT.
 - `login.py`.  Functions to:
     - Log in using a driver, which is a plain function.  We use a driver for this because logging in is particular to the API that each project has.  The driver does the actual call to the API endpoint for login, and returns the access token.  The framework caches the access token and its expiration date.
     - Log in from a cached token using a driver.
     - Building authorization values:
       - For HTTP headers.
       - For the Python GraphQL client.
```

### Comparing `verifit-3.0.1/pyproject.toml` & `verifit-3.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 packages = ['verifit']
 
 [tool.check-manifest]
 ignore = [".pytest_cache/*", "node_modules/**/*"]
 
 [project]
 name = "verifit"
-version = "3.0.1"
+version = "3.0.2"
 description = "Verify It: Automatic Testing helper tools & sample tests"
 readme = "Readme.md"
 authors = [{ name = "Sorel Mitra", email = "sorelmitra@yahoo.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `verifit-3.0.1/src/verifit/cache.py` & `verifit-3.0.2/src/verifit/cache.py`

 * *Files identical despite different names*

### Comparing `verifit-3.0.1/src/verifit/config.py` & `verifit-3.0.2/src/verifit/config.py`

 * *Files identical despite different names*

### Comparing `verifit-3.0.1/src/verifit/login.py` & `verifit-3.0.2/src/verifit/login.py`

 * *Files identical despite different names*

### Comparing `verifit-3.0.1/src/verifit/retrieve.py` & `verifit-3.0.2/src/verifit/retrieve.py`

 * *Files identical despite different names*

### Comparing `verifit-3.0.1/src/verifit/web_sockets.py` & `verifit-3.0.2/src/verifit/web_sockets.py`

 * *Files identical despite different names*

### Comparing `verifit-3.0.1/verifit.egg-info/PKG-INFO` & `verifit-3.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: verifit
-Version: 3.0.1
+Version: 3.0.2
 Summary: Verify It: Automatic Testing helper tools & sample tests
 Author-email: Sorel Mitra <sorelmitra@yahoo.com>
 License: MIT License
         
         Copyright (c) 2022 sorelmitra
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -113,32 +113,64 @@
 
 ### 2.2. Sample Tests
 
 The sample tests use dummy online services or commands in order to show how to test various types of applications, and how to use our lib: 
 
 1. `post_service/post/test_post.py`. Tests simple APIs using HTTP and GraphQL servers.
 
-2. `shopping_service/login/test_login.py`. Here we test log in to a server.
+2. `post_service/drivers/test_post_via_drivers.py`. The same as `test_post.py`, but showcasing using different drivers.
 
-3. `shopping_service/login/test_products.py`. This one does the following:
+   If you need to run your tests through multiple channels, then it's best if you keep your tests unified, and add a couple of layers to help directing the tests through the right channel.
+
+    Assume you need to 'Post' items via two channels, 'foo', and 'bar'.  The layers would be:
+    
+    1. Test declaration
+    	- Does the actual testing, 'Posting' an item and verifying the result
+    	- Does not call directly to 'foo' or 'bar'
+    	- Calls to a Domain-Specific Language, aka DSL
+    2. DSL implementation
+    	- Based on the 'driver' parameter, it calls either to 'foo' or 'bar'
+    3. Drivers implementation
+    	- Each driver 'Posts' items in the way it knows
+    	- There is one driver implementation for each channel, i.e., 'foo' and 'bar'
+        - If 'bar' cannot 'Post' an item, then the corresponding driver is missing 
+
+    The files:
+
+    - `drivers.py` contains the list of our particular drivers
+    - The test itself is straightforward, as it imports the DSL, calls it, and verifies the result.  Note that the test is skipped for the 'bar' driver, because in our example, we are pretending that the 'bar' channel has no way to 'Post an item.
+    - `dsl_post.py`: The DSL uses the driver lib to call to the right driver from a driver map it provides.  In our case, the 'foo' driver is omitted from the map, because we know it cannot create an 'Item'.
+    - `driver_foo.py`: The 'foo' driver to 'Post' an item.  The 'bar' driver to 'Post' an item does not exist, as it cannot perform this action.
+
+    To run this test via the 'bar' driver, do this:
+
+    ```
+    DRIVER=bar pytest . -k 'post'
+    ```
+   
+    By default, `DRIVER` is `foo`.
+
+3. `shopping_service/login/test_login.py`. Here we test log in to a server.
+
+4. `shopping_service/login/test_products.py`. This one does the following:
 
    - Log in from cache.  This returns the cached token if it is valid, or logs in and caches the token before returning it.
    - Call to a private endpoint, passing in an authorization header with a cached access token.
 
-4. `shopping_service/login/test_carts.py`. It shows Gherkin features and BDD.
+5. `shopping_service/login/test_carts.py`. It shows Gherkin features and BDD.
 
-5. `echo_service/test_echo_service.py`.  Shows how to simplify testing WebSockets using our library.
+6. `echo_service/test_echo_service.py`.  Shows how to simplify testing WebSockets using our library.
 
     **Note**: As of _2023-04-26_, the online server that we were using for this sample test stopped accepting the API key that they provide.  As a result, we've marked this test as skipped.
 
-6. `date_service/test_date.py`.  Shows how to test CLI programs using this lib: it runs the shell command `date` with some arguments, and verifies the resulting output.
+7. `date_service/test_date.py`.  Shows how to test CLI programs using this lib: it runs the shell command `date` with some arguments, and verifies the resulting output.
 
-7. `self_check/test_self.py`.  Tests the lib itself.
+8. `self_check/test_self.py`.  Tests the lib itself.
 
-8. `kitchen_service/test_kitchen_service.py`.  Showcase doing a Web UI test using Cypress.IO and their kitchen sink sample page.
+9. `kitchen_service/test_kitchen_service.py`.  Showcase doing a Web UI test using Cypress.IO and their kitchen sink sample page.
 
 To prepare for running the sample tests that are included with this project, do this:
 
 ```shell
 cd tests
 pip install -r requirements.txt
 ```
@@ -174,14 +206,18 @@
 - No global variables, not even a singleton - memoize takes care of this.
 
 ## Helpers
 
 - `cache.py`.  Implements a simple cache, that is being stored in a file named `.<env>-cache.json` from the `tests` directory.
 - `config.py`.  Loads configuration via the `dotenv` package, and returns a unique store for getting/setting values across tests.
 - `date_diff.py`.  Simple date diff.
+- `driver.py`.  The driver lib is pretty simple:
+    - It gets the current driver from the environment
+    - It calls the corresponding function from a driver name / function dict
+    - It also offers a helper function to skip a test for a particular driver
 - `json_web_token.py`.  Decoding and extracting data from a JWT.
 - `login.py`.  Functions to:
     - Log in using a driver, which is a plain function.  We use a driver for this because logging in is particular to the API that each project has.  The driver does the actual call to the API endpoint for login, and returns the access token.  The framework caches the access token and its expiration date.
     - Log in from a cached token using a driver.
     - Building authorization values:
       - For HTTP headers.
       - For the Python GraphQL client.
```

