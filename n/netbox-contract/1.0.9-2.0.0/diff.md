# Comparing `tmp/netbox_contract-1.0.9.tar.gz` & `tmp/netbox-contract-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_contract-1.0.9.tar", last modified: Tue Feb 21 21:41:17 2023, max compression
+gzip compressed data, was "netbox-contract-2.0.0.tar", last modified: Thu May 25 20:33:15 2023, max compression
```

## Comparing `netbox_contract-1.0.9.tar` & `netbox-contract-2.0.0.tar`

### file list

```diff
@@ -1,54 +1,57 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-02-21 21:41:17.771381 netbox_contract-1.0.9/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1056 2023-01-03 17:10:18.000000 netbox_contract-1.0.9/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-01-08 15:22:13.000000 netbox_contract-1.0.9/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2299 2023-02-21 21:41:17.771381 netbox_contract-1.0.9/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1759 2023-02-21 21:33:50.000000 netbox_contract-1.0.9/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)      774 2023-02-21 21:39:43.000000 netbox_contract-1.0.9/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-02-21 21:41:17.771381 netbox_contract-1.0.9/setup.cfg
--rw-rw-r--   0 vscode    (1000) vscode    (1000)       52 2023-01-03 18:27:10.000000 netbox_contract-1.0.9/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-02-21 21:41:17.747381 netbox_contract-1.0.9/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-02-21 21:41:17.751381 netbox_contract-1.0.9/src/netbox_contract/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      468 2023-02-21 21:39:25.000000 netbox_contract-1.0.9/src/netbox_contract/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-02-21 21:41:17.755381 netbox_contract-1.0.9/src/netbox_contract/api/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)        0 2023-01-03 17:10:18.000000 netbox_contract-1.0.9/src/netbox_contract/api/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2457 2023-01-24 19:02:09.000000 netbox_contract-1.0.9/src/netbox_contract/api/serializers.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      314 2023-01-03 21:38:07.000000 netbox_contract-1.0.9/src/netbox_contract/api/urls.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      730 2023-01-22 19:07:28.000000 netbox_contract-1.0.9/src/netbox_contract/api/views.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1089 2023-02-19 15:04:41.000000 netbox_contract-1.0.9/src/netbox_contract/filtersets.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5026 2023-01-30 21:38:17.000000 netbox_contract-1.0.9/src/netbox_contract/forms.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-02-21 21:41:17.763382 netbox_contract-1.0.9/src/netbox_contract/migrations/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4598 2023-01-03 21:49:17.000000 netbox_contract-1.0.9/src/netbox_contract/migrations/0001_initial.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      764 2023-01-03 23:22:17.000000 netbox_contract-1.0.9/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1579 2023-01-15 09:38:37.000000 netbox_contract-1.0.9/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      601 2023-01-15 10:03:41.000000 netbox_contract-1.0.9/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      584 2023-01-15 10:48:38.000000 netbox_contract-1.0.9/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      563 2023-01-22 10:09:31.000000 netbox_contract-1.0.9/src/netbox_contract/migrations/0006_alter_contract_circuit.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      403 2023-01-22 10:53:55.000000 netbox_contract-1.0.9/src/netbox_contract/migrations/0007_invoice_date.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      386 2023-01-22 18:33:12.000000 netbox_contract-1.0.9/src/netbox_contract/migrations/0008_invoice_comments.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      428 2023-01-22 18:51:18.000000 netbox_contract-1.0.9/src/netbox_contract/migrations/0009_contract_external_reference.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      494 2023-01-24 18:34:51.000000 netbox_contract-1.0.9/src/netbox_contract/migrations/0010_invoice_contracts.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-01-24 18:34:51.000000 netbox_contract-1.0.9/src/netbox_contract/migrations/0011_auto_20230122_2112.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      339 2023-01-24 18:34:51.000000 netbox_contract-1.0.9/src/netbox_contract/migrations/0012_remove_invoice_contract.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      549 2023-01-30 21:27:12.000000 netbox_contract-1.0.9/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      422 2023-01-30 21:38:17.000000 netbox_contract-1.0.9/src/netbox_contract/migrations/0014_contract_end_date.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)        0 2023-01-03 17:10:18.000000 netbox_contract-1.0.9/src/netbox_contract/migrations/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4856 2023-02-10 21:39:07.000000 netbox_contract-1.0.9/src/netbox_contract/models.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1644 2023-02-21 21:38:33.000000 netbox_contract-1.0.9/src/netbox_contract/navigation.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-02-19 15:04:41.000000 netbox_contract-1.0.9/src/netbox_contract/search.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2079 2023-01-30 21:27:12.000000 netbox_contract-1.0.9/src/netbox_contract/tables.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      539 2023-01-03 23:12:00.000000 netbox_contract-1.0.9/src/netbox_contract/template_content.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-02-21 21:41:17.763382 netbox_contract-1.0.9/src/netbox_contract/templates/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      305 2023-01-03 17:10:18.000000 netbox_contract-1.0.9/src/netbox_contract/templates/contract_list_bottom.html
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-02-21 21:41:17.767382 netbox_contract-1.0.9/src/netbox_contract/templates/netbox_contract/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3750 2023-01-30 21:38:17.000000 netbox_contract-1.0.9/src/netbox_contract/templates/netbox_contract/contract.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2334 2023-01-30 21:27:12.000000 netbox_contract-1.0.9/src/netbox_contract/templates/netbox_contract/invoice.html
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1128 2023-01-03 17:10:18.000000 netbox_contract-1.0.9/src/netbox_contract/templates/netbox_contract/serviceprovider.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2986 2023-01-22 09:11:05.000000 netbox_contract-1.0.9/src/netbox_contract/urls.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6805 2023-01-24 18:34:51.000000 netbox_contract-1.0.9/src/netbox_contract/views.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-02-21 21:41:17.755381 netbox_contract-1.0.9/src/netbox_contract.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2299 2023-02-21 21:41:17.000000 netbox_contract-1.0.9/src/netbox_contract.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1950 2023-02-21 21:41:17.000000 netbox_contract-1.0.9/src/netbox_contract.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-02-21 21:41:17.000000 netbox_contract-1.0.9/src/netbox_contract.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-02-19 10:47:00.000000 netbox_contract-1.0.9/src/netbox_contract.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-02-21 21:41:17.000000 netbox_contract-1.0.9/src/netbox_contract.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-02-21 21:41:17.000000 netbox_contract-1.0.9/src/netbox_contract.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-25 20:33:15.427488 netbox-contract-2.0.0/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1056 2023-01-03 17:10:18.000000 netbox-contract-2.0.0/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-03-12 14:44:04.000000 netbox-contract-2.0.0/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2299 2023-05-25 20:33:15.427488 netbox-contract-2.0.0/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1759 2023-03-12 15:14:54.000000 netbox-contract-2.0.0/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      774 2023-05-25 20:27:44.000000 netbox-contract-2.0.0/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-25 20:33:15.427488 netbox-contract-2.0.0/setup.cfg
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       52 2023-01-03 18:27:10.000000 netbox-contract-2.0.0/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-25 20:33:15.391487 netbox-contract-2.0.0/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-25 20:33:15.399487 netbox-contract-2.0.0/src/netbox_contract/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      469 2023-05-25 20:31:35.000000 netbox-contract-2.0.0/src/netbox_contract/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-25 20:33:15.407487 netbox-contract-2.0.0/src/netbox_contract/api/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/api/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4016 2023-05-25 20:01:58.000000 netbox-contract-2.0.0/src/netbox_contract/api/serializers.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      387 2023-05-23 17:57:34.000000 netbox-contract-2.0.0/src/netbox_contract/api/urls.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      955 2023-05-22 22:26:02.000000 netbox-contract-2.0.0/src/netbox_contract/api/views.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1369 2023-05-10 21:06:50.000000 netbox-contract-2.0.0/src/netbox_contract/filtersets.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5629 2023-05-16 21:07:49.000000 netbox-contract-2.0.0/src/netbox_contract/forms.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-25 20:33:15.419488 netbox-contract-2.0.0/src/netbox_contract/migrations/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4598 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0001_initial.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      764 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1579 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      601 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      584 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      563 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0006_alter_contract_circuit.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      403 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0007_invoice_date.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      386 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0008_invoice_comments.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      428 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0009_contract_external_reference.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      494 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0010_invoice_contracts.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0011_auto_20230122_2112.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      339 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0012_remove_invoice_contract.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      549 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      422 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0014_contract_end_date.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2104 2023-05-13 17:53:07.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/0015_contractassignement.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/migrations/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5517 2023-05-24 18:15:36.000000 netbox-contract-2.0.0/src/netbox_contract/models.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1644 2023-03-12 18:00:52.000000 netbox-contract-2.0.0/src/netbox_contract/navigation.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/search.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2700 2023-05-24 18:08:42.000000 netbox-contract-2.0.0/src/netbox_contract/tables.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1325 2023-05-23 21:14:03.000000 netbox-contract-2.0.0/src/netbox_contract/template_content.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-25 20:33:15.419488 netbox-contract-2.0.0/src/netbox_contract/templates/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      775 2023-05-23 19:02:53.000000 netbox-contract-2.0.0/src/netbox_contract/templates/contract_assignements_bottom.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      305 2023-05-24 18:09:51.000000 netbox-contract-2.0.0/src/netbox_contract/templates/contract_list_bottom.html
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-25 20:33:15.423488 netbox-contract-2.0.0/src/netbox_contract/templates/netbox_contract/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4257 2023-05-23 21:01:17.000000 netbox-contract-2.0.0/src/netbox_contract/templates/netbox_contract/contract.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      810 2023-05-22 21:27:25.000000 netbox-contract-2.0.0/src/netbox_contract/templates/netbox_contract/contract_assignement.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2284 2023-03-12 17:52:54.000000 netbox-contract-2.0.0/src/netbox_contract/templates/netbox_contract/invoice.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1128 2023-03-12 14:46:55.000000 netbox-contract-2.0.0/src/netbox_contract/templates/netbox_contract/serviceprovider.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3751 2023-05-23 19:01:13.000000 netbox-contract-2.0.0/src/netbox_contract/urls.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8384 2023-05-23 18:08:26.000000 netbox-contract-2.0.0/src/netbox_contract/views.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-25 20:33:15.403487 netbox-contract-2.0.0/src/netbox_contract.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2299 2023-05-25 20:33:15.000000 netbox-contract-2.0.0/src/netbox_contract.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2145 2023-05-25 20:33:15.000000 netbox-contract-2.0.0/src/netbox_contract.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-25 20:33:15.000000 netbox-contract-2.0.0/src/netbox_contract.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-02-19 10:47:00.000000 netbox-contract-2.0.0/src/netbox_contract.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-05-25 20:33:15.000000 netbox-contract-2.0.0/src/netbox_contract.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-05-25 20:33:15.000000 netbox-contract-2.0.0/src/netbox_contract.egg-info/top_level.txt
```

### Comparing `netbox_contract-1.0.9/LICENSE` & `netbox-contract-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_contract-1.0.9/PKG-INFO` & `netbox-contract-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: netbox_contract
-Version: 1.0.9
+Name: netbox-contract
+Version: 2.0.0
 Summary: Contract management plugin for Netbox
 Author-email: Marc Lebreuil <marc@famillelebreuil.net>
 Project-URL: Homepage, https://github.com/mlebreuil/netbox-contract
 Project-URL: Bug Tracker, https://github.com/mlebreuil/netbox-contract/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,15 +26,15 @@
 ```bash
 $ source /opt/netbox/venv/bin/activate
 ```
 
 ### Install the package 
 
 ```bash
-$ python3 -m pip install netbox_contract
+$ python3 -m pip install netbox-contract
 ```
 
 ### Configure NetBox
 
 Finally, we need to configure NetBox to enable our new plugin. Over in the NetBox installation path, open `netbox/netbox/configuration.py` and look for the `PLUGINS` parameter; this should be an empty list. (If it's not yet defined, go ahead and create it.) Add the name of our plugin to this list:
 
 ```python
```

### Comparing `netbox_contract-1.0.9/README.md` & `netbox-contract-2.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ```bash
 $ source /opt/netbox/venv/bin/activate
 ```
 
 ### Install the package 
 
 ```bash
-$ python3 -m pip install netbox_contract
+$ python3 -m pip install netbox-contract
 ```
 
 ### Configure NetBox
 
 Finally, we need to configure NetBox to enable our new plugin. Over in the NetBox installation path, open `netbox/netbox/configuration.py` and look for the `PLUGINS` parameter; this should be an empty list. (If it's not yet defined, go ahead and create it.) Add the name of our plugin to this list:
 
 ```python
```

### Comparing `netbox_contract-1.0.9/pyproject.toml` & `netbox-contract-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
-name = "netbox_contract"
-version = "1.0.9"
+name = "netbox-contract"
+version = "2.0.0"
 authors = [
   { name="Marc Lebreuil", email="marc@famillelebreuil.net" },
 ]
 description = "Contract management plugin for Netbox"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `netbox_contract-1.0.9/src/netbox_contract/api/views.py` & `netbox-contract-2.0.0/src/netbox_contract/api/views.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from netbox.api.viewsets import NetBoxModelViewSet
 
 from .. import filtersets, models
-from .serializers import ContractSerializer, InvoiceSerializer, ServiceProviderSerializer
+from .serializers import ContractSerializer, InvoiceSerializer, ServiceProviderSerializer, ContractAssignementSerializer
 
 class ContractViewSet(NetBoxModelViewSet):
     queryset = models.Contract.objects.prefetch_related('circuit','tags')
     serializer_class = ContractSerializer
 
 class InvoiceViewSet(NetBoxModelViewSet):
     queryset = models.Invoice.objects.prefetch_related(
@@ -13,7 +13,11 @@
     )
     serializer_class = InvoiceSerializer
     filterset_class = filtersets.InvoiceFilterSet
 
 class ServiceProviderViewSet(NetBoxModelViewSet):
     queryset = models.ServiceProvider.objects.prefetch_related('tags')
     serializer_class = ServiceProviderSerializer
+
+class ContractAssignementViewSet(NetBoxModelViewSet):
+    queryset = models.ContractAssignement.objects.prefetch_related('contract','tags')
+    serializer_class = ContractAssignementSerializer
```

### Comparing `netbox_contract-1.0.9/src/netbox_contract/filtersets.py` & `netbox-contract-2.0.0/src/netbox_contract/filtersets.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from django.db.models import Q
 from netbox.filtersets import NetBoxModelFilterSet
-from .models import Contract,Invoice,ServiceProvider
+from .models import Contract,Invoice,ServiceProvider,ContractAssignement
 
 class ContractFilterSet(NetBoxModelFilterSet):
 
     class Meta:
         model = Contract
         fields = ('id', 'external_partie', 'internal_partie', 'status','circuit')
 
@@ -28,7 +28,16 @@
 
     class Meta:
         model = ServiceProvider
         fields = ('id','name')
 
     def search(self, queryset, name, value):
         return queryset.filter(name__icontains=value)
+
+class ContractAssignementFilterSet(NetBoxModelFilterSet):
+
+    class Meta:
+        model = ContractAssignement
+        fields = ('id','contract')
+
+    def search(self, queryset, name, value):
+        return queryset.filter(Q(contract__name__icontains=value))
```

### Comparing `netbox_contract-1.0.9/src/netbox_contract/forms.py` & `netbox-contract-2.0.0/src/netbox_contract/forms.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django import forms
 import django_filters
 from netbox.forms import NetBoxModelForm, NetBoxModelFilterSetForm, NetBoxModelBulkEditForm, NetBoxModelCSVForm
 from utilities.forms.fields import CommentField, DynamicModelChoiceField, DynamicModelMultipleChoiceField, MultipleChoiceField
 from utilities.forms import CSVModelChoiceField, DatePicker,SlugField
 from extras.filters import TagFilter
 from circuits.models import Circuit
-from .models import Contract, Invoice, ServiceProvider, StatusChoices
+from .models import Contract, Invoice, ServiceProvider, StatusChoices, ContractAssignement
 
 class ContractForm(NetBoxModelForm):
     comments = CommentField()
     circuit=DynamicModelMultipleChoiceField(
         queryset=Circuit.objects.all(),
         required=False
     )
@@ -170,7 +170,27 @@
         required=True
     )
     comments = CommentField()
     nullable_fields = (
         'comments',
     )
     model = ServiceProvider
