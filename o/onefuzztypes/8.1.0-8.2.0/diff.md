# Comparing `tmp/onefuzztypes-8.1.0.tar.gz` & `tmp/onefuzztypes-8.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/onefuzztypes-8.1.0.tar", last modified: Mon May  8 15:53:18 2023, max compression
+gzip compressed data, was "dist/onefuzztypes-8.2.0.tar", last modified: Wed May 24 18:19:51 2023, max compression
```

## Comparing `onefuzztypes-8.1.0.tar` & `onefuzztypes-8.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/onefuzztypes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/_monkeypatch.py
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/consts.py
--rw-r--r--   0 runner    (1001) docker     (122)    11453 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     8396 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/events.py
--rw-r--r--   0 runner    (1001) docker     (122)     5118 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/job_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)    25305 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/primitives.py
--rw-r--r--   0 runner    (1001) docker     (122)     5829 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/requests.py
--rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/responses.py
--rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/validators.py
--rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/onefuzztypes/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/onefuzztypes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/onefuzztypes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      768 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/onefuzztypes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/onefuzztypes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/onefuzztypes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/onefuzztypes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/onefuzztypes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/requirements-lint.txt
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1366 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 15:53:18.000000 onefuzztypes-8.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      556 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/tests/test_alnum_filter.py
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/tests/test_container_def.py
--rw-r--r--   0 runner    (1001) docker     (122)      979 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/tests/test_instance_config_update.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2820 2023-05-08 15:53:16.000000 onefuzztypes-8.1.0/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 18:19:51.000000 onefuzztypes-8.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-05-24 18:19:51.000000 onefuzztypes-8.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 18:19:51.000000 onefuzztypes-8.2.0/onefuzztypes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/_monkeypatch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/consts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11852 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8387 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5118 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/job_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25283 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5821 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/requests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/responses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/validators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/onefuzztypes/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 18:19:51.000000 onefuzztypes-8.2.0/onefuzztypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-05-24 18:19:50.000000 onefuzztypes-8.2.0/onefuzztypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      768 2023-05-24 18:19:51.000000 onefuzztypes-8.2.0/onefuzztypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 18:19:50.000000 onefuzztypes-8.2.0/onefuzztypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 18:19:50.000000 onefuzztypes-8.2.0/onefuzztypes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-24 18:19:50.000000 onefuzztypes-8.2.0/onefuzztypes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-24 18:19:50.000000 onefuzztypes-8.2.0/onefuzztypes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/requirements-lint.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-24 18:19:51.000000 onefuzztypes-8.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1366 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 18:19:51.000000 onefuzztypes-8.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      556 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/tests/test_alnum_filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/tests/test_container_def.py
+-rw-r--r--   0 runner    (1001) docker     (122)      979 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/tests/test_instance_config_update.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2947 2023-05-24 18:19:48.000000 onefuzztypes-8.2.0/tests/test_models.py
```

### Comparing `onefuzztypes-8.1.0/PKG-INFO` & `onefuzztypes-8.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzztypes
-Version: 8.1.0
+Version: 8.2.0
 Summary: Onefuzz Types Library
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # Python types used by OneFuzz
```

### Comparing `onefuzztypes-8.1.0/README.md` & `onefuzztypes-8.2.0/README.md`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.1.0/onefuzztypes/_monkeypatch.py` & `onefuzztypes-8.2.0/onefuzztypes/_monkeypatch.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.1.0/onefuzztypes/enums.py` & `onefuzztypes-8.2.0/onefuzztypes/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,14 +277,25 @@
     TASK_FAILED = 468
     INVALID_NODE = 469
     NOTIFICATION_FAILURE = 470
     UNABLE_TO_UPDATE = 471
     PROXY_FAILED = 472
     INVALID_CONFIGURATION = 473
     UNABLE_TO_CREATE_CONTAINER = 474
+    UNABLE_TO_DOWNLOAD_FILE = 475
+    VM_UPDATE_FAILED = 476
+    UNSUPPORTED_FIELD_OPERATION = 477
+    ADO_VALIDATION_INVALID_PAT = 478
+    ADO_VALIDATION_INVALID_FIELDS = 479
+    GITHUB_VALIDATION_INVALID_PAT = 480
+    GITHUB_VALIDATION_INVALID_REPOSITORY = 481
+    UNEXPECTED_DATA_SHAPE = 482
+    UNABLE_TO_SEND = 483
+    NODE_DELETED = 484
+    # NB: if you update this enum, also update Enums.cs
 
 
 class HeartbeatType(Enum):
     MachineAlive = "MachineAlive"
     TaskAlive = "TaskAlive"
```

