# Comparing `tmp/prospector-1.8.4.tar.gz` & `tmp/prospector-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prospector-1.8.4.tar", max compression
+gzip compressed data, was "prospector-1.9.0.tar", max compression
```

## Comparing `prospector-1.8.4.tar` & `prospector-1.9.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0    18044 2023-01-10 19:20:23.901352 prospector-1.8.4/LICENSE
--rw-r--r--   0        0        0     7385 2023-01-10 19:20:23.901352 prospector-1.8.4/README.rst
--rw-r--r--   0        0        0        0 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/__init__.py
--rw-r--r--   0        0        0       71 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/__main__.py
--rw-r--r--   0        0        0     2956 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/autodetect.py
--rw-r--r--   0        0        0     4444 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/blender.py
--rw-r--r--   0        0        0     6551 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/blender_combinations.yaml
--rw-r--r--   0        0        0      360 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/compat.py
--rw-r--r--   0        0        0    13155 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/config/__init__.py
--rw-r--r--   0        0        0    13905 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/config/configuration.py
--rw-r--r--   0        0        0      628 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/config/datatype.py
--rw-r--r--   0        0        0     1542 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/encoding.py
--rw-r--r--   0        0        0     1291 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/exceptions.py
--rw-r--r--   0        0        0     4723 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/finder.py
--rw-r--r--   0        0        0      439 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/formatters/__init__.py
--rw-r--r--   0        0        0     1252 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/formatters/base.py
--rw-r--r--   0        0        0      767 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/formatters/emacs.py
--rw-r--r--   0        0        0     1239 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/formatters/grouped.py
--rw-r--r--   0        0        0      930 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/formatters/json.py
--rw-r--r--   0        0        0     1741 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/formatters/pylint.py
--rw-r--r--   0        0        0     3020 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/formatters/text.py
--rw-r--r--   0        0        0     1295 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/formatters/vscode.py
--rw-r--r--   0        0        0     2431 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/formatters/xunit.py
--rw-r--r--   0        0        0      613 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/formatters/yaml.py
--rw-r--r--   0        0        0     2732 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/message.py
--rw-r--r--   0        0        0     1306 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/pathutils.py
--rw-r--r--   0        0        0     2256 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/postfilter.py
--rw-r--r--   0        0        0      683 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/profiles/__init__.py
--rw-r--r--   0        0        0      871 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/profiles/exceptions.py
--rw-r--r--   0        0        0    15580 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/profiles/profile.py
--rw-r--r--   0        0        0      100 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/profiles/profiles/default.yaml
--rw-r--r--   0        0        0       48 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/profiles/profiles/doc_warnings.yaml
--rw-r--r--   0        0        0      156 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/profiles/profiles/flake8.yaml
--rw-r--r--   0        0        0      873 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/profiles/profiles/full_pep8.yaml
--rw-r--r--   0        0        0       82 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/profiles/profiles/member_warnings.yaml
--rw-r--r--   0        0        0      271 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/profiles/profiles/no_doc_warnings.yaml
--rw-r--r--   0        0        0       83 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/profiles/profiles/no_member_warnings.yaml
--rw-r--r--   0        0        0      348 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/profiles/profiles/no_pep8.yaml
--rw-r--r--   0        0        0      175 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/profiles/profiles/no_test_warnings.yaml
--rw-r--r--   0        0        0      818 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/profiles/profiles/strictness_high.yaml
--rw-r--r--   0        0        0     1066 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/profiles/profiles/strictness_low.yaml
--rw-r--r--   0        0        0     1836 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/profiles/profiles/strictness_medium.yaml
--rw-r--r--   0        0        0      151 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/profiles/profiles/strictness_none.yaml
--rw-r--r--   0        0        0      594 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/profiles/profiles/strictness_veryhigh.yaml
--rw-r--r--   0        0        0      833 2023-01-10 19:20:23.901352 prospector-1.8.4/prospector/profiles/profiles/strictness_verylow.yaml
--rw-r--r--   0        0        0       23 2023-01-10 19:20:23.905352 prospector-1.8.4/prospector/profiles/profiles/test_warnings.yaml
--rw-r--r--   0        0        0     8103 2023-01-10 19:20:23.905352 prospector-1.8.4/prospector/run.py
--rw-r--r--   0        0        0     4467 2023-01-10 19:20:23.905352 prospector-1.8.4/prospector/suppression.py
--rw-r--r--   0        0        0     2609 2023-01-10 19:20:23.905352 prospector-1.8.4/prospector/tools/__init__.py
--rw-r--r--   0        0        0     2212 2023-01-10 19:20:23.905352 prospector-1.8.4/prospector/tools/bandit/__init__.py
--rw-r--r--   0        0        0     1575 2023-01-10 19:20:23.905352 prospector-1.8.4/prospector/tools/base.py
--rw-r--r--   0        0        0     1482 2023-01-10 19:20:23.905352 prospector-1.8.4/prospector/tools/dodgy/__init__.py
--rw-r--r--   0        0        0      170 2023-01-10 19:20:23.905352 prospector-1.8.4/prospector/tools/exceptions.py
--rw-r--r--   0        0        0     2919 2023-01-10 19:20:23.905352 prospector-1.8.4/prospector/tools/mccabe/__init__.py
--rw-r--r--   0        0        0     3684 2023-01-10 19:20:23.905352 prospector-1.8.4/prospector/tools/mypy/__init__.py
--rw-r--r--   0        0        0     7931 2023-01-10 19:20:23.905352 prospector-1.8.4/prospector/tools/profile_validator/__init__.py
--rw-r--r--   0        0        0     5452 2023-01-10 19:20:23.905352 prospector-1.8.4/prospector/tools/pycodestyle/__init__.py
--rw-r--r--   0        0        0     2538 2023-01-10 19:20:23.905352 prospector-1.8.4/prospector/tools/pydocstyle/__init__.py
--rw-r--r--   0        0        0     4998 2023-01-10 19:20:23.905352 prospector-1.8.4/prospector/tools/pyflakes/__init__.py
--rw-r--r--   0        0        0     9886 2023-01-10 19:20:23.905352 prospector-1.8.4/prospector/tools/pylint/__init__.py
--rw-r--r--   0        0        0     1335 2023-01-10 19:20:23.905352 prospector-1.8.4/prospector/tools/pylint/collector.py
--rw-r--r--   0        0        0     1820 2023-01-10 19:20:23.905352 prospector-1.8.4/prospector/tools/pylint/linter.py
--rw-r--r--   0        0        0     2947 2023-01-10 19:20:23.905352 prospector-1.8.4/prospector/tools/pyroma/__init__.py
--rw-r--r--   0        0        0     1161 2023-01-10 19:20:23.905352 prospector-1.8.4/prospector/tools/utils.py
--rw-r--r--   0        0        0     3058 2023-01-10 19:20:23.905352 prospector-1.8.4/prospector/tools/vulture/__init__.py
--rw-r--r--   0        0        0     2710 2023-01-10 19:20:23.905352 prospector-1.8.4/pyproject.toml
--rw-r--r--   0        0        0     9664 1970-01-01 00:00:00.000000 prospector-1.8.4/setup.py
--rw-r--r--   0        0        0     9932 1970-01-01 00:00:00.000000 prospector-1.8.4/PKG-INFO
+-rw-r--r--   0        0        0    18044 2023-02-15 20:45:36.997320 prospector-1.9.0/LICENSE
+-rw-r--r--   0        0        0     7385 2023-02-15 20:45:36.997320 prospector-1.9.0/README.rst
+-rw-r--r--   0        0        0        0 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/__init__.py
+-rw-r--r--   0        0        0       71 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/__main__.py
+-rw-r--r--   0        0        0     2955 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/autodetect.py
+-rw-r--r--   0        0        0     4444 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/blender.py
+-rw-r--r--   0        0        0     6551 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/blender_combinations.yaml
+-rw-r--r--   0        0        0      360 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/compat.py
+-rw-r--r--   0        0        0    13429 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/config/__init__.py
+-rw-r--r--   0        0        0    13905 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/config/configuration.py
+-rw-r--r--   0        0        0      628 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/config/datatype.py
+-rw-r--r--   0        0        0     1542 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/encoding.py
+-rw-r--r--   0        0        0     1291 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/exceptions.py
+-rw-r--r--   0        0        0     4723 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/finder.py
+-rw-r--r--   0        0        0      439 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/formatters/__init__.py
+-rw-r--r--   0        0        0     1252 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/formatters/base.py
+-rw-r--r--   0        0        0      767 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/formatters/emacs.py
+-rw-r--r--   0        0        0     1239 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/formatters/grouped.py
+-rw-r--r--   0        0        0      930 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/formatters/json.py
+-rw-r--r--   0        0        0     1741 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/formatters/pylint.py
+-rw-r--r--   0        0        0     3020 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/formatters/text.py
+-rw-r--r--   0        0        0     1294 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/formatters/vscode.py
+-rw-r--r--   0        0        0     2431 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/formatters/xunit.py
+-rw-r--r--   0        0        0      613 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/formatters/yaml.py
+-rw-r--r--   0        0        0     2732 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/message.py
+-rw-r--r--   0        0        0     1306 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/pathutils.py
+-rw-r--r--   0        0        0     2235 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/postfilter.py
+-rw-r--r--   0        0        0      683 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/profiles/__init__.py
+-rw-r--r--   0        0        0      871 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/profiles/exceptions.py
+-rw-r--r--   0        0        0    15579 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/profiles/profile.py
+-rw-r--r--   0        0        0      100 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/profiles/profiles/default.yaml
+-rw-r--r--   0        0        0       48 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/profiles/profiles/doc_warnings.yaml
+-rw-r--r--   0        0        0      156 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/profiles/profiles/flake8.yaml
+-rw-r--r--   0        0        0      873 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/profiles/profiles/full_pep8.yaml
+-rw-r--r--   0        0        0       82 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/profiles/profiles/member_warnings.yaml
+-rw-r--r--   0        0        0      271 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/profiles/profiles/no_doc_warnings.yaml
+-rw-r--r--   0        0        0       83 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/profiles/profiles/no_member_warnings.yaml
+-rw-r--r--   0        0        0      348 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/profiles/profiles/no_pep8.yaml
+-rw-r--r--   0        0        0      175 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/profiles/profiles/no_test_warnings.yaml
+-rw-r--r--   0        0        0      818 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/profiles/profiles/strictness_high.yaml
+-rw-r--r--   0        0        0     1066 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/profiles/profiles/strictness_low.yaml
+-rw-r--r--   0        0        0     1836 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/profiles/profiles/strictness_medium.yaml
+-rw-r--r--   0        0        0      151 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/profiles/profiles/strictness_none.yaml
+-rw-r--r--   0        0        0      594 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/profiles/profiles/strictness_veryhigh.yaml
+-rw-r--r--   0        0        0      833 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/profiles/profiles/strictness_verylow.yaml
+-rw-r--r--   0        0        0       23 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/profiles/profiles/test_warnings.yaml
+-rw-r--r--   0        0        0     8102 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/run.py
+-rw-r--r--   0        0        0     4467 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/suppression.py
+-rw-r--r--   0        0        0     2609 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/tools/__init__.py
+-rw-r--r--   0        0        0     2212 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/tools/bandit/__init__.py
+-rw-r--r--   0        0        0     1575 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/tools/base.py
+-rw-r--r--   0        0        0     1481 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/tools/dodgy/__init__.py
+-rw-r--r--   0        0        0      170 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/tools/exceptions.py
+-rw-r--r--   0        0        0     2919 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/tools/mccabe/__init__.py
+-rw-r--r--   0        0        0     3684 2023-02-15 20:45:36.997320 prospector-1.9.0/prospector/tools/mypy/__init__.py
+-rw-r--r--   0        0        0     7930 2023-02-15 20:45:37.001320 prospector-1.9.0/prospector/tools/profile_validator/__init__.py
+-rw-r--r--   0        0        0     5452 2023-02-15 20:45:37.001320 prospector-1.9.0/prospector/tools/pycodestyle/__init__.py
+-rw-r--r--   0        0        0     2537 2023-02-15 20:45:37.001320 prospector-1.9.0/prospector/tools/pydocstyle/__init__.py
+-rw-r--r--   0        0        0     4997 2023-02-15 20:45:37.001320 prospector-1.9.0/prospector/tools/pyflakes/__init__.py
+-rw-r--r--   0        0        0     9885 2023-02-15 20:45:37.001320 prospector-1.9.0/prospector/tools/pylint/__init__.py
+-rw-r--r--   0        0        0     1334 2023-02-15 20:45:37.001320 prospector-1.9.0/prospector/tools/pylint/collector.py
+-rw-r--r--   0        0        0     1820 2023-02-15 20:45:37.001320 prospector-1.9.0/prospector/tools/pylint/linter.py
+-rw-r--r--   0        0        0     2947 2023-02-15 20:45:37.001320 prospector-1.9.0/prospector/tools/pyroma/__init__.py
+-rw-r--r--   0        0        0     1161 2023-02-15 20:45:37.001320 prospector-1.9.0/prospector/tools/utils.py
+-rw-r--r--   0        0        0     3058 2023-02-15 20:45:37.001320 prospector-1.9.0/prospector/tools/vulture/__init__.py
+-rw-r--r--   0        0        0     2708 2023-02-15 20:45:37.001320 prospector-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     9661 1970-01-01 00:00:00.000000 prospector-1.9.0/setup.py
+-rw-r--r--   0        0        0     9876 1970-01-01 00:00:00.000000 prospector-1.9.0/PKG-INFO
```

### Comparing `prospector-1.8.4/LICENSE` & `prospector-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/README.rst` & `prospector-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/autodetect.py` & `prospector-1.9.0/prospector/autodetect.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,14 @@
     for requirement in reqs:
         if requirement.name is not None and requirement.name.lower() in POSSIBLE_LIBRARIES:
             names.append(requirement.name.lower())
     return names
 
 
 def autodetect_libraries(path):