+
+# ContractAssignement
+
+class ContractAssignementForm(NetBoxModelForm):
+    contract=DynamicModelChoiceField(
+        queryset=Contract.objects.all()
+    )
+    class Meta:
+        model = ContractAssignement
+        fields = ['content_type', 'object_id', 'contract','tags']
+        widgets = {
+            'content_type': forms.HiddenInput(),
+            'object_id': forms.HiddenInput(),
+        }
+
+class ContractAssignementFilterSetForm(NetBoxModelFilterSetForm):
+    model = ContractAssignement
+    contract=DynamicModelChoiceField(
+        queryset=Contract.objects.all()
+    )
```

### Comparing `netbox_contract-1.0.9/src/netbox_contract/migrations/0001_initial.py` & `netbox-contract-2.0.0/src/netbox_contract/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_contract-1.0.9/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py` & `netbox-contract-2.0.0/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_contract-1.0.9/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py` & `netbox-contract-2.0.0/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_contract-1.0.9/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py` & `netbox-contract-2.0.0/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py`

 * *Files identical despite different names*

### Comparing `netbox_contract-1.0.9/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py` & `netbox-contract-2.0.0/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_contract-1.0.9/src/netbox_contract/migrations/0006_alter_contract_circuit.py` & `netbox-contract-2.0.0/src/netbox_contract/migrations/0006_alter_contract_circuit.py`

 * *Files identical despite different names*

### Comparing `netbox_contract-1.0.9/src/netbox_contract/migrations/0011_auto_20230122_2112.py` & `netbox-contract-2.0.0/src/netbox_contract/migrations/0011_auto_20230122_2112.py`

 * *Files identical despite different names*

### Comparing `netbox_contract-1.0.9/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py` & `netbox-contract-2.0.0/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py`

 * *Files identical despite different names*

### Comparing `netbox_contract-1.0.9/src/netbox_contract/models.py` & `netbox-contract-2.0.0/src/netbox_contract/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,14 +61,37 @@
 
     def __str__(self):
         return self.name
 
     def get_absolute_url(self):
         return reverse('plugins:netbox_contract:serviceprovider', args=[self.pk])
 
