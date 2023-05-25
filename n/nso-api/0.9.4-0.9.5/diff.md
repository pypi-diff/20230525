# Comparing `tmp/nso-api-0.9.4.tar.gz` & `tmp/nso-api-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nso-api-0.9.4.tar", last modified: Fri Mar  3 02:51:41 2023, max compression
+gzip compressed data, was "nso-api-0.9.5.tar", last modified: Thu May 25 17:13:06 2023, max compression
```

## Comparing `nso-api-0.9.4.tar` & `nso-api-0.9.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dbot      (1003) dbot      (1003)        0 2023-03-03 02:51:41.719827 nso-api-0.9.4/
--rw-r--r--   0 dbot      (1003) dbot      (1003)      227 2023-03-03 02:51:41.719827 nso-api-0.9.4/PKG-INFO
--rw-r--r--   0 dbot      (1003) dbot      (1003)     1106 2022-10-12 00:03:22.000000 nso-api-0.9.4/README.md
-drwxr-xr-x   0 dbot      (1003) dbot      (1003)        0 2023-03-03 02:51:41.715827 nso-api-0.9.4/nso_api/
--rw-rw-r--   0 dbot      (1003) dbot      (1003)       55 2022-10-12 00:03:22.000000 nso-api-0.9.4/nso_api/__init__.py
--rw-r--r--   0 dbot      (1003) dbot      (1003)     1299 2023-03-03 02:50:50.000000 nso-api-0.9.4/nso_api/imink.py
--rw-rw-r--   0 dbot      (1003) dbot      (1003)     1183 2022-10-12 00:03:22.000000 nso-api-0.9.4/nso_api/jwt.py
--rw-r--r--   0 dbot      (1003) dbot      (1003)    21859 2023-03-03 02:50:50.000000 nso-api-0.9.4/nso_api/nso_api.py
--rw-rw-r--   0 dbot      (1003) dbot      (1003)     2053 2022-10-12 00:03:22.000000 nso-api-0.9.4/nso_api/nso_api_account.py
--rw-r--r--   0 dbot      (1003) dbot      (1003)    10145 2023-02-08 21:46:57.000000 nso-api-0.9.4/nso_api/nso_api_acnh.py
--rw-r--r--   0 dbot      (1003) dbot      (1003)      394 2023-02-08 21:46:57.000000 nso-api-0.9.4/nso_api/nso_api_app.py
--rw-r--r--   0 dbot      (1003) dbot      (1003)    16247 2023-03-03 02:50:50.000000 nso-api-0.9.4/nso_api/nso_api_s2.py
--rw-r--r--   0 dbot      (1003) dbot      (1003)    15851 2023-03-03 02:50:50.000000 nso-api-0.9.4/nso_api/nso_api_s3.py
--rw-rw-r--   0 dbot      (1003) dbot      (1003)     1320 2022-10-12 00:03:22.000000 nso-api-0.9.4/nso_api/nso_expiring_token.py
--rw-rw-r--   0 dbot      (1003) dbot      (1003)     1257 2023-02-14 22:31:54.000000 nso-api-0.9.4/nso_api/utils.py
--rw-r--r--   0 dbot      (1003) dbot      (1003)       45 2023-03-03 02:50:50.000000 nso-api-0.9.4/nso_api/version.py
-drwxr-xr-x   0 dbot      (1003) dbot      (1003)        0 2023-03-03 02:51:41.715827 nso-api-0.9.4/nso_api.egg-info/
--rw-r--r--   0 dbot      (1003) dbot      (1003)      227 2023-03-03 02:51:41.000000 nso-api-0.9.4/nso_api.egg-info/PKG-INFO
--rw-r--r--   0 dbot      (1003) dbot      (1003)      442 2023-03-03 02:51:41.000000 nso-api-0.9.4/nso_api.egg-info/SOURCES.txt
--rw-r--r--   0 dbot      (1003) dbot      (1003)        1 2023-03-03 02:51:41.000000 nso-api-0.9.4/nso_api.egg-info/dependency_links.txt
--rw-r--r--   0 dbot      (1003) dbot      (1003)        9 2023-03-03 02:51:41.000000 nso-api-0.9.4/nso_api.egg-info/requires.txt
--rw-r--r--   0 dbot      (1003) dbot      (1003)        8 2023-03-03 02:51:41.000000 nso-api-0.9.4/nso_api.egg-info/top_level.txt
--rw-r--r--   0 dbot      (1003) dbot      (1003)      514 2023-03-03 02:50:50.000000 nso-api-0.9.4/pyproject.toml
--rw-r--r--   0 dbot      (1003) dbot      (1003)       38 2023-03-03 02:51:41.719827 nso-api-0.9.4/setup.cfg
--rw-r--r--   0 dbot      (1003) dbot      (1003)      405 2023-02-08 21:46:57.000000 nso-api-0.9.4/setup.py
+drwxr-xr-x   0 dbot      (1003) dbot      (1003)        0 2023-05-25 17:13:06.214424 nso-api-0.9.5/
+-rw-r--r--   0 dbot      (1003) dbot      (1003)      227 2023-05-25 17:13:06.214424 nso-api-0.9.5/PKG-INFO
+-rw-r--r--   0 dbot      (1003) dbot      (1003)     1106 2022-10-12 00:03:22.000000 nso-api-0.9.5/README.md
+drwxr-xr-x   0 dbot      (1003) dbot      (1003)        0 2023-05-25 17:13:06.214424 nso-api-0.9.5/nso_api/
+-rw-rw-r--   0 dbot      (1003) dbot      (1003)       55 2022-10-12 00:03:22.000000 nso-api-0.9.5/nso_api/__init__.py
+-rw-r--r--   0 dbot      (1003) dbot      (1003)     1425 2023-05-25 17:03:21.000000 nso-api-0.9.5/nso_api/imink.py
+-rw-rw-r--   0 dbot      (1003) dbot      (1003)     1183 2022-10-12 00:03:22.000000 nso-api-0.9.5/nso_api/jwt.py
+-rw-r--r--   0 dbot      (1003) dbot      (1003)    21909 2023-05-25 17:03:21.000000 nso-api-0.9.5/nso_api/nso_api.py
+-rw-rw-r--   0 dbot      (1003) dbot      (1003)     2053 2022-10-12 00:03:22.000000 nso-api-0.9.5/nso_api/nso_api_account.py
+-rw-r--r--   0 dbot      (1003) dbot      (1003)    10145 2023-02-08 21:46:57.000000 nso-api-0.9.5/nso_api/nso_api_acnh.py
+-rw-r--r--   0 dbot      (1003) dbot      (1003)      394 2023-02-08 21:46:57.000000 nso-api-0.9.5/nso_api/nso_api_app.py
+-rw-r--r--   0 dbot      (1003) dbot      (1003)    16247 2023-03-03 02:50:50.000000 nso-api-0.9.5/nso_api/nso_api_s2.py
+-rw-r--r--   0 dbot      (1003) dbot      (1003)    15851 2023-05-25 17:10:26.000000 nso-api-0.9.5/nso_api/nso_api_s3.py
+-rw-rw-r--   0 dbot      (1003) dbot      (1003)     1320 2022-10-12 00:03:22.000000 nso-api-0.9.5/nso_api/nso_expiring_token.py
+-rw-rw-r--   0 dbot      (1003) dbot      (1003)     1257 2023-02-14 22:31:54.000000 nso-api-0.9.5/nso_api/utils.py
+-rw-r--r--   0 dbot      (1003) dbot      (1003)       45 2023-05-25 17:10:26.000000 nso-api-0.9.5/nso_api/version.py
+drwxr-xr-x   0 dbot      (1003) dbot      (1003)        0 2023-05-25 17:13:06.214424 nso-api-0.9.5/nso_api.egg-info/
+-rw-r--r--   0 dbot      (1003) dbot      (1003)      227 2023-05-25 17:13:06.000000 nso-api-0.9.5/nso_api.egg-info/PKG-INFO
+-rw-r--r--   0 dbot      (1003) dbot      (1003)      442 2023-05-25 17:13:06.000000 nso-api-0.9.5/nso_api.egg-info/SOURCES.txt
+-rw-r--r--   0 dbot      (1003) dbot      (1003)        1 2023-05-25 17:13:06.000000 nso-api-0.9.5/nso_api.egg-info/dependency_links.txt
+-rw-r--r--   0 dbot      (1003) dbot      (1003)        9 2023-05-25 17:13:06.000000 nso-api-0.9.5/nso_api.egg-info/requires.txt
+-rw-r--r--   0 dbot      (1003) dbot      (1003)        8 2023-05-25 17:13:06.000000 nso-api-0.9.5/nso_api.egg-info/top_level.txt
+-rw-r--r--   0 dbot      (1003) dbot      (1003)      514 2023-05-25 17:10:26.000000 nso-api-0.9.5/pyproject.toml
+-rw-r--r--   0 dbot      (1003) dbot      (1003)       38 2023-05-25 17:13:06.214424 nso-api-0.9.5/setup.cfg
+-rw-r--r--   0 dbot      (1003) dbot      (1003)      405 2023-02-08 21:46:57.000000 nso-api-0.9.5/setup.py
```

### Comparing `nso-api-0.9.4/README.md` & `nso-api-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `nso-api-0.9.4/nso_api/jwt.py` & `nso-api-0.9.5/nso_api/jwt.py`

 * *Files identical despite different names*

