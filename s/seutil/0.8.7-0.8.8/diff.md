# Comparing `tmp/seutil-0.8.7.tar.gz` & `tmp/seutil-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seutil-0.8.7.tar", last modified: Wed May  3 22:40:14 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `seutil-0.8.7.tar` & `seutil-0.8.8.tar`

### file list

```diff
@@ -1,59 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:40:14.252116 seutil-0.8.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 22:40:03.000000 seutil-0.8.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-03 22:40:14.248116 seutil-0.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-03 22:40:03.000000 seutil-0.8.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 22:40:14.252116 seutil-0.8.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-03 22:40:03.000000 seutil-0.8.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:40:14.248116 seutil-0.8.7/seutil/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/BashUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/CliUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/GitHubUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16042 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/IOUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/LoggingUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/MiscUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/Stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/TimeUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/bash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:40:14.248116 seutil-0.8.7/seutil/ds/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/ds/graph_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/ds/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/ds/trie.py
--rw-r--r--   0 runner    (1001) docker     (123)    31481 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/latex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:40:14.248116 seutil-0.8.7/seutil/latex_old/
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/latex_old/File.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/latex_old/Macro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/latex_old/Table.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/latex_old/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/maven.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/pbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-05-03 22:40:03.000000 seutil-0.8.7/seutil/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:40:14.248116 seutil-0.8.7/seutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-03 22:40:14.000000 seutil-0.8.7/seutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-03 22:40:14.000000 seutil-0.8.7/seutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 22:40:14.000000 seutil-0.8.7/seutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-03 22:40:14.000000 seutil-0.8.7/seutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 22:40:14.000000 seutil-0.8.7/seutil.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:40:14.248116 seutil-0.8.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:40:14.248116 seutil-0.8.7/tests/ds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/ds/test_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/ds/test_trie.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_BashUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_GitHubUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_IOUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_arg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_io_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_io_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_io_ser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_io_ser_3rd_party.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_latex_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-05-03 22:40:03.000000 seutil-0.8.7/tests/test_project.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 seutil-0.8.8/.readthedocs.yaml
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 seutil-0.8.8/Dockerfile
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 seutil-0.8.8/Makefile
+-rwxr-xr-x   0        0        0      884 2020-02-02 00:00:00.000000 seutil-0.8.8/prepare-env.sh
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 seutil-0.8.8/.github/dependabot.yml
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 seutil-0.8.8/.github/workflows/python-build.yml
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 seutil-0.8.8/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 seutil-0.8.8/.vscode/settings.json
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 seutil-0.8.8/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 seutil-0.8.8/docs/make.bat
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 seutil-0.8.8/docs/source/conf.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 seutil-0.8.8/docs/source/index.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 seutil-0.8.8/docs/source/modules.rst
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 seutil-0.8.8/docs/source/setup.rst
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 seutil-0.8.8/docs/source/seutil.latex.rst
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 seutil-0.8.8/docs/source/seutil.project.rst
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 seutil-0.8.8/docs/source/seutil.rst
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/BashUtils.py
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/CliUtils.py
+-rw-r--r--   0        0        0    11708 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/GitHubUtils.py
+-rw-r--r--   0        0        0    16046 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/IOUtils.py
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/LoggingUtils.py
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/MiscUtils.py
+-rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/Stream.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/TimeUtils.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/__about__.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/arg.py
+-rw-r--r--   0        0        0     5892 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/bash.py
+-rw-r--r--   0        0        0    35702 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/io.py
+-rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/latex.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/log.py
+-rw-r--r--   0        0        0     7929 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/maven.py
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/pbar.py
+-rw-r--r--   0        0        0    11518 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/project.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/ds/__init__.py
+-rw-r--r--   0        0        0     5864 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/ds/graph_common.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/ds/lattice.py
+-rw-r--r--   0        0        0    13411 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/ds/trie.py
+-rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/latex_old/File.py
+-rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/latex_old/Macro.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/latex_old/Table.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 seutil-0.8.8/src/seutil/latex_old/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 seutil-0.8.8/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 seutil-0.8.8/tests/ds/__init__.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 seutil-0.8.8/tests/ds/test_lattice.py
+-rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 seutil-0.8.8/tests/ds/test_trie.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 seutil-0.8.8/tests/integration/__init__.py
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 seutil-0.8.8/tests/integration/test_latex_integration.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 seutil-0.8.8/tests/resources/.gitignore
+-rw-r--r--   0        0        0  1323560 2020-02-02 00:00:00.000000 seutil-0.8.8/tests/resources/git-game.git.tgz
+-rw-r--r--   0        0        0   368601 2020-02-02 00:00:00.000000 seutil-0.8.8/tests/resources/sample-dataset.pkl.gz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 seutil-0.8.8/tests/unit/__init__.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 seutil-0.8.8/tests/unit/test_BashUtils.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 seutil-0.8.8/tests/unit/test_GitHubUtils.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 seutil-0.8.8/tests/unit/test_arg.py
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 seutil-0.8.8/tests/unit/test_bash.py
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 seutil-0.8.8/tests/unit/test_io_path.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 seutil-0.8.8/tests/unit/test_io_rw.py
+-rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 seutil-0.8.8/tests/unit/test_io_ser.py
+-rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 seutil-0.8.8/tests/unit/test_io_ser_3rd_party.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 seutil-0.8.8/tests/unit/test_latex.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 seutil-0.8.8/tests/unit/test_log.py
+-rw-r--r--   0        0        0    12666 2020-02-02 00:00:00.000000 seutil-0.8.8/tests/unit/test_project.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 seutil-0.8.8/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 seutil-0.8.8/LICENSE
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 seutil-0.8.8/README.rst
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 seutil-0.8.8/pyproject.toml
+-rw-r--r--   0        0        0    16214 2020-02-02 00:00:00.000000 seutil-0.8.8/PKG-INFO
```

### Comparing `seutil-0.8.7/LICENSE` & `seutil-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `seutil-0.8.7/PKG-INFO` & `seutil-0.8.8/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: seutil
-Version: 0.8.7
-Summary: Python utilities for SE research
-Home-page: https://github.com/pengyunie/seutil
-Author: Pengyu Nie
-Author-email: prodigy.sov@gmail.com
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX :: Linux
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-Provides-Extra: io-3rd-party
-License-File: LICENSE
-
 Project ``seutil``
 ==================
 
 |PyPI|_ |GitHubRelease|_ |GitHubWorkflow|_
 
 Python utilities for SE(+ML) research. This library stays reasonably
 up-to-date with the latest Python 3, currently 3.8.
```

### Comparing `seutil-0.8.7/seutil/BashUtils.py` & `seutil-0.8.8/src/seutil/BashUtils.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,26 +5,29 @@
 import subprocess
 
 
 class BashUtils:
     """
     Utility functions for running Bash commands.
     """
+
     PRINT_LIMIT = 1000
 
     class RunResult(NamedTuple):
         return_code: int
         stdout: str
         stderr: str
 
     @classmethod
-    def run(cls, cmd: str,
-            expected_return_code: int = None,
-            is_update_env: bool = False,
-            timeout: Optional[float] = None,
+    def run(
+        cls,
+        cmd: str,
+        expected_return_code: int = None,
+        is_update_env: bool = False,
+        timeout: Optional[float] = None,
     ) -> RunResult:
         """
         Runs a Bash command and returns the stdout.
         :param cmd: the command to run.
         :param expected_return_code: if set to an int, will raise exception if the return code mismatch.
         :param is_update_env: if true, the environment in *this python process (os.environ)* will be updated upon the successful execution of cmd (i.e., returns 0), to reflect the changes to the enrionment variables cmd may make.  Note it can not change the environment of the process that invoked this python process.  It is useful because the updated environment will be used for later BashUtils.run executions.
         :param timeout: if not None, kill the process after timeout seconds and raise TimeoutExpire exception.
@@ -32,16 +35,18 @@
         """
         # If update env is requested, append an additional command to the cmd
         if is_update_env:
             tempfile_update_env = cls.get_temp_file()
             cmd += f" && env > {tempfile_update_env}"
         # end if
 
-        completed_process = subprocess.run(["bash", "-c", cmd], stdout=subprocess.PIPE, stderr=subprocess.PIPE, timeout=timeout)
-        #completed_process = subprocess.run(cmd, shell=True, executable="/bin/bash", stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        completed_process = subprocess.run(
+            ["bash", "-c", cmd], stdout=subprocess.PIPE, stderr=subprocess.PIPE, timeout=timeout
+        )
+        # completed_process = subprocess.run(cmd, shell=True, executable="/bin/bash", stdout=subprocess.PIPE, stderr=subprocess.PIPE)
 
         return_code = completed_process.returncode
         stdout = completed_process.stdout.decode("utf-8", errors="ignore")
         stderr = completed_process.stderr.decode("utf-8", errors="ignore")
 
         # Update env, if requested and return code is 0
         if is_update_env and return_code == 0:
@@ -53,28 +58,38 @@
                 # end for
             # end with
         # end if
 
         if expected_return_code is not None:
             if return_code != expected_return_code:
                 if len(stdout) > cls.PRINT_LIMIT:
-                    tempfile_stdout = subprocess.run(["bash", "-c", "mktemp"], stdout=subprocess.PIPE, stderr=subprocess.PIPE).stdout.decode("utf-8", errors="ignore").strip()
+                    tempfile_stdout = (
+                        subprocess.run(["bash", "-c", "mktemp"], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+                        .stdout.decode("utf-8", errors="ignore")
+                        .strip()
+                    )
                     with open(tempfile_stdout, "w") as f:
                         f.write(stdout)
                     # end with
                     stdout = f"{stdout[:cls.PRINT_LIMIT]} //////////TOO LONG; dumped to {tempfile_stdout}//////////"
                 # end if
                 if len(stderr) > cls.PRINT_LIMIT:
-                    tempfile_stderr = subprocess.run(["bash", "-c", "mktemp"], stdout=subprocess.PIPE, stderr=subprocess.PIPE).stdout.decode("utf-8", errors="ignore").strip()
+                    tempfile_stderr = (
+                        subprocess.run(["bash", "-c", "mktemp"], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+                        .stdout.decode("utf-8", errors="ignore")
+                        .strip()
+                    )
                     with open(tempfile_stderr, "w") as f:
                         f.write(stderr)
                     # end with
                     stderr = f"{stderr[:cls.PRINT_LIMIT]} //////////TOO LONG; dumped to {tempfile_stderr}//////////"
                 # end if
-                raise RuntimeError(f"Expected {expected_return_code} but returned {return_code} while executing bash command '{cmd}'.\nstdout: {stdout}\nstderr: {stderr}")
+                raise RuntimeError(
+                    f"Expected {expected_return_code} but returned {return_code} while executing bash command '{cmd}'.\nstdout: {stdout}\nstderr: {stderr}"
+                )
         # end if, if
 
         return cls.RunResult(return_code, stdout, stderr)
 
     @classmethod
     def get_temp_dir(cls) -> Path:
         return Path(cls.run("mktemp -d", expected_return_code=0).stdout.strip())
```

### Comparing `seutil-0.8.7/seutil/CliUtils.py` & `seutil-0.8.8/src/seutil/CliUtils.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     #                 new_option.
     #     # end while
     #     if new_option is not None:
     #         options.append(new_option)
     #     # end if
     #     return options, args
 
-
     def __call__(self, parser, namespace, values, option_string=None):
         d = getattr(namespace, self.dest)
         types = dict()
         for opt in values:
             try:
                 name, value = opt.split("=", 1)
             except:
@@ -57,15 +56,15 @@
             else:
                 d[name] = [value]
         for name in d:
             if not types[name] == "list" and len(d[name]) == 1:
                 d[name] = d[name][0]
             # end if
             if types[name] != "":
-                d[name] = eval("{}(\"{}\")".format(types[name], d[name]))
+                d[name] = eval('{}("{}")'.format(types[name], d[name]))
                 continue
             # end if
             try:
                 intval = int(d[name])
             except:
                 pass
             else:
@@ -102,15 +101,15 @@
         cli_options = argv
     else:
         action = argv[0]
         cli_options = argv[1:]
     # end if
 
     # Prevent distinguish between positional arguments and optional arguments (HACK)
-    p = argparse.ArgumentParser(prefix_chars=' ')
+    p = argparse.ArgumentParser(prefix_chars=" ")
     p.add_argument("options", nargs="*", action=StoreInDict, default=dict())
     options = p.parse_args(cli_options).options
 
     # normalize options
     options = normalize_options(options)
 
     if action in actions:
```

### Comparing `seutil-0.8.7/seutil/GitHubUtils.py` & `seutil-0.8.8/src/seutil/GitHubUtils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 import math
+import os
 import traceback
 from datetime import datetime
 from time import sleep
-from typing import *
+from typing import Callable, List, TypeVar
 
 from github import Github, RateLimitExceededException
 from github.GithubException import GithubException
 from github.NamedUser import NamedUser
 from github.Repository import Repository
 
-from . import _config
-from .LoggingUtils import LoggingUtils
 from .BashUtils import BashUtils
+from .LoggingUtils import LoggingUtils
 
 
 class GitHubUtils:
-
     logger = LoggingUtils.get_logger("GitHubUtils", LoggingUtils.DEBUG)
 
     GITHUB_SEARCH_ITEMS_MAX = 1000
-    try:
-        DEFAULT_ACCESS_TOKEN = _config.get_config("github_access_token")
-        DEFAULT_GITHUB_OBJECT = Github(DEFAULT_ACCESS_TOKEN, per_page=100)
-    except:
-        DEFAULT_ACCESS_TOKEN = None
-        DEFAULT_GITHUB_OBJECT = None
-        logger.info("Fail to get github_access_token from config file.  Using GitHubUtils APIs will require compulsory input access_token")
-    # end try
+
+    DEFAULT_GITHUB_OBJECT = (
+        Github(os.environ["SU_GITHUB_ACCESS_TOKEN"], per_page=100) if "SU_GITHUB_ACCESS_TOKEN" in os.environ else None
+    )
 
     @classmethod
     def get_github(cls, access_token: str = None) -> Github:
         if access_token is None:
             return cls.DEFAULT_GITHUB_OBJECT
         else:
             return Github(access_token)
 
     class wait_rate_limit:
         """
         Wait for rate limit of the github accessor. For use with "with".
         Use the default github accessor if no argument is given.
         """
+
         DEFAULT_GITHUB_OBJECT = None
         logger = None
 
         def __init__(self, github: Github = DEFAULT_GITHUB_OBJECT):
             self.github = github
             return
 
@@ -55,31 +51,38 @@
             # Check rate limit
             rate_limit_remain, rate_limit = self.github.rate_limiting
             if rate_limit_remain <= 1:
                 self.logger.debug("Rate limit {} / {}".format(rate_limit_remain, rate_limit))
                 rate_limit_reset_time = datetime.fromtimestamp(self.github.rate_limiting_resettime)
                 rate_limit_wait_seconds = math.ceil((rate_limit_reset_time - datetime.now()).total_seconds()) + 1
                 if rate_limit_wait_seconds > 0:
-                    self.logger.warning("Rate limit will recover at: {}, will wait for {} seconds.".format(rate_limit_reset_time, rate_limit_wait_seconds))
+                    self.logger.warning(
+                        "Rate limit will recover at: {}, will wait for {} seconds.".format(
+                            rate_limit_reset_time, rate_limit_wait_seconds
+                        )
+                    )
                     sleep(rate_limit_wait_seconds)
                     self.logger.warning("Rate limit recovered")
                 # end if
             # end if
             return self.github
 
         def __exit__(self, type, value, tb):
             return
 
     # end class
     wait_rate_limit.DEFAULT_GITHUB_OBJECT = DEFAULT_GITHUB_OBJECT
     wait_rate_limit.logger = logger
 
     T = TypeVar("T")
+
     @classmethod
-    def ensure_github_api_call(cls, call: Callable[[Github], T], github: Github = DEFAULT_GITHUB_OBJECT, max_retry_times: int = float("inf")) -> T:
+    def ensure_github_api_call(
+        cls, call: Callable[[Github], T], github: Github = DEFAULT_GITHUB_OBJECT, max_retry_times: int = float("inf")
+    ) -> T:
         retry_times = 0
         while True:
             try:
                 with cls.wait_rate_limit(github) as g:
                     return call(g)
                 # end with
             except (GithubException, RateLimitExceededException) as e:
@@ -97,20 +100,26 @@
                     retry_wait_time = min(retry_times * 30, 600)
                     cls.logger.warning("Will wait {} seconds before retry {}".format(retry_wait_time, retry_times))
                     sleep(retry_wait_time)
             # end try
         # end while
 
     @classmethod
-    def search_repos(cls, q: str = "", sort: str = "stars", order: str = "desc",
-                     is_allow_fork: bool = False,
-                     max_num_repos: int = GITHUB_SEARCH_ITEMS_MAX,
-                     github: Github = DEFAULT_GITHUB_OBJECT,
-                     max_retry_times: int = float("inf"),
-                     *_, **qualifiers) -> List[Repository]:
+    def search_repos(
+        cls,
+        q: str = "",
+        sort: str = "stars",
+        order: str = "desc",
+        is_allow_fork: bool = False,
+        max_num_repos: int = GITHUB_SEARCH_ITEMS_MAX,
+        github: Github = DEFAULT_GITHUB_OBJECT,
+        max_retry_times: int = float("inf"),
+        *_,
+        **qualifiers,
+    ) -> List[Repository]:
         """
         Searches the repos by querying GitHub API v3.
         :return: a list of full names of the repos match the query.
         """
         cls.logger.debug("Search for repos with query {}, sort {}, order {}".format(q, sort, order))
         repos = list()
         num_repos = 0
@@ -146,19 +155,25 @@
         else:
             cls.logger.info("Got {}/{} repos".format(num_repos, max_num_repos))
         # end if
 
         return repos
 
     @classmethod
-    def search_users(cls, q: str = "", sort: str = "repositories", order: str = "desc",
-                     max_num_users: int = GITHUB_SEARCH_ITEMS_MAX,
-                     github: Github = DEFAULT_GITHUB_OBJECT,
-                     max_retry_times: int = float("inf"),
-                     *_, **qualifiers) -> List[NamedUser]:
+    def search_users(
+        cls,
+        q: str = "",
+        sort: str = "repositories",
+        order: str = "desc",
+        max_num_users: int = GITHUB_SEARCH_ITEMS_MAX,
+        github: Github = DEFAULT_GITHUB_OBJECT,
+        max_retry_times: int = float("inf"),
+        *_,
+        **qualifiers,
+    ) -> List[NamedUser]:
         """
         Searches the users by querying GitHub API v3.
         :return: a list of usernames (login) of the users match the query.
         """
         cls.logger.debug("Search for users with query {}, sort {}, order {}".format(q, sort, order))
         users = list()
         num_users = 0
@@ -188,18 +203,22 @@
         else:
             cls.logger.info("Got {}/{} users".format(num_users, max_num_users))
         # end if
 
         return users
 
     @classmethod
-    def search_repos_of_language(cls, language: str, max_num_repos: int = float("inf"),
-                                 is_allow_fork: bool = False,
-                                 max_retry_times: int = float("inf"),
-                                 strategies: List[str] = None) -> List[Repository]:
+    def search_repos_of_language(
+        cls,
+        language: str,
+        max_num_repos: int = float("inf"),
+        is_allow_fork: bool = False,
+        max_retry_times: int = float("inf"),
+        strategies: List[str] = None,
+    ) -> List[Repository]:
         """
         Searches for all the repos of the language.
         :return: a list of full names of matching repos.
         """
         if strategies is None:
             strategies = ["search_repos", "search_users"]
         # end if
@@ -213,15 +232,20 @@
         names_repos = dict()
 
         try:
             # Strategy 1: search repos (limited to 1000)
             strategy = "search_repos"
             if strategy in strategies:
                 cls.logger.info("Using strategy {}".format(strategy))
-                new_repos = cls.search_repos("language:{}".format(language), is_allow_fork=is_allow_fork, max_retry_times=max_retry_times, max_num_repos=max_num_repos)
+                new_repos = cls.search_repos(
+                    "language:{}".format(language),
+                    is_allow_fork=is_allow_fork,
+                    max_retry_times=max_retry_times,
+                    max_num_repos=max_num_repos,
+                )
                 for repo in new_repos:
                     names_repos[repo.full_name] = repo
                 # end for
                 cls.logger.warning("Progress {}/{} repos.".format(len(names_repos), max_num_repos))
                 if len(names_repos) >= max_num_repos:
                     return list(names_repos.values())
                 # end if
@@ -229,30 +253,45 @@
 
             # Strategy 2: search users (~37000?)
             strategy = "search_users"
             if strategy in strategies:
                 cls.logger.info("Using strategy {}".format(strategy))
                 s_users = set()
                 # s_users = s_users.union([u.login for u in cls.search_users("language:{}".format(language), sort="repositories", max_retry_times=max_retry_times)])
-                s_users = s_users.union([u.login for u in cls.search_users("language:{}".format(language), sort="followers", max_retry_times=max_retry_times)])
+                s_users = s_users.union(
+                    [
+                        u.login
+                        for u in cls.search_users(
+                            "language:{}".format(language), sort="followers", max_retry_times=max_retry_times
+                        )
+                    ]
+                )
                 # s_users = s_users.union([u.login for u in cls.search_users("language:{}".format(language), sort="joined", max_retry_times=max_retry_times)])
                 users_count = 0
                 total_users_count = len(s_users)
                 for user in s_users:
                     try:
-                        new_repos = cls.search_repos("language:{} user:{}".format(language, user), is_allow_fork=is_allow_fork, max_retry_times=max_retry_times)
+                        new_repos = cls.search_repos(
+                            "language:{} user:{}".format(language, user),
+                            is_allow_fork=is_allow_fork,
+                            max_retry_times=max_retry_times,
+                        )
                     except GithubException as e:
                         cls.logger.warning("Cannot get the repos of user {}".format(user))
                         continue
                     # end try
                     for repo in new_repos:
                         names_repos[repo.full_name] = repo
                     # end for
                     users_count += 1
-                    cls.logger.debug("Progress {}/{} repos, {}/{} users.".format(len(names_repos), max_num_repos, users_count, total_users_count))
+                    cls.logger.debug(
+                        "Progress {}/{} repos, {}/{} users.".format(
+                            len(names_repos), max_num_repos, users_count, total_users_count
+                        )
+                    )
                     if len(names_repos) >= max_num_repos:
                         return list(names_repos.values())
                     # end if
                 # end for
             # end if
 
             # Strategy 3: enum users (?)
```

### Comparing `seutil-0.8.7/seutil/IOUtils.py` & `seutil-0.8.8/src/seutil/IOUtils.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 import shutil
 import subprocess
 import typing_inspect
 import yaml
 
 
 def is_obj_record_class(obj: Any) -> bool:
-    return obj is not None \
-           and isinstance(obj, recordclass.mutabletuple) or isinstance(obj, recordclass.dataobject)
+    return obj is not None and isinstance(obj, recordclass.mutabletuple) or isinstance(obj, recordclass.dataobject)
 
 
 def is_clz_record_class(clz: Type) -> bool:
-    return clz is not None \
-           and inspect.isclass(clz) \
-           and (issubclass(clz, recordclass.mutabletuple) or issubclass(clz, recordclass.dataobject))
-
+    return (
+        clz is not None
+        and inspect.isclass(clz)
+        and (issubclass(clz, recordclass.mutabletuple) or issubclass(clz, recordclass.dataobject))
+    )
 
 
 class IOUtils:
     """
     Utility functions for I/O.
     """
 
@@ -68,17 +68,15 @@
     @classmethod
     def has_dir(cls, dirname) -> bool:
         return os.path.isdir(dirname)
 
     # Deprecated
     # Use pathlib.Path.mkdir() instead
     @classmethod
-    def mk_dir(cls, dirname, mode=0o777,
-               is_remove_if_exists: bool = False,
-               is_make_parent: bool = True):
+    def mk_dir(cls, dirname, mode=0o777, is_remove_if_exists: bool = False, is_make_parent: bool = True):
         """
         Makes the directory.
         :param dirname: the name of the directory.
         :param mode: mode of the directory.
         :param is_remove_if_exists: if the directory with name already exists, whether to remove.
         :param is_make_parent: if make parent directory if not exists.
         """
@@ -97,18 +95,18 @@
                 raise FileNotFoundError("Path not found: {}".format(parent_dir))
         # end if
         os.mkdir(dirname, mode)
         return
 
     @classmethod
     def rm_dir(
-            cls,
-            path: Path,
-            ignore_non_exist: bool = True,
-            force: bool = True,
+        cls,
+        path: Path,
+        ignore_non_exist: bool = True,
+        force: bool = True,
     ):
         """
         Removes the directory.
         :param path: the name of the directory.
         :param ignore_non_exist: ignores error if the directory does not exist.
         :param force: force remove the directory even it's non-empty.
         """
@@ -125,18 +123,18 @@
                 raise FileNotFoundError("Trying to remove non-exist directory {}".format(path))
             # end if
         # end if
         return
 
     @classmethod
     def rm(
-            cls,
-            path: Path,
-            ignore_non_exist: bool = True,
-            force: bool = True,
+        cls,
+        path: Path,
+        ignore_non_exist: bool = True,
+        force: bool = True,
     ):
         """
         Removes the file/dir.
         :param path: the path to the file/dir to remove.
         :param ignore_non_exist: ignores error if the file/dir does not exist.
         :param force: force remove the file even it's protected / dir even it's non-empty.
         """
@@ -149,22 +147,22 @@
                 if not ignore_non_exist:
                     raise IOError(f"{path} does not exist")
 
     # ----------
     # File operations
 
     class Format(Enum):
-        txt = 0,  # Plain text format
-        pkl = 1,  # Pickle format
-        jsonPretty = 2,  # Json format, with pretty-printing
-        jsonNoSort = 3,  # Json format, with pretty-printing, without sorting the keys in dictionary
-        json = 4,  # Json format, without pretty-printing (eveything on one line)
-        jsonList = 5,  # Json format, assuming a list structure and put each item on one line
-        txtList = 6,  # Plain text format, dump/load as a list where each line is an element
-        yaml = 7,  # YAML format
+        txt = (0,)  # Plain text format
+        pkl = (1,)  # Pickle format
+        jsonPretty = (2,)  # Json format, with pretty-printing
+        jsonNoSort = (3,)  # Json format, with pretty-printing, without sorting the keys in dictionary
+        json = (4,)  # Json format, without pretty-printing (eveything on one line)
+        jsonList = (5,)  # Json format, assuming a list structure and put each item on one line
+        txtList = (6,)  # Plain text format, dump/load as a list where each line is an element
+        yaml = (7,)  # YAML format
 
         @classmethod
         def from_str(cls, string: str) -> "IOUtils.Format":
             return {
                 "pkl": IOUtils.Format.pkl,
                 "json": IOUtils.Format.jsonPretty,
                 "json-nosort": IOUtils.Format.jsonNoSort,
@@ -181,29 +179,31 @@
                 IOUtils.Format.jsonNoSort: "json",
                 IOUtils.Format.json: "json",
                 IOUtils.Format.jsonList: "jsonl",
                 IOUtils.Format.txtList: "txt",
                 IOUtils.Format.yaml: "yml",
             }.get(self, "unknown")
 
-    IO_FORMATS: Dict[Format, Dict] = defaultdict(lambda: {
-        "mode": "t",
-        "dumpf": (lambda obj, f: f.write(obj)),
-        "loadf": (lambda f: f.read())
-    })
+    IO_FORMATS: Dict[Format, Dict] = defaultdict(
+        lambda: {"mode": "t", "dumpf": (lambda obj, f: f.write(obj)), "loadf": (lambda f: f.read())}
+    )
 
     IO_FORMATS[Format.pkl]["mode"] = "b"
     IO_FORMATS[Format.pkl]["dumpf"] = lambda obj, f: pkl.dump(obj, f, protocol=pkl.HIGHEST_PROTOCOL)
     IO_FORMATS[Format.pkl]["loadf"] = lambda f: pkl.load(f)
 
     IO_FORMATS[Format.jsonPretty]["dumpf"] = lambda obj, f: json.dump(obj, f, indent=4, sort_keys=True)
-    IO_FORMATS[Format.jsonPretty]["loadf"] = lambda f: yaml.load(f, Loader=yaml.FullLoader)  # allows some format errors (e.g., trailing commas)
+    IO_FORMATS[Format.jsonPretty]["loadf"] = lambda f: yaml.load(
+        f, Loader=yaml.FullLoader
+    )  # allows some format errors (e.g., trailing commas)
 
     IO_FORMATS[Format.jsonNoSort]["dumpf"] = lambda obj, f: json.dump(obj, f, indent=4)
-    IO_FORMATS[Format.jsonNoSort]["loadf"] = lambda f: yaml.load(f, Loader=yaml.FullLoader)  # allows some format errors (e.g., trailing commas)
+    IO_FORMATS[Format.jsonNoSort]["loadf"] = lambda f: yaml.load(
+        f, Loader=yaml.FullLoader
+    )  # allows some format errors (e.g., trailing commas)
 
     IO_FORMATS[Format.json]["dumpf"] = lambda obj, f: json.dump(obj, f, sort_keys=True)
     IO_FORMATS[Format.json]["loadf"] = lambda f: json.load(f)
 
     IO_FORMATS[Format.yaml]["dumpf"] = lambda obj, f: yaml.dump(obj, f)
     IO_FORMATS[Format.yaml]["loadf"] = lambda f: yaml.load(f, Loader=yaml.FullLoader)
 
@@ -232,49 +232,51 @@
         return f.read().splitlines()
 
     IO_FORMATS[Format.txtList]["dumpf"] = lambda obj, f: IOUtils.dumpf_txt_list(obj, f)
     IO_FORMATS[Format.txtList]["loadf"] = lambda f: IOUtils.loadf_txt_list(f)
 
     @classmethod
     def dump(
-            cls,
-            file_path: Union[str, Path],
-            obj: object,
-            fmt: Union[Format, str] = Format.jsonPretty,
-            append: bool = False,
+        cls,
+        file_path: Union[str, Path],
+        obj: object,
+        fmt: Union[Format, str] = Format.jsonPretty,
+        append: bool = False,
     ) -> None:
         """
         Saves an object to the file in the specified format.
         By default, the format is json pretty-print, and the existing content in the file will be erased.
         :param file_path: the file to save the object into.
         :param obj: the object to save.
         :param fmt: the format, one of IOUtils.Format.
         :param append: if true, appends to the file instead of erasing existing content in the file.
         """
         if isinstance(file_path, str):
             file_path = Path(file_path)
 
         file_path.touch(exist_ok=True)
 
-        if isinstance(fmt, str):  fmt = cls.Format.from_str(fmt)
+        if isinstance(fmt, str):
+            fmt = cls.Format.from_str(fmt)
         conf = cls.IO_FORMATS[fmt]
 
         write_mode = "w" if not append else "a"
         with open(file_path, write_mode + conf["mode"]) as f:
             conf["dumpf"](obj, f)
 
         return
 
     @classmethod
     def load(cls, file_path: Union[str, Path], fmt: Union[Format, str] = Format.jsonPretty) -> Any:
         if isinstance(file_path, str):
             file_path = Path(file_path)
         # end if
 
-        if isinstance(fmt, str):  fmt = cls.Format.from_str(fmt)
+        if isinstance(fmt, str):
+            fmt = cls.Format.from_str(fmt)
         conf = cls.IO_FORMATS[fmt]
 
         try:
             with open(file_path, "r" + conf["mode"]) as f:
                 obj = conf["loadf"](f)
             # end with
         except FileNotFoundError as e:
@@ -285,19 +287,21 @@
 
     @classmethod
     def load_json_stream(cls, file_path: Union[str, Path], fmt: Union[Format, str] = Format.jsonPretty):
         """
         Reads large json file containing a list of data iteratively. Returns a generator function.
         """
         import ijson
+
         if isinstance(file_path, str):
             file_path = Path(file_path)
         # end if
 
-        if isinstance(fmt, str):  fmt = cls.Format.from_str(fmt)
+        if isinstance(fmt, str):
+            fmt = cls.Format.from_str(fmt)
         conf = cls.IO_FORMATS[fmt]
 
         try:
             with open(file_path, "r" + conf["mode"]) as f:
                 objects = ijson.items(f, "item")
                 for obj in objects:
                     yield obj
@@ -400,15 +404,17 @@
             # None value
             return None
         elif clz is not None and typing_inspect.get_origin(clz) == list:
             # List[XXX]
             return [cls.dejsonfy(item, clz.__args__[0]) for item in data]
         elif clz is not None and typing_inspect.get_origin(clz) == tuple:
             # Tuple[XXX]
-            return tuple([cls.dejsonfy(item, clz.__args__[min(i, len(clz.__args__)-1)]) for i, item in enumerate(data)])
+            return tuple(
+                [cls.dejsonfy(item, clz.__args__[min(i, len(clz.__args__) - 1)]) for i, item in enumerate(data)]
+            )
         elif clz is not None and typing_inspect.get_origin(clz) == set:
             # Set[XXX]
             return set([cls.dejsonfy(item, clz.__args__[0]) for item in data])
         elif clz is not None and hasattr(clz, cls.DEJSONFY_FUNC_NAME):
             # with dejsonfy function
             return clz.dejsonfy(data)
         elif isinstance(data, list):
```

### Comparing `seutil-0.8.7/seutil/LoggingUtils.py` & `seutil-0.8.8/src/seutil/LoggingUtils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 import sys
 from logging.handlers import RotatingFileHandler
 
 
 class LoggingUtils:
-
     logging_format = "[{relativeCreated:6.0f}{levelname[0]}]{name}: {message}"
     logging_format_detail = "[{asctime}|{relativeCreated:.3f}|{levelname:7}]{name}: {message} [@{filename}:{lineno}|{funcName}|pid {process}|tid {thread}]"
 
     # Copied from logging
     DEBUG = logging.DEBUG
     INFO = logging.INFO
     WARNING = logging.WARNING
@@ -45,16 +44,15 @@
         # end if
         cls.refresh_loggers()
         return
 
     loggers = list()
 
     @classmethod
-    def get_logger(cls, name: str,
-                   level: int = None) -> logging.Logger:
+    def get_logger(cls, name: str, level: int = None) -> logging.Logger:
         if level is None:
             level = cls.default_level
         # end if
 
         # Always use the same handlers
         handlers = cls.default_handlers
```

### Comparing `seutil-0.8.7/seutil/MiscUtils.py` & `seutil-0.8.8/src/seutil/MiscUtils.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,16 +41,16 @@
     Counts the length with the iterator.
     """
     return sum(1 for _ in iterator)
 
 
 # Human-readable numbers
 
-POWERS = [10 ** x for x in (3, 6, 9, 12, 15, 18, 21, 24)]
-HUMAN_READABLE_POWERS = ('K', 'M', 'B', 'T', 'Qa', 'Qi', 'Sx', 'Sp')
+POWERS = [10**x for x in (3, 6, 9, 12, 15, 18, 21, 24)]
+HUMAN_READABLE_POWERS = ("K", "M", "B", "T", "Qa", "Qi", "Sx", "Sp")
 
 
 def itos_human_readable(value: int, precision: int = 1) -> str:
     """
     Converts a large integer to a human-readable string representation.
     :return the human-readable string representation of the int.
     :raises TypeError if the value passed was unable to be coaxed into int.
@@ -74,21 +74,21 @@
             return formatted + HUMAN_READABLE_POWERS[ordinal - 1]
     return str(value)
 
 
 def chunks(l, n):
     """Yield successive n-sized chunks from l."""
     for i in range(0, len(l), n):
-        yield l[i:i + n]
+        yield l[i : i + n]
 
 
 # Class Property
 
-class ClassPropertyDescriptor(object):
 
+class ClassPropertyDescriptor(object):
     def __init__(self, fget, fset=None):
         self.fget = fget
         self.fset = fset
 
     def __get__(self, obj, klass=None):
         if klass is None:
             klass = type(obj)
@@ -102,12 +102,13 @@
 
     def setter(self, func):
         if not isinstance(func, (classmethod, staticmethod)):
             func = classmethod(func)
         self.fset = func
         return self
 
+
 def classproperty(func):
     if not isinstance(func, (classmethod, staticmethod)):
         func = classmethod(func)
 
     return ClassPropertyDescriptor(func)
```

### Comparing `seutil-0.8.7/seutil/Stream.py` & `seutil-0.8.8/src/seutil/Stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .IOUtils import IOUtils
 
 
 class Stream:
     """
     Streams help manipulate sequences of objects.
     """
+
     def __init__(self):
         self.items = list()
         return
 
     @classmethod
     def of(cls, one_or_more_items):
         """
@@ -30,29 +31,33 @@
     @classmethod
     def of_files(cls, dir_path: Union[str, Path]):
         """
         Get a stream of the files under the directory.
         """
         with IOUtils.cd(dir_path):
             cmd_find = "find -mindepth 1 -maxdepth 1 -type f"
-            files = subprocess.run(["bash","-c",cmd_find], stdout=subprocess.PIPE).stdout.decode("utf-8").split("\n")[:-1]
+            files = (
+                subprocess.run(["bash", "-c", cmd_find], stdout=subprocess.PIPE).stdout.decode("utf-8").split("\n")[:-1]
+            )
         # end with
         files = [file[2:] for file in files]
         stream = cls.of(files)
         stream.sorted()
         return stream
 
     @classmethod
     def of_dirs(cls, dir_path: Union[str, Path]):
         """
         Get a stream of the sub-directories under the directory.
         """
         with IOUtils.cd(dir_path):
             cmd_find = "find -mindepth 1 -maxdepth 1 -type d"
-            dirs = subprocess.run(["bash","-c",cmd_find], stdout=subprocess.PIPE).stdout.decode("utf-8").split("\n")[:-1]
+            dirs = (
+                subprocess.run(["bash", "-c", cmd_find], stdout=subprocess.PIPE).stdout.decode("utf-8").split("\n")[:-1]
+            )
         # end with
         dirs = [dir[2:] for dir in dirs]
         stream = cls.of(dirs)
         stream.sorted()
         return stream
 
     def filter(self, predicate_func: Callable[[object], bool]):
@@ -63,54 +68,51 @@
 
     def count(self):
         return sum(self.items)
 
     def reduce(self, count_func: Callable[[str], float] = lambda x: 1):
         return sum([count_func(f) for f in self.items])
 
-    def sorted(self, key: Callable[[str], object] = lambda f: f,
-               reverse: bool = False):
+    def sorted(self, key: Callable[[str], object] = lambda f: f, reverse: bool = False):
         """
         Sorts the list of files in the dataset.
         """
         list.sort(self.items, key=key, reverse=reverse)
         return self
 
-    def map(self, map_func: Callable[[str], object],
-            errors: str = "raise", default: object = ""):
+    def map(self, map_func: Callable[[str], object], errors: str = "raise", default: object = ""):
         def new_items_generator():
             for item in self.items:
                 try:
                     new_item = map_func(item)
                 except:
                     if errors == "ignore":
                         yield default
                     else:
                         raise
                 else:
                     yield new_item
             # end for
+
         # end def
         return Stream.of(new_items_generator())
 
-    def peak(self, peak_func: Callable[[str], None],
-             errors: str = "ignore"):
+    def peak(self, peak_func: Callable[[str], None], errors: str = "ignore"):
         for item in self.items:
             try:
                 peak_func(item)
             except:
                 if errors == "ignore":
                     continue
                 else:
                     raise
         # end for
         return self
 
-    def split(self, fraction_list: List[float],
-              count_func: Callable[[str], float] = lambda x: 1):
+    def split(self, fraction_list: List[float], count_func: Callable[[str], float] = lambda x: 1):
         """
         Splits the dataset as each part specified by the fractions (assumed to sum up to 1).
         Splitting is done by finding the cutting points. If randomization is needed, call shuffle first.
         :param count_func: customize the number of data counts in each file.
         """
         if self.is_empty():
             return tuple(Stream() for i in range(len(fraction_list)))
@@ -118,25 +120,27 @@
         count_list = [count_func(f) for f in self.items]
         cum_count_list = np.cumsum(count_list)
         cum_expected_count_list = [f * cum_count_list[-1] for f in np.cumsum(fraction_list)]
         cut_index_list = []
         last_i = 0
         for i, cum_count in enumerate(cum_count_list):
             if cum_count >= cum_expected_count_list[len(cut_index_list)]:
-                last_i = i+1
-                cut_index_list.append(i+1)
+                last_i = i + 1
+                cut_index_list.append(i + 1)
                 if len(cut_index_list) >= len(cum_expected_count_list):
                     break
                 # end if
         # end for if
         if last_i != len(cum_count_list):
             cut_index_list.append(len(cum_count_list))
         # end if
-        cut_index_list.insert(0,0)
-        return tuple(Stream.of(self.items[cut_index_list[i]:cut_index_list[i + 1]]) for i in range(len(cut_index_list) - 1))
+        cut_index_list.insert(0, 0)
+        return tuple(
+            Stream.of(self.items[cut_index_list[i] : cut_index_list[i + 1]]) for i in range(len(cut_index_list) - 1)
+        )
 
     def shuffle(self, seed=None):
         """
         Shuffles the list of files in the dataset.
         """
         random.seed(seed)
         random.shuffle(self.items)
@@ -170,10 +174,10 @@
         return "Stream with {} items".format(len(self.items))
 
     def __repr__(self):
         return self.__str__()
 
     def __add__(self, other):
         if isinstance(other, Stream):
-            return Stream.of(self.items+other.items)
+            return Stream.of(self.items + other.items)
         else:
             raise NotImplementedError
```

### Comparing `seutil-0.8.7/seutil/__init__.py` & `seutil-0.8.8/src/seutil/__init__.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.7/seutil/arg.py` & `seutil-0.8.8/src/seutil/arg.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.7/seutil/bash.py` & `seutil-0.8.8/src/seutil/bash.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,23 +30,19 @@
             "False",
         }
         if show_full_output:
             s += f"STDOUT:\n{self.stdout}\n"
             s += f"STDERR:\n{self.stderr}\n"
         else:
             if len(self.stdout) > 800:
-                s += (
-                    f"STDOUT (truncated):\n{self.stdout[:400]}...{self.stdout[-400:]}\n"
-                )
+                s += f"STDOUT (truncated):\n{self.stdout[:400]}...{self.stdout[-400:]}\n"
             else:
                 s += f"STDOUT:\n{self.stdout}\n"
             if len(self.stderr) > 800:
-                s += (
-                    f"STDERR (truncated):\n{self.stderr[:400]}...{self.stderr[-400:]}\n"
-                )
+                s += f"STDERR (truncated):\n{self.stderr[:400]}...{self.stderr[-400:]}\n"
             else:
                 s += f"STDERR:\n{self.stderr}\n"
         return s
 
     def __repr__(self) -> str:
         return self.__str__()
 
@@ -114,38 +110,29 @@
             process.wait()
             raise
         except:  # including KeyboardInterrupt, communicate handled that.
             process.kill()
             # we don't call process.wait() as .__exit__ does that for us.
             raise
         retcode = process.poll()
-    completed_process = subprocess.CompletedProcess(
-        process.args, retcode, stdout, stderr
-    )
+    completed_process = subprocess.CompletedProcess(process.args, retcode, stdout, stderr)
 
     # check return code
-    if (
-        check_returncode is not None
-        and completed_process.returncode != check_returncode
-    ):
+    if check_returncode is not None and completed_process.returncode != check_returncode:
         raise BashError(cmd, completed_process, check_returncode)
 
-    if (
-        completed_process.returncode != 0
-        and check_returncode is not None
-        and warn_nonzero
-    ):
+    if completed_process.returncode != 0 and check_returncode is not None and warn_nonzero:
         warnings.warn(
             f"Bash command `{cmd}` returned non-zero exit code: {completed_process.returncode}",
             RuntimeWarning,
         )
 
     # potentially update the environment variables
     if update_env:
-        envs = io.load(tempfile_update_env, io.Fmt.txtList)
+        envs = io.load(tempfile_update_env, io.fmts.txtList)
         if update_env_clear_existing:
             os.environ.clear()
         for env in envs:
             key, value = env.split("=", 1)
             os.environ[key] = value
         io.rm(tempfile_update_env)
```

### Comparing `seutil-0.8.7/seutil/ds/graph_common.py` & `seutil-0.8.8/src/seutil/ds/graph_common.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.7/seutil/ds/lattice.py` & `seutil-0.8.8/src/seutil/ds/lattice.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.7/seutil/ds/trie.py` & `seutil-0.8.8/src/seutil/ds/trie.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,15 @@
 
     def to_tree(self):
         """
         TODO: Converts the trie to a `seutil.ds.tree.Tree` (to be added).
         """
         raise NotImplementedError()
 
-    def get(
-        self, key: Iterable[TElem], default: Optional[TValue] = None
-    ) -> Optional[TValue]:
+    def get(self, key: Iterable[TElem], default: Optional[TValue] = None) -> Optional[TValue]:
         """
         Gets the value of the given key, or the default value if the key does not exist.
         """
         try:
             return self[key]
         except KeyError:
             return default
@@ -59,17 +57,15 @@
             if c not in cur:
                 raise KeyError(f"Key {key} does not exist in the trie")
             cur = cur[c]
         if self.empty_elem not in cur:
             raise KeyError(f"Key {key} does not exist in the trie")
         return cur[self.empty_elem]
 
-    def set(
-        self, key: Iterable[TElem], value: TValue = True, exist_ok: bool = True
-    ) -> TValue:
+    def set(self, key: Iterable[TElem], value: TValue = True, exist_ok: bool = True) -> TValue:
         """
         Sets the value of the given key.
         :param key: the key to set.
         :param value: the value to set, by default `True` if the value is not important.
         :param exist_ok: if the key already exists, whether to overwrite the value.
         :raises KeyError: if the key already exists and `exist_ok` is False.
         :return: the old value of the key, or `Trie.MISSING` if there was no old value.
@@ -85,17 +81,15 @@
             old_value = cur.get(self.empty_elem, self.MISSING)
             cur[self.empty_elem] = value
             return old_value
 
     def __setitem__(self, key: Iterable[TElem], value: TValue):
         self.set(key, value, exist_ok=True)
 
-    def compute(
-        self, key: Iterable[TElem], update_func: Callable[[Optional[TValue]], TValue]
-    ) -> TValue:
+    def compute(self, key: Iterable[TElem], update_func: Callable[[Optional[TValue]], TValue]) -> TValue:
         """
         Computes the value of the given key (potentially add/remove a key-value pair).
         Faster than get+set by avoiding searching for the key twice.
         :param key: the key to update.
         :param update_func: the function to update the value, which takes as input the old value (or `Trie.MISSING` if there was no old value), and returns the new value (or `Trie.MISSING` to indicate removing the key from trie).
         :return: the old value of the key, or `Trie.MISSING` if there was no old value.
         """
```

### Comparing `seutil-0.8.7/seutil/io.py` & `seutil-0.8.8/src/seutil/io.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 import bz2
 import collections
 import csv
 import dataclasses
+import enum
 import gzip
 import inspect
 import io
 import json
 import lzma
 import os
 import pickle as pkl
 import pydoc
 import shutil
 import tempfile
 import warnings
 from enum import Enum
 from pathlib import Path
-from typing import (Any, Callable, Dict, Iterator, List, Optional, Tuple, Type,
-                    TypeVar, Union, get_type_hints)
+from typing import (
+    Any,
+    Callable,
+    Iterator,
+    List,
+    Optional,
+    OrderedDict,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+    get_type_hints,
+)
 
-import recordclass
 import typing_inspect
 import yaml
 
 __all__ = [
     "cd",
     "rmdir",
     "rm",
@@ -53,44 +64,20 @@
 
 def _unify_path(path: Union[str, Path]) -> Path:
     if not isinstance(path, Path):
         path = Path(path)
     return path
 
 
-def _is_obj_record_class(obj: Any) -> bool:
-    return (
-        obj is not None
-        and isinstance(obj, recordclass.mutabletuple)
-        or isinstance(obj, recordclass.dataobject)
-    )
-
-
-def _is_clz_record_class(clz: Type) -> bool:
-    return (
-        clz is not None
-        and inspect.isclass(clz)
-        and (
-            issubclass(clz, recordclass.mutabletuple)
-            or issubclass(clz, recordclass.dataobject)
-        )
-    )
-
-
 def _is_obj_named_tuple(obj: Any) -> bool:
     return obj is not None and isinstance(obj, tuple) and hasattr(obj, "_fields")
 
 
 def _is_clz_named_tuple(clz: Type) -> bool:
-    return (
-        clz is not None
-        and inspect.isclass(clz)
-        and issubclass(clz, tuple)
-        and hasattr(clz, "_fields")
-    )
+    return clz is not None and inspect.isclass(clz) and issubclass(clz, tuple) and hasattr(clz, "_fields")
 
 
 # ==========
 # file and directory manipulation (creation/removal/browsing)
 # ==========
 
 
@@ -227,80 +214,172 @@
 # ==========
 
 
 # object before serialization
 TObj = TypeVar("TObj")
 # data after serialization, usually contain only primitive types and simple list and dict structures, that can be directly stored to disk
 TData = TypeVar("TData")
+# the target of deserialization, either a type or a type hint
+TType = TypeVar("TType")
+# the serializer callable: f(obj) -> data
+TSerializer = Callable[[TObj], TData]
+# the deserializer callable: f(data) -> obj OR f(data, type) -> obj
+TDeserializer = Union[Callable[[TData], TObj], Callable[[TData, TType], TObj]]
 
 
 _NON_TYPE = type(None)
 
 
-_SERIALIZERS: Dict[type, Callable[[TObj], TData]] = {}
-_DESERIALIZERS: Dict[type, Callable[[TData], TObj]] = {}
+class isobj_predefined(enum.Enum):
+    type_eq = enum.auto()
+    isinstance = enum.auto()
+
+
+class isclz_predefined(enum.Enum):
+    eq = enum.auto()
+    issubclass = enum.auto()
+
+
+@dataclasses.dataclass(frozen=True)
+class TypeAdapter:
+    isobj: Callable[[Any], bool]
+    isclz: Callable[[Type], bool]
+    serializer: Optional[TSerializer] = None
+    deserializer: Optional[TDeserializer] = None
+    deserializer_2args: bool = dataclasses.field(default=False, init=False)
+
+    def __post_init__(self):
+        if self.deserializer is not None and inspect.isfunction(self.deserializer):
+            deserializer_sign = inspect.signature(self.deserializer)
+            object.__setattr__(self, "deserializer_2args", len(deserializer_sign.parameters) >= 2)
+
+    @classmethod
+    def for_clz(
+        cls,
+        clz: Type,
+        isobj: Union[isobj_predefined, Callable[[Any], bool]] = isobj_predefined.isinstance,
+        isclz: Union[isclz_predefined, Callable[[Type], bool]] = isclz_predefined.issubclass,
+        serializer: Optional[TSerializer] = None,
+        deserializer: Optional[TDeserializer] = None,
+    ) -> "TypeAdapter":
+        """
+        Creates a type adapter for a type with predefined isobj and isclz checkers.
+        :param clz: the type to adapt.
+        :param isobj: the isobj checker, can use one of isobj_predefined:
+            * type_eq: check if the object strictly matches the given type.
+            * isinstance (default): check if the object is an instance of the given type.
+            Or, can use a custom checker, which takes an object and returns a bool.
+        :param isclz: the isclz checker, can use one of isclz_predefined:
+            * eq: check if the type strictly matches the given type.
+            * issubclass (default): check if the type is a subclass of the given type.
+            Or, can use a custom checker, which takes a type and returns a bool.
+        :param serializer: the serializer, can be None if only registering a deserializer.
+        :param deserializer: the deserializer, can be None if only registering a serializer.
+        :return: the type adapter.
+        """
+        if isinstance(isobj, isobj_predefined):
+            if isobj == isobj_predefined.type_eq:
+
+                def isobj(x):
+                    return type(x) == clz
+
+            elif isobj == isobj_predefined.isinstance:
+
+                def isobj(x):
+                    return isinstance(x, clz)
+
+        elif isobj is None:
+            raise ValueError("isobj cannot be None")
+
+        if isinstance(isclz, isclz_predefined):
+            if isclz == isclz_predefined.eq:
+
+                def isclz(x):
+                    return x == clz
+
+            elif isclz == isclz_predefined.issubclass:
+
+                def isclz(x):
+                    return inspect.isclass(x) and issubclass(x, clz)
+
+        elif isclz is None:
+            raise ValueError("isclz cannot be None")
 
+        return cls(isobj=isobj, isclz=isclz, serializer=serializer, deserializer=deserializer)
 
-def register_type(
+
+_ADAPTERS: OrderedDict[Any, TypeAdapter] = collections.OrderedDict()
+
+
+def has_adapter(key: Any) -> bool:
+    """
+    Checks if a type adapter is registered for the given key.
+    :param key: the key of the type adapter.
+    :return: if a type adapter is registered for the given key.
+    """
+    return key in _ADAPTERS
+
+
+def set_adapter(key: Any, adapter: TypeAdapter, replace_existing: bool = True) -> None:
+    """
+    Registers a type adapter for the given key.
+    :param key: the key of the type adapter.
+    :param adapter: the type adapter.
+    :param replace_existing: if True, replace the existing type adapter if any;
+        otherwise, do not try to change the existing type adapter.
+    :raises KeyError: if a type adapter for the given key already exists and replace_existing is False.
+    """
+    if key in _ADAPTERS and not replace_existing:
+        raise KeyError(f"TypeAdapter for {key} already exists")
+    _ADAPTERS[key] = adapter
+
+
+def set_adapter_simple(
     clz: Type,
     serializer: Optional[Callable[[TObj], TData]] = None,
-    deserializer: Optional[Callable[[TData], TObj]] = None,
-    replace: bool = True,
-) -> bool:
-    """
-    Register customized serializer and/or deserializer of a type.
-    The registered (de)serializer is only good for this particular type and *not* for its subtypes.
-    If an inheritable (de)serializer is desired, declare a method in the base class called `(de)serializer` instead.
-
-    :param clz: the type to register.
+    deserializer: Optional[Callable[[TData, Type], TObj]] = None,
+    replace_existing: bool = True,
+) -> None:
+    """
+    Registers a type adapter for the given class, using it as the key, and with the given serializer & deserializer.
+    :param clz: the class to set type adapter for.
     :param serializer: the serializer, can be None if only registering a deserializer.
     :param deserializer: the deserializer, can be None if only registering a serializer.
-    :param replace: if True, replace the existing (de)serializer if any; otherwise, do not change the existing (de)serializer.
-    :return: if any new (de)serializer is registered.
+    :param replace_existing: if True, replace the existing type adapter if any;
     """
-    changed = False
+    set_adapter(
+        clz,
+        TypeAdapter.for_clz(clz, serializer=serializer, deserializer=deserializer),
+        replace_existing=replace_existing,
+    )
 
-    if serializer is not None:
-        if clz in _SERIALIZERS and not replace:
-            pass
-        else:
-            _SERIALIZERS[clz] = serializer
-            changed = True
-    if deserializer is not None:
-        if clz in _DESERIALIZERS and not replace:
-            pass
-        else:
-            _DESERIALIZERS[clz] = deserializer
-            changed = True
-
-    return changed
-
-
-def unregister_type(
-    clz: Type, serializer: bool = True, deserializer: bool = True
-) -> bool:
-    """
-    Unregister customized serializer and/or deserializer of a type.
-    Similar to register_type, the unregistering only happens for this particular type and *not* for its subtypes.
-
-    :param clz: the type to unregister.
-    :param serializer: if True (default), unregister the serializer.
-    :param deserializer: if True (default), unregister the deserializer.
-    :return: if any (de)serializer is unregistered.
-    """
-    changed = False
-    if serializer:
-        if clz in _SERIALIZERS:
-            del _SERIALIZERS[clz]
-            changed = True
-    if deserializer:
-        if clz in _DESERIALIZERS:
-            del _DESERIALIZERS[clz]
-            changed = True
-    return changed
+
+def unset_adapter(key: Any) -> None:
+    """
+    Unregisters a type adapter for the given key.
+    :param key: the key of the type adapter.
+    """
+    if key in _ADAPTERS:
+        del _ADAPTERS[key]
+
+
+def rank_first_adapter(key: Any) -> None:
+    """
+    Moves the type adapter for the given key to the first position.
+    :param key: the key of the type adapter.
+    """
+    _ADAPTERS.move_to_end(key, last=False)
+
+
+def rank_last_adapter(key: Any) -> None:
+    """
+    Moves the type adapter for the given key to the last position.
+    :param key: the key of the type adapter.
+    """
+    _ADAPTERS.move_to_end(key, last=True)
 
 
 def serialize(
     obj: TObj,
     fmt: Optional["Formatter"] = None,
 ) -> TData:
     """
@@ -324,47 +403,37 @@
         # Call customized serialization method if exists
         return getattr(obj, "serialize")()
     elif _is_obj_named_tuple(obj):
         # NamedTuple
         return {k: serialize(v, fmt) for k, v in obj._asdict().items()}
     elif dataclasses.is_dataclass(obj):
         # Dataclass
-        return {
-            f.name: serialize(getattr(obj, f.name), fmt)
-            for f in dataclasses.fields(obj)
-        }
+        return {f.name: serialize(getattr(obj, f.name), fmt) for f in dataclasses.fields(obj)}
     elif isinstance(obj, (list, set, tuple)):
         # List-like: uniform to list; recursively serialize content
         return [serialize(item, fmt) for item in obj]
     elif isinstance(obj, dict):
         # Dict: recursively serialize content
         ret = {serialize(k, fmt): serialize(v, fmt) for k, v in obj.items()}
 
         # Json-like formats constraint: dict key must be str
         if fmt in [fmts.json, fmts.jsonPretty, fmts.jsonNoSort, fmts.jsonList]:
             ret = {str(k): v for k, v in ret.items()}
         return ret
     elif isinstance(obj, Enum):
         # Enum: use name
         return serialize(obj.name, fmt)
-    elif _is_obj_record_class(obj):
-        # RecordClass: convert to dict
-        if hasattr(obj, "__dict__"):
-            # Older versions of recordclass
-            return {k: serialize(v, fmt) for k, v in obj.__dict__.items()}
-        else:
-            # Newer versions of recordclass
-            return {f: serialize(getattr(obj, f), fmt) for f in obj.__fields__}
-    elif type(obj) in _SERIALIZERS:
-        # Use registered serializer if exists
-        return _SERIALIZERS[type(obj)](obj)
     else:
-        raise TypeError(
-            f"Cannot serialize object of type {type(obj)}, please consider writing a serialize() function"
-        )
+        # find in all registered type adapters
+        for _, adapter in _ADAPTERS.items():
+            if adapter.isobj(obj) and adapter.serializer is not None:
+                return adapter.serializer(obj)
+
+        # no serializer found
+        raise TypeError(f"Cannot serialize object of type {type(obj)}, please consider writing a serialize() function")
 
 
 class DeserializationError(RuntimeError):
     def __init__(self, data: TData, clz: Optional[Union[Type, str]], reason: str):
         self.data = data
         self.clz = clz
         self.reason = reason
@@ -434,40 +503,40 @@
             try:
                 ret = deserialize(data, inner_clz, error="raise")
             except DeserializationError:
                 continue
 
         if ret is None:
             if error == "raise":
-                raise DeserializationError(
-                    data, clz, "All inner types are incompatible"
-                )
+                raise DeserializationError(data, clz, "All inner types are incompatible")
             else:
                 return data
         else:
             return ret
 
     # None data, but not NoneType
     if data is None:
         if error == "raise":
             raise DeserializationError(data, clz, "None data for non-None type")
         else:
             return data
 
-    # Use registered deserializer if exists
-    if clz in _DESERIALIZERS:
-        return _DESERIALIZERS[clz](data)
+    # Find in all registered type adapters
+    for _, adapter in _ADAPTERS.items():
+        if adapter.isclz(clz) and adapter.deserializer is not None:
+            if adapter.deserializer_2args:
+                return adapter.deserializer(data, clz)
+            else:
+                return adapter.deserializer(data)
 
     # List-like types
     if clz_origin in [list, tuple, set, collections.deque, frozenset]:
         if not isinstance(data, list):
             if error == "raise":
-                raise DeserializationError(
-                    data, clz, "Data does not have list structure"
-                )
+                raise DeserializationError(data, clz, "Data does not have list structure")
             else:
                 return data
 
         if clz_origin == tuple:
             # Unpack list to tuple
             return tuple(
                 [
@@ -478,18 +547,15 @@
                         error=error,
                     )
                     for i, x in enumerate(data)
                 ]
             )
         else:
             # Unpack list
-            ret = [
-                deserialize(x, clz_args[0] if generic else None, error=error)
-                for x in data
-            ]
+            ret = [deserialize(x, clz_args[0] if generic else None, error=error) for x in data]
 
             if clz_origin != list:
                 # Convert to appropriate type
                 return clz_origin(ret)
             else:
                 return ret
 
@@ -498,17 +564,15 @@
         dict,
         collections.OrderedDict,
         collections.defaultdict,
         collections.Counter,
     ]:
         if not isinstance(data, dict):
             if error == "raise":
-                raise DeserializationError(
-                    data, clz, "Data does not have dict structure"
-                )
+                raise DeserializationError(data, clz, "Data does not have dict structure")
             else:
                 return data
 
         if clz_origin == collections.OrderedDict:
             warnings.warn(
                 f"The order of items in OrderedDict may not be preserved during deserialization",
                 InfoLossWarning,
@@ -540,22 +604,14 @@
             return clz[data]
         else:
             if error == "raise":
                 raise DeserializationError(data, clz, "Enum data must be str (name)")
             else:
                 return data
 
-    # RecordClass
-    if _is_clz_record_class(clz):
-        field_values = {}
-        for f, t in get_type_hints(clz).items():
-            if f in data:
-                field_values[f] = deserialize(data.get(f), t, error=error)
-        return clz(**field_values)
-
     # NamedTuple
     if _is_clz_named_tuple(clz):
         field_values = {}
         for f in clz._fields:
             if hasattr(clz, "_field_types"):
                 # for Python <3.9
                 t = clz._field_types.get(f)
@@ -571,17 +627,15 @@
     # DataClass
     if dataclasses.is_dataclass(clz):
         init_field_values = {}
         non_init_field_values = {}
         for f in dataclasses.fields(clz):
             if f.name in data:
                 field_values = init_field_values if f.init else non_init_field_values
-                field_values[f.name] = deserialize(
-                    data.get(f.name), f.type, error=error
-                )
+                field_values[f.name] = deserialize(data.get(f.name), f.type, error=error)
         obj = clz(**init_field_values)
         for f_name, f_value in non_init_field_values.items():
             # use object.__setattr__ in case clz is frozen
             object.__setattr__(obj, f_name, f_value)
         return obj
 
     # Primitive types
@@ -601,80 +655,127 @@
 
 
 # register (de)serializers for some popular 3rd party libraries
 
 try:
     import numpy as np
 
-    register_type(
+    set_adapter_simple(
         np.ndarray,
         serializer=lambda x: serialize(x.tolist()),
         deserializer=lambda x: np.array(x),
     )
 
     # integers
-    register_type(np.byte, serializer=np.byte.item, deserializer=np.byte)
-    register_type(np.short, serializer=np.short.item, deserializer=np.short)
-    register_type(np.intc, serializer=np.intc.item, deserializer=np.intc)
-    register_type(np.int_, serializer=np.int_.item, deserializer=np.int_)
-    register_type(np.longlong, serializer=np.longlong.item, deserializer=np.longlong)
+    set_adapter_simple(np.byte, serializer=np.byte.item, deserializer=np.byte)
+    set_adapter_simple(np.short, serializer=np.short.item, deserializer=np.short)
+    set_adapter_simple(np.intc, serializer=np.intc.item, deserializer=np.intc)
+    set_adapter_simple(np.int_, serializer=np.int_.item, deserializer=np.int_)
+    set_adapter_simple(np.longlong, serializer=np.longlong.item, deserializer=np.longlong)
 
     # unsigned integers
-    register_type(np.ubyte, serializer=np.ubyte.item, deserializer=np.ubyte)
-    register_type(np.ushort, serializer=np.ushort.item, deserializer=np.ushort)
-    register_type(np.uintc, serializer=np.uintc.item, deserializer=np.uintc)
-    register_type(np.uint, serializer=np.uint.item, deserializer=np.uint)
-    register_type(np.ulonglong, serializer=np.ulonglong.item, deserializer=np.ulonglong)
+    set_adapter_simple(np.ubyte, serializer=np.ubyte.item, deserializer=np.ubyte)
+    set_adapter_simple(np.ushort, serializer=np.ushort.item, deserializer=np.ushort)
+    set_adapter_simple(np.uintc, serializer=np.uintc.item, deserializer=np.uintc)
+    set_adapter_simple(np.uint, serializer=np.uint.item, deserializer=np.uint)
+    set_adapter_simple(np.ulonglong, serializer=np.ulonglong.item, deserializer=np.ulonglong)
 
     # floats
-    register_type(np.half, serializer=np.half.item, deserializer=np.half)
-    register_type(np.single, serializer=np.single.item, deserializer=np.single)
-    register_type(np.double, serializer=np.double.item, deserializer=np.double)
-    register_type(
-        np.longdouble, serializer=np.longdouble.item, deserializer=np.longdouble
-    )
+    set_adapter_simple(np.half, serializer=np.half.item, deserializer=np.half)
+    set_adapter_simple(np.single, serializer=np.single.item, deserializer=np.single)
+    set_adapter_simple(np.double, serializer=np.double.item, deserializer=np.double)
+    set_adapter_simple(np.longdouble, serializer=np.longdouble.item, deserializer=np.longdouble)
 
     # other scalars
-    register_type(np.bool_, serializer=np.bool_.item, deserializer=np.bool_)
+    set_adapter_simple(np.bool_, serializer=np.bool_.item, deserializer=np.bool_)
     # TODO: np.datetime64, np.timedelta64, np.object_, np.bytes_, np.str_, np.void, etc.
 except ImportError:
     pass
 
 
 try:
     import pandas as pd
 
     # series
-    register_type(
-        pd.Series, serializer=lambda x: serialize(x.to_dict()), deserializer=pd.Series
-    )
+    set_adapter_simple(pd.Series, serializer=lambda x: serialize(x.to_dict()), deserializer=pd.Series)
 
     # dataframe
-    register_type(
+    set_adapter_simple(
         pd.DataFrame,
         serializer=lambda x: serialize(x.to_dict(orient="records")),
         deserializer=pd.DataFrame.from_records,
     )
 except ImportError:
     pass
 
 
 try:
     import torch
 
     # tensor
-    register_type(
+    set_adapter_simple(
         torch.Tensor,
         serializer=lambda x: serialize(x.tolist()),
         deserializer=torch.tensor,
     )
 except ImportError:
     pass
 
 
+try:
+    import recordclass
+
+    def _is_obj_record_class(obj: Any) -> bool:
+        return obj is not None and isinstance(obj, recordclass.mutabletuple) or isinstance(obj, recordclass.dataobject)
+
+    def _is_clz_record_class(clz: Type) -> bool:
+        return (
+            clz is not None
+            and inspect.isclass(clz)
+            and (issubclass(clz, recordclass.mutabletuple) or issubclass(clz, recordclass.dataobject))
+        )
+
+    def _serialize_recordclass(obj) -> dict:
+        warnings.warn(
+            "The support for recordclass may be dropped in the future. Please consider using dataclass instead.",
+            DeprecationWarning,
+        )
+        if hasattr(obj, "__dict__"):
+            # Older versions of recordclass
+            return {k: serialize(v) for k, v in obj.__dict__.items()}
+        else:
+            # Newer versions of recordclass
+            return {f: serialize(getattr(obj, f)) for f in obj.__fields__}
+
+    def _deseralize_recordclass(data, clz) -> Any:
+        warnings.warn(
+            "The support for recordclass may be dropped in the future. Please consider using dataclass instead.",
+            DeprecationWarning,
+        )
+        field_values = {}
+        for f, t in get_type_hints(clz).items():
+            if f in data:
+                # TODO: the error parameter is lost
+                field_values[f] = deserialize(data.get(f), t)
+        return clz(**field_values)
+
+    set_adapter(
+        recordclass.RecordClass,
+        TypeAdapter(
+            isobj=_is_obj_record_class,
+            isclz=_is_clz_record_class,
+            serializer=_serialize_recordclass,
+            deserializer=_deseralize_recordclass,
+        ),
+    )
+
+except ImportError:
+    pass
+
+
 # ==========
 # file read and write
 # ==========
 
 
 @dataclasses.dataclass(frozen=True)
 class Formatter:
@@ -721,27 +822,21 @@
     json = Formatter(
         writer=lambda f, obj: json.dump(obj, f, sort_keys=True),
         reader=lambda f: json.load(f),
         exts=["json"],
         serialize=True,
     )
     # Use yaml loader to allow formatting errors (e.g., trailing commas), but cannot handle unprintable chars
-    jsonFlexible = dataclasses.replace(
-        json, reader=lambda f: yaml.load(f, Loader=yaml.FullLoader)
-    )
+    jsonFlexible = dataclasses.replace(json, reader=lambda f: yaml.load(f, Loader=yaml.FullLoader))
     json_flexible = jsonFlexible
     # Pretty-print version with sorting keys
-    jsonPretty = dataclasses.replace(
-        json, writer=lambda f, obj: json.dump(obj, f, sort_keys=True, indent=4)
-    )
+    jsonPretty = dataclasses.replace(json, writer=lambda f, obj: json.dump(obj, f, sort_keys=True, indent=4))
     json_pretty = jsonPretty
     # Pretty-print version without sorting keys
-    jsonNoSort = dataclasses.replace(
-        json, writer=lambda f, obj: json.dump(obj, f, indent=4)
-    )
+    jsonNoSort = dataclasses.replace(json, writer=lambda f, obj: json.dump(obj, f, indent=4))
     json_no_sort = jsonNoSort
 
     # === jsonl (json list) ===
     jsonList = Formatter(
         writer=lambda item: json.dumps(item),
         reader=lambda line: json.loads(line),
         exts=["jsonl"],
@@ -993,17 +1088,15 @@
     if not fmt.line_mode:
         with open_fn(path, file_mode) as f:
             obj = fmt.reader(f)
             if serialization:
                 obj = deserialize(obj, clz, error=error)
             return obj
     else:
-        iterator = LoadIterator(
-            path, file_mode, open_fn, fmt, serialization, clz, error
-        )
+        iterator = LoadIterator(path, file_mode, open_fn, fmt, serialization, clz, error)
         if iter_line:
             return iterator
         else:
             return list(iterator)
 
 
 class LoadIterator(Iterator):
```

### Comparing `seutil-0.8.7/seutil/latex.py` & `seutil-0.8.8/src/seutil/latex.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 Utilities for generating/manipulating latex files.
 
 Some parts inspired by https://github.com/JelteF/PyLaTeX, but this module means to be more lightweight.
 """
 
 import abc
+import re
 import sys
 from enum import Enum
 from pathlib import Path
-from typing import List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from . import io, log
 
 logger = log.get_logger("latex")
 
 __all__ = ["LatexItem", "File"]
 
@@ -66,29 +67,62 @@
 
     def to_latex(self) -> str:
         return "\\" + self.USEMACRO_COMMAND + "{" + self.key + "}"
 
 
 class Macro(LatexItem):
     DEFMACRO_COMMAND = "DefMacro"
+    RE_DEF_MACRO = re.compile(r"\\DefMacro{(?P<key>[^}]+)}{(?P<value>[^}]*)}")
 
-    def __init__(self, key: str, value: Optional[str] = None):
+    def __init__(self, key: str, value: Optional[Any] = None):
         self.key = key
         self.value = value
 
     def use(self) -> str:
         # deprecated: use `MacroUse` instead
         return "\\" + MacroUse.USEMACRO_COMMAND + "{" + self.key + "}"
 
     def to_latex(self) -> str:
         if self.value is None:
             raise ValueError(f"Macro {self.key} has no value")
-        s = "\\" + self.DEFMACRO_COMMAND + "{" + self.key + "}{" + self.value + "}\n"
+        s = "\\" + self.DEFMACRO_COMMAND + "{" + self.key + "}{" + str(self.value) + "}\n"
         return s
 
+    @classmethod
+    def load_from_file(cls, file: Path) -> Dict[str, "Macro"]:
+        """
+        Loads the macros from a latex file.
+        Will convert the value of the macros to int or float, if possible.
+        TODO: does not work if the macro spans multiple lines.
+
+        :param file: the latex file.
+        :return: the indexed dictionary of {macro.key, macro}.
+        """
+        macros_indexed: Dict[str, Macro] = dict()
+
+        lines: List[str] = io.load(file, io.fmts.txtList)
+        for line in lines:
+            match = cls.RE_DEF_MACRO.fullmatch(line.strip())
+            if match is not None:
+                key = match.group("key")
+                value = match.group("value")
+
+                # Try to convert to int, then (if failing) float.
+                try:
+                    value = int(value)
+                except ValueError:
+                    try:
+                        value = float(value)
+                    except ValueError:
+                        pass
+
+                macros_indexed[key] = Macro(key, value)
+
+        return macros_indexed
+
 
 class File(LatexItem):
     class NewlineMode(Enum):
         auto = "auto"
         always = "always"
         never = "never"
 
@@ -151,18 +185,15 @@
         appending = is_append and path.exists()
         if appending:
             s = io.load(path, io.fmts.txt) + s
 
         # add the auto notice (only if it is a new file)
         if self.auto_notice and not appending:
             src = sys._getframe(1).f_code
-            s = (
-                f"%% Automatically generated by: {Path(src.co_filename).name} {src.co_name}\n"
-                + s
-            )
+            s = f"%% Automatically generated by: {Path(src.co_filename).name} {src.co_name}\n" + s
 
         # save
         io.dump(path, s, io.fmts.txt)
 
     def append(self, item: Union[str, LatexItem]) -> "File":
         if isinstance(item, str):
             item = Text(item)
```

### Comparing `seutil-0.8.7/seutil/latex_old/File.py` & `seutil-0.8.8/src/seutil/latex_old/File.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         """
         self.path: Path = path
         self.is_append: bool = is_append
 
         self.old_content: str = ""
         if self.is_append:
             if path.is_file():
-                self.old_content = io.load(path, io.Fmt.txt)
+                self.old_content = io.load(path, io.fmts.txt)
 
         # Contents
         self.items: List[Union[str, Macro, Table]] = list()
         self.macros_indexed: Dict[str, Macro] = dict()
         return
 
     def append(self, line: str) -> "File":
@@ -45,15 +45,15 @@
 
     def append_comment(self, line: str) -> "File":
         self.items.append("%% " + line)
         return self
 
     def save(self) -> None:
         content = self.old_content + "\n" + self.eval_content()
-        io.dump(self.path, content, io.Fmt.txt)
+        io.dump(self.path, content, io.fmts.txt)
         return
 
     def eval_content(self) -> str:
         content_lines: List[str] = list()
         if not self.is_append:
             content_lines.append(self.autogen_notice())
         # end if
```

### Comparing `seutil-0.8.7/seutil/latex_old/Macro.py` & `seutil-0.8.8/src/seutil/latex_old/Macro.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from .. import io, log
 
 logger = log.get_logger("latex.Macro")
 
 
 class Macro:
-
     T = TypeVar("T")
 
     def __init__(
         self,
         key: str,
         value: Optional[T] = None,
         value_func: Optional[Callable[[Dict[str, "Macro"]], T]] = None,
@@ -48,17 +47,15 @@
         logger.info(f"Macro {self.key} evaluates to {self.value}")
 
         tostring_func = self.tostring_func if self.tostring_func is not None else str
         return f"\\DefMacro{{{self.key}}}{{{tostring_func(self.value)}}}"
 
     # Deprecated
     @classmethod
-    def define(
-        cls, key: str, value_fmt: Union[str, Any], *values, **values_items
-    ) -> "Macro":
+    def define(cls, key: str, value_fmt: Union[str, Any], *values, **values_items) -> "Macro":
         if len(values) != 0 or len(values_items) != 0:
             return Macro(key, value=value_fmt.format(*values, **values_items))
         else:
             return Macro(key, value=value_fmt)
 
     def use(self) -> str:
         latex_line = f"\\UseMacro{{{self.key}}}"
@@ -74,15 +71,15 @@
         TODO: does not work if the macro spans multiple lines.
 
         :param file: the latex file.
         :return: the indexed dictionary of {macro.key, macro}.
         """
         macros_indexed: Dict[str, Macro] = dict()
 
-        lines: List[str] = io.load(file, io.Fmt.txtList)
+        lines: List[str] = io.load(file, io.fmts.txtList)
         for line in lines:
             match = cls.RE_DEF_MACRO.fullmatch(line.strip())
             if match is not None:
                 key = match.group("key")
                 value = match.group("value")
 
                 # Try to convert to int, then (if failing) float.
```

### Comparing `seutil-0.8.7/seutil/latex_old/Table.py` & `seutil-0.8.8/src/seutil/latex_old/Table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 class Table:
-
-    def __init__(self, big=False, font_size="small", align="center", caption="Default Table",
-                 label="fig:table:default"):
+    def __init__(
+        self, big=False, font_size="small", align="center", caption="Default Table", label="fig:table:default"
+    ):
         self.big = big
         self.font_size = font_size
         self.align = align
         self.caption = caption
         self.label = label
 
         self.tabular = ""
```

### Comparing `seutil-0.8.7/seutil/log.py` & `seutil-0.8.8/src/seutil/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,17 +55,15 @@
     root_logger.setLevel(logging.NOTSET + 1)
 
     if clear_handlers:
         root_logger.handlers = []
 
     # update the stderr handler
     handler_stderr.setLevel(level_stderr)
-    handler_stderr.setFormatter(
-        logging.Formatter(fmt_stderr, datefmt_stderr, style="{")
-    )
+    handler_stderr.setFormatter(logging.Formatter(fmt_stderr, datefmt_stderr, style="{"))
     root_logger.addHandler(handler_stderr)
 
     # update the file handler
     root_logger.removeHandler(handler_file)
 
     if log_file is not None:
         kwargs_file.setdefault("maxBytes", 10_000_000)
```

### Comparing `seutil-0.8.7/seutil/maven.py` & `seutil-0.8.8/src/seutil/maven.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import functools
 import os
 from pathlib import Path
 from typing import List, Set
 
 import xmltodict
 
-import seutil as su
+from . import bash, io, log, project
 
-logger = su.log.get_logger(__name__, su.log.INFO)
+logger = log.get_logger(__name__, log.INFO)
 
 SKIPS = "-Djacoco.skip -Dcheckstyle.skip -Drat.skip -Denforcer.skip -Danimal.sniffer.skip -Dmaven.javadoc.skip -Dfindbugs.skip -Dwarbucks.skip -Dmodernizer.skip -Dimpsort.skip -Dpmd.skip -Dxjc.skip -Dair.check.skip-all"
 
 
 @dataclasses.dataclass
 class MavenModule:
     group_id: str
@@ -46,92 +46,86 @@
 
     @functools.cached_property
     def test_classpath(self) -> str:
         return str(self.project.dir / self.rel_path / "target" / "test-classes")
 
     @functools.cached_property
     def dependency_classpath(self) -> str:
-        with su.io.cd(self.project.dir / self.rel_path):
-            tmp_file = su.io.mktmp(prefix="cp")
-            su.bash.run(
-                f"mvn dependency:build-classpath -Dmdep.outputFile={tmp_file}", 0
-            )
-            classpath = su.io.load(tmp_file, fmt=su.io.Fmt.txt)
-            su.io.rm(tmp_file)
+        with io.cd(self.project.dir / self.rel_path):
+            tmp_file = io.mktmp(prefix="cp")
+            bash.run(f"mvn dependency:build-classpath -Dmdep.outputFile={tmp_file}", 0)
+            classpath = io.load(tmp_file, fmt=io.fmts.txt)
+            io.rm(tmp_file)
             return classpath
 
     @functools.cached_property
     def exec_classpath(self) -> str:
-        with su.io.cd(self.project.dir / self.rel_path):
-            tmp_file = su.io.mktmp(prefix="ecp")
-            su.bash.run(
+        with io.cd(self.project.dir / self.rel_path):
+            tmp_file = io.mktmp(prefix="ecp")
+            bash.run(
                 f"mvn -q exec:exec -Dexec.executable=echo -Dexec.args='%classpath' > {tmp_file}",
                 0,
             )
-            classpath = su.io.load(tmp_file, fmt=su.io.Fmt.txt).strip()
-            su.io.rm(tmp_file)
+            classpath = io.load(tmp_file, fmt=io.fmts.txt).strip()
+            io.rm(tmp_file)
             return classpath
 
     @functools.cached_property
     def coordinate(self) -> str:
         return f"{self.group_id}:{self.artifact_id}:{self.version}"
 
     def backup_pom(self):
         if len(self.pom_modified) > 0:
-            raise RuntimeError(
-                f"Cannot backup pom.xml for {self.coordinate} because it has been modified"
-            )
-        with su.io.cd(self.project.dir / self.rel_path):
-            su.bash.run("cp pom.xml pom.xml.backup", 0)
+            raise RuntimeError(f"Cannot backup pom.xml for {self.coordinate} because it has been modified")
+        with io.cd(self.project.dir / self.rel_path):
+            bash.run("cp pom.xml pom.xml.backup", 0)
 
     def restore_pom(self):
-        with su.io.cd(self.project.dir / self.rel_path):
-            su.bash.run("cp pom.xml.backup pom.xml", 0)
+        with io.cd(self.project.dir / self.rel_path):
+            bash.run("cp pom.xml.backup pom.xml", 0)
         self.pom_modified.clear()
 
     def hack_pom_delete_plugin(self, artifact_id: str):
         """Hack the pom.xml to delete plugin with the given artifact_id"""
         modification = f"delete_plugin:{artifact_id}"
         if modification in self.pom_modified:
             logger.debug(f"pom.xml for {self.coordinate} already did {modification}")
             return
 
-        pom = xmltodict.parse(
-            su.io.load(self.project.dir / self.rel_path / "pom.xml", fmt=su.io.Fmt.txt)
-        )
+        pom = xmltodict.parse(io.load(self.project.dir / self.rel_path / "pom.xml", fmt=io.fmts.txt))
 
         plugins = pom.get("project", {}).get("build", {}).get("plugins", {}).get("plugin", [])
         if not isinstance(plugins, list):
             plugins = [plugins]
             pom.get("build", {}).get("plugins", {})["plugin"] = plugins
-            
+
         to_remove = None
         for i, plugin in enumerate(plugins):
             if plugin.get("artifactId") == artifact_id:
                 to_remove = i
                 break
         if to_remove is not None:
             del plugins[to_remove]
 
-        su.io.dump(
+        io.dump(
             self.project.dir / self.rel_path / "pom.xml",
             xmltodict.unparse(pom),
-            fmt=su.io.Fmt.txt,
+            fmt=io.fmts.txt,
         )
 
         self.pom_modified.add(modification)
 
     def compile(self, timeout=600, retry_with_package=True, clean=False):
-        with su.io.cd(self.dir / self.rel_path):
+        with io.cd(self.dir / self.rel_path):
             if clean:
-                su.bash.run("mvn clean", 0)
-            rr = su.bash.run(f"mvn test-compile {SKIPS}", timeout=timeout)
+                bash.run("mvn clean", 0)
+            rr = bash.run(f"mvn test-compile {SKIPS}", timeout=timeout)
             if rr.returncode != 0:
                 if retry_with_package:
-                    su.bash.run(f"mvn package -DskipTests {SKIPS}", 0, timeout=timeout)
+                    bash.run(f"mvn package -DskipTests {SKIPS}", 0, timeout=timeout)
                 else:
                     raise RuntimeError(f"Failed to compile")
 
     @property
     def dir(self) -> Path:
         return self.project.dir / self.rel_path
 
@@ -141,26 +135,26 @@
     multi_module: bool = False
     modules: List[MavenModule] = dataclasses.field(default_factory=list)
     dir: Path = None
 
     def serialize(self):
         return {
             "multi_module": self.multi_module,
-            "modules": su.io.serialize(self.modules),
+            "modules": io.serialize(self.modules),
         }
 
     @classmethod
-    def from_project(cls, project: su.project.Project) -> "MavenProject":
+    def from_project(cls, project: project.Project) -> "MavenProject":
         if not (project.dir / "pom.xml").exists():
             return None
         project.require_cloned()
         maven_proj = cls(dir=project.dir)
         # detect modules from the project
-        with su.io.cd(maven_proj.dir):
-            rr = su.bash.run(
+        with io.cd(maven_proj.dir):
+            rr = bash.run(
                 """mvn -Dexec.executable='bash' -Dexec.args='-c '"'"'echo ${project.groupId}:${project.artifactId}:${project.version} ${project.packaging} ${PWD}'"'"'' exec:exec -q""",
                 0,
             )
         for line in rr.stdout.splitlines():
             coord, packaging, abs_path = line.split(" ", 2)
             group_id, artifact_id, version = coord.split(":")
             rel_path = str(Path(abs_path).relative_to(maven_proj.dir))
@@ -187,37 +181,35 @@
             module.restore_pom()
 
     def hack_pom_delete_plugin(self, artifact_id: str):
         for module in self.modules:
             module.hack_pom_delete_plugin(artifact_id)
 
     def compile(self, timeout=600, retry_with_package=True, clean=False):
-        with su.io.cd(self.dir):
+        with io.cd(self.dir):
             if clean:
-                su.bash.run("mvn clean", 0)
-            rr = su.bash.run(f"mvn test-compile {SKIPS}", timeout=timeout)
+                bash.run("mvn clean", 0)
+            rr = bash.run(f"mvn test-compile {SKIPS}", timeout=timeout)
             if rr.returncode != 0:
                 if retry_with_package:
-                    su.bash.run(f"mvn package -DskipTests {SKIPS}", 0, timeout=timeout)
+                    bash.run(f"mvn package -DskipTests {SKIPS}", 0, timeout=timeout)
                 else:
                     raise RuntimeError(f"Failed to compile")
 
     def install(self, timeout=600, clean=False):
-        with su.io.cd(self.dir):
+        with io.cd(self.dir):
             if clean:
-                su.bash.run("mvn clean", 0)
-            rr = su.bash.run(f"mvn install -DskipTests {SKIPS}", 0, timeout=timeout)
+                bash.run("mvn clean", 0)
+            rr = bash.run(f"mvn install -DskipTests {SKIPS}", 0, timeout=timeout)
             if rr.returncode != 0:
                 raise RuntimeError(f"Failed to install")
 
     def get_module_by_path(self, file_path: Path) -> MavenModule:
         module_path = file_path.parent
         while module_path != Path("."):
-            if (module_path / "src/main/java").exists() or (
-                module_path / "src/test/java"
-            ).exists():
+            if (module_path / "src/main/java").exists() or (module_path / "src/test/java").exists():
                 break
             module_path = module_path.parent
         for module in self.modules:
             if os.path.realpath(module.rel_path) == os.path.realpath(module_path):
                 return module
         raise RuntimeError(f"Failed to find module for {file_path}, {module_path}")
```

### Comparing `seutil-0.8.7/seutil/pbar.py` & `seutil-0.8.8/src/seutil/pbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,15 @@
                 # write summaries of all instances
                 summaries = self.format_summaries()
                 self.out.write(summaries)
 
                 # write details of the current focused instance
                 focus = self.instances[self.cur]
                 ncols = _screen_shape_wrapper()(self.out)[0] - len(summaries)
-                self.out.write(
-                    focus.format_meter(**{**focus.format_dict, "ncols": ncols})
-                )
+                self.out.write(focus.format_meter(**{**focus.format_dict, "ncols": ncols}))
 
                 self.out.flush()
 
     def format_summaries(self) -> str:
         s = ""
         for i, instance in enumerate(self.instances):
             if i > 0:
```

### Comparing `seutil-0.8.7/seutil/project.py` & `seutil-0.8.8/src/seutil/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,28 +111,22 @@
             name = self.full_name
         assert exists in ["ignore", "remove", "pull", "error"]
         logger.info(f"Project {self.full_name}: cloning to {downloads_dir / name}")
 
         if (downloads_dir / name).exists():
             if exists == "ignore":
                 self._dir = downloads_dir / name
-                logger.info(
-                    f"Project {self.full_name}: existing at {downloads_dir / name}"
-                )
+                logger.info(f"Project {self.full_name}: existing at {downloads_dir / name}")
                 return
             elif exists == "remove":
                 io.rmdir(downloads_dir / name)
-                logger.info(
-                    f"Project {self.full_name}: removed existing at {downloads_dir / name}"
-                )
+                logger.info(f"Project {self.full_name}: removed existing at {downloads_dir / name}")
             elif exists == "pull":
                 self._dir = downloads_dir / name
-                logger.info(
-                    f"Project {self.full_name}: existing at {downloads_dir / name}"
-                )
+                logger.info(f"Project {self.full_name}: existing at {downloads_dir / name}")
                 self.fetch()
                 return
             elif exists == "error":
                 raise RuntimeError(
                     f"Project {self.full_name}: can not clone to existing directory {downloads_dir}/{name}"
                 )
 
@@ -152,17 +146,15 @@
     def remove(self, error_not_exists: bool = False) -> None:
         """
         Removes the project from the local directory.
         :param error_not_exists: if True, raise an error if the project has not been cloned yet.
         """
         if self._dir is None:
             if error_not_exists:
-                raise RuntimeError(
-                    f"Project {self.full_name}: not cloned yet, can not remove"
-                )
+                raise RuntimeError(f"Project {self.full_name}: not cloned yet, can not remove")
             else:
                 logger.info(f"Project {self.full_name}: already removed")
         else:
             io.rmdir(self._dir)
             self._dir = None
             logger.info(f"Project {self.full_name}: removed")
 
@@ -186,17 +178,15 @@
     def checkout(self, revision: str, forced: bool = False) -> None:
         """
         Checks out the given revision (or branch or tag) of the project.
         :param revision: the revision (or branch or tag) to checkout.
         :param forced: if True, do force checkout (discarding all local changes that might prevent a checkout).
         """
         self.require_cloned("checkout")
-        logger.info(
-            f"Project {self.full_name}: checking out revision {revision} ({forced=})"
-        )
+        logger.info(f"Project {self.full_name}: checking out revision {revision} ({forced=})")
 
         with io.cd(self._dir):
             cmd = f"git checkout {revision}"
             if forced:
                 cmd += " -f"
             bash.run(cmd, 0)
 
@@ -211,17 +201,15 @@
 
     def get_revisions_lattice(self) -> ds.lattice.Lattice:
         """
         Gets the revisions lattice of the project, ending at the current revision.
         """
         self.require_cloned("get_revisions_lattice")
         with io.cd(self._dir):
-            revisions = bash.run(
-                "git rev-list HEAD --topo-order --reverse --parents", 0
-            ).stdout.strip()
+            revisions = bash.run("git rev-list HEAD --topo-order --reverse --parents", 0).stdout.strip()
         revision2node = {}
         lattice = ds.lattice.Lattice()
         for line in revisions.splitlines():
             parts = line.split()
             revision = parts[0]
             node = lattice.add_node(parents=[revision2node[p] for p in parts[1:]])
             revision2node[revision] = node
@@ -268,21 +256,17 @@
                     results.append(func(self, revision))
             except KeyboardInterrupt:
                 raise
             except:
                 if errors == "ignore":
                     pass
                 elif errors == "warning":
-                    warnings.warn(
-                        f"Project {self.full_name}: error at revision {revision}: {traceback.format_exc()}"
-                    )
+                    warnings.warn(f"Project {self.full_name}: error at revision {revision}: {traceback.format_exc()}")
                 elif errors == "collate":
-                    warnings.warn(
-                        f"Project {self.full_name}: error at revision {revision}: {traceback.format_exc()}"
-                    )
+                    warnings.warn(f"Project {self.full_name}: error at revision {revision}: {traceback.format_exc()}")
                     errored_revisions.append(revision)
                     exc_infos.append(sys.exc_info())
                 elif errors == "error":
                     raise
             finally:
                 if pbar is not None:
                     pbar.update(1)
```

### Comparing `seutil-0.8.7/tests/ds/test_lattice.py` & `seutil-0.8.8/tests/ds/test_lattice.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.7/tests/ds/test_trie.py` & `seutil-0.8.8/tests/ds/test_trie.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,17 +257,15 @@
     trie1["beta"] = 2
     trie1["gamma"] = 3
 
     trie2 = su.ds.trie.Trie()
     trie2["alphaXXX"] = 1
     trie2["betaXXX"] = 1
 
-    e2overlaps = {
-        k: (t1, t2) for k, t1, t2 in trie1.overlaps_with(trie2, self_has_value=True)
-    }
+    e2overlaps = {k: (t1, t2) for k, t1, t2 in trie1.overlaps_with(trie2, self_has_value=True)}
     assert len(e2overlaps) == 2
     assert e2overlaps["alpha"][0][""] == 1
     assert "" not in e2overlaps["alpha"][1]
     assert e2overlaps["beta"][0][""] == 2
     assert "" not in e2overlaps["beta"][1]
 
 
@@ -277,13 +275,11 @@
     trie1["beta"] = 2
     trie1["gamma"] = 3
 
     trie2 = su.ds.trie.Trie()
     trie2["aaa"] = 4
     trie2["b"] = 5
 
-    e2overlaps = {
-        k: (t1, t2) for k, t1, t2 in trie1.overlaps_with(trie2, other_has_value=True)
-    }
+    e2overlaps = {k: (t1, t2) for k, t1, t2 in trie1.overlaps_with(trie2, other_has_value=True)}
     assert len(e2overlaps) == 1
     assert e2overlaps["b"][1][""] == 5
     assert "" not in e2overlaps["b"][0]
```

### Comparing `seutil-0.8.7/tests/test_BashUtils.py` & `seutil-0.8.8/tests/unit/test_BashUtils.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,21 +3,26 @@
 import os
 import unittest
 
 from seutil import BashUtils
 
 
 class test_BashUtils(unittest.TestCase):
-
     TEST_ENV_A_KEY = "TEST_BASHUTILS_ENV_A"
     TEST_ENV_A_VALUE = "aaa"
 
     def test_inherit_env(self):
         os.environ[self.TEST_ENV_A_KEY] = self.TEST_ENV_A_VALUE
         self.assertEqual(self.TEST_ENV_A_VALUE, BashUtils.run(f"echo -n ${self.TEST_ENV_A_KEY}").stdout)
         return
 
     def test_propagate_env(self):
         del os.environ[self.TEST_ENV_A_KEY]
         self.assertTrue(self.TEST_ENV_A_KEY not in os.environ)
-        self.assertEqual(self.TEST_ENV_A_VALUE, BashUtils.run(f"export {self.TEST_ENV_A_KEY}={self.TEST_ENV_A_VALUE}; echo -n ${self.TEST_ENV_A_KEY}", is_update_env=True).stdout)
+        self.assertEqual(
+            self.TEST_ENV_A_VALUE,
+            BashUtils.run(
+                f"export {self.TEST_ENV_A_KEY}={self.TEST_ENV_A_VALUE}; echo -n ${self.TEST_ENV_A_KEY}",
+                is_update_env=True,
+            ).stdout,
+        )
         self.assertEqual(self.TEST_ENV_A_VALUE, os.environ[self.TEST_ENV_A_KEY])
```

### Comparing `seutil-0.8.7/tests/test_GitHubUtils.py` & `seutil-0.8.8/tests/unit/test_GitHubUtils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import os
 import unittest
 from github.GithubException import GithubException
 
 from seutil import GitHubUtils
-from .TestSupport import TestSupport
 
 
 class test_GitHubUtils(unittest.TestCase):
-
     @unittest.skip("Require GitHub token, which is not available on CI")
     def test_search_repos_with_username(self):
         test_user = "google"
         test_repos_1 = GitHubUtils.search_repos("user:{}".format(test_user), language="Java")
         self.assertTrue(len(test_repos_1) > 0)
 
         test_repos_2 = GitHubUtils.search_repos("user:{} language:Java".format(test_user))
         self.assertTrue(len(test_repos_2) > 0)
 
         # Query separator "+" will not work
         test_repos_3 = GitHubUtils.search_repos("user:{}+language:Java".format(test_user), max_retry_times=0)
         self.assertTrue(len(test_repos_3) == 0)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `seutil-0.8.7/tests/test_arg.py` & `seutil-0.8.8/tests/unit/test_arg.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.7/tests/test_bash.py` & `seutil-0.8.8/tests/unit/test_bash.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.7/tests/test_io_path.py` & `seutil-0.8.8/tests/unit/test_io_path.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,24 +39,20 @@
     su.io.rmdir(tmp_dir)
 
 
 def test_mktmp_argument_dir():
     # Test argument dir of mktmp, mktmp_dir
     tmp_dir_1 = su.io.mktmp_dir()
 
-    tmp_dir_2 = su.io.mktmp_dir(
-        prefix=PREFIX, suffix=SUFFIX, separator=SEPARATOR, dir=tmp_dir_1
-    )
+    tmp_dir_2 = su.io.mktmp_dir(prefix=PREFIX, suffix=SUFFIX, separator=SEPARATOR, dir=tmp_dir_1)
     assert tmp_dir_2.is_dir()
     assert tmp_dir_2.name.startswith(PREFIX + SEPARATOR)
     assert tmp_dir_2.name.endswith(SEPARATOR + SUFFIX)
 
-    tmp_file = su.io.mktmp(
-        prefix=PREFIX, suffix=SUFFIX, separator=SEPARATOR, dir=tmp_dir_1
-    )
+    tmp_file = su.io.mktmp(prefix=PREFIX, suffix=SUFFIX, separator=SEPARATOR, dir=tmp_dir_1)
     assert tmp_file.is_file()
     assert tmp_file.name.startswith(PREFIX + SEPARATOR)
     assert tmp_file.name.endswith(SEPARATOR + SUFFIX)
 
     su.io.rmdir(tmp_dir_1)
```

### Comparing `seutil-0.8.7/tests/test_io_rw.py` & `seutil-0.8.8/tests/unit/test_io_rw.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,37 +4,31 @@
 import seutil as su
 
 # sample data that should not require serialization (thus works for all formats)
 SAMPLE_DATA = "Hello, world!"
 SAMPLE_LIST = [SAMPLE_DATA] * 20
 
 
-@pytest.mark.parametrize(
-    "name", ["a.txt", "a.pkl", "a.pickle", "a.json", "a.yml", "a.yaml"]
-)
+@pytest.mark.parametrize("name", ["a.txt", "a.pkl", "a.pickle", "a.json", "a.yml", "a.yaml"])
 def test_dump_load_auto_infer(tmp_path: Path, name: str):
     su.io.dump(tmp_path / name, SAMPLE_DATA)
     assert su.io.load(tmp_path / name) == SAMPLE_DATA
 
 
-@pytest.mark.parametrize(
-    "fmt", [fmt for fmt in su.io.fmts.all_fmts if not fmt.line_mode]
-)
+@pytest.mark.parametrize("fmt", [fmt for fmt in su.io.fmts.all_fmts if not fmt.line_mode])
 @pytest.mark.parametrize("compressor", su.io.compressors.all_compressors + [None])
 def test_dump_load(tmp_path: Path, fmt: su.io.Formatter, compressor: su.io.Compressor):
     su.io.dump(tmp_path / "a", SAMPLE_DATA, fmt=fmt, compressor=compressor)
     assert su.io.load(tmp_path / "a", fmt=fmt, compressor=compressor) == SAMPLE_DATA
 
 
 @pytest.mark.parametrize("name", ["a.jsonl"])
 def test_dump_load_list_auto_infer(tmp_path: Path, name: str):
     su.io.dump(tmp_path / name, SAMPLE_LIST)
     assert su.io.load(tmp_path / name) == SAMPLE_LIST
 
 
 @pytest.mark.parametrize("fmt", [fmt for fmt in su.io.fmts.all_fmts if fmt.line_mode])
 @pytest.mark.parametrize("compressor", su.io.compressors.all_compressors + [None])
-def test_dump_load_list(
-    tmp_path: Path, fmt: su.io.Formatter, compressor: su.io.Compressor
-):
+def test_dump_load_list(tmp_path: Path, fmt: su.io.Formatter, compressor: su.io.Compressor):
     su.io.dump(tmp_path / "a", SAMPLE_LIST, fmt=fmt, compressor=compressor)
     assert su.io.load(tmp_path / "a", fmt=fmt, compressor=compressor) == SAMPLE_LIST
```

### Comparing `seutil-0.8.7/tests/test_io_ser.py` & `seutil-0.8.8/tests/unit/test_io_ser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import collections
 import dataclasses
 import operator
 import warnings
 from typing import Callable, Dict, NamedTuple, Optional, Tuple
 
 import pytest
+
 import seutil as su
-from recordclass import RecordClass
 from seutil.io import TData, TObj
 
 _MISSING = object()
 
 
 def check_serialization_ok(
     obj: TObj,
@@ -179,50 +179,26 @@
     ExampleNamedTuple = collections.namedtuple("ExampleNamedTuple", ["e", "f", "g"])
     check_serialization_ok(
         obj=ExampleNamedTuple(99, [3, 5], 42.0),
         data={"e": 99, "f": [3, 5], "g": 42.0},
     )
 
 
-def test_ser_record_class():
-    ExampleNamedTuple = collections.namedtuple("ExampleNamedTuple", ["e", "f", "g"])
-
-    class ExampleRecordClass(RecordClass):
-        h: int
-        i: float
-        j: Dict[str, float] = None
-        k: Optional[ExampleNamedTuple] = None
-
-    check_serialization_ok(
-        obj=ExampleRecordClass(
-            h=4, i=0.5, j={"a": 4, "b": 6.0}, k=ExampleNamedTuple(99, [3, 5], 42.0)
-        ),
-        data={
-            "h": 4,
-            "i": 0.5,
-            "j": {"a": 4, "b": 6.0},
-            "k": {"e": 99, "f": [3, 5], "g": 42.0},
-        },
-    )
-
-
 def test_ser_data_class():
     ExampleNamedTuple = collections.namedtuple("ExampleNamedTuple", ["e", "f", "g"])
 
     @dataclasses.dataclass
     class ExampleDataClass:
         h: int
         i: float
         j: Dict[str, float] = None
         k: Optional[ExampleNamedTuple] = None
 
     check_serialization_ok(
-        obj=ExampleDataClass(
-            h=4, i=0.5, j={"a": 4, "b": 6.0}, k=ExampleNamedTuple(99, [3, 5], 42.0)
-        ),
+        obj=ExampleDataClass(h=4, i=0.5, j={"a": 4, "b": 6.0}, k=ExampleNamedTuple(99, [3, 5], 42.0)),
         data={
             "h": 4,
             "i": 0.5,
             "j": {"a": 4, "b": 6.0},
             "k": {"e": 99, "f": [3, 5], "g": 42.0},
         },
     )
```

### Comparing `seutil-0.8.7/tests/test_io_ser_3rd_party.py` & `seutil-0.8.8/tests/unit/test_io_ser_3rd_party.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+import collections
 import math
+from typing import Dict, Optional
+
 import pytest
 
 from .test_io_ser import check_serialization_ok
 
 
 class Test_io_ser_numpy:
-
     np = pytest.importorskip("numpy")
 
     def test_ser_array_int_1d(self):
         check_serialization_ok(
             obj=self.np.array([1, 2, 3]),
             data=[1, 2, 3],
             obj_eq=self.np.array_equal,
@@ -114,15 +116,14 @@
         check_serialization_ok(
             obj=obj,
             data=obj.item(),
         )
 
 
 class Test_io_ser_pandas:
-
     pd = pytest.importorskip("pandas")
 
     def test_ser_series(self):
         check_serialization_ok(
             obj=self.pd.Series([1, 2, 3]),
             data={0: 1, 1: 2, 2: 3},
             obj_eq=self.pd.Series.equals,
@@ -133,15 +134,14 @@
             obj=self.pd.DataFrame({"a": [1, 2, 3], "b": [4, 5, 6]}),
             data=[{"a": 1, "b": 4}, {"a": 2, "b": 5}, {"a": 3, "b": 6}],
             obj_eq=self.pd.DataFrame.equals,
         )
 
 
 class Test_io_ser_pytorch:
-
     torch = pytest.importorskip("torch")
 
     def test_ser_tensor_scaler_long(self):
         check_serialization_ok(
             obj=self.torch.tensor(1),
             data=1,
             obj_eq=self.torch.equal,
@@ -170,7 +170,31 @@
     )
     def test_ser_tensor_not_serializing_type_float(self):
         check_serialization_ok(
             obj=self.torch.tensor(4.2, dtype=self.torch.double),
             data=4.2,
             obj_eq=self.torch.equal,
         )
+
+
+class Test_io_ser_recordclass:
+    recordclass = pytest.importorskip("recordclass")
+
+    def test_ser_record_class(self):
+        ExampleNamedTuple = collections.namedtuple("ExampleNamedTuple", ["e", "f", "g"])
+
+        class ExampleRecordClass(self.recordclass.RecordClass):
+            h: int
+            i: float
+            j: Dict[str, float] = None
+            k: Optional[ExampleNamedTuple] = None
+
+        with pytest.deprecated_call():
+            check_serialization_ok(
+                obj=ExampleRecordClass(h=4, i=0.5, j={"a": 4, "b": 6.0}, k=ExampleNamedTuple(99, [3, 5], 42.0)),
+                data={
+                    "h": 4,
+                    "i": 0.5,
+                    "j": {"a": 4, "b": 6.0},
+                    "k": {"e": 99, "f": [3, 5], "g": 42.0},
+                },
+            )
```

### Comparing `seutil-0.8.7/tests/test_latex_integration.py` & `seutil-0.8.8/tests/integration/test_latex_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 
 import pytest
 
 import seutil as su
 
 resources_dir = Path(__file__).parent.parent / "resources"
-out_dir = Path(__file__).parent / "out"
+out_dir = Path(__file__).parent.parent / "out"
 
 
 main_tex_prefix = r"""
 \pdfminorversion=7
 \documentclass[letter]{article}
 
 %%%----------
@@ -103,40 +103,37 @@
 \caption{Example table.\label{tab:example}}
 \input{table}
 \end{small}
 \end{center}
 \end{table}
 \end{document}
 """,
-            su.io.Fmt.txt,
+            su.io.fmts.txt,
         )
         with su.io.cd(tmp_path):
             su.bash.run("latexmk -pdf main.tex", 0)
 
         # move outputs
         this_out_dir = out_dir / request.node.nodeid
         su.io.mkdir(this_out_dir)
         su.bash.run(f"mv {tmp_path}/* {this_out_dir}/", 0)
 
     def gen_numbers(self, path: Path):
         f = su.latex.File()
         for subset, subset_fn in [("all", lambda df: df)] + [
-            (sn, lambda df, sn=sn: df[df["sn"] == sn])
-            for sn in ["train", "val", "test"]
+            (sn, lambda df, sn=sn: df[df["sn"] == sn]) for sn in ["train", "val", "test"]
         ]:
             df_subset: self.pd.DataFrame = subset_fn(self.df_method)
             f.append(
                 su.latex.Macro(
                     f"corpus-{subset}-num_proj",
                     f"{len(df_subset['proj_name'].unique()):,d}",
                 )
             )
-            f.append(
-                su.latex.Macro(f"corpus-{subset}-num_test", f"{len(df_subset):,d}")
-            )
+            f.append(su.latex.Macro(f"corpus-{subset}-num_test", f"{len(df_subset):,d}"))
             f.append(
                 su.latex.Macro(
                     f"corpus-{subset}-tok_mut",
                     f"{df_subset['num_tok_mut'].mean():,.2f}",
                 )
             )
             f.append(
@@ -205,40 +202,37 @@
 \caption{Example table.\label{tab:example}}
 \input{table}
 \end{small}
 \end{center}
 \end{table}
 \end{document}
 """,
-            su.io.Fmt.txt,
+            su.io.fmts.txt,
         )
         with su.io.cd(tmp_path):
             su.bash.run("latexmk -pdf main.tex", 0)
 
         # move outputs
         this_out_dir = out_dir / request.node.nodeid
         su.io.mkdir(this_out_dir)
         su.bash.run(f"mv {tmp_path}/* {this_out_dir}/", 0)
 
     def gen_numbers(self, path: Path):
         f = su.latex.File(path / "numbers.tex")
         for subset, subset_fn in [("all", lambda df: df)] + [
-            (sn, lambda df, sn=sn: df[df["sn"] == sn])
-            for sn in ["train", "val", "test"]
+            (sn, lambda df, sn=sn: df[df["sn"] == sn]) for sn in ["train", "val", "test"]
         ]:
             df_subset: self.pd.DataFrame = subset_fn(self.df_method)
             f.append_macro(
                 su.latex.Macro(
                     f"corpus-{subset}-num_proj",
                     f"{len(df_subset['proj_name'].unique()):,d}",
                 )
             )
-            f.append_macro(
-                su.latex.Macro(f"corpus-{subset}-num_test", f"{len(df_subset):,d}")
-            )
+            f.append_macro(su.latex.Macro(f"corpus-{subset}-num_test", f"{len(df_subset):,d}"))
             f.append_macro(
                 su.latex.Macro(
                     f"corpus-{subset}-tok_mut",
                     f"{df_subset['num_tok_mut'].mean():,.2f}",
                 )
             )
             f.append_macro(
```

### Comparing `seutil-0.8.7/tests/test_log.py` & `seutil-0.8.8/tests/unit/test_log.py`

 * *Files identical despite different names*

### Comparing `seutil-0.8.7/tests/test_project.py` & `seutil-0.8.8/tests/unit/test_project.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,54 @@
-import logging
 import os
 from pathlib import Path
 
 import pytest
+
 import seutil as su
 
 resources_dir = Path(__file__).parent.parent / "resources"
 
 
-# we use the https://github.com/git-game/git-game as the test subject for the project module; I checkpointed the state of the repository on 2022-05-11 --- forked to my github account, and also downloaded+compressed as a tgz.
+# the repo used for testing: git-game/git-game version d851edda3009332dd5d3f8f949a102f279dad809 (on 2022/05/11)
 
 
 @pytest.fixture
 def local_gitgame_repo(tmp_path: Path):
-    """The git-game repo comes with this project as a test subject."""
+    """The repo stored locally, for testing pull/checkout operations without the need of internet."""
     os.chdir(tmp_path)
     git_game_tgz = resources_dir / "git-game.git.tgz"
     su.bash.run(f"tar -xzf {git_game_tgz}", 0)
 
     return su.project.Project(
         full_name="pengyunie_git-game",
         url=f"file://{tmp_path.absolute()}/git-game.git",
         data={"metadata1": "aaa", "metadata2": "bbb"},
     )
 
 
 @pytest.fixture
 def remote_gitgame_repo():
-    """The git-game repo on github."""
+    """The repo on github, for testing url analysis etc."""
     return su.project.Project(
         full_name="pengyunie_git-game",
-        url=f"https://github.com/pengyunie/git-game.git",
+        url="https://github.com/pengyunie/git-game.git",
         data={"metadata1": "aaa", "metadata2": "bbb"},
     )
 
 
 REMOTE_GITGAME_REPO_JSON = {
     "full_name": "pengyunie_git-game",
     "url": "https://github.com/pengyunie/git-game.git",
     "metadata1": "aaa",
     "metadata2": "bbb",
 }
 
 
 def test_deserialize(remote_gitgame_repo: su.project.Project):
-    assert (
-        su.io.deserialize(REMOTE_GITGAME_REPO_JSON, su.project.Project)
-        == remote_gitgame_repo
-    )
+    assert su.io.deserialize(REMOTE_GITGAME_REPO_JSON, su.project.Project) == remote_gitgame_repo
 
 
 def test_serialize(remote_gitgame_repo: su.project.Project):
     assert su.io.serialize(remote_gitgame_repo) == REMOTE_GITGAME_REPO_JSON
 
 
 def test_clone_local(local_gitgame_repo: su.project.Project, tmp_path: Path):
@@ -64,101 +61,71 @@
 def test_clone_local_name(local_gitgame_repo: su.project.Project, tmp_path: Path):
     local_gitgame_repo.clone(tmp_path, name="aaa")
     assert (tmp_path / "aaa").exists()
     assert (tmp_path / "aaa" / ".git").exists()
     assert local_gitgame_repo.dir == tmp_path / "aaa"
 
 
-def test_clone_local_exists_ignore(
-    local_gitgame_repo: su.project.Project, tmp_path: Path
-):
+def test_clone_local_exists_ignore(local_gitgame_repo: su.project.Project, tmp_path: Path):
     local_gitgame_repo.clone(tmp_path)
     assert (tmp_path / "pengyunie_git-game").exists()
 
     local_gitgame_repo.clone(tmp_path, exists="ignore")
     assert (tmp_path / "pengyunie_git-game").exists()
     assert (tmp_path / "pengyunie_git-game" / ".git").exists()
     assert local_gitgame_repo.dir == tmp_path / "pengyunie_git-game"
 
 
-def test_clone_local_exists_remove(
-    local_gitgame_repo: su.project.Project, tmp_path: Path
-):
+def test_clone_local_exists_remove(local_gitgame_repo: su.project.Project, tmp_path: Path):
     local_gitgame_repo.clone(tmp_path)
     assert (tmp_path / "pengyunie_git-game").exists()
     # touch a random file in the cloned directory, to test if it is later removed
-    su.io.dump(local_gitgame_repo.dir / "random.txt", "abc", su.io.Fmt.txt)
+    su.io.dump(local_gitgame_repo.dir / "random.txt", "abc", su.io.fmts.txt)
     assert (local_gitgame_repo.dir / "random.txt").exists()
 
     local_gitgame_repo.clone(tmp_path, exists="remove")
     assert (tmp_path / "pengyunie_git-game").exists()
     assert (tmp_path / "pengyunie_git-game" / ".git").exists()
     assert local_gitgame_repo.dir == tmp_path / "pengyunie_git-game"
     assert not (local_gitgame_repo.dir / "random.txt").exists()
 
 
-def test_clone_local_exists_pull(
-    local_gitgame_repo: su.project.Project, tmp_path: Path
-):
+def test_clone_local_exists_pull(local_gitgame_repo: su.project.Project, tmp_path: Path):
     local_gitgame_repo.clone(tmp_path)
     assert (tmp_path / "pengyunie_git-game").exists()
-    assert (
-        local_gitgame_repo.get_cur_revision()
-        == "d851edda3009332dd5d3f8f949a102f279dad809"
-    )
+    assert local_gitgame_repo.get_cur_revision() == "d851edda3009332dd5d3f8f949a102f279dad809"
     # undo the last commit, to test if it is later pulled back
     with su.io.cd(local_gitgame_repo.dir):
         su.bash.run("git reset --hard HEAD~1", 0)
-    assert (
-        local_gitgame_repo.get_cur_revision()
-        == "7c8c3ccc2f4bb118a657f1f7a7ab4e163d1b7a30"
-    )
+    assert local_gitgame_repo.get_cur_revision() == "7c8c3ccc2f4bb118a657f1f7a7ab4e163d1b7a30"
 
     local_gitgame_repo.clone(tmp_path, exists="pull")
     assert (tmp_path / "pengyunie_git-game").exists()
     assert (tmp_path / "pengyunie_git-game" / ".git").exists()
     assert local_gitgame_repo.dir == tmp_path / "pengyunie_git-game"
     with su.io.cd(local_gitgame_repo.dir):
         su.bash.run("git checkout origin/master", 0)
-    assert (
-        local_gitgame_repo.get_cur_revision()
-        == "d851edda3009332dd5d3f8f949a102f279dad809"
-    )
+    assert local_gitgame_repo.get_cur_revision() == "d851edda3009332dd5d3f8f949a102f279dad809"
 
 
-def test_clone_local_exists_error(
-    local_gitgame_repo: su.project.Project, tmp_path: Path
-):
+def test_clone_local_exists_error(local_gitgame_repo: su.project.Project, tmp_path: Path):
     local_gitgame_repo.clone(tmp_path)
     assert (tmp_path / "pengyunie_git-game").exists()
 
     with pytest.raises(RuntimeError):
         local_gitgame_repo.clone(tmp_path, exists="error")
 
 
-@pytest.mark.slow  # TODO: mark this item as something like "need internet" instead
-def test_clone_remote(remote_gitgame_repo: su.project.Project, tmp_path: Path):
-    remote_gitgame_repo.clone(tmp_path)
-    assert (tmp_path / "pengyunie_git-game").exists()
-    assert (tmp_path / "pengyunie_git-game" / ".git").exists()
-    assert remote_gitgame_repo.dir == tmp_path / "pengyunie_git-game"
-
-
-# for the remaining tests about the operations after cloning, it does not matter if the project is from local or online
-
-
 def test_set_cloned_dir(local_gitgame_repo: su.project.Project, tmp_path: Path):
     local_gitgame_repo.clone(tmp_path)
     assert (tmp_path / "pengyunie_git-game").exists()
     assert (tmp_path / "pengyunie_git-game" / ".git").exists()
     assert local_gitgame_repo.dir == tmp_path / "pengyunie_git-game"
 
-    su.bash.run(
-        f"mv {tmp_path / 'pengyunie_git-game'} {tmp_path / 'pengyunie_git-game2'}", 0
-    )
+    su.bash.run(f"mv {tmp_path / 'pengyunie_git-game'} {tmp_path / 'pengyunie_git-game2'}", 0)
     assert local_gitgame_repo.dir == tmp_path / "pengyunie_git-game"
 
     local_gitgame_repo.set_cloned_dir(tmp_path / "pengyunie_git-game2")
     assert local_gitgame_repo.dir == tmp_path / "pengyunie_git-game2"
 
 
 def test_remove(local_gitgame_repo: su.project.Project, tmp_path: Path):
@@ -170,76 +137,52 @@
     with pytest.raises(RuntimeError):
         local_gitgame_repo.dir
 
 
 def test_fetch(local_gitgame_repo: su.project.Project, tmp_path: Path):
     local_gitgame_repo.clone(tmp_path)
     assert (tmp_path / "pengyunie_git-game").exists()
-    assert (
-        local_gitgame_repo.get_cur_revision()
-        == "d851edda3009332dd5d3f8f949a102f279dad809"
-    )
+    assert local_gitgame_repo.get_cur_revision() == "d851edda3009332dd5d3f8f949a102f279dad809"
     # undo the last commit, to test if it is later pulled back
     with su.io.cd(local_gitgame_repo.dir):
         su.bash.run("git reset --hard HEAD~1", 0)
-    assert (
-        local_gitgame_repo.get_cur_revision()
-        == "7c8c3ccc2f4bb118a657f1f7a7ab4e163d1b7a30"
-    )
+    assert local_gitgame_repo.get_cur_revision() == "7c8c3ccc2f4bb118a657f1f7a7ab4e163d1b7a30"
 
     local_gitgame_repo.fetch()
     with su.io.cd(local_gitgame_repo.dir):
         su.bash.run("git checkout origin/master", 0)
-    assert (
-        local_gitgame_repo.get_cur_revision()
-        == "d851edda3009332dd5d3f8f949a102f279dad809"
-    )
+    assert local_gitgame_repo.get_cur_revision() == "d851edda3009332dd5d3f8f949a102f279dad809"
 
 
 def test_checkout(local_gitgame_repo: su.project.Project, tmp_path: Path):
     local_gitgame_repo.clone(tmp_path)
     assert (tmp_path / "pengyunie_git-game").exists()
-    assert (
-        local_gitgame_repo.get_cur_revision()
-        == "d851edda3009332dd5d3f8f949a102f279dad809"
-    )
+    assert local_gitgame_repo.get_cur_revision() == "d851edda3009332dd5d3f8f949a102f279dad809"
     local_gitgame_repo.checkout("7c8c3ccc2f4bb118a657f1f7a7ab4e163d1b7a30")
-    assert (
-        local_gitgame_repo.get_cur_revision()
-        == "7c8c3ccc2f4bb118a657f1f7a7ab4e163d1b7a30"
-    )
+    assert local_gitgame_repo.get_cur_revision() == "7c8c3ccc2f4bb118a657f1f7a7ab4e163d1b7a30"
 
 
 def test_checkout_forced(local_gitgame_repo: su.project.Project, tmp_path: Path):
     local_gitgame_repo.clone(tmp_path)
     assert (tmp_path / "pengyunie_git-game").exists()
-    assert (
-        local_gitgame_repo.get_cur_revision()
-        == "d851edda3009332dd5d3f8f949a102f279dad809"
-    )
+    assert local_gitgame_repo.get_cur_revision() == "d851edda3009332dd5d3f8f949a102f279dad809"
     # modify the README so that normal checkout should fail
-    su.io.dump(local_gitgame_repo.dir / "README.md", "modified", su.io.Fmt.txt)
+    su.io.dump(local_gitgame_repo.dir / "README.md", "modified", su.io.fmts.txt)
     with pytest.raises(su.bash.BashError):
         local_gitgame_repo.checkout("7c8c3ccc2f4bb118a657f1f7a7ab4e163d1b7a30")
 
     # a forced checkout should do it
     local_gitgame_repo.checkout("7c8c3ccc2f4bb118a657f1f7a7ab4e163d1b7a30", forced=True)
-    assert (
-        local_gitgame_repo.get_cur_revision()
-        == "7c8c3ccc2f4bb118a657f1f7a7ab4e163d1b7a30"
-    )
+    assert local_gitgame_repo.get_cur_revision() == "7c8c3ccc2f4bb118a657f1f7a7ab4e163d1b7a30"
 
 
 def test_get_cur_revision(local_gitgame_repo: su.project.Project, tmp_path: Path):
     local_gitgame_repo.clone(tmp_path)
     assert (tmp_path / "pengyunie_git-game").exists()
-    assert (
-        local_gitgame_repo.get_cur_revision()
-        == "d851edda3009332dd5d3f8f949a102f279dad809"
-    )
+    assert local_gitgame_repo.get_cur_revision() == "d851edda3009332dd5d3f8f949a102f279dad809"
 
 
 def test_get_revisions_lattice(local_gitgame_repo: su.project.Project, tmp_path: Path):
     local_gitgame_repo.clone(tmp_path)
     assert (tmp_path / "pengyunie_git-game").exists()
 
     lattice = local_gitgame_repo.get_revisions_lattice()
@@ -273,34 +216,30 @@
         return (p.get_cur_revision(), su.bash.run("pwd").stdout.strip())
 
     ret = local_gitgame_repo.for_each_revision(action, revisions)
     assert [x[0] for x in ret] == revisions
     assert [Path(x[1]) for x in ret] == [local_gitgame_repo.dir] * len(revisions)
 
 
-def test_for_each_revision_no_auto_checkout(
-    local_gitgame_repo: su.project.Project, tmp_path: Path
-):
+def test_for_each_revision_no_auto_checkout(local_gitgame_repo: su.project.Project, tmp_path: Path):
     local_gitgame_repo.clone(tmp_path)
 
     lattice = local_gitgame_repo.get_revisions_lattice()
     revisions = [n["revision"] for n in lattice.nodes()]
     local_gitgame_repo.checkout(revisions[0])
 
     def action(p: su.project.Project, r: str):
         return (p.get_cur_revision(), su.bash.run("pwd").stdout.strip())
 
     ret = local_gitgame_repo.for_each_revision(action, revisions, auto_checkout=False)
     assert [x[0] for x in ret] == [revisions[0]] * len(revisions)
     assert [Path(x[1]) for x in ret] == [local_gitgame_repo.dir] * len(revisions)
 
 
-def test_for_each_revision_errors_ignore(
-    local_gitgame_repo: su.project.Project, tmp_path: Path
-):
+def test_for_each_revision_errors_ignore(local_gitgame_repo: su.project.Project, tmp_path: Path):
     local_gitgame_repo.clone(tmp_path)
 
     lattice = local_gitgame_repo.get_revisions_lattice()
     revisions = [n["revision"] for n in lattice.nodes()]
 
     def action(p: su.project.Project, r: str):
         nonlocal revisions
@@ -357,17 +296,15 @@
     with pytest.raises(su.project.CollatedErrors) as exc_info:
         local_gitgame_repo.for_each_revision(action, revisions, errors="collate")
 
     assert exc_info.value.contexts == [revisions[0], revisions[-1]]
     assert len(recwarn.list) == 2
 
 
-def test_for_each_revision_errors_error(
-    local_gitgame_repo: su.project.Project, tmp_path: Path
-):
+def test_for_each_revision_errors_error(local_gitgame_repo: su.project.Project, tmp_path: Path):
     local_gitgame_repo.clone(tmp_path)
 
     lattice = local_gitgame_repo.get_revisions_lattice()
     revisions = [n["revision"] for n in lattice.nodes()]
     assert len(revisions) >= 2
 
     def action(p: su.project.Project, r: str):
```

