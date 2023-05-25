# Comparing `tmp/itkdb_gtk-0.0.6.tar.gz` & `tmp/itkdb_gtk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itkdb_gtk-0.0.6.tar", last modified: Mon May 15 11:02:03 2023, max compression
+gzip compressed data, was "itkdb_gtk-0.0.7.tar", last modified: Thu May 25 15:35:02 2023, max compression
```

## Comparing `itkdb_gtk-0.0.6.tar` & `itkdb_gtk-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-15 11:02:03.171526 itkdb_gtk-0.0.6/
--rw-r--r--   0 lacasta    (503) staff       (20)     2499 2023-05-15 11:02:03.171124 itkdb_gtk-0.0.6/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)     1997 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.6/README.md
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-15 11:02:03.164464 itkdb_gtk-0.0.6/itkdb_gtk/
--rw-r--r--   0 lacasta    (503) staff       (20)    12294 2023-05-11 14:03:05.000000 itkdb_gtk-0.0.6/itkdb_gtk/GlueWeight.py
--rw-r--r--   0 lacasta    (503) staff       (20)      172 2023-04-21 15:44:09.000000 itkdb_gtk-0.0.6/itkdb_gtk/ITkDB.desktop
--rw-r--r--   0 lacasta    (503) staff       (20)    23991 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.6/itkdb_gtk/ITkDB.svg
--rw-r--r--   0 lacasta    (503) staff       (20)     9902 2023-03-21 10:25:38.000000 itkdb_gtk-0.0.6/itkdb_gtk/ITkDBlogin.py
--rw-r--r--   0 lacasta    (503) staff       (20)    14208 2023-05-11 14:04:07.000000 itkdb_gtk-0.0.6/itkdb_gtk/ITkDButils.py
--rw-r--r--   0 lacasta    (503) staff       (20)      552 2023-04-11 16:04:01.000000 itkdb_gtk-0.0.6/itkdb_gtk/__init__.py
--rw-r--r--   0 lacasta    (503) staff       (20)     3342 2023-04-13 14:46:29.000000 itkdb_gtk-0.0.6/itkdb_gtk/checkComponent.py
--rw-r--r--   0 lacasta    (503) staff       (20)     1432 2023-05-11 13:27:56.000000 itkdb_gtk-0.0.6/itkdb_gtk/checkJSon.py
--rw-r--r--   0 lacasta    (503) staff       (20)     4375 2023-05-11 14:02:42.000000 itkdb_gtk-0.0.6/itkdb_gtk/dashBoard.py
--rw-r--r--   0 lacasta    (503) staff       (20)    20708 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.6/itkdb_gtk/dbGtkUtils.py
--rw-r--r--   0 lacasta    (503) staff       (20)    18718 2023-04-11 15:15:43.000000 itkdb_gtk-0.0.6/itkdb_gtk/getShipments.py
--rw-r--r--   0 lacasta    (503) staff       (20)     7140 2023-04-11 15:50:48.000000 itkdb_gtk-0.0.6/itkdb_gtk/groundingTest.py
--rw-r--r--   0 lacasta    (503) staff       (20)    19401 2023-04-11 15:22:03.000000 itkdb_gtk-0.0.6/itkdb_gtk/readAVSdata.py
--rw-r--r--   0 lacasta    (503) staff       (20)     2679 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.6/itkdb_gtk/readGoogleSheet.py
--rw-r--r--   0 lacasta    (503) staff       (20)    13133 2023-04-11 15:22:19.000000 itkdb_gtk-0.0.6/itkdb_gtk/sendShipments.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)    21093 2023-04-11 15:23:27.000000 itkdb_gtk-0.0.6/itkdb_gtk/uploadPetalInformation.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)    13689 2023-05-15 10:52:22.000000 itkdb_gtk-0.0.6/itkdb_gtk/uploadTest.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-15 11:02:03.170466 itkdb_gtk-0.0.6/itkdb_gtk.egg-info/
--rw-r--r--   0 lacasta    (503) staff       (20)     2499 2023-05-15 11:02:03.000000 itkdb_gtk-0.0.6/itkdb_gtk.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      654 2023-05-15 11:02:03.000000 itkdb_gtk-0.0.6/itkdb_gtk.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-05-15 11:02:03.000000 itkdb_gtk-0.0.6/itkdb_gtk.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      239 2023-05-15 11:02:03.000000 itkdb_gtk-0.0.6/itkdb_gtk.egg-info/entry_points.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       62 2023-05-15 11:02:03.000000 itkdb_gtk-0.0.6/itkdb_gtk.egg-info/requires.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       10 2023-05-15 11:02:03.000000 itkdb_gtk-0.0.6/itkdb_gtk.egg-info/top_level.txt
--rw-r--r--   0 lacasta    (503) staff       (20)     1087 2023-05-15 11:01:53.000000 itkdb_gtk-0.0.6/pyproject.toml
--rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-05-15 11:02:03.171638 itkdb_gtk-0.0.6/setup.cfg
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-25 15:35:02.215579 itkdb_gtk-0.0.7/
+-rw-r--r--   0 lacasta    (503) staff       (20)     2689 2023-05-25 15:35:02.215180 itkdb_gtk-0.0.7/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)     2187 2023-05-24 15:05:26.000000 itkdb_gtk-0.0.7/README.md
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-25 15:35:02.211917 itkdb_gtk-0.0.7/itkdb_gtk/
+-rw-r--r--   0 lacasta    (503) staff       (20)    12294 2023-05-11 14:03:05.000000 itkdb_gtk-0.0.7/itkdb_gtk/GlueWeight.py
+-rw-r--r--   0 lacasta    (503) staff       (20)      172 2023-04-21 15:44:09.000000 itkdb_gtk-0.0.7/itkdb_gtk/ITkDB.desktop
+-rw-r--r--   0 lacasta    (503) staff       (20)    23991 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.7/itkdb_gtk/ITkDB.svg
+-rw-r--r--   0 lacasta    (503) staff       (20)     9902 2023-03-21 10:25:38.000000 itkdb_gtk-0.0.7/itkdb_gtk/ITkDBlogin.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    14824 2023-05-25 13:27:59.000000 itkdb_gtk-0.0.7/itkdb_gtk/ITkDButils.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     4693 2023-05-24 15:19:53.000000 itkdb_gtk-0.0.7/itkdb_gtk/ShowAttachments.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     2989 2023-05-24 13:13:04.000000 itkdb_gtk-0.0.7/itkdb_gtk/ShowComments.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     3329 2023-05-24 13:24:38.000000 itkdb_gtk-0.0.7/itkdb_gtk/ShowDefects.py
+-rw-r--r--   0 lacasta    (503) staff       (20)      691 2023-05-25 15:34:56.000000 itkdb_gtk-0.0.7/itkdb_gtk/__init__.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     3731 2023-05-24 13:12:38.000000 itkdb_gtk-0.0.7/itkdb_gtk/checkComponent.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     1432 2023-05-11 13:27:56.000000 itkdb_gtk-0.0.7/itkdb_gtk/checkJSon.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     4412 2023-05-25 15:33:11.000000 itkdb_gtk-0.0.7/itkdb_gtk/dashBoard.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    20713 2023-05-24 14:24:41.000000 itkdb_gtk-0.0.7/itkdb_gtk/dbGtkUtils.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    18718 2023-04-11 15:15:43.000000 itkdb_gtk-0.0.7/itkdb_gtk/getShipments.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     7142 2023-05-24 13:24:49.000000 itkdb_gtk-0.0.7/itkdb_gtk/groundingTest.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    19401 2023-04-11 15:22:03.000000 itkdb_gtk-0.0.7/itkdb_gtk/readAVSdata.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     2679 2023-03-21 10:15:51.000000 itkdb_gtk-0.0.7/itkdb_gtk/readGoogleSheet.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    13133 2023-04-11 15:22:19.000000 itkdb_gtk-0.0.7/itkdb_gtk/sendShipments.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)    19659 2023-05-25 15:33:19.000000 itkdb_gtk-0.0.7/itkdb_gtk/uploadMultipleTests.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)    22252 2023-05-24 13:37:58.000000 itkdb_gtk-0.0.7/itkdb_gtk/uploadPetalInformation.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)    12154 2023-05-24 16:04:02.000000 itkdb_gtk-0.0.7/itkdb_gtk/uploadTest.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-05-25 15:35:02.214600 itkdb_gtk-0.0.7/itkdb_gtk.egg-info/
+-rw-r--r--   0 lacasta    (503) staff       (20)     2689 2023-05-25 15:35:02.000000 itkdb_gtk-0.0.7/itkdb_gtk.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      767 2023-05-25 15:35:02.000000 itkdb_gtk-0.0.7/itkdb_gtk.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-05-25 15:35:02.000000 itkdb_gtk-0.0.7/itkdb_gtk.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      291 2023-05-25 15:35:02.000000 itkdb_gtk-0.0.7/itkdb_gtk.egg-info/entry_points.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       62 2023-05-25 15:35:02.000000 itkdb_gtk-0.0.7/itkdb_gtk.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       10 2023-05-25 15:35:02.000000 itkdb_gtk-0.0.7/itkdb_gtk.egg-info/top_level.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)     1141 2023-05-25 15:30:22.000000 itkdb_gtk-0.0.7/pyproject.toml
+-rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-05-25 15:35:02.215713 itkdb_gtk-0.0.7/setup.cfg
```

### Comparing `itkdb_gtk-0.0.6/PKG-INFO` & `itkdb_gtk-0.0.7/itkdb_gtk.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: itkdb_gtk
-Version: 0.0.6
+Name: itkdb-gtk
+Version: 0.0.7
 Summary: A collection of Gtk based GUI to access ITkDB.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -36,14 +36,18 @@
 the petal core in the DB, if not yet there, make the assembly of the components,
 and uploadas the test runs made at AVS.
 
 ## uploadTest.py
 A GUI to upload the JSON files corresponding to a test and, also, to add
 attachmetns.
 