### Comparing `onefuzztypes-8.1.0/onefuzztypes/events.py` & `onefuzztypes-8.2.0/onefuzztypes/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,35 +94,35 @@
 
 
 class EventPing(BaseEvent, BaseResponse):
     ping_id: UUID
 
 
 class EventScalesetCreated(BaseEvent):
-    scaleset_id: UUID
+    scaleset_id: str
     pool_name: PoolName
     vm_sku: str
     image: str
     region: Region
     size: int
 
 
 class EventScalesetFailed(BaseEvent):
-    scaleset_id: UUID
+    scaleset_id: str
     pool_name: PoolName
     error: Error
 
 
 class EventScalesetDeleted(BaseEvent):
-    scaleset_id: UUID
+    scaleset_id: str
     pool_name: PoolName
 
 
 class EventScalesetResizeScheduled(BaseEvent):
-    scaleset_id: UUID
+    scaleset_id: str
     pool_name: PoolName
     size: int
 
 
 class EventPoolDeleted(BaseEvent):
     pool_name: PoolName
 
@@ -155,40 +155,40 @@
     region: Region
     proxy_id: UUID
     state: VmState
 
 
 class EventNodeCreated(BaseEvent):
     machine_id: UUID
-    scaleset_id: Optional[UUID]
+    scaleset_id: Optional[str]
     pool_name: PoolName
 
 
 class EventNodeHeartbeat(BaseEvent):
     machine_id: UUID
-    scaleset_id: Optional[UUID]
+    scaleset_id: Optional[str]
     pool_name: PoolName
     machine_state: Optional[NodeState]
 
 
 class EventNodeDeleted(BaseEvent):
     machine_id: UUID
-    scaleset_id: Optional[UUID]
+    scaleset_id: Optional[str]
     pool_name: PoolName
 
 
 class EventScalesetStateUpdated(BaseEvent):
-    scaleset_id: UUID
+    scaleset_id: str
     pool_name: PoolName
     state: ScalesetState
 
 
 class EventNodeStateUpdated(BaseEvent):
     machine_id: UUID
-    scaleset_id: Optional[UUID]
+    scaleset_id: Optional[str]
     pool_name: PoolName
     state: NodeState
 
 
 class EventCrashReported(BaseEvent):
     report: Report
     container: Container
```

### Comparing `onefuzztypes-8.1.0/onefuzztypes/job_templates.py` & `onefuzztypes-8.2.0/onefuzztypes/job_templates.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.1.0/onefuzztypes/models.py` & `onefuzztypes-8.2.0/onefuzztypes/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,15 @@
     project: str
     type: str
     unique_fields: List[str]
     comment: Optional[str]
     ado_fields: Dict[str, str]
     on_duplicate: ADODuplicateTemplate
 
-    # validator needed for backward compatibility
+    # validator needed to convert auth_token to SecretData
     @validator("auth_token", pre=True, always=True)
     def validate_auth_token(cls, v: Any) -> SecretData:
         if isinstance(v, str):
             return SecretData(secret=v)
         elif isinstance(v, SecretData):
             return v
         elif isinstance(v, dict):
@@ -283,15 +283,15 @@
         else:
             raise TypeError(f"invalid datatype {type(v)}")
 
 
 class TeamsTemplate(BaseModel):
     url: SecretData[str]
 
-    # validator needed for backward compatibility
+    # validator needed to convert url to SecretData
     @validator("url", pre=True, always=True)
     def validate_url(cls, v: Any) -> SecretData:
         if isinstance(v, str):
             return SecretData(secret=v)
         elif isinstance(v, SecretData):
             return v
         elif isinstance(v, dict):
@@ -491,15 +491,15 @@
     title: str = Field(min_length=1)
     body: str
     unique_search: GithubIssueSearch
     assignees: List[str]
     labels: List[str]
     on_duplicate: GithubIssueDuplicate
 
