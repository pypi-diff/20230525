# Comparing `tmp/app_transport_framework_library-0.1.5.tar.gz` & `tmp/app_transport_framework_library-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "app_transport_framework_library-0.1.5.tar", max compression
+gzip compressed data, was "app_transport_framework_library-0.1.6.tar", max compression
```

## Comparing `app_transport_framework_library-0.1.5.tar` & `app_transport_framework_library-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2023-05-22 22:04:58.127954 app_transport_framework_library-0.1.5/app_transport_framework_library/__init__.py
--rw-r--r--   0        0        0     6427 2023-05-23 19:52:56.836795 app_transport_framework_library-0.1.5/app_transport_framework_library/atf_bundle_processor.py
--rw-r--r--   0        0        0      848 2023-05-22 22:04:58.129954 app_transport_framework_library-0.1.5/app_transport_framework_library/base_use_case_handler.py
--rw-r--r--   0        0        0      287 2023-05-22 22:04:58.131960 app_transport_framework_library-0.1.5/app_transport_framework_library/models/bundle_focus_content.py
--rw-r--r--   0        0        0      452 2023-05-23 19:53:32.165799 app_transport_framework_library-0.1.5/app_transport_framework_library/models/empfangsbestaetigung.py
--rw-r--r--   0        0        0      363 2023-05-22 22:04:58.132952 app_transport_framework_library-0.1.5/app_transport_framework_library/models/event.py
--rw-r--r--   0        0        0      261 2023-05-23 18:58:39.501228 app_transport_framework_library-0.1.5/app_transport_framework_library/models/message_to_send.py
--rw-r--r--   0        0        0     1172 2023-05-22 22:04:58.137428 app_transport_framework_library-0.1.5/app_transport_framework_library/ressource_creators/message_bundle_creator.py
--rw-r--r--   0        0        0     1232 2023-05-22 22:04:58.138443 app_transport_framework_library-0.1.5/app_transport_framework_library/ressource_creators/message_header_creator.py
--rw-r--r--   0        0        0     1757 2023-05-23 19:52:55.631553 app_transport_framework_library-0.1.5/app_transport_framework_library/ressource_creators/operation_outcome_bundle_creator.py
--rw-r--r--   0        0        0      859 2023-05-22 22:04:58.140443 app_transport_framework_library-0.1.5/app_transport_framework_library/ressource_creators/operation_outcome_creator.py
--rw-r--r--   0        0        0     3930 2023-05-23 19:52:55.631553 app_transport_framework_library-0.1.5/app_transport_framework_library/ressource_creators/test_message_creator.py
--rw-r--r--   0        0        0     1706 2023-05-23 19:06:28.832327 app_transport_framework_library-0.1.5/app_transport_framework_library/use_cases/empfangsbestaetigung_handler.py
--rw-r--r--   0        0        0     1977 2023-05-22 22:04:58.143445 app_transport_framework_library-0.1.5/app_transport_framework_library/use_cases/selbsttest_lieferung_handler.py
--rw-r--r--   0        0        0      390 2023-05-23 19:58:06.639312 app_transport_framework_library-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3943 2023-05-22 22:04:58.126959 app_transport_framework_library-0.1.5/README.md
--rw-r--r--   0        0        0     4348 1970-01-01 00:00:00.000000 app_transport_framework_library-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-22 22:04:58.127954 app_transport_framework_library-0.1.6/app_transport_framework_library/__init__.py
+-rw-r--r--   0        0        0     6420 2023-05-24 21:18:31.761522 app_transport_framework_library-0.1.6/app_transport_framework_library/atf_bundle_processor.py
+-rw-r--r--   0        0        0      848 2023-05-22 22:04:58.129954 app_transport_framework_library-0.1.6/app_transport_framework_library/base_use_case_handler.py
+-rw-r--r--   0        0        0      287 2023-05-22 22:04:58.131960 app_transport_framework_library-0.1.6/app_transport_framework_library/models/bundle_focus_content.py
+-rw-r--r--   0        0        0      452 2023-05-23 19:53:32.165799 app_transport_framework_library-0.1.6/app_transport_framework_library/models/empfangsbestaetigung.py
+-rw-r--r--   0        0        0      363 2023-05-22 22:04:58.132952 app_transport_framework_library-0.1.6/app_transport_framework_library/models/event.py
+-rw-r--r--   0        0        0      261 2023-05-23 18:58:39.501228 app_transport_framework_library-0.1.6/app_transport_framework_library/models/message_to_send.py
+-rw-r--r--   0        0        0     1172 2023-05-22 22:04:58.137428 app_transport_framework_library-0.1.6/app_transport_framework_library/ressource_creators/message_bundle_creator.py
+-rw-r--r--   0        0        0     1232 2023-05-22 22:04:58.138443 app_transport_framework_library-0.1.6/app_transport_framework_library/ressource_creators/message_header_creator.py
+-rw-r--r--   0        0        0     1757 2023-05-23 19:52:55.631553 app_transport_framework_library-0.1.6/app_transport_framework_library/ressource_creators/operation_outcome_bundle_creator.py
+-rw-r--r--   0        0        0      859 2023-05-22 22:04:58.140443 app_transport_framework_library-0.1.6/app_transport_framework_library/ressource_creators/operation_outcome_creator.py
+-rw-r--r--   0        0        0     3930 2023-05-23 19:52:55.631553 app_transport_framework_library-0.1.6/app_transport_framework_library/ressource_creators/test_message_creator.py
+-rw-r--r--   0        0        0     1706 2023-05-23 19:06:28.832327 app_transport_framework_library-0.1.6/app_transport_framework_library/use_cases/empfangsbestaetigung_handler.py
+-rw-r--r--   0        0        0     1977 2023-05-22 22:04:58.143445 app_transport_framework_library-0.1.6/app_transport_framework_library/use_cases/selbsttest_lieferung_handler.py
+-rw-r--r--   0        0        0      390 2023-05-24 21:21:29.013547 app_transport_framework_library-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3943 2023-05-22 22:04:58.126959 app_transport_framework_library-0.1.6/README.md
+-rw-r--r--   0        0        0     4348 1970-01-01 00:00:00.000000 app_transport_framework_library-0.1.6/PKG-INFO
```

### Comparing `app_transport_framework_library-0.1.5/app_transport_framework_library/atf_bundle_processor.py` & `app_transport_framework_library-0.1.6/app_transport_framework_library/atf_bundle_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             return
 
         handler_key = (message_header.eventCoding.system,
                        message_header.eventCoding.code)
 
         if handler_key in self.use_case_handlers:
             handler = self.use_case_handlers[handler_key]
