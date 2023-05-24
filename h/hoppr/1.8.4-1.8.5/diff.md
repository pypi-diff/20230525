# Comparing `tmp/hoppr-1.8.4.tar.gz` & `tmp/hoppr-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr-1.8.4.tar", max compression
+gzip compressed data, was "hoppr-1.8.5.tar", max compression
```

## Comparing `hoppr-1.8.4.tar` & `hoppr-1.8.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1084 2023-04-26 14:25:36.000000 hoppr-1.8.4/LICENSE
--rw-r--r--   0        0        0     1214 2023-04-26 14:25:36.000000 hoppr-1.8.4/README.md
--rw-r--r--   0        0        0     1035 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/__init__.py
--rw-r--r--   0        0        0      161 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/__main__.py
--rw-r--r--   0        0        0        0 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/base_plugins/__init__.py
--rw-r--r--   0        0        0    10990 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/base_plugins/collector.py
--rw-r--r--   0        0        0    10732 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/base_plugins/hoppr.py
--rw-r--r--   0        0        0        0 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/base_plugins/py.typed
--rw-r--r--   0        0        0        0 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/cli/__init__.py
--rw-r--r--   0        0        0     6256 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/cli/hopctl.py
--rw-r--r--   0        0        0      563 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/constants.py
--rw-r--r--   0        0        0        0 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/__init__.py
--rw-r--r--   0        0        0     3046 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/bundle_tar.py
--rw-r--r--   0        0        0    12943 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/collect_apt_plugin.py
--rw-r--r--   0        0        0    10272 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/collect_dnf_plugin.py
--rw-r--r--   0        0        0     3321 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/collect_docker_plugin.py
--rw-r--r--   0        0        0     4664 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/collect_git_plugin.py
--rw-r--r--   0        0        0     3992 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/collect_helm_plugin.py
--rw-r--r--   0        0        0     6369 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/collect_maven_plugin.py
--rw-r--r--   0        0        0     7978 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/collect_nexus_search.py
--rw-r--r--   0        0        0     4418 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/collect_pypi_plugin.py
--rw-r--r--   0        0        0     3043 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/collect_raw_plugin.py
--rw-r--r--   0        0        0     3739 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/collect_yum_plugin.py
--rw-r--r--   0        0        0     4278 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/composite_collector.py
--rw-r--r--   0        0        0     5673 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/delta_sbom.py
--rw-r--r--   0        0        0     6885 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/oras_bundle.py
--rw-r--r--   0        0        0     5301 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/oras_registry.py
--rw-r--r--   0        0        0        0 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/py.typed
--rw-r--r--   0        0        0      202 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/report_generator/__init__.py
--rw-r--r--   0        0        0   126749 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
--rw-r--r--   0        0        0     4577 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/report_generator/report_generator.py
--rw-r--r--   0        0        0    60554 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
--rw-r--r--   0        0        0      518 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/report_generator/scripts/custom.js
--rw-r--r--   0        0        0   220780 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
--rw-r--r--   0        0        0     3562 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/report_generator/styles/custom.css
--rw-r--r--   0        0        0     4810 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/report_generator/templates/component_card.jinja2
--rw-r--r--   0        0        0     1230 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
--rw-r--r--   0        0        0     7246 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/core_plugins/report_generator/templates/index.jinja2
--rw-r--r--   0        0        0      458 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/exceptions.py
--rw-r--r--   0        0        0     6847 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/in_toto.py
--rw-r--r--   0        0        0     3074 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/main.py
--rw-r--r--   0        0        0     4106 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/mem_logger.py
--rw-r--r--   0        0        0     1708 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/models/__init__.py
--rw-r--r--   0        0        0     1602 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/models/__main__.py
--rw-r--r--   0        0        0     1409 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/models/base.py
--rw-r--r--   0        0        0     4001 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/models/credentials.py
--rw-r--r--   0        0        0    17452 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/models/manifest.py
--rw-r--r--   0        0        0        0 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/models/py.typed
--rw-r--r--   0        0        0     3975 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/models/transfer.py
--rw-r--r--   0        0        0     5071 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/models/types.py
--rw-r--r--   0        0        0     2335 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/net.py
--rw-r--r--   0        0        0     4323 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/oci_artifacts.py
--rw-r--r--   0        0        0     1332 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/plugin_utils.py
--rw-r--r--   0        0        0    25929 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/processor.py
--rw-r--r--   0        0        0        0 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/py.typed
--rw-r--r--   0        0        0    22579 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/resources/hoppr-hippo-large.ansi
--rw-r--r--   0        0        0    10419 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/resources/hoppr-hippo.ansi
--rw-r--r--   0        0        0     4036 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/result.py
--rw-r--r--   0        0        0     5791 2023-04-26 14:25:36.000000 hoppr-1.8.4/hoppr/utils.py
--rw-r--r--   0        0        0     3614 2023-04-26 14:25:36.000000 hoppr-1.8.4/pyproject.toml
--rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 hoppr-1.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-05-24 23:07:22.000000 hoppr-1.8.5/LICENSE
+-rw-r--r--   0        0        0     1214 2023-05-24 23:07:22.000000 hoppr-1.8.5/README.md
+-rw-r--r--   0        0        0     1035 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/__init__.py
+-rw-r--r--   0        0        0      161 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/base_plugins/__init__.py
+-rw-r--r--   0        0        0    11010 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/base_plugins/collector.py
+-rw-r--r--   0        0        0    10707 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/base_plugins/hoppr.py
+-rw-r--r--   0        0        0        0 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/base_plugins/py.typed
+-rw-r--r--   0        0        0        0 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/cli/__init__.py
+-rw-r--r--   0        0        0     6256 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/cli/hopctl.py
+-rw-r--r--   0        0        0      563 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/constants.py
+-rw-r--r--   0        0        0        0 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/__init__.py
+-rw-r--r--   0        0        0     3046 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/bundle_tar.py
+-rw-r--r--   0        0        0    12943 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/collect_apt_plugin.py
+-rw-r--r--   0        0        0    10272 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/collect_dnf_plugin.py
+-rw-r--r--   0        0        0     3840 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/collect_docker_plugin.py
+-rw-r--r--   0        0        0     4664 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/collect_git_plugin.py
+-rw-r--r--   0        0        0     4113 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/collect_helm_plugin.py
+-rw-r--r--   0        0        0     6369 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/collect_maven_plugin.py
+-rw-r--r--   0        0        0     7961 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/collect_nexus_search.py
+-rw-r--r--   0        0        0     4418 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/collect_pypi_plugin.py
+-rw-r--r--   0        0        0     3043 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/collect_raw_plugin.py
+-rw-r--r--   0        0        0     3739 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/collect_yum_plugin.py
+-rw-r--r--   0        0        0     4278 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/composite_collector.py
+-rw-r--r--   0        0        0     5673 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/delta_sbom.py
+-rw-r--r--   0        0        0     6885 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/oras_bundle.py
+-rw-r--r--   0        0        0     5301 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/oras_registry.py
+-rw-r--r--   0        0        0        0 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/py.typed
+-rw-r--r--   0        0        0      202 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/report_generator/__init__.py
+-rw-r--r--   0        0        0   126749 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png
+-rw-r--r--   0        0        0     4606 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/report_generator/report_generator.py
+-rw-r--r--   0        0        0    60554 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js
+-rw-r--r--   0        0        0      518 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/report_generator/scripts/custom.js
+-rw-r--r--   0        0        0   220780 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/report_generator/styles/bootstrap.min.css
+-rw-r--r--   0        0        0     3562 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/report_generator/styles/custom.css
+-rw-r--r--   0        0        0     5052 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/report_generator/templates/component_card.jinja2
+-rw-r--r--   0        0        0     1230 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/report_generator/templates/general_summary.jinja2
+-rw-r--r--   0        0        0     7246 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/core_plugins/report_generator/templates/index.jinja2
+-rw-r--r--   0        0        0      458 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/exceptions.py
+-rw-r--r--   0        0        0     6847 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/in_toto.py
+-rw-r--r--   0        0        0     3074 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/main.py
+-rw-r--r--   0        0        0     4106 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/mem_logger.py
+-rw-r--r--   0        0        0     1708 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/models/__init__.py
+-rw-r--r--   0        0        0     1602 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/models/__main__.py
+-rw-r--r--   0        0        0     1409 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/models/base.py
+-rw-r--r--   0        0        0     4001 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/models/credentials.py
+-rw-r--r--   0        0        0    17448 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/models/manifest.py
+-rw-r--r--   0        0        0        0 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/models/py.typed
+-rw-r--r--   0        0        0     3975 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/models/transfer.py
+-rw-r--r--   0        0        0     5023 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/models/types.py
+-rw-r--r--   0        0        0     2335 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/net.py
+-rw-r--r--   0        0        0     4323 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/oci_artifacts.py
+-rw-r--r--   0        0        0     1332 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/plugin_utils.py
+-rw-r--r--   0        0        0    26282 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/processor.py
+-rw-r--r--   0        0        0        0 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/py.typed
+-rw-r--r--   0        0        0    22579 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/resources/hoppr-hippo-large.ansi
+-rw-r--r--   0        0        0    10419 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/resources/hoppr-hippo.ansi
+-rw-r--r--   0        0        0     4036 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/result.py
+-rw-r--r--   0        0        0     5791 2023-05-24 23:07:22.000000 hoppr-1.8.5/hoppr/utils.py
+-rw-r--r--   0        0        0     3614 2023-05-24 23:07:22.000000 hoppr-1.8.5/pyproject.toml
+-rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 hoppr-1.8.5/PKG-INFO
```

### Comparing `hoppr-1.8.4/LICENSE` & `hoppr-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/README.md` & `hoppr-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/__init__.py` & `hoppr-1.8.5/hoppr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     "Property",
     "PurlType",
     "Result",
     "Sbom",
     "Transfer",
 ]
 
