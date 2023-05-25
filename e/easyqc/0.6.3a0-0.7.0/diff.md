# Comparing `tmp/easyqc-0.6.3a0.tar.gz` & `tmp/easyqc-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyqc-0.6.3a0.tar", last modified: Mon Mar 21 10:52:22 2022, max compression
+gzip compressed data, was "easyqc-0.7.0.tar", last modified: Thu May 25 16:38:12 2023, max compression
```

## Comparing `easyqc-0.6.3a0.tar` & `easyqc-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2022-03-21 10:52:22.942567 easyqc-0.6.3a0/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1071 2021-04-03 13:59:02.000000 easyqc-0.6.3a0/LICENSE
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     3011 2022-03-21 10:52:22.942567 easyqc-0.6.3a0/PKG-INFO
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     2523 2021-05-11 14:19:23.000000 easyqc-0.6.3a0/README.md
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       38 2022-03-21 10:52:22.942567 easyqc-0.6.3a0/setup.cfg
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      946 2022-03-20 11:08:46.000000 easyqc-0.6.3a0/setup.py
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2022-03-21 10:52:22.938567 easyqc-0.6.3a0/src/
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2022-03-21 10:52:22.942567 easyqc-0.6.3a0/src/easyqc/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)        0 2021-04-03 19:09:46.000000 easyqc-0.6.3a0/src/easyqc/__init__.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     4075 2021-04-10 21:37:23.000000 easyqc-0.6.3a0/src/easyqc/easyqc.svg
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    11473 2022-02-14 08:46:10.000000 easyqc-0.6.3a0/src/easyqc/easyqc.ui
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    23812 2022-03-14 10:35:26.000000 easyqc-0.6.3a0/src/easyqc/gui.py
--rw-r--r--   0 olivier   (1000) olivier   (1000)     2229 2021-05-11 14:19:23.000000 easyqc-0.6.3a0/src/easyqc/pgtools.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1209 2022-02-18 20:43:08.000000 easyqc-0.6.3a0/src/easyqc/qt.py
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2022-03-21 10:52:22.942567 easyqc-0.6.3a0/src/easyqc.egg-info/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     3011 2022-03-21 10:52:22.000000 easyqc-0.6.3a0/src/easyqc.egg-info/PKG-INFO
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      318 2022-03-21 10:52:22.000000 easyqc-0.6.3a0/src/easyqc.egg-info/SOURCES.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)        1 2022-03-21 10:52:22.000000 easyqc-0.6.3a0/src/easyqc.egg-info/dependency_links.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       28 2022-03-21 10:52:22.000000 easyqc-0.6.3a0/src/easyqc.egg-info/requires.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)        7 2022-03-21 10:52:22.000000 easyqc-0.6.3a0/src/easyqc.egg-info/top_level.txt
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-05-25 16:38:12.650714 easyqc-0.7.0/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1071 2022-12-14 14:25:09.000000 easyqc-0.7.0/LICENSE
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     3044 2023-05-25 16:38:12.650714 easyqc-0.7.0/PKG-INFO
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     2595 2023-05-25 16:36:46.000000 easyqc-0.7.0/README.md
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       38 2023-05-25 16:38:12.650714 easyqc-0.7.0/setup.cfg
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      945 2023-05-25 16:35:18.000000 easyqc-0.7.0/setup.py
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-05-25 16:38:12.650714 easyqc-0.7.0/src/
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-05-25 16:38:12.650714 easyqc-0.7.0/src/easyqc/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)        0 2022-12-14 14:25:09.000000 easyqc-0.7.0/src/easyqc/__init__.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     4075 2022-12-14 14:25:09.000000 easyqc-0.7.0/src/easyqc/easyqc.svg
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    12525 2022-12-14 14:25:09.000000 easyqc-0.7.0/src/easyqc/easyqc.ui
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)    24716 2023-05-25 16:34:13.000000 easyqc-0.7.0/src/easyqc/gui.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     2229 2022-12-14 14:25:09.000000 easyqc-0.7.0/src/easyqc/pgtools.py
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     1209 2022-12-14 14:25:09.000000 easyqc-0.7.0/src/easyqc/qt.py
+drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2023-05-25 16:38:12.650714 easyqc-0.7.0/src/easyqc.egg-info/
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)     3044 2023-05-25 16:38:12.000000 easyqc-0.7.0/src/easyqc.egg-info/PKG-INFO
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)      318 2023-05-25 16:38:12.000000 easyqc-0.7.0/src/easyqc.egg-info/SOURCES.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)        1 2023-05-25 16:38:12.000000 easyqc-0.7.0/src/easyqc.egg-info/dependency_links.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)       36 2023-05-25 16:38:12.000000 easyqc-0.7.0/src/easyqc.egg-info/requires.txt
+-rw-rw-r--   0 olivier   (1000) olivier   (1000)        7 2023-05-25 16:38:12.000000 easyqc-0.7.0/src/easyqc.egg-info/top_level.txt
```

### Comparing `easyqc-0.6.3a0/LICENSE` & `easyqc-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easyqc-0.6.3a0/PKG-INFO` & `easyqc-0.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: easyqc
-Version: 0.6.3a0
+Version: 0.7.0
 Summary: Seismic viewer for numpy
 Home-page: https://github.com/oliche/easyqc
 Author: Olivier Winter
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/oliche/easyqc/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -22,14 +20,15 @@
 NB: if you use `ipython` use the `%gui qt` magic command before !
 
 ### Keyboard Shortcuts
 -   **ctrl + A**: increase display gain by +3dB 
 -   **ctrl + Z**: deacrease display gain by +3dB
 -   **ctrl + P**: take screenshot to clipboard
 -   **ctrl + P**: propagates display accross all windows (same window size, same axis, same gain)
