# Comparing `tmp/generation_models-0.2.0.tar.gz` & `tmp/generation_models-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generation_models-0.2.0.tar", max compression
+gzip compressed data, was "generation_models-0.2.1.tar", max compression
```

## Comparing `generation_models-0.2.0.tar` & `generation_models-0.2.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    33527 2023-05-12 21:53:55.261646 generation_models-0.2.0/generation_models.py
--rw-r--r--   0        0        0      600 2023-05-12 22:00:03.663359 generation_models-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 generation_models-0.2.0/setup.py
--rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 generation_models-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    34110 2023-05-25 19:28:19.185968 generation_models-0.2.1/generation_models.py
+-rw-r--r--   0        0        0      600 2023-05-25 19:28:11.792032 generation_models-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 generation_models-0.2.1/setup.py
+-rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 generation_models-0.2.1/PKG-INFO
```

### Comparing `generation_models-0.2.0/generation_models.py` & `generation_models-0.2.1/generation_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,18 @@
 
     @validator("initial_mip_gap_tolerance", "secondary_mip_gap_tolerance")
     def validate_mip_gaps(cls, v):
         assert 0 <= v < 1, f"mip_gap must be between 0 and 1, got {v}."
         return v
 
 
-class StorageType(str, Enum):
+class StorageCoupling(str, Enum):
     ac = "ac"
     dc = "dc"
+    hv_ac = "hv_ac"
 
 
 class SingleAxisTracking(BaseModel):
     tracking_type: t.Optional[t.Literal["SAT"]] = "SAT"
     rotation_limit: float = 45.0
     backtrack: bool = True
 
@@ -592,14 +593,33 @@
         )
         return values
 
     def __len__(self) -> int:
         return len(self.production_override)
 
 
+class Bus(str, Enum):
+    DC = "DC"
+    MV = "MV"
+    HV = "HV"
+
+
+class DownstreamSystem(BaseModel):
+    losses: ACLosses  # still only ACLosses if modeling from inverter input, since almost every DC loss pertains to PV.
+    system_design: BaseSystemDesign
+    model_losses_from: Bus
+    inverter: t.Optional[InverterTypes]
+
+    @root_validator(skip_on_failure=True)
+    def inverter_only_if_dc(cls, values):
+        if values["inverter"] is not None:
+            assert values["model_losses_from"] == Bus.DC, "model_losses_from must be 'DC' if inverter is provided"
+        return values
+
+
 class ACExternalGenerationModel(ExternalGenerationModel):
     generation_type: t.Optional[t.Literal["ExternalAC"]] = "ExternalAC"
     losses: ACLosses = ACLosses()
     production_override: ACProductionProfile
 
 
 class DCExternalGenerationModel(ExternalGenerationModel):
@@ -771,20 +791,14 @@
     def check_battery_terms(cls, v):
         if len(v) > 1:  # don't worry about terms if there's only one battery
             for battery in v:
                 assert battery.term, "if multiple batteries are provided, terms must also be provided"
         return v
 
 
-class StorageCoupling(str, Enum):
-    ac = "ac"
-    dc = "dc"
-    hv_ac = "hv_ac"
-
-
 def _get_price_str_and_price(values):
     if isinstance(values["energy_prices"], (DARTPrices, DARTPriceScenarios)):
         return "rtm prices", values["energy_prices"].rtm
     return "energy_prices", values["energy_prices"]
 
 
 class PeakWindow(BaseModel):
@@ -912,14 +926,15 @@
     def check_sym_reg_inputs(cls, values):
         return _check_symmetric_reg_inputs(values)
 
 
 class StandaloneStorageModel(ProjectTermMixin, ImportExportLimitMixin, MarketBase):
     project_type: t.Optional[t.Literal["storage"]] = "storage"
     storage_inputs: MultiStorageInputs
+    downstream_system: t.Optional[DownstreamSystem]
     ambient_temp: t.Optional[t.List[float]]
 
     @root_validator(skip_on_failure=True)
     def check_ambient_temp_length(cls, values):
         if values["ambient_temp"]:
             price_str, price = _get_price_str_and_price(values)
             _check_lengths({price_str: price, "ambient_temp": values["ambient_temp"]})
```

### Comparing `generation_models-0.2.0/pyproject.toml` & `generation_models-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "generation-models"
-version = "0.2.0"
+version = "0.2.1"
 description = "generation API data model"
 authors = ["battery_al <allenlawrence94@gmail.com>"]
 packages = [{include = "generation_models.py"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.5.1"
```

### Comparing `generation_models-0.2.0/setup.py` & `generation_models-0.2.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 modules = \
 ['generation_models']
 install_requires = \
 ['pydantic>=1.5.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'generation-models',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'generation API data model',
     'long_description': 'None',
     'author': 'battery_al',
     'author_email': 'allenlawrence94@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

