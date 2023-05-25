# Comparing `tmp/PyMySQL-1.0.3rc1.tar.gz` & `tmp/PyMySQL-1.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMySQL-1.0.3rc1.tar", last modified: Fri Mar 24 08:57:41 2023, max compression
+gzip compressed data, was "PyMySQL-1.1.0rc1.tar", last modified: Thu May 25 06:27:52 2023, max compression
```

## Comparing `PyMySQL-1.0.3rc1.tar` & `PyMySQL-1.1.0rc1.tar`

### file list

```diff
@@ -1,27 +1,36 @@
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-03-24 08:57:41.613093 PyMySQL-1.0.3rc1/
--rw-r--r--   0 inada-n    (502) staff       (20)    11228 2023-01-19 01:09:53.000000 PyMySQL-1.0.3rc1/CHANGELOG.md
--rw-r--r--   0 inada-n    (502) staff       (20)     1070 2013-11-27 14:43:24.000000 PyMySQL-1.0.3rc1/LICENSE
--rw-r--r--   0 inada-n    (502) staff       (20)       39 2023-03-22 15:10:23.000000 PyMySQL-1.0.3rc1/MANIFEST.in
--rw-r--r--   0 inada-n    (502) staff       (20)     4273 2023-03-24 08:57:41.612983 PyMySQL-1.0.3rc1/PKG-INFO
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-03-24 08:57:41.611604 PyMySQL-1.0.3rc1/PyMySQL.egg-info/
--rw-r--r--   0 inada-n    (502) staff       (20)     4273 2023-03-24 08:57:41.000000 PyMySQL-1.0.3rc1/PyMySQL.egg-info/PKG-INFO
--rw-r--r--   0 inada-n    (502) staff       (20)      424 2023-03-24 08:57:41.000000 PyMySQL-1.0.3rc1/PyMySQL.egg-info/SOURCES.txt
--rw-r--r--   0 inada-n    (502) staff       (20)        1 2023-03-24 08:57:41.000000 PyMySQL-1.0.3rc1/PyMySQL.egg-info/dependency_links.txt
--rw-r--r--   0 inada-n    (502) staff       (20)       45 2023-03-24 08:57:41.000000 PyMySQL-1.0.3rc1/PyMySQL.egg-info/requires.txt
--rw-r--r--   0 inada-n    (502) staff       (20)        8 2023-03-24 08:57:41.000000 PyMySQL-1.0.3rc1/PyMySQL.egg-info/top_level.txt
--rw-r--r--   0 inada-n    (502) staff       (20)     3181 2023-03-22 15:10:36.000000 PyMySQL-1.0.3rc1/README.md
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-03-24 08:57:41.612734 PyMySQL-1.0.3rc1/pymysql/
--rw-r--r--   0 inada-n    (502) staff       (20)     4392 2023-03-23 16:42:27.000000 PyMySQL-1.0.3rc1/pymysql/__init__.py
--rw-r--r--   0 inada-n    (502) staff       (20)     7399 2023-01-19 01:09:53.000000 PyMySQL-1.0.3rc1/pymysql/_auth.py
--rw-r--r--   0 inada-n    (502) staff       (20)    10293 2022-01-31 04:32:36.000000 PyMySQL-1.0.3rc1/pymysql/charset.py
--rw-r--r--   0 inada-n    (502) staff       (20)    51465 2022-10-05 00:46:59.000000 PyMySQL-1.0.3rc1/pymysql/connections.py
--rw-r--r--   0 inada-n    (502) staff       (20)     9550 2022-10-05 00:46:59.000000 PyMySQL-1.0.3rc1/pymysql/converters.py
--rw-r--r--   0 inada-n    (502) staff       (20)    15692 2022-01-31 04:32:36.000000 PyMySQL-1.0.3rc1/pymysql/cursors.py
--rw-r--r--   0 inada-n    (502) staff       (20)     3773 2021-01-03 03:07:14.000000 PyMySQL-1.0.3rc1/pymysql/err.py
--rw-r--r--   0 inada-n    (502) staff       (20)      573 2021-01-03 03:07:14.000000 PyMySQL-1.0.3rc1/pymysql/optionfile.py
--rw-r--r--   0 inada-n    (502) staff       (20)    11859 2022-01-31 04:32:36.000000 PyMySQL-1.0.3rc1/pymysql/protocol.py
--rw-r--r--   0 inada-n    (502) staff       (20)      360 2021-01-02 07:55:27.000000 PyMySQL-1.0.3rc1/pymysql/times.py
--rw-r--r--   0 inada-n    (502) staff       (20)     1425 2023-03-23 16:42:27.000000 PyMySQL-1.0.3rc1/pyproject.toml
--rw-r--r--   0 inada-n    (502) staff       (20)       38 2023-03-24 08:57:41.613123 PyMySQL-1.0.3rc1/setup.cfg
-drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-03-24 08:57:41.612845 PyMySQL-1.0.3rc1/tests/
--rw-r--r--   0 inada-n    (502) staff       (20)     2140 2021-01-03 03:07:14.000000 PyMySQL-1.0.3rc1/tests/test_auth.py
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-25 06:27:52.993198 PyMySQL-1.1.0rc1/
+-rw-r--r--   0 inada-n    (502) staff       (20)    12745 2023-05-25 06:27:10.000000 PyMySQL-1.1.0rc1/CHANGELOG.md
+-rw-r--r--   0 inada-n    (502) staff       (20)     1070 2013-11-27 14:43:24.000000 PyMySQL-1.1.0rc1/LICENSE
+-rw-r--r--   0 inada-n    (502) staff       (20)       39 2023-05-23 15:12:24.000000 PyMySQL-1.1.0rc1/MANIFEST.in
+-rw-r--r--   0 inada-n    (502) staff       (20)     4260 2023-05-25 06:27:52.993087 PyMySQL-1.1.0rc1/PKG-INFO
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-25 06:27:52.990740 PyMySQL-1.1.0rc1/PyMySQL.egg-info/
+-rw-r--r--   0 inada-n    (502) staff       (20)     4260 2023-05-25 06:27:52.000000 PyMySQL-1.1.0rc1/PyMySQL.egg-info/PKG-INFO
+-rw-r--r--   0 inada-n    (502) staff       (20)      652 2023-05-25 06:27:52.000000 PyMySQL-1.1.0rc1/PyMySQL.egg-info/SOURCES.txt
+-rw-r--r--   0 inada-n    (502) staff       (20)        1 2023-05-25 06:27:52.000000 PyMySQL-1.1.0rc1/PyMySQL.egg-info/dependency_links.txt
+-rw-r--r--   0 inada-n    (502) staff       (20)       45 2023-05-25 06:27:52.000000 PyMySQL-1.1.0rc1/PyMySQL.egg-info/requires.txt
+-rw-r--r--   0 inada-n    (502) staff       (20)        8 2023-05-25 06:27:52.000000 PyMySQL-1.1.0rc1/PyMySQL.egg-info/top_level.txt
+-rw-r--r--   0 inada-n    (502) staff       (20)     3168 2023-05-24 05:52:56.000000 PyMySQL-1.1.0rc1/README.md
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-25 06:27:52.991877 PyMySQL-1.1.0rc1/pymysql/
+-rw-r--r--   0 inada-n    (502) staff       (20)     4264 2023-05-25 06:27:10.000000 PyMySQL-1.1.0rc1/pymysql/__init__.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     7416 2023-05-24 05:21:28.000000 PyMySQL-1.1.0rc1/pymysql/_auth.py
+-rw-r--r--   0 inada-n    (502) staff       (20)    10301 2023-05-24 16:54:14.000000 PyMySQL-1.1.0rc1/pymysql/charset.py
+-rw-r--r--   0 inada-n    (502) staff       (20)    53589 2023-05-25 06:27:10.000000 PyMySQL-1.1.0rc1/pymysql/connections.py
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-25 06:27:52.992849 PyMySQL-1.1.0rc1/pymysql/constants/
+-rw-r--r--   0 inada-n    (502) staff       (20)      878 2021-01-03 03:07:14.000000 PyMySQL-1.1.0rc1/pymysql/constants/CLIENT.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      679 2021-01-03 03:07:14.000000 PyMySQL-1.1.0rc1/pymysql/constants/COMMAND.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     2320 2023-05-23 15:12:24.000000 PyMySQL-1.1.0rc1/pymysql/constants/CR.py
+-rw-r--r--   0 inada-n    (502) staff       (20)    12357 2023-05-23 15:12:24.000000 PyMySQL-1.1.0rc1/pymysql/constants/ER.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      370 2021-01-03 03:07:14.000000 PyMySQL-1.1.0rc1/pymysql/constants/FIELD_TYPE.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      214 2018-12-18 12:04:22.000000 PyMySQL-1.1.0rc1/pymysql/constants/FLAG.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      333 2021-01-03 03:07:14.000000 PyMySQL-1.1.0rc1/pymysql/constants/SERVER_STATUS.py
+-rw-r--r--   0 inada-n    (502) staff       (20)        0 2014-08-29 11:32:54.000000 PyMySQL-1.1.0rc1/pymysql/constants/__init__.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     9591 2023-05-24 07:46:55.000000 PyMySQL-1.1.0rc1/pymysql/converters.py
+-rw-r--r--   0 inada-n    (502) staff       (20)    16535 2023-05-24 16:03:44.000000 PyMySQL-1.1.0rc1/pymysql/cursors.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     3773 2021-01-03 03:07:14.000000 PyMySQL-1.1.0rc1/pymysql/err.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      651 2023-05-24 13:30:02.000000 PyMySQL-1.1.0rc1/pymysql/optionfile.py
+-rw-r--r--   0 inada-n    (502) staff       (20)    11863 2023-05-24 16:03:44.000000 PyMySQL-1.1.0rc1/pymysql/protocol.py
+-rw-r--r--   0 inada-n    (502) staff       (20)      360 2021-01-02 07:55:27.000000 PyMySQL-1.1.0rc1/pymysql/times.py
+-rw-r--r--   0 inada-n    (502) staff       (20)     1557 2023-05-25 02:33:20.000000 PyMySQL-1.1.0rc1/pyproject.toml
+-rw-r--r--   0 inada-n    (502) staff       (20)       38 2023-05-25 06:27:52.993228 PyMySQL-1.1.0rc1/setup.cfg
+drwxr-xr-x   0 inada-n    (502) staff       (20)        0 2023-05-25 06:27:52.992940 PyMySQL-1.1.0rc1/tests/
+-rw-r--r--   0 inada-n    (502) staff       (20)     2140 2021-01-03 03:07:14.000000 PyMySQL-1.1.0rc1/tests/test_auth.py
```

### Comparing `PyMySQL-1.0.3rc1/CHANGELOG.md` & `PyMySQL-1.1.0rc1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,38 @@
 # Changes
 