+-   **ctrl + S**: captures screenshot of the plot area in the clipboard
 -   **up/down/right/left arrows**: pan using keyboard
 
 ### Minimum working example to display a numpy array.
 
 ```python
 import numpy as np
 import scipy.signal
@@ -106,9 +105,7 @@
 Test wheel:
 ```shell
 virtualenv easyqc --python=3.8
 source ./easyqc/bin/activate
 pip install easyqc
 #pip install -i https://test.pypi.org/simple/ easyqc  # doesnt' seem to install deps
 ```
-
-
```

### Comparing `easyqc-0.6.3a0/README.md` & `easyqc-0.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 NB: if you use `ipython` use the `%gui qt` magic command before !
 
 ### Keyboard Shortcuts
 -   **ctrl + A**: increase display gain by +3dB 
 -   **ctrl + Z**: deacrease display gain by +3dB
 -   **ctrl + P**: take screenshot to clipboard
 -   **ctrl + P**: propagates display accross all windows (same window size, same axis, same gain)
+-   **ctrl + S**: captures screenshot of the plot area in the clipboard
 -   **up/down/right/left arrows**: pan using keyboard
 
 ### Minimum working example to display a numpy array.
 
 ```python
 import numpy as np
 import scipy.signal
```

### Comparing `easyqc-0.6.3a0/setup.py` & `easyqc-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     require = [x.strip() for x in f.readlines() if not x.startswith('git+')]
 
 setuptools.setup(
     name="easyqc",
-    version="0.6.3a",
+    version="0.7.0",
     author="Olivier Winter",
     description="Seismic viewer for numpy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/oliche/easyqc",
     project_urls={
         "Bug Tracker": "https://github.com/oliche/easyqc/issues",
```

### Comparing `easyqc-0.6.3a0/src/easyqc/easyqc.svg` & `easyqc-0.7.0/src/easyqc/easyqc.svg`

 * *Files identical despite different names*

### Comparing `easyqc-0.6.3a0/src/easyqc/easyqc.ui` & `easyqc-0.7.0/src/easyqc/easyqc.ui`

 * *Files 2% similar despite different names*

#### Comparing `easyqc-0.6.3a0/src/easyqc/easyqc.ui` & `easyqc-0.7.0/src/easyqc/easyqc.ui`

```diff
@@ -374,28 +374,64 @@
           <bool>false</bool>
         </property>
         <property name="title">
           <string>File</string>
         </property>
         <addaction name="actionopen"/>
       </widget>
+      <widget class="QMenu" name="menuView">
+        <property name="title">
+          <string>View</string>
+        </property>
+        <widget class="QMenu" name="menuColormaps">
+          <property name="title">
+            <string>Colormaps</string>
+          </property>
+          <addaction name="actionColormap_CET_L2"/>
+          <addaction name="actionColormap_MPL_PuOr"/>
+          <addaction name="actionColormap_CET_D1"/>
+          <addaction name="actionColormap_CET_D6"/>
+        </widget>
+        <addaction name="menuColormaps"/>
+      </widget>
       <addaction name="menufile"/>
+      <addaction name="menuView"/>
     </widget>
     <widget class="QStatusBar" name="statusbar"/>
     <action name="actionopen">
       <property name="enabled">
         <bool>true</bool>
       </property>
       <property name="text">
         <string>open</string>
       </property>
       <property name="visible">
         <bool>true</bool>
       </property>
     </action>
+    <action name="actionColormap_CET_L2">
+      <property name="text">
+        <string>Gray (CET-L2)</string>
+      </property>
+    </action>
+    <action name="actionColormap_MPL_PuOr">
+      <property name="text">
+        <string>PuOr</string>
+      </property>
+    </action>
+    <action name="actionColormap_CET_D1">
+      <property name="text">
+        <string>Blue White Red (CET-D1)</string>
+      </property>
+    </action>
+    <action name="actionColormap_CET_D6">
+      <property name="text">
+        <string>Blue Black Red (CET-D6)</string>
+      </property>
+    </action>
   </widget>
   <customwidgets>
     <customwidget>
       <class>PlotWidget</class>
       <extends>QGraphicsView</extends>
       <header>pyqtgraph</header>
     </customwidget>
```

### Comparing `easyqc-0.6.3a0/src/easyqc/gui.py` & `easyqc-0.7.0/src/easyqc/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         background_color = self.palette().color(self.backgroundRole())
         # init the seismic density display
         self.plotItem_seismic.setAspectLocked(False)
         self.imageItem_seismic = pg.ImageItem()
         self.plotItem_seismic.setBackground(background_color)
         self.plotItem_seismic.addItem(self.imageItem_seismic)
         self.viewBox_seismic = self.plotItem_seismic.getPlotItem().getViewBox()
+        self._init_menu()
         self._init_cmenu()
         # init the header display and link X and Y axis with density display
         self.plotDataItem_header_h = pg.PlotDataItem()
         self.plotItem_header_h.addItem(self.plotDataItem_header_h)
         self.plotItem_seismic.setXLink(self.plotItem_header_h)
         self.plotDataItem_header_v = pg.PlotDataItem()
         self.plotItem_header_h.setBackground(background_color)
@@ -78,14 +79,21 @@
         self.lineEdit_gain.returnPressed.connect(self.editGain)
         self.lineEdit_sort.returnPressed.connect(self.editSort)
         self.comboBox_header.activated[str].connect(self.ctrl.set_header)
         self.viewBox_seismic.sigRangeChanged.connect(self.on_sigRangeChanged)
         self.horizontalScrollBar.sliderMoved.connect(self.on_horizontalSliderChange)
         self.verticalScrollBar.sliderMoved.connect(self.on_verticalSliderChange)
 
+    def _init_menu(self):
+        # pre-defined colormaps
+        self.actionColormap_CET_D6.triggered.connect(lambda: self.setColorMap('CET-D6'))
+        self.actionColormap_CET_D1.triggered.connect(lambda: self.setColorMap('CET-D1'))
+        self.actionColormap_CET_L2.triggered.connect(lambda: self.setColorMap('CET-L2'))
+        self.actionColormap_MPL_PuOr.triggered.connect(lambda: self.setColorMap('PuOr'))
+
     def _init_cmenu(self):
         """
         Setup context menus - on instantiation only
         """
         self.viewBox_seismic.scene().contextMenu = None  # this gets rid of the export context menu
         self.plotItem_seismic.plotItem.ctrlMenu = None  # this gets rid of the plot context menu
         for act in self.viewBox_seismic.menu.actions():
@@ -131,15 +139,15 @@
             self.ctrl.propagate()
         # arrows keys move seismic
         elif k in (QtCore.Qt.Key_Up, QtCore.Qt.Key_Left, QtCore.Qt.Key_Right, QtCore.Qt.Key_Down):
             self.translate_seismic(k, m == QtCore.Qt.ControlModifier)
         # ctrl + s: screenshot to clipboard
         elif m == QtCore.Qt.ControlModifier and k == QtCore.Qt.Key_S:
             qtapp = QtWidgets.QApplication.instance()
-            qtapp.clipboard().setPixmap(self.grab())
+            qtapp.clipboard().setPixmap(self.plotItem_seismic.grab())
 
     def editGain(self):
         self.ctrl.set_gain()
 
     def editSort(self):
         keys = self.lineEdit_sort.text().split(' ')
         self.ctrl.sort(keys)
@@ -246,14 +254,24 @@
 
     def cmenu_ViewSpectrum(self):
         self._cmenu_hover('Spectrum')
 
     def cmenu_ViewSpectrogram(self):
         self._cmenu_hover('Spectrogram', image=True)
 
+    def setColorMap(self, cmap):
+        """
+        Set the colormap for the seismic display - useful for the propagation feature
+        :param cmap:
+        :return:
+        """
+        if isinstance(cmap, str) and cmap not in pg.colormap.listMaps():
+            cmap = pg.colormap.getFromMatplotlib(cmap)
+        self.imageItem_seismic.setColorMap(cmap)
+
 
 class Controller:
 
     def __init__(self, view):
         self.view = view
         self.model = Model(None, None)
         self.order = None
@@ -316,14 +334,15 @@
         eqcs = self.view._instances()
         if len(eqcs) == 1:
             return
         for i, eqc in enumerate(eqcs):
             if eqc is self.view:
                 continue
             else:
+                eqc.setColorMap(self.view.imageItem_seismic.getColorMap() or 'CET-L2')
                 eqc.setGeometry(self.view.geometry())
                 eqc.ctrl.set_gain(self.gain)
                 eqc.plotItem_seismic.setXLink(self.view.plotItem_seismic)
                 eqc.plotItem_seismic.setYLink(self.view.plotItem_seismic)
                 # eqc.plotItem_seismic.setXLink(eqc.plotItem_header_h)
                 # eqc.plotItem_seismic.setYLink(eqc.plotItem_header_v)
                 # also propagate sorting
```

### Comparing `easyqc-0.6.3a0/src/easyqc/pgtools.py` & `easyqc-0.7.0/src/easyqc/pgtools.py`

 * *Files identical despite different names*

### Comparing `easyqc-0.6.3a0/src/easyqc/qt.py` & `easyqc-0.7.0/src/easyqc/qt.py`

 * *Files identical despite different names*

### Comparing `easyqc-0.6.3a0/src/easyqc.egg-info/PKG-INFO` & `easyqc-0.7.0/src/easyqc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: easyqc
-Version: 0.6.3a0
+Version: 0.7.0
 Summary: Seismic viewer for numpy
 Home-page: https://github.com/oliche/easyqc
 Author: Olivier Winter
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/oliche/easyqc/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -22,14 +20,15 @@
 NB: if you use `ipython` use the `%gui qt` magic command before !
 
 ### Keyboard Shortcuts
 -   **ctrl + A**: increase display gain by +3dB 
 -   **ctrl + Z**: deacrease display gain by +3dB
 -   **ctrl + P**: take screenshot to clipboard
 -   **ctrl + P**: propagates display accross all windows (same window size, same axis, same gain)
+-   **ctrl + S**: captures screenshot of the plot area in the clipboard
 -   **up/down/right/left arrows**: pan using keyboard
 
 ### Minimum working example to display a numpy array.
 
 ```python
 import numpy as np
 import scipy.signal
@@ -106,9 +105,7 @@
 Test wheel:
 ```shell
 virtualenv easyqc --python=3.8
 source ./easyqc/bin/activate
 pip install easyqc
 #pip install -i https://test.pypi.org/simple/ easyqc  # doesnt' seem to install deps
 ```
-
-
```

