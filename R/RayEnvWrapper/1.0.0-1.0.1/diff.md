# Comparing `tmp/RayEnvWrapper-1.0.0.tar.gz` & `tmp/RayEnvWrapper-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RayEnvWrapper-1.0.0.tar", last modified: Sat Jan 22 19:04:55 2022, max compression
+gzip compressed data, was "RayEnvWrapper-1.0.1.tar", last modified: Thu May 25 19:57:52 2023, max compression
```

## Comparing `RayEnvWrapper-1.0.0.tar` & `RayEnvWrapper-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ingambe    (501) staff       (20)        0 2022-01-22 19:04:55.575535 RayEnvWrapper-1.0.0/
--rw-r--r--   0 ingambe    (501) staff       (20)    18264 2022-01-22 18:58:55.000000 RayEnvWrapper-1.0.0/LICENSE
--rw-r--r--   0 ingambe    (501) staff       (20)      471 2022-01-22 19:04:55.575438 RayEnvWrapper-1.0.0/PKG-INFO
--rw-r--r--   0 ingambe    (501) staff       (20)     4215 2022-01-22 19:00:00.000000 RayEnvWrapper-1.0.0/README.md
-drwxr-xr-x   0 ingambe    (501) staff       (20)        0 2022-01-22 19:04:55.574672 RayEnvWrapper-1.0.0/RayEnvWrapper/
--rw-r--r--   0 ingambe    (501) staff       (20)     6074 2022-01-21 14:33:11.000000 RayEnvWrapper-1.0.0/RayEnvWrapper/CustomRayRemoteEnv.py
--rw-r--r--   0 ingambe    (501) staff       (20)     1599 2022-01-22 18:06:32.000000 RayEnvWrapper-1.0.0/RayEnvWrapper/CustomWrapperRayVecEnv.py
--rw-r--r--   0 ingambe    (501) staff       (20)      136 2022-01-21 14:41:01.000000 RayEnvWrapper-1.0.0/RayEnvWrapper/__init__.py
-drwxr-xr-x   0 ingambe    (501) staff       (20)        0 2022-01-22 19:04:55.575308 RayEnvWrapper-1.0.0/RayEnvWrapper.egg-info/
--rw-r--r--   0 ingambe    (501) staff       (20)      471 2022-01-22 19:04:55.000000 RayEnvWrapper-1.0.0/RayEnvWrapper.egg-info/PKG-INFO
--rw-r--r--   0 ingambe    (501) staff       (20)      312 2022-01-22 19:04:55.000000 RayEnvWrapper-1.0.0/RayEnvWrapper.egg-info/SOURCES.txt
--rw-r--r--   0 ingambe    (501) staff       (20)        1 2022-01-22 19:04:55.000000 RayEnvWrapper-1.0.0/RayEnvWrapper.egg-info/dependency_links.txt
--rw-r--r--   0 ingambe    (501) staff       (20)       43 2022-01-22 19:04:55.000000 RayEnvWrapper-1.0.0/RayEnvWrapper.egg-info/requires.txt
--rw-r--r--   0 ingambe    (501) staff       (20)       14 2022-01-22 19:04:55.000000 RayEnvWrapper-1.0.0/RayEnvWrapper.egg-info/top_level.txt
--rw-r--r--   0 ingambe    (501) staff       (20)       38 2022-01-22 19:04:55.575568 RayEnvWrapper-1.0.0/setup.cfg
--rw-r--r--   0 ingambe    (501) staff       (20)      661 2022-01-22 18:37:51.000000 RayEnvWrapper-1.0.0/setup.py
+drwxr-xr-x   0 ingambe    (501) staff       (20)        0 2023-05-25 19:57:52.049630 RayEnvWrapper-1.0.1/
+-rw-r--r--   0 ingambe    (501) staff       (20)    18264 2023-05-25 15:27:04.000000 RayEnvWrapper-1.0.1/LICENSE
+-rw-r--r--   0 ingambe    (501) staff       (20)     4683 2023-05-25 19:57:52.049503 RayEnvWrapper-1.0.1/PKG-INFO
+-rw-r--r--   0 ingambe    (501) staff       (20)     4215 2023-05-25 15:27:04.000000 RayEnvWrapper-1.0.1/README.md
+drwxr-xr-x   0 ingambe    (501) staff       (20)        0 2023-05-25 19:57:52.048656 RayEnvWrapper-1.0.1/RayEnvWrapper/
+-rw-r--r--   0 ingambe    (501) staff       (20)     6095 2023-05-25 17:48:01.000000 RayEnvWrapper-1.0.1/RayEnvWrapper/CustomRayRemoteEnv.py
+-rw-r--r--   0 ingambe    (501) staff       (20)     1599 2023-05-25 15:27:04.000000 RayEnvWrapper-1.0.1/RayEnvWrapper/CustomWrapperRayVecEnv.py
+-rw-r--r--   0 ingambe    (501) staff       (20)      136 2023-05-25 15:27:04.000000 RayEnvWrapper-1.0.1/RayEnvWrapper/__init__.py
+drwxr-xr-x   0 ingambe    (501) staff       (20)        0 2023-05-25 19:57:52.049314 RayEnvWrapper-1.0.1/RayEnvWrapper.egg-info/
+-rw-r--r--   0 ingambe    (501) staff       (20)     4683 2023-05-25 19:57:52.000000 RayEnvWrapper-1.0.1/RayEnvWrapper.egg-info/PKG-INFO
+-rw-r--r--   0 ingambe    (501) staff       (20)      312 2023-05-25 19:57:52.000000 RayEnvWrapper-1.0.1/RayEnvWrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 ingambe    (501) staff       (20)        1 2023-05-25 19:57:52.000000 RayEnvWrapper-1.0.1/RayEnvWrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 ingambe    (501) staff       (20)       43 2023-05-25 19:57:52.000000 RayEnvWrapper-1.0.1/RayEnvWrapper.egg-info/requires.txt
+-rw-r--r--   0 ingambe    (501) staff       (20)       14 2023-05-25 19:57:52.000000 RayEnvWrapper-1.0.1/RayEnvWrapper.egg-info/top_level.txt
+-rw-r--r--   0 ingambe    (501) staff       (20)       38 2023-05-25 19:57:52.049673 RayEnvWrapper-1.0.1/setup.cfg
+-rw-r--r--   0 ingambe    (501) staff       (20)      842 2023-05-25 19:55:48.000000 RayEnvWrapper-1.0.1/setup.py
```

### Comparing `RayEnvWrapper-1.0.0/LICENSE` & `RayEnvWrapper-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `RayEnvWrapper-1.0.0/README.md` & `RayEnvWrapper-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `RayEnvWrapper-1.0.0/RayEnvWrapper/CustomRayRemoteEnv.py` & `RayEnvWrapper-1.0.1/RayEnvWrapper/CustomRayRemoteEnv.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,16 @@
         self.num_envs = num_workers * env_per_worker
         self.multiagent = multiagent
         self.poll_timeout = None
 
         self.actors = None  # lazy init
         self.pending = None  # lazy init
 