+## uploadMultipleTests.py
+This will allow to select various test files, or even scan a whole directory to
+find them, and assign comments, defects or attachments to each of the tests found.
+
 ## getShipments.py
 Find all shipments to be received at a given site and list them. It handles a
 barcode reader that helps identifying the items actually received for the
 reception. It will finally make the DB aware of the items receptioned.
 
 ## sendShipments.py
 Create a new shipment. Allows to add items with the QR reader as well as from a
```

### Comparing `itkdb_gtk-0.0.6/README.md` & `itkdb_gtk-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 the petal core in the DB, if not yet there, make the assembly of the components,
 and uploadas the test runs made at AVS.
 
 ## uploadTest.py
 A GUI to upload the JSON files corresponding to a test and, also, to add
 attachmetns.
 
+## uploadMultipleTests.py
+This will allow to select various test files, or even scan a whole directory to
+find them, and assign comments, defects or attachments to each of the tests found.
+
 ## getShipments.py
 Find all shipments to be received at a given site and list them. It handles a
 barcode reader that helps identifying the items actually received for the
 reception. It will finally make the DB aware of the items receptioned.
 
 ## sendShipments.py
 Create a new shipment. Allows to add items with the QR reader as well as from a
```

### Comparing `itkdb_gtk-0.0.6/itkdb_gtk/GlueWeight.py` & `itkdb_gtk-0.0.7/itkdb_gtk/GlueWeight.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.6/itkdb_gtk/ITkDB.svg` & `itkdb_gtk-0.0.7/itkdb_gtk/ITkDB.svg`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.6/itkdb_gtk/ITkDBlogin.py` & `itkdb_gtk-0.0.7/itkdb_gtk/ITkDBlogin.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.6/itkdb_gtk/ITkDButils.py` & `itkdb_gtk-0.0.7/itkdb_gtk/ITkDButils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 
 # define an Attachment object.
 class Attachment(object):
     """Encapsulates Attachment information."""
 
     def __init__(self, path=None, title=None, desc=None):
         """Initialization."""
-        self.path = path
+        if path is not None:
+            self.path = Path(path).expanduser().resolve()
+        else:
+            self.path = None
+
         self.title = title
         self.desc = desc
 
 
 def is_iterable(obj):
     """Tell if an object is iterable. Strings are not considered iterables."""
     if isinstance(obj, Iterable):
@@ -202,28 +206,50 @@
 
     except Exception as e:
         print("Problems assemblying {} into {}:\n\t{}".format(
             child, parent, str(e)))
         return None
 
 
+def set_object_stage(client, SN, stage):
+    """Set stage of object
+
+    Args:
+    ----
+        client: DB session
+        SN: Serial number
+        stage: Stage
+
+    """
+    global db_response
+    try:
+        db_response = client.post("setComponentStage",
+                                  json={"component": SN, "stage": stage})
+        return db_response
+
+    except Exception as e:
+        print("Problems changing stage of {} into {}:\n\t{}".format(
+            SN, stage, str(e)))
+        return None
+
+
 def get_DB_component(client, SN):
     """Get ta component by its serial number."""
     global db_response
     db_response = client.get('getComponent', json={'component': SN})
     return db_response
 
 
 def upload_test(client, data, attachments=None):
     """Upload a test to the DB.
 
     Args:
     ----
         client: The DB client
-        data (dict): A distionary with all the elements of thee test.
+        data (dict): A dictionary with all the elements of thee test.
         attachments (Attachments): one or more (in a list) Attachments to the test
 
     Return:
     ------
         resp: The response of the DB session.
 
     """
```