-## v1.0.3
+## v1.1.0
 
 Release date: TBD
 
+* Fixed SSCursor raising OperationalError for query timeouts on wrong statement (#1032)
+* Exposed `Cursor.warning_count` to check for warnings without additional query (#1056)
+* Make Cursor iterator (#995)
+* Support '_' in key name in my.cnf (#1114)
+* `Cursor.fetchall()` returns empty list instead of tuple (#1115). Note that `Cursor.fetchmany()` still return empty tuple after reading all rows for compatibility with Django.
+* Deprecate Error classes in Cursor class (#1117)
+* Add `Connection.set_character_set(charset, collation=None)` (#1119)
+* Deprecate `Connection.set_charset(charset)` (#1119)
+* New connection always send "SET NAMES charset [COLLATE collation]" query. (#1119)
+  Since collation table is vary on MySQL server versions, collation in handshake is fragile.
+
+
+## v1.0.3
+
+Release date: 2023-03-28
+
 * Dropped support of end of life MySQL version 5.6
 * Dropped support of end of life MariaDB versions below 10.3
 * Dropped support of end of life Python version 3.6
+* Removed _last_executed because of duplication with _executed by @rajat315315 in https://github.com/PyMySQL/PyMySQL/pull/948
+* Fix generating authentication response with long strings by @netch80 in https://github.com/PyMySQL/PyMySQL/pull/988
+* update pymysql.constants.CR by @Nothing4You in https://github.com/PyMySQL/PyMySQL/pull/1029
+* Document that the ssl connection parameter can be an SSLContext by @cakemanny in https://github.com/PyMySQL/PyMySQL/pull/1045
+* Raise ProgrammingError on -np.inf in addition to np.inf by @cdcadman in https://github.com/PyMySQL/PyMySQL/pull/1067
+* Use Python 3.11 release instead of -dev in tests by @Nothing4You in https://github.com/PyMySQL/PyMySQL/pull/1076
 
 
 ## v1.0.2
 
 Release date: 2021-01-09
 
 * Fix `user`, `password`, `host`, `database` are still positional arguments.
```

### Comparing `PyMySQL-1.0.3rc1/LICENSE` & `PyMySQL-1.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMySQL-1.0.3rc1/PKG-INFO` & `PyMySQL-1.1.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMySQL
-Version: 1.0.3rc1
+Version: 1.1.0rc1
 Summary: Pure Python MySQL Driver
 Author-email: Inada Naoki <songofacandy@gmail.com>, Yutaka Matsubara <yutaka.matsubara@gmail.com>
 License: MIT License
 Project-URL: Project, https://github.com/PyMySQL/PyMySQL
 Project-URL: Documentation, https://pymysql.readthedocs.io/
 Keywords: MySQL
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,15 +22,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: rsa
 Provides-Extra: ed25519
 License-File: LICENSE
 
 [![Documentation Status](https://readthedocs.org/projects/pymysql/badge/?version=latest)](https://pymysql.readthedocs.io/)
-[![image](https://coveralls.io/repos/PyMySQL/PyMySQL/badge.svg?branch=main&service=github)](https://coveralls.io/github/PyMySQL/PyMySQL?branch=main)
+[![codecov](https://codecov.io/gh/PyMySQL/PyMySQL/branch/main/graph/badge.svg?token=ppEuaNXBW4)](https://codecov.io/gh/PyMySQL/PyMySQL)
 
 # PyMySQL
 
 This package contains a pure-Python MySQL client library, based on [PEP
 249](https://www.python.org/dev/peps/pep-0249/).
 
 ## Requirements
```

### Comparing `PyMySQL-1.0.3rc1/PyMySQL.egg-info/PKG-INFO` & `PyMySQL-1.1.0rc1/PyMySQL.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMySQL
-Version: 1.0.3rc1
+Version: 1.1.0rc1
 Summary: Pure Python MySQL Driver
 Author-email: Inada Naoki <songofacandy@gmail.com>, Yutaka Matsubara <yutaka.matsubara@gmail.com>
 License: MIT License
 Project-URL: Project, https://github.com/PyMySQL/PyMySQL
 Project-URL: Documentation, https://pymysql.readthedocs.io/
 Keywords: MySQL
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,15 +22,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: rsa
 Provides-Extra: ed25519
 License-File: LICENSE
 
 [![Documentation Status](https://readthedocs.org/projects/pymysql/badge/?version=latest)](https://pymysql.readthedocs.io/)
-[![image](https://coveralls.io/repos/PyMySQL/PyMySQL/badge.svg?branch=main&service=github)](https://coveralls.io/github/PyMySQL/PyMySQL?branch=main)
+[![codecov](https://codecov.io/gh/PyMySQL/PyMySQL/branch/main/graph/badge.svg?token=ppEuaNXBW4)](https://codecov.io/gh/PyMySQL/PyMySQL)
 
 # PyMySQL
 
 This package contains a pure-Python MySQL client library, based on [PEP
 249](https://www.python.org/dev/peps/pep-0249/).
 
 ## Requirements
```

### Comparing `PyMySQL-1.0.3rc1/README.md` & `PyMySQL-1.1.0rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [![Documentation Status](https://readthedocs.org/projects/pymysql/badge/?version=latest)](https://pymysql.readthedocs.io/)
-[![image](https://coveralls.io/repos/PyMySQL/PyMySQL/badge.svg?branch=main&service=github)](https://coveralls.io/github/PyMySQL/PyMySQL?branch=main)
+[![codecov](https://codecov.io/gh/PyMySQL/PyMySQL/branch/main/graph/badge.svg?token=ppEuaNXBW4)](https://codecov.io/gh/PyMySQL/PyMySQL)
 
 # PyMySQL
 
 This package contains a pure-Python MySQL client library, based on [PEP
 249](https://www.python.org/dev/peps/pep-0249/).
 
 ## Requirements
```

### Comparing `PyMySQL-1.0.3rc1/pymysql/__init__.py` & `PyMySQL-1.1.0rc1/pymysql/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -42,20 +42,39 @@
     Time,
     Timestamp,
     DateFromTicks,
     TimeFromTicks,
     TimestampFromTicks,
 )
 
+# PyMySQL version.
+# Used by setuptools and connection_attrs
+VERSION = (1, 1, 0, "rc", 1)
+VERSION_STRING = "1.1.0rc1"
+
+### for mysqlclient compatibility
+### Django checks mysqlclient version.
+version_info = (1, 4, 3, "final", 0)
+__version__ = "1.4.3"
+
+
+def get_client_info():  # for MySQLdb compatibility
+    return __version__
+
+
+def install_as_MySQLdb():
+    """
+    After this function is called, any application that imports MySQLdb
+    will unwittingly actually use pymysql.
+    """
+    sys.modules["MySQLdb"] = sys.modules["pymysql"]
+
+
+# end of mysqlclient compatibility code
 
-VERSION = (1, 0, 3, "rc1")
-if VERSION[3] is not None:
-    VERSION_STRING = "%d.%d.%d_%s" % VERSION
-else:
-    VERSION_STRING = "%d.%d.%d" % VERSION[:3]
 threadsafety = 1
 apilevel = "2.0"
 paramstyle = "pyformat"
 
 from . import connections  # noqa: E402
 
 
@@ -105,42 +124,20 @@
 
 
 def Binary(x):
     """Return x as a binary type."""
     return bytes(x)
 
 
-Connect = connect = Connection = connections.Connection
-
-
-def get_client_info():  # for MySQLdb compatibility
-    version = VERSION
-    if VERSION[3] is None:
-        version = VERSION[:3]
-    return ".".join(map(str, version))
-
-
-# we include a doctored version_info here for MySQLdb compatibility
-version_info = (1, 4, 0, "final", 0)
-
-NULL = "NULL"
-
-__version__ = get_client_info()
-
-
 def thread_safe():
     return True  # match MySQLdb.thread_safe()
 
 
-def install_as_MySQLdb():
-    """
-    After this function is called, any application that imports MySQLdb or
-    _mysql will unwittingly actually use pymysql.
-    """
-    sys.modules["MySQLdb"] = sys.modules["_mysql"] = sys.modules["pymysql"]
+Connect = connect = Connection = connections.Connection
+NULL = "NULL"
 
 
 __all__ = [
     "BINARY",
     "Binary",
     "Connect",
     "Connection",
```

### Comparing `PyMySQL-1.0.3rc1/pymysql/_auth.py` & `PyMySQL-1.1.0rc1/pymysql/_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,16 @@
 def sha2_rsa_encrypt(password, salt, public_key):
     """Encrypt password with salt and public_key.
 
     Used for sha256_password and caching_sha2_password.
     """
     if not _have_cryptography:
         raise RuntimeError(
-            "'cryptography' package is required for sha256_password or caching_sha2_password auth methods"
+            "'cryptography' package is required for sha256_password or"
+            + " caching_sha2_password auth methods"
         )
     message = _xor_password(password + b"\0", salt)
     rsa_key = serialization.load_pem_public_key(public_key, default_backend())
     return rsa_key.encrypt(
         message,
         padding.OAEP(
             mgf=padding.MGF1(algorithm=hashes.SHA1()),
```

### Comparing `PyMySQL-1.0.3rc1/pymysql/charset.py` & `PyMySQL-1.1.0rc1/pymysql/charset.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 class Charset:
     def __init__(self, id, name, collation, is_default):
         self.id, self.name, self.collation = id, name, collation
         self.is_default = is_default == "Yes"
 
     def __repr__(self):
-        return "Charset(id=%s, name=%r, collation=%r)" % (
+        return "Charset(id={}, name={!r}, collation={!r})".format(
             self.id,
             self.name,
             self.collation,
         )
 
     @property
     def encoding(self):
```

### Comparing `PyMySQL-1.0.3rc1/pymysql/connections.py` & `PyMySQL-1.1.0rc1/pymysql/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,17 +104,20 @@
     :param password: Password to use.
     :param database: Database to use, None to not use a particular one.
     :param port: MySQL port to use, default is usually OK. (default: 3306)
     :param bind_address: When the client has multiple network interfaces, specify
         the interface from which to connect to the host. Argument can be
         a hostname or an IP address.
     :param unix_socket: Use a unix socket rather than TCP/IP.
-    :param read_timeout: The timeout for reading from the connection in seconds (default: None - no timeout)
-    :param write_timeout: The timeout for writing to the connection in seconds (default: None - no timeout)
-    :param charset: Charset to use.
+    :param read_timeout: The timeout for reading from the connection in seconds.
+        (default: None - no timeout)
+    :param write_timeout: The timeout for writing to the connection in seconds.
+        (default: None - no timeout)
+    :param str charset: Charset to use.
+    :param str collation: Collation name to use.
     :param sql_mode: Default SQL_MODE to use.
     :param read_default_file:
         Specifies  my.cnf file to read these parameters from under the [client] section.
     :param conv:
         Conversion dictionary to use instead of the default one.
         This is used to provide custom marshalling and unmarshalling of types.
         See converters.
@@ -126,15 +129,16 @@
     :param init_command: Initial SQL statement to run when connection is established.
     :param connect_timeout: The timeout for connecting to the database in seconds.
         (default: 10, min: 1, max: 31536000)
     :param ssl: A dict of arguments similar to mysql_ssl_set()'s parameters or an ssl.SSLContext.
     :param ssl_ca: Path to the file that contains a PEM-formatted CA certificate.
     :param ssl_cert: Path to the file that contains a PEM-formatted client certificate.
     :param ssl_disabled: A boolean value that disables usage of TLS.
-    :param ssl_key: Path to the file that contains a PEM-formatted private key for the client certificate.
+    :param ssl_key: Path to the file that contains a PEM-formatted private key for
+        the client certificate.
     :param ssl_verify_cert: Set to true to check the server certificate's validity.
     :param ssl_verify_identity: Set to true to check the server's identity.
     :param read_default_group: Group to read from in the configuration file.
     :param autocommit: Autocommit mode. None means use server default. (default: False)
     :param local_infile: Boolean to enable the use of LOAD DATA LOCAL command. (default: False)
     :param max_allowed_packet: Max size of packet sent to server in bytes. (default: 16MB)
         Only used to limit size of "LOAD LOCAL INFILE" data packet smaller than default (16KB).
@@ -167,14 +171,15 @@
         user=None,  # The first four arguments is based on DB-API 2.0 recommendation.
         password="",
         host=None,
         database=None,
         unix_socket=None,
         port=0,
         charset="",
+        collation=None,
         sql_mode=None,
         read_default_file=None,
         conv=None,
         use_unicode=True,
         client_flag=0,
         cursorclass=Cursor,
         init_command=None,
@@ -301,14 +306,15 @@
             raise ValueError("read_timeout should be > 0")
         self._read_timeout = read_timeout
         if write_timeout is not None and write_timeout <= 0:
             raise ValueError("write_timeout should be > 0")
         self._write_timeout = write_timeout
 
         self.charset = charset or DEFAULT_CHARSET
+        self.collation = collation
         self.use_unicode = use_unicode
 
         self.encoding = charset_by_name(self.charset).encoding
 
         client_flag |= CLIENT.CAPABILITIES
         if self.db:
             client_flag |= CLIENT.CONNECT_WITH_DB
@@ -335,16 +341,16 @@
         self.max_allowed_packet = max_allowed_packet
         self._auth_plugin_map = auth_plugin_map or {}
         self._binary_prefix = binary_prefix
         self.server_public_key = server_public_key
 
         self._connect_attrs = {
             "_client_name": "pymysql",
-            "_pid": str(os.getpid()),
             "_client_version": VERSION_STRING,
+            "_pid": str(os.getpid()),
         }
 
         if program_name:
             self._connect_attrs["program_name"] = program_name
 
         if defer_connect:
             self._sock = None
@@ -521,23 +527,26 @@
     def escape_string(self, s):
         if self.server_status & SERVER_STATUS.SERVER_STATUS_NO_BACKSLASH_ESCAPES:
             return s.replace("'", "''")
         return converters.escape_string(s)
 
     def _quote_bytes(self, s):
         if self.server_status & SERVER_STATUS.SERVER_STATUS_NO_BACKSLASH_ESCAPES:
-            return "'%s'" % (s.replace(b"'", b"''").decode("ascii", "surrogateescape"),)
+            return "'{}'".format(
+                s.replace(b"'", b"''").decode("ascii", "surrogateescape")
+            )
         return converters.escape_bytes(s)
 
     def cursor(self, cursor=None):
         """
         Create a new cursor to execute queries with.
 
         :param cursor: The type of cursor to create. None means use Cursor.
-        :type cursor: :py:class:`Cursor`, :py:class:`SSCursor`, :py:class:`DictCursor`, or :py:class:`SSDictCursor`.
+        :type cursor: :py:class:`Cursor`, :py:class:`SSCursor`, :py:class:`DictCursor`,
+            or :py:class:`SSDictCursor`.
         """
         if cursor:
             return cursor(self)
         return self.cursorclass(self)
 
     # The following methods are INTERNAL USE ONLY (called from Cursor)
     def query(self, sql, unbuffered=False):
@@ -583,21 +592,40 @@
             if reconnect:
                 self.connect()
                 self.ping(False)
             else:
                 raise
 
     def set_charset(self, charset):
+        """Deprecated. Use set_character_set() instead."""
+        # This function has been implemented in old PyMySQL.
+        # But this name is different from MySQLdb.
+        # So we keep this function for compatibility and add
+        # new set_character_set() function.
+        self.set_character_set(charset)
+
+    def set_character_set(self, charset, collation=None):
+        """
+        Set charaset (and collation)
+
+        Send "SET NAMES charset [COLLATE collation]" query.
+        Update Connection.encoding based on charset.
+        """
         # Make sure charset is supported.
         encoding = charset_by_name(charset).encoding
 
-        self._execute_command(COMMAND.COM_QUERY, "SET NAMES %s" % self.escape(charset))
+        if collation:
+            query = f"SET NAMES {charset} COLLATE {collation}"
+        else:
+            query = f"SET NAMES {charset}"
+        self._execute_command(COMMAND.COM_QUERY, query)
         self._read_packet()
         self.charset = charset
         self.encoding = encoding
+        self.collation = collation
 
     def connect(self, sock=None):
         self._closed = False
         try:
             if sock is None:
                 if self.unix_socket:
                     sock = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
@@ -613,15 +641,15 @@
                         kwargs["source_address"] = (self.bind_address, 0)
                     while True:
                         try:
                             sock = socket.create_connection(
                                 (self.host, self.port), self.connect_timeout, **kwargs
                             )
                             break
-                        except (OSError, IOError) as e:
+                        except OSError as e:
                             if e.errno == errno.EINTR:
                                 continue
                             raise
                     self.host_info = "socket %s:%d" % (self.host, self.port)
                     if DEBUG:
                         print("connected using socket")
                     sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
@@ -631,38 +659,53 @@
             self._sock = sock
             self._rfile = sock.makefile("rb")
             self._next_seq_id = 0
 
             self._get_server_information()
             self._request_authentication()
 
+            # Send "SET NAMES" query on init for:
+            # - Ensure charaset (and collation) is set to the server.
+            #   - collation_id in handshake packet may be ignored.
+            # - If collation is not specified, we don't know what is server's
+            #   default collation for the charset. For example, default collation
+            #   of utf8mb4 is:
+            #   - MySQL 5.7, MariaDB 10.x: utf8mb4_general_ci
+            #   - MySQL 8.0: utf8mb4_0900_ai_ci
+            #
+            # Reference:
+            # - https://github.com/PyMySQL/PyMySQL/issues/1092
+            # - https://github.com/wagtail/wagtail/issues/9477
+            # - https://zenn.dev/methane/articles/2023-mysql-collation (Japanese)
+            self.set_character_set(self.charset, self.collation)
+
             if self.sql_mode is not None:
                 c = self.cursor()
                 c.execute("SET sql_mode=%s", (self.sql_mode,))
+                c.close()
 
             if self.init_command is not None:
                 c = self.cursor()
                 c.execute(self.init_command)
                 c.close()
-                self.commit()
 
             if self.autocommit_mode is not None:
                 self.autocommit(self.autocommit_mode)
         except BaseException as e:
             self._rfile = None
             if sock is not None:
                 try:
                     sock.close()
                 except:  # noqa
                     pass
 
             if isinstance(e, (OSError, IOError)):
                 exc = err.OperationalError(
                     CR.CR_CONN_HOST_ERROR,
-                    "Can't connect to MySQL server on %r (%s)" % (self.host, e),
+                    f"Can't connect to MySQL server on {self.host!r} ({e})",
                 )
                 # Keep original exception and traceback to investigate error.
                 exc.original_exception = e
                 exc.traceback = traceback.format_exc()
                 if DEBUG:
                     print(exc.traceback)
                 raise exc
@@ -731,21 +774,21 @@
 
     def _read_bytes(self, num_bytes):
         self._sock.settimeout(self._read_timeout)
         while True:
             try:
                 data = self._rfile.read(num_bytes)
                 break
-            except (IOError, OSError) as e:
+            except OSError as e:
                 if e.errno == errno.EINTR:
                     continue
                 self._force_close()
                 raise err.OperationalError(
                     CR.CR_SERVER_LOST,
-                    "Lost connection to MySQL server during query (%s)" % (e,),
+                    f"Lost connection to MySQL server during query ({e})",
                 )
             except BaseException:
                 # Don't convert unknown exception to MySQLError.
                 self._force_close()
                 raise
         if len(data) < num_bytes:
             self._force_close()
@@ -754,18 +797,18 @@
             )
         return data
 
     def _write_bytes(self, data):
         self._sock.settimeout(self._write_timeout)
         try:
             self._sock.sendall(data)
-        except IOError as e:
+        except OSError as e:
             self._force_close()
             raise err.OperationalError(
-                CR.CR_SERVER_GONE_ERROR, "MySQL server has gone away (%r)" % (e,)
+                CR.CR_SERVER_GONE_ERROR, f"MySQL server has gone away ({e!r})"
             )
 
     def _read_query_result(self, unbuffered=False):
         self._result = None
         if unbuffered:
             try:
                 result = MySQLResult(self)
@@ -998,15 +1041,15 @@
                             "Authentication plugin '%s'"
                             " %r didn't respond with string. Returned '%r' to prompt %r"
                             % (plugin_name, handler, resp, prompt),
                         )
                 else:
                     raise err.OperationalError(
                         CR.CR_AUTH_PLUGIN_CANNOT_LOAD,
-                        "Authentication plugin '%s' not configured" % (plugin_name,),
+                        f"Authentication plugin '{plugin_name}' not configured",
                     )
                 pkt = self._read_packet()
                 pkt.check_error()
                 if pkt.is_ok_packet() or last:
                     break
             return pkt
         else:
@@ -1224,15 +1267,16 @@
 
     def _check_packet_is_eof(self, packet):
         if not packet.is_eof_packet():
             return False
         # TODO: Support CLIENT.DEPRECATE_EOF
         # 1) Add DEPRECATE_EOF to CAPABILITIES
         # 2) Mask CAPABILITIES with server_capabilities
-        # 3) if server_capabilities & CLIENT.DEPRECATE_EOF: use OKPacketWrapper instead of EOFPacketWrapper
+        # 3) if server_capabilities & CLIENT.DEPRECATE_EOF:
+        #    use OKPacketWrapper instead of EOFPacketWrapper
         wp = EOFPacketWrapper(packet)
         self.warning_count = wp.warning_count
         self.has_next = wp.has_next
         return True
 
     def _read_result_packet(self, first_packet):
         self.field_count = first_packet.read_length_encoded_integer()
@@ -1258,15 +1302,28 @@
         return row
 
     def _finish_unbuffered_query(self):
         # After much reading on the MySQL protocol, it appears that there is,
         # in fact, no way to stop MySQL from sending all the data after
         # executing a query, so we just spin, and wait for an EOF packet.
         while self.unbuffered_active:
-            packet = self.connection._read_packet()
+            try:
+                packet = self.connection._read_packet()
+            except err.OperationalError as e:
+                if e.args[0] in (
+                    ER.QUERY_TIMEOUT,
+                    ER.STATEMENT_TIMEOUT,
+                ):
+                    # if the query timed out we can simply ignore this error
+                    self.unbuffered_active = False
+                    self.connection = None
+                    return
+
+                raise
+
             if self._check_packet_is_eof(packet):
                 self.unbuffered_active = False
                 self.connection = None  # release reference to kill cyclic reference.
 
     def _read_rowdata_packet(self):
         """Read a rowdata packet for each data row in the result set."""
         rows = []
@@ -1348,27 +1405,28 @@
         self.filename = filename
         self.connection = connection
 
     def send_data(self):
         """Send data packets from the local file to the server"""
         if not self.connection._sock:
             raise err.InterfaceError(0, "")
-        conn = self.connection
+        conn: Connection = self.connection
 
         try:
             with open(self.filename, "rb") as open_file:
                 packet_size = min(
                     conn.max_allowed_packet, 16 * 1024
                 )  # 16KB is efficient enough
                 while True:
                     chunk = open_file.read(packet_size)
                     if not chunk:
                         break
                     conn.write_packet(chunk)
-        except IOError:
+        except OSError:
             raise err.OperationalError(
                 ER.FILE_NOT_FOUND,
                 f"Can't find file '{self.filename}'",
             )
         finally:
-            # send the empty packet to signify we are done sending data
-            conn.write_packet(b"")
+            if not conn._closed:
+                # send the empty packet to signify we are done sending data
+                conn.write_packet(b"")
```

### Comparing `PyMySQL-1.0.3rc1/pymysql/converters.py` & `PyMySQL-1.1.0rc1/pymysql/converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,18 @@
     else:
         fmt = "'{0.hour:02}:{0.minute:02}:{0.second:02}'"
     return fmt.format(obj)
 
 
 def escape_datetime(obj, mapping=None):
     if obj.microsecond:
-        fmt = "'{0.year:04}-{0.month:02}-{0.day:02} {0.hour:02}:{0.minute:02}:{0.second:02}.{0.microsecond:06}'"
+        fmt = (
+            "'{0.year:04}-{0.month:02}-{0.day:02}"
+            + " {0.hour:02}:{0.minute:02}:{0.second:02}.{0.microsecond:06}'"
+        )
     else:
         fmt = "'{0.year:04}-{0.month:02}-{0.day:02} {0.hour:02}:{0.minute:02}:{0.second:02}'"
     return fmt.format(obj)
 
 
 def escape_date(obj, mapping=None):
     fmt = "'{0.year:04}-{0.month:02}-{0.day:02}'"
```

### Comparing `PyMySQL-1.0.3rc1/pymysql/cursors.py` & `PyMySQL-1.1.0rc1/pymysql/cursors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+import warnings
 from . import err
 
 
 #: Regular expression for :meth:`Cursor.executemany`.
 #: executemany only supports simple bulk insert.
 #: You can use it to load large dataset.
 RE_INSERT_VALUES = re.compile(
@@ -28,14 +29,15 @@
     #:
     #: Max size of allowed statement is max_allowed_packet - packet_header_size.
     #: Default value of max_allowed_packet is 1048576.
     max_stmt_length = 1024000
 
     def __init__(self, connection):
         self.connection = connection
+        self.warning_count = 0
         self.description = None
         self.rownumber = 0
         self.rowcount = -1
         self.arraysize = 1
         self._executed = None
         self._result = None
         self._rows = None
@@ -91,21 +93,14 @@
         conn.next_result(unbuffered=unbuffered)
         self._do_get_result()
         return True
 
     def nextset(self):
         return self._nextset(False)
 
-    def _ensure_bytes(self, x, encoding=None):
-        if isinstance(x, str):
-            x = x.encode(encoding)
-        elif isinstance(x, (tuple, list)):
-            x = type(x)(self._ensure_bytes(v, encoding=encoding) for v in x)
-        return x
-
     def _escape_args(self, args, conn):
         if isinstance(args, (tuple, list)):
             return tuple(conn.literal(arg) for arg in args)
         elif isinstance(args, dict):
             return {key: conn.literal(val) for (key, val) in args.items()}
         else:
             # If it's not a dictionary let's try escaping it anyways.
@@ -263,15 +258,15 @@
                 "SET %s"
                 % ",".join(
                     fmt % (index, conn.escape(arg)) for index, arg in enumerate(args)
                 )
             )
             self.nextset()
 
-        q = "CALL %s(%s)" % (
+        q = "CALL {}({})".format(
             procname,
             ",".join(["@_%s_%d" % (procname, i) for i in range(len(args))]),
         )
         self._query(q)
         self._executed = q
         return args
 
@@ -284,25 +279,27 @@
         self.rownumber += 1
         return result
 
     def fetchmany(self, size=None):
         """Fetch several rows."""
         self._check_executed()
         if self._rows is None:
+            # Django expects () for EOF.
+            # https://github.com/django/django/blob/0c1518ee429b01c145cf5b34eab01b0b92f8c246/django/db/backends/mysql/features.py#L8
             return ()
         end = self.rownumber + (size or self.arraysize)
         result = self._rows[self.rownumber : end]
         self.rownumber = min(end, len(self._rows))
         return result
 
     def fetchall(self):
         """Fetch all the rows."""
         self._check_executed()
         if self._rows is None:
-            return ()
+            return []
         if self.rownumber:
             result = self._rows[self.rownumber :]
         else:
             result = self._rows
         self.rownumber = len(self._rows)
         return result
 
@@ -327,49 +324,70 @@
         return self.rowcount
 
     def _clear_result(self):
         self.rownumber = 0
         self._result = None
 
         self.rowcount = 0
+        self.warning_count = 0
         self.description = None
         self.lastrowid = None
         self._rows = None
 
     def _do_get_result(self):
         conn = self._get_db()
 
         self._result = result = conn._result
 
         self.rowcount = result.affected_rows
+        self.warning_count = result.warning_count
         self.description = result.description
         self.lastrowid = result.insert_id
         self._rows = result.rows
 
     def __iter__(self):
-        return iter(self.fetchone, None)
+        return self
 
-    Warning = err.Warning
-    Error = err.Error
-    InterfaceError = err.InterfaceError
-    DatabaseError = err.DatabaseError
-    DataError = err.DataError
-    OperationalError = err.OperationalError
-    IntegrityError = err.IntegrityError
-    InternalError = err.InternalError
-    ProgrammingError = err.ProgrammingError
-    NotSupportedError = err.NotSupportedError
+    def __next__(self):
+        row = self.fetchone()
+        if row is None:
+            raise StopIteration
+        return row
+
+    def __getattr__(self, name):
+        # DB-API 2.0 optional extension says these errors can be accessed
+        # via Connection object. But MySQLdb had defined them on Cursor object.
+        if name in (
+            "Warning",
+            "Error",
+            "InterfaceError",
+            "DatabaseError",
+            "DataError",
+            "OperationalError",
+            "IntegrityError",
+            "InternalError",
+            "ProgrammingError",
+            "NotSupportedError",
+        ):
+            # Deprecated since v1.1
+            warnings.warn(
+                "PyMySQL errors hould be accessed from `pymysql` package",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+            return getattr(err, name)
+        raise AttributeError(name)
 
 
 class DictCursorMixin:
     # You can override this to use OrderedDict or other dict-like types.
     dict_type = dict
 
     def _do_get_result(self):
-        super(DictCursorMixin, self)._do_get_result()
+        super()._do_get_result()
         fields = []
         if self.description:
             for f in self._result.fields:
                 name = f.name
                 if name in fields:
                     name = f.table_name + "." + name
                 fields.append(name)
@@ -438,14 +456,15 @@
         return self._conv_row(self._result._read_rowdata_packet_unbuffered())
 
     def fetchone(self):
         """Fetch next row."""
         self._check_executed()
         row = self.read_next()
         if row is None:
+            self.warning_count = self._result.warning_count
             return None
         self.rownumber += 1
         return row
 
     def fetchall(self):
         """
         Fetch all, as per MySQLdb. Pretty useless for large queries, as
@@ -458,30 +477,32 @@
         """
         Fetch all, implemented as a generator, which isn't to standard,
         however, it doesn't make sense to return everything in a list, as that
         would use ridiculous memory for large result sets.
         """
         return iter(self.fetchone, None)
 
-    def __iter__(self):
-        return self.fetchall_unbuffered()
-
     def fetchmany(self, size=None):
         """Fetch many."""
         self._check_executed()
         if size is None:
             size = self.arraysize
 
         rows = []
         for i in range(size):
             row = self.read_next()
             if row is None:
+                self.warning_count = self._result.warning_count
                 break
             rows.append(row)
             self.rownumber += 1
+        if not rows:
+            # Django expects () for EOF.
+            # https://github.com/django/django/blob/0c1518ee429b01c145cf5b34eab01b0b92f8c246/django/db/backends/mysql/features.py#L8
+            return ()
         return rows
 
     def scroll(self, value, mode="relative"):
         self._check_executed()
 
         if mode == "relative":
             if value < 0:
```

### Comparing `PyMySQL-1.0.3rc1/pymysql/err.py` & `PyMySQL-1.1.0rc1/pymysql/err.py`

 * *Files identical despite different names*

### Comparing `PyMySQL-1.0.3rc1/pymysql/optionfile.py` & `PyMySQL-1.1.0rc1/pymysql/optionfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,10 +9,13 @@
     def __remove_quotes(self, value):
         quotes = ["'", '"']
         for quote in quotes:
             if len(value) >= 2 and value[0] == value[-1] == quote:
                 return value[1:-1]
         return value
 
+    def optionxform(self, key):
+        return key.lower().replace("_", "-")
+
     def get(self, section, option):
         value = configparser.RawConfigParser.get(self, section, option)
         return self.__remove_quotes(value)
```

### Comparing `PyMySQL-1.0.3rc1/pymysql/protocol.py` & `PyMySQL-1.1.0rc1/pymysql/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             print("call[%d]: %s (line %d)" % (i, f.f_code.co_name, f.f_lineno))
         print("-" * 66)
     except ValueError:
         pass
     dump_data = [data[i : i + 16] for i in range(0, min(len(data), 256), 16)]
     for d in dump_data:
         print(
-            " ".join("{:02X}".format(x) for x in d)
+            " ".join(f"{x:02X}" for x in d)
             + "   " * (16 - len(d))
             + " " * 2
             + "".join(printable(x) for x in d)
         )
     print("-" * 66)
     print()
 
@@ -271,15 +271,15 @@
     def get_column_length(self):
         if self.type_code == FIELD_TYPE.VAR_STRING:
             mblen = MBLENGTH.get(self.charsetnr, 1)
             return self.length // mblen
         return self.length
 
     def __str__(self):
-        return "%s %r.%r.%r, type=%s, flags=%x" % (
+        return "{} {!r}.{!r}.{!r}, type={}, flags={:x}".format(
             self.__class__,
             self.db,
             self.table_name,
             self.name,
             self.type_code,
             self.flags,
         )
```

### Comparing `PyMySQL-1.0.3rc1/pyproject.toml` & `PyMySQL-1.1.0rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -36,17 +36,28 @@
 ]
 
 [project.urls]
 "Project" = "https://github.com/PyMySQL/PyMySQL"
 "Documentation" = "https://pymysql.readthedocs.io/"
 
 [build-system]
-requires = ["setuptools>=61", "wheel"]
+requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 namespaces = false
-include = ["pymysql"]
+include = ["pymysql*"]
 exclude = ["tests*", "pymysql.tests*"]
 
 [tool.setuptools.dynamic]
 version = {attr = "pymysql.VERSION"}
+
+[tool.ruff]
+line-length = 99
+exclude = [
+    "pymysql/tests/thirdparty",
+]
+
+[tool.pdm.dev-dependencies]
+dev = [
+    "pytest-cov>=4.0.0",
+]
```

### Comparing `PyMySQL-1.0.3rc1/tests/test_auth.py` & `PyMySQL-1.1.0rc1/tests/test_auth.py`

 * *Files identical despite different names*

