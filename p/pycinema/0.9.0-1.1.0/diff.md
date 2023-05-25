# Comparing `tmp/pycinema-0.9.0.tar.gz` & `tmp/pycinema-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycinema-0.9.0.tar", last modified: Wed Feb  8 21:45:28 2023, max compression
+gzip compressed data, was "pycinema-1.1.0.tar", last modified: Thu May 25 20:44:10 2023, max compression
```

## Comparing `pycinema-0.9.0.tar` & `pycinema-1.1.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2023-02-08 21:45:28.799007 pycinema-0.9.0/
--rw-r--r--   0 dhr      (24423) staff       (20)      574 2023-02-08 21:45:28.798861 pycinema-0.9.0/PKG-INFO
-drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2023-02-08 21:45:28.792307 pycinema-0.9.0/doc/
--rw-r--r--   0 dhr      (24423) staff       (20)      195 2023-02-06 16:41:51.000000 pycinema-0.9.0/doc/description.md
-drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2023-02-08 21:45:28.797723 pycinema-0.9.0/pycinema/
--rw-r--r--   0 dhr      (24423) staff       (20)     3493 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/Annotation.py
--rw-r--r--   0 dhr      (24423) staff       (20)     1283 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/Border.py
--rw-r--r--   0 dhr      (24423) staff       (20)     1016 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/CinemaDatabaseReader.py
--rw-r--r--   0 dhr      (24423) staff       (20)     4201 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/CinemaDatabaseViewer.py
--rw-r--r--   0 dhr      (24423) staff       (20)     3783 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/CinemaDatabaseWriter.py
--rw-r--r--   0 dhr      (24423) staff       (20)     3756 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/ColorMapping.py
--rw-r--r--   0 dhr      (24423) staff       (20)     4353 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/ColorMappingWidgets.py
--rw-r--r--   0 dhr      (24423) staff       (20)      323 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/ColorSource.py
--rw-r--r--   0 dhr      (24423) staff       (20)     4376 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/Core.py
--rw-r--r--   0 dhr      (24423) staff       (20)     1876 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/DatabaseQuery.py
--rw-r--r--   0 dhr      (24423) staff       (20)     6897 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/DemoScene.py
--rw-r--r--   0 dhr      (24423) staff       (20)     4688 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/DepthCompositing.py
--rw-r--r--   0 dhr      (24423) staff       (20)     1060 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/ImageCanny.py
--rw-r--r--   0 dhr      (24423) staff       (20)     1092 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/ImageConvert.py
--rw-r--r--   0 dhr      (24423) staff       (20)     2421 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/ImageReader.py
--rw-r--r--   0 dhr      (24423) staff       (20)     1507 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/ImageViewer.py
--rw-r--r--   0 dhr      (24423) staff       (20)     2464 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/MaskCompositing.py
--rw-r--r--   0 dhr      (24423) staff       (20)      906 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/NumberWidget.py
--rw-r--r--   0 dhr      (24423) staff       (20)     7027 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/ParameterWidgets.py
--rw-r--r--   0 dhr      (24423) staff       (20)     2544 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/Shader.py
--rw-r--r--   0 dhr      (24423) staff       (20)     4705 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/ShaderFXAA.py
--rw-r--r--   0 dhr      (24423) staff       (20)     5943 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/ShaderIBS.py
--rw-r--r--   0 dhr      (24423) staff       (20)     8915 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/ShaderPBR.py
--rw-r--r--   0 dhr      (24423) staff       (20)     4674 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/ShaderPhong.py
--rw-r--r--   0 dhr      (24423) staff       (20)     4043 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/ShaderSSAO.py
--rw-r--r--   0 dhr      (24423) staff       (20)      704 2023-02-06 16:41:51.000000 pycinema-0.9.0/pycinema/__init__.py
-drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2023-02-08 21:45:28.798647 pycinema-0.9.0/pycinema.egg-info/
--rw-r--r--   0 dhr      (24423) staff       (20)      574 2023-02-08 21:45:28.000000 pycinema-0.9.0/pycinema.egg-info/PKG-INFO
--rw-r--r--   0 dhr      (24423) staff       (20)      845 2023-02-08 21:45:28.000000 pycinema-0.9.0/pycinema.egg-info/SOURCES.txt
--rw-r--r--   0 dhr      (24423) staff       (20)        1 2023-02-08 21:45:28.000000 pycinema-0.9.0/pycinema.egg-info/dependency_links.txt
--rw-r--r--   0 dhr      (24423) staff       (20)       84 2023-02-08 21:45:28.000000 pycinema-0.9.0/pycinema.egg-info/requires.txt
--rw-r--r--   0 dhr      (24423) staff       (20)        9 2023-02-08 21:45:28.000000 pycinema-0.9.0/pycinema.egg-info/top_level.txt
--rw-r--r--   0 dhr      (24423) staff       (20)       38 2023-02-08 21:45:28.799056 pycinema-0.9.0/setup.cfg
--rw-r--r--   0 dhr      (24423) staff       (20)     1211 2023-02-08 20:27:08.000000 pycinema-0.9.0/setup.py
--rw-r--r--   0 dhr      (24423) staff       (20)        6 2023-02-07 22:33:59.000000 pycinema-0.9.0/version.md
+drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2023-05-25 20:44:10.473672 pycinema-1.1.0/
+-rw-r--r--   0 dhr      (24423) staff       (20)      743 2023-05-25 20:44:10.473535 pycinema-1.1.0/PKG-INFO
+drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2023-05-25 20:44:10.467525 pycinema-1.1.0/doc/
+-rw-r--r--   0 dhr      (24423) staff       (20)      364 2023-05-25 20:44:01.000000 pycinema-1.1.0/doc/description.md
+drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2023-05-25 20:44:10.472434 pycinema-1.1.0/pycinema/
+-rw-r--r--   0 dhr      (24423) staff       (20)     3493 2023-05-22 20:20:39.000000 pycinema-1.1.0/pycinema/Annotation.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     1283 2023-05-22 20:20:39.000000 pycinema-1.1.0/pycinema/Border.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     1016 2023-05-22 20:20:39.000000 pycinema-1.1.0/pycinema/CinemaDatabaseReader.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     4201 2023-05-22 20:20:39.000000 pycinema-1.1.0/pycinema/CinemaDatabaseViewer.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     3783 2023-05-22 20:20:39.000000 pycinema-1.1.0/pycinema/CinemaDatabaseWriter.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     3756 2023-05-22 20:20:39.000000 pycinema-1.1.0/pycinema/ColorMapping.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     4353 2023-05-22 20:20:39.000000 pycinema-1.1.0/pycinema/ColorMappingWidgets.py
+-rw-r--r--   0 dhr      (24423) staff       (20)      323 2023-05-22 20:20:39.000000 pycinema-1.1.0/pycinema/ColorSource.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     4628 2023-05-25 20:44:01.000000 pycinema-1.1.0/pycinema/Core.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     3357 2023-05-25 20:44:01.000000 pycinema-1.1.0/pycinema/DatabaseMerger.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     2071 2023-05-25 20:44:01.000000 pycinema-1.1.0/pycinema/DatabaseQuery.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     6897 2023-05-22 20:20:39.000000 pycinema-1.1.0/pycinema/DemoScene.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     4688 2023-05-22 20:20:39.000000 pycinema-1.1.0/pycinema/DepthCompositing.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     1060 2023-05-22 20:20:39.000000 pycinema-1.1.0/pycinema/ImageCanny.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     1092 2023-05-22 20:20:39.000000 pycinema-1.1.0/pycinema/ImageConvert.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     2421 2023-05-22 20:20:39.000000 pycinema-1.1.0/pycinema/ImageReader.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     1507 2023-05-22 20:20:39.000000 pycinema-1.1.0/pycinema/ImageViewer.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     2464 2023-05-22 20:20:39.000000 pycinema-1.1.0/pycinema/MaskCompositing.py
+-rw-r--r--   0 dhr      (24423) staff       (20)      906 2023-05-22 20:20:39.000000 pycinema-1.1.0/pycinema/NumberWidget.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     7045 2023-05-25 20:44:01.000000 pycinema-1.1.0/pycinema/ParameterWidgets.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     2544 2023-05-22 20:20:39.000000 pycinema-1.1.0/pycinema/Shader.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     4705 2023-05-22 20:20:39.000000 pycinema-1.1.0/pycinema/ShaderFXAA.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     5943 2023-05-22 20:20:39.000000 pycinema-1.1.0/pycinema/ShaderIBS.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     8915 2023-05-22 20:20:39.000000 pycinema-1.1.0/pycinema/ShaderPBR.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     4674 2023-05-22 20:20:39.000000 pycinema-1.1.0/pycinema/ShaderPhong.py
+-rw-r--r--   0 dhr      (24423) staff       (20)     4043 2023-05-22 20:20:39.000000 pycinema-1.1.0/pycinema/ShaderSSAO.py
+-rw-r--r--   0 dhr      (24423) staff       (20)      734 2023-05-25 20:44:01.000000 pycinema-1.1.0/pycinema/__init__.py
+drwxr-xr-x   0 dhr      (24423) staff       (20)        0 2023-05-25 20:44:10.473324 pycinema-1.1.0/pycinema.egg-info/
+-rw-r--r--   0 dhr      (24423) staff       (20)      743 2023-05-25 20:44:10.000000 pycinema-1.1.0/pycinema.egg-info/PKG-INFO
+-rw-r--r--   0 dhr      (24423) staff       (20)      872 2023-05-25 20:44:10.000000 pycinema-1.1.0/pycinema.egg-info/SOURCES.txt
+-rw-r--r--   0 dhr      (24423) staff       (20)        1 2023-05-25 20:44:10.000000 pycinema-1.1.0/pycinema.egg-info/dependency_links.txt
+-rw-r--r--   0 dhr      (24423) staff       (20)      154 2023-05-25 20:44:10.000000 pycinema-1.1.0/pycinema.egg-info/requires.txt
+-rw-r--r--   0 dhr      (24423) staff       (20)        9 2023-05-25 20:44:10.000000 pycinema-1.1.0/pycinema.egg-info/top_level.txt
+-rw-r--r--   0 dhr      (24423) staff       (20)       38 2023-05-25 20:44:10.473708 pycinema-1.1.0/setup.cfg
+-rw-r--r--   0 dhr      (24423) staff       (20)     1281 2023-05-25 20:44:01.000000 pycinema-1.1.0/setup.py
+-rw-r--r--   0 dhr      (24423) staff       (20)        6 2023-05-25 20:44:01.000000 pycinema-1.1.0/version.md
```

### Comparing `pycinema-0.9.0/pycinema/Annotation.py` & `pycinema-1.1.0/pycinema/Annotation.py`

 * *Files identical despite different names*

### Comparing `pycinema-0.9.0/pycinema/Border.py` & `pycinema-1.1.0/pycinema/Border.py`

 * *Files identical despite different names*

### Comparing `pycinema-0.9.0/pycinema/CinemaDatabaseReader.py` & `pycinema-1.1.0/pycinema/CinemaDatabaseReader.py`

 * *Files identical despite different names*

### Comparing `pycinema-0.9.0/pycinema/CinemaDatabaseViewer.py` & `pycinema-1.1.0/pycinema/CinemaDatabaseViewer.py`

 * *Files identical despite different names*

### Comparing `pycinema-0.9.0/pycinema/CinemaDatabaseWriter.py` & `pycinema-1.1.0/pycinema/CinemaDatabaseWriter.py`

 * *Files identical despite different names*

### Comparing `pycinema-0.9.0/pycinema/ColorMapping.py` & `pycinema-1.1.0/pycinema/ColorMapping.py`

 * *Files identical despite different names*

### Comparing `pycinema-0.9.0/pycinema/ColorMappingWidgets.py` & `pycinema-1.1.0/pycinema/ColorMappingWidgets.py`

 * *Files identical despite different names*

### Comparing `pycinema-0.9.0/pycinema/Core.py` & `pycinema-1.1.0/pycinema/Core.py`

 * *Files 12% similar despite different names*

```diff
@@ -80,54 +80,62 @@
     def __init__(self):
         return
 
 class Filter():
 
     _debug = False
     _processing = False
