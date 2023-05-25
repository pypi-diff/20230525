# Comparing `tmp/meowerbot-2.5.4.tar.gz` & `tmp/meowerbot-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meowerbot-2.5.4.tar", max compression
+gzip compressed data, was "meowerbot-2.5.5.tar", max compression
```

## Comparing `meowerbot-2.5.4.tar` & `meowerbot-2.5.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1093 2023-02-15 00:38:57.652815 meowerbot-2.5.4/LICENSE
--rw-r--r--   0        0        0      191 2023-05-25 00:29:18.440299 meowerbot-2.5.4/MeowerBot/__init__.py
--rw-r--r--   0        0        0      118 2023-04-15 02:04:05.213537 meowerbot-2.5.4/MeowerBot/_Commands.py
--rw-r--r--   0        0        0     1381 2023-05-24 23:08:36.965919 meowerbot-2.5.4/MeowerBot/API.py
--rw-r--r--   0        0        0    14218 2023-05-25 00:29:18.437296 meowerbot-2.5.4/MeowerBot/Bot.py
--rw-r--r--   0        0        0       26 2023-03-25 06:14:31.582953 meowerbot-2.5.4/MeowerBot/cloudlink/__init__.py
--rw-r--r--   0        0        0     8309 2023-03-25 06:14:31.583953 meowerbot-2.5.4/MeowerBot/cloudlink/cloudlink.py
--rw-r--r--   0        0        0      747 2023-04-14 01:23:14.205535 meowerbot-2.5.4/MeowerBot/cog.py
--rw-r--r--   0        0        0     2443 2023-05-25 00:29:18.441297 meowerbot-2.5.4/MeowerBot/command.py
--rw-r--r--   0        0        0     1507 2023-04-15 00:22:16.273775 meowerbot-2.5.4/MeowerBot/context.py
--rw-r--r--   0        0        0      639 2023-05-25 00:32:10.714177 meowerbot-2.5.4/pyproject.toml
--rw-r--r--   0        0        0      244 2023-04-14 22:42:08.188135 meowerbot-2.5.4/README.md
--rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 meowerbot-2.5.4/setup.py
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 meowerbot-2.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-02-15 00:38:57.652815 meowerbot-2.5.5/LICENSE
+-rw-r--r--   0        0        0      191 2023-05-25 01:57:18.056383 meowerbot-2.5.5/MeowerBot/__init__.py
+-rw-r--r--   0        0        0      118 2023-04-15 02:04:05.213537 meowerbot-2.5.5/MeowerBot/_Commands.py
+-rw-r--r--   0        0        0     1381 2023-05-24 23:08:36.965919 meowerbot-2.5.5/MeowerBot/API.py
+-rw-r--r--   0        0        0    14286 2023-05-25 02:29:49.057081 meowerbot-2.5.5/MeowerBot/Bot.py
+-rw-r--r--   0        0        0       26 2023-03-25 06:14:31.582953 meowerbot-2.5.5/MeowerBot/cloudlink/__init__.py
+-rw-r--r--   0        0        0     8309 2023-03-25 06:14:31.583953 meowerbot-2.5.5/MeowerBot/cloudlink/cloudlink.py
+-rw-r--r--   0        0        0      747 2023-04-14 01:23:14.205535 meowerbot-2.5.5/MeowerBot/cog.py
+-rw-r--r--   0        0        0     2443 2023-05-25 00:29:18.441297 meowerbot-2.5.5/MeowerBot/command.py
+-rw-r--r--   0        0        0     1507 2023-04-15 00:22:16.273775 meowerbot-2.5.5/MeowerBot/context.py
+-rw-r--r--   0        0        0      649 2023-05-25 02:34:23.921191 meowerbot-2.5.5/pyproject.toml
+-rw-r--r--   0        0        0      244 2023-04-14 22:42:08.188135 meowerbot-2.5.5/README.md
+-rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 meowerbot-2.5.5/setup.py
+-rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 meowerbot-2.5.5/PKG-INFO
```

### Comparing `meowerbot-2.5.4/LICENSE` & `meowerbot-2.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.4/MeowerBot/API.py` & `meowerbot-2.5.5/MeowerBot/API.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.4/MeowerBot/Bot.py` & `meowerbot-2.5.5/MeowerBot/Bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import sys
 
 if sys.version_info >= (3, 11):
     from enum import StrEnum
 else:
     from backports.strenum import StrEnum
 
