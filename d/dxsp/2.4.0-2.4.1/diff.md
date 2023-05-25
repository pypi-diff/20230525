# Comparing `tmp/dxsp-2.4.0.tar.gz` & `tmp/dxsp-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.4.0.tar", max compression
+gzip compressed data, was "dxsp-2.4.1.tar", max compression
```

## Comparing `dxsp-2.4.0.tar` & `dxsp-2.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-25 14:02:49.751742 dxsp-2.4.0/LICENSE
--rw-r--r--   0        0        0     2439 2023-05-25 14:02:49.751742 dxsp-2.4.0/README.md
--rw-r--r--   0        0        0       86 2023-05-25 14:02:50.415747 dxsp-2.4.0/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-25 14:02:49.751742 dxsp-2.4.0/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-25 14:02:49.751742 dxsp-2.4.0/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-25 14:02:49.751742 dxsp-2.4.0/dxsp/config.py
--rw-r--r--   0        0        0     3583 2023-05-25 14:02:49.751742 dxsp-2.4.0/dxsp/default_settings.toml
--rw-r--r--   0        0        0    20509 2023-05-25 14:02:49.751742 dxsp-2.4.0/dxsp/main.py
--rw-r--r--   0        0        0     1973 2023-05-25 14:02:50.415747 dxsp-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 dxsp-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-25 17:36:55.652250 dxsp-2.4.1/LICENSE
+-rw-r--r--   0        0        0     2439 2023-05-25 17:36:55.652250 dxsp-2.4.1/README.md
+-rw-r--r--   0        0        0       86 2023-05-25 17:36:56.324249 dxsp-2.4.1/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-25 17:36:55.652250 dxsp-2.4.1/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-25 17:36:55.652250 dxsp-2.4.1/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-25 17:36:55.652250 dxsp-2.4.1/dxsp/config.py
+-rw-r--r--   0        0        0     3583 2023-05-25 17:36:55.652250 dxsp-2.4.1/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    20388 2023-05-25 17:36:55.652250 dxsp-2.4.1/dxsp/main.py
+-rw-r--r--   0        0        0     1973 2023-05-25 17:36:56.324249 dxsp-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 dxsp-2.4.1/PKG-INFO
```

### Comparing `dxsp-2.4.0/LICENSE` & `dxsp-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.4.0/README.md` & `dxsp-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.4.0/dxsp/assets/blockchains.py` & `dxsp-2.4.1/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.4.0/dxsp/default_settings.toml` & `dxsp-2.4.1/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-2.4.0/dxsp/main.py` & `dxsp-2.4.1/dxsp/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,72 +115,68 @@
                     await self.get_confirmation(order_hash)
 
         except Exception as e:
             self.logger.error("Error in get_swap: %s", e)
             return e
 
     async def get_confirmation(self, order_hash):
-        """Returns trade confirmation"""
+        """Returns trade confirmation."""
         try:
             receipt = self.w3.eth.get_transaction(order_hash)
-            block = self.w3.eth.get_block(receipt['blockNumber'])
+            block = self.w3.eth.get_block(receipt["blockNumber"])
             trade = {
-                'timestamp': block['timestamp'],
-                'id': receipt['blockHash'],
-                'instrument': receipt['to'],
-                'contract': receipt['to'],
-                'amount': receipt['value'],
-                'price': receipt['value'],  # TBD
-                'fee': receipt['gas'],
-                'confirmation': f"➕ Size: {round(receipt['value'], 4)}\n"
-                                f"⚫️ Entry: {round(receipt['value'], 4)}\n"
-                                f"ℹ️ {receipt['blockHash']}\n"
-                                f"🗓️ {block['timestamp']}"
+                "timestamp": block["timestamp"],
+                "id": receipt["blockHash"],
+                "instrument": receipt["to"],
+                "contract": receipt["to"],
+                "amount": receipt["value"],
+                "price": receipt["value"],  # To be determined.
+                "fee": receipt["gas"],
+                "confirmation": (
+                    f"➕ Size: {round(receipt['value'], 4)}\n"
+                    f"⚫️ Entry: {round(receipt['value'], 4)}\n"
+                    f"ℹ️ {receipt['blockHash']}\n"
+                    f"🗓️ {block['timestamp']}"
+                ),
             }
             return trade
         except Exception as e:
-            self.logger.error("Error getting trade confirmation %s", e)
-            return
+            self.logger.error("Error getting trade confirmation: %s", e)
 
     async def execute_order(self, order_params):
-        """execute swap function"""
+        """Execute swap function."""
         action = order_params.get('action')
         instrument = order_params.get('instrument')
         quantity = order_params.get('quantity', 1)
 
         try:
-            asset_out_symbol = (
-                settings.trading_quote_ccy if
-                action == "BUY" else instrument)
-            asset_in_symbol = (
-                instrument if action == "BUY"
-                else settings.trading_quote_ccy)
+            if action == "BUY":
+                asset_out_symbol = settings.trading_quote_ccy
+                asset_in_symbol = instrument
+            else:
+                asset_out_symbol = instrument
+                asset_in_symbol = settings.trading_quote_ccy
+
             try:
-                asset_out_contract = await self.get_token_contract(
-                    asset_out_symbol)
-                asset_out_decimals = (
-                    asset_out_contract.functions.decimals().call()
-                    or 18)
+                asset_out_contract = await self.get_token_contract(asset_out_symbol)
+                asset_out_decimals = asset_out_contract.functions.decimals().call() or 18
             except Exception as e:
                 self.logger.error("execute_order decimals: %s", e)
                 asset_out_decimals = 18
+
             asset_out_balance = await self.get_token_balance(asset_out_symbol)
 
-            #  Amount to risk percentage - DEFAULT OPTION is 10%
-            asset_out_amount = (
-                (asset_out_balance) /
-                (settings.trading_risk_amount
-                 ** asset_out_decimals)
-                )*(float(quantity)/100)
+            # Amount to risk percentage - DEFAULT OPTION is 10%
+            asset_out_amount = (asset_out_balance / (settings.trading_risk_amount ** asset_out_decimals)) * (float(quantity) / 100)
 
             order = await self.get_swap(
-                    asset_out_symbol,
-                    asset_in_symbol,
-                    asset_out_amount
-                    )
+                asset_out_symbol,
+                asset_in_symbol,
+                asset_out_amount
+            )
             if order:
                 return order['confirmation']
 
         except Exception as e:
             self.logger.debug("error execute_order %s", e)
             return "error processing order in DXSP"
 
@@ -321,20 +317,19 @@
                     settings.dex_quoter_contract_addr),
                 abi=quoter_abi)
             return contract
         except Exception as e:
             self.logger.error("quoter setup: %s", e)
 
     async def get_approve(self, symbol):
-
         try:
             if self.protocol_type in ["uniswap_v2", "uniswap_v3"]:
                 await self.get_approve_uniswap(symbol)
         except Exception as e:
-            self.logger.error("get_approve %s", e)
+            self.logger.error("Error in get_approve: %s", e)
             return None
 
     async def get_sign(self, transaction):
         try:
             if self.protocol_type in ['uniswap_v2', 'uniswap_v3']:
                 transaction_params = {
                     'from': self.wallet_address,
@@ -460,15 +455,15 @@
                     settings.trading_quote_ccy)
         except Exception as e:
             self.logger.error("get_quote_uniswap %s", e)
             return
 
     async def get_approve_uniswap(self, symbol):
         try:
-            contract = self.get_token_contract(symbol)
+            contract = await self.get_token_contract(symbol)
             approved_amount = self.w3.to_wei(2**64-1, 'ether')
             approval_check = contract.functions.allowance(
                 self.w3.to_checksum_address(self.wallet_address),
                 self.w3.to_checksum_address(settings.dex_router_contract_addr)
             ).call()
             if approval_check == 0:
                 approval_transaction = contract.functions.approve(
```

### Comparing `dxsp-2.4.0/pyproject.toml` & `dxsp-2.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.4.0"
+version = "2.4.1"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-2.4.0/PKG-INFO` & `dxsp-2.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.4.0
+Version: 2.4.1
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