### Comparing `itkdb_gtk-0.0.6/itkdb_gtk/checkComponent.py` & `itkdb_gtk-0.0.7/itkdb_gtk/checkComponent.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-"""Check childre of DB component."""
+"""Check children of DB component."""
 
 try:
     import readAVSdata
     import ITkDBlogin
     import ITkDButils
 
     from dbGtkUtils import replace_in_container, complain, DictDialog, ask_for_confirmation
@@ -60,30 +60,37 @@
     Args:
     -----
         child (): object
 
     Returns
     -------
         str: object type
-        
+
     """
     if child["type"] is not None:
         ctype = child["type"]["code"]
     else:
         ctype = child["componentType"]["code"]
-        
+
     return ctype
 
 
 def main():
     """Main entry point."""
     # ITk_PB authentication
     dlg = ITkDBlogin.ITkDBlogin()
     session = dlg.get_client()
 
+    final_stage = {
+        "BT_PETAL_FRONT": "COMPLETED",
+        "BT_PETAL_BACK": "COMPLETED",
+        "COOLING_LOOP_PETAL": "CLINCORE",
+        "THERMALFOAMSET_PETAL": "IN_CORE"
+    }
+
     # find all cores
     # Now all the objects
     payload = {
         "componentType": ["BT"],
         "componentType": ["CORE_PETAL"],
         "type": ["CORE_AVS"],
     }
@@ -112,20 +119,25 @@
                 clist.append((ctype, cstage, None, None))
 
             else:
                 SN = child["component"]["serialNumber"]
                 ctype = get_type(child)
                 cobj = ITkDButils.get_DB_component(session, SN)
                 cstage = cobj["currentStage"]['code']
+                if cstage != final_stage[ctype]:
+                    rc = ITkDButils.set_object_stage(session, SN, final_stage[ctype])
+                    if rc is not None:
+                        cstage = final_stage[ctype]
+
                 clocation = cobj["currentLocation"]['code']
                 clist.append((ctype, cstage, SN, clocation))
 
         for item in clist:
             print("\t{} [{}] - {} at {}".format(item[2], item[0], item[1], item[3]))
-            
+
         print()
 
     dlg.die()
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `itkdb_gtk-0.0.6/itkdb_gtk/checkJSon.py` & `itkdb_gtk-0.0.7/itkdb_gtk/checkJSon.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.6/itkdb_gtk/dashBoard.py` & `itkdb_gtk-0.0.7/itkdb_gtk/dashBoard.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 try:
     import dbGtkUtils
     import getShipments
     import groundingTest
     import ITkDBlogin
     import sendShipments
-    import uploadTest
+    import uploadMultipleTests
     import GlueWeight
 
 except Exception:
-    from itkdb_gtk import dbGtkUtils, getShipments, groundingTest, ITkDBlogin, sendShipments, uploadTest, GlueWeight
+    from itkdb_gtk import dbGtkUtils, getShipments, groundingTest, ITkDBlogin, sendShipments, uploadMultipleTests, GlueWeight
 
 import gi
 
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
 
 
@@ -42,15 +42,15 @@
         irow = 0
         lbl = Gtk.Label()
         lbl.set_markup("<b>Tests</b>")
         lbl.set_xalign(0)
         grid.attach(lbl, 0, irow, 1, 1)
 
         irow += 1
-        btnTest = Gtk.Button(label="Upload Test (json)")
+        btnTest = Gtk.Button(label="Upload Tests (json)")
         btnTest.connect("clicked", self.upload_test)
         grid.attach(btnTest, 0, irow, 1, 1)
 
         btnGnd = Gtk.Button(label="Petal VI/GND")
         btnGnd.connect("clicked", self.petal_gnd)
         grid.attach(btnGnd, 1, irow, 1, 1)
 
@@ -85,15 +85,15 @@
         """Launch upload test."""
         bitn = 1
         bt = 1 << bitn
         if self.mask & bt:
             return
 
         self.mask |= bt
-        W = uploadTest.UploadTest(self.session)
+        W = uploadMultipleTests.UploadMultipleTests(self.session)
         W.connect("destroy", self.app_closed, bitn)
 
     def create_shipment(self, *args):
         """Launch sendShipment."""
         bitn = 2
         bt = 1 << bitn
         if self.mask & bt:
```

### Comparing `itkdb_gtk-0.0.6/itkdb_gtk/dbGtkUtils.py` & `itkdb_gtk-0.0.7/itkdb_gtk/dbGtkUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,15 +371,15 @@
         self.hide()
         self.destroy()
 
     def query_db(self, *args):
         """Search button clicked."""
         pass
 
-    def new_login(self, msg):
+    def new_login(self, obj, msg):
         """A new user logged in."""
         if msg == "<OK>":
             self.session = self.session.user_gui.get_client()
             self.userLabel.get_child().set_text(self.session.user.name)
 
         else:
             self.write_message("Could not login.\n{}".format(msg))
```

### Comparing `itkdb_gtk-0.0.6/itkdb_gtk/getShipments.py` & `itkdb_gtk-0.0.7/itkdb_gtk/getShipments.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.6/itkdb_gtk/groundingTest.py` & `itkdb_gtk-0.0.7/itkdb_gtk/groundingTest.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,14 +192,15 @@
         if rc is not None:
             dbGtkUtils.complain("Could not upload test", rc)
 
         else:
             dbGtkUtils.ask_for_confirmation("Test uploaded.",
                                             "{} - {}".format(values["component"], values["testType"]))
 
+
 def main():
     """Main entry."""
     # DB login
     dlg = ITkDBlogin.ITkDBlogin()
     client = dlg.get_client()
     if client is None:
         print("Could not connect to DB with provided credentials.")
@@ -218,8 +219,8 @@
     except KeyboardInterrupt:
         print("Arrrgggg!!!")
 
     dlg.die()
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `itkdb_gtk-0.0.6/itkdb_gtk/readAVSdata.py` & `itkdb_gtk-0.0.7/itkdb_gtk/readAVSdata.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.6/itkdb_gtk/readGoogleSheet.py` & `itkdb_gtk-0.0.7/itkdb_gtk/readGoogleSheet.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.6/itkdb_gtk/sendShipments.py` & `itkdb_gtk-0.0.7/itkdb_gtk/sendShipments.py`

 * *Files identical despite different names*

### Comparing `itkdb_gtk-0.0.6/itkdb_gtk/uploadPetalInformation.py` & `itkdb_gtk-0.0.7/itkdb_gtk/uploadPetalInformation.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     import ITkDButils
 
     from dbGtkUtils import replace_in_container, complain, DictDialog, ask_for_confirmation
 
 except ModuleNotFoundError:
     from itkdb_gtk import readAVSdata, ITkDBlogin, ITkDButils
     from itkdb_gtk.dbGtkUtils import replace_in_container, complain, DictDialog, ask_for_confirmation
-    
+
 
 def create_scrolled_dictdialog(the_dict, hidden=("component", "testType")):
     """Create a DictDialog within a scrolled window.
 
     Return:
     ------
         scrolled: the scrolled window
