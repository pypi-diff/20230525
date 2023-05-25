# Comparing `tmp/dagster-shell-0.9.9rc1.tar.gz` & `tmp/dagster-shell-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-shell-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:53 2020, max compression
+gzip compressed data, was "dagster-shell-1.0.5.tar", last modified: Fri Aug 26 13:45:42 2022, max compression
```

## Comparing `dagster-shell-0.9.9rc1.tar` & `dagster-shell-1.0.5.tar`

### file list

```diff
@@ -1,28 +1,20 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      572 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      125 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/dagster_shell/
--rw-r--r--   0 bobchen    (501) staff       (20)      329 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     7450 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell/solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)     6050 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell/utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/dagster_shell.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      572 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/dagster_shell.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      673 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/dagster_shell.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/dagster_shell.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/dagster_shell.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)        8 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/dagster_shell.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/dagster_shell.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/dagster_shell_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)      404 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell_tests/conftest.py
--rw-r--r--   0 bobchen    (501) staff       (20)      184 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell_tests/example_shell_command_solid.py
--rw-r--r--   0 bobchen    (501) staff       (20)      226 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell_tests/example_shell_script_solid.py
--rw-r--r--   0 bobchen    (501) staff       (20)      479 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell_tests/test_examples.py
--rw-r--r--   0 bobchen    (501) staff       (20)     3350 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell_tests/test_solids.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2769 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell_tests/test_utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       91 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/dagster_shell_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:53.000000 dagster-shell-0.9.9rc1/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1012 2020-09-17 21:04:59.000000 dagster-shell-0.9.9rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:42.368535 dagster-shell-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-shell-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       65 2022-08-26 13:33:01.000000 dagster-shell-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      649 2022-08-26 13:45:42.368535 dagster-shell-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      125 2022-08-26 13:33:01.000000 dagster-shell-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:42.368535 dagster-shell-1.0.5/dagster_shell/
+-rw-r--r--   0 root         (0) root         (0)      499 2022-08-26 13:33:01.000000 dagster-shell-1.0.5/dagster_shell/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-shell-1.0.5/dagster_shell/py.typed
+-rw-r--r--   0 root         (0) root         (0)     6728 2022-08-26 13:33:01.000000 dagster-shell-1.0.5/dagster_shell/solids.py
+-rw-r--r--   0 root         (0) root         (0)     7168 2022-08-26 13:33:01.000000 dagster-shell-1.0.5/dagster_shell/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-shell-1.0.5/dagster_shell/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:42.368535 dagster-shell-1.0.5/dagster_shell.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      649 2022-08-26 13:45:42.000000 dagster-shell-1.0.5/dagster_shell.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      389 2022-08-26 13:45:42.000000 dagster-shell-1.0.5/dagster_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:42.000000 dagster-shell-1.0.5/dagster_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:42.000000 dagster-shell-1.0.5/dagster_shell.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       30 2022-08-26 13:45:42.000000 dagster-shell-1.0.5/dagster_shell.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2022-08-26 13:45:42.000000 dagster-shell-1.0.5/dagster_shell.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      160 2022-08-26 13:45:42.372535 dagster-shell-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1318 2022-08-26 13:33:01.000000 dagster-shell-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dagster-shell-0.9.9rc1/LICENSE` & `dagster-shell-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-shell-0.9.9rc1/PKG-INFO` & `dagster-shell-1.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-shell
-Version: 0.9.9rc1
-Summary: Package for Dagster shell solids.
+Version: 1.0.5
+Summary: Package for Dagster shell ops.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-shell
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Description: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Provides-Extra: test
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-shell-0.9.9rc1/dagster_shell/solids.py` & `dagster-shell-1.0.5/dagster_shell/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,210 +1,171 @@
+#
+# NOTE: This file is based on the bash operator from Apache Airflow, which can be found here:
+# https://github.com/apache/airflow/blob/master/airflow/operators/bash.py
+#
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
 import os
+import signal
+from subprocess import PIPE, STDOUT, Popen
 
