# Comparing `tmp/copr-messaging-0.8.tar.gz` & `tmp/copr-messaging-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copr-messaging-0.8.tar", last modified: Wed Jan 25 14:19:31 2023, max compression
+gzip compressed data, was "copr-messaging-0.9.tar", last modified: Wed Apr  5 15:27:03 2023, max compression
```

## Comparing `copr-messaging-0.8.tar` & `copr-messaging-0.9.tar`

### file list

```diff
@@ -1,41 +1,39 @@
-drwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)        0 2023-01-25 14:19:31.026262 copr-messaging-0.8/
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)    18092 2021-12-12 15:37:48.000000 copr-messaging-0.8/LICENSE
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      136 2022-11-13 20:33:19.000000 copr-messaging-0.8/MANIFEST.in
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      203 2022-11-13 20:33:19.000000 copr-messaging-0.8/Makefile
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      824 2023-01-25 14:19:31.025262 copr-messaging-0.8/PKG-INFO
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      398 2021-12-12 15:37:48.000000 copr-messaging-0.8/README.md
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     2726 2023-01-25 13:29:44.000000 copr-messaging-0.8/copr-messaging.spec
-drwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)        0 2023-01-25 14:19:31.024262 copr-messaging-0.8/copr_messaging/
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      742 2021-12-12 15:37:48.000000 copr-messaging-0.8/copr_messaging/__init__.py
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     2450 2021-12-12 15:37:48.000000 copr-messaging-0.8/copr_messaging/fedora.py
-drwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)        0 2023-01-25 14:19:31.025262 copr-messaging-0.8/copr_messaging/private/
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)        0 2021-12-12 15:37:48.000000 copr-messaging-0.8/copr_messaging/private/__init__.py
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      933 2021-12-12 15:37:48.000000 copr-messaging-0.8/copr_messaging/private/consumer.py
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     5066 2021-12-12 15:37:48.000000 copr-messaging-0.8/copr_messaging/private/hierarchy.py
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     4427 2021-12-12 15:37:48.000000 copr-messaging-0.8/copr_messaging/private/schema_old.py
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     3915 2021-12-12 15:37:48.000000 copr-messaging-0.8/copr_messaging/private/schema_stomp_old.py
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     4035 2021-12-12 15:37:48.000000 copr-messaging-0.8/copr_messaging/schema.py
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     2813 2022-06-25 00:43:16.000000 copr-messaging-0.8/copr_messaging/stomp.py
-drwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)        0 2023-01-25 14:19:31.025262 copr-messaging-0.8/copr_messaging/tests/
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      742 2021-12-12 15:37:48.000000 copr-messaging-0.8/copr_messaging/tests/__init__.py
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)    16557 2021-12-12 15:37:48.000000 copr-messaging-0.8/copr_messaging/tests/test_schema.py
-drwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)        0 2023-01-25 14:19:31.024262 copr-messaging-0.8/copr_messaging.egg-info/
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      824 2023-01-25 14:19:30.000000 copr-messaging-0.8/copr_messaging.egg-info/PKG-INFO
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      825 2023-01-25 14:19:30.000000 copr-messaging-0.8/copr_messaging.egg-info/SOURCES.txt
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)        1 2023-01-25 14:19:30.000000 copr-messaging-0.8/copr_messaging.egg-info/dependency_links.txt
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      434 2023-01-25 14:19:30.000000 copr-messaging-0.8/copr_messaging.egg-info/entry_points.txt
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)        1 2022-11-29 13:17:26.000000 copr-messaging-0.8/copr_messaging.egg-info/not-zip-safe
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)       29 2023-01-25 14:19:30.000000 copr-messaging-0.8/copr_messaging.egg-info/requires.txt
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)       15 2023-01-25 14:19:30.000000 copr-messaging-0.8/copr_messaging.egg-info/top_level.txt
-drwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)        0 2023-01-25 14:19:31.025262 copr-messaging-0.8/docs/
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      580 2021-12-12 15:37:48.000000 copr-messaging-0.8/docs/Makefile
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      787 2021-12-12 15:37:48.000000 copr-messaging-0.8/docs/api.rst
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     6153 2021-12-12 15:37:48.000000 copr-messaging-0.8/docs/conf.py
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     3422 2021-12-12 15:37:48.000000 copr-messaging-0.8/docs/consuming.rst
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      598 2021-12-12 15:37:48.000000 copr-messaging-0.8/docs/index.rst
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)      173 2021-12-12 15:37:48.000000 copr-messaging-0.8/docs/installation.rst
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     4849 2022-11-13 20:33:19.000000 copr-messaging-0.8/pylintrc
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)       29 2021-12-12 15:37:48.000000 copr-messaging-0.8/requirements.txt
--rwxr-xr-x   0 jkadlcik  (1000) jkadlcik  (1000)      148 2022-11-13 20:33:19.000000 copr-messaging-0.8/run_tests.sh
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)       38 2023-01-25 14:19:31.026262 copr-messaging-0.8/setup.cfg
--rw-r--r--   0 jkadlcik  (1000) jkadlcik  (1000)     2619 2023-01-25 13:29:44.000000 copr-messaging-0.8/setup.py
+drwxr-xr-x   0 jkyjovsk (4203067) jkyjovsk (4203067)        0 2023-04-05 15:27:03.293357 copr-messaging-0.9/
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)    18092 2023-03-20 15:10:09.000000 copr-messaging-0.9/LICENSE
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)      136 2023-03-20 15:10:09.000000 copr-messaging-0.9/MANIFEST.in
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)      824 2023-04-05 15:27:03.293357 copr-messaging-0.9/PKG-INFO
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)      398 2023-03-20 15:10:09.000000 copr-messaging-0.9/README.md
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)     2839 2023-03-27 07:35:00.000000 copr-messaging-0.9/copr-messaging.spec
+drwxr-xr-x   0 jkyjovsk (4203067) jkyjovsk (4203067)        0 2023-04-05 15:27:03.292356 copr-messaging-0.9/copr_messaging/
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)      742 2023-03-20 15:10:09.000000 copr-messaging-0.9/copr_messaging/__init__.py
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)     2450 2023-03-20 15:10:09.000000 copr-messaging-0.9/copr_messaging/fedora.py
+drwxr-xr-x   0 jkyjovsk (4203067) jkyjovsk (4203067)        0 2023-04-05 15:27:03.293357 copr-messaging-0.9/copr_messaging/private/
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)        0 2023-03-20 15:10:09.000000 copr-messaging-0.9/copr_messaging/private/__init__.py
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)      933 2023-03-20 15:10:09.000000 copr-messaging-0.9/copr_messaging/private/consumer.py
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)     5287 2023-03-20 15:10:09.000000 copr-messaging-0.9/copr_messaging/private/hierarchy.py
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)     4427 2023-03-20 15:10:09.000000 copr-messaging-0.9/copr_messaging/private/schema_old.py
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)     3915 2023-03-20 15:10:09.000000 copr-messaging-0.9/copr_messaging/private/schema_stomp_old.py
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)     4035 2023-03-20 15:10:09.000000 copr-messaging-0.9/copr_messaging/schema.py
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)     2813 2023-03-20 15:10:09.000000 copr-messaging-0.9/copr_messaging/stomp.py
+drwxr-xr-x   0 jkyjovsk (4203067) jkyjovsk (4203067)        0 2023-04-05 15:27:03.293357 copr-messaging-0.9/copr_messaging/tests/
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)      742 2023-03-20 15:10:09.000000 copr-messaging-0.9/copr_messaging/tests/__init__.py
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)    16878 2023-03-20 15:10:09.000000 copr-messaging-0.9/copr_messaging/tests/test_schema.py
+drwxr-xr-x   0 jkyjovsk (4203067) jkyjovsk (4203067)        0 2023-04-05 15:27:03.292356 copr-messaging-0.9/copr_messaging.egg-info/
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)      824 2023-04-05 15:27:02.000000 copr-messaging-0.9/copr_messaging.egg-info/PKG-INFO
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)      807 2023-04-05 15:27:03.000000 copr-messaging-0.9/copr_messaging.egg-info/SOURCES.txt
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)        1 2023-04-05 15:27:03.000000 copr-messaging-0.9/copr_messaging.egg-info/dependency_links.txt
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)      434 2023-04-05 15:27:03.000000 copr-messaging-0.9/copr_messaging.egg-info/entry_points.txt
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)        1 2023-04-05 15:27:02.000000 copr-messaging-0.9/copr_messaging.egg-info/not-zip-safe
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)       29 2023-04-05 15:27:03.000000 copr-messaging-0.9/copr_messaging.egg-info/requires.txt
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)       15 2023-04-05 15:27:03.000000 copr-messaging-0.9/copr_messaging.egg-info/top_level.txt
+drwxr-xr-x   0 jkyjovsk (4203067) jkyjovsk (4203067)        0 2023-04-05 15:27:03.293357 copr-messaging-0.9/docs/
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)      580 2023-03-20 15:10:09.000000 copr-messaging-0.9/docs/Makefile
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)      787 2023-03-20 15:10:09.000000 copr-messaging-0.9/docs/api.rst
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)     6153 2023-03-20 15:10:09.000000 copr-messaging-0.9/docs/conf.py
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)     3422 2023-03-20 15:10:09.000000 copr-messaging-0.9/docs/consuming.rst
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)      606 2023-03-20 15:10:09.000000 copr-messaging-0.9/docs/index.rst
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)      173 2023-03-20 15:10:09.000000 copr-messaging-0.9/docs/installation.rst
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)       29 2023-03-20 15:10:09.000000 copr-messaging-0.9/requirements.txt
+-rwxr-xr-x   0 jkyjovsk (4203067) jkyjovsk (4203067)      148 2023-03-20 15:10:09.000000 copr-messaging-0.9/run_tests.sh
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)       38 2023-04-05 15:27:03.293357 copr-messaging-0.9/setup.cfg
+-rw-r--r--   0 jkyjovsk (4203067) jkyjovsk (4203067)     2619 2023-03-27 07:35:00.000000 copr-messaging-0.9/setup.py
```

### Comparing `copr-messaging-0.8/LICENSE` & `copr-messaging-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `copr-messaging-0.8/PKG-INFO` & `copr-messaging-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copr-messaging
-Version: 0.8
+Version: 0.9
 Summary: A schema and tooling for Copr fedora-messaging
 Home-page: https://github.com/fedora-copr/copr
 Maintainer: Copr Team
 Maintainer-email: copr-devel@lists.fedorahosted.org
 License: GPLv2+
 Keywords: fedora
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
```

