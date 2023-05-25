# Comparing `tmp/DSSE-0.1.12.tar.gz` & `tmp/DSSE-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DSSE-0.1.12.tar", last modified: Mon May 22 19:18:06 2023, max compression
+gzip compressed data, was "DSSE-0.1.13.tar", last modified: Thu May 25 13:18:45 2023, max compression
```

## Comparing `DSSE-0.1.12.tar` & `DSSE-0.1.13.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 19:18:06.983030 DSSE-0.1.12/
--rw-rw-rw-   0        0        0       15 2023-05-20 21:35:05.000000 DSSE-0.1.12/MANIFEST.in
--rw-rw-rw-   0        0        0    14585 2023-05-22 19:18:06.983030 DSSE-0.1.12/PKG-INFO
--rw-rw-rw-   0        0        0    14019 2023-05-22 19:17:37.000000 DSSE-0.1.12/README.md
--rw-rw-rw-   0        0        0     1090 2023-05-20 19:28:40.000000 DSSE-0.1.12/license.txt
--rw-rw-rw-   0        0        0      108 2023-05-20 19:48:09.000000 DSSE-0.1.12/pyproject.toml
--rw-rw-rw-   0        0        0      738 2023-05-22 19:18:06.983030 DSSE-0.1.12/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-22 19:18:06.924181 DSSE-0.1.12/src/
-drwxrwxrwx   0        0        0        0 2023-05-22 19:18:06.951015 DSSE-0.1.12/src/DSSE/
--rw-rw-rw-   0        0        0        4 2023-05-20 21:07:23.000000 DSSE-0.1.12/src/DSSE/__init__.py
--rw-rw-rw-   0        0        0    17049 2023-05-22 14:28:56.000000 DSSE-0.1.12/src/DSSE/env.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:18:06.975031 DSSE-0.1.12/src/DSSE/generator/
--rw-rw-rw-   0        0        0        0 2023-05-20 21:18:36.000000 DSSE-0.1.12/src/DSSE/generator/__init__.py
--rw-rw-rw-   0        0        0     6371 2023-05-22 14:27:49.000000 DSSE-0.1.12/src/DSSE/generator/dynamic_probability.py
--rw-rw-rw-   0        0        0     1266 2023-05-22 14:27:57.000000 DSSE-0.1.12/src/DSSE/generator/map.py
-drwxrwxrwx   0        0        0        0 2023-05-22 19:18:06.983030 DSSE-0.1.12/src/DSSE/imgs/
--rw-rw-rw-   0        0        0        0 2023-05-20 21:27:33.000000 DSSE-0.1.12/src/DSSE/imgs/__init__.py
--rw-rw-rw-   0        0        0    14774 2023-04-24 18:51:34.000000 DSSE-0.1.12/src/DSSE/imgs/drone.png
--rw-rw-rw-   0        0        0    13193 2023-04-24 19:07:28.000000 DSSE-0.1.12/src/DSSE/imgs/person-swimming.png
-drwxrwxrwx   0        0        0        0 2023-05-22 19:18:06.967036 DSSE-0.1.12/src/DSSE.egg-info/
--rw-rw-rw-   0        0        0    14585 2023-05-22 19:18:06.000000 DSSE-0.1.12/src/DSSE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-05-22 19:18:06.000000 DSSE-0.1.12/src/DSSE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 19:18:06.000000 DSSE-0.1.12/src/DSSE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-22 19:18:06.000000 DSSE-0.1.12/src/DSSE.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 13:18:45.890947 DSSE-0.1.13/
+-rw-rw-rw-   0        0        0       15 2023-05-20 21:35:05.000000 DSSE-0.1.13/MANIFEST.in
+-rw-rw-rw-   0        0        0    14585 2023-05-25 13:18:45.891949 DSSE-0.1.13/PKG-INFO
+-rw-rw-rw-   0        0        0    14019 2023-05-22 19:17:37.000000 DSSE-0.1.13/README.md
+-rw-rw-rw-   0        0        0     1090 2023-05-20 19:28:40.000000 DSSE-0.1.13/license.txt
+-rw-rw-rw-   0        0        0      108 2023-05-20 19:48:09.000000 DSSE-0.1.13/pyproject.toml
+-rw-rw-rw-   0        0        0      738 2023-05-25 13:18:45.893932 DSSE-0.1.13/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 13:18:45.839123 DSSE-0.1.13/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 13:18:45.868254 DSSE-0.1.13/src/DSSE/
+-rw-rw-rw-   0        0        0        4 2023-05-20 21:07:23.000000 DSSE-0.1.13/src/DSSE/__init__.py
+-rw-rw-rw-   0        0        0    16883 2023-05-25 13:17:22.000000 DSSE-0.1.13/src/DSSE/env.py
+drwxrwxrwx   0        0        0        0 2023-05-25 13:18:45.883250 DSSE-0.1.13/src/DSSE/generator/
+-rw-rw-rw-   0        0        0        0 2023-05-20 21:18:36.000000 DSSE-0.1.13/src/DSSE/generator/__init__.py
+-rw-rw-rw-   0        0        0     6371 2023-05-22 14:27:49.000000 DSSE-0.1.13/src/DSSE/generator/dynamic_probability.py
+-rw-rw-rw-   0        0        0     1266 2023-05-22 14:27:57.000000 DSSE-0.1.13/src/DSSE/generator/map.py
+drwxrwxrwx   0        0        0        0 2023-05-25 13:18:45.889914 DSSE-0.1.13/src/DSSE/imgs/
+-rw-rw-rw-   0        0        0        0 2023-05-20 21:27:33.000000 DSSE-0.1.13/src/DSSE/imgs/__init__.py
+-rw-rw-rw-   0        0        0    14774 2023-04-24 18:51:34.000000 DSSE-0.1.13/src/DSSE/imgs/drone.png
+-rw-rw-rw-   0        0        0    13193 2023-04-24 19:07:28.000000 DSSE-0.1.13/src/DSSE/imgs/person-swimming.png
+drwxrwxrwx   0        0        0        0 2023-05-25 13:18:45.877250 DSSE-0.1.13/src/DSSE.egg-info/
+-rw-rw-rw-   0        0        0    14585 2023-05-25 13:18:45.000000 DSSE-0.1.13/src/DSSE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-05-25 13:18:45.000000 DSSE-0.1.13/src/DSSE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 13:18:45.000000 DSSE-0.1.13/src/DSSE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-25 13:18:45.000000 DSSE-0.1.13/src/DSSE.egg-info/top_level.txt
```

### Comparing `DSSE-0.1.12/PKG-INFO` & `DSSE-0.1.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DSSE
-Version: 0.1.12
+Version: 0.1.13
 Summary: An environment to train drones to search and find a shipwrecked person lost in the ocean using reinforcement learning.
 Home-page: https://github.com/PFE-Embraer/drone-swarm-search
 Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `DSSE-0.1.12/README.md` & `DSSE-0.1.13/README.md`

 * *Files identical despite different names*