-from dagster import (
-    Enum,
-    EnumValue,
-    Failure,
-    Field,
-    InputDefinition,
-    Noneable,
-    Nothing,
-    OutputDefinition,
-    Permissive,
-    check,
-    solid,
-)
-
-from .utils import execute, execute_script_file
-
-
-def shell_solid_config():
-    return {
-        "env": Field(
-            Noneable(Permissive()),
-            default_value=os.environ.copy(),
-            is_required=False,
-            description="An optional dict of environment variables to pass to the subprocess. "
-            "Defaults to using os.environ.copy().",
-        ),
-        "output_logging": Field(
-            Enum(
-                name="OutputType",
-                enum_values=[
-                    EnumValue("STREAM", description="Stream script stdout/stderr."),
-                    EnumValue(
-                        "BUFFER",
-                        description="Buffer shell script stdout/stderr, then log upon completion.",
-                    ),
-                    EnumValue("NONE", description="No logging"),
-                ],
-            ),
-            is_required=False,
-            default_value="BUFFER",
-        ),
-        "cwd": Field(
-            Noneable(str),
-            default_value=None,
-            is_required=False,
-            description="Working directory in which to execute shell script",
-        ),
-    }
-
-
-@solid(
-    name="shell_solid",
-    description=(
-        "This solid executes a shell command it receives as input.\n\n"
-        "This solid is suitable for uses where the command to execute is generated dynamically by "
-        "upstream solids. If you know the command to execute at pipeline construction time, "
-        "consider `shell_command_solid` instead."
-    ),
-    input_defs=[InputDefinition("shell_command", str)],
-    output_defs=[OutputDefinition(str, "result")],
-    config_schema=shell_solid_config(),
-)
-def shell_solid(context, shell_command):
-    """This solid executes a shell command it receives as input.
-
-    This solid is suitable for uses where the command to execute is generated dynamically by
-    upstream solids. If you know the command to execute at pipeline construction time, consider
-    `shell_command_solid` instead.
-    """
-    output, return_code = execute(
-        shell_command=shell_command, log=context.log, **context.solid_config
-    )
-
-    if return_code:
-        raise Failure(
-            description="Shell command execution failed with output: {output}".format(output=output)
-        )
+import dagster._check as check
+from dagster._utils import safe_tempfile_path
 
-    return output
+OUTPUT_LOGGING_OPTIONS = ["STREAM", "BUFFER", "NONE"]
 
 
-def create_shell_command_solid(
-    shell_command, name, description=None, required_resource_keys=None, tags=None,
-):
-    """This function is a factory that constructs solids to execute a shell command.
+def execute_script_file(shell_script_path, output_logging, log, cwd=None, env=None):
+    """Execute a shell script file specified by the argument ``shell_script_path``. The script will be
+    invoked via ``subprocess.Popen(['bash', shell_script_path], ...)``.
 
-    Note that you can only use `shell_command_solid` if you know the command you'd like to execute
-    at pipeline construction time. If you'd like to construct shell commands dynamically during
-    pipeline execution and pass them between solids, you should use `shell_solid` instead.
+    In the Popen invocation, ``stdout=PIPE, stderr=STDOUT`` is used, and the combined stdout/stderr
+    output is retrieved.
 
     Examples:
 
-    .. literalinclude:: ../../../../../python_modules/libraries/dagster-shell/dagster_shell_tests/example_shell_command_solid.py
-       :language: python
-
+        .. literalinclude:: ../../../../../../python_modules/libraries/dagster-shell/dagster_shell_tests/example_shell_script_utility.py
+           :language: python
 
     Args:
-        shell_command (str): The shell command that the constructed solid will execute.
-        name (str): The name of the constructed solid.
-        description (Optional[str]): Human-readable description of this solid.
-        required_resource_keys (Optional[Set[str]]): Set of resource handles required by this solid.
-            Setting this ensures that resource spin up for the required resources will occur before
-            the shell command is executed.
-        tags (Optional[Dict[str, Any]]): Arbitrary metadata for the solid. Frameworks may
-            expect and require certain metadata to be attached to a solid. Users should generally
-            not set metadata directly. Values that are not strings will be json encoded and must meet
-            the criteria that `json.loads(json.dumps(value)) == value`.
+        shell_script_path (str): The shell script to execute.
+        output_logging (str): The logging mode to use. Supports STREAM, BUFFER, and NONE.
+        log (Union[logging.Logger, DagsterLogManager]): Any logger which responds to .info()
+        cwd (str, optional): Working directory for the shell command to use. Defaults to the
+            temporary path where we store the shell command in a script file.
+        env (Dict[str, str], optional): Environment dictionary to pass to ``subprocess.Popen``.
+            Unused by default.
 
     Raises:
-        Failure: Raised when the shell command returns a non-zero exit code.
+        Exception: When an invalid output_logging is selected. Unreachable from op-based
+            invocation since the config system will check output_logging against the config
+            enum.
 
     Returns:
-        SolidDefinition: Returns the constructed solid definition.
+        Tuple[str, int]: A tuple where the first element is the combined stdout/stderr output of running the shell
+        command and the second element is the return code.
     """
-    check.str_param(shell_command, "shell_command")
-    name = check.str_param(name, "name")
-
-    @solid(
-        name=name,
-        description=description,
-        input_defs=[InputDefinition("start", Nothing)],
-        output_defs=[OutputDefinition(str, "result")],
-        config_schema=shell_solid_config(),
-        required_resource_keys=required_resource_keys,
-        tags=tags,
-    )
-    def _shell_solid(context):
-        output, return_code = execute(
-            shell_command=shell_command, log=context.log, **context.solid_config
+    check.str_param(shell_script_path, "shell_script_path")
+    check.str_param(output_logging, "output_logging")
+    check.opt_str_param(cwd, "cwd", default=os.path.dirname(shell_script_path))
+    env = check.opt_dict_param(env, "env")
+
+    if output_logging not in OUTPUT_LOGGING_OPTIONS:
+        raise Exception("Unrecognized output_logging %s" % output_logging)
+
+    def pre_exec():
+        # Restore default signal disposition and invoke setsid
+        for sig in ("SIGPIPE", "SIGXFZ", "SIGXFSZ"):
+            if hasattr(signal, sig):
+                signal.signal(getattr(signal, sig), signal.SIG_DFL)
+        os.setsid()
+
+    with open(shell_script_path, "rb") as f:
+        shell_command = f.read().decode("utf-8")
+
+    log.info(f"Running command:\n{shell_command}")
+
+    # pylint: disable=subprocess-popen-preexec-fn
+    sub_process = None
+    try:
+        stdout_pipe = PIPE
+        stderr_pipe = STDOUT
+        if output_logging == "NONE":
+            stdout_pipe = stderr_pipe = None
+
+        sub_process = Popen(
+            ["bash", shell_script_path],
+            stdout=stdout_pipe,
+            stderr=stderr_pipe,
+            cwd=cwd,
+            env=env,
+            preexec_fn=pre_exec,
+            encoding="UTF-8",
         )
 
-        if return_code:
-            raise Failure(
-                description="Shell command execution failed with output: {output}".format(
-                    output=output
-                )
-            )
-
-        return output
-
-    return _shell_solid
+        log.info(f"Command pid: {sub_process.pid}")
 
+        output = ""
+        if output_logging == "STREAM":
+            # Stream back logs as they are emitted
+            lines = []
+            for line in sub_process.stdout:
+                log.info(line.rstrip())
+                lines.append(line)
+            output = "".join(lines)
+        elif output_logging == "BUFFER":
+            # Collect and buffer all logs, then emit
+            output, _ = sub_process.communicate()
+            log.info(output)
+
+        sub_process.wait()
+        log.info("Command exited with return code {retcode}".format(retcode=sub_process.returncode))
+
+        return output, sub_process.returncode
+    finally:
+        # Always terminate subprocess, including in cases where the pipeline run is terminated
+        if sub_process:
+            sub_process.terminate()
 
-def create_shell_script_solid(
-    shell_script_path, name="create_shell_script_solid", input_defs=None, **kwargs
-):
-    """This function is a factory which constructs a solid that will execute a shell command read
-    from a script file.
 
