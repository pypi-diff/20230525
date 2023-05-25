# Comparing `tmp/meowerbot-2.5.3.tar.gz` & `tmp/meowerbot-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meowerbot-2.5.3.tar", max compression
+gzip compressed data, was "meowerbot-2.5.4.tar", max compression
```

## Comparing `meowerbot-2.5.3.tar` & `meowerbot-2.5.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1093 2023-02-15 00:38:57.652815 meowerbot-2.5.3/LICENSE
--rw-r--r--   0        0        0      154 2023-04-24 21:38:04.560934 meowerbot-2.5.3/MeowerBot/__init__.py
--rw-r--r--   0        0        0      118 2023-04-15 02:04:05.213537 meowerbot-2.5.3/MeowerBot/_Commands.py
--rw-r--r--   0        0        0     1381 2023-04-24 21:38:04.548919 meowerbot-2.5.3/MeowerBot/API.py
--rw-r--r--   0        0        0    13858 2023-05-12 00:23:19.898042 meowerbot-2.5.3/MeowerBot/Bot.py
--rw-r--r--   0        0        0       26 2023-03-25 06:14:31.582953 meowerbot-2.5.3/MeowerBot/cloudlink/__init__.py
--rw-r--r--   0        0        0     8309 2023-03-25 06:14:31.583953 meowerbot-2.5.3/MeowerBot/cloudlink/cloudlink.py
--rw-r--r--   0        0        0      747 2023-04-14 01:23:14.205535 meowerbot-2.5.3/MeowerBot/cog.py
--rw-r--r--   0        0        0     2436 2023-05-12 00:38:58.514877 meowerbot-2.5.3/MeowerBot/command.py
--rw-r--r--   0        0        0     1507 2023-04-15 00:22:16.273775 meowerbot-2.5.3/MeowerBot/context.py
--rw-r--r--   0        0        0      566 2023-05-12 00:40:21.284157 meowerbot-2.5.3/pyproject.toml
--rw-r--r--   0        0        0      244 2023-04-14 22:42:08.188135 meowerbot-2.5.3/README.md
--rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 meowerbot-2.5.3/setup.py
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 meowerbot-2.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-02-15 00:38:57.652815 meowerbot-2.5.4/LICENSE
+-rw-r--r--   0        0        0      191 2023-05-25 00:29:18.440299 meowerbot-2.5.4/MeowerBot/__init__.py
+-rw-r--r--   0        0        0      118 2023-04-15 02:04:05.213537 meowerbot-2.5.4/MeowerBot/_Commands.py
+-rw-r--r--   0        0        0     1381 2023-05-24 23:08:36.965919 meowerbot-2.5.4/MeowerBot/API.py
+-rw-r--r--   0        0        0    14218 2023-05-25 00:29:18.437296 meowerbot-2.5.4/MeowerBot/Bot.py
+-rw-r--r--   0        0        0       26 2023-03-25 06:14:31.582953 meowerbot-2.5.4/MeowerBot/cloudlink/__init__.py
+-rw-r--r--   0        0        0     8309 2023-03-25 06:14:31.583953 meowerbot-2.5.4/MeowerBot/cloudlink/cloudlink.py
+-rw-r--r--   0        0        0      747 2023-04-14 01:23:14.205535 meowerbot-2.5.4/MeowerBot/cog.py
+-rw-r--r--   0        0        0     2443 2023-05-25 00:29:18.441297 meowerbot-2.5.4/MeowerBot/command.py
+-rw-r--r--   0        0        0     1507 2023-04-15 00:22:16.273775 meowerbot-2.5.4/MeowerBot/context.py
+-rw-r--r--   0        0        0      639 2023-05-25 00:32:10.714177 meowerbot-2.5.4/pyproject.toml
+-rw-r--r--   0        0        0      244 2023-04-14 22:42:08.188135 meowerbot-2.5.4/README.md
+-rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 meowerbot-2.5.4/setup.py
+-rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 meowerbot-2.5.4/PKG-INFO
```

### Comparing `meowerbot-2.5.3/LICENSE` & `meowerbot-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.3/MeowerBot/API.py` & `meowerbot-2.5.4/MeowerBot/API.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.3/MeowerBot/Bot.py` & `meowerbot-2.5.4/MeowerBot/Bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,35 @@
 import time
 import logging
 
 from .API import MeowerAPI
 
 from websocket._exceptions import WebSocketConnectionClosedException, WebSocketException
 