-    # validator needed for backward compatibility
+    # validator needed to convert auth to SecretData
     @validator("auth", pre=True, always=True)
     def validate_auth(cls, v: Any) -> SecretData:
         def try_parse_GithubAuth(x: dict) -> Optional[GithubAuth]:
             try:
                 return GithubAuth.parse_obj(x)
             except Exception:
                 return None
@@ -600,26 +600,26 @@
 
     # Set only once, when a node is initialized.
     initialized_at: Optional[datetime]
     pool_name: PoolName
     pool_id: Optional[UUID]
     machine_id: UUID
     state: NodeState = Field(default=NodeState.init)
-    scaleset_id: Optional[UUID] = None
+    scaleset_id: Optional[str] = None
     tasks: Optional[List[NodeTasks]] = None
     messages: Optional[List[NodeCommand]] = None
     heartbeat: Optional[datetime]
     version: str = Field(default="1.0.0")
     reimage_requested: bool = Field(default=False)
     delete_requested: bool = Field(default=False)
     debug_keep_node: bool = Field(default=False)
 
 
 class ScalesetSummary(BaseModel):
-    scaleset_id: UUID
+    scaleset_id: str
     state: ScalesetState
 
 
 class AutoScaleConfig(BaseModel):
     image: str
     max_size: int = Field(default=1000, le=1000, ge=0)  # max size of pool
     min_size: int = Field(default=0, le=1000, ge=0)  # min size of pool
@@ -664,15 +664,15 @@
     instance_id: str
     state: Optional[NodeState]
 
 
 class Scaleset(BaseModel):
     timestamp: Optional[datetime] = Field(alias="Timestamp")
     pool_name: PoolName
-    scaleset_id: UUID = Field(default_factory=uuid4)
+    scaleset_id: str
     state: ScalesetState = Field(default=ScalesetState.init)
     auth: Optional[Authentication]
     vm_sku: str
     image: str
     region: Region
     size: int = Field(ge=0)
     spot_instances: bool
@@ -682,15 +682,15 @@
     nodes: Optional[List[ScalesetNodeState]]
     client_id: Optional[UUID]
     client_object_id: Optional[UUID]
     tags: Dict[str, str] = Field(default_factory=lambda: {})
 
 
 class AutoScale(BaseModel):
-    scaleset_id: UUID
+    scaleset_id: str
     min: int = Field(ge=0)
     max: int = Field(ge=1)
     default: int = Field(ge=0)
     scale_out_amount: int = Field(ge=1)
     scale_out_cooldown: int = Field(ge=1)
     scale_in_amount: int = Field(ge=1)
     scale_in_cooldown: int = Field(ge=1)
@@ -808,15 +808,15 @@
     timestamp: Optional[datetime]
     event_data: str
     event_type: str
 
 
 class NodeAssignment(BaseModel):
     node_id: UUID
-    scaleset_id: Optional[UUID]
+    scaleset_id: Optional[str]
     state: NodeTaskState
 
 
 class Task(BaseModel):
     timestamp: Optional[datetime] = Field(alias="Timestamp")
     job_id: UUID
     task_id: UUID = Field(default_factory=uuid4)
```

### Comparing `onefuzztypes-8.1.0/onefuzztypes/primitives.py` & `onefuzztypes-8.2.0/onefuzztypes/primitives.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.1.0/onefuzztypes/requests.py` & `onefuzztypes-8.2.0/onefuzztypes/requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
 class AgentRegistrationGet(BaseRequest):
     machine_id: UUID
 
 
 class AgentRegistrationPost(BaseRequest):
     pool_name: PoolName
-    scaleset_id: Optional[UUID]
+    scaleset_id: Optional[str]
     machine_id: UUID
     version: str = Field(default="1.0.0")
 
 
 class PoolCreate(BaseRequest):
     name: PoolName
     os: OS
@@ -118,15 +118,15 @@
 
 class PoolStop(BaseRequest):
     name: PoolName
     now: bool
 
 
 class ProxyGet(BaseRequest):
-    scaleset_id: Optional[UUID]
+    scaleset_id: Optional[str]
     machine_id: Optional[UUID]
     dst_port: Optional[int]
 
     @root_validator()
     def check_proxy_get(cls, value: Any) -> Any:
         check_keys = ["scaleset_id", "machine_id", "dst_port"]
         included = [x in value for x in check_keys]
@@ -135,55 +135,55 @@
                 "ProxyGet must provide all or none of the following: %s"
                 % ", ".join(check_keys)
             )
         return value
 
 
 class ProxyCreate(BaseRequest):