### Comparing `copr-messaging-0.8/copr-messaging.spec` & `copr-messaging-0.9/copr-messaging.spec`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 fedora-messaging documentation page \
 https://fedora-messaging.readthedocs.io/en/latest/messages.html#schema \
 \
 Package also provides several convenience methods for working with \
 copr messages.
 
 Name:       copr-messaging
-Version:    0.8
+Version:    0.9
 Release:    1%{?dist}
 Summary:    Abstraction for Copr messaging listeners/publishers
 
 License:    GPL-2.0-or-later
 URL:        https://github.com/fedora-copr/copr
 
 # Source is created by:
@@ -82,14 +82,16 @@
 
 %files -n python3-%name-doc
 %license LICENSE
 %doc html
 
 
 %changelog
+* Wed Mar 22 2023 Jiri Kyjovsky <j1.kyjovsky@gmail.com> 0.9-1
+- Add app_name property to _CoprMessage base class
 * Tue Jan 24 2023 Jakub Kadlcik <frostyx@email.cz> 0.8-1
 - Use SPDX license
 
 * Sat Nov 26 2022 Jakub Kadlcik <frostyx@email.cz> 0.7-1
 - move to GitHub home page
 - sync tooling with other sub-projects
```

### Comparing `copr-messaging-0.8/copr_messaging/__init__.py` & `copr-messaging-0.9/copr_messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `copr-messaging-0.8/copr_messaging/fedora.py` & `copr-messaging-0.9/copr_messaging/fedora.py`

 * *Files identical despite different names*