### Comparing `nso-api-0.9.4/nso_api/nso_api.py` & `nso-api-0.9.5/nso_api/nso_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 			return None
 		elif self.payload.get('status') != 0:
 			return None
 
 		return self.payload.get('result')
 
 class NSO_API:
-	FALLBACK_APP_VERSION = "2.5.0"
+	FALLBACK_APP_VERSION = "2.5.1"
 
 	global_data = {}
 	global_callbacks = {}
 
 	def __init__(self, f_provider, context = None, debug = 0):
 		self.session = requests.Session()
 		self.f_provider = f_provider
@@ -620,20 +620,21 @@
 			return False
 
 		if not self.ensure_api_tokens():
 			self.errors.append("Could not get api_tokens")
 			return False
 
 		guid = str(uuid.uuid4())
-		nso_f_dict = self.f_provider.get_nso_f(self.api_tokens.value['id_token'], guid)
+		nso_f_dict = self.f_provider.get_nso_f(self.api_tokens.value['id_token'], guid, self.user_info['id'])
 		if not nso_f_dict:
 			self.errors.append("Could not get nso f hash from f_provider")
 			return False
 
-		api_login_response = self.do_json_request(self.create_api_login_request(nso_f_dict['f'], nso_f_dict['timestamp'], nso_f_dict['request_id']))
+		print(repr(nso_f_dict))
+		api_login_response = self.do_json_request(self.create_api_login_request(nso_f_dict['f'], nso_f_dict['timestamp'], guid))
 		if not api_login_response:
 			self.errors.append("API login request failed")
 			return False
 		elif api_login_response.get("status") != 0:
 			self.errors.append("Unexpected response getting api login")
 			return False
 