-
     if os.path.isfile(path):
         path = os.path.dirname(path)
         if path == "":
             path = "."
 
     libraries = []
```

### Comparing `prospector-1.8.4/prospector/blender.py` & `prospector-1.9.0/prospector/blender.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/blender_combinations.yaml` & `prospector-1.9.0/prospector/blender_combinations.yaml`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/config/__init__.py` & `prospector-1.9.0/prospector/config/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,22 +36,28 @@
         self.libraries = self._find_used_libraries(self.config, self.profile)
         self.tools_to_run = self._determine_tool_runners(self.config, self.profile)
         self.ignores = self._determine_ignores(self.config, self.profile, self.libraries)
         self.configured_by: Dict[str, str] = {}
         self.messages: List[Message] = []
 
     def make_exclusion_filter(self):
+        # Only close over the attributes required by the filter, rather
+        # than the entire self, because ProspectorConfig can't be pickled
+        # because of the config attribute, which would break parallel
+        # pylint.
+        ignores, workdir = self.ignores, self.workdir
+
         def _filter(path: Path):
-            for ignore in self.ignores:
+            for ignore in ignores:
                 # first figure out where the path is, relative to the workdir
                 # ignore-paths/patterns will usually be relative to a repository
                 # root or the CWD, but the path passed to prospector may not be
                 path = path.resolve().absolute()
-                if is_relative_to(path, self.workdir):
-                    path = path.relative_to(self.workdir)
+                if is_relative_to(path, workdir):
+                    path = path.relative_to(workdir)
                 if ignore.match(str(path)):
                     return True
             return False
 
         return _filter
 
     def get_tools(self, found_files):
```

