# Comparing `tmp/tap_exact-0.3.3.tar.gz` & `tmp/tap_exact-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_exact-0.3.3.tar", max compression
+gzip compressed data, was "tap_exact-0.4.0.tar", max compression
```

## Comparing `tap_exact-0.3.3.tar` & `tap_exact-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      932 2023-05-17 16:27:14.161580 tap_exact-0.3.3/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.3.3/tap_exact/__init__.py
--rw-r--r--   0        0        0      842 2023-04-20 11:44:26.669328 tap_exact-0.3.3/tap_exact/client.py
--rw-r--r--   0        0        0    33433 2023-05-17 16:25:35.741580 tap_exact-0.3.3/tap_exact/streams.py
--rw-r--r--   0        0        0     1727 2023-05-17 16:28:37.291580 tap_exact-0.3.3/tap_exact/tap.py
--rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.3.3/tap_exact/tests/__init__.py
--rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.3.3/tap_exact/tests/test_core.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.3.3/setup.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      932 2023-05-25 08:57:52.556947 tap_exact-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.4.0/tap_exact/__init__.py
+-rw-r--r--   0        0        0     2661 2023-05-25 09:03:37.456947 tap_exact-0.4.0/tap_exact/client.py
+-rw-r--r--   0        0        0    27526 2023-05-25 09:04:32.326947 tap_exact-0.4.0/tap_exact/streams.py
+-rw-r--r--   0        0        0     1727 2023-05-25 08:12:48.176947 tap_exact-0.4.0/tap_exact/tap.py
+-rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.4.0/tap_exact/tests/__init__.py
+-rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.4.0/tap_exact/tests/test_core.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.4.0/setup.py
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.4.0/PKG-INFO
```

### Comparing `tap_exact-0.3.3/pyproject.toml` & `tap_exact-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-exact"
-version = "0.3.3"
+version = "0.4.0"
 description = "`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK."
 authors = ["Janick Otten"]
 keywords = [
     "ELT",
     "Exact Online",
 ]
 license = "Apache 2.0"
```

### Comparing `tap_exact-0.3.3/tap_exact/streams.py` & `tap_exact-0.4.0/tap_exact/streams.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from pathlib import Path
 from typing import Any, Dict, Optional, Union, List, Iterable
 
 from singer_sdk import typing as th  # JSON Schema typing helpers
 
 from tap_exact.client import ExactOnlineStream
-from exactonline.resource import GET
 
 from datetime import datetime
 
 # TODO: Delete this is if not using json files for schema definition
 SCHEMAS_DIR = Path(__file__).parent / Path("./schemas")
 # TODO: - Override `UsersStream` and `GroupsStream` with your own stream definition.
 #       - Copy-paste as many times as needed to create multiple stream types.
@@ -18,14 +17,15 @@
 
 class SalesInvoicesStream(ExactOnlineStream):
     """Define custom stream."""
 
     name = "sales_invoices"
     primary_keys = ["InvoiceID"]
     replication_key = "Modified"