@@ -36,14 +36,34 @@
     gM = DictDialog(the_dict, hidden)
     scrolled = Gtk.ScrolledWindow()
     scrolled.set_policy(Gtk.PolicyType.NEVER, Gtk.PolicyType.AUTOMATIC)
     scrolled.add(gM)
     return scrolled, gM
 
 
+def get_type(child):
+    """Return object type
+
+    Args:
+    -----
+        child (): object
+
+    Returns
+    -------
+        str: object type
+
+    """
+    if child["type"] is not None:
+        ctype = child["type"]["code"]
+    else:
+        ctype = child["componentType"]["code"]
+
+    return ctype
+
+
 class AVSPanel(Gtk.Window):
     """Dialog for interaction with DB."""
 
     def __init__(self, session, options):
         """Initialization."""
         super().__init__(title="Upload AVS Data")
         self.db_session = session
@@ -447,14 +467,20 @@
 
         comp_map = {
             "BT_PETAL_FRONT": "FacingFront",
             "BT_PETAL_BACK": "FacingBack",
             "COOLING_LOOP_PETAL": "CoolingLoop",
             "THERMALFOAMSET_PETAL": "AllcompSet"
         }
+        final_stage = {
+            "BT_PETAL_FRONT": "COMPLETED",
+            "BT_PETAL_BACK": "COMPLETED",
+            "COOLING_LOOP_PETAL": "CLINCORE",
+            "THERMALFOAMSET_PETAL": "IN_CORE"
+        }
         missing = []
         for child in self.petal_core["children"]:
             if child["component"] is None:
                 if child["type"] is not None:
                     ctype = child["type"]["code"]
                 else:
                     ctype = child["componentType"]["code"]
