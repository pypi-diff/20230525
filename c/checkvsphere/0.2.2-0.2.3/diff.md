# Comparing `tmp/checkvsphere-0.2.2.tar.gz` & `tmp/checkvsphere-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkvsphere-0.2.2.tar", last modified: Tue May  2 14:13:36 2023, max compression
+gzip compressed data, was "checkvsphere-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `checkvsphere-0.2.2.tar` & `checkvsphere-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      275 2023-04-21 14:16:49.947749 checkvsphere-0.2.2/README.md
--rw-r--r--   0        0        0      174 2023-04-21 14:16:49.947749 checkvsphere-0.2.2/checkvsphere/__init__.py
--rw-r--r--   0        0        0     3882 2023-04-21 14:16:49.959749 checkvsphere-0.2.2/checkvsphere/cli.py
--rw-r--r--   0        0        0      760 2023-04-21 14:16:49.971748 checkvsphere-0.2.2/checkvsphere/tools/__init__.py
--rw-r--r--   0        0        0    16614 2023-04-21 14:16:49.971748 checkvsphere-0.2.2/checkvsphere/tools/cli.py
--rw-r--r--   0        0        0     6363 2023-04-21 14:16:49.971748 checkvsphere-0.2.2/checkvsphere/tools/helper.py
--rw-r--r--   0        0        0     5200 2023-04-21 14:16:49.971748 checkvsphere-0.2.2/checkvsphere/tools/pchelper.py
--rw-r--r--   0        0        0     2183 2023-04-21 14:16:49.971748 checkvsphere-0.2.2/checkvsphere/tools/service_instance.py
--rw-r--r--   0        0        0     4153 2023-04-21 14:16:49.975748 checkvsphere-0.2.2/checkvsphere/tools/serviceutil.py
--rw-r--r--   0        0        0      760 2023-04-21 14:16:49.975748 checkvsphere-0.2.2/checkvsphere/vcmd/__init__.py
--rw-r--r--   0        0        0     1819 2023-04-21 14:16:49.975748 checkvsphere-0.2.2/checkvsphere/vcmd/about.py
--rw-r--r--   0        0        0     6692 2023-05-02 11:25:14.016969 checkvsphere-0.2.2/checkvsphere/vcmd/datastores.py
--rw-r--r--   0        0        0     4497 2023-04-21 14:16:49.975748 checkvsphere-0.2.2/checkvsphere/vcmd/hostnic.py
--rw-r--r--   0        0        0    11156 2023-04-28 12:52:00.785872 checkvsphere-0.2.2/checkvsphere/vcmd/hostruntime.py
--rw-r--r--   0        0        0     4038 2023-04-21 14:16:49.975748 checkvsphere-0.2.2/checkvsphere/vcmd/hostservice.py
--rw-r--r--   0        0        0     7633 2023-04-21 14:16:49.975748 checkvsphere-0.2.2/checkvsphere/vcmd/hoststorage.py
--rw-r--r--   0        0        0     2039 2023-04-21 14:16:49.983748 checkvsphere-0.2.2/checkvsphere/vcmd/listmetrics.py
--rw-r--r--   0        0        0     3341 2023-04-21 14:16:49.983748 checkvsphere-0.2.2/checkvsphere/vcmd/media.py
--rw-r--r--   0        0        0     8301 2023-04-21 14:16:49.983748 checkvsphere-0.2.2/checkvsphere/vcmd/perf.py
--rw-r--r--   0        0        0     4929 2023-04-21 14:16:49.983748 checkvsphere-0.2.2/checkvsphere/vcmd/snapshots.py
--rw-r--r--   0        0        0     8945 2023-04-21 14:16:49.983748 checkvsphere-0.2.2/checkvsphere/vcmd/vsan.py
--rw-r--r--   0        0        0      941 2023-05-02 14:12:48.139031 checkvsphere-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 checkvsphere-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      275 2023-05-03 13:33:32.671674 checkvsphere-0.2.3/README.md
+-rw-r--r--   0        0        0      174 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/__init__.py
+-rw-r--r--   0        0        0     3882 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/cli.py
+-rw-r--r--   0        0        0      760 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/tools/__init__.py
+-rw-r--r--   0        0        0    16614 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/tools/cli.py
+-rw-r--r--   0        0        0     6363 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/tools/helper.py
+-rw-r--r--   0        0        0     5200 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/tools/pchelper.py
+-rw-r--r--   0        0        0     2183 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/tools/service_instance.py
+-rw-r--r--   0        0        0     4153 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/tools/serviceutil.py
+-rw-r--r--   0        0        0      760 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/vcmd/__init__.py
+-rw-r--r--   0        0        0     1819 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/vcmd/about.py
+-rw-r--r--   0        0        0     6692 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/vcmd/datastores.py
+-rw-r--r--   0        0        0     4497 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/vcmd/hostnic.py
+-rw-r--r--   0        0        0    11076 2023-05-24 13:31:30.446500 checkvsphere-0.2.3/checkvsphere/vcmd/hostruntime.py
+-rw-r--r--   0        0        0     4038 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/vcmd/hostservice.py
+-rw-r--r--   0        0        0     7633 2023-05-03 13:33:32.675674 checkvsphere-0.2.3/checkvsphere/vcmd/hoststorage.py
+-rw-r--r--   0        0        0     2039 2023-05-03 13:33:32.679674 checkvsphere-0.2.3/checkvsphere/vcmd/listmetrics.py
+-rw-r--r--   0        0        0     3341 2023-05-03 13:33:32.679674 checkvsphere-0.2.3/checkvsphere/vcmd/media.py
+-rw-r--r--   0        0        0     8301 2023-05-03 13:33:32.679674 checkvsphere-0.2.3/checkvsphere/vcmd/perf.py
+-rw-r--r--   0        0        0     4929 2023-05-03 13:33:32.679674 checkvsphere-0.2.3/checkvsphere/vcmd/snapshots.py
+-rw-r--r--   0        0        0     8945 2023-05-03 13:33:32.679674 checkvsphere-0.2.3/checkvsphere/vcmd/vsan.py
+-rw-r--r--   0        0        0      941 2023-05-25 08:27:33.439404 checkvsphere-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 checkvsphere-0.2.3/PKG-INFO
```

### Comparing `checkvsphere-0.2.2/checkvsphere/cli.py` & `checkvsphere-0.2.3/checkvsphere/cli.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.2/checkvsphere/tools/__init__.py` & `checkvsphere-0.2.3/checkvsphere/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.2/checkvsphere/tools/cli.py` & `checkvsphere-0.2.3/checkvsphere/tools/cli.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.2/checkvsphere/tools/helper.py` & `checkvsphere-0.2.3/checkvsphere/tools/helper.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.2/checkvsphere/tools/pchelper.py` & `checkvsphere-0.2.3/checkvsphere/tools/pchelper.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.2/checkvsphere/tools/service_instance.py` & `checkvsphere-0.2.3/checkvsphere/tools/service_instance.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.2/checkvsphere/tools/serviceutil.py` & `checkvsphere-0.2.3/checkvsphere/tools/serviceutil.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.2/checkvsphere/vcmd/__init__.py` & `checkvsphere-0.2.3/checkvsphere/vcmd/__init__.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.2/checkvsphere/vcmd/about.py` & `checkvsphere-0.2.3/checkvsphere/vcmd/about.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.2/checkvsphere/vcmd/datastores.py` & `checkvsphere-0.2.3/checkvsphere/vcmd/datastores.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.2/checkvsphere/vcmd/hostnic.py` & `checkvsphere-0.2.3/checkvsphere/vcmd/hostnic.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.2/checkvsphere/vcmd/hostruntime.py` & `checkvsphere-0.2.3/checkvsphere/vcmd/hostruntime.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,22 +77,22 @@
     #vm_view = si.content.viewManager.CreateContainerView(parentView, [vim.VirtualMachine], True)
     try:
         vm = find_entity_views(
             si,
             vim.HostSystem,
             begin_entity=si.content.rootFolder,
             sieve=({'name': args.vihost} if args.vihost else None),
-            properties=['name', 'runtime', 'overallStatus', 'configIssue', 'summary.config']
+            properties=['name', 'runtime.inMaintenanceMode'],
         )[0]
     except IndexError:
         check.exit(Status.UNKNOWN, f"host {args.vihost or ''} not found")
 
     result = []
 
