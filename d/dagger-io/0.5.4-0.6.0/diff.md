# Comparing `tmp/dagger_io-0.5.4.tar.gz` & `tmp/dagger_io-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagger_io-0.5.4.tar", max compression
+gzip compressed data, was "dagger_io-0.6.0.tar", max compression
```

## Comparing `dagger_io-0.5.4.tar` & `dagger_io-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    10758 2023-05-18 17:53:16.702461 dagger_io-0.5.4/LICENSE
--rw-r--r--   0        0        0     4727 2023-05-18 17:53:16.702461 dagger_io-0.5.4/README.md
--rw-r--r--   0        0        0     6344 2023-05-18 17:54:33.893909 dagger_io-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      313 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/__init__.py
--rw-r--r--   0        0        0       71 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/__main__.py
--rw-r--r--   0        0        0       69 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/api/.gitattributes
--rw-r--r--   0        0        0        0 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/api/__init__.py
--rw-r--r--   0        0        0    11866 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/api/base.py
--rw-r--r--   0        0        0    88720 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/api/gen.py
--rw-r--r--   0        0        0    88384 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/api/gen_sync.py
--rw-r--r--   0        0        0     1683 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/cli.py
--rw-r--r--   0        0        0    19680 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/codegen.py
--rw-r--r--   0        0        0     1302 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/config.py
--rw-r--r--   0        0        0     1585 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/connection.py
--rw-r--r--   0        0        0      964 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/context.py
--rw-r--r--   0        0        0       37 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/engine/.gitattributes
--rw-r--r--   0        0        0       35 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/engine/__init__.py
--rw-r--r--   0        0        0       64 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/engine/_version.py
--rw-r--r--   0        0        0     4202 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/engine/cli.py
--rw-r--r--   0        0        0     2068 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/engine/conn.py
--rw-r--r--   0        0        0     8163 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/engine/download.py
--rw-r--r--   0        0        0     3042 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/exceptions.py
--rw-r--r--   0        0        0      677 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/log.py
--rw-r--r--   0        0        0        0 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/py.typed
--rw-r--r--   0        0        0     2320 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/server/__init__.py
--rw-r--r--   0        0        0       78 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/server/__main__.py
--rw-r--r--   0        0        0      911 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/server/cli.py
--rw-r--r--   0        0        0      865 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/server/converter.py
--rw-r--r--   0        0        0     3892 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/session.py
--rw-r--r--   0        0        0        0 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/transport/__init__.py
--rw-r--r--   0        0        0     5820 2023-05-18 17:53:16.702461 dagger_io-0.5.4/src/dagger/transport/httpx.py
--rw-r--r--   0        0        0     5951 1970-01-01 00:00:00.000000 dagger_io-0.5.4/setup.py
--rw-r--r--   0        0        0     6524 1970-01-01 00:00:00.000000 dagger_io-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0    10758 2023-05-25 16:59:18.260135 dagger_io-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4727 2023-05-25 16:59:18.260135 dagger_io-0.6.0/README.md
+-rw-r--r--   0        0        0     6344 2023-05-25 17:00:26.780909 dagger_io-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      360 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/__init__.py
+-rw-r--r--   0        0        0       71 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/__main__.py
+-rw-r--r--   0        0        0       69 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/api/.gitattributes
+-rw-r--r--   0        0        0        0 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/api/__init__.py
+-rw-r--r--   0        0        0    11873 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/api/base.py
+-rw-r--r--   0        0        0    89082 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/api/gen.py
+-rw-r--r--   0        0        0    88681 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/api/gen_sync.py
+-rw-r--r--   0        0        0     1683 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/cli.py
+-rw-r--r--   0        0        0    20021 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/codegen.py
+-rw-r--r--   0        0        0     1302 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/config.py
+-rw-r--r--   0        0        0     1884 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/connection.py
+-rw-r--r--   0        0        0      964 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/context.py
+-rw-r--r--   0        0        0       37 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/engine/.gitattributes
+-rw-r--r--   0        0        0       35 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/engine/__init__.py
+-rw-r--r--   0        0        0       64 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/engine/_version.py
+-rw-r--r--   0        0        0     4202 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/engine/cli.py
+-rw-r--r--   0        0        0     2068 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/engine/conn.py
+-rw-r--r--   0        0        0     8163 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/engine/download.py
+-rw-r--r--   0        0        0     4262 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/exceptions.py
+-rw-r--r--   0        0        0      677 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/log.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/py.typed
+-rw-r--r--   0        0        0     2320 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/server/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/server/__main__.py
+-rw-r--r--   0        0        0      911 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/server/cli.py
+-rw-r--r--   0        0        0      865 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/server/converter.py
+-rw-r--r--   0        0        0     3892 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/session.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/transport/__init__.py
+-rw-r--r--   0        0        0     5820 2023-05-25 16:59:18.260135 dagger_io-0.6.0/src/dagger/transport/httpx.py
+-rw-r--r--   0        0        0     5951 1970-01-01 00:00:00.000000 dagger_io-0.6.0/setup.py
+-rw-r--r--   0        0        0     6524 1970-01-01 00:00:00.000000 dagger_io-0.6.0/PKG-INFO
```

### Comparing `dagger_io-0.5.4/LICENSE` & `dagger_io-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.4/README.md` & `dagger_io-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.4/pyproject.toml` & `dagger_io-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dagger-io"
-version = "0.5.4"
+version = "0.6.0"
 description = "A client package for running Dagger pipelines in Python."
 license = "Apache-2.0"
 authors = ["Dagger <hello@dagger.io>"]
 readme = "README.md"
 homepage = "https://dagger.io"
 documentation = "https://docs.dagger.io/sdk/python"
 repository = "https://github.com/dagger/dagger/tree/main/sdk/python"
