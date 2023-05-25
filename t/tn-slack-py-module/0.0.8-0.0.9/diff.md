# Comparing `tmp/tn-slack-py-module-0.0.8.tar.gz` & `tmp/tn-slack-py-module-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tn-slack-py-module-0.0.8.tar", last modified: Tue Apr 25 22:09:21 2023, max compression
+gzip compressed data, was "tn-slack-py-module-0.0.9.tar", last modified: Thu May 25 18:36:45 2023, max compression
```

## Comparing `tn-slack-py-module-0.0.8.tar` & `tn-slack-py-module-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 paribaker   (501) staff       (20)        0 2023-04-25 22:09:21.643325 tn-slack-py-module-0.0.8/
--rw-r--r--   0 paribaker   (501) staff       (20)     1073 2021-06-15 00:51:59.000000 tn-slack-py-module-0.0.8/LICENSE
--rw-r--r--   0 paribaker   (501) staff       (20)      785 2023-04-25 22:09:21.643474 tn-slack-py-module-0.0.8/PKG-INFO
--rw-r--r--   0 paribaker   (501) staff       (20)      475 2023-03-13 13:25:36.000000 tn-slack-py-module-0.0.8/README.md
--rw-r--r--   0 paribaker   (501) staff       (20)      328 2023-01-14 22:12:41.000000 tn-slack-py-module-0.0.8/pyproject.toml
--rw-r--r--   0 paribaker   (501) staff       (20)      651 2023-04-25 22:09:21.644195 tn-slack-py-module-0.0.8/setup.cfg
-drwxr-xr-x   0 paribaker   (501) staff       (20)        0 2023-04-25 22:09:21.633303 tn-slack-py-module-0.0.8/src/
-drwxr-xr-x   0 paribaker   (501) staff       (20)        0 2023-04-25 22:09:21.637186 tn-slack-py-module-0.0.8/src/tn_slack_py_module.egg-info/
--rw-r--r--   0 paribaker   (501) staff       (20)      785 2023-04-25 22:09:21.000000 tn-slack-py-module-0.0.8/src/tn_slack_py_module.egg-info/PKG-INFO
--rw-r--r--   0 paribaker   (501) staff       (20)      402 2023-04-25 22:09:21.000000 tn-slack-py-module-0.0.8/src/tn_slack_py_module.egg-info/SOURCES.txt
--rw-r--r--   0 paribaker   (501) staff       (20)        1 2023-04-25 22:09:21.000000 tn-slack-py-module-0.0.8/src/tn_slack_py_module.egg-info/dependency_links.txt
--rw-r--r--   0 paribaker   (501) staff       (20)        8 2023-04-25 22:09:21.000000 tn-slack-py-module-0.0.8/src/tn_slack_py_module.egg-info/top_level.txt
-drwxr-xr-x   0 paribaker   (501) staff       (20)        0 2023-04-25 22:09:21.642576 tn-slack-py-module-0.0.8/src/tnslack/
--rw-r--r--   0 paribaker   (501) staff       (20)        0 2021-06-07 22:51:18.000000 tn-slack-py-module-0.0.8/src/tnslack/__init__.py
--rw-r--r--   0 paribaker   (501) staff       (20)    22375 2023-03-13 13:48:06.000000 tn-slack-py-module-0.0.8/src/tnslack/block_builder.py
--rw-r--r--   0 paribaker   (501) staff       (20)      206 2021-06-07 22:51:24.000000 tn-slack-py-module-0.0.8/src/tnslack/constants.py
--rw-r--r--   0 paribaker   (501) staff       (20)     1305 2021-06-07 22:51:25.000000 tn-slack-py-module-0.0.8/src/tnslack/decorators.py
--rw-r--r--   0 paribaker   (501) staff       (20)     4657 2023-01-14 22:23:29.000000 tn-slack-py-module-0.0.8/src/tnslack/exceptions.py
--rw-r--r--   0 paribaker   (501) staff       (20)    15022 2023-01-14 22:25:43.000000 tn-slack-py-module-0.0.8/src/tnslack/slack_app.py
--rw-r--r--   0 paribaker   (501) staff       (20)     1069 2021-06-07 22:51:33.000000 tn-slack-py-module-0.0.8/src/tnslack/utils.py
+drwxr-xr-x   0 paribaker   (501) staff       (20)        0 2023-05-25 18:36:45.736579 tn-slack-py-module-0.0.9/
+-rw-r--r--   0 paribaker   (501) staff       (20)     1073 2021-06-15 00:51:59.000000 tn-slack-py-module-0.0.9/LICENSE
+-rw-r--r--   0 paribaker   (501) staff       (20)      785 2023-05-25 18:36:45.736742 tn-slack-py-module-0.0.9/PKG-INFO
+-rw-r--r--   0 paribaker   (501) staff       (20)      475 2023-03-13 13:25:36.000000 tn-slack-py-module-0.0.9/README.md
+-rw-r--r--   0 paribaker   (501) staff       (20)      328 2023-01-14 22:12:41.000000 tn-slack-py-module-0.0.9/pyproject.toml
+-rw-r--r--   0 paribaker   (501) staff       (20)      651 2023-05-25 18:36:45.737660 tn-slack-py-module-0.0.9/setup.cfg
+drwxr-xr-x   0 paribaker   (501) staff       (20)        0 2023-05-25 18:36:45.723827 tn-slack-py-module-0.0.9/src/
+drwxr-xr-x   0 paribaker   (501) staff       (20)        0 2023-05-25 18:36:45.728264 tn-slack-py-module-0.0.9/src/tn_slack_py_module.egg-info/
+-rw-r--r--   0 paribaker   (501) staff       (20)      785 2023-05-25 18:36:45.000000 tn-slack-py-module-0.0.9/src/tn_slack_py_module.egg-info/PKG-INFO
+-rw-r--r--   0 paribaker   (501) staff       (20)      402 2023-05-25 18:36:45.000000 tn-slack-py-module-0.0.9/src/tn_slack_py_module.egg-info/SOURCES.txt
+-rw-r--r--   0 paribaker   (501) staff       (20)        1 2023-05-25 18:36:45.000000 tn-slack-py-module-0.0.9/src/tn_slack_py_module.egg-info/dependency_links.txt
+-rw-r--r--   0 paribaker   (501) staff       (20)        8 2023-05-25 18:36:45.000000 tn-slack-py-module-0.0.9/src/tn_slack_py_module.egg-info/top_level.txt
+drwxr-xr-x   0 paribaker   (501) staff       (20)        0 2023-05-25 18:36:45.735784 tn-slack-py-module-0.0.9/src/tnslack/
+-rw-r--r--   0 paribaker   (501) staff       (20)        0 2021-06-07 22:51:18.000000 tn-slack-py-module-0.0.9/src/tnslack/__init__.py
+-rw-r--r--   0 paribaker   (501) staff       (20)    22375 2023-03-13 13:48:06.000000 tn-slack-py-module-0.0.9/src/tnslack/block_builder.py
+-rw-r--r--   0 paribaker   (501) staff       (20)      206 2021-06-07 22:51:24.000000 tn-slack-py-module-0.0.9/src/tnslack/constants.py
+-rw-r--r--   0 paribaker   (501) staff       (20)     1305 2021-06-07 22:51:25.000000 tn-slack-py-module-0.0.9/src/tnslack/decorators.py
+-rw-r--r--   0 paribaker   (501) staff       (20)     4657 2023-01-14 22:23:29.000000 tn-slack-py-module-0.0.9/src/tnslack/exceptions.py
+-rw-r--r--   0 paribaker   (501) staff       (20)    14761 2023-05-13 18:59:06.000000 tn-slack-py-module-0.0.9/src/tnslack/slack_app.py
+-rw-r--r--   0 paribaker   (501) staff       (20)     1069 2021-06-07 22:51:33.000000 tn-slack-py-module-0.0.9/src/tnslack/utils.py
```

### Comparing `tn-slack-py-module-0.0.8/LICENSE` & `tn-slack-py-module-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tn-slack-py-module-0.0.8/PKG-INFO` & `tn-slack-py-module-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tn-slack-py-module
-Version: 0.0.8
+Version: 0.0.9
 Summary: A slack ready module
 Home-page: https://github.com/thinknimble/tn-slack-py-module
 Author: Pari Baker
 Author-email: pari@thinknimble.com
 License: : OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tn-slack-py-module-0.0.8/setup.cfg` & `tn-slack-py-module-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = tn-slack-py-module
 
 [metadata]
 name = tn-slack-py-module
