# Comparing `tmp/bovine_process-0.2.0.tar.gz` & `tmp/bovine_process-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine_process-0.2.0.tar", max compression
+gzip compressed data, was "bovine_process-0.2.2.tar", max compression
```

## Comparing `bovine_process-0.2.0.tar` & `bovine_process-0.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1681 2023-05-22 14:17:04.658842 bovine_process-0.2.0/README.md
--rw-r--r--   0        0        0     1664 2023-05-22 14:17:04.658842 bovine_process-0.2.0/bovine_process/__init__.py
--rw-r--r--   0        0        0      770 2023-05-22 14:17:04.658842 bovine_process-0.2.0/bovine_process/add_to_queue.py
--rw-r--r--   0        0        0      809 2023-05-22 14:17:04.658842 bovine_process-0.2.0/bovine_process/incoming/__init__.py
--rw-r--r--   0        0        0      863 2023-05-22 14:17:04.658842 bovine_process-0.2.0/bovine_process/incoming/follow_accept.py
--rw-r--r--   0        0        0      709 2023-05-22 14:17:04.658842 bovine_process-0.2.0/bovine_process/incoming/handle_update.py
--rw-r--r--   0        0        0      847 2023-05-22 14:17:04.658842 bovine_process-0.2.0/bovine_process/incoming/incoming_delete.py
--rw-r--r--   0        0        0      877 2023-05-22 14:17:58.083053 bovine_process-0.2.0/bovine_process/incoming/store_incoming.py
--rw-r--r--   0        0        0     1414 2023-05-22 14:17:04.658842 bovine_process-0.2.0/bovine_process/incoming/test_handle_update.py
--rw-r--r--   0        0        0      983 2023-05-22 14:17:04.662842 bovine_process-0.2.0/bovine_process/incoming/test_store_incoming.py
--rw-r--r--   0        0        0     1604 2023-05-22 14:17:04.662842 bovine_process-0.2.0/bovine_process/incoming/test_undo.py
--rw-r--r--   0        0        0      721 2023-05-22 14:17:04.662842 bovine_process-0.2.0/bovine_process/incoming/undo.py
--rw-r--r--   0        0        0      693 2023-05-22 14:17:04.662842 bovine_process-0.2.0/bovine_process/outgoing/__init__.py
--rw-r--r--   0        0        0      642 2023-05-22 14:17:04.662842 bovine_process-0.2.0/bovine_process/outgoing/accept_follow.py
--rw-r--r--   0        0        0      878 2023-05-22 14:17:04.662842 bovine_process-0.2.0/bovine_process/outgoing/outgoing_delete.py
--rw-r--r--   0        0        0      943 2023-05-22 14:17:04.662842 bovine_process-0.2.0/bovine_process/outgoing/outgoing_update.py
--rw-r--r--   0        0        0      972 2023-05-22 14:17:58.095053 bovine_process-0.2.0/bovine_process/outgoing/store_outgoing.py
--rw-r--r--   0        0        0     1626 2023-05-22 14:17:04.662842 bovine_process-0.2.0/bovine_process/outgoing/test_outgoing_update.py
--rw-r--r--   0        0        0      386 2023-05-22 14:17:04.662842 bovine_process-0.2.0/bovine_process/outgoing/update_id.py
--rw-r--r--   0        0        0     1598 2023-05-22 14:17:04.662842 bovine_process-0.2.0/bovine_process/send_item.py
--rw-r--r--   0        0        0      364 2023-05-22 14:17:04.662842 bovine_process-0.2.0/bovine_process/test_types.py
--rw-r--r--   0        0        0      723 2023-05-22 14:17:04.662842 bovine_process-0.2.0/bovine_process/types.py
--rw-r--r--   0        0        0        0 2023-05-22 14:17:04.662842 bovine_process-0.2.0/bovine_process/utils/__init__.py
--rw-r--r--   0        0        0      741 2023-05-22 14:17:04.662842 bovine_process-0.2.0/bovine_process/utils/by_activity_type.py
--rw-r--r--   0        0        0      844 2023-05-22 14:17:04.662842 bovine_process-0.2.0/bovine_process/utils/processor_list.py
--rw-r--r--   0        0        0     1084 2023-05-22 14:17:04.662842 bovine_process-0.2.0/bovine_process/utils/test_by_activity_type.py
--rw-r--r--   0        0        0      429 2023-03-30 06:22:46.664327 bovine_process-0.2.0/bovine_process/utils/test_processor_list.py
--rw-r--r--   0        0        0      759 2023-05-22 14:17:04.662842 bovine_process-0.2.0/bovine_process/utils/test_update_id.py
--rw-r--r--   0        0        0      481 2023-05-22 14:17:04.662842 bovine_process-0.2.0/bovine_process/utils/update_id.py
--rw-r--r--   0        0        0      939 2023-05-22 14:25:13.884647 bovine_process-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2554 1970-01-01 00:00:00.000000 bovine_process-0.2.0/setup.py
--rw-r--r--   0        0        0     2371 1970-01-01 00:00:00.000000 bovine_process-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1681 2023-05-22 14:17:04.658842 bovine_process-0.2.2/README.md
+-rw-r--r--   0        0        0     1664 2023-05-22 14:17:04.658842 bovine_process-0.2.2/bovine_process/__init__.py
+-rw-r--r--   0        0        0      770 2023-05-22 14:17:04.658842 bovine_process-0.2.2/bovine_process/add_to_queue.py
+-rw-r--r--   0        0        0      809 2023-05-22 14:17:04.658842 bovine_process-0.2.2/bovine_process/incoming/__init__.py
+-rw-r--r--   0        0        0      863 2023-05-22 14:17:04.658842 bovine_process-0.2.2/bovine_process/incoming/follow_accept.py
+-rw-r--r--   0        0        0      709 2023-05-22 14:17:04.658842 bovine_process-0.2.2/bovine_process/incoming/handle_update.py
+-rw-r--r--   0        0        0      847 2023-05-22 14:17:04.658842 bovine_process-0.2.2/bovine_process/incoming/incoming_delete.py
+-rw-r--r--   0        0        0      877 2023-05-25 09:12:33.552414 bovine_process-0.2.2/bovine_process/incoming/store_incoming.py
+-rw-r--r--   0        0        0     1414 2023-05-22 14:17:04.658842 bovine_process-0.2.2/bovine_process/incoming/test_handle_update.py
+-rw-r--r--   0        0        0      983 2023-05-22 14:17:04.662842 bovine_process-0.2.2/bovine_process/incoming/test_store_incoming.py
+-rw-r--r--   0        0        0     1604 2023-05-22 14:17:04.662842 bovine_process-0.2.2/bovine_process/incoming/test_undo.py
+-rw-r--r--   0        0        0      721 2023-05-22 14:17:04.662842 bovine_process-0.2.2/bovine_process/incoming/undo.py
+-rw-r--r--   0        0        0      693 2023-05-22 14:17:04.662842 bovine_process-0.2.2/bovine_process/outgoing/__init__.py
+-rw-r--r--   0        0        0      642 2023-05-22 14:17:04.662842 bovine_process-0.2.2/bovine_process/outgoing/accept_follow.py
+-rw-r--r--   0        0        0      878 2023-05-22 14:17:04.662842 bovine_process-0.2.2/bovine_process/outgoing/outgoing_delete.py
+-rw-r--r--   0        0        0      943 2023-05-22 14:17:04.662842 bovine_process-0.2.2/bovine_process/outgoing/outgoing_update.py
+-rw-r--r--   0        0        0      972 2023-05-25 09:12:33.564414 bovine_process-0.2.2/bovine_process/outgoing/store_outgoing.py
+-rw-r--r--   0        0        0     1626 2023-05-22 14:17:04.662842 bovine_process-0.2.2/bovine_process/outgoing/test_outgoing_update.py
+-rw-r--r--   0        0        0      386 2023-05-22 14:17:04.662842 bovine_process-0.2.2/bovine_process/outgoing/update_id.py
+-rw-r--r--   0        0        0     1598 2023-05-22 14:17:04.662842 bovine_process-0.2.2/bovine_process/send_item.py
+-rw-r--r--   0        0        0      364 2023-05-22 14:17:04.662842 bovine_process-0.2.2/bovine_process/test_types.py
+-rw-r--r--   0        0        0      723 2023-05-22 14:17:04.662842 bovine_process-0.2.2/bovine_process/types.py
+-rw-r--r--   0        0        0        0 2023-05-22 14:17:04.662842 bovine_process-0.2.2/bovine_process/utils/__init__.py
+-rw-r--r--   0        0        0      741 2023-05-22 14:17:04.662842 bovine_process-0.2.2/bovine_process/utils/by_activity_type.py
+-rw-r--r--   0        0        0      844 2023-05-22 14:17:04.662842 bovine_process-0.2.2/bovine_process/utils/processor_list.py
+-rw-r--r--   0        0        0     1084 2023-05-22 14:17:04.662842 bovine_process-0.2.2/bovine_process/utils/test_by_activity_type.py
+-rw-r--r--   0        0        0      429 2023-03-30 06:22:46.664327 bovine_process-0.2.2/bovine_process/utils/test_processor_list.py
+-rw-r--r--   0        0        0      759 2023-05-22 14:17:04.662842 bovine_process-0.2.2/bovine_process/utils/test_update_id.py
+-rw-r--r--   0        0        0      481 2023-05-22 14:17:04.662842 bovine_process-0.2.2/bovine_process/utils/update_id.py
+-rw-r--r--   0        0        0      939 2023-05-25 18:44:02.806690 bovine_process-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2554 1970-01-01 00:00:00.000000 bovine_process-0.2.2/setup.py
+-rw-r--r--   0        0        0     2371 1970-01-01 00:00:00.000000 bovine_process-0.2.2/PKG-INFO
```

### Comparing `bovine_process-0.2.0/README.md` & `bovine_process-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/bovine_process/__init__.py` & `bovine_process-0.2.2/bovine_process/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/bovine_process/add_to_queue.py` & `bovine_process-0.2.2/bovine_process/add_to_queue.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/bovine_process/incoming/__init__.py` & `bovine_process-0.2.2/bovine_process/incoming/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/bovine_process/incoming/follow_accept.py` & `bovine_process-0.2.2/bovine_process/incoming/follow_accept.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/bovine_process/incoming/handle_update.py` & `bovine_process-0.2.2/bovine_process/incoming/handle_update.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/bovine_process/incoming/incoming_delete.py` & `bovine_process-0.2.2/bovine_process/incoming/incoming_delete.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/bovine_process/incoming/store_incoming.py` & `bovine_process-0.2.2/bovine_process/incoming/store_incoming.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/bovine_process/incoming/test_handle_update.py` & `bovine_process-0.2.2/bovine_process/incoming/test_handle_update.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/bovine_process/incoming/test_store_incoming.py` & `bovine_process-0.2.2/bovine_process/incoming/test_store_incoming.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/bovine_process/incoming/test_undo.py` & `bovine_process-0.2.2/bovine_process/incoming/test_undo.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/bovine_process/incoming/undo.py` & `bovine_process-0.2.2/bovine_process/incoming/undo.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/bovine_process/outgoing/__init__.py` & `bovine_process-0.2.2/bovine_process/outgoing/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/bovine_process/outgoing/accept_follow.py` & `bovine_process-0.2.2/bovine_process/outgoing/accept_follow.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/bovine_process/outgoing/outgoing_delete.py` & `bovine_process-0.2.2/bovine_process/outgoing/outgoing_delete.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/bovine_process/outgoing/outgoing_update.py` & `bovine_process-0.2.2/bovine_process/outgoing/outgoing_update.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/bovine_process/outgoing/store_outgoing.py` & `bovine_process-0.2.2/bovine_process/outgoing/store_outgoing.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/bovine_process/outgoing/test_outgoing_update.py` & `bovine_process-0.2.2/bovine_process/outgoing/test_outgoing_update.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/bovine_process/send_item.py` & `bovine_process-0.2.2/bovine_process/send_item.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/bovine_process/types.py` & `bovine_process-0.2.2/bovine_process/types.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/bovine_process/utils/by_activity_type.py` & `bovine_process-0.2.2/bovine_process/utils/by_activity_type.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/bovine_process/utils/processor_list.py` & `bovine_process-0.2.2/bovine_process/utils/processor_list.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/bovine_process/utils/test_by_activity_type.py` & `bovine_process-0.2.2/bovine_process/utils/test_by_activity_type.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/bovine_process/utils/test_update_id.py` & `bovine_process-0.2.2/bovine_process/utils/test_update_id.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.0/pyproject.toml` & `bovine_process-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bovine-process"
-version = "0.2.0"
+version = "0.2.2"
 description = "Processing of Side Effects of ActivityPub Activities for an ActivityPub Server"
 authors = ["Helge <helge.krueger@gmail.com>"]
 readme = "README.md"
 packages = [{include = "bovine_process"}]
 license = "MIT"
 repository = "https://codeberg.org/bovine/bovine"