### Comparing `prospector-1.8.4/prospector/config/configuration.py` & `prospector-1.9.0/prospector/config/configuration.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/config/datatype.py` & `prospector-1.9.0/prospector/config/datatype.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/encoding.py` & `prospector-1.9.0/prospector/encoding.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/exceptions.py` & `prospector-1.9.0/prospector/exceptions.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/finder.py` & `prospector-1.9.0/prospector/finder.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/formatters/base.py` & `prospector-1.9.0/prospector/formatters/base.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/formatters/emacs.py` & `prospector-1.9.0/prospector/formatters/emacs.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/formatters/grouped.py` & `prospector-1.9.0/prospector/formatters/grouped.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/formatters/json.py` & `prospector-1.9.0/prospector/formatters/json.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/formatters/pylint.py` & `prospector-1.9.0/prospector/formatters/pylint.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/formatters/text.py` & `prospector-1.9.0/prospector/formatters/text.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/formatters/vscode.py` & `prospector-1.9.0/prospector/formatters/vscode.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
     def render(self, summary=True, messages=True, profile=False):
         # this formatter will always ignore the summary and profile
         cur_loc = None
         output = []
 
         for message in sorted(self.messages):
-
             if cur_loc != message.location.path:
                 cur_loc = message.location.path
                 module_name = self._make_path(message.location.path).replace(os.path.sep, ".")
                 module_name = re.sub(r"(\.__init__)?\.py$", "", module_name)
 
                 header = "************* Module %s" % module_name
                 output.append(header)