-version = 0.0.8
+version = 0.0.9
 author = Pari Baker
 author_email = pari@thinknimble.com
 description = A slack ready module
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/thinknimble/tn-slack-py-module
 project_urls =
```

### Comparing `tn-slack-py-module-0.0.8/src/tn_slack_py_module.egg-info/PKG-INFO` & `tn-slack-py-module-0.0.9/src/tn_slack_py_module.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tn-slack-py-module
-Version: 0.0.8
+Version: 0.0.9
 Summary: A slack ready module
 Home-page: https://github.com/thinknimble/tn-slack-py-module
 Author: Pari Baker
 Author-email: pari@thinknimble.com
 License: : OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tn-slack-py-module-0.0.8/src/tnslack/block_builder.py` & `tn-slack-py-module-0.0.9/src/tnslack/block_builder.py`

 * *Files identical despite different names*

### Comparing `tn-slack-py-module-0.0.8/src/tnslack/decorators.py` & `tn-slack-py-module-0.0.9/src/tnslack/decorators.py`

 * *Files identical despite different names*

### Comparing `tn-slack-py-module-0.0.8/src/tnslack/exceptions.py` & `tn-slack-py-module-0.0.9/src/tnslack/exceptions.py`

 * *Files identical despite different names*

### Comparing `tn-slack-py-module-0.0.8/src/tnslack/slack_app.py` & `tn-slack-py-module-0.0.9/src/tnslack/slack_app.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,52 +72,38 @@
         slack_consts.BLOCK_ACTIONS,
         slack_consts.BLOCK_SUGGESTION,
         slack_consts.VIEW_CLOSED,
         slack_consts.VIEW_SUBMISSION,
     ]
     BLOCK_SETS = dict()
 
