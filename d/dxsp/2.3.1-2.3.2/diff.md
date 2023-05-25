# Comparing `tmp/dxsp-2.3.1.tar.gz` & `tmp/dxsp-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.3.1.tar", max compression
+gzip compressed data, was "dxsp-2.3.2.tar", max compression
```

## Comparing `dxsp-2.3.1.tar` & `dxsp-2.3.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-24 14:56:23.577067 dxsp-2.3.1/LICENSE
--rw-r--r--   0        0        0     2439 2023-05-24 14:56:23.581067 dxsp-2.3.1/README.md
--rw-r--r--   0        0        0       86 2023-05-24 14:56:24.453069 dxsp-2.3.1/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-24 14:56:23.581067 dxsp-2.3.1/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-24 14:56:23.581067 dxsp-2.3.1/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-24 14:56:23.581067 dxsp-2.3.1/dxsp/config.py
--rw-r--r--   0        0        0     3552 2023-05-24 14:56:23.581067 dxsp-2.3.1/dxsp/default_settings.toml
--rw-r--r--   0        0        0    26416 2023-05-24 14:56:23.581067 dxsp-2.3.1/dxsp/main.py
--rw-r--r--   0        0        0     1973 2023-05-24 14:56:24.453069 dxsp-2.3.1/pyproject.toml
--rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 dxsp-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-24 15:32:40.483287 dxsp-2.3.2/LICENSE
+-rw-r--r--   0        0        0     2439 2023-05-24 15:32:40.483287 dxsp-2.3.2/README.md
+-rw-r--r--   0        0        0       86 2023-05-24 15:32:41.159287 dxsp-2.3.2/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-24 15:32:40.483287 dxsp-2.3.2/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-24 15:32:40.483287 dxsp-2.3.2/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-24 15:32:40.483287 dxsp-2.3.2/dxsp/config.py
+-rw-r--r--   0        0        0     3552 2023-05-24 15:32:40.483287 dxsp-2.3.2/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    26438 2023-05-24 15:32:40.483287 dxsp-2.3.2/dxsp/main.py
+-rw-r--r--   0        0        0     1973 2023-05-24 15:32:41.159287 dxsp-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 dxsp-2.3.2/PKG-INFO
```

### Comparing `dxsp-2.3.1/LICENSE` & `dxsp-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.3.1/README.md` & `dxsp-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.3.1/dxsp/assets/blockchains.py` & `dxsp-2.3.2/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.3.1/dxsp/default_settings.toml` & `dxsp-2.3.2/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-2.3.1/dxsp/main.py` & `dxsp-2.3.2/dxsp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -434,20 +434,21 @@
         # Log the transaction
         self.logger.debug("get_gas %s", tx)
         # Estimate the gas cost of the transaction
         gasestimate = self.w3.eth.estimate_gas(tx) * 1.25
         # Return the estimated gas cost in wei
         return int(self.w3.to_wei(gasestimate, 'wei'))
 
-    async def get_gasPrice(self, tx):
+    async def get_gasPrice(self):
         '''
         Get the gas price for a transaction
         '''
         gasprice = self.w3.eth.generate_gas_price()
-        return self.w3.to_wei(gasprice, 'gwei')
+        return gasprice
+        # return self.w3.to_wei(gasprice, 'gwei')
 
     async def get_abi(self, addr):
         # Log a debug message to the logger
         self.logger.debug("get_abi %s", addr)
         if settings.dex_block_explorer_api:
             try:
                 # Create a dictionary of parameters
```

### Comparing `dxsp-2.3.1/pyproject.toml` & `dxsp-2.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.3.1"
+version = "2.3.2"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-2.3.1/PKG-INFO` & `dxsp-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.3.1
+Version: 2.3.2
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