```

### Comparing `dagger_io-0.5.4/src/dagger/api/base.py` & `dagger_io-0.6.0/src/dagger/api/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
         return selectable
 
     def query(self) -> graphql.DocumentNode:
         return dsl_gql(DSLQuery(self.build()))
 
     @overload
-    async def execute(self, return_type: None) -> None:
+    async def execute(self, return_type: None = None) -> None:
         ...
 
     @overload
     async def execute(self, return_type: type[T]) -> T:
         ...
 
     async def execute(self, return_type: type[T] | None = None) -> T | None:
```

### Comparing `dagger_io-0.5.4/src/dagger/api/gen.py` & `dagger_io-0.6.0/src/dagger/api/gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -821,14 +821,17 @@
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("sync", _args)
         await _ctx.execute()
         return self
 
+    def __await__(self):
+        return self.sync().__await__()
+
     @typecheck
     async def user(self) -> Optional[str]:
         """Retrieves the user to be set for all commands.
 
         Returns
         -------
         Optional[str]
@@ -917,27 +920,37 @@
         _args = [
             Arg("args", args),
         ]
         _ctx = self._select("withEntrypoint", _args)
         return Container(_ctx)
 
     @typecheck
-    def with_env_variable(self, name: str, value: str) -> "Container":
+    def with_env_variable(
+        self,
+        name: str,
+        value: str,
+        expand: Optional[bool] = None,
+    ) -> "Container":
         """Retrieves this container plus the given environment variable.
 
         Parameters
         ----------
         name:
             The name of the environment variable (e.g., "HOST").
         value:
             The value of the environment variable. (e.g., "localhost").
+        expand:
+            Replace ${VAR} or $VAR in the value according to the current
+            environment
+            variables defined in the container (e.g., "/opt/bin:$PATH").
         """
         _args = [
             Arg("name", name),
             Arg("value", value),
+            Arg("expand", expand, None),
         ]
         _ctx = self._select("withEnvVariable", _args)
         return Container(_ctx)
 
     @typecheck
     def with_exec(
         self,
```

### Comparing `dagger_io-0.5.4/src/dagger/api/gen_sync.py` & `dagger_io-0.6.0/src/dagger/api/gen_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -917,27 +917,37 @@
         _args = [
             Arg("args", args),
         ]
         _ctx = self._select("withEntrypoint", _args)
         return Container(_ctx)
 
     @typecheck
-    def with_env_variable(self, name: str, value: str) -> "Container":
+    def with_env_variable(
+        self,
+        name: str,
+        value: str,
+        expand: Optional[bool] = None,
+    ) -> "Container":
         """Retrieves this container plus the given environment variable.
 
         Parameters
         ----------
         name:
             The name of the environment variable (e.g., "HOST").
         value:
             The value of the environment variable. (e.g., "localhost").