-    if vm['props']['runtime'].inMaintenanceMode:
+    if vm['props']['runtime.inMaintenanceMode']:
         status = getattr(Status, args.maintenance_state)
         check.exit(
             status,
             f"host {vm['props']['name']} is in maintenance"
         )
 
     okmessage = "No errors"
@@ -147,45 +147,44 @@
         if formattedThing:
             formattedThings.append( formattedThing )
 
     return ", ".join(formattedThings)
 
 
 def check_issues(check, vm, args, result):
-    issues = vm['props']['configIssue']
+    issues = vm['obj'].obj.configIssue
     for issue in issues:
         if isbanned(args, issue.fullFormattedMessage):
             continue
         if not isallowed(args, issue.fullFormattedMessage):
             continue
         check.add_message(Status.CRITICAL, format_issue(issue))
 
     return "No issues found"
 
 
 def check_con(check, vm, args, result):
-    con = vm['props']['runtime'].connectionState
+    con = vm['obj'].obj.runtime.connectionState
     status = Status.OK
     if con == "disconnected":
         status = Status.WARNING
     elif con == "notResponding":
         status = Status.CRITICAL
     check.exit(
         status,
         message = f"connection state is '{con}'"
     )
 
 def check_status(check, vm, args, result):
-    color = vm['props']['overallStatus']
+    color = vm['obj'].obj.overallStatus
     status = health2state(color)
     check.exit(status, f"overall status is {str(color).upper()}")
 
 def check_temp(check, vm, args, result):