### Comparing `copr-messaging-0.8/copr_messaging/private/consumer.py` & `copr-messaging-0.9/copr_messaging/private/consumer.py`

 * *Files identical despite different names*

### Comparing `copr-messaging-0.8/copr_messaging/private/hierarchy.py` & `copr-messaging-0.9/copr_messaging/private/hierarchy.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,24 @@
     """
     def __str__(self):
         return "Unspecified Copr message"
 
     def _str_prefix(self):
         return "Copr Message"
 
+    @property
+    def app_name(self):
+        """
+        Return the name of the application that generated the message.
+
+        Returns:
+            the name of the application (copr)
+        """
+        return "Copr"
+
 
 class _CoprProjectMessage(_CoprMessage):
     def _str_prefix(self):
         return '{0} in project "{1}"'.format(
             super(_CoprProjectMessage, self)._str_prefix(),
             self.project_full_name,
         )
```

### Comparing `copr-messaging-0.8/copr_messaging/private/schema_old.py` & `copr-messaging-0.9/copr_messaging/private/schema_old.py`

 * *Files identical despite different names*

### Comparing `copr-messaging-0.8/copr_messaging/private/schema_stomp_old.py` & `copr-messaging-0.9/copr_messaging/private/schema_stomp_old.py`

 * *Files identical despite different names*

### Comparing `copr-messaging-0.8/copr_messaging/schema.py` & `copr-messaging-0.9/copr_messaging/schema.py`

 * *Files identical despite different names*

### Comparing `copr-messaging-0.8/copr_messaging/stomp.py` & `copr-messaging-0.9/copr_messaging/stomp.py`

 * *Files identical despite different names*

### Comparing `copr-messaging-0.8/copr_messaging/tests/__init__.py` & `copr-messaging-0.9/copr_messaging/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `copr-messaging-0.8/copr_messaging/tests/test_schema.py` & `copr-messaging-0.9/copr_messaging/tests/test_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,7 +281,19 @@
         self.fedmsg_message = {
             "chroot": "fedora-29-x86_64"
         }
 
     def test_chroot(self):
         msg = self.msg_class(body=self.fedmsg_message)
         msg.validate()
+
+
+class CoprMessageBaseClassTest(unittest.TestCase):
+
+    def setUp(self):
+        # we can't test the base class directly, so we use
+        # something that is a subclass of it
+        #
+        self.message = schema.BuildChrootStartedV1({})
+
+    def test_app_name(self):
+        assert self.message.app_name == "Copr"
```

### Comparing `copr-messaging-0.8/copr_messaging.egg-info/PKG-INFO` & `copr-messaging-0.9/copr_messaging.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copr-messaging
-Version: 0.8
+Version: 0.9
 Summary: A schema and tooling for Copr fedora-messaging
 Home-page: https://github.com/fedora-copr/copr
 Maintainer: Copr Team
 Maintainer-email: copr-devel@lists.fedorahosted.org
 License: GPLv2+
 Keywords: fedora
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
```

### Comparing `copr-messaging-0.8/copr_messaging.egg-info/SOURCES.txt` & `copr-messaging-0.9/copr_messaging.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 LICENSE
 MANIFEST.in
-Makefile
 README.md
 copr-messaging.spec
-pylintrc
 requirements.txt
 run_tests.sh
 setup.py
 copr_messaging/__init__.py
 copr_messaging/fedora.py
 copr_messaging/schema.py
 copr_messaging/stomp.py
```

### Comparing `copr-messaging-0.8/docs/Makefile` & `copr-messaging-0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `copr-messaging-0.8/docs/api.rst` & `copr-messaging-0.9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `copr-messaging-0.8/docs/conf.py` & `copr-messaging-0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `copr-messaging-0.8/docs/consuming.rst` & `copr-messaging-0.9/docs/consuming.rst`

 * *Files identical despite different names*

### Comparing `copr-messaging-0.8/docs/index.rst` & `copr-messaging-0.9/docs/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 ------------------
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
 
 
-.. _`Copr build system`: https://pagure.io/copr/copr
+.. _`Copr build system`: https://github.com/fedora-copr/copr
```

### Comparing `copr-messaging-0.8/setup.py` & `copr-messaging-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 
 with open(os.path.join(here, "requirements.txt")) as f:
     __requires__ = f.read().split("\n")[:-1]
 
 setup(
     name=__name__,
-    version="0.8",
+    version="0.9",
     description=__description__,
     long_description=README,
     url=__url__,
 
     # Possible options are at https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
```

