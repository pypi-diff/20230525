# Comparing `tmp/desim-tool-0.3.1.tar.gz` & `tmp/desim-tool-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desim-tool-0.3.1.tar", last modified: Thu Dec  1 10:40:46 2022, max compression
+gzip compressed data, was "desim-tool-0.3.2.tar", last modified: Thu May 25 10:34:15 2023, max compression
```

## Comparing `desim-tool-0.3.1.tar` & `desim-tool-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 chops     (1000) chops     (1000)        0 2022-12-01 10:40:46.251275 desim-tool-0.3.1/
--rw-r--r--   0 chops     (1000) chops     (1000)     1089 2022-11-24 19:42:14.000000 desim-tool-0.3.1/LICENSE.md
--rw-r--r--   0 chops     (1000) chops     (1000)      211 2022-12-01 10:40:46.251275 desim-tool-0.3.1/PKG-INFO
--rw-r--r--   0 chops     (1000) chops     (1000)     1561 2022-11-25 09:38:51.000000 desim-tool-0.3.1/README.md
-drwxr-xr-x   0 chops     (1000) chops     (1000)        0 2022-12-01 10:40:46.251275 desim-tool-0.3.1/desim/
--rw-r--r--   0 chops     (1000) chops     (1000)        0 2022-08-08 15:49:11.000000 desim-tool-0.3.1/desim/__init__.py
--rw-r--r--   0 chops     (1000) chops     (1000)     2363 2022-11-24 19:42:14.000000 desim-tool-0.3.1/desim/data.py
--rw-r--r--   0 chops     (1000) chops     (1000)     6831 2022-11-25 09:38:51.000000 desim-tool-0.3.1/desim/interface.py
--rw-r--r--   0 chops     (1000) chops     (1000)    10027 2022-11-25 09:38:51.000000 desim-tool-0.3.1/desim/simulation.py
-drwxr-xr-x   0 chops     (1000) chops     (1000)        0 2022-12-01 10:40:46.251275 desim-tool-0.3.1/desim_tool.egg-info/
--rw-r--r--   0 chops     (1000) chops     (1000)      211 2022-12-01 10:40:46.000000 desim-tool-0.3.1/desim_tool.egg-info/PKG-INFO
--rw-r--r--   0 chops     (1000) chops     (1000)      279 2022-12-01 10:40:46.000000 desim-tool-0.3.1/desim_tool.egg-info/SOURCES.txt
--rw-r--r--   0 chops     (1000) chops     (1000)        1 2022-12-01 10:40:46.000000 desim-tool-0.3.1/desim_tool.egg-info/dependency_links.txt
--rw-r--r--   0 chops     (1000) chops     (1000)       12 2022-12-01 10:40:46.000000 desim-tool-0.3.1/desim_tool.egg-info/requires.txt
--rw-r--r--   0 chops     (1000) chops     (1000)        6 2022-12-01 10:40:46.000000 desim-tool-0.3.1/desim_tool.egg-info/top_level.txt
--rw-r--r--   0 chops     (1000) chops     (1000)      106 2022-12-01 10:40:46.251275 desim-tool-0.3.1/setup.cfg
--rw-r--r--   0 chops     (1000) chops     (1000)      283 2022-12-01 10:40:42.000000 desim-tool-0.3.1/setup.py
+drwxr-xr-x   0 oscarbennet   (501) staff       (20)        0 2023-05-25 10:34:15.284187 desim-tool-0.3.2/
+-rw-r--r--   0 oscarbennet   (501) staff       (20)     1089 2023-05-18 16:32:34.000000 desim-tool-0.3.2/LICENSE.md
+-rw-r--r--   0 oscarbennet   (501) staff       (20)      211 2023-05-25 10:34:15.284631 desim-tool-0.3.2/PKG-INFO
+-rw-r--r--   0 oscarbennet   (501) staff       (20)     1561 2023-05-18 16:32:34.000000 desim-tool-0.3.2/README.md
+drwxr-xr-x   0 oscarbennet   (501) staff       (20)        0 2023-05-25 10:34:15.276680 desim-tool-0.3.2/desim/
+-rw-r--r--   0 oscarbennet   (501) staff       (20)        0 2023-05-18 16:32:34.000000 desim-tool-0.3.2/desim/__init__.py
+-rw-r--r--   0 oscarbennet   (501) staff       (20)     2363 2023-05-18 16:32:34.000000 desim-tool-0.3.2/desim/data.py
+-rw-r--r--   0 oscarbennet   (501) staff       (20)     6831 2023-05-18 16:32:34.000000 desim-tool-0.3.2/desim/interface.py
+-rw-r--r--   0 oscarbennet   (501) staff       (20)    10078 2023-05-25 08:06:50.000000 desim-tool-0.3.2/desim/simulation.py
+drwxr-xr-x   0 oscarbennet   (501) staff       (20)        0 2023-05-25 10:34:15.282771 desim-tool-0.3.2/desim_tool.egg-info/
+-rw-r--r--   0 oscarbennet   (501) staff       (20)      211 2023-05-25 10:34:15.000000 desim-tool-0.3.2/desim_tool.egg-info/PKG-INFO
+-rw-r--r--   0 oscarbennet   (501) staff       (20)      279 2023-05-25 10:34:15.000000 desim-tool-0.3.2/desim_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 oscarbennet   (501) staff       (20)        1 2023-05-25 10:34:15.000000 desim-tool-0.3.2/desim_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 oscarbennet   (501) staff       (20)       12 2023-05-25 10:34:15.000000 desim-tool-0.3.2/desim_tool.egg-info/requires.txt
+-rw-r--r--   0 oscarbennet   (501) staff       (20)        6 2023-05-25 10:34:15.000000 desim-tool-0.3.2/desim_tool.egg-info/top_level.txt
+-rw-r--r--   0 oscarbennet   (501) staff       (20)      106 2023-05-25 10:34:15.285820 desim-tool-0.3.2/setup.cfg
+-rw-r--r--   0 oscarbennet   (501) staff       (20)      283 2023-05-25 08:10:46.000000 desim-tool-0.3.2/setup.py
```

### Comparing `desim-tool-0.3.1/LICENSE.md` & `desim-tool-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `desim-tool-0.3.1/README.md` & `desim-tool-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `desim-tool-0.3.1/desim/data.py` & `desim-tool-0.3.2/desim/data.py`

 * *Files identical despite different names*

### Comparing `desim-tool-0.3.1/desim/interface.py` & `desim-tool-0.3.2/desim/interface.py`

 * *Files identical despite different names*

### Comparing `desim-tool-0.3.1/desim/simulation.py` & `desim-tool-0.3.2/desim/simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 
 class Simulation(object):
     #@param:
     #flow_time = the time that entities will flow in the system
     #interarrival_time = the rate at which entities will flow in the system
     #interarrival_process = the process at which the entities will start flowing
     #until = the total simulation time