+    _filters = {}
 
     def __init__(self):
         self.inputs = PortList()
         self.outputs = PortList()
         self.time = -2
+        self._filters[self] = self
+
+    def __del__(self):
+        del self._filters[self]
 
     def addInputPort(self, name, value):
         setattr(self.inputs, name, Port(name, value, self, True))
 
     def addOutputPort(self, name, value):
         setattr(self.outputs, name, Port(name, value, self))
 
     def _update(self):
         # needs to be overriden
         return 1
 
     def computeDAG(self,edges):
-        if self in edges:
-            return 1
-
-        edges[self] = set({})
+        for f in self._filters:
+            edges[f] = set({})
 
-        for name in [o for o in dir(self.outputs) if not o.startswith('__')]:
-            port = getattr(self.outputs, name)
-            for listener in port.connections:
-                edges[self].add(listener.parent)
-                listener.parent.computeDAG(edges)
+        for f in self._filters:
+            for name in [o for o in dir(f.outputs) if not o.startswith('__')]:
+                port = getattr(f.outputs, name)
+                for listener in port.connections:
+                    edges[f].add(listener.parent)
 
         return 1
 
     def computeTopologicalOrdering(self,edges):
-      L = []
-      S = [self]
+
       edgesR = {}
       for n in edges:
         for m in edges[n]:
           if not m in edgesR:
               edgesR[m] = 0
           edgesR[m]+=1
 
