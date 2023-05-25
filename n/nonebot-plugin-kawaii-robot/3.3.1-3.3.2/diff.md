# Comparing `tmp/nonebot_plugin_kawaii_robot-3.3.1.tar.gz` & `tmp/nonebot_plugin_kawaii_robot-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_kawaii_robot-3.3.1.tar", last modified: Sat Feb  4 19:06:06 2023, max compression
+gzip compressed data, was "nonebot_plugin_kawaii_robot-3.3.2.tar", last modified: Thu May 25 05:08:22 2023, max compression
```

## Comparing `nonebot_plugin_kawaii_robot-3.3.1.tar` & `nonebot_plugin_kawaii_robot-3.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-02-04 19:06:06.459922 nonebot_plugin_kawaii_robot-3.3.1/
--rw-rw-rw-   0        0        0    35184 2022-08-21 05:19:27.000000 nonebot_plugin_kawaii_robot-3.3.1/LICENSE
--rw-rw-rw-   0        0        0       63 2022-07-08 21:05:45.000000 nonebot_plugin_kawaii_robot-3.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0      334 2023-02-04 19:06:06.459422 nonebot_plugin_kawaii_robot-3.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     3285 2022-12-24 11:13:16.000000 nonebot_plugin_kawaii_robot-3.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-04 19:06:06.446911 nonebot_plugin_kawaii_robot-3.3.1/nonebot_plugin_kawaii_robot/
--rw-rw-rw-   0        0        0     5168 2023-02-04 19:02:17.000000 nonebot_plugin_kawaii_robot-3.3.1/nonebot_plugin_kawaii_robot/__init__.py
--rw-rw-rw-   0        0        0      327 2023-02-04 18:57:46.000000 nonebot_plugin_kawaii_robot-3.3.1/nonebot_plugin_kawaii_robot/config.py
-drwxrwxrwx   0        0        0        0 2023-02-04 19:06:06.457921 nonebot_plugin_kawaii_robot-3.3.1/nonebot_plugin_kawaii_robot/resource/
--rw-rw-rw-   0        0        0    81633 2022-08-21 05:19:27.000000 nonebot_plugin_kawaii_robot-3.3.1/nonebot_plugin_kawaii_robot/resource/data.json
--rw-rw-rw-   0        0        0    12541 2022-08-21 05:19:27.000000 nonebot_plugin_kawaii_robot-3.3.1/nonebot_plugin_kawaii_robot/resource/leaf.json
--rw-rw-rw-   0        0        0     3790 2022-12-24 11:08:54.000000 nonebot_plugin_kawaii_robot-3.3.1/nonebot_plugin_kawaii_robot/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-04 19:06:06.452917 nonebot_plugin_kawaii_robot-3.3.1/nonebot_plugin_kawaii_robot.egg-info/
--rw-rw-rw-   0        0        0      334 2023-02-04 19:06:06.000000 nonebot_plugin_kawaii_robot-3.3.1/nonebot_plugin_kawaii_robot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      501 2023-02-04 19:06:06.000000 nonebot_plugin_kawaii_robot-3.3.1/nonebot_plugin_kawaii_robot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-04 19:06:06.000000 nonebot_plugin_kawaii_robot-3.3.1/nonebot_plugin_kawaii_robot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-02-04 19:06:06.000000 nonebot_plugin_kawaii_robot-3.3.1/nonebot_plugin_kawaii_robot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-02-04 19:06:06.000000 nonebot_plugin_kawaii_robot-3.3.1/nonebot_plugin_kawaii_robot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-04 19:06:06.459922 nonebot_plugin_kawaii_robot-3.3.1/setup.cfg
--rw-rw-rw-   0        0        0      610 2023-02-04 19:03:15.000000 nonebot_plugin_kawaii_robot-3.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 05:08:22.254099 nonebot_plugin_kawaii_robot-3.3.2/
+-rw-rw-rw-   0        0        0    35184 2022-08-21 05:19:27.000000 nonebot_plugin_kawaii_robot-3.3.2/LICENSE
+-rw-rw-rw-   0        0        0       63 2022-07-08 21:05:45.000000 nonebot_plugin_kawaii_robot-3.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      334 2023-05-25 05:08:22.253598 nonebot_plugin_kawaii_robot-3.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3285 2022-12-24 11:13:16.000000 nonebot_plugin_kawaii_robot-3.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 05:08:22.235082 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot/
+-rw-rw-rw-   0        0        0     5220 2023-05-25 04:47:57.000000 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot/__init__.py
+-rw-rw-rw-   0        0        0      912 2023-05-25 04:43:40.000000 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot/config.py
+drwxrwxrwx   0        0        0        0 2023-05-25 05:08:22.250596 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot/resource/
+-rw-rw-rw-   0        0        0    81633 2022-08-21 05:19:27.000000 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot/resource/data.json
+-rw-rw-rw-   0        0        0    12541 2022-08-21 05:19:27.000000 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot/resource/leaf.json
+-rw-rw-rw-   0        0        0     3944 2023-05-25 04:42:06.000000 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 05:08:22.244090 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot.egg-info/
+-rw-rw-rw-   0        0        0      334 2023-05-25 05:08:22.000000 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2023-05-25 05:08:22.000000 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 05:08:22.000000 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-25 05:08:22.000000 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-05-25 05:08:22.000000 nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 05:08:22.254599 nonebot_plugin_kawaii_robot-3.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      610 2023-05-25 05:08:17.000000 nonebot_plugin_kawaii_robot-3.3.2/setup.py
```

### Comparing `nonebot_plugin_kawaii_robot-3.3.1/LICENSE` & `nonebot_plugin_kawaii_robot-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_robot-3.3.1/README.md` & `nonebot_plugin_kawaii_robot-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_robot-3.3.1/nonebot_plugin_kawaii_robot/__init__.py` & `nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 import re
 import random
 
 from .utils import (
     MyThesaurus,
     LeafThesaurus,
     AnimeThesaurus,
-    get_chat_result,
-    hello__bot,
+    keyword_search,
     hello__reply,
     poke__reply,
     unknow_reply,
     interrupt_msg,
     messagePreprocess
     )
 