-    runtime = vm['props']['runtime']
-    systemRuntime = runtime.healthSystemRuntime
+    systemRuntime = vm['obj'].obj.runtime.healthSystemRuntime
     if not systemRuntime:
         check.exit(
             Status.UNKNOWN,
             "Temperature status unavailable"
         )
 
     numericinfo = systemRuntime.systemHealthInfo.numericSensorInfo
@@ -200,16 +199,15 @@
         name = info.name.rstrip(' Temp')
         check.add_perfdata(label=name, value=info.currentReading * (10 ** info.unitModifier))
         check.add_message(state, f"{name} is {info.healthState.key}")
 
     return "All temperature sensors green"
 
 def check_health(check, vm, args, result):
-    runtime = vm['props']['runtime']
-    healthsystem = runtime.healthSystemRuntime
+    healthsystem = vm['obj'].obj.runtime.healthSystemRuntime
     if not healthsystem:
         check.exit(
             Status.UNKNOWN,
             "system health status not available, "
             "no vim.Host.runtime.healthSystemRuntime found"
         )
     if not healthsystem.hardwareStatusInfo:
```

### Comparing `checkvsphere-0.2.2/checkvsphere/vcmd/hostservice.py` & `checkvsphere-0.2.3/checkvsphere/vcmd/hostservice.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.2/checkvsphere/vcmd/hoststorage.py` & `checkvsphere-0.2.3/checkvsphere/vcmd/hoststorage.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.2/checkvsphere/vcmd/listmetrics.py` & `checkvsphere-0.2.3/checkvsphere/vcmd/listmetrics.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.2/checkvsphere/vcmd/media.py` & `checkvsphere-0.2.3/checkvsphere/vcmd/media.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.2/checkvsphere/vcmd/perf.py` & `checkvsphere-0.2.3/checkvsphere/vcmd/perf.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.2/checkvsphere/vcmd/snapshots.py` & `checkvsphere-0.2.3/checkvsphere/vcmd/snapshots.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.2/checkvsphere/vcmd/vsan.py` & `checkvsphere-0.2.3/checkvsphere/vcmd/vsan.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.2/pyproject.toml` & `checkvsphere-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.2,<4"]
 
 [project]
 name = "checkvsphere"
 readme = "README.md"
 description = "check_vsphere monitoring plugin"
-version = "0.2.2"
+version = "0.2.3"
 requires-python = ">= 3.6"
 authors = [
     { name = "Danijel Tasov", email = "danijel.tasov@consol.de" }
 ]
 dependencies = [
     "pyvmomi >= 8.0.0.1, < 9",
     "monplugin >= 0.6.1",
```

### Comparing `checkvsphere-0.2.2/PKG-INFO` & `checkvsphere-0.2.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkvsphere
-Version: 0.2.2
+Version: 0.2.3
 Summary: check_vsphere monitoring plugin
 Author-email: Danijel Tasov <danijel.tasov@consol.de>
 Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