+      L = []
+      S = []
+      for f in self._filters:
+          if f not in edgesR or not edgesR[f]:
+              S.append(f)
+
       while len(S)>0:
           n = S.pop()
           L.append(n)
           for m in edges[n]:
               edgesR[m]-=1
               if edgesR[m]<1:
                   S.append(m)
@@ -138,25 +146,28 @@
 
         Filter._processing = True
 
         dagt = time.time()
         edges = {}
         self.computeDAG(edges)
         filters = self.computeTopologicalOrdering(edges)
+
         if Filter._debug:
+            for k, v in edges.items():
+              print(k,v)
             print("DAG (%.2fs)" % (time.time()-dagt))
 
         for i,f in enumerate(filters):
             lt = f.time
             needsUpdate = False
             for name in [o for o in dir(f.inputs) if not o.startswith('__')]:
                 iport = getattr(f.inputs, name)
                 if lt<iport.getTime():
                     needsUpdate = True
-            if i==0 or needsUpdate:
+            if f==self or needsUpdate:
                 t0 = time.time()
                 if Filter._debug:
                     print('PROCESS',f)
                 f._update()
                 f.time = time.time()
                 if Filter._debug:
                     print(" -> Done (%.2fs)" % (f.time-t0))
```

### Comparing `pycinema-0.9.0/pycinema/DatabaseQuery.py` & `pycinema-1.1.0/pycinema/DatabaseQuery.py`

 * *Files 15% similar despite different names*

```diff
@@ -47,30 +47,36 @@
             for v in table[i]:
                 row += '"' + str(v) + '",'
             sql += row[0:-1] + '),\n'
         sql = sql[0:-2];
         self.executeSQL(db,sql)
 
     def queryData(self, db, sqlQuery):
