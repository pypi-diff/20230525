# Comparing `tmp/tgtg-0.8.0.tar.gz` & `tmp/tgtg-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgtg-0.8.0.tar", max compression
+gzip compressed data, was "tgtg-0.9.0.tar", max compression
```

## Comparing `tgtg-0.8.0.tar` & `tgtg-0.9.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    12920 2021-11-24 21:46:18.898241 tgtg-0.8.0/README.md
--rw-r--r--   0        0        0      611 2021-11-24 21:47:08.205917 tgtg-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     9916 2021-11-24 21:46:46.529626 tgtg-0.8.0/tgtg/__init__.py
--rw-r--r--   0        0        0      130 2021-11-23 20:49:40.870516 tgtg-0.8.0/tgtg/exceptions.py
--rw-r--r--   0        0        0    14006 2021-11-24 21:47:39.408866 tgtg-0.8.0/setup.py
--rw-r--r--   0        0        0    13601 2021-11-24 21:47:39.410005 tgtg-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    12920 2021-11-24 21:46:18.898241 tgtg-0.9.0/README.md
+-rw-r--r--   0        0        0      611 2021-12-02 08:15:35.823056 tgtg-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    10067 2021-12-02 08:12:25.678877 tgtg-0.9.0/tgtg/__init__.py
+-rw-r--r--   0        0        0      130 2021-11-23 20:49:40.870516 tgtg-0.9.0/tgtg/exceptions.py
+-rw-r--r--   0        0        0    14006 2021-12-02 08:17:49.395578 tgtg-0.9.0/setup.py
+-rw-r--r--   0        0        0    13601 2021-12-02 08:17:49.396721 tgtg-0.9.0/PKG-INFO
```

### Comparing `tgtg-0.8.0/README.md` & `tgtg-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `tgtg-0.8.0/pyproject.toml` & `tgtg-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tgtg"
-version = "0.8.0"
+version = "0.9.0"
 description = "Unoffical python client for TooGoodToGo API"
 readme = "README.md"
 authors = ["Anthony Hivert <anthony.hivert@gmail.com>"]
 repository = "https://github.com/ahivert/tgtg-python"
 
 [tool.poetry.dependencies]
 python = "^3.6"
```

### Comparing `tgtg-0.8.0/tgtg/__init__.py` & `tgtg-0.9.0/tgtg/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,16 @@
         self.last_time_token_refreshed = None
         self.access_token_lifetime = access_token_lifetime
 
         self.user_agent = user_agent if user_agent else random.choice(USER_AGENTS)
         self.language = language
         self.proxies = proxies
         self.timeout = timeout