@@ -483,14 +509,26 @@
                                                            "HC_ID",
                                                            components["HoneyCombSet"])
                     if rc is None:
                         error_txt.append("Problems setting HoneCombSet ID.\n")
 
                     break
 
+            # Check the final stage of the assembled objects
+            for child in self.petal_core["children"]:
+                if child["component"]:
+                    cSN = child["component"]["serialNumber"]
+                    ctype = get_type(child)
+                    cobj = ITkDButils.get_DB_component(session, cSN)
+                    cstage = cobj["currentStage"]['code']
+                    if cstage != final_stage[ctype]:
+                        rc = ITkDButils.set_object_stage(session, cSN, final_stage[ctype])
+                        if rc is None:
+                            print("Could not set final stage of {}".format(cSN))
+
             if len(error_txt):
                 complain("Assembly of {} could not be completeed:".format(this_petal),
                          "\n".join(error_txt))
 
     def upload_current_test(self, *args):
         """Called with upload button clcked."""
         SN = self.SN.get_text()
```

### Comparing `itkdb_gtk-0.0.6/itkdb_gtk/uploadTest.py` & `itkdb_gtk-0.0.7/itkdb_gtk/uploadTest.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,25 +5,50 @@
 import sys
 from pathlib import Path
 
 try:
     import dbGtkUtils
     import ITkDBlogin
     import ITkDButils
+    from ShowComments import ShowComments
+    from ShowAttachments import ShowAttachments
+    from ShowDefects import ShowDefects
+
 except ModuleNotFoundError:
     from itkdb_gtk import dbGtkUtils, ITkDBlogin, ITkDButils
+    from itkdb_gtk.ShowComments import ShowComments
+    from itkdb_gtk.ShowAttachments import ShowAttachments
+    from itkdb_gtk.ShowDefects import ShowDefects
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk, Gio
 
 # Check if Gtk can be open
 gtk_runs, gtk_args = Gtk.init_check()
 
 