-    Any kwargs passed to this function will be passed along to the underlying :func:`@solid
-    <dagster.solid>` decorator. However, note that overriding ``config`` or ``output_defs`` is not
-    supported.
+def execute(shell_command, output_logging, log, cwd=None, env=None):
+    """
+    This function is a utility for executing shell commands from within a Dagster op (or from Python in general).
+    It can be used to execute shell commands on either op input data, or any data generated within a generic python op.
 
-    You might consider using :func:`@composite_solid <dagster.composite_solid>` to wrap this solid
-    in the cases where you'd like to configure the shell solid with different config fields.
+    Internally, it executes a shell script specified by the argument ``shell_command``. The script will be written
+    to a temporary file first and invoked via ``subprocess.Popen(['bash', shell_script_path], ...)``.
 
+    In the Popen invocation, ``stdout=PIPE, stderr=STDOUT`` is used, and the combined stdout/stderr
+    output is retrieved.
 
     Examples:
 
-    .. literalinclude:: ../../../../../python_modules/libraries/dagster-shell/dagster_shell_tests/example_shell_script_solid.py
-       :language: python
-
+        .. literalinclude:: ../../../../../../python_modules/libraries/dagster-shell/dagster_shell_tests/example_shell_command_utility.py
+           :language: python
 
     Args:
-        shell_script_path (str): The script file to execute.
-        name (str, optional): The name of this solid. Defaults to "create_shell_script_solid".
-        input_defs (List[InputDefinition], optional): input definitions for the solid. Defaults to
-            a single Nothing input.
-
-    Raises:
-        Failure: Raised when the shell command returns a non-zero exit code.
+        shell_command (str): The shell command to execute
+        output_logging (str): The logging mode to use. Supports STREAM, BUFFER, and NONE.
+        log (Union[logging.Logger, DagsterLogManager]): Any logger which responds to .info()
+        cwd (str, optional): Working directory for the shell command to use. Defaults to the
+            temporary path where we store the shell command in a script file.
+        env (Dict[str, str], optional): Environment dictionary to pass to ``subprocess.Popen``.
+            Unused by default.
 
     Returns:
-        SolidDefinition: Returns the constructed solid definition.
+        Tuple[str, int]: A tuple where the first element is the combined stdout/stderr output of running the shell
+        command and the second element is the return code.
     """
-    check.str_param(shell_script_path, "shell_script_path")
-    name = check.str_param(name, "name")
-    check.opt_list_param(input_defs, "input_defs", of_type=InputDefinition)
-
-    if "output_defs" in kwargs:
-        raise TypeError("Overriding output_defs for shell solid is not supported.")
-
-    if "config" in kwargs:
-        raise TypeError("Overriding config for shell solid is not supported.")
-
-    @solid(
-        name=name,
-        description=kwargs.pop("description", "A solid to invoke a shell command."),
-        input_defs=input_defs or [InputDefinition("start", Nothing)],
-        output_defs=[OutputDefinition(str, "result")],
-        config_schema=shell_solid_config(),
-        **kwargs
-    )
-    def _shell_script_solid(context):
-        output, return_code = execute_script_file(
-            shell_script_path=shell_script_path, log=context.log, **context.solid_config
-        )
+    check.str_param(shell_command, "shell_command")
+    # other args checked in execute_file
 
-        if return_code:
-            raise Failure(
-                description="Shell command execution failed with output: {output}".format(
-                    output=output
-                )
+    with safe_tempfile_path() as tmp_file_path:
+        tmp_path = os.path.dirname(tmp_file_path)
+        log.info("Using temporary directory: %s" % tmp_path)
+
+        with open(tmp_file_path, "wb") as tmp_file:
+            tmp_file.write(shell_command.encode("utf-8"))
+            tmp_file.flush()
+            script_location = os.path.abspath(tmp_file.name)
+            log.info("Temporary script location: {location}".format(location=script_location))
+            return execute_script_file(
+                shell_script_path=tmp_file.name,
+                output_logging=output_logging,
+                log=log,
+                cwd=(cwd or tmp_path),
+                env=env,
             )
-
-        return output
-
-    return _shell_script_solid
```

### Comparing `dagster-shell-0.9.9rc1/dagster_shell.egg-info/PKG-INFO` & `dagster-shell-1.0.5/dagster_shell.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: dagster-shell
-Version: 0.9.9rc1
-Summary: Package for Dagster shell solids.
+Version: 1.0.5
+Summary: Package for Dagster shell ops.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-shell
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
-Description: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Provides-Extra: test
+License-File: LICENSE
+
+UNKNOWN
+
```

