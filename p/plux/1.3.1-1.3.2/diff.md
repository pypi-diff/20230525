# Comparing `tmp/plux-1.3.1.tar.gz` & `tmp/plux-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plux-1.3.1.tar", last modified: Wed Mar  2 10:47:40 2022, max compression
+gzip compressed data, was "plux-1.3.2.tar", last modified: Thu May 25 11:28:13 2023, max compression
```

## Comparing `plux-1.3.1.tar` & `plux-1.3.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2022-03-02 10:47:40.532651 plux-1.3.1/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10117 2022-03-02 10:47:40.532651 plux-1.3.1/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7602 2022-03-01 23:48:07.000000 plux-1.3.1/README.md
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2022-03-02 10:47:40.532651 plux-1.3.1/plugin/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      525 2022-03-02 01:02:34.000000 plux-1.3.1/plugin/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7213 2022-03-01 23:48:07.000000 plux-1.3.1/plugin/core.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2802 2022-03-01 23:48:07.000000 plux-1.3.1/plugin/discovery.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1778 2022-03-01 23:48:07.000000 plux-1.3.1/plugin/entrypoint.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    12563 2022-03-01 23:48:07.000000 plux-1.3.1/plugin/manager.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6904 2022-03-02 02:56:46.000000 plux-1.3.1/plugin/setuptools.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2022-03-02 10:47:40.532651 plux-1.3.1/plux.egg-info/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10117 2022-03-02 10:47:40.000000 plux-1.3.1/plux.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      354 2022-03-02 10:47:40.000000 plux-1.3.1/plux.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2022-03-02 10:47:40.000000 plux-1.3.1/plux.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      130 2022-03-02 10:47:40.000000 plux-1.3.1/plux.egg-info/entry_points.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2022-03-02 10:47:34.000000 plux-1.3.1/plux.egg-info/not-zip-safe
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       63 2022-03-02 10:47:40.000000 plux-1.3.1/plux.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        7 2022-03-02 10:47:40.000000 plux-1.3.1/plux.egg-info/top_level.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      197 2022-03-01 23:48:07.000000 plux-1.3.1/pyproject.toml
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1296 2022-03-02 10:47:40.532651 plux-1.3.1/setup.cfg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       60 2022-03-01 23:48:07.000000 plux-1.3.1/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-25 11:28:13.017880 plux-1.3.2/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    11358 2023-02-17 21:14:38.000000 plux-1.3.2/LICENSE
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     9287 2023-05-25 11:28:13.017880 plux-1.3.2/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8421 2023-05-15 20:31:40.000000 plux-1.3.2/README.md
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-25 11:28:13.017880 plux-1.3.2/plugin/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      525 2023-05-25 11:27:35.000000 plux-1.3.2/plugin/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     7213 2023-02-17 21:14:38.000000 plux-1.3.2/plugin/core.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2802 2023-02-17 21:14:38.000000 plux-1.3.2/plugin/discovery.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1778 2023-02-17 21:14:38.000000 plux-1.3.2/plugin/entrypoint.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    12564 2023-05-25 11:26:56.000000 plux-1.3.2/plugin/manager.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     6904 2023-02-17 21:14:38.000000 plux-1.3.2/plugin/setuptools.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-25 11:28:13.017880 plux-1.3.2/plux.egg-info/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     9287 2023-05-25 11:28:13.000000 plux-1.3.2/plux.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      362 2023-05-25 11:28:13.000000 plux-1.3.2/plux.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-05-25 11:28:13.000000 plux-1.3.2/plux.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      129 2023-05-25 11:28:13.000000 plux-1.3.2/plux.egg-info/entry_points.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-05-25 11:28:13.000000 plux-1.3.2/plux.egg-info/not-zip-safe
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       63 2023-05-25 11:28:13.000000 plux-1.3.2/plux.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        7 2023-05-25 11:28:13.000000 plux-1.3.2/plux.egg-info/top_level.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      197 2023-02-17 21:14:38.000000 plux-1.3.2/pyproject.toml
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1296 2023-05-25 11:28:13.017880 plux-1.3.2/setup.cfg
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       60 2023-02-17 21:14:38.000000 plux-1.3.2/setup.py
```

### Comparing `plux-1.3.1/PKG-INFO` & `plux-1.3.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,227 +1,238 @@
 Metadata-Version: 2.1
 Name: plux
-Version: 1.3.1
+Version: 1.3.2
 Summary: A dynamic code loading framework for building pluggable Python distributions
 Home-page: https://github.com/localstack/plux
 Author: Thomas Rausch
 Author-email: thomas@localstack.cloud
 License: Apache License 2.0