-        c = db.cursor();
-        c.execute(sqlQuery);
-        res = c.fetchall();
-        columns = [];
+        c = db.cursor()
+        c.execute(sqlQuery)
+        res = c.fetchall()
+        columns = []
         for d in c.description:
-            columns.append(d[0]);
-        res.insert(0,columns);
-        return res;
+            columns.append(d[0])
+        res.insert(0,columns)
+        return res
 
     def _update(self):
 
-      db = sqlite3.connect(":memory:");
+      db = sqlite3.connect(":memory:")
 
-      table = self.inputs.table.get();
+      table = self.inputs.table.get()
+      sql = self.inputs.sql.get()
 
-      self.createTable(db, table);
-      self.insertData(db, table);
+      if isinstance(sql, dict):
+        header = table[0]
+        sql2 = {k: v for k, v in sql.items() if k in header}
+        sql = 'SELECT * FROM input WHERE '+ ' AND '.join(sql2.values())
 
-      output = self.queryData(db, self.inputs.sql.get());
+      self.createTable(db, table)
+      self.insertData(db, table)
 
-      self.outputs.table.set(output);
+      output = self.queryData(db, sql)
+
+      self.outputs.table.set(output)
 
       return 1;
```

### Comparing `pycinema-0.9.0/pycinema/DemoScene.py` & `pycinema-1.1.0/pycinema/DemoScene.py`

 * *Files identical despite different names*

### Comparing `pycinema-0.9.0/pycinema/DepthCompositing.py` & `pycinema-1.1.0/pycinema/DepthCompositing.py`

 * *Files identical despite different names*

### Comparing `pycinema-0.9.0/pycinema/ImageCanny.py` & `pycinema-1.1.0/pycinema/ImageCanny.py`

 * *Files identical despite different names*

### Comparing `pycinema-0.9.0/pycinema/ImageConvert.py` & `pycinema-1.1.0/pycinema/ImageConvert.py`

 * *Files identical despite different names*

### Comparing `pycinema-0.9.0/pycinema/ImageReader.py` & `pycinema-1.1.0/pycinema/ImageReader.py`

 * *Files identical despite different names*

### Comparing `pycinema-0.9.0/pycinema/ImageViewer.py` & `pycinema-1.1.0/pycinema/ImageViewer.py`

 * *Files identical despite different names*

### Comparing `pycinema-0.9.0/pycinema/MaskCompositing.py` & `pycinema-1.1.0/pycinema/MaskCompositing.py`

 * *Files identical despite different names*

### Comparing `pycinema-0.9.0/pycinema/NumberWidget.py` & `pycinema-1.1.0/pycinema/NumberWidget.py`

 * *Files identical despite different names*

### Comparing `pycinema-0.9.0/pycinema/ParameterWidgets.py` & `pycinema-1.1.0/pycinema/ParameterWidgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,17 @@
             return '"' + wt['parameter'] + '"=' + v
         else:
             return '"' + wt['parameter'] + '"="' + v + '"'
 
     def generateWidgets(self):
 
         table = self.inputs.table.get()