-        self.observation_space = self.local_env.observation_space
-        self.keys, shapes, dtypes = obs_space_info(self.observation_space)
+        #self.observation_space = self.local_env.observation_space
+        self.keys, shapes, dtypes = obs_space_info(self.local_env.observation_space)
 
         self.buf_obs = OrderedDict(
             [(k, np.zeros((self.num_envs,) + tuple(shapes[k]), dtype=dtypes[k])) for k in self.keys])
         self.buf_dones = np.zeros((self.num_envs,), dtype=bool)
         self.buf_rews = np.zeros((self.num_envs,), dtype=np.float32)
         self.buf_infos = [{} for _ in range(self.num_envs)]
 
@@ -89,15 +89,15 @@
             self._save_obs(env_id, ob)
             self.buf_rews[env_id * self.env_per_worker: (env_id + 1) * self.env_per_worker] = rew
             self.buf_dones[env_id * self.env_per_worker: (env_id + 1) * self.env_per_worker] = done
             self.buf_infos[env_id * self.env_per_worker: (env_id + 1) * self.env_per_worker] = info
         return (self._obs_from_buf(), np.copy(self.buf_rews), np.copy(self.buf_dones), deepcopy(self.buf_infos))
 
     def _obs_from_buf(self) -> VecEnvObs:
-        return dict_to_obs(self.observation_space, copy_obs_dict(self.buf_obs))
+        return dict_to_obs(self.local_env.observation_space, copy_obs_dict(self.buf_obs))
 
     @PublicAPI
     def send_actions(self, action_list) -> None:
         for worker_id in range(self.num_workers):
             actions = action_list[worker_id * self.env_per_worker: (worker_id + 1) * self.env_per_worker]
             actor = self.actors[worker_id]
             obj_ref = actor.step.remote(actions)
```

### Comparing `RayEnvWrapper-1.0.0/RayEnvWrapper/CustomWrapperRayVecEnv.py` & `RayEnvWrapper-1.0.1/RayEnvWrapper/CustomWrapperRayVecEnv.py`

 * *Files identical despite different names*