+import sys
+
+if sys.version_info >= (3, 11):
+    from enum import StrEnum
+else:
+    from backports.strenum import StrEnum
+
+
+class cbids(StrEnum):
+        error = "error"
+        __raw__ = "__raw__"
+        login = "login"
+        close = "close"
+        statuscode = "statuscode"
+        ulist = "ulist"
+        message = "message"
+        raw_message = "raw_message"
+        chat_list = "chat_list"
+        direct = "direct"
+
+
 
 class Bot:
     """
     A class that holds all of the networking for a meower bot to function and run
 
     """
     __bridges__ = [
@@ -85,14 +106,16 @@
         self._t_ping_thread = threading.Thread(target=self._t_ping, daemon=True)  # (:
         self.logger = logging.getLogger("MeowerBot")
         self.bad_exit = False
         self.server = None
 
         self.cogs = {}
 
+
+
     def run_cb(self, cbid, args=(), kwargs=None):  # cq: ignore
         if cbid not in self.callbacks:
             return  # ignore
 
         if not kwargs:
             kwargs = {}
         
@@ -109,14 +132,16 @@
                     *args, **kwargs
                 )  # multi callback per id is supported (unlike cloudlink 0.1.7.3 LOL)
             except Exception as e:  # cq ignore
 
                 self.logger.error(traceback.format_exc())
                 self.run_cb("error", args=(e,))
 
+
+
     def __handle_error__(self, e):
         self.run_cb("error", args=(e,))
         if type(e) == WebSocketConnectionClosedException and self.autoreload:
             self.__handle_close__()
             return
 
 
@@ -181,69 +206,70 @@
         for cmd in self.cogs[cogname].get_info().values():
             del self.commands[cmd.name]
         del self.cogs[cogname]
 
     def _handle_status(self, status, listener):
         if status == "I:112 | Trusted Access enabled":
             return
+
         if self.logger_in:
             self.logger_in = False
-            if not status == "I:100 | OK":
+
+            if status != "I:100 | OK":
                 raise RuntimeError("CloudLink Trust Failed")
 
-            self.wss.sendPacket(
-                {
-                    "cmd": "direct",
-                    "val": {
-                        "cmd": "authpswd",
-                        "val": {"username": self.username, "pswd": self._password},
-                    },
-                    "listener": "__meowerbot__login",
-                }
-            )
+            auth_packet = {
+                "cmd": "direct",
+                "val": {
+                    "cmd": "authpswd",
+                    "val": {"username": self.username, "pswd": self._password},
+                },
+                "listener": "__meowerbot__login",
+            }
+            self.wss.sendPacket(auth_packet)
 
         elif listener == "__meowerbot__login":
             if status == "E:104 | Internal":
                 requests.post(
                     "https://webhooks.meower.org/post/home",
                     json={
                         "post": "ERROR: MeowerBot.py Webhooks Logging\n\n Account Softlocked.",
-                         "username": self.username,
+                        "username": self.username,
                     },
                 )
                 print("CRITICAL ERROR! ACCOUNT SOFTLOCKED!!!!.", file=sys.__stdout__)
                 self.bad_exit = True
                 self.wss.stop()
                 return
 
-            if not status == "I:100 | OK":
+            if status != "I:100 | OK":
                 raise RuntimeError("Password Or Username Is Incorrect")
 
             time.sleep(0.5)
             self.run_cb("login", args=(), kwargs={})
 
         elif listener == "__meowerbot__send_message":
             if status == "I:100 | OK":
                 self.autoreload_time = self.autoreload_original
-                return  # This is just checking if a post went OK
-            #autoreload time should reset if 
-
+                return
 
             raise RuntimeError("Post Failed to send")
-        
 
-    def callback(self, callback, cbid=None):
-        """Connects a callback ID to a callback"""
+    def callback(self, callback, cbid: cbids |  None |  str =None):
+        """Connects a callback ID to a callback
+        """
         if cbid is None:
             cbid = callback.__name__
 
         if cbid not in self.callbacks:
             self.callbacks[cbid] = []
         self.callbacks[cbid].append(callback)
 
+    
+
     def __handle_close__(self, *args, **kwargs):
         if self.autoreload:
             self.autoreload = False #to stop race condisons 
             self.logger_in = True
             self.autoreload_time *= 1.2 
             
             