-    scaleset_id: UUID
+    scaleset_id: str
     machine_id: UUID
     dst_port: int
     duration: int = Field(ge=ONE_HOUR, le=SEVEN_DAYS)
 
 
 class ProxyDelete(BaseRequest):
-    scaleset_id: UUID
+    scaleset_id: str
     machine_id: UUID
     dst_port: Optional[int]
 
 
 class NodeSearch(BaseRequest):
     machine_id: Optional[UUID]
     state: Optional[List[NodeState]]
-    scaleset_id: Optional[UUID]
+    scaleset_id: Optional[str]
     pool_name: Optional[PoolName]
 
 
 class NodeGet(BaseRequest):
     machine_id: UUID
 
 
 class NodeUpdate(BaseRequest):
     machine_id: UUID
     debug_keep_node: Optional[bool]
 
 
 class ScalesetSearch(BaseRequest):
-    scaleset_id: Optional[UUID]
+    scaleset_id: Optional[str]
     state: Optional[List[ScalesetState]]
     include_auth: bool = Field(default=False)
 
 
 class ScalesetStop(BaseRequest):
-    scaleset_id: UUID
+    scaleset_id: str
     now: bool
 
 
 class ScalesetUpdate(BaseRequest):
-    scaleset_id: UUID
+    scaleset_id: str
     size: Optional[int] = Field(ge=1)
 
 
 class AutoScaleOptions(BaseModel):
     min: int = Field(ge=0)
     max: int = Field(ge=1)
     default: int = Field(ge=0)
```

### Comparing `onefuzztypes-8.1.0/onefuzztypes/responses.py` & `onefuzztypes-8.2.0/onefuzztypes/responses.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.1.0/onefuzztypes/validators.py` & `onefuzztypes-8.2.0/onefuzztypes/validators.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.1.0/onefuzztypes/webhooks.py` & `onefuzztypes-8.2.0/onefuzztypes/webhooks.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.1.0/onefuzztypes.egg-info/PKG-INFO` & `onefuzztypes-8.2.0/onefuzztypes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzztypes
-Version: 8.1.0
+Version: 8.2.0
 Summary: Onefuzz Types Library
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # Python types used by OneFuzz
```

### Comparing `onefuzztypes-8.1.0/onefuzztypes.egg-info/SOURCES.txt` & `onefuzztypes-8.2.0/onefuzztypes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.1.0/setup.py` & `onefuzztypes-8.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.1.0/tests/test_alnum_filter.py` & `onefuzztypes-8.2.0/tests/test_alnum_filter.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.1.0/tests/test_container_def.py` & `onefuzztypes-8.2.0/tests/test_container_def.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.1.0/tests/test_instance_config_update.py` & `onefuzztypes-8.2.0/tests/test_instance_config_update.py`

 * *Files identical despite different names*

### Comparing `onefuzztypes-8.1.0/tests/test_models.py` & `onefuzztypes-8.2.0/tests/test_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,33 +50,36 @@
             NotificationCreate.parse_obj(missing_container)
 
 
 class TestScaleset(unittest.TestCase):
     def test_scaleset_size(self) -> None:
         with self.assertRaises(ValueError):
             Scaleset(
+                scaleset_id="test-pool-000",
                 pool_name=PoolName("test-pool"),
                 vm_sku="Standard_D2ds_v4",
                 image="Canonical:0001-com-ubuntu-server-focal:20_04-lts:latest",
                 region=Region("westus2"),
                 size=-1,
                 spot_instances=False,
             )
 
         scaleset = Scaleset(
+            scaleset_id="test-pool-000",
             pool_name=PoolName("test-pool"),
             vm_sku="Standard_D2ds_v4",
             image="Canonical:0001-com-ubuntu-server-focal:20_04-lts:latest",
             region=Region("westus2"),
             size=0,
             spot_instances=False,
         )
         self.assertEqual(scaleset.size, 0)
 
         scaleset = Scaleset(
+            scaleset_id="test-pool-000",
             pool_name=PoolName("test-pool"),
             vm_sku="Standard_D2ds_v4",
             image="Canonical:0001-com-ubuntu-server-focal:20_04-lts:latest",
             region=Region("westus2"),
             size=80,
             spot_instances=False,
         )
```

