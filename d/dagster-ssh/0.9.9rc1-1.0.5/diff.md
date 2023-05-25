# Comparing `tmp/dagster-ssh-0.9.9rc1.tar.gz` & `tmp/dagster-ssh-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-ssh-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:28 2020, max compression
+gzip compressed data, was "dagster-ssh-1.0.5.tar", last modified: Fri Aug 26 13:43:59 2022, max compression
```

## Comparing `dagster-ssh-0.9.9rc1.tar` & `dagster-ssh-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,19 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-ssh-0.9.9rc1/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:04:59.000000 dagster-ssh-0.9.9rc1/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      580 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      119 2020-09-17 21:04:59.000000 dagster-ssh-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/dagster_ssh/
--rw-r--r--   0 bobchen    (501) staff       (20)      246 2020-09-17 21:04:59.000000 dagster-ssh-0.9.9rc1/dagster_ssh/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     9297 2020-09-17 21:04:59.000000 dagster-ssh-0.9.9rc1/dagster_ssh/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-ssh-0.9.9rc1/dagster_ssh/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/dagster_ssh.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      580 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/dagster_ssh.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      428 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/dagster_ssh.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/dagster_ssh.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/dagster_ssh.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/dagster_ssh.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       30 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/dagster_ssh.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/dagster_ssh_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-ssh-0.9.9rc1/dagster_ssh_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     8086 2020-09-17 21:04:59.000000 dagster-ssh-0.9.9rc1/dagster_ssh_tests/test_resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       89 2020-09-17 21:04:59.000000 dagster-ssh-0.9.9rc1/dagster_ssh_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1043 2020-09-17 21:04:59.000000 dagster-ssh-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:43:59.031971 dagster-ssh-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-ssh-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       63 2022-08-26 13:33:01.000000 dagster-ssh-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      660 2022-08-26 13:43:59.031971 dagster-ssh-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      119 2022-08-26 13:33:01.000000 dagster-ssh-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:43:59.027971 dagster-ssh-1.0.5/dagster_ssh/
+-rw-r--r--   0 root         (0) root         (0)      247 2022-08-26 13:33:01.000000 dagster-ssh-1.0.5/dagster_ssh/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-ssh-1.0.5/dagster_ssh/py.typed
+-rw-r--r--   0 root         (0) root         (0)     9346 2022-08-26 13:33:01.000000 dagster-ssh-1.0.5/dagster_ssh/resources.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-ssh-1.0.5/dagster_ssh/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:43:59.027971 dagster-ssh-1.0.5/dagster_ssh.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      660 2022-08-26 13:43:58.000000 dagster-ssh-1.0.5/dagster_ssh.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      349 2022-08-26 13:43:58.000000 dagster-ssh-1.0.5/dagster_ssh.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:43:58.000000 dagster-ssh-1.0.5/dagster_ssh.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:43:58.000000 dagster-ssh-1.0.5/dagster_ssh.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       87 2022-08-26 13:43:58.000000 dagster-ssh-1.0.5/dagster_ssh.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-08-26 13:43:58.000000 dagster-ssh-1.0.5/dagster_ssh.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2022-08-26 13:43:59.031971 dagster-ssh-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1391 2022-08-26 13:33:01.000000 dagster-ssh-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagster-ssh-0.9.9rc1/LICENSE` & `dagster-ssh-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-ssh-0.9.9rc1/PKG-INFO` & `dagster-ssh-1.0.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-ssh
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: Package for ssh Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-ssh
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Description: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Provides-Extra: test
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-ssh-0.9.9rc1/dagster_ssh/resources.py` & `dagster-ssh-1.0.5/dagster_ssh/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import getpass
 import os
+from io import StringIO
 
 import paramiko
 from paramiko.config import SSH_PORT
-from six import StringIO
 from sshtunnel import SSHTunnelForwarder
 
-from dagster import Field, StringSource, check, resource
-from dagster.utils import merge_dicts, mkdir_p
+from dagster import Field, StringSource
+from dagster import _check as check
+from dagster import resource
+from dagster._utils import merge_dicts, mkdir_p
 
 
 def key_from_str(key_str):
     """Creates a paramiko SSH key from a string."""
     check.str_param(key_str, "key_str")
 
     # py2 StringIO doesn't support with
     key_file = StringIO(key_str)
     result = paramiko.RSAKey.from_private_key(key_file)
     key_file.close()
     return result
 
 
-class SSHResource(object):
+class SSHResource:
     """
     Resource for ssh remote execution using Paramiko.
     ref: https://github.com/paramiko/paramiko
     """
 
     def __init__(
         self,
@@ -68,15 +70,15 @@
                 " getpass.getuser()" % self.remote_host
             )
             self.username = getpass.getuser()
 
         user_ssh_config_filename = os.path.expanduser("~/.ssh/config")
         if os.path.isfile(user_ssh_config_filename):
             ssh_conf = paramiko.SSHConfig()
-            ssh_conf.parse(open(user_ssh_config_filename))
+            ssh_conf.parse(open(user_ssh_config_filename, encoding="utf8"))
             host_info = ssh_conf.lookup(self.remote_host)
             if host_info and host_info.get("proxycommand"):
                 self.host_proxy = paramiko.ProxyCommand(host_info.get("proxycommand"))
 
             if not (self.password or self.key_file):
                 if host_info and host_info.get("identityfile"):
                     self.key_file = host_info.get("identityfile")[0]
@@ -249,9 +251,9 @@
         "compress": Field(bool, is_required=False, default_value=True),
         "no_host_key_check": Field(bool, is_required=False, default_value=True),
         "allow_host_key_change": Field(bool, is_required=False, default_value=False),
     }
 )
 def ssh_resource(init_context):
     args = init_context.resource_config
-    args = merge_dicts(init_context.resource_config, {"logger": init_context.log_manager})
+    args = merge_dicts(init_context.resource_config, {"logger": init_context.log})
     return SSHResource(**args)
```

### Comparing `dagster-ssh-0.9.9rc1/dagster_ssh.egg-info/PKG-INFO` & `dagster-ssh-1.0.5/dagster_ssh.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-ssh
-Version: 0.9.9rc1
+Version: 1.0.5
 Summary: Package for ssh Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-ssh
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Description: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Provides-Extra: test
+License-File: LICENSE
+
+UNKNOWN
+
```