-    def __init__(self, flow_time: float, flow_rate: float, flow_process: str, simulation_runtime: float, discount_rate: float, processes, non_tech_processes, non_tech_addition, dsm, time_format: TimeFormat) -> None:
+    def __init__(self, flow_time: float, flow_rate: int, flow_process: str, simulation_runtime: float, discount_rate: float, processes, non_tech_processes, non_tech_addition, dsm, time_format: TimeFormat) -> None:
         self.flow_time = flow_time
-        self.interarrival_time =  0 if flow_rate <= 0 else 1 / (flow_rate * time_format.value) #Causes the interarrival time to be in years. 
+        self.flow_rate = flow_rate
+        self.interarrival_time = 0 if flow_rate <= 0 else 1 / (flow_rate * time_format.value) #Causes the interarrival time to be in years.
         self.interarrival_process = flow_process
         self.until = simulation_runtime / time_format.value #Causes the runtime to be in years. 
         self.discount_rate = discount_rate
         self.cum_NPV = [0]
         self.total_costs = [0]
         self.total_revenue = [0]
         self.time_steps = [0]
@@ -51,19 +52,19 @@
         
         e = Entity(env, self.processes, self.non_tech_costs)
         self.entities.append(e)
         yield env.process(e.lifecycle(self.dsm_before_flow, [self.processes[0]], 1))
         
         end_flow = env.now + self.flow_time
         while env.now < end_flow:
-            yield env.timeout(self.generate_interarrival())
-        
-            e = Entity(env, self.processes, self.non_tech_costs)
-            self.entities.append(e)
-            env.process(e.lifecycle(self.dsm_after_flow, interarrival_process, total_ent_amount))
+            for i in range(self.flow_rate):
+                e = Entity(env, self.processes, self.non_tech_costs)
+                self.entities.append(e)
+                env.process(e.lifecycle(self.dsm_after_flow, interarrival_process, total_ent_amount))
+            yield env.timeout(1)
         
 
         #print('Done')
             
             
     #Observes the total time, cost, revenue, and NPV for each entity in each timestep. 
     def observe_costs(self, env): #TODO fix calculation of NPV. Currently it's bonkers
```