+    date_fields = ['InvoiceDate', 'Modified', 'OrderDate']
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     # schema_filepath = SCHEMAS_DIR / "users.json"
     schema = th.PropertiesList(
         th.Property(
             "InvoiceID",
             th.StringType,
             description="The unique identifier of the invoice"
@@ -94,36 +94,21 @@
         
         path = "/salesinvoice/SalesInvoices?" \
             f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&" \
             "$select=InvoiceID,InvoiceDate,InvoiceNumber,InvoiceTo,InvoiceToName,OrderDate,OrderedBy,OrderedByName,Creator,AmountDC,AmountDiscount,Modified"
 
         return path
 
-    def get_records(self, context: Optional[dict]) -> Iterable[dict]:
-        """Return a generator or row-type dictionary objects"""
-        
-        resp = self.conn.rest(GET('v1/%d/%s' % (self.division, self.get_path(context) )))
-        
-        # The fields that have /Date(unixmilliseconds)/ objects that should be converted into datetime objects
-        keys = ['InvoiceDate', 'Modified', 'OrderDate']
-
-        for row in resp:
-            
-            # We loop through the keys that should be modified
-            for key in keys:
-                row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
-
-            yield row
-
 class PurchaseInvoicesStream(ExactOnlineStream):
     """Define custom stream."""
 
     name = "purchase_invoices"
     primary_keys = ["ID"]
     replication_key = "Modified"
+    date_fields = ['InvoiceDate', 'Modified', 'DueDate']
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     # schema_filepath = SCHEMAS_DIR / "users.json"
     schema = th.PropertiesList(
         th.Property(
             "ID",
             th.StringType,
             description="The unique identifier of the invoice"
@@ -192,36 +177,21 @@
         
         path = "/purchase/PurchaseInvoices?" \
             f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&" \
             "$select=ID,InvoiceDate,YourRef,Supplier,Description,DueDate,PaymentCondition,Status,Journal,Amount,VATAmount,Modified"
 
         return path
 
-    def get_records(self, context: Optional[dict]) -> Iterable[dict]:
-        """Return a generator or row-type dictionary objects"""
-        
-        resp = self.conn.rest(GET('v1/%d/%s' % (self.division, self.get_path(context) )))
-        
-        # The fields that have /Date(unixmilliseconds)/ objects that should be converted into datetime objects
-        keys = ['InvoiceDate', 'Modified', 'DueDate']
-
-        for row in resp:
-            
-            # We loop through the keys that should be modified
-            for key in keys:
-                row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
-
-            yield row
-
 class GeneralLedgerAccountsStream(ExactOnlineStream):
     """Define custom stream."""
 
     name = "general_ledger_accounts"
     primary_keys = ["ID"]
     replication_key = "Modified"
+    date_fields = ['Modified']
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     # schema_filepath = SCHEMAS_DIR / "users.json"
     schema = th.PropertiesList(
         th.Property(
             "ID",
             th.StringType,
             description="The unique identifier of the account"
@@ -273,36 +243,21 @@
             filter_path = f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&"
                 
         path = f"/financial/GLAccounts?{filter_path if 'filter_path' in locals() else ''}" \
             "$select=ID,Code,Description,Costcenter,CostcenterDescription,Costunit,CostunitDescription,Modified"
 
         return path
 
-    def get_records(self, context: Optional[dict]) -> Iterable[dict]:
-        """Return a generator or row-type dictionary objects"""
-        
-        resp = self.conn.rest(GET('v1/%d/%s' % (self.division, self.get_path(context) )))
-        
-        # The fields that have /Date(unixmilliseconds)/ objects that should be converted into datetime objects
-        keys = ['Modified']
-
-        for row in resp:
-            
-            # We loop through the keys that should be modified
-            for key in keys:
-                row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
-
-            yield row
-
 class BankEntryLinesStream(ExactOnlineStream):
     """Define custom stream."""
 
     name = "bank_entry_lines"
     primary_keys = ["ID"]
     replication_key = "Modified"
+    date_fields = ['Date', 'Modified']
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     # schema_filepath = SCHEMAS_DIR / "users.json"
     schema = th.PropertiesList(
         th.Property(
             "ID",
             th.StringType,
             description="The unique identifier of the line"
@@ -366,36 +321,21 @@
         
         path = "/financialtransaction/BankEntryLines?" \
             f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&" \
             "$select=ID,AccountCode,AccountName,GLAccount,GLAccountCode,Date,Description,OurRef,LineNumber,AmountDC,Modified"
 
         return path
 
-    def get_records(self, context: Optional[dict]) -> Iterable[dict]:
-        """Return a generator or row-type dictionary objects"""
-        
-        resp = self.conn.rest(GET('v1/%d/%s' % (self.division, self.get_path(context) )))
-        
-        # The fields that have /Date(unixmilliseconds)/ objects that should be converted into datetime objects
-        keys = ['Date', 'Modified']
-
-        for row in resp:
-            
-            # We loop through the keys that should be modified
-            for key in keys:
-                row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
-
-            yield row
-
 class CashEntryLinesStream(ExactOnlineStream):
     """Define custom stream."""
 
     name = "cash_entry_lines"
     primary_keys = ["ID"]
     replication_key = "Modified"
+    date_fields = ['Date', 'Modified']
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     # schema_filepath = SCHEMAS_DIR / "users.json"
     schema = th.PropertiesList(
         th.Property(
             "ID",
             th.StringType,
             description="The unique identifier of the line"
@@ -459,36 +399,21 @@
         
         path = "/financialtransaction/CashEntryLines?" \
             f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&" \
             "$select=ID,AccountCode,AccountName,GLAccount,GLAccountCode,Date,Description,OurRef,LineNumber,AmountDC,Modified"
 
         return path
 
-    def get_records(self, context: Optional[dict]) -> Iterable[dict]:
-        """Return a generator or row-type dictionary objects"""
-        
-        resp = self.conn.rest(GET('v1/%d/%s' % (self.division, self.get_path(context) )))
-        
-        # The fields that have /Date(unixmilliseconds)/ objects that should be converted into datetime objects
-        keys = ['Date', 'Modified']
-
-        for row in resp:
-            
-            # We loop through the keys that should be modified
-            for key in keys:
-                row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
-
-            yield row
-
 class GeneralJournalEntryLinesStream(ExactOnlineStream):
     """Define custom stream."""
 
     name = "general_journal_entry_lines"
     primary_keys = ["ID"]
     replication_key = "Modified"
+    date_fields = ['Date', 'Modified']
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     # schema_filepath = SCHEMAS_DIR / "users.json"
     schema = th.PropertiesList(
         th.Property(
             "ID",
             th.StringType,
             description="The unique identifier of the line"
@@ -557,36 +482,21 @@
         
         path = "/generaljournalentry/GeneralJournalEntryLines?" \
             f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&" \
             "$select=ID,AccountCode,AccountName,GLAccount,GLAccountCode,Date,Description,OurRef,LineNumber,AmountDC,AmountVATDC,Modified"
 
         return path
 
-    def get_records(self, context: Optional[dict]) -> Iterable[dict]:
-        """Return a generator or row-type dictionary objects"""
-        
-        resp = self.conn.rest(GET('v1/%d/%s' % (self.division, self.get_path(context) )))
-        
-        # The fields that have /Date(unixmilliseconds)/ objects that should be converted into datetime objects
-        keys = ['Date', 'Modified']
-
-        for row in resp:
-            
-            # We loop through the keys that should be modified
-            for key in keys:
-                row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
-
-            yield row
-
 class PurchaseEntriesStream(ExactOnlineStream):
     """Define custom stream."""
 
     name = "purchase_entries"
     primary_keys = ["EntryID"]
     replication_key = "Modified"
+    date_fields = ['Created', 'EntryDate', 'DueDate', 'Modified']
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     # schema_filepath = SCHEMAS_DIR / "users.json"
     schema = th.PropertiesList(
         th.Property(
             "EntryID",
             th.StringType,
             description="The unique identifier of the line"
@@ -675,36 +585,21 @@
         
         path = "/purchaseentry/PurchaseEntries?" \
             f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&" \
             "$select=EntryID,Created,EntryDate,InvoiceNumber,EntryNumber,Description,OrderNumber,DueDate,PaymentCondition,Status,Journal,Supplier,SupplierName,AmountDC,VATAmountDC,Modified"
 
         return path
 
-    def get_records(self, context: Optional[dict]) -> Iterable[dict]:
-        """Return a generator or row-type dictionary objects"""
-        
-        resp = self.conn.rest(GET('v1/%d/%s' % (self.division, self.get_path(context) )))
-        
-        # The fields that have /Date(unixmilliseconds)/ objects that should be converted into datetime objects
-        keys = ['Created', 'EntryDate', 'DueDate', 'Modified']
-
-        for row in resp:
-            
-            # We loop through the keys that should be modified
-            for key in keys:
-                row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
-
-            yield row
-
 class SalesEntriesStream(ExactOnlineStream):
     """Define custom stream."""
 
     name = "sales_entries"
     primary_keys = ["EntryID"]
     replication_key = "Modified"
+    date_fields = ['Created', 'EntryDate', 'DueDate', 'Modified']
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     # schema_filepath = SCHEMAS_DIR / "users.json"
     schema = th.PropertiesList(
         th.Property(
             "EntryID",
             th.StringType,
             description="The unique identifier of the line"
@@ -793,36 +688,21 @@
         
         path = "/salesentry/SalesEntries?" \
             f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&" \
             "$select=EntryID,Created,EntryDate,YourRef,EntryNumber,Description,OrderNumber,DueDate,PaymentCondition,Status,Journal,Customer,CustomerName,AmountDC,VATAmountDC,Modified"
 
         return path
 
-    def get_records(self, context: Optional[dict]) -> Iterable[dict]:
-        """Return a generator or row-type dictionary objects"""
-        
-        resp = self.conn.rest(GET('v1/%d/%s' % (self.division, self.get_path(context) )))
-        
-        # The fields that have /Date(unixmilliseconds)/ objects that should be converted into datetime objects
-        keys = ['Created', 'EntryDate', 'DueDate', 'Modified']
-
-        for row in resp:
-            
-            # We loop through the keys that should be modified
-            for key in keys:
-                row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
-
-            yield row
-
 class CrmAccountsStream(ExactOnlineStream):
     """Define custom stream."""
 
     name = "crm_accounts"
     primary_keys = ["ID"]
     replication_key = "Modified"
+    date_fields = ['Modified']
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     # schema_filepath = SCHEMAS_DIR / "users.json"
     schema = th.PropertiesList(
         th.Property(
             "ID",
             th.StringType,
             description="The unique identifier of the account"
@@ -889,36 +769,21 @@
             filter_path = f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&"
         
         path = f"/crm/Accounts?{filter_path if 'filter_path' in locals() else ''}" \
             "$select=ID,AccountManager,AccountManagerFullName,Code,City,CountryName,Latitude,Longitude,Name,SearchCode,Modified"
 
         return path
 
-    def get_records(self, context: Optional[dict]) -> Iterable[dict]:
-        """Return a generator or row-type dictionary objects"""
-        
-        resp = self.conn.rest(GET('v1/%d/%s' % (self.division, self.get_path(context) )))
-        
-        # The fields that have /Date(unixmilliseconds)/ objects that should be converted into datetime objects
-        keys = ['Modified']
-
-        for row in resp:
-            
-            # We loop through the keys that should be modified
-            for key in keys:
-                row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
-
-            yield row
-
 # class SystemUsersStream(ExactOnlineStream):
 #     """Define custom stream."""
 
 #     name = "system_users"
 #     primary_keys = ["UserID"]
 #     replication_key = "Modified"
+#     date_fields = ['StartDate', 'EndDate', 'Modified']
 #     # Optionally, you may also use `schema_filepath` in place of `schema`:
 #     # schema_filepath = SCHEMAS_DIR / "users.json"
 #     schema = th.PropertiesList(
 #         th.Property(
 #             "UserID",
 #             th.StringType,
 #             description="The unique identifier of the user"
@@ -958,24 +823,8 @@
 #             replication_key_value = self.get_starting_timestamp(context).strftime('%Y-%m-%dT%H:%M:%S.%fZ')
             
 #             filter_path = f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&"
         
 #         path = f"/system/Users?{filter_path if 'filter_path' in locals() else ''}" \
 #             "$select=UserID,FullName,Email,StartDate,EndDate,Modified"
 
-#         return path
-
-#     def get_records(self, context: Optional[dict]) -> Iterable[dict]:
-#         """Return a generator or row-type dictionary objects"""
-        
-#         resp = self.conn.rest(GET('v1/%s' % (self.get_path(context) )))
-        
-#         # The fields that have /Date(unixmilliseconds)/ objects that should be converted into datetime objects
-#         keys = ['StartDate', 'EndDate', 'Modified']
-
-#         for row in resp:
-            
-#             # We loop through the keys that should be modified
-#             for key in keys:
-#                 row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
-
-#             yield row
+#         return path
```

### Comparing `tap_exact-0.3.3/tap_exact/tap.py` & `tap_exact-0.4.0/tap_exact/tap.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.3.3/tap_exact/tests/test_core.py` & `tap_exact-0.4.0/tap_exact/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.3.3/setup.py` & `tap_exact-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 {'s3': ['fs-s3fs>=1.1.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['tap-exact = tap_exact.tap:TapExactOnline.cli']}
 
 setup_kwargs = {
     'name': 'tap-exact',
-    'version': '0.3.3',
+    'version': '0.4.0',
     'description': '`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.',
     'long_description': 'None',
     'author': 'Janick Otten',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tap_exact-0.3.3/PKG-INFO` & `tap_exact-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-exact
-Version: 0.3.3
+Version: 0.4.0
 Summary: `tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,Exact Online
 Author: Janick Otten
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