+        expand:
+            Replace ${VAR} or $VAR in the value according to the current
+            environment
+            variables defined in the container (e.g., "/opt/bin:$PATH").
         """
         _args = [
             Arg("name", name),
             Arg("value", value),
+            Arg("expand", expand, None),
         ]
         _ctx = self._select("withEnvVariable", _args)
         return Container(_ctx)
 
     @typecheck
     def with_exec(
         self,
```

### Comparing `dagger_io-0.5.4/src/dagger/cli.py` & `dagger_io-0.6.0/src/dagger/cli.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.4/src/dagger/codegen.py` & `dagger_io-0.6.0/src/dagger/codegen.py`

 * *Files 2% similar despite different names*

```diff
@@ -425,14 +425,23 @@
         yield from (
             "",
             "@typecheck",
             self.func_signature(),
             indent(self.func_body()),
         )
 
+        # convenience to await any object that has a sync method
+        # without having to call it explicitly
+        if not self.ctx.sync and self.is_leaf and self.name == "sync":
+            yield from (
+                "",
+                "def __await__(self):",
+                indent("return self.sync().__await__()"),
+            )
+
     def func_signature(self) -> str:
         params = ", ".join(chain(("self",), (a.as_param() for a in self.args)))
         # arbitrary heuristic to force trailing comma in long signatures
         if len(params) > 40:  # noqa: PLR2004
             params = f"{params},"
         prefix = "" if self.ctx.sync or not self.is_leaf else "async "
         sig = f"{prefix}def {self.name}({params}) -> {self.type}:"
```

### Comparing `dagger_io-0.5.4/src/dagger/config.py` & `dagger_io-0.6.0/src/dagger/config.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.4/src/dagger/connection.py` & `dagger_io-0.6.0/src/dagger/connection.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import warnings
+
 from dagger import Client, Config, SyncClient
 
 from .context import ResourceManager, SyncResourceManager
 from .engine import Engine
 from .session import Session
 
 
@@ -41,11 +43,18 @@
     async def __aenter__(self) -> Client:
         async with self.get_stack() as stack:
             conn = await stack.enter_async_context(Engine(self.cfg))
             session = await stack.enter_async_context(Session(conn, self.cfg))
         return Client.from_session(session)
 
     def __enter__(self) -> SyncClient:
+        warnings.warn(
+            "The synchronous API is deprecated and will be removed in a future"
+            " release. See https://github.com/dagger/dagger/issues/5192"
+            " for more information.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
         with self.get_sync_stack() as stack:
             conn = stack.enter_context(Engine(self.cfg))
             session = stack.enter_context(Session(conn, self.cfg))
         return SyncClient.from_session(session)
```

### Comparing `dagger_io-0.5.4/src/dagger/context.py` & `dagger_io-0.6.0/src/dagger/context.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.4/src/dagger/engine/cli.py` & `dagger_io-0.6.0/src/dagger/engine/cli.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.4/src/dagger/engine/conn.py` & `dagger_io-0.6.0/src/dagger/engine/conn.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.4/src/dagger/engine/download.py` & `dagger_io-0.6.0/src/dagger/engine/download.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.4/src/dagger/log.py` & `dagger_io-0.6.0/src/dagger/log.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.4/src/dagger/server/__init__.py` & `dagger_io-0.6.0/src/dagger/server/__init__.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.4/src/dagger/server/cli.py` & `dagger_io-0.6.0/src/dagger/server/cli.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.4/src/dagger/server/converter.py` & `dagger_io-0.6.0/src/dagger/server/converter.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.4/src/dagger/session.py` & `dagger_io-0.6.0/src/dagger/session.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.4/src/dagger/transport/httpx.py` & `dagger_io-0.6.0/src/dagger/transport/httpx.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.4/setup.py` & `dagger_io-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  'typing_extensions>=4.4.0']
 
 extras_require = \
 {'server': ['strawberry-graphql>=0.133.5']}
 
 setup_kwargs = {
     'name': 'dagger-io',
-    'version': '0.5.4',
+    'version': '0.6.0',
     'description': 'A client package for running Dagger pipelines in Python.',
     'long_description': '# Dagger Python SDK\n\n[![PyPI Version](https://img.shields.io/pypi/v/dagger-io)](https://pypi.org/project/dagger-io/) \n[![Conda Version](https://img.shields.io/conda/vn/conda-forge/dagger-io.svg)](https://anaconda.org/conda-forge/dagger-io)\n[![Supported Python Versions](https://img.shields.io/pypi/pyversions/dagger-io.svg)](https://pypi.org/project/dagger-io/)\n[![License](https://img.shields.io/pypi/l/dagger-io.svg)](https://pypi.python.org/pypi/dagger-io)\n[![Code style](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)\n\nA client package for running [Dagger](https://dagger.io/) pipelines.\n\n## What is the Dagger Python SDK?\n\nThe Dagger Python SDK contains everything you need to develop CI/CD pipelines in Python, and run them on any OCI-compatible container runtime.\n\n## Requirements\n\n- Python 3.10 or later\n- [Docker](https://docs.docker.com/engine/install/), or another OCI-compatible container runtime\n\nA compatible version of the  [Dagger CLI](https://docs.dagger.io/cli) is automatically downloaded and run by the SDK for you, although it’s possible to manage it manually.\n\n## Installation\n\nFrom [PyPI](https://pypi.org/project/dagger-io/), using `pip`:\n\n```shell\npip install dagger-io\n```\n\nYou can also install via [Conda](https://anaconda.org/conda-forge/dagger-io), from the [conda-forge](https://conda-forge.org/docs/user/introduction.html#how-can-i-install-packages-from-conda-forge) channel:\n\n```shell\nconda install dagger-io\n```\n\n## Example\n\nCreate a `main.py` file:\n\n```python\nimport sys\n\nimport anyio\nimport dagger\n\n\nasync def main(args: list[str]):\n    async with dagger.Connection() as client:\n        # build container with cowsay entrypoint\n        ctr = (\n            client.container()\n            .from_("python:alpine")\n            .with_exec(["pip", "install", "cowsay"])\n            .with_entrypoint(["cowsay"])\n        )\n\n        # run cowsay with requested message\n        result = await ctr.with_exec(args).stdout()\n\n    print(result)\n\n\nanyio.run(main, sys.argv[1:])\n```\n\nRun with:\n\n```console\n$ python main.py "Simple is better than complex"\n  _____________________________\n| Simple is better than complex |\n  =============================\n                             \\\n                              \\\n                                ^__^\n                                (oo)\\_______\n                                (__)\\       )\\/\\\n                                    ||----w |\n                                    ||     ||\n```\n\n> **Note**\n> It may take a while for it to finish, especially on first run with cold cache.\n\nIf you need to debug, you can stream the logs from the engine with the `log_output`  config:\n\n```python\nconfig = dagger.Config(log_output=sys.stderr)\nasync with dagger.Connection(config) as client:\n    ...\n```\n\n## Learn more\n\n- [Documentation](https://docs.dagger.io/sdk/python)\n- [API Reference](https://dagger-io.readthedocs.org)\n- [Source code](https://github.com/dagger/dagger/tree/main/sdk/python)\n\n## Development\n\nThis library is maintained with [Poetry](https://python-poetry.org/docs/).\n\nIf you already have a [Python 3.10 or later](https://docs.python.org/3/using/index.html) interpreter in your `$PATH`, you can let [Poetry manage](https://python-poetry.org/docs/basic-usage/#using-your-virtual-environment) the [virtual environment](https://packaging.python.org/en/latest/tutorials/installing-packages/#creating-virtual-environments) automatically. Otherwise you need to activate it first, before installing dependencies:\n\n```shell\npoetry install\n```\n\nThe following commands are available:\n- `poe test`: Run tests.\n- `poe fmt`: Re-format code following common styling conventions.\n- `poe lint`: Check for linting violations.\n- `poe generate`: Regenerate API client after changes to the codegen.\n- `poe docs`: Build reference docs locally.\n\n### Engine changes\n\nTesting and regenerating the client may fail if there’s changes in the engine code that haven’t been released yet. \n\nThe simplest way to run those commands locally with the most updated engine version is to build it using [Dagger’s CI pipelines](https://github.com/dagger/dagger/blob/main/internal/mage/sdk/python.go) :\n\n```shell\n../../hack/make sdk:python:test\n../../hack/make sdk:python:generate\n```\n\nYou can also build the CLI and use it directly within the Python SDK:\n\n```shell\n../../hack/dev poe test\n```\n\nOr build it separately and tell the SDK to use it directly (or any other CLI binary):\n\n```shell\n../../hack/make\n_EXPERIMENTAL_DAGGER_CLI_BIN=../../bin/dagger poe test\n```\n\n',
     'author': 'Dagger',
     'author_email': 'hello@dagger.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://dagger.io',
```

### Comparing `dagger_io-0.5.4/PKG-INFO` & `dagger_io-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagger-io
-Version: 0.5.4
+Version: 0.6.0
 Summary: A client package for running Dagger pipelines in Python.
 Home-page: https://dagger.io
 License: Apache-2.0
 Author: Dagger
 Author-email: hello@dagger.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