+class ContractAssignement(NetBoxModel):
+    content_type = models.ForeignKey(
+        to=ContentType,
+        on_delete=models.CASCADE
+    )
+    object_id = models.PositiveBigIntegerField()
+    content_object = GenericForeignKey(
+        ct_field='content_type',
+        fk_field='object_id'
+    )
+    contract = models.ForeignKey(
+        to='Contract',
+        on_delete=models.PROTECT,
+        related_name='assignments'
+    )
+    clone_fields = ('content_type', 'object_id','contract')
+
+    class Meta:
+        ordering = ('contract',)
+
+    def get_absolute_url(self):
+        return reverse('plugins:netbox_contract:contractassignement', args=[self.pk])
+
 class Contract(NetBoxModel):
     name = models.CharField(
         max_length=100
     )
     external_partie = models.ForeignKey(
         to=ServiceProvider,
         on_delete=models.CASCADE,
@@ -155,14 +178,15 @@
 
     class Meta:
         ordering = ('name',)
 
     def __str__(self):
         return self.name
 
+
 class Invoice(NetBoxModel):
     number = models.CharField(
         max_length=100
     )
     date = models.DateField(
         blank=True,
         null=True
```

### Comparing `netbox_contract-1.0.9/src/netbox_contract/navigation.py` & `netbox-contract-2.0.0/src/netbox_contract/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_contract-1.0.9/src/netbox_contract/search.py` & `netbox-contract-2.0.0/src/netbox_contract/search.py`

 * *Files identical despite different names*

### Comparing `netbox_contract-1.0.9/src/netbox_contract/tables.py` & `netbox-contract-2.0.0/src/netbox_contract/tables.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,32 @@
 import django_tables2 as tables
 
-from netbox.tables import NetBoxTable
+from netbox.tables import NetBoxTable, columns
 from circuits.models import Circuit
-from .models import Contract, Invoice, ServiceProvider
+from .models import ContractAssignement, Contract, Invoice, ServiceProvider
+
+class ContractAssignementListTable(NetBoxTable):
+    content_type = columns.ContentTypeColumn(
+        verbose_name='Object Type'
+    )
+    content_object = tables.Column(
+        linkify=True,
+        orderable=False
+    )
+    contract = tables.Column(
+        linkify=True
+    )
+    actions = columns.ActionsColumn(
+        actions=('edit', 'delete')
+    )
+
+    class Meta(NetBoxTable.Meta):
+        model = ContractAssignement
+        fields = ('pk', 'content_type', 'content_object', 'contract', 'actions')
+        default_columns = ('pk', 'content_type', 'content_object', 'contract')
 
 class ContractListTable(NetBoxTable):
 
     name = tables.Column(
         linkify=True
     )
     external_partie = tables.Column(
```

### Comparing `netbox_contract-1.0.9/src/netbox_contract/template_content.py` & `netbox-contract-2.0.0/src/netbox_contract/template_content.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,33 @@
+from django.contrib.contenttypes.models import ContentType
 from extras.plugins import PluginTemplateExtension
-from .models import Contract
+from circuits.models import Circuit
+from .models import ContractAssignement
 from . import tables
 
 class CircuitContracts(PluginTemplateExtension):
     model = 'circuits.circuit'
 
     def full_width_page(self):
         circuit = self.context['object']
         table = tables.ContractListBottomTable(circuit.contracts.all())
         table.configure(self.context['request'])
 
         return self.render('contract_list_bottom.html', extra_context={
             'contracts_table': table,
         })
 
-template_extensions = [CircuitContracts]
+class CircuitContractAssignements(PluginTemplateExtension):
+    model = 'circuits.circuit'
+
+    def full_width_page(self):
+        circuit = self.context['object']
+        circuit_type = ContentType.objects.get_for_model(Circuit)
+        contract_assignements = ContractAssignement.objects.filter(content_type__pk=circuit_type.id, object_id=circuit.id)
+        assignements_table = tables.ContractAssignementListTable(contract_assignements)
+        assignements_table.configure(self.context['request'])
+
+        return self.render('contract_assignements_bottom.html', extra_context={
+            'assignements_table': assignements_table,
+        })
+
+template_extensions = [ CircuitContracts, CircuitContractAssignements]
```

### Comparing `netbox_contract-1.0.9/src/netbox_contract/templates/netbox_contract/contract.html` & `netbox-contract-2.0.0/src/netbox_contract/templates/netbox_contract/contract.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 {% extends 'generic/object.html' %}
 {% load render_table from django_tables2 %}
+{% block breadcrumbs %}
+  {{ block.super }}
+  <li class="breadcrumb-item"><a href="{% url 'plugins:netbox_contract:contract_list' %}?external_partie={{ object.external_partie.pk }}">{{ object.external_partie }}</a></li>
+{% endblock %}
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Contract</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
@@ -96,14 +100,24 @@
         </div>
       </div>
     </div>
   </div>
   <div class="row">
     <div class="col col-md-12">
       <div class="card">
+        <h5 class="card-header">Assignements</h5>
+        <div class="card-body table-responsive">
+          {% render_table assignements_table %}
+        </div>
+      </div>
+    </div>
+  </div>
+  <div class="row">
+    <div class="col col-md-12">
+      <div class="card">
         <h5 class="card-header">Invoices</h5>
         <div class="card-body table-responsive">
           {% render_table invoices_table %}
         </div>
         <div class="card-footer text-end noprint">
           <a href="{% url 'plugins:netbox_contract:invoice_add' %}?contracts={{ object.pk }}" class="btn btn-primary btn-sm">
               <i class="mdi mdi-plus-thick" aria-hidden="true"></i>
```

#### html2text {}

```diff
@@ -1,9 +1,11 @@
 {% extends 'generic/object.html' %} {% load render_table from django_tables2 %}
-{% block content %}
+{% block breadcrumbs %} {{ block.super }}
+{{_object.external_partie_}}
+{% endblock %} {% block content %}
 ** Contract **
 Name                   {{ object.name }}
 External partie        {{_object.external_partie.name_}}
 Status                 {{ object.status }}
 External reference     {{ object.external_reference }}
 Internal partie        {{ object.internal_partie }}
 Tenant                 {{ object.tenant }}
@@ -17,11 +19,13 @@
 Non recuring costs     {{ object.nrc }}
 Invoice frequency      {{ object.invoice_frequency }}
 Documents              Documents
 {% include 'inc/panels/custom_fields.html' %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
 ** Circuits **
 {% render_table circuit_table %}
+** Assignements **
+{% render_table assignements_table %}
 ** Invoices **
 {% render_table invoices_table %}
  Add_an_invoice
 {% endblock content %}
```

### Comparing `netbox_contract-1.0.9/src/netbox_contract/templates/netbox_contract/serviceprovider.html` & `netbox-contract-2.0.0/src/netbox_contract/templates/netbox_contract/serviceprovider.html`

 * *Files identical despite different names*

### Comparing `netbox_contract-1.0.9/src/netbox_contract/urls.py` & `netbox-contract-2.0.0/src/netbox_contract/urls.py`

 * *Files 21% similar despite different names*

```diff
@@ -38,9 +38,18 @@
     path('invoices/<int:pk>/', views.InvoiceView.as_view(), name='invoice'),
     path('invoices/<int:pk>/edit/', views.InvoiceEditView.as_view(), name='invoice_edit'),
     path('invoices/<int:pk>/delete/', views.InvoiceDeleteView.as_view(), name='invoice_delete'),
     path('invoices/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='invoice_changelog', kwargs={
         'model': models.Invoice
     }),
 
+    # Contract assignements
+    path('assignements/', views.ContractAssignementListView.as_view(), name='contractassignement_list'),
+    path('assignements/add/', views.ContractAssignementEditView.as_view(), name='contractassignement_add'),
+    path('assignements/<int:pk>/', views.ContractAssignementView.as_view(), name='contractassignement'),
+    path('assignements/<int:pk>/edit/', views.ContractAssignementEditView.as_view(), name='contractassignement_edit'),
+    path('assignements/<int:pk>/delete/', views.ContractAssignementDeleteView.as_view(), name='contractassignement_delete'),
+    path('assignements/<int:pk>/changelog/', ObjectChangeLogView.as_view(), name='contractassignement_changelog', kwargs={
+        'model': models.ContractAssignement
+    }),
 
 )
```

### Comparing `netbox_contract-1.0.9/src/netbox_contract.egg-info/PKG-INFO` & `netbox-contract-2.0.0/src/netbox_contract.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-contract
-Version: 1.0.9
+Version: 2.0.0
 Summary: Contract management plugin for Netbox
 Author-email: Marc Lebreuil <marc@famillelebreuil.net>
 Project-URL: Homepage, https://github.com/mlebreuil/netbox-contract
 Project-URL: Bug Tracker, https://github.com/mlebreuil/netbox-contract/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,15 +26,15 @@
 ```bash
 $ source /opt/netbox/venv/bin/activate
 ```
 
 ### Install the package 
 
 ```bash
-$ python3 -m pip install netbox_contract
+$ python3 -m pip install netbox-contract
 ```
 
 ### Configure NetBox
 
 Finally, we need to configure NetBox to enable our new plugin. Over in the NetBox installation path, open `netbox/netbox/configuration.py` and look for the `PLUGINS` parameter; this should be an empty list. (If it's not yet defined, go ahead and create it.) Add the name of our plugin to this list:
 
 ```python
```

### Comparing `netbox_contract-1.0.9/src/netbox_contract.egg-info/SOURCES.txt` & `netbox-contract-2.0.0/src/netbox_contract.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -33,12 +33,15 @@
 src/netbox_contract/migrations/0008_invoice_comments.py
 src/netbox_contract/migrations/0009_contract_external_reference.py
 src/netbox_contract/migrations/0010_invoice_contracts.py
 src/netbox_contract/migrations/0011_auto_20230122_2112.py
 src/netbox_contract/migrations/0012_remove_invoice_contract.py
 src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py
 src/netbox_contract/migrations/0014_contract_end_date.py
+src/netbox_contract/migrations/0015_contractassignement.py
 src/netbox_contract/migrations/__init__.py
+src/netbox_contract/templates/contract_assignements_bottom.html
 src/netbox_contract/templates/contract_list_bottom.html
 src/netbox_contract/templates/netbox_contract/contract.html
+src/netbox_contract/templates/netbox_contract/contract_assignement.html
 src/netbox_contract/templates/netbox_contract/invoice.html
 src/netbox_contract/templates/netbox_contract/serviceprovider.html
```

