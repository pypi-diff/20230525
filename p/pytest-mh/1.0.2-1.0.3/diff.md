# Comparing `tmp/pytest_mh-1.0.2.tar.gz` & `tmp/pytest_mh-1.0.3.tar.gz`

## Comparing `pytest_mh-1.0.2.tar` & `pytest_mh-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/requirements.txt
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/docs/requirements.txt
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/__init__.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/py.typed
--rw-r--r--   0        0        0    31460 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/ssh.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/_private/data.py
--rw-r--r--   0        0        0     8103 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/_private/fixtures.py
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/_private/logging.py
--rw-r--r--   0        0        0     8334 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/_private/marks.py
--rw-r--r--   0        0        0    18781 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/_private/multihost.py
--rw-r--r--   0        0        0    14927 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/_private/plugin.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/_private/topology.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/_private/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/utils/__init__.py
--rw-r--r--   0        0        0     9886 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/utils/firewall.py
--rw-r--r--   0        0        0    14342 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/utils/fs.py
--rw-r--r--   0        0        0     7953 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pytest_mh/utils/services.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/LICENSE
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/readme.md
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 pytest_mh-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pytest_mh-1.0.3/requirements.txt
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pytest_mh-1.0.3/docs/requirements.txt
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 pytest_mh-1.0.3/pytest_mh/__init__.py
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 pytest_mh-1.0.3/pytest_mh/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_mh-1.0.3/pytest_mh/py.typed
+-rw-r--r--   0        0        0    31460 2020-02-02 00:00:00.000000 pytest_mh-1.0.3/pytest_mh/ssh.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 pytest_mh-1.0.3/pytest_mh/_private/data.py
+-rw-r--r--   0        0        0     8103 2020-02-02 00:00:00.000000 pytest_mh-1.0.3/pytest_mh/_private/fixtures.py
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 pytest_mh-1.0.3/pytest_mh/_private/logging.py
+-rw-r--r--   0        0        0     8334 2020-02-02 00:00:00.000000 pytest_mh-1.0.3/pytest_mh/_private/marks.py
+-rw-r--r--   0        0        0    18781 2020-02-02 00:00:00.000000 pytest_mh-1.0.3/pytest_mh/_private/multihost.py
+-rw-r--r--   0        0        0    14927 2020-02-02 00:00:00.000000 pytest_mh-1.0.3/pytest_mh/_private/plugin.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 pytest_mh-1.0.3/pytest_mh/_private/topology.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 pytest_mh-1.0.3/pytest_mh/_private/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_mh-1.0.3/pytest_mh/utils/__init__.py
+-rw-r--r--   0        0        0     9886 2020-02-02 00:00:00.000000 pytest_mh-1.0.3/pytest_mh/utils/firewall.py
+-rw-r--r--   0        0        0    14342 2020-02-02 00:00:00.000000 pytest_mh-1.0.3/pytest_mh/utils/fs.py
+-rw-r--r--   0        0        0     7953 2020-02-02 00:00:00.000000 pytest_mh-1.0.3/pytest_mh/utils/services.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pytest_mh-1.0.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pytest_mh-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pytest_mh-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pytest_mh-1.0.3/readme.md
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 pytest_mh-1.0.3/PKG-INFO
```

### Comparing `pytest_mh-1.0.2/pytest_mh/__init__.py` & `pytest_mh-1.0.3/pytest_mh/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.2/pytest_mh/cli.py` & `pytest_mh-1.0.3/pytest_mh/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,16 @@
             match type:
                 case self.option.POSITIONAL:
                     argv.append(_get_value(value))
                 case self.option.SWITCH:
                     if self.__match_shell(SSHPowerShellProcess):
                         argv.append(f'{_get_option(key)}:{"$True" if value else "$False"}')
                     else:
-                        argv.append(_get_option(key))
+                        if value:
+                            argv.append(_get_option(key))
                 case self.option.VALUE:
                     argv.append(_get_option(key))
                     argv.append(_get_value(value))
                 case self.option.PLAIN:
                     argv.append(_get_option(key))
                     argv.append(str(value))
                 case _:
```

### Comparing `pytest_mh-1.0.2/pytest_mh/ssh.py` & `pytest_mh-1.0.3/pytest_mh/ssh.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.2/pytest_mh/_private/data.py` & `pytest_mh-1.0.3/pytest_mh/_private/data.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.2/pytest_mh/_private/fixtures.py` & `pytest_mh-1.0.3/pytest_mh/_private/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.2/pytest_mh/_private/logging.py` & `pytest_mh-1.0.3/pytest_mh/_private/logging.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.2/pytest_mh/_private/marks.py` & `pytest_mh-1.0.3/pytest_mh/_private/marks.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.2/pytest_mh/_private/multihost.py` & `pytest_mh-1.0.3/pytest_mh/_private/multihost.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.2/pytest_mh/_private/plugin.py` & `pytest_mh-1.0.3/pytest_mh/_private/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.2/pytest_mh/_private/topology.py` & `pytest_mh-1.0.3/pytest_mh/_private/topology.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.2/pytest_mh/_private/utils.py` & `pytest_mh-1.0.3/pytest_mh/_private/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.2/pytest_mh/utils/firewall.py` & `pytest_mh-1.0.3/pytest_mh/utils/firewall.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.2/pytest_mh/utils/fs.py` & `pytest_mh-1.0.3/pytest_mh/utils/fs.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.2/pytest_mh/utils/services.py` & `pytest_mh-1.0.3/pytest_mh/utils/services.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.2/LICENSE` & `pytest_mh-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.2/pyproject.toml` & `pytest_mh-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.2/readme.md` & `pytest_mh-1.0.3/readme.md`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.2/PKG-INFO` & `pytest_mh-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-mh
-Version: 1.0.2
+Version: 1.0.3
 Summary: Pytest multihost plugin
 Project-URL: Homepage, https://github.com/next-actions/pytest-mh
 Project-URL: Bug Tracker, https://github.com/next-actions/pytest-mh/issues
 Author-email: Pavel Březina <pbrezina@redhat.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