@@ -259,15 +285,15 @@
     def handle_bridges(self, packet):
         if packet["val"]["u"] in self.__bridges__ and ": " in packet["val"]["p"]:
                 split = packet["val"]["p"].split(": ", 1)
                 packet["val"]["p"] = split[1]
                 packet["val"]["u"] = split[0]
         
         if packet["val"]["p"].startswith(self.prefix+"#0000"):
-            packet["val"]["p"] = packet["val"]["p"].replace("#0000", self.prefix)
+            packet["val"]["p"] = packet["val"]["p"].replace("#0000", "")
         
         return packet
 
     def __handle_packet__(self, packet):
         if packet["cmd"] == "statuscode":
 
             self._handle_status(packet["val"], packet.get("listener", None))
```

### Comparing `meowerbot-2.5.3/MeowerBot/cloudlink/cloudlink.py` & `meowerbot-2.5.4/MeowerBot/cloudlink/cloudlink.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.3/MeowerBot/cog.py` & `meowerbot-2.5.4/MeowerBot/cog.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.3/MeowerBot/command.py` & `meowerbot-2.5.4/MeowerBot/command.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import warnings
 import inspect
 
+from logging import getLogger
+
+logger = getLogger("MeowerBot")
+
 
 class AppCommand:
     connected = None
 
     def __init__(self, func, name=None, args=0):
         if name is None:
             name = func.__name__
@@ -22,41 +26,40 @@
 
     def register_class(self, con):
         self.connected = con
 
         for subcommand in self.subcommands.values():
             subcommand.register_class(con)
 
+
     def subcommand(self, name=None, args=0):
         def inner(func):
 
             cmd = AppCommand(func, name=name, args=args)
             cmd.register_class(self.connected)
 
             self.subcommands.update(cmd.info())
 
 
             return func #dont want mb to register this as a root command
         return inner
     
 
     def run_cmd(self, ctx, *args):
-        print(
-            f"Running command {self.name} with args {args} and ctx {ctx} and connected {self.connected}"
-
-        )
         
         try:
             self.subcommands[args[0]]["command"].run_cmd(ctx, *args[1:])
             return
         except KeyError:
-            print(f"KeyError: {args}")
-            print(f"Subcommands: {self.subcommands}")
+            #print(f"KeyError: {args}")
+            #print(f"Subcommands: {self.subcommands}")
+            logger.debug(f"Cant find subcommand {args[0]}")
+
         except IndexError:
-            print(f"IndexError: {args}")
+            logger.debug(f"IndexError: {args}")
         
         if not self.args == 0:
             args = args[: self.args]
 
         if self.connected is None:
             self.func(ctx, *args)
         else:
```

### Comparing `meowerbot-2.5.3/MeowerBot/context.py` & `meowerbot-2.5.4/MeowerBot/context.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.3/pyproject.toml` & `meowerbot-2.5.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MeowerBot"
-version = "2.5.3"
+version = "2.5.4"
 description = "A meower bot lib for py"
 authors = ["showierdata9978 <68120127+showierdata9978@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "MeowerBot"}
 ]
@@ -15,10 +15,13 @@
 python = "^3.8"
 requests = "^2.28.0"
 websocket-client = "*"
 
 [tool.poetry.dev-dependencies]
 black = "^22.6.0"
 
+[tool.poetry.group.extras.dependencies]
+backports-strenum = "^1.2.4"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `meowerbot-2.5.3/setup.py` & `meowerbot-2.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.0,<3.0.0', 'websocket-client']
 
 setup_kwargs = {
     'name': 'meowerbot',
-    'version': '2.5.3',
+    'version': '2.5.4',
     'description': 'A meower bot lib for py',
     'long_description': '# MeowerBot.py\n\nA bot lib for Meower\n\n\n## License\n\nsee [LICENSE](./LICENSE)\n\n\n## docs\n\nThe Docs are located [here](https://meowerbot-py.showierdata.tech/)\n\n\n## Quick Example\n\nlook at the [tests directory](./tests) for examples ',
     'author': 'showierdata9978',
     'author_email': '68120127+showierdata9978@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/MeowerBots/MeowerBot.py',
```

### Comparing `meowerbot-2.5.3/PKG-INFO` & `meowerbot-2.5.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meowerbot
-Version: 2.5.3
+Version: 2.5.4
 Summary: A meower bot lib for py
 Home-page: https://github.com/MeowerBots/MeowerBot.py
 License: MIT
 Author: showierdata9978
 Author-email: 68120127+showierdata9978@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