### Comparing `DSSE-0.1.12/license.txt` & `DSSE-0.1.13/license.txt`

 * *Files identical despite different names*

### Comparing `DSSE-0.1.12/setup.cfg` & `DSSE-0.1.13/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2044 5353 450d 0a76 6572 7369 6f6e   = DSSE..version
-00000020: 203d 2030 2e31 2e31 320d 0a61 7574 686f   = 0.1.12..autho
+00000020: 203d 2030 2e31 2e31 330d 0a61 7574 686f   = 0.1.13..autho
 00000030: 7220 3d20 4c75 6973 2046 696c 6970 6520  r = Luis Filipe 
 00000040: 4361 7272 6574 652c 204d 616e 7565 6c20  Carrete, Manuel 
 00000050: 4361 7374 616e 6172 6573 2c20 456e 7269  Castanares, Enri
 00000060: 636f 2044 616d 6961 6e69 2c20 4c65 6f6e  co Damiani, Leon
 00000070: 6172 646f 204d 616c 7461 0d0a 6465 7363  ardo Malta..desc
 00000080: 7269 7074 696f 6e20 3d20 416e 2065 6e76  ription = An env
 00000090: 6972 6f6e 6d65 6e74 2074 6f20 7472 6169  ironment to trai
```

### Comparing `DSSE-0.1.12/src/DSSE/env.py` & `DSSE-0.1.13/src/DSSE/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,23 +248,17 @@
                 terminations[i] = is_terminal
                 truncations[i] = is_terminal
 
             elif drone_action == 4:  # search
                 isSearching = True
 
             if drone_x == self.person_x and drone_y == self.person_y and isSearching:
-                rewards = {
-                    a: self.reward_scheme["search_and_find"]
-                       + self.reward_scheme["search_and_find"]
-                       * (1 - self.timestep / self.timestep_limit)
-                    for a in self.agents
-                }
+                rewards[i] = self.reward_scheme["search_and_find"] + self.reward_scheme["search_and_find"] * (1 - self.timestep / self.timestep_limit)
                 terminations = {a: True for a in self.agents}
                 truncations = {a: True for a in self.agents}
-                self.agents = []
                 person_found = True
 
             elif isSearching:
                 prob_matrix = self.probability_matrix.get_matrix()
                 rewards[i] = prob_matrix[drone_y][drone_x] * 10000 if prob_matrix[drone_y][drone_x] * 100 > 1 else -100
 
             # Check truncation conditions (overwrites termination conditions)
@@ -323,14 +317,15 @@
             self.person_img = pygame.image.load(
                 os.path.dirname(__file__)+"/imgs/person-swimming.png"
             ).convert()
             self.person_img = pygame.transform.scale(
                 self.person_img, (self.block_size, self.block_size)
             )
 
+
             self.renderOn = True
 
     def render(self):
         """Renders the environment."""
         self.enable_render(self.render_mode)
         self.draw()
         if self.render_mode == "human":
@@ -447,8 +442,8 @@
     @functools.lru_cache(maxsize=None)
     def observation_space(self, agent):
         # TODO: If x and y are the observation, then this should the observation space
         return MultiDiscrete([self.grid_size] * 2)
 
     @functools.lru_cache(maxsize=None)
     def action_space(self, agent):
-        return [0, 1, 2, 3, 4]
+        return [0, 1, 2, 3, 4]
```

### Comparing `DSSE-0.1.12/src/DSSE/generator/dynamic_probability.py` & `DSSE-0.1.13/src/DSSE/generator/dynamic_probability.py`

 * *Files identical despite different names*

### Comparing `DSSE-0.1.12/src/DSSE/generator/map.py` & `DSSE-0.1.13/src/DSSE/generator/map.py`

 * *Files identical despite different names*

### Comparing `DSSE-0.1.12/src/DSSE/imgs/drone.png` & `DSSE-0.1.13/src/DSSE/imgs/drone.png`

 * *Files identical despite different names*

### Comparing `DSSE-0.1.12/src/DSSE/imgs/person-swimming.png` & `DSSE-0.1.13/src/DSSE/imgs/person-swimming.png`

 * *Files identical despite different names*

### Comparing `DSSE-0.1.12/src/DSSE.egg-info/PKG-INFO` & `DSSE-0.1.13/src/DSSE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DSSE
-Version: 0.1.12
+Version: 0.1.13
 Summary: An environment to train drones to search and find a shipwrecked person lost in the ocean using reinforcement learning.
 Home-page: https://github.com/PFE-Embraer/drone-swarm-search
 Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