-__version__ = "1.8.4"
+__version__ = "1.8.5"
```

### Comparing `hoppr-1.8.4/hoppr/base_plugins/collector.py` & `hoppr-1.8.5/hoppr/base_plugins/collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,20 +31,20 @@
 
     default_component_coverage = ComponentCoverage.EXACTLY_ONCE
     bom_access = BomAccess.COMPONENT_ACCESS
     system_repositories: list[str] = []
 
     @staticmethod
     def _get_repo_search_list(comp: Component) -> list[str]:
-        repo_list = []
+        repo_list: list[str] = []
         for prop in comp.properties or []:
             if prop.name == constants.BomProps.COMPONENT_SEARCH_SEQUENCE:
                 search_sequence_str = json.loads(prop.value or '{"version": "v1", "repositories": []}')
                 search_sequence = SearchSequence.parse_obj(search_sequence_str)
-                repo_list.extend(search_sequence.repositories)
+                repo_list.extend(map(str, search_sequence.repositories))
 
         return repo_list
 
     def _get_repos(self, comp: Component) -> list[str]:
         """
         Returns all repos listed in all BOM_PROPS_COMPONENT_SEARCH_SEQUENCE properties for this component
         """
@@ -212,15 +212,14 @@
         missing_props = []
         for req_prop in [
             constants.BomProps.COLLECTION_REPOSITORY,
             constants.BomProps.COLLECTION_DIRECTORY,
             constants.BomProps.COLLECTION_PLUGIN,
             constants.BomProps.COLLECTION_TIMETAG,
         ]:
-
             if req_prop.value not in [prop.name for prop in result.return_obj.properties or []]:
                 missing_props.append(req_prop.value)
 
         if missing_props:
             return result.fail(
                 f"Collector class {type(self).__name__} process_component method returned a successful result "
                 f"without updating the following component properties: {', '.join(missing_props)}"
@@ -238,16 +237,16 @@
     @hoppr_rerunner
     def collect(self, comp: Any, repo_url: str, creds: CredentialRequiredService | None = None):
         """
         This method should attempt to collect a single component from the specified URL
         """
 
     @final
-    @hoppr_process
     @hoppr_ignore_excluded
+    @hoppr_process
     def process_component(self, comp: Component) -> Result:
         """
         Copy a component to the local collection directory structure
 
         A CollectorPlugin will never return a RETRY result, but handles the retry logic internally.
         """
 
@@ -296,16 +295,16 @@
 
         Use of a single batch operation (i.e. dynamically constructed
         shell command) is encouraged if supported by the underlying
         collection tool(s).
         """
 
     @final
-    @hoppr_process
     @hoppr_ignore_excluded
+    @hoppr_process
     def process_component(self, comp: Component) -> Result:
         """
         Copy a component to the local collection directory structure
 
         A CollectorPlugin will never return a RETRY result, but handles the retry logic internally.
         """
         logger = self.get_logger()
```

### Comparing `hoppr-1.8.4/hoppr/base_plugins/hoppr.py` & `hoppr-1.8.5/hoppr/base_plugins/hoppr.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,21 @@
 import time
 import traceback
 
 from abc import ABC, abstractmethod
 from os import PathLike
 from typing import Any, Callable, Dict, List, Optional
 
-from packageurl import PackageURL
-
 from hoppr import plugin_utils
 from hoppr.mem_logger import MemoryLogger
 from hoppr.models import HopprContext
 from hoppr.models.transfer import ComponentCoverage
 from hoppr.models.types import BomAccess
 from hoppr.result import Result
-from hoppr.utils import obscure_passwords
+from hoppr.utils import obscure_passwords, get_package_url
 
 
 def _get_component(*args, **kwargs) -> Optional[Any]:
     # TODO: This will only utilize the first Component found in 1) args, 2) kwargs  # pylint: disable=fixme
     # and assumes all plugins operate this way
     comp = None
     for arg in args:
@@ -61,15 +59,15 @@
 
         result = None
         if comp is not None:
             if comp.purl is None:
                 result = Result.fail("No purl supplied for component")
 
             else:
-                purl_type = PackageURL.from_string(comp.purl).type
+                purl_type = get_package_url(comp.purl).type
 
                 if not self.supports_purl_type(purl_type):
                     return Result.skip(f"Class {self.__class__.__name__} does not support purl type {purl_type}")
 
                 component_header = f"{comp.name}" + (f"@{comp.version}" if comp.version is not None else "")
 
                 self.get_logger().info(
```

### Comparing `hoppr-1.8.4/hoppr/cli/hopctl.py` & `hoppr-1.8.5/hoppr/cli/hopctl.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/constants.py` & `hoppr-1.8.5/hoppr/constants.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/core_plugins/bundle_tar.py` & `hoppr-1.8.5/hoppr/core_plugins/bundle_tar.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/core_plugins/collect_apt_plugin.py` & `hoppr-1.8.5/hoppr/core_plugins/collect_apt_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/core_plugins/collect_dnf_plugin.py` & `hoppr-1.8.5/hoppr/core_plugins/collect_dnf_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/core_plugins/collect_docker_plugin.py` & `hoppr-1.8.5/hoppr/core_plugins/collect_raw_plugin.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,95 +1,87 @@
 """
-Collector plugin for docker images
+Collector plugin for raw files
 """
-from __future__ import annotations
 
-import os
-import re
-import urllib.parse
+import shutil
 
-from typing import Any
+from pathlib import Path
+from typing import Any, List
+from urllib.parse import unquote
 
 from packageurl import PackageURL
 
 from hoppr import __version__
 from hoppr.base_plugins.collector import SerialCollectorPlugin
 from hoppr.base_plugins.hoppr import hoppr_rerunner
-from hoppr.models import HopprContext
 from hoppr.models.credentials import CredentialRequiredService
+from hoppr.models.types import RepositoryUrl
+from hoppr.net import download_file
 from hoppr.result import Result
 
 
-class CollectDockerPlugin(SerialCollectorPlugin):
+class CollectRawPlugin(SerialCollectorPlugin):
     """
-    Collector plugin for docker images
+    Collector plugin for raw files
     """
 
-    supported_purl_types = ["docker"]
-    required_commands = ["skopeo"]
-    products: list[str] = ["docker/*"]
-    system_repositories: list[str] = ["https://docker.io/"]
-    process_timeout = 300
+    supported_purl_types = ["binary", "generic", "raw"]
+    products: List[str] = ["binary/*", "generic/*", "raw/*"]
 
-    def get_version(self) -> str:  # pylint: disable=duplicate-code
+    def get_version(self) -> str:
         return __version__
 
-    def __init__(self, context: HopprContext, config: dict | None = None) -> None:
-        super().__init__(context=context, config=config)
-        if self.config is not None:
-            if "skopeo_command" in self.config:
-                self.required_commands = [self.config["skopeo_command"]]
-
     @hoppr_rerunner
     def collect(self, comp: Any, repo_url: str, creds: CredentialRequiredService | None = None):
         """
         Copy a component to the local collection directory structure
         """
-        purl = PackageURL.from_string(comp.purl)
+        source_url = RepositoryUrl(url=repo_url)
 
-        source_image = os.path.join(repo_url, purl.namespace or "", purl.name + ":" + purl.version)
-        source_image = re.sub(r"^https?://", "", source_image)
+        purl = PackageURL.from_string(comp.purl)
 
-        file_name = urllib.parse.unquote(purl.name) + "_" + purl.version
-        target_dir = self.directory_for(purl.type, repo_url, subdir=purl.namespace)
-        target_path = os.path.join(target_dir, file_name)
-        destination = f'docker-archive:{target_path}:{source_image}'
+        subdir = None
+        if purl.namespace is not None:
+            source_url /= f"{purl.namespace}"
+            subdir = unquote(purl.namespace)
 
-        if not source_image.startswith("docker://"):
-            source_image = "docker://" + source_image
+        target_dir = self.directory_for(purl.type, repo_url, subdir=subdir)
 
-        self.get_logger().info(msg="Copying docker image:", indent_level=2)
-        self.get_logger().info(msg=f"source: {source_image}", indent_level=3)
-        self.get_logger().info(msg=f"destination: {destination}", indent_level=3)
+        file_name = unquote(purl.name)
 
-        command = [self.required_commands[0], "copy"]
+        if source_url.scheme == "file":
+            repo_path = Path(repo_url.removeprefix("file:").removeprefix("//"))
+            source_file = (repo_path / (purl.namespace or "") / file_name).expanduser()
 
-        password_list = []
+            self.get_logger().info(msg="Copying component:", indent_level=2)
+            self.get_logger().info(msg=f"source: {source_file}", indent_level=3)
+            self.get_logger().info(msg=f"destination: {target_dir.joinpath(file_name)}", indent_level=3)
 
-        if creds is not None:
-            password_list = [creds.password.get_secret_value()]
-            command.extend(["--src-creds", f"{creds.username}:{creds.password.get_secret_value()}"])
+            if not source_file.is_file():
+                msg = f"Unable to locate file {source_file}, skipping remaining attempts"
+                self.get_logger().error(msg=msg, indent_level=2)
+                return Result.fail(message=msg)
 
-        if re.match("^http://", repo_url):
-            command.append("--src-tls-verify=false")
+            shutil.copy(source_file, target_dir)
 
-        command.extend([source_image, destination])
+            self.set_collection_params(comp, repo_url, target_dir)
+            return Result.success(return_obj=comp)
 
-        proc = self.run_command(command, password_list)
+        download_url = source_url / file_name
 
-        if proc.returncode != 0:
-            msg = f"Skopeo failed to copy docker image to {destination}, " + f"return_code={proc.returncode}"
+        self.get_logger().info(msg="Downloading file:", indent_level=2)
+        self.get_logger().info(msg=f"source: {download_url}", indent_level=3)
+        self.get_logger().info(msg=f"destination: {target_dir.joinpath(file_name)}", indent_level=3)
 
-            self.get_logger().debug(msg=msg, indent_level=2)
+        response = download_file(f"{download_url}", str(target_dir / file_name), creds)
+        result = Result.from_http_response(response)
 
-            if os.path.exists(target_path):
-                self.get_logger().info(
-                    msg="Artifact collection failed, deleting file and retrying",
-                    indent_level=2,
-                )
-                os.remove(target_path)
+        if result.is_fail():
+            msg = f"Unable to download from {download_url}, skipping remaining attempts"
+            self.get_logger().error(msg=msg, indent_level=2)
 
-            return Result.retry(message=msg)
+        if not result.is_success():
+            return result
 
         self.set_collection_params(comp, repo_url, target_dir)
 
         return Result.success(return_obj=comp)
```

### Comparing `hoppr-1.8.4/hoppr/core_plugins/collect_git_plugin.py` & `hoppr-1.8.5/hoppr/core_plugins/collect_git_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/core_plugins/collect_helm_plugin.py` & `hoppr-1.8.5/hoppr/core_plugins/collect_helm_plugin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Collector plugin for helm charts
 """
 from __future__ import annotations
 
 from pathlib import Path
 
-from packageurl import PackageURL
+import hoppr.utils
 
-from hoppr import __version__, utils
+from hoppr import __version__
 from hoppr.base_plugins.collector import SerialCollectorPlugin
 from hoppr.base_plugins.hoppr import hoppr_rerunner
 from hoppr.exceptions import HopprLoadDataError
 from hoppr.models import HopprContext
 from hoppr.models.credentials import CredentialRequiredService
 from hoppr.models.manifest import Component
 from hoppr.models.types import RepositoryUrl
@@ -32,26 +32,23 @@
         return __version__
 
     def __init__(self, context: HopprContext, config: dict | None = None) -> None:
         super().__init__(context=context, config=config)
 
         self.create_logger()
 
-        if self.config is not None:
-            if "helm_command" in self.config:
-                self.required_commands = [self.config["helm_command"]]
-
+        self.required_commands = (self.config or {}).get("helm_command", self.required_commands)
         self.base_command = [self.required_commands[0], "fetch"]
 
         system_repos_file = Path.home() / ".config" / "helm" / "repositories.yaml"
         if not self.context.strict_repos and system_repos_file.exists():
             system_repos: list[dict[str, str]] = []
 
             try:
-                system_repos_dict = utils.load_file(input_file_path=system_repos_file)
+                system_repos_dict = hoppr.utils.load_file(input_file_path=system_repos_file)
                 if not isinstance(system_repos_dict, dict):
                     raise HopprLoadDataError("Incorrect format.")
 
                 system_repos = system_repos_dict["repositories"]
             except HopprLoadDataError as ex:
                 self.get_logger().warning(msg=f"Unable to parse Helm repositories file ({system_repos_file}): '{ex}'")
 
@@ -60,18 +57,19 @@
     @hoppr_rerunner
     # pylint: disable=duplicate-code
     def collect(self, comp: Component, repo_url: str, creds: CredentialRequiredService | None = None):
         """
         Collect helm chart
         """
 
-        purl: PackageURL = PackageURL.from_string(comp.purl)  # pyright: ignore[reportGeneralTypeIssues]
+        purl = hoppr.utils.get_package_url(comp.purl)
 
         target_dir = self.directory_for(purl.type, repo_url, subdir=f"{purl.name}_{purl.version}")
 
+        run_result = None
         for subdir in ["", purl.name]:
             source_url = RepositoryUrl(url=repo_url) / subdir
 
             self.get_logger().info(msg="Fetching helm chart:", indent_level=2)
             self.get_logger().info(msg=f"source: {source_url}", indent_level=3)
             self.get_logger().info(msg=f"destination: {target_dir}", indent_level=3)
 
@@ -103,10 +101,15 @@
 
             if run_result.returncode == 0:
                 self.get_logger().info(f"Complete helm chart artifact copy for {purl.name} version {purl.version}")
                 self.set_collection_params(comp, repo_url, target_dir)
 
                 return Result.success(return_obj=comp)
 
-        msg = f"Failed to download {purl.name} version {purl.version} helm chart"
+        msg = f"Failed to download {purl.name} version {purl.version} helm chart from {repo_url}."
+
+        if run_result is not None and "404 Not Found" in str(run_result.stderr):
+            self.get_logger().debug(msg=msg, indent_level=2)
+            return Result.fail(f"{msg} Chart not found.")
+
         self.get_logger().debug(msg=msg, indent_level=2)
         return Result.retry(msg)
```

### Comparing `hoppr-1.8.4/hoppr/core_plugins/collect_maven_plugin.py` & `hoppr-1.8.5/hoppr/core_plugins/collect_maven_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/core_plugins/collect_nexus_search.py` & `hoppr-1.8.5/hoppr/core_plugins/collect_nexus_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,22 +115,20 @@
             nexus_repo = repo_match.group(1)
             path = repo_match.group(2)
             if path is not None:
                 path = path[1:]
 
         subdir = None
         match purl.type:
-            case "docker" | "generic" | "maven" | "rpm":
+            case "docker" | "generic" | "maven" | "raw" | "rpm":
                 subdir = path
             case "helm" | "pypi":
                 subdir = f"{purl.name}_{purl.version}"
 
-        target_dir = self.directory_for(purl.type, nexus_repo, subdir=subdir)
-
-        return target_dir
+        return self.directory_for(purl.type, nexus_repo, subdir=subdir)
 
     @staticmethod
     def is_nexus_instance(repo_url: str, auth: HTTPBasicAuth | None = None) -> bool:
         """
         Checks whether or not the repo_url refers to a Nexus instance
         """
         test_url = RepositoryUrl(url=repo_url) / "service" / "rest" / "v1" / "status"
@@ -168,15 +166,15 @@
         match purl.type:
             case "deb":
                 nexus_format = "apt"
             case "gems":
                 nexus_format = "rubygems"
             case "golang":
                 nexus_format = "go"
-            case "generic":
+            case "generic" | "raw":
                 nexus_format = "raw"
             case "maven":
                 nexus_format = "maven2"
                 additional_search_params = [
                     {"maven.extension": "jar", "maven.classifier": ""},
                     {"maven.extension": "jar", "maven.classifier": "sources"},
                     {"maven.extension": "pom"},
```

### Comparing `hoppr-1.8.4/hoppr/core_plugins/collect_pypi_plugin.py` & `hoppr-1.8.5/hoppr/core_plugins/collect_pypi_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/core_plugins/collect_yum_plugin.py` & `hoppr-1.8.5/hoppr/core_plugins/collect_yum_plugin.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/core_plugins/composite_collector.py` & `hoppr-1.8.5/hoppr/core_plugins/composite_collector.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -54,16 +54,16 @@
         for plugin in self.child_plugins:
             result = plugin.pre_stage_process()
             if result.is_fail() or result.is_retry():
                 return Result.fail(f"Failure running {plugin.__class__.__name__}")
 
         return Result.success()
 
-    @hoppr_process
     @hoppr_ignore_excluded
+    @hoppr_process
     def process_component(self, comp: Any) -> Result:  # pylint: disable=unused-argument
         """
         Run component through each child plugin component processes
         """
 
         for plugin in self.child_plugins:
             self._log_and_flush(f"Attempting to process {comp.purl} using {plugin.__class__.__name__}")
```

### Comparing `hoppr-1.8.4/hoppr/core_plugins/delta_sbom.py` & `hoppr-1.8.5/hoppr/core_plugins/delta_sbom.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/core_plugins/oras_bundle.py` & `hoppr-1.8.5/hoppr/core_plugins/oras_bundle.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/core_plugins/oras_registry.py` & `hoppr-1.8.5/hoppr/core_plugins/oras_registry.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png` & `hoppr-1.8.5/hoppr/core_plugins/report_generator/assets/hoppr_hippo.png`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/core_plugins/report_generator/report_generator.py` & `hoppr-1.8.5/hoppr/core_plugins/report_generator/report_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """
 Report Generating Plugin
 """
 
-import json
 import shutil
 
 from pathlib import Path
 from typing import Any, Optional
 from uuid import UUID
 
 import typer
 
 from jinja2 import Environment, FileSystemLoader
 
 from hoppr import __version__
 from hoppr.base_plugins.hoppr import HopprPlugin
-from hoppr.models.manifest import Component
+from hoppr.models.manifest import Component, SearchSequence
 from hoppr.result import ResultStatus
 
 
 class Report:  # pylint: disable=too-few-public-methods
     """
     A report of a plugin's execution stage result.
     """
@@ -88,15 +87,15 @@
             "report_count": report_count,
             "error_count": error_count,
             "reports_by_stage": reports_by_stage,
             "reports_by_plugin": reports_by_plugin,
             "ResultStatus": ResultStatus,
             "get_type": type,
             "get_length": len,
-            "json_loads": json.loads,
+            "parse_search_sequence": SearchSequence.parse_raw,
             "get_successful_report_total": self._get_successful_report_total,
             "get_overall_status_button_class": self._get_overall_status_button_class,
         }
 
         results_file_name.write_text(index_template.render(context), encoding="utf-8")
         typer.echo(f"HTML report generated: {results_file_name}")
```

### Comparing `hoppr-1.8.4/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js` & `hoppr-1.8.5/hoppr/core_plugins/report_generator/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/core_plugins/report_generator/scripts/custom.js` & `hoppr-1.8.5/hoppr/core_plugins/report_generator/scripts/custom.js`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/core_plugins/report_generator/styles/bootstrap.min.css` & `hoppr-1.8.5/hoppr/core_plugins/report_generator/styles/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/core_plugins/report_generator/styles/custom.css` & `hoppr-1.8.5/hoppr/core_plugins/report_generator/styles/custom.css`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/core_plugins/report_generator/templates/component_card.jinja2` & `hoppr-1.8.5/hoppr/core_plugins/report_generator/templates/component_card.jinja2`

 * *Files 10% similar despite different names*

```diff
@@ -29,30 +29,34 @@
                     <div class="component-indent">Hashes: {{ reference.hashes | default("None") }}</div>
                     {% endfor %}
                 </div>
                 {% endif %}
                 {% if report["component"].properties %}
                 <div class="component-indent">Properites:
                     {% for prop in report["component"].properties %}
-                    {% set prop_value_dict = json_loads(prop.value) %}
                     <div>
                         <div class="component-indent">Name: {{ prop.name }}</div>
                         <div class="component-indent">
                             Value:
+                            {% if prop.name == "hoppr:repository:component_search_sequence" %}
+                            {% set search_sequence = parse_search_sequence(prop.value) %}
                             <div class="component-indent">
-                                <div>Version: {{ prop_value_dict.version }}</div>
+                                <div>Version: {{ search_sequence.version }}</div>
                                 <div>
                                     Repositories:
-                                    {% for repository in prop_value_dict.repositories %}
+                                    {% for repository in search_sequence.repositories %}
                                         <div class="component-indent">
                                             <a href="{{ repository }}" target="_blank">{{ repository }}</a>
                                         </div>
                                     {% endfor %}
                                 </div>
                             </div>
+                            {% else %}
+                                {{ prop.value }}
+                            {% endif %}
                         </div>
                     </div>
                     {% endfor %}
                 </div>
                 {% endif %}
             </div>
             {% if report["details"] %}
```

#### html2text {}

```diff
@@ -15,22 +15,23 @@
 %}
 URL: {{_reference.url_}}
 Comment: {{ reference.comment }}
 Type: {{ reference.type }}
 Hashes: {{ reference.hashes | default("None") }}
 {% endfor %}
 {% endif %} {% if report["component"].properties %}
-Properites: {% for prop in report["component"].properties %} {% set
-prop_value_dict = json_loads(prop.value) %}
+Properites: {% for prop in report["component"].properties %}
 Name: {{ prop.name }}
-Value:
-Version: {{ prop_value_dict.version }}
-Repositories: {% for repository in prop_value_dict.repositories %}
+Value: {% if prop.name == "hoppr:repository:component_search_sequence" %} {%
+set search_sequence = parse_search_sequence(prop.value) %}
+Version: {{ search_sequence.version }}
+Repositories: {% for repository in search_sequence.repositories %}
 {{_repository_}}
 {% endfor %}
+{% else %} {{ prop.value }} {% endif %}
 {% endfor %}
 {% endif %}
 {% if report["details"] %}
 Failure Details
 {{ report["details"] }}
 {% endif %}
 {% if report["result"] == ResultStatus.SUCCESS %}    {% else %}     {% endif %}
```

### Comparing `hoppr-1.8.4/hoppr/core_plugins/report_generator/templates/general_summary.jinja2` & `hoppr-1.8.5/hoppr/core_plugins/report_generator/templates/general_summary.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/core_plugins/report_generator/templates/index.jinja2` & `hoppr-1.8.5/hoppr/core_plugins/report_generator/templates/index.jinja2`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/in_toto.py` & `hoppr-1.8.5/hoppr/in_toto.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/main.py` & `hoppr-1.8.5/hoppr/main.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/mem_logger.py` & `hoppr-1.8.5/hoppr/mem_logger.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/models/__init__.py` & `hoppr-1.8.5/hoppr/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/models/__main__.py` & `hoppr-1.8.5/hoppr/models/__main__.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/models/base.py` & `hoppr-1.8.5/hoppr/models/base.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/models/credentials.py` & `hoppr-1.8.5/hoppr/models/credentials.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/models/manifest.py` & `hoppr-1.8.5/hoppr/models/manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 class SearchSequence(HopprBaseModel):
     """
     SearchSequence data model
     """
 
     version: Literal["v1"]
-    repositories: list[HttpUrl | FileUrl | str] = []
+    repositories: list[RepositoryUrl | str] = []
 
 
 IncludeRef = Annotated[LocalFile | UrlFile, Field(..., description="Reference to a local or remote manifest file")]
 Includes = Annotated[list[IncludeRef], Field(..., description="List of manifest files to load")]
 SbomRef = Annotated[LocalFile | OciFile | UrlFile, Field(..., description="Reference to a local or remote SBOM file")]
 Sboms = Annotated[list[SbomRef], Field(..., description="List of SBOMs to process")]
 SbomRefMap = Annotated[MutableMapping[SbomRef, "Sbom"], Field(...)]
```

### Comparing `hoppr-1.8.4/hoppr/models/transfer.py` & `hoppr-1.8.5/hoppr/models/transfer.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/models/types.py` & `hoppr-1.8.5/hoppr/models/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     GITHUB = "github"
     GITLAB = "gitlab"
     GOLANG = "golang"
     HELM = "helm"
     MAVEN = "maven"
     NPM = "npm"
     PYPI = "pypi"
+    RAW = "raw"
     REPO = "repo"
     RPM = "rpm"
 
 
 class RepositoryUrl(HopprBaseModel):
     """
     RepositoryUrl data model
@@ -91,17 +92,14 @@
         """
         if not (url := values.get("url")):
             raise ValueError("Input parameter `url` must be a non-empty string")
 
         if url.endswith(":"):
             url = f"{url}//"
 
-        if "://" not in url:
-            url = f"http://{url}"
-
         if not (
             match := re.search(
                 pattern=(
                     r"^((?P<scheme>[^:/?#]+):(?=//))?(//)?((("
                     r"?P<username>[^:]+)(?::("
                     r"?P<password>[^@]+)?)?@)?("
                     r"?P<hostname>[^@/?#:]*)(?::("
```

### Comparing `hoppr-1.8.4/hoppr/net.py` & `hoppr-1.8.5/hoppr/net.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/oci_artifacts.py` & `hoppr-1.8.5/hoppr/oci_artifacts.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/plugin_utils.py` & `hoppr-1.8.5/hoppr/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/processor.py` & `hoppr-1.8.5/hoppr/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,19 +120,26 @@
         return result
 
     def _run_all(self, method_name: str):
         """
         Run the named method for all plugins.  If appropriate to the method, run it for
         all components for all plug-ins.
         """
+
         # Map to allow access to the arguments that went into a future call
         future_argument_map: dict[Future[Result], tuple[Plugin, Component | None]] = {}
 
         with ProcessPoolExecutor(max_workers=self.context.max_processes) as executor:
             for plugin in self.plugin_ref_list:
+
+                plugin_cls = plugin_class(plugin.name)
+
+                if getattr(plugin_cls, method_name) == getattr(HopprPlugin, method_name):
+                    continue
+
                 if method_name in self.component_based_methods:
                     # Create one concurrent future object to run this method for each component
                     for component in self.context.delivered_sbom.components or []:
                         future_proc = executor.submit(
                             _run_plugin,
                             plugin_name=plugin.name,
                             context=self.context,
@@ -164,17 +171,19 @@
                 if not future_result.is_skip():
                     if need_method_label:
                         echo(f"   Beginning method {method_name}")
                         need_method_label = False
 
                     plugin_cls = plugin_class(plugin.name)
 
-                    self._save_result(method_name, plugin_cls.__name__, future_result, comp)
+                    if not future_result.is_excluded():
+                        self._save_result(method_name, plugin_cls.__name__, future_result, comp)
+                        self._update_bom(future_result.return_obj, comp)
                     self._report_result(plugin_cls.__name__, comp, future_result)
-                    self._update_bom(future_result.return_obj, comp)
+
                     ReportGenerator.report_gen_list.append(
                         Report(
                             uuid.uuid4(),
                             plugin_cls.__name__,
                             self.stage_id,
                             future_result.status,
                             future_result.message,
@@ -226,15 +235,18 @@
         result_count: dict[str | None, int] = {}
         for (_, purl, _) in self.results.get(method_name, []):
             result_count[purl] = result_count.get(purl, 0) + 1
 
         additional_failures = 0
         for component in self.context.delivered_sbom.components or []:
             count = result_count.get(component.purl, 0)
-            if not self.required_coverage.accepts_count(count):
+            if not self.required_coverage.accepts_count(count) and str(component.scope) not in {
+                'excluded',
+                'Scope.excluded',
+            }:
                 bad_comp_result = Result.fail(
                     f"Component processed {count} times, {self.required_coverage.name} coverage required"
                 )
                 self._save_result(method_name, f"Stage {self.stage_id}", bad_comp_result, component)
                 self._report_result(f"Stage {self.stage_id}", component, bad_comp_result)
                 additional_failures += 1
```

### Comparing `hoppr-1.8.4/hoppr/resources/hoppr-hippo-large.ansi` & `hoppr-1.8.5/hoppr/resources/hoppr-hippo-large.ansi`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/resources/hoppr-hippo.ansi` & `hoppr-1.8.5/hoppr/resources/hoppr-hippo.ansi`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/result.py` & `hoppr-1.8.5/hoppr/result.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/hoppr/utils.py` & `hoppr-1.8.5/hoppr/utils.py`

 * *Files identical despite different names*

### Comparing `hoppr-1.8.4/pyproject.toml` & `hoppr-1.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hoppr"
-version = "1.8.4"
+version = "1.8.5"
 description = "A tool for defining, verifying, and transferring software dependencies between environments."
 authors = ["LMCO Open Source <open.source@lmco.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://hoppr.dev"
 repository = "https://gitlab.com/hoppr/hoppr"
```

### Comparing `hoppr-1.8.4/PKG-INFO` & `hoppr-1.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr
-Version: 1.8.4
+Version: 1.8.5
 Summary: A tool for defining, verifying, and transferring software dependencies between environments.
 Home-page: https://hoppr.dev
 License: MIT
 Keywords: packaging,reports,build dependencies,software bill of materials
 Author: LMCO Open Source
 Author-email: open.source@lmco.com
 Requires-Python: >=3.10,<4.0
```