@@ -37,14 +36,23 @@
 poke_rand = leaf.leaf_poke_rand
 
 repeater_limit = leaf.leaf_repeater_limit
 interrupt = leaf.leaf_interrupt
 
 ignore = leaf.leaf_ignore
 
+match_pattern = leaf.leaf_match_pattern
+
+if match_pattern == 0:
+    get_chat_result = lambda resource,key:resource.get(key,"")
+else:
+    get_chat_result = keyword_search
+
+at_mod = leaf.leaf_at_mod
+
 # 配置合法检测
 
 if repeater_limit[0] < 2 or repeater_limit[0] > repeater_limit[1]:
     raise Exception('config error: repeater_limit')
 
 # 权限判断
 
@@ -52,64 +60,62 @@
     permission = GROUP
 else:
     permission = None
 
 # 优先级99，条件：艾特bot就触发
 
 if reply_type > -1:
-    talk = on_message(rule = to_me(), permission = permission, priority=99, block=False)
+    talk = on_message(
+        rule = to_me() if at_mod == 0 else None,
+        permission = permission,
+        priority = 99,
+        block = False
+        )
 
     @talk.handle()
     async def _(event: MessageEvent):
         # 获取消息文本
         msg = str(event.get_message())
         # 去掉带中括号的内容(去除cq码)
         msg = re.sub(r"\[.*?\]", "", msg)
 
         # 如果是光艾特bot(没消息返回)，就回复以下内容
         if (not msg) or msg.isspace():
-            await talk.finish(Message(random.choice(hello__reply)))
-
-        # 如果是打招呼的话，就回复以下内容
-        if  msg in hello__bot:
-            await talk.finish(Message(random.choice(hello__reply)))
+            if at_mod == 0:
+                await talk.finish(Message(random.choice(hello__reply)))
 
         # 如果是已配置的忽略项，直接结束事件
         for i in range(len(ignore)):
             if msg.startswith(ignore[i]):
                 await talk.finish()
 
         # 获取用户nickname
         if isinstance(event, GroupMessageEvent):
             nickname = event.sender.card or event.sender.nickname
         else:
             nickname = event.sender.nickname
 
         if len(nickname) > 10:
-            nickname = nickname[:2] + random.choice(["酱","亲","ちゃん","同志","老师"])
+            nickname = nickname[:2] + \
+                random.choice(["酱", "亲", "ちゃん", "同志", "老师"])
 
         # 从个人字典里获取结果
         if result := get_chat_result(MyThesaurus, msg):
             await talk.finish(Message(result))
 
-        result = get_chat_result(MyThesaurus, msg)
-        if result:
-            await talk.finish(Message(result))
-
-
         # 从 LeafThesaurus 里获取结果
-        if result := get_chat_result(LeafThesaurus,msg):
+        if result := get_chat_result(LeafThesaurus, msg):
             await talk.finish(Message(result.replace("name", nickname)))
 
         # 从 AnimeThesaurus 里获取结果
-        if result := get_chat_result(AnimeThesaurus,msg):
+        if result := get_chat_result(AnimeThesaurus, msg):
             await talk.finish(Message(result.replace("你", nickname)))
 
         # 不明白的内容
-        if reply_type == 1:
+        if at_mod == 0 and reply_type == 1:
             await talk.finish(Message(random.choice(unknow_reply)))
 
 # 优先级10，不会向下阻断，条件：戳一戳bot触发
 
 if poke_rand > -1:
     poke_ = on_notice(rule = to_me(), priority=10, block=False)
     @poke_.handle()
```

### Comparing `nonebot_plugin_kawaii_robot-3.3.1/nonebot_plugin_kawaii_robot/resource/data.json` & `nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot/resource/data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_robot-3.3.1/nonebot_plugin_kawaii_robot/resource/leaf.json` & `nonebot_plugin_kawaii_robot-3.3.2/nonebot_plugin_kawaii_robot/resource/leaf.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kawaii_robot-3.3.1/setup.py` & `nonebot_plugin_kawaii_robot-3.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_kawaii_robot',
-version='3.3.1',
+version='3.3.2',
 description='使用Kyomotoi / AnimeThesaurus的nonebot2的回复（文i）插件',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='AGPLv3 License',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_kawaii_robot","nonebot_plugin_kawaii_robot.*"]),
```

