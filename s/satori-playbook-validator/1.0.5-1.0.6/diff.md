# Comparing `tmp/satori_playbook_validator-1.0.5.tar.gz` & `tmp/satori_playbook_validator-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_playbook_validator-1.0.5.tar", last modified: Tue May 23 21:03:34 2023, max compression
+gzip compressed data, was "satori_playbook_validator-1.0.6.tar", last modified: Thu May 25 02:15:22 2023, max compression
```

## Comparing `satori_playbook_validator-1.0.5.tar` & `satori_playbook_validator-1.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       30 2023-05-23 21:03:15.885929 satori_playbook_validator-1.0.5/README.md
--rw-r--r--   0        0        0      433 2023-05-23 21:03:34.134093 satori_playbook_validator-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      163 2023-05-23 21:03:15.885929 satori_playbook_validator-1.0.5/src/satorici/validator/__init__.py
--rw-r--r--   0        0        0     3268 2023-05-23 21:03:15.885929 satori_playbook_validator-1.0.5/src/satorici/validator/_validator.py
--rw-r--r--   0        0        0      223 2023-05-23 21:03:15.885929 satori_playbook_validator-1.0.5/src/satorici/validator/exceptions.py
--rw-r--r--   0        0        0      267 2023-05-23 21:03:15.885929 satori_playbook_validator-1.0.5/src/satorici/validator/schemas/command.json
--rw-r--r--   0        0        0      251 2023-05-23 21:03:15.885929 satori_playbook_validator-1.0.5/src/satorici/validator/schemas/import.json
--rw-r--r--   0        0        0     2197 2023-05-23 21:03:15.885929 satori_playbook_validator-1.0.5/src/satorici/validator/schemas/input.json
--rw-r--r--   0        0        0     1025 2023-05-23 21:03:15.885929 satori_playbook_validator-1.0.5/src/satorici/validator/schemas/settings.json
--rw-r--r--   0        0        0     1743 2023-05-23 21:03:15.885929 satori_playbook_validator-1.0.5/src/satorici/validator/schemas/test.json
--rw-r--r--   0        0        0      286 1970-01-01 00:00:00.000000 satori_playbook_validator-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-05-25 02:15:07.408222 satori_playbook_validator-1.0.6/README.md
+-rw-r--r--   0        0        0      433 2023-05-25 02:15:22.191980 satori_playbook_validator-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-05-25 02:15:07.408222 satori_playbook_validator-1.0.6/src/satorici/validator/__init__.py
+-rw-r--r--   0        0        0     3268 2023-05-25 02:15:07.408222 satori_playbook_validator-1.0.6/src/satorici/validator/_validator.py
+-rw-r--r--   0        0        0      223 2023-05-25 02:15:07.408222 satori_playbook_validator-1.0.6/src/satorici/validator/exceptions.py
+-rw-r--r--   0        0        0      267 2023-05-25 02:15:07.408222 satori_playbook_validator-1.0.6/src/satorici/validator/schemas/command.json
+-rw-r--r--   0        0        0      251 2023-05-25 02:15:07.408222 satori_playbook_validator-1.0.6/src/satorici/validator/schemas/import.json
+-rw-r--r--   0        0        0     2197 2023-05-25 02:15:07.408222 satori_playbook_validator-1.0.6/src/satorici/validator/schemas/input.json
+-rw-r--r--   0        0        0     1025 2023-05-25 02:15:07.408222 satori_playbook_validator-1.0.6/src/satorici/validator/schemas/settings.json
+-rw-r--r--   0        0        0     1818 2023-05-25 02:15:07.408222 satori_playbook_validator-1.0.6/src/satorici/validator/schemas/test.json
+-rw-r--r--   0        0        0      286 1970-01-01 00:00:00.000000 satori_playbook_validator-1.0.6/PKG-INFO
```

### Comparing `satori_playbook_validator-1.0.5/src/satorici/validator/_validator.py` & `satori_playbook_validator-1.0.6/src/satorici/validator/_validator.py`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-1.0.5/src/satorici/validator/schemas/input.json` & `satori_playbook_validator-1.0.6/src/satorici/validator/schemas/input.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-1.0.5/src/satorici/validator/schemas/settings.json` & `satori_playbook_validator-1.0.6/src/satorici/validator/schemas/settings.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-1.0.5/src/satorici/validator/schemas/test.json` & `satori_playbook_validator-1.0.6/src/satorici/validator/schemas/test.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9571428571428572%*

 * *Differences: {"'patternProperties'": "{'^assertStd(out|err)SHA256$': OrderedDict([('type', ['string', "*

 * *                        "'array']), ('pattern', '^[a-fA-F0-9]{64}$'), ('items', "*

 * *                        "OrderedDict([('type', 'string'), ('pattern', '^[a-fA-F0-9]{64}$')])), "*

 * *                        "('uniqueItems', True)])}",*

 * * "'properties'": "{'assertKilled': OrderedDict([('type', 'boolean')]), delete: "*

 * *                 "['assertStdoutSHA256']}"}*

```diff
@@ -40,34 +40,37 @@
                 "string"
             ],
             "uniqueItems": true
         },
         "^assertStd(out|err)(Not)?Regex$": {
             "format": "regex",
             "type": "string"
-        }
-    },
-    "properties": {
-        "assertDifferent": {
-            "type": "boolean"
         },
-        "assertReturnCode": {
-            "type": "integer"
-        },
-        "assertStdoutSHA256": {
+        "^assertStd(out|err)SHA256$": {
             "items": {
                 "pattern": "^[a-fA-F0-9]{64}$",
                 "type": "string"
             },
             "pattern": "^[a-fA-F0-9]{64}$",
             "type": [
                 "string",
                 "array"
             ],
             "uniqueItems": true
+        }
+    },
+    "properties": {
+        "assertDifferent": {
+            "type": "boolean"
+        },
+        "assertKilled": {
+            "type": "boolean"
+        },
+        "assertReturnCode": {
+            "type": "integer"
         },
         "settings": false
     },
     "propertyNames": {
         "pattern": "^[\\w-]+$"
     },
     "type": "object"
```