+        if len(table)<1:
+          return 0
+
         header = table[0]
         self.widgets = []
 
         def on_change(change):
             if change['type'] == 'change' and change['name'] == 'value':
                 self.update()
 
@@ -183,30 +186,28 @@
           )
 
           container.children = [grid]
 
     def _update(self):
 
         table = self.inputs.table.get()
-        header = table[0]
-
-        sql = 'SELECT * FROM input WHERE '
+        if len(table)<1:
+          return 0
 
         # compute widgets
         if len(self.widgets) < 1:
             self.generateWidgets()
 
+        sql = {}
         for i,wt in enumerate(self.widgets):
             wsql = self.widgetToSQL(wt)
             if len(wsql)>0:
-                sql += wsql+ ' AND '
-
-        sql += ' '
+                sql[wt['parameter']] = wsql
 
-        self.outputs.sql.set(sql[:-6])
+        self.outputs.sql.set(sql)
 
         composite_by_meta = (None,{})
         for i,wt in enumerate(self.widgets):
             if wt['C'].value:
                 valueMap = {}
                 for i,v in enumerate(wt['values']):
                     valueMap[v] = i
```

### Comparing `pycinema-0.9.0/pycinema/Shader.py` & `pycinema-1.1.0/pycinema/Shader.py`

 * *Files identical despite different names*

### Comparing `pycinema-0.9.0/pycinema/ShaderFXAA.py` & `pycinema-1.1.0/pycinema/ShaderFXAA.py`

 * *Files identical despite different names*

### Comparing `pycinema-0.9.0/pycinema/ShaderIBS.py` & `pycinema-1.1.0/pycinema/ShaderIBS.py`

 * *Files identical despite different names*

### Comparing `pycinema-0.9.0/pycinema/ShaderPBR.py` & `pycinema-1.1.0/pycinema/ShaderPBR.py`

 * *Files identical despite different names*

### Comparing `pycinema-0.9.0/pycinema/ShaderPhong.py` & `pycinema-1.1.0/pycinema/ShaderPhong.py`

 * *Files identical despite different names*

### Comparing `pycinema-0.9.0/pycinema/ShaderSSAO.py` & `pycinema-1.1.0/pycinema/ShaderSSAO.py`

 * *Files identical despite different names*

### Comparing `pycinema-0.9.0/pycinema/__init__.py` & `pycinema-1.1.0/pycinema/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .CinemaDatabaseReader import *
 from .CinemaDatabaseViewer import *
 from .CinemaDatabaseWriter import *
 from .ColorMapping import *
 from .ColorMappingWidgets import *
 from .ColorSource import *
 from .DatabaseQuery import *
+from .DatabaseMerger import *
 from .DemoScene import *
 from .DepthCompositing import *
 from .ImageCanny import *
 from .ImageConvert import *
 from .ImageReader import *
 from .ImageViewer import *
 from .MaskCompositing import *
```

### Comparing `pycinema-0.9.0/pycinema.egg-info/SOURCES.txt` & `pycinema-1.1.0/pycinema.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 pycinema/CinemaDatabaseReader.py
 pycinema/CinemaDatabaseViewer.py
 pycinema/CinemaDatabaseWriter.py
 pycinema/ColorMapping.py
 pycinema/ColorMappingWidgets.py
 pycinema/ColorSource.py
 pycinema/Core.py
+pycinema/DatabaseMerger.py
 pycinema/DatabaseQuery.py
 pycinema/DemoScene.py
 pycinema/DepthCompositing.py
 pycinema/ImageCanny.py
 pycinema/ImageConvert.py
 pycinema/ImageReader.py
 pycinema/ImageViewer.py
```

### Comparing `pycinema-0.9.0/setup.py` & `pycinema-1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,24 +18,24 @@
     description="Cinema scientific toolset.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/cinemascience/pycinema",
     include_package_data=True,
     packages=[  "pycinema"  ],
     install_requires=[
-        "numpy",
-        "scipy",
-        "h5py",
-        "matplotlib",
-        "py",
-        "Pillow",
+        "numpy==1.24.2",
+        "scipy==1.10.0",
+        "h5py==3.8.0",
+        "matplotlib==3.6.0",
+        "py==1.11.0",
+        "Pillow==9.4.0",
         "moderngl<6",
-        "opencv-python",
-        "ipycanvas",
-        "ipywidgets"
+        "opencv-python==4.7.0.68",
+        "ipycanvas==0.13.1",
+        "ipywidgets==8.0.6"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
     scripts=[
```

