# Comparing `tmp/ntdsdotsqlite-0.9.5.tar.gz` & `tmp/ntdsdotsqlite-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntdsdotsqlite-0.9.5.tar", max compression
+gzip compressed data, was "ntdsdotsqlite-0.9.6.tar", max compression
```

## Comparing `ntdsdotsqlite-0.9.5.tar` & `ntdsdotsqlite-0.9.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0        0 2023-04-24 19:34:15.811658 ntdsdotsqlite-0.9.5/ntdsdotsqlite/__init__.py
--rw-r--r--   0        0        0      854 2023-05-08 16:23:21.892529 ntdsdotsqlite-0.9.5/ntdsdotsqlite/__main__.py
--rw-r--r--   0        0        0     5134 2023-05-10 17:20:33.263014 ntdsdotsqlite-0.9.5/ntdsdotsqlite/accounts.py
--rw-r--r--   0        0        0     1454 2023-05-08 09:43:59.572323 ntdsdotsqlite-0.9.5/ntdsdotsqlite/containers.py
--rw-r--r--   0        0        0     4145 2023-05-06 15:44:55.688794 ntdsdotsqlite-0.9.5/ntdsdotsqlite/decrypt.py
--rw-r--r--   0        0        0     3089 2023-05-08 21:09:08.053917 ntdsdotsqlite-0.9.5/ntdsdotsqlite/domain.py
--rw-r--r--   0        0        0      905 2023-05-08 13:52:27.251046 ntdsdotsqlite-0.9.5/ntdsdotsqlite/groups.py
--rw-r--r--   0        0        0      320 2023-05-08 21:09:14.178994 ntdsdotsqlite-0.9.5/ntdsdotsqlite/links.py
--rw-r--r--   0        0        0     2726 2023-05-08 15:41:39.616697 ntdsdotsqlite-0.9.5/ntdsdotsqlite/model.sql
--rw-r--r--   0        0        0     4644 2023-05-10 17:08:18.055714 ntdsdotsqlite-0.9.5/ntdsdotsqlite/ntdsdotsqlite.py
--rw-r--r--   0        0        0     1595 2023-05-08 09:44:10.802061 ntdsdotsqlite-0.9.5/ntdsdotsqlite/orga_units.py
--rw-r--r--   0        0        0    26966 2023-05-09 20:30:13.020077 ntdsdotsqlite-0.9.5/ntdsdotsqlite/secretsdump.py
--rw-r--r--   0        0        0     5851 2023-05-09 20:32:50.342772 ntdsdotsqlite-0.9.5/ntdsdotsqlite/utils.py
--rw-r--r--   0        0        0      695 2023-05-10 17:21:14.997394 ntdsdotsqlite-0.9.5/pyproject.toml
--rw-r--r--   0        0        0     2005 2023-05-08 16:12:51.277756 ntdsdotsqlite-0.9.5/README.md
--rw-r--r--   0        0        0     2775 1970-01-01 00:00:00.000000 ntdsdotsqlite-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-24 19:34:15.811658 ntdsdotsqlite-0.9.6/ntdsdotsqlite/__init__.py
+-rw-r--r--   0        0        0      854 2023-05-08 16:23:21.892529 ntdsdotsqlite-0.9.6/ntdsdotsqlite/__main__.py
+-rw-r--r--   0        0        0     5305 2023-05-25 17:10:04.235334 ntdsdotsqlite-0.9.6/ntdsdotsqlite/accounts.py
+-rw-r--r--   0        0        0     1454 2023-05-08 09:43:59.572323 ntdsdotsqlite-0.9.6/ntdsdotsqlite/containers.py
+-rw-r--r--   0        0        0     4145 2023-05-06 15:44:55.688794 ntdsdotsqlite-0.9.6/ntdsdotsqlite/decrypt.py
+-rw-r--r--   0        0        0     3089 2023-05-08 21:09:08.053917 ntdsdotsqlite-0.9.6/ntdsdotsqlite/domain.py
+-rw-r--r--   0        0        0      905 2023-05-08 13:52:27.251046 ntdsdotsqlite-0.9.6/ntdsdotsqlite/groups.py
+-rw-r--r--   0        0        0      320 2023-05-08 21:09:14.178994 ntdsdotsqlite-0.9.6/ntdsdotsqlite/links.py
+-rw-r--r--   0        0        0     2958 2023-05-25 17:11:24.932653 ntdsdotsqlite-0.9.6/ntdsdotsqlite/model.sql
+-rw-r--r--   0        0        0     5104 2023-05-25 17:13:31.077881 ntdsdotsqlite-0.9.6/ntdsdotsqlite/ntdsdotsqlite.py
+-rw-r--r--   0        0        0     1769 2023-05-25 17:14:27.627333 ntdsdotsqlite-0.9.6/ntdsdotsqlite/orga_units.py
+-rw-r--r--   0        0        0    26966 2023-05-09 20:30:13.020077 ntdsdotsqlite-0.9.6/ntdsdotsqlite/secretsdump.py
+-rw-r--r--   0        0        0     2178 2023-05-25 17:13:23.481309 ntdsdotsqlite-0.9.6/ntdsdotsqlite/trusts.py
+-rw-r--r--   0        0        0     6185 2023-05-25 17:13:16.795269 ntdsdotsqlite-0.9.6/ntdsdotsqlite/utils.py
+-rw-r--r--   0        0        0      695 2023-05-25 18:12:55.859839 ntdsdotsqlite-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0     2005 2023-05-08 16:12:51.277756 ntdsdotsqlite-0.9.6/README.md
+-rw-r--r--   0        0        0     2775 1970-01-01 00:00:00.000000 ntdsdotsqlite-0.9.6/PKG-INFO
```

### Comparing `ntdsdotsqlite-0.9.5/ntdsdotsqlite/__main__.py` & `ntdsdotsqlite-0.9.6/ntdsdotsqlite/__main__.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.5/ntdsdotsqlite/accounts.py` & `ntdsdotsqlite-0.9.6/ntdsdotsqlite/accounts.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,19 @@
         cur = sqlite_db.cursor()
         parent_dnt = a.get("PDNT_col")
         res = cur.execute(f"SELECT dn FROM organizational_units WHERE id={parent_dnt}")
         res = res.fetchone()
         if res is None:
             res = cur.execute(f"SELECT dn FROM containers WHERE id={parent_dnt}")
             res = res.fetchone()
