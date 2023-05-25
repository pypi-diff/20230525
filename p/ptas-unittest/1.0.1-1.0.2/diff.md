# Comparing `tmp/ptas_unittest-1.0.1-py3-none-any.whl.zip` & `tmp/ptas_unittest-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,8 @@
-Zip file size: 4337 bytes, number of entries: 5
--rw-r--r--  2.0 unx    11501 b- defN 23-May-08 01:34 ptas_unittest/index.py
--rw-r--r--  2.0 unx      221 b- defN 23-May-08 02:54 ptas_unittest-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-08 02:54 ptas_unittest-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-May-08 02:54 ptas_unittest-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      401 b- defN 23-May-08 02:54 ptas_unittest-1.0.1.dist-info/RECORD
-5 files, 12235 bytes uncompressed, 3587 bytes compressed:  70.7%
+Zip file size: 4886 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     6148 b- defN 23-May-25 07:05 .DS_Store
+-rw-r--r--  2.0 unx    11554 b- defN 23-May-25 07:13 ptas_unittest/index.py
+-rw-r--r--  2.0 unx      222 b- defN 23-May-25 07:17 ptas_unittest-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-25 07:17 ptas_unittest-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-May-25 07:17 ptas_unittest-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      467 b- defN 23-May-25 07:17 ptas_unittest-1.0.2.dist-info/RECORD
+6 files, 18503 bytes uncompressed, 4042 bytes compressed:  78.2%
```

## zipnote {}

```diff
@@ -1,16 +1,19 @@
+Filename: .DS_Store
+Comment: 
+
 Filename: ptas_unittest/index.py
 Comment: 
 
-Filename: ptas_unittest-1.0.1.dist-info/METADATA
+Filename: ptas_unittest-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: ptas_unittest-1.0.1.dist-info/WHEEL
+Filename: ptas_unittest-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: ptas_unittest-1.0.1.dist-info/top_level.txt
+Filename: ptas_unittest-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: ptas_unittest-1.0.1.dist-info/RECORD
+Filename: ptas_unittest-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ptas_unittest/index.py

```diff
@@ -29,14 +29,15 @@
 Ui_MainWindow, QtBaseClass = uic.loadUiType(API_UI)
 Ui_PopBox, QtSubClass = uic.loadUiType(dialog)
 
 # form = resource_path("API_UI.ui")
 # form_class = uic.loadUiType(form)[0]
 
 from_class = uic.loadUiType(API_UI)[0]
+from_dialog = uic.loadUiType(dialog)[0]
 BASE_URL = ''
 headers = []
 user_info = []
 status = []
 api = ''
 parameters = ''
 parameters_id = ''
@@ -364,15 +365,15 @@
 
         if info[0] == method_info and info[1] == item:
           self.payload_text.setPlainText(info[2])
     # else:
     #   self.payload_text.clear()
 
 
-class ParmeterDialog(QDialog):
+class ParmeterDialog(QDialog, from_dialog):
   def __init__(self, parent=None):
     super().__init__(parent)
     loadUi("dialog.ui", self)
 
     self.btn_cancel.clicked.connect(self.close)
     self.btn_save.clicked.connect(self.click_save)
```