+        self.session = requests.Session()
+        self.session.headers = self._headers
 
     def _get_url(self, path):
         return urljoin(self.base_url, path)
 
     def get_credentials(self):
         self.login()
         return {
@@ -85,18 +87,18 @@
         if (
             self.last_time_token_refreshed
             and (datetime.datetime.now() - self.last_time_token_refreshed).seconds
             <= self.access_token_lifetime
         ):
             return
 
-        response = requests.post(
+        response = self.session.post(
             self._get_url(REFRESH_ENDPOINT),
-            headers=self._headers,
             json={"refresh_token": self.refresh_token},
+            headers=self._headers,
             proxies=self.proxies,
             timeout=self.timeout,
         )
         if response.status_code == HTTPStatus.OK:
             self.access_token = response.json()["access_token"]
             self.refresh_token = response.json()["refresh_token"]
             self.last_time_token_refreshed = datetime.datetime.now()
@@ -109,15 +111,15 @@
         ):
             raise TypeError(
                 "You must provide at least email or access_token, refresh_token and user_id"
             )
         if self._already_logged:
             self._refresh_token()
         else:
-            response = requests.post(
+            response = self.session.post(
                 self._get_url(AUTH_BY_EMAIL_ENDPOINT),
                 headers=self._headers,
                 json={
                     "device_type": "ANDROID",
                     "email": self.email,
                 },
                 proxies=self.proxies,
@@ -134,15 +136,15 @@
                 if response.status_code == 429:
                     raise TgtgAPIError("429 - Too many requests. Try again later.")
                 else:
                     raise TgtgLoginError(response.status_code, response.content)
 
     def start_polling(self, polling_id):
         for _ in range(MAX_POLLING_TRIES):
-            response = requests.post(
+            response = self.session.post(
                 self._get_url(AUTH_POLLING_ENDPOINT),
                 headers=self._headers,
                 json={
                     "device_type": "ANDROID",
                     "email": self.email,
                     "request_polling_id": polling_id,
                 },
@@ -150,14 +152,15 @@
                 timeout=self.timeout,
             )
             if response.status_code == HTTPStatus.ACCEPTED:
                 print("Check your mailbox to continue...")
                 time.sleep(POLLING_WAIT_TIME)
                 continue
             elif response.status_code == HTTPStatus.OK:
+                print("Logged in!")
                 login_response = response.json()
                 self.access_token = login_response["access_token"]
                 self.refresh_token = login_response["refresh_token"]
                 self.last_time_token_refreshed = datetime.datetime.now()
                 self.user_id = login_response["startup_data"]["user"]["user_id"]
                 return
             else:
@@ -205,43 +208,43 @@
             "pickup_earliest": pickup_earliest,
             "pickup_latest": pickup_latest,
             "search_phrase": search_phrase if search_phrase else None,
             "with_stock_only": with_stock_only,
             "hidden_only": hidden_only,
             "we_care_only": we_care_only,
         }
-        response = requests.post(
+        response = self.session.post(
             self._get_url(API_ITEM_ENDPOINT),
             headers=self._headers,
             json=data,
             proxies=self.proxies,
             timeout=self.timeout,
         )
         if response.status_code == HTTPStatus.OK:
             return response.json()["items"]
         else:
             raise TgtgAPIError(response.status_code, response.content)
 
     def get_item(self, item_id):
         self.login()
-        response = requests.post(
+        response = self.session.post(
             urljoin(self._get_url(API_ITEM_ENDPOINT), str(item_id)),
             headers=self._headers,
             json={"user_id": self.user_id, "origin": None},
             proxies=self.proxies,
             timeout=self.timeout,
         )
         if response.status_code == HTTPStatus.OK:
             return response.json()
         else:
             raise TgtgAPIError(response.status_code, response.content)
 
     def set_favorite(self, item_id, is_favorite):
         self.login()
-        response = requests.post(
+        response = self.session.post(
             urljoin(self._get_url(API_ITEM_ENDPOINT), f"{item_id}/setFavorite"),
             headers=self._headers,
             json={"is_favorite": is_favorite},
             proxies=self.proxies,
             timeout=self.timeout,
         )
         if response.status_code != HTTPStatus.OK:
@@ -254,15 +257,15 @@
         password,
         name,
         country_id="GB",
         device_type="ANDROID",
         newsletter_opt_in=False,
         push_notification_opt_in=True,
     ):
-        response = requests.post(
+        response = self.session.post(
             self._get_url(SIGNUP_BY_EMAIL_ENDPOINT),
             headers=self._headers,
             json={
                 "country_id": country_id,
                 "device_type": device_type,
                 "email": email,
                 "name": name,
```

### Comparing `tgtg-0.8.0/setup.py` & `tgtg-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests==2.26.0']
 
 setup_kwargs = {
     'name': 'tgtg',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Unoffical python client for TooGoodToGo API',
     'long_description': '[![Actions Status](https://github.com/ahivert/tgtg-python/workflows/CI/badge.svg)](https://github.com/ahivert/tgtg-python/actions)\n[![codecov](https://codecov.io/gh/ahivert/tgtg-python/branch/master/graph/badge.svg)](https://codecov.io/gh/ahivert/tgtg-python)\n[![PyPI version](https://img.shields.io/pypi/v/tgtg?color=blue)](https://pypi.org/project/tgtg/)\n\n# tgtg-python\n\nPython client that help you to talk with [TooGoodToGo](https://toogoodtogo.com) API.\n\nPython version: 3.6, 3.7, 3.8, 3.9\n\nHandle:\n- login (`/api/auth/v3/authByEmail`)\n- list stores (`/api/item/`)\n- get a store (`/api/item/:id`)\n- set favorite (`/api/item/:id/setFavorite`)\n- create an account (`auth/v2/signUpByEmail`)\n\nUsed by:\n- https://tgtg-notifier.com\n\n## Install\n\n```\npip install tgtg\n```\n\n## Use it\n\n### Retrieve tokens\n\nBuild the client with your email\n\n```python\nfrom tgtg import TgtgClient\n\nclient = TgtgClient(email="<your_email>")\nclient.get_credentials()\n```\n\nYou should receive an email from tgtg. \nThe will wait until you validate the login by clicking the link inside the email.\n\nOnce you clicked the link in the email, the client will print you tokens\n\n```python\n{\n    \'access_token\': \'<your_access_token>\',\n    \'refresh_token\': \'<your_refresh_token>\',\n    \'user_id\': \'<your_user_id>\',\n}\n```\n\n\n\n### Build the client from tokens\n\n```python\nfrom tgtg import TgtgClient\n\nclient = TgtgClient(access_token="<access_token>", refresh_token="<refresh_token>", user_id="<user_id>")\n\n```\n\n### Get items\n\n```python\n# You can then get some items, by default it will *only* get your favorites\nclient.get_items()\n\n# To get items (not only your favorites) you need to provide location informations\nclient.get_items(\n    favorites_only=False,\n    latitude=48.126,\n    longitude=-1.723,\n    radius=10,\n)\n```\n\n<details>\n    <summary>Example response</summary>\n\n```python\n[\n    {\n        "item": {\n            "item_id": "64346",\n            "price": {"code": "EUR", "minor_units": 499, "decimals": 2},\n            "sales_taxes": [],\n            "tax_amount": {"code": "EUR", "minor_units": 0, "decimals": 2},\n            "price_excluding_taxes": {"code": "EUR", "minor_units": 499, "decimals": 2},\n            "price_including_taxes": {"code": "EUR", "minor_units": 499, "decimals": 2},\n            "value_excluding_taxes": {\n                "code": "EUR",\n                "minor_units": 1500,\n                "decimals": 2,\n            },\n            "value_including_taxes": {\n                "code": "EUR",\n                "minor_units": 1500,\n                "decimals": 2,\n            },\n            "taxation_policy": "PRICE_INCLUDES_TAXES",\n            "show_sales_taxes": False,\n            "value": {"code": "EUR", "minor_units": 1500, "decimals": 2},\n            "cover_picture": {\n                "picture_id": "110628",\n                "current_url": "https://images.tgtg.ninja/item/cover/2b69cbdd-43d3-4ade-bd51-50e338260859.jpg",\n            },\n            "logo_picture": {\n                "picture_id": "110618",\n                "current_url": "https://images.tgtg.ninja/store/fb893813-a775-4dec-ac7b-d4a7dd326fa8.png",\n            },\n            "name": "",\n            "description": "Salva comida en Ecofamily Bufé y tu pack podrá contener: comidas caseras.",\n            "can_user_supply_packaging": False,\n            "packaging_option": "MUST_BRING_BAG",\n            "collection_info": "",\n            "diet_categories": [],\n            "item_category": "MEAL",\n            "badges": [\n                {\n                    "badge_type": "SERVICE_RATING_SCORE",\n                    "rating_group": "LIKED",\n                    "percentage": 93,\n                    "user_count": 178,\n                    "month_count": 5,\n                }\n            ],\n            "favorite_count": 0,\n            "buffet": False,\n        },\n        "store": {\n            "store_id": "59949s",\n            "store_name": "Ecofamily Bufé - Centro",\n            "branch": "",\n            "description": "",\n            "tax_identifier": "",\n            "website": "",\n            "store_location": {\n                "address": {\n                    "country": {"iso_code": "ES", "name": "Spain"},\n                    "address_line": "Av. de los Piconeros, S/N, 14001 Córdoba, España",\n                    "city": "",\n                    "postal_code": "",\n                },\n                "location": {"longitude": -4.776045, "latitude": 37.894249},\n            },\n            "logo_picture": {\n                "picture_id": "110618",\n                "current_url": "https://images.tgtg.ninja/store/fb893813-a775-4dec-ac7b-d4a7dd326fa8.png",\n            },\n            "store_time_zone": "Europe/Madrid",\n            "hidden": False,\n            "favorite_count": 0,\n            "we_care": False,\n        },\n        "display_name": "Ecofamily Bufé - Centro",\n        "pickup_location": {\n            "address": {\n                "country": {"iso_code": "ES", "name": "Spain"},\n                "address_line": "Av. de los Piconeros, S/N, 14001 Córdoba, España",\n                "city": "",\n                "postal_code": "",\n            },\n            "location": {"longitude": -4.776045, "latitude": 37.894249},\n        },\n        "items_available": 0,\n        "distance": 4241.995584076078,\n        "favorite": True,\n        "in_sales_window": False,\n        "new_item": False,\n    },\n]\n```\n</details>\n\n### Get an item\n*(Using item_id from get_items response)*\n```python\nclient.get_item(item_id=64346)\n```\n\n<details>\n<summary>Example response</summary>\n\n```python\n{\n    "item": {\n        "item_id": "64346",\n        "price": {"code": "EUR", "minor_units": 499, "decimals": 2},\n        "sales_taxes": [],\n        "tax_amount": {"code": "EUR", "minor_units": 0, "decimals": 2},\n        "price_excluding_taxes": {"code": "EUR", "minor_units": 499, "decimals": 2},\n        "price_including_taxes": {"code": "EUR", "minor_units": 499, "decimals": 2},\n        "value_excluding_taxes": {"code": "EUR", "minor_units": 1500, "decimals": 2},\n        "value_including_taxes": {"code": "EUR", "minor_units": 1500, "decimals": 2},\n        "taxation_policy": "PRICE_INCLUDES_TAXES",\n        "show_sales_taxes": False,\n        "value": {"code": "EUR", "minor_units": 1500, "decimals": 2},\n        "cover_picture": {\n            "picture_id": "110628",\n            "current_url": "https://images.tgtg.ninja/item/cover/2b69cbdd-43d3-4ade-bd51-50e338260859.jpg",\n        },\n        "logo_picture": {\n            "picture_id": "110618",\n            "current_url": "https://images.tgtg.ninja/store/fb893813-a775-4dec-ac7b-d4a7dd326fa8.png",\n        },\n        "name": "",\n        "description": "Salva comida en Ecofamily Buf\\xc3\\xa9 y tu pack podr\\xc3\\xa1 contener: comidas caseras.",\n        "can_user_supply_packaging": False,\n        "packaging_option": "MUST_BRING_BAG",\n        "collection_info": "",\n        "diet_categories": [],\n        "item_category": "MEAL",\n        "badges": [\n            {\n                "badge_type": "SERVICE_RATING_SCORE",\n                "rating_group": "LIKED",\n                "percentage": 93,\n                "user_count": 178,\n                "month_count": 5,\n            }\n        ],\n        "favorite_count": 0,\n        "buffet": False,\n    },\n    "store": {\n        "store_id": "59949s",\n        "store_name": "Ecofamily Buf\\xc3\\xa9 - Centro",\n        "branch": "",\n        "description": "",\n        "tax_identifier": "",\n        "website": "",\n        "store_location": {\n            "address": {\n                "country": {"iso_code": "ES", "name": "Spain"},\n                "address_line": "Av. de los Piconeros, S/N, 14001 C\\xc3\\xb3rdoba, Espa\\xc3\\xb1a",\n                "city": "",\n                "postal_code": "",\n            },\n            "location": {"longitude": -4.776045, "latitude": 37.894249},\n        },\n        "logo_picture": {\n            "picture_id": "110618",\n            "current_url": "https://images.tgtg.ninja/store/fb893813-a775-4dec-ac7b-d4a7dd326fa8.png",\n        },\n        "store_time_zone": "Europe/Madrid",\n        "hidden": False,\n        "favorite_count": 0,\n        "items": [\n            {\n                "item": {\n                    "item_id": "64346",\n                    "price": {"code": "EUR", "minor_units": 499, "decimals": 2},\n                    "sales_taxes": [],\n                    "tax_amount": {"code": "EUR", "minor_units": 0, "decimals": 2},\n                    "price_excluding_taxes": {\n                        "code": "EUR",\n                        "minor_units": 499,\n                        "decimals": 2,\n                    },\n                    "price_including_taxes": {\n                        "code": "EUR",\n                        "minor_units": 499,\n                        "decimals": 2,\n                    },\n                    "value_excluding_taxes": {\n                        "code": "EUR",\n                        "minor_units": 1500,\n                        "decimals": 2,\n                    },\n                    "value_including_taxes": {\n                        "code": "EUR",\n                        "minor_units": 1500,\n                        "decimals": 2,\n                    },\n                    "taxation_policy": "PRICE_INCLUDES_TAXES",\n                    "show_sales_taxes": False,\n                    "value": {"code": "EUR", "minor_units": 1500, "decimals": 2},\n                    "cover_picture": {\n                        "picture_id": "110628",\n                        "current_url": "https://images.tgtg.ninja/item/cover/2b69cbdd-43d3-4ade-bd51-50e338260859.jpg",\n                    },\n                    "logo_picture": {\n                        "picture_id": "110618",\n                        "current_url": "https://images.tgtg.ninja/store/fb893813-a775-4dec-ac7b-d4a7dd326fa8.png",\n                    },\n                    "name": "",\n                    "description": "Salva comida en Ecofamily Buf\\xc3\\xa9 y tu pack podr\\xc3\\xa1 contener: comidas caseras.",\n                    "can_user_supply_packaging": False,\n                    "packaging_option": "MUST_BRING_BAG",\n                    "collection_info": "",\n                    "diet_categories": [],\n                    "item_category": "MEAL",\n                    "badges": [\n                        {\n                            "badge_type": "SERVICE_RATING_SCORE",\n                            "rating_group": "LIKED",\n                            "percentage": 93,\n                            "user_count": 178,\n                            "month_count": 5,\n                        }\n                    ],\n                    "favorite_count": 0,\n                    "buffet": False,\n                },\n                "display_name": "Ecofamily Buf\\xc3\\xa9 - Centro",\n                "pickup_location": {\n                    "address": {\n                        "country": {"iso_code": "ES", "name": "Spain"},\n                        "address_line": "Av. de los Piconeros, S/N, 14001 C\\xc3\\xb3rdoba, Espa\\xc3\\xb1a",\n                        "city": "",\n                        "postal_code": "",\n                    },\n                    "location": {"longitude": -4.776045, "latitude": 37.894249},\n                },\n                "items_available": 0,\n                "distance": 0.0,\n                "favorite": True,\n                "in_sales_window": False,\n                "new_item": False,\n            }\n        ],\n        "milestones": [\n            {"type": "MEALS_SAVED", "value": "500"},\n            {"type": "MONTHS_ON_PLATFORM", "value": "6"},\n        ],\n        "we_care": False,\n    },\n    "display_name": "Ecofamily Buf\\xc3\\xa9 - Centro",\n    "pickup_location": {\n        "address": {\n            "country": {"iso_code": "ES", "name": "Spain"},\n            "address_line": "Av. de los Piconeros, S/N, 14001 C\\xc3\\xb3rdoba, Espa\\xc3\\xb1a",\n            "city": "",\n            "postal_code": "",\n        },\n        "location": {"longitude": -4.776045, "latitude": 37.894249},\n    },\n    "items_available": 0,\n    "distance": 0.0,\n    "favorite": True,\n    "in_sales_window": False,\n    "new_item": False,\n}\n\n```\n\n</details>\n\n### Set favorite\n*(Using item_id from get_items response)*\n\n```python\n# add favorite\nclient.set_favorite(item_id=64346, is_favorite=True)\n\n# remove favorite\nclient.set_favorite(item_id=64346, is_favorite=False)\n```\n\n### Create an account\n\n```python\nfrom tgtg import TgtgClient\n\nclient = TgtgClient(email="test@test.com", password="password", name="name")\n\n# client is now ready to be used\n```\n\n## Developers\n\nThis project uses poetry so you will need to install poetry locally to use following\ncommands.\n```\npip install poetry --user\npoetry install\n```\n\nThis project uses [pre-commit](https://pre-commit.com/) to format/check all the\ncode before each commit automatically.\n```\npip install pre-commit --user\npre-commit install\n```\n\nRun this command to run all tests:\n```\nmake test\n```\n',
     'author': 'Anthony Hivert',
     'author_email': 'anthony.hivert@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/ahivert/tgtg-python',
```

### Comparing `tgtg-0.8.0/PKG-INFO` & `tgtg-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgtg
-Version: 0.8.0
+Version: 0.9.0
 Summary: Unoffical python client for TooGoodToGo API
 Home-page: https://github.com/ahivert/tgtg-python
 Author: Anthony Hivert
 Author-email: anthony.hivert@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