@@ -651,15 +652,15 @@
 		if not self.ensure_api_login():
 			return None
 
 		if not self.ensure_app_version():
 			return False
 
 		guid = str(uuid.uuid4())
-		app_f_dict = self.f_provider.get_app_f(self.api_login.value, guid)
+		app_f_dict = self.f_provider.get_app_f(self.api_login.value, guid, self.user_info['id'])
 		if not app_f_dict:
 			self.errors.append("Could not get app f hash from f_provider")
 			return False
 
 		web_service_token_response = self.do_json_request(self.create_web_service_token_request(game_id, app_f_dict['f'], app_f_dict['timestamp'], guid))
 		if not web_service_token_response:
 			return None
```

### Comparing `nso-api-0.9.4/nso_api/nso_api_account.py` & `nso-api-0.9.5/nso_api/nso_api_account.py`

 * *Files identical despite different names*

### Comparing `nso-api-0.9.4/nso_api/nso_api_acnh.py` & `nso-api-0.9.5/nso_api/nso_api_acnh.py`

 * *Files identical despite different names*

### Comparing `nso-api-0.9.4/nso_api/nso_api_s2.py` & `nso-api-0.9.5/nso_api/nso_api_s2.py`

 * *Files identical despite different names*

### Comparing `nso-api-0.9.4/nso_api/nso_api_s3.py` & `nso-api-0.9.5/nso_api/nso_api_s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import time
 import hashlib
 
 from .nso_expiring_token import NSO_Expiring_Token
 import nso_api.utils
 
 class NSO_API_S3:
-	FALLBACK_VERSION = {"version": "3.0.0", "revision": "2857bc50653d316cb69f017b2eef24d2ae56a1b7"}
+	FALLBACK_VERSION = {"version": "3.0.0", "revision": "0742bda0f28edfcda33ec743b8afc4a95700e27d"}
 
 	GRAPHQL_QUERY_IDS = {
 		'LatestBattleHistoriesQuery':              '0176a47218d830ee447e10af4a287b3f',
 		'RegularBattleHistoriesQuery':             '3baef04b095ad8975ea679d722bc17de',
 		'BankaraBattleHistoriesQuery':             '0438ea6978ae8bd77c5d1250f4f84803',
 		'PrivateBattleHistoriesQuery':             '8e5ae78b194264a6c230e262d069bd28',
 		'VsHistoryDetailQuery':                    '291295ad311b99a6288fc95a5c4cb2d2',
```

### Comparing `nso-api-0.9.4/nso_api/nso_expiring_token.py` & `nso-api-0.9.5/nso_api/nso_expiring_token.py`

 * *Files identical despite different names*

### Comparing `nso-api-0.9.4/nso_api/utils.py` & `nso-api-0.9.5/nso_api/utils.py`

 * *Files identical despite different names*

### Comparing `nso-api-0.9.4/pyproject.toml` & `nso-api-0.9.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [owner]
 name = "jetsurf#8514 and Andy#3003 (Discord)"
 
 [project]
 name = "nso-api"
-version = "0.9.4"
+version = "0.9.5"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 	"Operating System :: OS Independent",
 ]
```