+def create_json_data_editor(data):
+    """Create a dialog to show the JSon file."""
+    dlg = Gtk.Dialog(title="Test Data")
+    dlg.add_buttons(Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL,
+                    Gtk.STOCK_OK, Gtk.ResponseType.OK)
+
+    dlg.set_property("height-request", 500)
+    box = dlg.get_content_area()
+    value = dbGtkUtils.DictDialog(data)
+    scrolled = Gtk.ScrolledWindow()
+    scrolled.set_policy(Gtk.PolicyType.NEVER, Gtk.PolicyType.AUTOMATIC)
+    scrolled.add(value)
+    box.pack_start(scrolled, True, True, 10)
+
+    dlg.show_all()
+    return value, dlg
+
+
 def check_data(data):
     """Checks validity of JSon data.
 
     Args:
     ----
         data (): The json data
 
@@ -50,29 +75,31 @@
         errors.append("Need some test results")
         missing.append("results")
 
     return errors, missing
 
 
 class UploadTest(dbGtkUtils.ITkDBWindow):
-    """Collects informatio to upload a test and its attachments."""
+    """Collects information to upload a test and its attachments."""
 
     def __init__(self, session, payload=None, attachment=None):
         """Initialization.
 
         Args:
         ----
             session: ITkDB session
             payload: path of test file
             attachment: an Attachment object.
 
         """
         self.payload = payload
         self.data = None
         self.attachments = []
+        self.comments = []
+        self.defects = []
         if attachment is not None:
             if isinstance(attachment, ITkDButils.Attachment):
                 if attachment.path is not None:
                     self.attachments.append(attachment)
             else:
                 print("Wrong attachment: {}".format(attachment))
 
@@ -108,23 +135,14 @@
         grid.attach(lbl, 0, 0, 1, 1)
 
         self.testF = Gtk.FileChooserButton()
         self.testF.set_tooltip_text("Click to select JSon test file.")
 
         grid.attach(self.testF, 1, 0, 1, 1)
         self.testF.connect("file-set", self.on_test_file)
-        if self.payload:
-            the_path = Path(self.payload).expanduser().resolve()
-            if the_path.exists():
-                ifile = Path(self.payload).expanduser().resolve().as_posix()
-                self.testF.set_filename(ifile)
-                self.on_test_file(self.testF)
-
-            else:
-                print("Input file does not exists: {}".format(self.payload))
 
         # This is to show/edit the test file data
         btn = Gtk.Button()
         icon = Gio.ThemedIcon(name="view-paged-symbolic")
         image = Gtk.Image.new_from_gicon(icon, Gtk.IconSize.BUTTON)
         btn.add(image)
         btn.set_tooltip_text("Click to view/edit test data.")
@@ -146,64 +164,51 @@
 
         self.entryTest = Gtk.Entry()
         grid.attach(self.entryTest, 1, 2, 1, 1)
 
         # The "Add attachment" button.
         box = Gtk.Box(orientation=Gtk.Orientation.HORIZONTAL)
         self.mainBox.pack_start(box, False, False, 0)
-
-        dbGtkUtils.add_button_to_container(box, "Add attachment",
-                                           "Click to add a new attachment.",
-                                           self.add_attachment)
-
-        dbGtkUtils.add_button_to_container(box, "Remove attachment",
-                                           "Click to remove selected attachment.",
-                                           self.remove_attachment)
+        dbGtkUtils.add_button_to_container(box, "Attachments",
+                                           "Click to edit attachments.",
+                                           self.edit_attachments)
+
+        dbGtkUtils.add_button_to_container(box, "Comments",
+                                           "Click to edit comments.",
+                                           self.edit_comments)
+
+        dbGtkUtils.add_button_to_container(box, "Defects",
+                                           "Click to edit defects.",
+                                           self.edit_defects)
 
         dbGtkUtils.add_button_to_container(box, "Upload Test",
                                            "Click to upload test.",
                                            self.upload_test_gui)
 
-        # Paned object
-        paned = Gtk.Paned(orientation=Gtk.Orientation.VERTICAL)
-        paned.set_size_request(-1, 200)
-        self.mainBox.pack_start(paned, True, True, 0)
-
-        # the list of attachments
-        tree_view = self.create_tree_view()
-        paned.add1(tree_view)
-
         # The text view
         frame = self.create_text_view()
-        paned.add2(frame)
+        self.mainBox.pack_start(frame, True, True, 0)
 
         self.show_all()
 
-    def create_tree_view(self, size=150):
-        """Creates the tree vew with the attachments."""
-        model = Gtk.ListStore(str, str, str, str)
-        self.tree = Gtk.TreeView(model=model)
-        scrolled = Gtk.ScrolledWindow()
-        scrolled.set_policy(Gtk.PolicyType.NEVER, Gtk.PolicyType.AUTOMATIC)
-        scrolled.add(self.tree)
-        scrolled.set_size_request(-1, size)
-
-        renderer = Gtk.CellRendererText()
-        column = Gtk.TreeViewColumn("Attachment", renderer, text=0)
-        self.tree.append_column(column)
-
-        renderer = Gtk.CellRendererText()
-        column = Gtk.TreeViewColumn("Title", renderer, text=1)
-        self.tree.append_column(column)
-
-        renderer = Gtk.CellRendererText()
-        column = Gtk.TreeViewColumn("Description", renderer, text=2)
-        self.tree.append_column(column)
+        if self.payload:
+            the_path = Path(self.payload).expanduser().resolve()
+            if the_path.exists():
+                ifile = Path(self.payload).expanduser().resolve().as_posix()
+                self.testF.set_filename(ifile)
+                self.on_test_file(self.testF)
+
+            else:
+                print("Input file does not exists: {}".format(self.payload))
 
-        return scrolled
+        if len(self.attachments):
+            dC = [A for A in self.attachments]
+            self.attachments.clear()
+            for A in dC:
+                self.append_attachment_to_view(A)
 
     def get_test_institute(self):
         """Select an institue."""
         dlg = Gtk.Dialog(title="Select Institution.", flags=0)
         dlg.add_buttons(Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL,
                         Gtk.STOCK_OK, Gtk.ResponseType.OK)
         area = dlg.get_content_area()
@@ -246,125 +251,77 @@
                         self.write_message("Setting Institution to {}\n".format(self.data["institution"]))
 
                 else:
                     dbGtkUtils.complain("Invalid JSON file\n{}".format('\n'.join(errors)), fnam)
 
             self.entrySN.set_text(self.data["component"])
             self.entryTest.set_text(self.data["testType"])
+            self.comments = self.data.get("comments", [])
+            self.defects = self.data.get("defects", [])
 
         except Exception as E:
             self.data = None
             self.write_message("Cannot load file {}\n".format(fnam))
             self.write_message("{}\n".format(str(E)))
 
     def show_data(self, *args):
         """Show data button clicked."""
         if self.data is None:
             return
 
-        dlg = Gtk.Dialog(title="Test Data")
-        dlg.add_buttons(Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL,
-                        Gtk.STOCK_OK, Gtk.ResponseType.OK)
-
-        dlg.set_property("height-request", 500)
-        box = dlg.get_content_area()
-        value = dbGtkUtils.DictDialog(self.data)
-        scrolled = Gtk.ScrolledWindow()
-        scrolled.set_policy(Gtk.PolicyType.NEVER, Gtk.PolicyType.AUTOMATIC)
-        scrolled.add(value)
-        box.pack_start(scrolled, True, True, 10)
-
-        dlg.show_all()
-
+        value, dlg = create_json_data_editor(self.data)
         rc = dlg.run()
         if rc == Gtk.ResponseType.OK:
             self.data = value.values
 
         dlg.hide()
         dlg.destroy()
 
-    def add_attachment_dialog(self):
-        """Create the add attachment dialog."""
-        dlg = Gtk.Dialog(title="Add Attachment")
-        dlg.add_buttons(Gtk.STOCK_CANCEL, Gtk.ResponseType.CANCEL,
-                        Gtk.STOCK_OK, Gtk.ResponseType.OK)
-        grid = Gtk.Grid(column_spacing=5, row_spacing=1)
-        box = dlg.get_content_area()
-        box.add(grid)
-
-        lbl = Gtk.Label(label="File")
-        lbl.set_xalign(0)
-        grid.attach(lbl, 0, 0, 1, 1)
-
-        lbl = Gtk.Label(label="Title")
-        lbl.set_xalign(0)
-        grid.attach(lbl, 0, 1, 1, 1)
-
-        lbl = Gtk.Label(label="Description")
-        lbl.set_xalign(0)
-        grid.attach(lbl, 0, 2, 1, 1)
-
-        dlg.fC = Gtk.FileChooserButton()
-        grid.attach(dlg.fC, 1, 0, 1, 1)
-
-        dlg.att_title = Gtk.Entry()
-        grid.attach(dlg.att_title, 1, 1, 1, 1)
-
-        dlg.att_desc = Gtk.Entry()
-        grid.attach(dlg.att_desc, 1, 2, 1, 1)
-
-        dlg.show_all()
-        return dlg
-
-    def add_attachment(self, *args):
-        """Add Attachment button clicked."""
-        dlg = self.add_attachment_dialog()
-        rc = dlg.run()
-        model = self.tree.get_model()
+    def edit_attachments(self, *args):
+        """Edit test attachmetns."""
+        SA = ShowAttachments("Test Attachments", self.session, self.attachments, parent=self)
+        response = SA.run()
+        if response == Gtk.ResponseType.OK:
+            self.attachments = SA.attachments
+
+        SA.hide()
+        SA.destroy()
+
+    def edit_comments(self, *args):
+        """Edit test comments."""
+        SC = ShowComments("Test Comments", self.comments, self)
+        rc = SC.run()
         if rc == Gtk.ResponseType.OK:
-            path = Path(dlg.fC.get_filename())
-            name = path.name
-            T = dlg.att_title.get_text().strip()
-            D = dlg.att_desc.get_text().strip()
-            model.append([name, T, D, path.as_posix()])
-
-            T = T if len(T) else None
-            D = D if len(D) else None
-            att = ITkDButils.Attachment(path.as_posix(), T, D)
-            self.attachments.append(att)
+            self.comments = SC.comments
 
-        dlg.hide()
-        dlg.destroy()
+        SC.hide()
+        SC.destroy()
 
-    def remove_attachment(self, *args):
-        """Remove selected attachment."""
-        select = self.tree.get_selection()
-        model, iter = select.get_selected()
-        if iter:
-            values = model[iter]
-            for a in self.attachments:
-                if a.path == values[3]:
-                    rc = dbGtkUtils.ask_for_confirmation("Remove this attachment ?",
-                                                         "{} - {}\n{}".format(a.title, a.desc, values[0]))
-                    if rc:
-                        self.attachments.remove(a)
-                        model.remove(iter)
+    def edit_defects(self, *args):
+        """Edit test defects."""
+        SD = ShowDefects("Test Defects", self.defects, self)
+        rc = SD.run()
+        if rc == Gtk.ResponseType.OK:
+            self.defects = SD.defects
 
-                    break
+        SD.hide()
+        SD.destroy()
 
     def upload_test_gui(self, *args):
         """Uploads test and attachments."""
         self.upload_test()
 
     def upload_test(self):
         """Uploads test and attachments."""
         if self.data is None:
             self.write_message("No data available to upload\n")
             return
 
+        self.data["comments"] = self.comments
+        self.data["defects"] = self.defects
         rc = ITkDButils.upload_test(self.session, self.data, self.attachments)
         if rc:
             ipos = rc.find("The following details may help:")
             msg = rc[ipos:]
             dbGtkUtils.complain("Failed uploading test", msg)
 
         else:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `itkdb_gtk-0.0.6/itkdb_gtk.egg-info/PKG-INFO` & `itkdb_gtk-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: itkdb-gtk
-Version: 0.0.6
+Name: itkdb_gtk
+Version: 0.0.7
 Summary: A collection of Gtk based GUI to access ITkDB.
 Author-email: Carlos Lacasta <carlos.lacasta@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itk-pdb-gtk-gui-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -36,14 +36,18 @@
 the petal core in the DB, if not yet there, make the assembly of the components,
 and uploadas the test runs made at AVS.
 
 ## uploadTest.py
 A GUI to upload the JSON files corresponding to a test and, also, to add
 attachmetns.
 
+## uploadMultipleTests.py
+This will allow to select various test files, or even scan a whole directory to
+find them, and assign comments, defects or attachments to each of the tests found.
+
 ## getShipments.py
 Find all shipments to be received at a given site and list them. It handles a
 barcode reader that helps identifying the items actually received for the
 reception. It will finally make the DB aware of the items receptioned.
 
 ## sendShipments.py
 Create a new shipment. Allows to add items with the QR reader as well as from a
```

### Comparing `itkdb_gtk-0.0.6/itkdb_gtk.egg-info/SOURCES.txt` & `itkdb_gtk-0.0.7/itkdb_gtk.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 README.md
 pyproject.toml
 itkdb_gtk/GlueWeight.py
 itkdb_gtk/ITkDB.desktop
 itkdb_gtk/ITkDB.svg
 itkdb_gtk/ITkDBlogin.py
 itkdb_gtk/ITkDButils.py
+itkdb_gtk/ShowAttachments.py
+itkdb_gtk/ShowComments.py
+itkdb_gtk/ShowDefects.py
 itkdb_gtk/__init__.py
 itkdb_gtk/checkComponent.py
 itkdb_gtk/checkJSon.py
 itkdb_gtk/dashBoard.py
 itkdb_gtk/dbGtkUtils.py
 itkdb_gtk/getShipments.py
 itkdb_gtk/groundingTest.py
 itkdb_gtk/readAVSdata.py
 itkdb_gtk/readGoogleSheet.py
 itkdb_gtk/sendShipments.py
+itkdb_gtk/uploadMultipleTests.py
 itkdb_gtk/uploadPetalInformation.py
 itkdb_gtk/uploadTest.py
 itkdb_gtk.egg-info/PKG-INFO
 itkdb_gtk.egg-info/SOURCES.txt
 itkdb_gtk.egg-info/dependency_links.txt
 itkdb_gtk.egg-info/entry_points.txt
 itkdb_gtk.egg-info/requires.txt
```

### Comparing `itkdb_gtk-0.0.6/pyproject.toml` & `itkdb_gtk-0.0.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "itkdb_gtk"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@cern.ch" },
 ]
 description = "A collection of Gtk based GUI to access ITkDB."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
@@ -27,14 +27,15 @@
 [project.gui-scripts]
 itkdb_dashBoard = "itkdb_gtk:dash_board"
 getShipments = "itkdb_gtk:getShipments"
 glueWeight = "itkdb_gtk:glueWeight"
 groundingTest = "itkdb_gtk:groundingTest"
 sendShipments = "itkdb_gtk:sendShipments"
 uploadTest = "itkdb_gtk:uploadTest"
+uploadMultipleTests = "itkdb_gtk:uploadMultipleTests"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.package-data]
 itkdb_gtk = ["*.desktop", "*.svg"]
```