-        account["dn"] = "CN=" + escape_dn_chars(account["commonname"]) + "," + res[0]
+        if res:
+            account["dn"] = "CN=" + escape_dn_chars(account["commonname"]) + "," + res[0]
+        else:
+            print(f"Warning: The DN for the account {account['commonname']} could not be computed")
+            account["dn"] = None
         primaryGroup = a.get(ese_db.column_names["primaryGroupID"])
         if primaryGroup:
             res = cur.execute(f"SELECT id, SID from groups WHERE SID LIKE '%-{primaryGroup}'")
             res = res.fetchone()
             account["primaryGroup"] = res[0]
         else:
             account["primaryGroup"] = None
```

### Comparing `ntdsdotsqlite-0.9.5/ntdsdotsqlite/containers.py` & `ntdsdotsqlite-0.9.6/ntdsdotsqlite/containers.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.5/ntdsdotsqlite/decrypt.py` & `ntdsdotsqlite-0.9.6/ntdsdotsqlite/decrypt.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.5/ntdsdotsqlite/domain.py` & `ntdsdotsqlite-0.9.6/ntdsdotsqlite/domain.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.5/ntdsdotsqlite/groups.py` & `ntdsdotsqlite-0.9.6/ntdsdotsqlite/groups.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.5/ntdsdotsqlite/model.sql` & `ntdsdotsqlite-0.9.6/ntdsdotsqlite/model.sql`

 * *Files 6% similar despite different names*

```diff
@@ -111,8 +111,19 @@
     id INTEGER PRIMARY KEY,
     name TEXT,
     description TEXT,
     commonname TEXT,
     parent INTEGER,
     dn TEXT,
     isDeleted BOOLEAN
-);
+);
+
+CREATE TABLE trusted_domains (
+    id INTEGER PRIMARY KEY,
+    commonname TEXT,
+    name TEXT,
+    trustAttributes INTEGER,
+    trustDirection TEXT,
+    trustPartner TEXT,
+    trustType TEXT,
+    attributeFlags JSON
+ );
```

### Comparing `ntdsdotsqlite-0.9.5/ntdsdotsqlite/ntdsdotsqlite.py` & `ntdsdotsqlite-0.9.6/ntdsdotsqlite/ntdsdotsqlite.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from ntdsdotsqlite.utils import create_database, get_ESE_column_names
 from ntdsdotsqlite.containers import containers_generator
 from ntdsdotsqlite.accounts import account_generator
 from ntdsdotsqlite.domain import get_domain_objects
 from ntdsdotsqlite.orga_units import ou_generator
 from ntdsdotsqlite.decrypt import decrypt_sqlite
+from ntdsdotsqlite.trusts import trust_generator
 from ntdsdotsqlite.groups import group_generator
 from ntdsdotsqlite.links import compute_links
 from dissect.esedb import EseDB
 import sqlite3
 import json
 
 