-    def __init__(
-        self,
-        client_id,
-        client_secret,
-        signing_secret,
-        redirect_url,
-        bot_scopes=[],
-        user_scopes=[],
-        error_webhook=None,
-    ):
-        self.CLIENT_ID = client_id
-        self.CLIENT_SECRET = client_secret
-        self.SIGNING_SECRET = signing_secret
-        self.BOT_SCOPES = bot_scopes
-        self.USER_SCOPES = user_scopes
-        self.REDIRECT_URL = redirect_url
-        self.ERROR_WEBHOOK = error_webhook
+    def __new__(cls):
+        if not hasattr(cls, "instance"):
+            cls.instance = super().__new__(cls)
+        return cls.instance
 
     @classmethod
     def configure(
         cls,
         client_id,
         client_secret,
         signing_secret,
         redirect_url,
         bot_scopes=[],
         user_scopes=[],
         error_webhook=None,
     ):
-        return cls(
-            client_id,
-            client_secret,
-            signing_secret,
-            redirect_url,
-            bot_scopes,
-            user_scopes,
-            error_webhook,
-        )
+        cls.CLIENT_ID = client_id
+        cls.CLIENT_SECRET = client_secret
+        cls.SIGNING_SECRET = signing_secret
+        cls.BOT_SCOPES = bot_scopes
+        cls.USER_SCOPES = user_scopes
+        cls.REDIRECT_URL = redirect_url
+        cls.ERROR_WEBHOOK = error_webhook
+        return cls
 
     def _handle_response(self, response, fn_name=None, blocks=[]):
         if not hasattr(response, "status_code"):
             raise ValueError
 
         else:
             status_code = response.status_code
```

### Comparing `tn-slack-py-module-0.0.8/src/tnslack/utils.py` & `tn-slack-py-module-0.0.9/src/tnslack/utils.py`

 * *Files identical despite different names*