-            ressources, issues = handler.handle(message_header, parsed_bundle)
+            ressources, issues = handler.handle(message_header, bundle)
 
             if issues:
                 self.send_empfangsbestätigung(message_header, issues)
 
             if ressources:
                 focusRessource = BundleFocusContent(
                     message_header.eventCoding.system, message_header.eventCoding.code, ressources)
```

### Comparing `app_transport_framework_library-0.1.5/app_transport_framework_library/base_use_case_handler.py` & `app_transport_framework_library-0.1.6/app_transport_framework_library/base_use_case_handler.py`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.5/app_transport_framework_library/ressource_creators/message_bundle_creator.py` & `app_transport_framework_library-0.1.6/app_transport_framework_library/ressource_creators/message_bundle_creator.py`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.5/app_transport_framework_library/ressource_creators/message_header_creator.py` & `app_transport_framework_library-0.1.6/app_transport_framework_library/ressource_creators/message_header_creator.py`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.5/app_transport_framework_library/ressource_creators/operation_outcome_bundle_creator.py` & `app_transport_framework_library-0.1.6/app_transport_framework_library/ressource_creators/operation_outcome_bundle_creator.py`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.5/app_transport_framework_library/ressource_creators/operation_outcome_creator.py` & `app_transport_framework_library-0.1.6/app_transport_framework_library/ressource_creators/operation_outcome_creator.py`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.5/app_transport_framework_library/ressource_creators/test_message_creator.py` & `app_transport_framework_library-0.1.6/app_transport_framework_library/ressource_creators/test_message_creator.py`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.5/app_transport_framework_library/use_cases/empfangsbestaetigung_handler.py` & `app_transport_framework_library-0.1.6/app_transport_framework_library/use_cases/empfangsbestaetigung_handler.py`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.5/app_transport_framework_library/use_cases/selbsttest_lieferung_handler.py` & `app_transport_framework_library-0.1.6/app_transport_framework_library/use_cases/selbsttest_lieferung_handler.py`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.5/README.md` & `app_transport_framework_library-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `app_transport_framework_library-0.1.5/PKG-INFO` & `app_transport_framework_library-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app-transport-framework-library
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Sven Sommer
 Author-email: rob.hoffmann@posteo.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