```

### Comparing `prospector-1.8.4/prospector/formatters/xunit.py` & `prospector-1.9.0/prospector/formatters/xunit.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/formatters/yaml.py` & `prospector-1.9.0/prospector/formatters/yaml.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/message.py` & `prospector-1.9.0/prospector/message.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/pathutils.py` & `prospector-1.9.0/prospector/pathutils.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/postfilter.py` & `prospector-1.9.0/prospector/postfilter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 from pathlib import Path
 from typing import List
 
 from prospector.message import Message
 from prospector.suppression import get_suppressions
 
 
@@ -26,15 +25,15 @@
     squash the unwanted redundant error from pyflakes and frosted.
     """
     paths_to_ignore, lines_to_ignore, messages_to_ignore = get_suppressions(filepaths, messages)
 
     filtered = []
     for message in messages:
         # first get rid of the pylint informational messages
-        relative_message_path = os.path.relpath(message.location.path)
+        relative_message_path = Path(message.location.path)
 
         if message.source == "pylint" and message.code in (
             "suppressed-message",
             "file-ignored",
         ):
             continue
```

### Comparing `prospector-1.8.4/prospector/profiles/__init__.py` & `prospector-1.9.0/prospector/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/profiles/exceptions.py` & `prospector-1.9.0/prospector/profiles/exceptions.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/profiles/profile.py` & `prospector-1.9.0/prospector/profiles/profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,15 +301,14 @@
 
 def _load_and_merge(
     name_or_path: Union[str, Path],
     profile_path: List[Path],
     allow_shorthand: bool = True,
     forced_inherits: List[str] = None,
 ) -> Tuple[Dict[str, Any], List[str]]:
-
     # First simply load all of the profiles and those that it explicitly inherits from
     data, inherit_list, shorthands_found = _load_profile(
         str(name_or_path),
         profile_path,
         allow_shorthand=allow_shorthand,
         forced_inherits=forced_inherits or [],
     )
```

### Comparing `prospector-1.8.4/prospector/profiles/profiles/full_pep8.yaml` & `prospector-1.9.0/prospector/profiles/profiles/full_pep8.yaml`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/profiles/profiles/strictness_high.yaml` & `prospector-1.9.0/prospector/profiles/profiles/strictness_high.yaml`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/profiles/profiles/strictness_low.yaml` & `prospector-1.9.0/prospector/profiles/profiles/strictness_low.yaml`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/profiles/profiles/strictness_medium.yaml` & `prospector-1.9.0/prospector/profiles/profiles/strictness_medium.yaml`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/profiles/profiles/strictness_veryhigh.yaml` & `prospector-1.9.0/prospector/profiles/profiles/strictness_veryhigh.yaml`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/profiles/profiles/strictness_verylow.yaml` & `prospector-1.9.0/prospector/profiles/profiles/strictness_verylow.yaml`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/run.py` & `prospector-1.9.0/prospector/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
                 msg.source = new_names.get(msg.source, msg.source)
                 updated.append(msg)
             messages = updated
 
         return postfilter.filter_messages(found_files.python_modules, messages)
 
     def execute(self):
-
         deprecated_names = self.config.replace_deprecated_tool_names()
 
         summary = {
             "started": datetime.now(),
         }
         summary.update(self.config.get_summary_information())
```

### Comparing `prospector-1.8.4/prospector/suppression.py` & `prospector-1.9.0/prospector/suppression.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/tools/__init__.py` & `prospector-1.9.0/prospector/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/tools/bandit/__init__.py` & `prospector-1.9.0/prospector/tools/bandit/__init__.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/tools/base.py` & `prospector-1.9.0/prospector/tools/base.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/tools/dodgy/__init__.py` & `prospector-1.9.0/prospector/tools/dodgy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 class DodgyTool(ToolBase):
     def configure(self, prospector_config, found_files):
         # empty: just implementing to satisfy the ABC contract
         pass
 
     def run(self, found_files: FileFinder):
-
         warnings = []
         for filepath in found_files.files:
             mimetype = mimetypes.guess_type(str(filepath.absolute()))
             if mimetype[0] is None or not mimetype[0].startswith("text/") or mimetype[1] is not None:
                 continue
             try:
                 contents = read_py_file(filepath)
```

### Comparing `prospector-1.8.4/prospector/tools/mccabe/__init__.py` & `prospector-1.9.0/prospector/tools/mccabe/__init__.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/tools/mypy/__init__.py` & `prospector-1.9.0/prospector/tools/mypy/__init__.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/tools/profile_validator/__init__.py` & `prospector-1.9.0/prospector/tools/profile_validator/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     tools = list(TOOLS)
     if with_deprecated:
         tools += DEPRECATED_TOOL_NAMES.keys()
     return tools
 
 
 class ProfileValidationTool(ToolBase):
-
     LIST_SETTINGS = ("inherits", "uses", "ignore", "ignore-paths", "ignore-patterns")
     BOOL_SETTINGS = ("doc-warnings", "test-warnings", "autodetect")
     OTHER_SETTINGS = (
         "strictness",
         "max-line-length",
         "output-format",
         "output-target",
```

### Comparing `prospector-1.8.4/prospector/tools/pycodestyle/__init__.py` & `prospector-1.9.0/prospector/tools/pycodestyle/__init__.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/tools/pydocstyle/__init__.py` & `prospector-1.9.0/prospector/tools/pydocstyle/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
         messages = []
 
         checker = ConventionChecker()
 
         for code_file in found_files.python_modules:
             try:
                 for error in checker.check_source(read_py_file(code_file), str(code_file.absolute()), None):
-
                     location = Location(path=code_file, module=None, function="", line=error.line, character=0)
                     message = Message(
                         source="pydocstyle",
                         code=error.code,
                         location=location,
                         message=error.message.partition(":")[2].strip(),
                     )
```

### Comparing `prospector-1.8.4/prospector/tools/pyflakes/__init__.py` & `prospector-1.9.0/prospector/tools/pyflakes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,14 @@
     def __init__(self, ignore=None):
         super().__init__(None, None)
         self._messages = []
         self.ignore = ignore or ()
 
     # pylint: disable=too-many-arguments
     def record_message(self, filename=None, line=None, character=None, code=None, message=None):
-
         code = code or "F999"
         if code in self.ignore:
             return
 
         location = Location(
             path=filename,
             module=None,
```

### Comparing `prospector-1.8.4/prospector/tools/pylint/__init__.py` & `prospector-1.9.0/prospector/tools/pylint/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,14 @@
                 try:
                     linter.load_plugin_modules([plugin])
                 except ImportError:
                     errors.append(self._error_message(pylintrc, f"Could not load plugin {plugin}"))
         return errors
 
     def configure(self, prospector_config, found_files: FileFinder):
-
         extra_sys_path = found_files.make_syspath()
         check_paths = self._get_pylint_check_paths(found_files)
 
         pylint_options = prospector_config.tool_options("pylint")
         self._set_path_finder(extra_sys_path, pylint_options)
 
         linter = ProspectorLinter(found_files)
```

### Comparing `prospector-1.8.4/prospector/tools/pylint/collector.py` & `prospector-1.9.0/prospector/tools/pylint/collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from pylint.message import Message as PylintMessage
 from pylint.reporters import BaseReporter
 
 from prospector.message import Location, Message
 
 
 class Collector(BaseReporter):
-
     name = "collector"
 
     def __init__(self, message_store):
         BaseReporter.__init__(self, output=StringIO())
         self._message_store = message_store
         self._messages = []
```

### Comparing `prospector-1.8.4/prospector/tools/pylint/linter.py` & `prospector-1.9.0/prospector/tools/pylint/linter.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/tools/pyroma/__init__.py` & `prospector-1.9.0/prospector/tools/pyroma/__init__.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/tools/utils.py` & `prospector-1.9.0/prospector/tools/utils.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/prospector/tools/vulture/__init__.py` & `prospector-1.9.0/prospector/tools/vulture/__init__.py`

 * *Files identical despite different names*

### Comparing `prospector-1.8.4/pyproject.toml` & `prospector-1.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prospector"
-version = "1.8.4"
+version = "1.9.0"
 description = "Prospector is a tool to analyse Python code by aggregating the result of other tools."
 authors = ["Carl Crowder <git@carlcrowder.com>"]
 maintainers = ["Carl Crowder <git@carlcrowder.com>",
                "Carlos Coelho <carlospecter@gmail.com>",
                "Pierre Sassoulas <pierre.sassoulas@gmail.com>"]
 readme = "README.rst"
 homepage = "http://prospector.readthedocs.io"
@@ -34,15 +34,15 @@
   "README.rst"
 ]
 
 [tool.poetry.scripts]
 prospector = 'prospector.run:main'
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
+python = ">=3.7.2,<4.0"
 pylint = ">=2.8.3"
 pylint-celery = "0.3"
 pylint-django = "~2.5"
 pylint-plugin-utils = "~0.7"
 pylint-flask = "0.6"
 requirements-detector = ">=1.0.3"
 PyYAML = "*"
@@ -56,15 +56,15 @@
 toml = "^0.10.2"
 bandit = {version = ">=1.5.1", optional = true}
 vulture = {version = ">=1.5", optional = true}
 mypy = {version = ">=0.600", optional = true}
 pyroma = {version = ">=2.4", optional = true}
 setoptconf-tmp = "^0.3.1"
 GitPython = "^3.1.27"
-packaging = "<22.0"
+packaging = "*"
 
 [tool.poetry.extras]
 with_bandit = ["bandit"]
 with_mypy = ["mypy"]
 with_pyroma = ["pyroma"]
 with_vulture = ["vulture"]
 with_everything = ["bandit", "mypy", "pyroma", "vulture"]
```

### Comparing `prospector-1.8.4/setup.py` & `prospector-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 install_requires = \
 ['GitPython>=3.1.27,<4.0.0',
  'PyYAML',
  'dodgy>=0.2.1,<0.3.0',
  'flake8<6.0.0',
  'mccabe>=0.7.0,<0.8.0',
- 'packaging<22.0',
+ 'packaging',
  'pep8-naming>=0.3.3,<=0.10.0',
  'pycodestyle>=2.9.0',
  'pydocstyle>=2.0.0',
  'pyflakes>=2.2.0,<3',
  'pylint-celery==0.3',
  'pylint-django>=2.5,<2.6',
  'pylint-flask==0.6',
@@ -53,25 +53,25 @@
  'with_vulture': ['vulture>=1.5']}
 
 entry_points = \
 {'console_scripts': ['prospector = prospector.run:main']}
 
 setup_kwargs = {
     'name': 'prospector',
-    'version': '1.8.4',
+    'version': '1.9.0',
     'description': 'Prospector is a tool to analyse Python code by aggregating the result of other tools.',
     'long_description': 'prospector\n==========\n\n.. image:: https://img.shields.io/pypi/v/prospector.svg\n   :target: https://pypi.python.org/pypi/prospector\n   :alt: Latest Version of Prospector\n.. image:: https://github.com/PyCQA/prospector/actions/workflows/ci.yaml/badge.svg\n   :target: https://github.com/PyCQA/prospector/actions/workflows/ci.yaml\n   :alt: Build Status\n.. image:: https://img.shields.io/coveralls/PyCQA/prospector.svg?style=flat\n   :target: https://coveralls.io/r/PyCQA/prospector\n   :alt: Test Coverage\n.. image:: https://readthedocs.org/projects/prospector/badge/?version=latest\n   :target: https://prospector.readthedocs.io/\n   :alt: Documentation\n\n\nAbout\n-----\n\nProspector is a tool to analyse Python code and output information about\nerrors, potential problems, convention violations and complexity.\n\nIt brings together the functionality of other Python analysis tools such as\n`Pylint <https://docs.pylint.org/>`_,\n`pycodestyle <https://pycodestyle.pycqa.org/>`_,\nand `McCabe complexity <https://pypi.python.org/pypi/mccabe>`_.\nSee the `Supported Tools <https://prospector.readthedocs.io/en/latest/supported_tools.html>`_\ndocumentation section for a complete list.\n\nThe primary aim of Prospector is to be useful \'out of the box\'. A common complaint of other\nPython analysis tools is that it takes a long time to filter through which errors are relevant\nor interesting to your own coding style. Prospector provides some default profiles, which\nhopefully will provide a good starting point and will be useful straight away, and adapts\nthe output depending on the libraries your project uses.\n\nInstallation\n------------\n\nProspector can be installed from PyPI using ``pip`` by running the following command::\n\n    pip install prospector\n\nOptional dependencies for Prospector, such as ``pyroma`` can also be installed by running::\n\n    pip install prospector[with_pyroma]\n\nSome shells (such as ``Zsh``, the default shell of macOS Catalina) require brackets to be escaped::\n\n    pip install prospector\\[with_pyroma\\]\n\nFor a list of all of the optional dependencies, see the optional extras section on the ReadTheDocs\npage on `Supported Tools Extras <https://prospector.readthedocs.io/en/latest/supported_tools.html#optional-extras>`_.\n\nFor local development, `poetry <https://python-poetry.org/>`_ is used. Check out the code, then run::\n\n    poetry install\n\nAnd for extras::\n\n    poetry install -E with_everything\n\nFor more detailed information on installing the tool, see the\n`installation section <https://prospector.readthedocs.io/en/latest/#installation>`_ of the tool\'s main page\non ReadTheDocs.\n\nDocumentation\n-------------\n\nFull `documentation is available at ReadTheDocs <https://prospector.readthedocs.io>`_.\n\nUsage\n-----\n\nSimply run prospector from the root of your project::\n\n    prospector\n\nThis will output a list of messages pointing out potential problems or errors, for example::\n\n    prospector.tools.base (prospector/tools/base.py):\n        L5:0 ToolBase: pylint - R0922\n        Abstract class is only referenced 1 times\n\nOptions\n```````\n\nRun ``prospector --help`` for a full list of options and their effects.\n\nOutput Format\n~~~~~~~~~~~~~\n\nThe default output format of ``prospector`` is designed to be human readable. For parsing\n(for example, for reporting), you can use the ``--output-format json`` flag to get JSON-formatted\noutput.\n\nProfiles\n~~~~~~~~\n\nProspector is configurable using "profiles". These are composable YAML files with directives to\ndisable or enable tools or messages. For more information, read\n`the documentation about profiles <https://prospector.readthedocs.io/en/latest/profiles.html>`_.\n\nIf your code uses frameworks and libraries\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\nOften tools such as pylint find errors in code which is not an error, for example due to attributes of classes being\ncreated at run time by a library or framework used by your project.\nFor example, by default, pylint will generate an error for Django models when accessing ``objects``, as the\n``objects`` attribute is not part of the ``Model`` class definition.\n\nProspector mitigates this by providing an understanding of these frameworks to the underlying tools.\n\nProspector will try to intuit which libraries your project uses by\n`detecting dependencies <https://github.com/landscapeio/requirements-detector>`_ and automatically turning on\nsupport for the requisite libraries. You can see which adaptors were run in the metadata section of the report.\n\nIf Prospector does not correctly detect your project\'s dependencies, you can specify them manually from the commandline::\n\n    prospector --uses django celery\n\nAdditionally, if Prospector is automatically detecting a library that you do not in fact use, you can turn\noff autodetection completely::\n\n    prospector --no-autodetect\n\nNote that as far as possible, these adaptors have been written as plugins or augmentations for the underlying\ntools so that they can be used without requiring Prospector. For example, the Django support is available as a pylint plugin.\n\nStrictness\n~~~~~~~~~~\n\nProspector has a configurable \'strictness\' level which will determine how harshly it searches for errors::\n\n    prospector --strictness high\n\nPossible values are ``verylow``, ``low``, ``medium``, ``high``, ``veryhigh``.\n\nProspector does not include documentation warnings by default, but you can turn\nthis on using the ``--doc-warnings`` flag.\n\npre-commit\n----------\n\nIf you\'d like Prospector to be run automatically when making changes to files in your Git\nrepository, you can install `pre-commit <https://pre-commit.com/>`_ and add the following\ntext to your repositories\' ``.pre-commit-config.yaml``::\n\n    repos:\n    -   repo: https://github.com/PyCQA/prospector\n        rev: 1.7.5 # The version of Prospector to use, if not \'master\' for latest\n        hooks:\n        -   id: prospector\n\nThis only installs base prospector - if you also use optional tools, for example bandit and/or mypy, then you can add\nthem to the hook configuration like so::\n\n    repos:\n    -   repo: https://github.com/PyCQA/prospector\n        rev: 1.7.5\n        hooks:\n        -   id: prospector\n            additional_dependencies:\n            - ".[with_mypy,with_bandit]"\n          - args: [\n            \'--with-tool=mypy\',\n            \'--with-tool=bandit\',\n            ]\n\nAdditional dependencies can be `individually configured <https://prospector.landscape.io/en/master/profiles.html#individual-configuration-options>`_ in your `prospector.yml` file ::\n\n    # https://bandit.readthedocs.io/en/latest/config.html\n    bandit:\n    options:\n        skips:\n        - B201\n        - B601\n        - B610\n        - B611\n        - B703\n\n    # https://mypy.readthedocs.io/en/stable/command_line.html\n    mypy:\n    options:\n        ignore-missing-imports: true\n\nFor prospector options which affect display only - those which are not configurable using a profile - these can be\nadded as command line arguments to the hook. For example::\n\n    repos:\n    -   repo: https://github.com/PyCQA/prospector\n        rev: 1.7.5\n        hooks:\n        -   id: prospector\n            additional_dependencies:\n            -   ".[with_mypy,with_bandit]"\n            args:\n            -   --with-tool=mypy\n            -   --with-tool=bandit\n            -   --summary-only\n            -   --zero-exit\n\n\n\nLicense\n-------\n\nProspector is available under the GPLv2 License.\n',
     'author': 'Carl Crowder',
     'author_email': 'git@carlcrowder.com',
     'maintainer': 'Carl Crowder',
     'maintainer_email': 'git@carlcrowder.com',
     'url': 'http://prospector.readthedocs.io',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.7.2,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `prospector-1.8.4/PKG-INFO` & `prospector-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: prospector
-Version: 1.8.4
+Version: 1.9.0
 Summary: Prospector is a tool to analyse Python code by aggregating the result of other tools.
 Home-page: http://prospector.readthedocs.io
 License: GPLv2+
 Keywords: pylint,prospector,static code analysis
 Author: Carl Crowder
 Author-email: git@carlcrowder.com
 Maintainer: Carl Crowder
 Maintainer-email: git@carlcrowder.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.7.2,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -35,15 +34,15 @@
 Requires-Dist: GitPython (>=3.1.27,<4.0.0)
 Requires-Dist: PyYAML
 Requires-Dist: bandit (>=1.5.1); extra == "with_bandit" or extra == "with_everything"
 Requires-Dist: dodgy (>=0.2.1,<0.3.0)
 Requires-Dist: flake8 (<6.0.0)
 Requires-Dist: mccabe (>=0.7.0,<0.8.0)
 Requires-Dist: mypy (>=0.600); extra == "with_mypy" or extra == "with_everything"
-Requires-Dist: packaging (<22.0)
+Requires-Dist: packaging
 Requires-Dist: pep8-naming (>=0.3.3,<=0.10.0)
 Requires-Dist: pycodestyle (>=2.9.0)
 Requires-Dist: pydocstyle (>=2.0.0)
 Requires-Dist: pyflakes (>=2.2.0,<3)
 Requires-Dist: pylint (>=2.8.3)
 Requires-Dist: pylint-celery (==0.3)
 Requires-Dist: pylint-django (>=2.5,<2.6)
```