```

### Comparing `bovine_process-0.2.0/setup.py` & `bovine_process-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['bovine-store>=0.2.1,<0.3.0', 'tortoise-orm[asyncpg]>=0.19.3,<0.20.0']
 
 setup_kwargs = {
     'name': 'bovine-process',
-    'version': '0.2.0',
+    'version': '0.2.2',
     'description': 'Processing of Side Effects of ActivityPub Activities for an ActivityPub Server',
     'long_description': "# bovine_process\n\n`bovine_process` consists of the side effect logic of Activity objects. This means it contains the code, the logic that for an incoming object, one executes:\n\n- Store object in bovine_store\n- Add reference to inbox\n- Perform side effects\n- Enque object for bovine_pubsub\n\nAnd a similar list of effects for outgoing objects, i.e\n\n- Store object in bovine_store\n- Add reference to outbox\n- Perform side effects\n- Send objects to follower's inbox\n- Enque object for bovine_pubsub\n\nThe behavior defined in this package corresponds to [6. Client to Server Interactions](https://www.w3.org/TR/activitypub/#client-to-server-interactions) and [7. Server to Server Interactions](https://www.w3.org/TR/activitypub/#server-to-server-interactions) of the ActivityPub specification. However, only a small subset of side effects is implemented.\n\n## Implemented Side Effects\n\n- Create, Update, Delete. Deletes are handled by replacing the object with a Tombstone. Various checks are performed to ensure only appropriate Updates happen.\n- [ ] Specify Update checks\n- Follow and Accept\n  - Outgoing Accept of Follow adds to followers\n  - Incoming Accept of Follows adds to following\n- [ ] Implement other side effects, in particular Like, Announce, and inReplyTo\n- [ ] Authority checks.\n\nThat's it. Currently, no collections for replies and likes are kept in bovine_store, so implementing these side effects cannot happen yet:\n\n- [ ] Announce -> add to share collection\n- [ ] Like -> add to likes collection\n- [ ] Create with inReplyTo -> add to replies collection\n\n## Tests\n\nThe folder `tests/data` contains test cases what side effects happen in the database for certain cases.\n",
     'author': 'Helge',
     'author_email': 'helge.krueger@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://codeberg.org/bovine/bovine',
```

### Comparing `bovine_process-0.2.0/PKG-INFO` & `bovine_process-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bovine-process
-Version: 0.2.0
+Version: 0.2.2
 Summary: Processing of Side Effects of ActivityPub Activities for an ActivityPub Server
 Home-page: https://codeberg.org/bovine/bovine
 License: MIT
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