-Description: Plux
-        ====
-        
-        <p>
-          <a href="https://github.com/localstack/plux/actions/workflows/build.yml"><img alt="CI badge" src="https://github.com/localstack/plux/actions/workflows/build.yml/badge.svg"></img></a>
-          <a href="https://pypi.org/project/plux/"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/plux?color=blue"></a>
-          <a href="https://img.shields.io/pypi/l/plux.svg"><img alt="PyPI License" src="https://img.shields.io/pypi/l/plux.svg"></a>
-          <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-        </p>
-        
-        plux is the dynamic code loading framework used in [LocalStack](https://github.com/localstack/localstack).
-        
-        
-        Overview
-        --------
-        
-        Plux builds a higher-level plugin mechanism around [Python's entry point mechanism](https://packaging.python.org/specifications/entry-points/).
-        It provides tools to load plugins from entry points at run time, and to discover entry points from plugins at build time (so you don't have to declare entry points statically in your `setup.py`).
-        
-        ### Core concepts
-        
-        * `PluginSpec`: describes a `Plugin`. Each plugin has a namespace, a unique name in that namespace, and a `PluginFactory` (something that creates `Plugin` the spec is describing.
-          In the simplest case, that can just be the Plugin's class).
-        * `Plugin`: an object that exposes a `should_load` and `load` method.
-          Note that it does not function as a domain object (it does not hold the plugins lifecycle state, like initialized, loaded, etc..., or other metadata of the Plugin)
-        * `PluginFinder`: finds plugins, either at build time (by scanning the modules using `pkgutil` and `setuptools`) or at run time (reading entrypoints of the distribution using [stevedore](https://docs.openstack.org/stevedore/latest/))
-        * `PluginManager`: manages the run time lifecycle of a Plugin, which has three states:
-          * resolved: the entrypoint pointing to the PluginSpec was imported and the `PluginSpec` instance was created
-          * init: the `PluginFactory` of the `PluginSpec` was successfully invoked
-          * loaded: the `load` method of the `Plugin` was successfully invoked
-        
-        ![architecture](https://raw.githubusercontent.com/localstack/plux/main/docs/plux-architecture.png)
-        
-        ### Loading Plugins
-        
-        At run time, a `PluginManager` uses a `PluginFinder` that in turn uses stevedore to scan the available entrypoints for things that look like a `PluginSpec`.
-        With `PluginManager.load(name: str)` or `PluginManager.load_all()`, plugins within the namespace that are discoverable in entrypoints can be loaded.
-        If an error occurs at any state of the lifecycle, the `PluginManager` informs the `PluginLifecycleListener` about it, but continues operating.
-        
-        ### Discovering entrypoints
-        
-        At build time (e.g., with `python setup.py develop/install/sdist`), a special `PluginFinder` collects anything that can be interpreted as a `PluginSpec`, and creates from it setuptools entrypoints.
-        In the `setup.py` we can use the `plugin.setuptools.load_entry_points` method to collect a dictionary for the `entry_points` value of `setup()`.
-        
-        ```python
-        from plugin.setuptools import load_entry_points
-        
-        setup(
-            entry_points=load_entry_points(exclude=("tests", "tests.*",))
-        )
-        ```
-        
-        Note that `load_entry_points` will try to resolve a cached version of `entry_points.txt` from the `.egg-info` directory,
-        to avoid resolving the entry points when building the package from a source distribution.
-        
-        Examples
-        --------
-        
-        To build something using the plugin framework, you will first want to introduce a Plugin that does something when it is loaded.
-        And then, at runtime, you need a component that uses the `PluginManager` to get those plugins.
-        
-        ### One class per plugin
-        
-        This is the way we went with `LocalstackCliPlugin`. Every plugin class (e.g., `ProCliPlugin`) is essentially a singleton.
-        This is easy, as the classes are discoverable as plugins.
-        Simply create a Plugin class with a name and namespace and it will be discovered by the build time `PluginFinder`.
-        
-        ```python
-        
-        # abstract case (not discovered at build time, missing name)
-        class CliPlugin(Plugin):
-            namespace = "my.plugins.cli"
-        
-            def load(self, cli):
-                self.attach(cli)
-        
-            def attach(self, cli):
-                raise NotImplementedError
-        
-        # discovered at build time (has a namespace, name, and is a Plugin)
-        class MyCliPlugin(CliPlugin):
-            name = "my"
-        
-            def attach(self, cli):
-                # ... attach commands to cli object
-        
-        ```
-        
-        now we need a `PluginManager` (which has a generic type) to load the plugins for us:
-        
-        ```python
-        cli = # ... needs to come from somewhere
-        
-        manager: PluginManager[CliPlugin] = PluginManager("my.plugins.cli", load_args=(cli,))
-        
-        plugins: List[CliPlugin] = manager.load_all()
-        
-        # todo: do stuff with the plugins, if you want/need
-        #  in this example, we simply use the plugin mechanism to run a one-shot function (attach) on a load argument
-        
-        ```
-        
-        ### Re-usable plugins
-        
-        When you have lots of plugins that are structured in a similar way, we may not want to create a separate Plugin class
-        for each plugin. Instead we want to use the same `Plugin` class to do the same thing, but use several instances of it.
-        The `PluginFactory`, and the fact that `PluginSpec` instances defined at module level are discoverable (inpired
-        by [pluggy](https://github.com/pytest-dev/pluggy)), can be used to achieve that.
-        
-        ```python
-        
-        class ServicePlugin(Plugin):
-        
-            def __init__(self, service_name):
-                self.service_name = service_name
-                self.service = None
-        
-            def should_load(self):
-                return self.service_name in config.SERVICES
-        
-            def load(self):
-                module = importlib.import_module("localstack.services.%s" % self.service_name)
-                # suppose we define a convention that each service module has a Service class, like moto's `Backend`
-                self.service = module.Service()
-        
-        def service_plugin_factory(name) -> PluginFactory:
-            def create():
-                return ServicePlugin(name)
-        
-            return create
-        
-        # discoverable
-        s3 = PluginSpec("localstack.plugins.services", "s3", service_plugin_factory("s3"))
-        
-        # discoverable
-        dynamodb = PluginSpec("localstack.plugins.services", "dynamodb", service_plugin_factory("dynamodb"))
-        
-        # ... could be simplified with convenience framework code, but the principle will stay the same
-        
-        ```
-        
-        Then we could use the `PluginManager` to build a Supervisor
-        
-        ```python
-        
-        class Supervisor:
-            manager: PluginManager[ServicePlugin]
-        
-            def start(self, service_name):
-                plugin = manager.load(service_name)
-                service = plugin.service
-                service.start()
-        
-        ```
-        
-        ### Functions as plugins
-        
-        with the `@plugin` decorator, you can expose functions as plugins. They will be wrapped by the framework
-        into `FunctionPlugin` instances, which satisfy both the contract of a Plugin, and that of the function.
-        
-        ```python
-        from plugin import plugin
-        
-        
-        @plugin(namespace="localstack.configurators")
-        def configure_logging(runtime):
-            logging.basicConfig(level=runtime.config.loglevel)
-        
-            
-        @plugin(namespace="localstack.configurators")
-        def configure_somethingelse(runtime):
-            # do other stuff with the runtime object
-            pass
-        ```
-        
-        With a PluginManager via `load_all`, you receive the `FunctionPlugin` instances, that you can call like the functions
-        
-        ```python
-        
-        runtime = LocalstackRuntime()
-        
-        for configurator in PluginManager("localstack.configurators").load_all():
-            configurator(runtime)
-        ```
-        
-        Install
-        -------
-        
-            pip install plux
-        
-        Develop
-        -------
-        
-        Create the virtual environment, install dependencies, and run tests
-        
-            make venv
-            make test
-        
-        Run the code formatter
-        
-            make format
-        
-        Upload the pypi package using twine
-        
-            make upload
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: dev
+License-File: LICENSE
+
+Plux
+====
+
+<p>
+  <a href="https://github.com/localstack/plux/actions/workflows/build.yml"><img alt="CI badge" src="https://github.com/localstack/plux/actions/workflows/build.yml/badge.svg"></img></a>
+  <a href="https://pypi.org/project/plux/"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/plux?color=blue"></a>
+  <a href="https://img.shields.io/pypi/l/plux.svg"><img alt="PyPI License" src="https://img.shields.io/pypi/l/plux.svg"></a>
+  <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+</p>
+
+plux is the dynamic code loading framework used in [LocalStack](https://github.com/localstack/localstack).
+
+
+Overview
+--------
+
+Plux builds a higher-level plugin mechanism around [Python's entry point mechanism](https://packaging.python.org/specifications/entry-points/).
+It provides tools to load plugins from entry points at run time, and to discover entry points from plugins at build time (so you don't have to declare entry points statically in your `setup.py`).
+
+### Core concepts
+
+* `PluginSpec`: describes a `Plugin`. Each plugin has a namespace, a unique name in that namespace, and a `PluginFactory` (something that creates `Plugin` the spec is describing.
+  In the simplest case, that can just be the Plugin's class).
+* `Plugin`: an object that exposes a `should_load` and `load` method.
+  Note that it does not function as a domain object (it does not hold the plugins lifecycle state, like initialized, loaded, etc..., or other metadata of the Plugin)
+* `PluginFinder`: finds plugins, either at build time (by scanning the modules using `pkgutil` and `setuptools`) or at run time (reading entrypoints of the distribution using [stevedore](https://docs.openstack.org/stevedore/latest/))
+* `PluginManager`: manages the run time lifecycle of a Plugin, which has three states:
+  * resolved: the entrypoint pointing to the PluginSpec was imported and the `PluginSpec` instance was created
+  * init: the `PluginFactory` of the `PluginSpec` was successfully invoked
+  * loaded: the `load` method of the `Plugin` was successfully invoked
+
+![architecture](https://raw.githubusercontent.com/localstack/plux/main/docs/plux-architecture.png)
+
+### Loading Plugins
+
+At run time, a `PluginManager` uses a `PluginFinder` that in turn uses stevedore to scan the available entrypoints for things that look like a `PluginSpec`.
+With `PluginManager.load(name: str)` or `PluginManager.load_all()`, plugins within the namespace that are discoverable in entrypoints can be loaded.
+If an error occurs at any state of the lifecycle, the `PluginManager` informs the `PluginLifecycleListener` about it, but continues operating.
+
+### Discovering entrypoints
+
+To build a source distribution and a wheel of your code with your plugins as entrypoints, simply run `python setup.py plugins sdist bdist_wheel`.
+
+How it works:
+For discovering plugins at build time, plux provides a custom setuptools command `plugins`, invoked via `python setup.py plugins`.
+The command uses a special `PluginFinder` that collects from the codebase anything that can be interpreted as a `PluginSpec`, and creates from it a plugin index file `plux.json`, that is placed into the `.egg-info` distribution metadata directory.
+When a setuptools command is used to create the distribution (e.g., `python setup.py sdist/bdist_wheel/...`), plux finds the `plux.json` plugin index and extends automatically the list of entry points (collected into `.egg-info/entry_points.txt`).
+The `plux.json` file becomes a part of the distribution, s.t., the plugins do not have to be discovered every time your distribution is installed elsewhere.
+
+
+
+Examples
+--------
+
+To build something using the plugin framework, you will first want to introduce a Plugin that does something when it is loaded.
+And then, at runtime, you need a component that uses the `PluginManager` to get those plugins.
+
+### One class per plugin
+
+This is the way we went with `LocalstackCliPlugin`. Every plugin class (e.g., `ProCliPlugin`) is essentially a singleton.
+This is easy, as the classes are discoverable as plugins.
+Simply create a Plugin class with a name and namespace and it will be discovered by the build time `PluginFinder`.
+
+```python
+
+# abstract case (not discovered at build time, missing name)
+class CliPlugin(Plugin):
+    namespace = "my.plugins.cli"
+
+    def load(self, cli):
+        self.attach(cli)
+
+    def attach(self, cli):
+        raise NotImplementedError
+
+# discovered at build time (has a namespace, name, and is a Plugin)
+class MyCliPlugin(CliPlugin):
+    name = "my"
+
+    def attach(self, cli):
+        # ... attach commands to cli object
+
+```
+
+now we need a `PluginManager` (which has a generic type) to load the plugins for us:
+
+```python
+cli = # ... needs to come from somewhere
+
+manager: PluginManager[CliPlugin] = PluginManager("my.plugins.cli", load_args=(cli,))
+
+plugins: List[CliPlugin] = manager.load_all()
+
+# todo: do stuff with the plugins, if you want/need
+#  in this example, we simply use the plugin mechanism to run a one-shot function (attach) on a load argument
+
+```
+
+### Re-usable plugins
+
+When you have lots of plugins that are structured in a similar way, we may not want to create a separate Plugin class
+for each plugin. Instead we want to use the same `Plugin` class to do the same thing, but use several instances of it.
+The `PluginFactory`, and the fact that `PluginSpec` instances defined at module level are discoverable (inpired
+by [pluggy](https://github.com/pytest-dev/pluggy)), can be used to achieve that.
+
+```python
+
+class ServicePlugin(Plugin):
+
+    def __init__(self, service_name):
+        self.service_name = service_name
+        self.service = None
+
+    def should_load(self):
+        return self.service_name in config.SERVICES
+
+    def load(self):
+        module = importlib.import_module("localstack.services.%s" % self.service_name)
+        # suppose we define a convention that each service module has a Service class, like moto's `Backend`
+        self.service = module.Service()
+
+def service_plugin_factory(name) -> PluginFactory:
+    def create():
+        return ServicePlugin(name)
+
+    return create
+
+# discoverable
+s3 = PluginSpec("localstack.plugins.services", "s3", service_plugin_factory("s3"))
+
+# discoverable
+dynamodb = PluginSpec("localstack.plugins.services", "dynamodb", service_plugin_factory("dynamodb"))
+
+# ... could be simplified with convenience framework code, but the principle will stay the same
+
+```
+
+Then we could use the `PluginManager` to build a Supervisor
+
+```python
+
+class Supervisor:
+    manager: PluginManager[ServicePlugin]
+
+    def start(self, service_name):
+        plugin = manager.load(service_name)
+        service = plugin.service
+        service.start()
+
+```
+
+### Functions as plugins
+
+with the `@plugin` decorator, you can expose functions as plugins. They will be wrapped by the framework
+into `FunctionPlugin` instances, which satisfy both the contract of a Plugin, and that of the function.
+
+```python
+from plugin import plugin
+
+
+@plugin(namespace="localstack.configurators")
+def configure_logging(runtime):
+    logging.basicConfig(level=runtime.config.loglevel)
+
+    
+@plugin(namespace="localstack.configurators")
+def configure_somethingelse(runtime):
+    # do other stuff with the runtime object
+    pass
+```
+
+With a PluginManager via `load_all`, you receive the `FunctionPlugin` instances, that you can call like the functions
+
+```python
+
+runtime = LocalstackRuntime()
+
+for configurator in PluginManager("localstack.configurators").load_all():
+    configurator(runtime)
+```
+
+Configuring your distribution
+-----------------------------
+
+If you are building a python distribution that exposes plugins discovered by plux, you need to configure your projects build system so other dependencies creates the `entry_points.txt` file when installing your distribution.
+
+For a [`pyproject.toml`](https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/) template this involves adding the `build-system` section:
+
+```toml
+[build-system]
+requires = ['setuptools', 'wheel', 'plux>=1.3.1']
+build-backend = "setuptools.build_meta"
+
+# ...
+```
+
+Install
+-------
+
+    pip install plux
+
+Develop
+-------
+
+Create the virtual environment, install dependencies, and run tests
+
+    make venv
+    make test
+
+Run the code formatter
+
+    make format
+
+Upload the pypi package using twine
+
+    make upload
```

### Comparing `plux-1.3.1/README.md` & `plux-1.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -35,27 +35,23 @@
 
 At run time, a `PluginManager` uses a `PluginFinder` that in turn uses stevedore to scan the available entrypoints for things that look like a `PluginSpec`.
 With `PluginManager.load(name: str)` or `PluginManager.load_all()`, plugins within the namespace that are discoverable in entrypoints can be loaded.
 If an error occurs at any state of the lifecycle, the `PluginManager` informs the `PluginLifecycleListener` about it, but continues operating.
 
 ### Discovering entrypoints
 
-At build time (e.g., with `python setup.py develop/install/sdist`), a special `PluginFinder` collects anything that can be interpreted as a `PluginSpec`, and creates from it setuptools entrypoints.
-In the `setup.py` we can use the `plugin.setuptools.load_entry_points` method to collect a dictionary for the `entry_points` value of `setup()`.
+To build a source distribution and a wheel of your code with your plugins as entrypoints, simply run `python setup.py plugins sdist bdist_wheel`.
 
-```python
-from plugin.setuptools import load_entry_points
+How it works:
+For discovering plugins at build time, plux provides a custom setuptools command `plugins`, invoked via `python setup.py plugins`.
+The command uses a special `PluginFinder` that collects from the codebase anything that can be interpreted as a `PluginSpec`, and creates from it a plugin index file `plux.json`, that is placed into the `.egg-info` distribution metadata directory.
+When a setuptools command is used to create the distribution (e.g., `python setup.py sdist/bdist_wheel/...`), plux finds the `plux.json` plugin index and extends automatically the list of entry points (collected into `.egg-info/entry_points.txt`).
+The `plux.json` file becomes a part of the distribution, s.t., the plugins do not have to be discovered every time your distribution is installed elsewhere.
 
-setup(
-    entry_points=load_entry_points(exclude=("tests", "tests.*",))
-)
-```
 
-Note that `load_entry_points` will try to resolve a cached version of `entry_points.txt` from the `.egg-info` directory,
-to avoid resolving the entry points when building the package from a source distribution.
 
 Examples
 --------
 
 To build something using the plugin framework, you will first want to introduce a Plugin that does something when it is loaded.
 And then, at runtime, you need a component that uses the `PluginManager` to get those plugins.
 
@@ -179,14 +175,29 @@
 
 runtime = LocalstackRuntime()
 
 for configurator in PluginManager("localstack.configurators").load_all():
     configurator(runtime)
 ```
 
+Configuring your distribution
+-----------------------------
+
+If you are building a python distribution that exposes plugins discovered by plux, you need to configure your projects build system so other dependencies creates the `entry_points.txt` file when installing your distribution.
+
+For a [`pyproject.toml`](https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/) template this involves adding the `build-system` section:
+
+```toml
+[build-system]
+requires = ['setuptools', 'wheel', 'plux>=1.3.1']
+build-backend = "setuptools.build_meta"
+
+# ...
+```
+
 Install
 -------
 
     pip install plux
 
 Develop
 -------
```

### Comparing `plux-1.3.1/plugin/__init__.py` & `plux-1.3.2/plugin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     PluginType,
     plugin,
 )
 from .manager import PluginManager, PluginSpecResolver
 
 name = "plugin"
 
-__version__ = "1.3.1"
+__version__ = "1.3.2"
 
 __all__ = [
     "FunctionPlugin",
     "Plugin",
     "PluginSpec",
     "PluginType",
     "PluginLifecycleListener",
```

### Comparing `plux-1.3.1/plugin/core.py` & `plux-1.3.2/plugin/core.py`

 * *Files identical despite different names*

### Comparing `plux-1.3.1/plugin/discovery.py` & `plux-1.3.2/plugin/discovery.py`

 * *Files identical despite different names*

### Comparing `plux-1.3.1/plugin/entrypoint.py` & `plux-1.3.2/plugin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `plux-1.3.1/plugin/manager.py` & `plux-1.3.2/plugin/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,15 +266,15 @@
 
             args = self.load_args
             kwargs = self.load_kwargs
 
             self._fire_on_load_before(plugin_spec, plugin, args, kwargs)
             try:
                 LOG.debug("loading plugin %s:%s", self.namespace, plugin_spec.name)
-                result = plugin.load(*args, *kwargs)
+                result = plugin.load(*args, **kwargs)
                 self._fire_on_load_after(plugin_spec, plugin, result)
                 container.load_value = result
                 container.is_loaded = True
             except Exception as e:
                 if LOG.isEnabledFor(logging.DEBUG):
                     LOG.exception("error loading plugin %s", plugin_spec)
                 self._fire_on_load_exception(plugin_spec, plugin, e)
```

### Comparing `plux-1.3.1/plugin/setuptools.py` & `plux-1.3.2/plugin/setuptools.py`

 * *Files identical despite different names*

### Comparing `plux-1.3.1/plux.egg-info/PKG-INFO` & `plux-1.3.2/plux.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,227 +1,238 @@
 Metadata-Version: 2.1
 Name: plux
-Version: 1.3.1
+Version: 1.3.2
 Summary: A dynamic code loading framework for building pluggable Python distributions
 Home-page: https://github.com/localstack/plux
 Author: Thomas Rausch
 Author-email: thomas@localstack.cloud
 License: Apache License 2.0
-Description: Plux
-        ====
-        
-        <p>
-          <a href="https://github.com/localstack/plux/actions/workflows/build.yml"><img alt="CI badge" src="https://github.com/localstack/plux/actions/workflows/build.yml/badge.svg"></img></a>
-          <a href="https://pypi.org/project/plux/"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/plux?color=blue"></a>
-          <a href="https://img.shields.io/pypi/l/plux.svg"><img alt="PyPI License" src="https://img.shields.io/pypi/l/plux.svg"></a>
-          <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-        </p>
-        
-        plux is the dynamic code loading framework used in [LocalStack](https://github.com/localstack/localstack).
-        
-        
-        Overview
-        --------
-        
-        Plux builds a higher-level plugin mechanism around [Python's entry point mechanism](https://packaging.python.org/specifications/entry-points/).
-        It provides tools to load plugins from entry points at run time, and to discover entry points from plugins at build time (so you don't have to declare entry points statically in your `setup.py`).
-        
-        ### Core concepts
-        
-        * `PluginSpec`: describes a `Plugin`. Each plugin has a namespace, a unique name in that namespace, and a `PluginFactory` (something that creates `Plugin` the spec is describing.
-          In the simplest case, that can just be the Plugin's class).
-        * `Plugin`: an object that exposes a `should_load` and `load` method.
-          Note that it does not function as a domain object (it does not hold the plugins lifecycle state, like initialized, loaded, etc..., or other metadata of the Plugin)
-        * `PluginFinder`: finds plugins, either at build time (by scanning the modules using `pkgutil` and `setuptools`) or at run time (reading entrypoints of the distribution using [stevedore](https://docs.openstack.org/stevedore/latest/))
-        * `PluginManager`: manages the run time lifecycle of a Plugin, which has three states:
-          * resolved: the entrypoint pointing to the PluginSpec was imported and the `PluginSpec` instance was created
-          * init: the `PluginFactory` of the `PluginSpec` was successfully invoked
-          * loaded: the `load` method of the `Plugin` was successfully invoked
-        
-        ![architecture](https://raw.githubusercontent.com/localstack/plux/main/docs/plux-architecture.png)
-        
-        ### Loading Plugins
-        
-        At run time, a `PluginManager` uses a `PluginFinder` that in turn uses stevedore to scan the available entrypoints for things that look like a `PluginSpec`.
-        With `PluginManager.load(name: str)` or `PluginManager.load_all()`, plugins within the namespace that are discoverable in entrypoints can be loaded.
-        If an error occurs at any state of the lifecycle, the `PluginManager` informs the `PluginLifecycleListener` about it, but continues operating.
-        
-        ### Discovering entrypoints
-        
-        At build time (e.g., with `python setup.py develop/install/sdist`), a special `PluginFinder` collects anything that can be interpreted as a `PluginSpec`, and creates from it setuptools entrypoints.
-        In the `setup.py` we can use the `plugin.setuptools.load_entry_points` method to collect a dictionary for the `entry_points` value of `setup()`.
-        
-        ```python
-        from plugin.setuptools import load_entry_points
-        
-        setup(
-            entry_points=load_entry_points(exclude=("tests", "tests.*",))
-        )
-        ```
-        
-        Note that `load_entry_points` will try to resolve a cached version of `entry_points.txt` from the `.egg-info` directory,
-        to avoid resolving the entry points when building the package from a source distribution.
-        
-        Examples
-        --------
-        
-        To build something using the plugin framework, you will first want to introduce a Plugin that does something when it is loaded.
-        And then, at runtime, you need a component that uses the `PluginManager` to get those plugins.
-        
-        ### One class per plugin
-        
-        This is the way we went with `LocalstackCliPlugin`. Every plugin class (e.g., `ProCliPlugin`) is essentially a singleton.
-        This is easy, as the classes are discoverable as plugins.
-        Simply create a Plugin class with a name and namespace and it will be discovered by the build time `PluginFinder`.
-        
-        ```python
-        
-        # abstract case (not discovered at build time, missing name)
-        class CliPlugin(Plugin):
-            namespace = "my.plugins.cli"
-        
-            def load(self, cli):
-                self.attach(cli)
-        
-            def attach(self, cli):
-                raise NotImplementedError
-        
-        # discovered at build time (has a namespace, name, and is a Plugin)
-        class MyCliPlugin(CliPlugin):
-            name = "my"
-        
-            def attach(self, cli):
-                # ... attach commands to cli object
-        
-        ```
-        
-        now we need a `PluginManager` (which has a generic type) to load the plugins for us:
-        
-        ```python
-        cli = # ... needs to come from somewhere
-        
-        manager: PluginManager[CliPlugin] = PluginManager("my.plugins.cli", load_args=(cli,))
-        
-        plugins: List[CliPlugin] = manager.load_all()
-        
-        # todo: do stuff with the plugins, if you want/need
-        #  in this example, we simply use the plugin mechanism to run a one-shot function (attach) on a load argument
-        
-        ```
-        
-        ### Re-usable plugins
-        
-        When you have lots of plugins that are structured in a similar way, we may not want to create a separate Plugin class
-        for each plugin. Instead we want to use the same `Plugin` class to do the same thing, but use several instances of it.
-        The `PluginFactory`, and the fact that `PluginSpec` instances defined at module level are discoverable (inpired
-        by [pluggy](https://github.com/pytest-dev/pluggy)), can be used to achieve that.
-        
-        ```python
-        
-        class ServicePlugin(Plugin):
-        
-            def __init__(self, service_name):
-                self.service_name = service_name
-                self.service = None
-        
-            def should_load(self):
-                return self.service_name in config.SERVICES
-        
-            def load(self):
-                module = importlib.import_module("localstack.services.%s" % self.service_name)
-                # suppose we define a convention that each service module has a Service class, like moto's `Backend`
-                self.service = module.Service()
-        
-        def service_plugin_factory(name) -> PluginFactory:
-            def create():
-                return ServicePlugin(name)
-        
-            return create
-        
-        # discoverable
-        s3 = PluginSpec("localstack.plugins.services", "s3", service_plugin_factory("s3"))
-        
-        # discoverable
-        dynamodb = PluginSpec("localstack.plugins.services", "dynamodb", service_plugin_factory("dynamodb"))
-        
-        # ... could be simplified with convenience framework code, but the principle will stay the same
-        
-        ```
-        
-        Then we could use the `PluginManager` to build a Supervisor
-        
-        ```python
-        
-        class Supervisor:
-            manager: PluginManager[ServicePlugin]
-        
-            def start(self, service_name):
-                plugin = manager.load(service_name)
-                service = plugin.service
-                service.start()
-        
-        ```
-        
-        ### Functions as plugins
-        
-        with the `@plugin` decorator, you can expose functions as plugins. They will be wrapped by the framework
-        into `FunctionPlugin` instances, which satisfy both the contract of a Plugin, and that of the function.
-        
-        ```python
-        from plugin import plugin
-        
-        
-        @plugin(namespace="localstack.configurators")
-        def configure_logging(runtime):
-            logging.basicConfig(level=runtime.config.loglevel)
-        
-            
-        @plugin(namespace="localstack.configurators")
-        def configure_somethingelse(runtime):
-            # do other stuff with the runtime object
-            pass
-        ```
-        
-        With a PluginManager via `load_all`, you receive the `FunctionPlugin` instances, that you can call like the functions
-        
-        ```python
-        
-        runtime = LocalstackRuntime()
-        
-        for configurator in PluginManager("localstack.configurators").load_all():
-            configurator(runtime)
-        ```
-        
-        Install
-        -------
-        
-            pip install plux
-        
-        Develop
-        -------
-        
-        Create the virtual environment, install dependencies, and run tests
-        
-            make venv
-            make test
-        
-        Run the code formatter
-        
-            make format
-        
-        Upload the pypi package using twine
-        
-            make upload
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: dev
+License-File: LICENSE
+
+Plux
+====
+
+<p>
+  <a href="https://github.com/localstack/plux/actions/workflows/build.yml"><img alt="CI badge" src="https://github.com/localstack/plux/actions/workflows/build.yml/badge.svg"></img></a>
+  <a href="https://pypi.org/project/plux/"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/plux?color=blue"></a>
+  <a href="https://img.shields.io/pypi/l/plux.svg"><img alt="PyPI License" src="https://img.shields.io/pypi/l/plux.svg"></a>
+  <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
+</p>
+
+plux is the dynamic code loading framework used in [LocalStack](https://github.com/localstack/localstack).
+
+
+Overview
+--------
+
+Plux builds a higher-level plugin mechanism around [Python's entry point mechanism](https://packaging.python.org/specifications/entry-points/).
+It provides tools to load plugins from entry points at run time, and to discover entry points from plugins at build time (so you don't have to declare entry points statically in your `setup.py`).
+
+### Core concepts
+
+* `PluginSpec`: describes a `Plugin`. Each plugin has a namespace, a unique name in that namespace, and a `PluginFactory` (something that creates `Plugin` the spec is describing.
+  In the simplest case, that can just be the Plugin's class).
+* `Plugin`: an object that exposes a `should_load` and `load` method.
+  Note that it does not function as a domain object (it does not hold the plugins lifecycle state, like initialized, loaded, etc..., or other metadata of the Plugin)
+* `PluginFinder`: finds plugins, either at build time (by scanning the modules using `pkgutil` and `setuptools`) or at run time (reading entrypoints of the distribution using [stevedore](https://docs.openstack.org/stevedore/latest/))
+* `PluginManager`: manages the run time lifecycle of a Plugin, which has three states:
+  * resolved: the entrypoint pointing to the PluginSpec was imported and the `PluginSpec` instance was created
+  * init: the `PluginFactory` of the `PluginSpec` was successfully invoked
+  * loaded: the `load` method of the `Plugin` was successfully invoked
+
+![architecture](https://raw.githubusercontent.com/localstack/plux/main/docs/plux-architecture.png)
+
+### Loading Plugins
+
+At run time, a `PluginManager` uses a `PluginFinder` that in turn uses stevedore to scan the available entrypoints for things that look like a `PluginSpec`.
+With `PluginManager.load(name: str)` or `PluginManager.load_all()`, plugins within the namespace that are discoverable in entrypoints can be loaded.
+If an error occurs at any state of the lifecycle, the `PluginManager` informs the `PluginLifecycleListener` about it, but continues operating.
+
+### Discovering entrypoints
+
+To build a source distribution and a wheel of your code with your plugins as entrypoints, simply run `python setup.py plugins sdist bdist_wheel`.
+
+How it works:
+For discovering plugins at build time, plux provides a custom setuptools command `plugins`, invoked via `python setup.py plugins`.
+The command uses a special `PluginFinder` that collects from the codebase anything that can be interpreted as a `PluginSpec`, and creates from it a plugin index file `plux.json`, that is placed into the `.egg-info` distribution metadata directory.
+When a setuptools command is used to create the distribution (e.g., `python setup.py sdist/bdist_wheel/...`), plux finds the `plux.json` plugin index and extends automatically the list of entry points (collected into `.egg-info/entry_points.txt`).
+The `plux.json` file becomes a part of the distribution, s.t., the plugins do not have to be discovered every time your distribution is installed elsewhere.
+
+
+
+Examples
+--------
+
+To build something using the plugin framework, you will first want to introduce a Plugin that does something when it is loaded.
+And then, at runtime, you need a component that uses the `PluginManager` to get those plugins.
+
+### One class per plugin
+
+This is the way we went with `LocalstackCliPlugin`. Every plugin class (e.g., `ProCliPlugin`) is essentially a singleton.
+This is easy, as the classes are discoverable as plugins.
+Simply create a Plugin class with a name and namespace and it will be discovered by the build time `PluginFinder`.
+
+```python
+
+# abstract case (not discovered at build time, missing name)
+class CliPlugin(Plugin):
+    namespace = "my.plugins.cli"
+
+    def load(self, cli):
+        self.attach(cli)
+
+    def attach(self, cli):
+        raise NotImplementedError
+
+# discovered at build time (has a namespace, name, and is a Plugin)
+class MyCliPlugin(CliPlugin):
+    name = "my"
+
+    def attach(self, cli):
+        # ... attach commands to cli object
+
+```
+
+now we need a `PluginManager` (which has a generic type) to load the plugins for us:
+
+```python
+cli = # ... needs to come from somewhere
+
+manager: PluginManager[CliPlugin] = PluginManager("my.plugins.cli", load_args=(cli,))
+
+plugins: List[CliPlugin] = manager.load_all()
+
+# todo: do stuff with the plugins, if you want/need
+#  in this example, we simply use the plugin mechanism to run a one-shot function (attach) on a load argument
+
+```
+
+### Re-usable plugins
+
+When you have lots of plugins that are structured in a similar way, we may not want to create a separate Plugin class
+for each plugin. Instead we want to use the same `Plugin` class to do the same thing, but use several instances of it.
+The `PluginFactory`, and the fact that `PluginSpec` instances defined at module level are discoverable (inpired
+by [pluggy](https://github.com/pytest-dev/pluggy)), can be used to achieve that.
+
+```python
+
+class ServicePlugin(Plugin):
+
+    def __init__(self, service_name):
+        self.service_name = service_name
+        self.service = None
+
+    def should_load(self):
+        return self.service_name in config.SERVICES
+
+    def load(self):
+        module = importlib.import_module("localstack.services.%s" % self.service_name)
+        # suppose we define a convention that each service module has a Service class, like moto's `Backend`
+        self.service = module.Service()
+
+def service_plugin_factory(name) -> PluginFactory:
+    def create():
+        return ServicePlugin(name)
+
+    return create
+
+# discoverable
+s3 = PluginSpec("localstack.plugins.services", "s3", service_plugin_factory("s3"))
+
+# discoverable
+dynamodb = PluginSpec("localstack.plugins.services", "dynamodb", service_plugin_factory("dynamodb"))
+
+# ... could be simplified with convenience framework code, but the principle will stay the same
+
+```
+
+Then we could use the `PluginManager` to build a Supervisor
+
+```python
+
+class Supervisor:
+    manager: PluginManager[ServicePlugin]
+
+    def start(self, service_name):
+        plugin = manager.load(service_name)
+        service = plugin.service
+        service.start()
+
+```
+
+### Functions as plugins
+
+with the `@plugin` decorator, you can expose functions as plugins. They will be wrapped by the framework
+into `FunctionPlugin` instances, which satisfy both the contract of a Plugin, and that of the function.
+
+```python
+from plugin import plugin
+
+
+@plugin(namespace="localstack.configurators")
+def configure_logging(runtime):
+    logging.basicConfig(level=runtime.config.loglevel)
+
+    
+@plugin(namespace="localstack.configurators")
+def configure_somethingelse(runtime):
+    # do other stuff with the runtime object
+    pass
+```
+
+With a PluginManager via `load_all`, you receive the `FunctionPlugin` instances, that you can call like the functions
+
+```python
+
+runtime = LocalstackRuntime()
+
+for configurator in PluginManager("localstack.configurators").load_all():
+    configurator(runtime)
+```
+
+Configuring your distribution
+-----------------------------
+
+If you are building a python distribution that exposes plugins discovered by plux, you need to configure your projects build system so other dependencies creates the `entry_points.txt` file when installing your distribution.
+
+For a [`pyproject.toml`](https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/) template this involves adding the `build-system` section:
+
+```toml
+[build-system]
+requires = ['setuptools', 'wheel', 'plux>=1.3.1']
+build-backend = "setuptools.build_meta"
+
+# ...
+```
+
+Install
+-------
+
+    pip install plux
+
+Develop
+-------
+
+Create the virtual environment, install dependencies, and run tests
+
+    make venv
+    make test
+
+Run the code formatter
+
+    make format
+
+Upload the pypi package using twine
+
+    make upload
```

### Comparing `plux-1.3.1/setup.cfg` & `plux-1.3.2/setup.cfg`

 * *Files identical despite different names*