@@ -107,13 +108,24 @@
         :supplementalCredentials, :lmPwdHistory, :ntPwdHistory, :accountExpires,
         :uac_flags, :parent, :dn, :isDeleted, :primaryGroup, :links,
         :isDisabled
         )
     """
     cursor.executemany(stmt, machines_iter)
     sqlite_db.commit()
+    # Insert trust information
+    print("Retrieving trust information with other domains...")
+    trusts_iter = trust_generator(ese_db)
+    stmt = """
+        INSERT INTO trusted_domains VALUES (
+        :id, :commonname, :name, :trustAttributes, :trustDirection, :trustPartner, :trustType,
+        :attributeFlags
+        )
+    """
+    cursor.executemany(stmt, trusts_iter)
+    sqlite_db.commit()
     if system_path:
         print("Decrypting stuff with SYSTEM hive ...")
         decrypt_sqlite(sqlite_db, ese_path, system_path)
     if sqlite_db:
         sqlite_db.close()
     fd.close()
```

### Comparing `ntdsdotsqlite-0.9.5/ntdsdotsqlite/orga_units.py` & `ntdsdotsqlite-0.9.6/ntdsdotsqlite/orga_units.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,13 +29,17 @@
         dn_prefix = "OU=" + escape_dn_chars(ou_object["name"])
         cur_object = ou
         while True:
             parent_dnt = cur_object.get("PDNT_col")
             # if $ROOT_OBJECT" is reached or the current object is not an OU anymore
             if parent_dnt == domain_id:
                 break
-            parent = ous[parent_dnt]
+            try:
+                parent = ous[parent_dnt]
+            except KeyError:
+                print(f"Warning: the OU {ou_object['name']} has a missing parent in its path...")
+                break
             cur_object = parent
             name = parent.get(ese_db.column_names["name"])
             dn_prefix += "," + "OU=" + escape_dn_chars(name)
         ou_object["dn"] = f"{dn_prefix},{dn_suffix}"
         yield ou_object
```

### Comparing `ntdsdotsqlite-0.9.5/ntdsdotsqlite/secretsdump.py` & `ntdsdotsqlite-0.9.6/ntdsdotsqlite/secretsdump.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.5/ntdsdotsqlite/utils.py` & `ntdsdotsqlite-0.9.6/ntdsdotsqlite/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -105,14 +105,27 @@
             (guid := row.get("ATTk589972")) and
             guid.hex() == sguid
         ):
             return row.get("DNT_col"), row
     return None, None
 
 
+class TRUST_FLAGS(IntFlag):
+    NON_TRANSITIVE = 0x1
+    UPLEVEL_ONLY = 0x2
+    QUARANTINED_DOMAIN = 0x4
+    FOREST_TRANSITIVE = 0x8
+    CROSS_ORGANIZATION = 0x10
+    WITHIN_FOREST = 0x20
+    TREAT_AS_EXTERNAL = 0x40
+    USES_RC4_ENCRYPTION = 0x80
+    CROSS_ORGANIZATION_NO_TGT_DELEGATION = 0x200
+    PIM_TRUST = 0x400
+
+
 class UAC_FLAGS(IntFlag):
     SCRIPT = 0x0001
     ACCOUNTDISABLE = 0x0002
     HOMEDIR_REQUIRED = 0x0008
     LOCKOUT = 0x0010
     PASSWD_NOTREQD = 0x0020
     PASSWD_CANT_CHANGE = 0x0040
```

### Comparing `ntdsdotsqlite-0.9.5/pyproject.toml` & `ntdsdotsqlite-0.9.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ntdsdotsqlite"
-version = "0.9.5"
+version = "0.9.6"
 description = "A small utility to get an SQLite  database from an NTDS.DIT file."
 authors = ["Virgile Jarry <virgile@mailbox.org>"]
 readme = "README.md"
 license = "Beerware"
 homepage = "https://github.com/almandin/ntdsdotsqlite"
 repository = "https://github.com/almandin/ntdsdotsqlite"
 documentation = "https://github.com/almandin/ntdsdotsqlite/README.md"
```

### Comparing `ntdsdotsqlite-0.9.5/README.md` & `ntdsdotsqlite-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.5/PKG-INFO` & `ntdsdotsqlite-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntdsdotsqlite
-Version: 0.9.5
+Version: 0.9.6
 Summary: A small utility to get an SQLite  database from an NTDS.DIT file.
 Home-page: https://github.com/almandin/ntdsdotsqlite
 License: Beerware
 Author: Virgile Jarry
 Author-email: virgile@mailbox.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