+from typing import Union
 
 class cbids(StrEnum):
         error = "error"
         __raw__ = "__raw__"
         login = "login"
         close = "close"
         statuscode = "statuscode"
@@ -231,14 +232,15 @@
             if status == "E:104 | Internal":
                 requests.post(
                     "https://webhooks.meower.org/post/home",
                     json={
                         "post": "ERROR: MeowerBot.py Webhooks Logging\n\n Account Softlocked.",
                         "username": self.username,
                     },
+                    timeout=5
                 )
                 print("CRITICAL ERROR! ACCOUNT SOFTLOCKED!!!!.", file=sys.__stdout__)
                 self.bad_exit = True
                 self.wss.stop()
                 return
 
             if status != "I:100 | OK":
@@ -250,15 +252,15 @@
         elif listener == "__meowerbot__send_message":
             if status == "I:100 | OK":
                 self.autoreload_time = self.autoreload_original
                 return
 
             raise RuntimeError("Post Failed to send")
 
-    def callback(self, callback, cbid: cbids |  None |  str =None):
+    def callback(self, callback, cbid: Union[Union[cbids,  None], str] =None):
         """Connects a callback ID to a callback
         """
         if cbid is None:
             cbid = callback.__name__
 
         if cbid not in self.callbacks:
             self.callbacks[cbid] = []
```

### Comparing `meowerbot-2.5.4/MeowerBot/cloudlink/cloudlink.py` & `meowerbot-2.5.5/MeowerBot/cloudlink/cloudlink.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.4/MeowerBot/cog.py` & `meowerbot-2.5.5/MeowerBot/cog.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.4/MeowerBot/command.py` & `meowerbot-2.5.5/MeowerBot/command.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.4/MeowerBot/context.py` & `meowerbot-2.5.5/MeowerBot/context.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.4/pyproject.toml` & `meowerbot-2.5.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MeowerBot"
-version = "2.5.4"
+version = "2.5.5"
 description = "A meower bot lib for py"
 authors = ["showierdata9978 <68120127+showierdata9978@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "MeowerBot"}
 ]
@@ -12,16 +12,18 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.28.0"
 websocket-client = "*"
 
-[tool.poetry.dev-dependencies]
-black = "^22.6.0"
 
 [tool.poetry.group.extras.dependencies]
 backports-strenum = "^1.2.4"
 
+
+[tool.poetry.group.dev.dependencies]
+bandit = "^1.7.5"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `meowerbot-2.5.4/setup.py` & `meowerbot-2.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.0,<3.0.0', 'websocket-client']
 
 setup_kwargs = {
     'name': 'meowerbot',
-    'version': '2.5.4',
+    'version': '2.5.5',
     'description': 'A meower bot lib for py',
     'long_description': '# MeowerBot.py\n\nA bot lib for Meower\n\n\n## License\n\nsee [LICENSE](./LICENSE)\n\n\n## docs\n\nThe Docs are located [here](https://meowerbot-py.showierdata.tech/)\n\n\n## Quick Example\n\nlook at the [tests directory](./tests) for examples ',
     'author': 'showierdata9978',
     'author_email': '68120127+showierdata9978@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/MeowerBots/MeowerBot.py',
```

### Comparing `meowerbot-2.5.4/PKG-INFO` & `meowerbot-2.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meowerbot
-Version: 2.5.4
+Version: 2.5.5
 Summary: A meower bot lib for py
 Home-page: https://github.com/MeowerBots/MeowerBot.py
 License: MIT
 Author: showierdata9978
 Author-email: 68120127+showierdata9978@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

