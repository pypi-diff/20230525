# Comparing `tmp/clean_ioc-0.1.1.tar.gz` & `tmp/clean_ioc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean_ioc-0.1.1.tar", max compression
+gzip compressed data, was "clean_ioc-0.1.2.tar", max compression
```

## Comparing `clean_ioc-0.1.1.tar` & `clean_ioc-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1067 2023-05-23 17:42:19.708716 clean_ioc-0.1.1/LICENSE
--rw-r--r--   0        0        0    15650 2023-05-23 17:42:19.708716 clean_ioc-0.1.1/README.md
--rw-r--r--   0        0        0    31136 2023-05-23 17:42:19.708716 clean_ioc-0.1.1/clean_ioc/__init__.py
--rw-r--r--   0        0        0      674 2023-05-23 17:42:19.708716 clean_ioc-0.1.1/clean_ioc/factories.py
--rw-r--r--   0        0        0     1320 2023-05-23 17:42:19.708716 clean_ioc-0.1.1/clean_ioc/functional_utils.py
--rw-r--r--   0        0        0     1811 2023-05-23 17:42:19.708716 clean_ioc-0.1.1/clean_ioc/registration_filters.py
--rw-r--r--   0        0        0      587 2023-05-23 17:42:19.708716 clean_ioc-0.1.1/clean_ioc/type_filters.py
--rw-r--r--   0        0        0     6537 2023-05-23 17:42:19.708716 clean_ioc-0.1.1/clean_ioc/typing_utils.py
--rw-r--r--   0        0        0     1125 2023-05-23 17:42:19.708716 clean_ioc-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    16897 1970-01-01 00:00:00.000000 clean_ioc-0.1.1/setup.py
--rw-r--r--   0        0        0    16290 1970-01-01 00:00:00.000000 clean_ioc-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-25 21:56:13.654200 clean_ioc-0.1.2/LICENSE
+-rw-r--r--   0        0        0    15650 2023-05-25 21:56:13.654200 clean_ioc-0.1.2/README.md
+-rw-r--r--   0        0        0    32274 2023-05-25 21:56:13.654200 clean_ioc-0.1.2/clean_ioc/__init__.py
+-rw-r--r--   0        0        0      674 2023-05-25 21:56:13.654200 clean_ioc-0.1.2/clean_ioc/factories.py
+-rw-r--r--   0        0        0     1320 2023-05-25 21:56:13.654200 clean_ioc-0.1.2/clean_ioc/functional_utils.py
+-rw-r--r--   0        0        0     1811 2023-05-25 21:56:13.654200 clean_ioc-0.1.2/clean_ioc/registration_filters.py
+-rw-r--r--   0        0        0      587 2023-05-25 21:56:13.654200 clean_ioc-0.1.2/clean_ioc/type_filters.py
+-rw-r--r--   0        0        0     6569 2023-05-25 21:56:13.654200 clean_ioc-0.1.2/clean_ioc/typing_utils.py
+-rw-r--r--   0        0        0     1125 2023-05-25 21:56:13.654200 clean_ioc-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    16897 1970-01-01 00:00:00.000000 clean_ioc-0.1.2/setup.py
+-rw-r--r--   0        0        0    16290 1970-01-01 00:00:00.000000 clean_ioc-0.1.2/PKG-INFO
```

### Comparing `clean_ioc-0.1.1/LICENSE` & `clean_ioc-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.1.1/README.md` & `clean_ioc-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.1.1/clean_ioc/__init__.py` & `clean_ioc-0.1.2/clean_ioc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,16 @@
     subject: Callable, local_ns: dict = {}, global_ns: dict | None = None
 ) -> dict[str, ArgInfo]:
     arg_spec_fn = subject if inspect.isfunction(subject) else subject.__init__
     args = get_type_hints(arg_spec_fn, global_ns, local_ns)
     signature = inspect.signature(subject)
     d: dict[str, ArgInfo] = {}
     for name, param in signature.parameters.items():
+        if "*" in str(param):
+            continue
         d[name] = ArgInfo(name=name, arg_type=args[name], default_value=param.default)
     return d
 
 
 _all_registartions = constant(True)
 
 
@@ -62,14 +64,16 @@
 class __Node__:
     service_type: type
     implementation: type | Callable
     parent: __Node__
     children: list[__Node__]
     decorator: __Node__
     decorated: __Node__
+    pre_configured_by: __Node__
+    pre_configures: __Node__
 
     @property
     def bottom_decorated(self):
         bottom = self.implementation
         decorated = self.decorated
         while decorated:
             bottom = decorated.implementation
@@ -79,14 +83,15 @@
 
 class EmptyNode(__Node__):
     def __init__(self):
         self.service_type = _empty
         self.implementation = _empty
         self.parent = self
         self.decorated = self
+        self.pre_configured_by = self
 
     def __bool__(self):
         return False
 
 
 class DependencyNode(__Node__):
     def __init__(
@@ -95,23 +100,29 @@
         self.service_type = service_type
         self.implementation = implementation
         self.lifespan = lifespan
         self.parent = EmptyNode()
         self.children = []
         self.decorated = EmptyNode()
         self.decorator = EmptyNode()
+        self.pre_configured_by = EmptyNode()
+        self.pre_configures = EmptyNode()
 
-    def add_child(self, node: DependencyNode):
-        self.children.append(node)
-        node.parent = self
-
-    def add_decorator(self, node: DependencyNode):
-        self.decorator = node
-        node.decorated = self
-        node.parent = self.parent
+    def add_child(self, child_node: DependencyNode):
+        self.children.append(child_node)
+        child_node.parent = self
+
+    def add_decorator(self, decorator_node: DependencyNode):
+        self.decorator = decorator_node
+        decorator_node.decorated = self
+        self.parent = decorator_node
+
+    def add_pre_configuration(self, pre_configuration_node: DependencyNode):
+        self.pre_configured_by = pre_configuration_node
+        pre_configuration_node.pre_configures = self
 
 
 class DependencyContext:
     def __init__(self, name: str, dependency_node: DependencyNode):
         self.name = name
         self.service_type = dependency_node.service_type
         self.implementation = dependency_node.implementation
@@ -257,25 +268,36 @@
     @classmethod
     def _get_dependencies(
         cls,
         creator_function: Callable,
         dependency_config: dict[str, DependencySettings],
     ) -> dict[str, Dependency]:
         args_infos = get_arg_info(creator_function)
-        return {
+        dependencies = {
             name: Dependency(
                 name=name,
                 parent_implementation=creator_function,
                 service_type=arg_info.arg_type,
                 settings=dependency_config[name],
                 default_value=arg_info.default_value,
             )
             for name, arg_info in args_infos.items()
         }
 
+        for extra_kwarg in set(dependency_config.keys()) ^ set(dependencies.keys()):
+            dependencies[extra_kwarg] = Dependency(
+                name=extra_kwarg,
+                parent_implementation=creator_function,
+                service_type=Any,
+                settings=dependency_config[extra_kwarg],
+                default_value=_empty,
+            )
+
+        return dependencies
+
     def create(
         self,
         context: ResolvingContext,
         dependency_node: DependencyNode,
         **kwargs,
     ):
         for arg_name, arg_dep in self.dependencies.items():
@@ -314,20 +336,20 @@
         self,
         service_type: type,
         pre_configuration: Callable[..., None],
         registration_filter: RegistartionFilter,
         dependency_config: dict[str, DependencySettings],
     ):
         self.service_type = service_type
-        self.pre_configuration = pre_configuration
+        self.configuration_fn = pre_configuration
         self.filter = registration_filter
         self.dependency_config = dependency_config
 
         self.creator = ImplementationCreator(
-            creator_function=self.pre_configuration,
+            creator_function=self.configuration_fn,
             dependency_config=self.dependency_config,
         )
 
         self.id = str(uuid4())
 
     def run(self, context: ResolvingContext, dependency_node: DependencyNode):
         self.creator.create(context=context, dependency_node=dependency_node)
@@ -383,33 +405,40 @@
         self._id = str(uuid4())
         self.generic_mapping = get_typevar_to_type_mapping(self.service_type)
 
     @property
     def is_named(self):
         return self.name is not None
 
-    def build(self, context: ResolvingContext, dependency_node: DependencyNode):
-        next_node = DependencyNode(
+    def build(self, context: ResolvingContext, parent_node: DependencyNode):
+        my_node = DependencyNode(
             service_type=self.service_type,
             implementation=self.implementation,
             lifespan=self.lifespan,
         )
 
-        dependency_node.add_child(next_node)
+        parent_node.add_child(my_node)
 
         pre_configurations = context.find_pre_configurations_that_apply(self)
 
         for pre_configuration in pre_configurations:
-            pre_configuration.run(context, dependency_node)
+            pre_configuration_node = DependencyNode(
+                self.service_type,
+                pre_configuration.configuration_fn,
+                lifespan=Lifespan.singleton,
+            )
+            my_node.add_pre_configuration(pre_configuration_node)
+
+            pre_configuration.run(context, pre_configuration_node)
 
         cached_instance = context.get_cached(self._id)
         if not cached_instance == _empty:
             return cached_instance
-        built_instance = self.creator.create(context, next_node)
-        decorated_node = next_node
+        built_instance = self.creator.create(context, my_node)
+        decorated_node = my_node
         for dec in context.find_decorators_that_apply(self):
             next_dec_node = DependencyNode(
                 service_type=self.service_type,
                 implementation=dec.decorator_type,
                 lifespan=self.lifespan,
             )
             decorated_node.add_decorator(next_dec_node)
@@ -478,22 +507,22 @@
         }
 
     def get(self, registration_id: str):
         instance = self._current_items.get(registration_id, _empty)
         if instance is not _empty:
             return instance
 
-        instance = self.registry.singletons.get(registration_id, _empty)
+        instance = self.scope.scoped_instances.get(registration_id, _empty)
         if instance is not _empty:
             self._current_items[registration_id] = instance
+            return instance
 
-        instance = self.scope.scoped_instances.get(registration_id, _empty)
+        instance = self.registry.singletons.get(registration_id, _empty)
         if instance is not _empty:
             self._current_items[registration_id] = instance
-            return instance
 
         return instance
 
     def put(self, registration_id: str, instance: Any, lifespan: Lifespan):
         if lifespan == Lifespan.singleton:
             self.registry.add_singleton_instance(registration_id, instance)
         elif lifespan == Lifespan.scoped:
```

### Comparing `clean_ioc-0.1.1/clean_ioc/factories.py` & `clean_ioc-0.1.2/clean_ioc/factories.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.1.1/clean_ioc/functional_utils.py` & `clean_ioc-0.1.2/clean_ioc/functional_utils.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.1.1/clean_ioc/registration_filters.py` & `clean_ioc-0.1.2/clean_ioc/registration_filters.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.1.1/clean_ioc/type_filters.py` & `clean_ioc-0.1.2/clean_ioc/type_filters.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.1.1/clean_ioc/typing_utils.py` & `clean_ioc-0.1.2/clean_ioc/typing_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import _GenericAlias, _SpecialGenericAlias  # type: ignore
+from typing import _GenericAlias, _SpecialGenericAlias, Protocol  # type: ignore
 from typing import Generic, TypeVar
 from collections.abc import Callable
 from typing import get_type_hints
 import types
 from queue import Queue
 import inspect
 
@@ -149,15 +149,15 @@
     aliases = []
 
     if root_origin := (getattr(cls, "__origin__", None)):
         queue.put(root_origin)
 
     while not queue.empty():
         type_check = queue.get()
-        if getattr(type_check, "__origin__", None) == Generic:
+        if getattr(type_check, "__origin__", None) in (Generic, Protocol):
             aliases.append(type_check)
 
         for base in getattr(type_check, "__orig_bases__", ()):
             queue.put(base)
             if orig := getattr(base, "__origin__", None):
                 queue.put(orig)
 
@@ -180,15 +180,15 @@
             queue.put(base)
             if base_orig := getattr(base, "__origin__", None):
                 queue.put(base_orig)
 
     return aliases
 
 
-def get_typevar_to_type_mapping(cls: type) -> dict[type, type]:
+def get_typevar_to_type_mapping(cls: type) -> dict[type | TypeVar, type]:
     generic_definitions = get_open_generic_aliases(cls)
     generic_implementations = get_generic_aliases(cls)
 
     generic_implementations = generic_implementations[: len(generic_definitions)]
 
     generic_definitions.reverse()
     generic_implementations.reverse()
```

### Comparing `clean_ioc-0.1.1/pyproject.toml` & `clean_ioc-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clean_ioc"
-version = "0.1.1"
+version = "0.1.2"
 description = "An IOC Container for Python 3.10+"
 authors = ["Peter Daly"]
 license = "MIT"
 homepage = "https://github.com/peter-daly/clean_ioc"
 repository = "https://github.com/peter-daly/clean_ioc"
 documentation = "https://github.com/peter-daly/clean_ioc"
 readme = "README.md"
```

### Comparing `clean_ioc-0.1.1/setup.py` & `clean_ioc-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['clean_ioc']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'clean-ioc',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'An IOC Container for Python 3.10+',
     'long_description': '# Clean IoC\nA simple dependency injection library for python that requires nothing of your application code (except that you use typing).\n\n\n## Basic Registering and resolving\n\nThere are 4 basic modes of registering a new set of classes\n\n### Implementation\n\n```python\n\nclass UserRepository(abc.ABC)\n    @abc.abstractmethod\n    def add(self, user):\n        pass\n\nclass InMemoryUserRepository(UserRepository)\n\n    def __init__(self):\n        self.users = []\n\n    def add(self, user):\n        # This is obviously terrible, but it\'s for demo purposes\n        self.users.append(user)\n\nclass SqlAlchemyUserRepository(UserRepository)\n\n    def __init__(self):\n        # Do some db stuff here\n        pass\n\n    def add(self, user):\n        # Do some db stuff here\n        pass\n\ncontainer = Container()\ncontainer.register(UserRepository, InMemoryUserRepository)\n\n\nrepository = container.resolve(UserRepository) # This will return an InMemoryUserRepository\n\n```\n\n### Concrete Class\n\n```python\n\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n### Factory\n\n```python\n\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\ndef client_factory(dep: ClientDependency):\n    return Client(dep=dep)\n\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client, factory=client_factory)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n\n### Instance\n\n```python\n\nclass ClientDependency\n    def __init__(self, num):\n        self.num = num\n\n    def get_int(self):\n        return self.num\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\nclient_dependency = ClientDependency(num=10)\n\ncontainer = Container()\ncontainer.register(ClientDependency, instance=client_dependency)\ncontainer.register(Client)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n## List resolving\n\n```python\n\nclass ClientDependency\n    def __init__(self, numbers: list[int]):\n        self.numbers = numbers\n\n    def get_numbers(self):\n        return self.numbers\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_numbers(self):\n        return self.dep.get_numbers()\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client)\ncontainer.register(int, instance=1)\ncontainer.register(int, instance=2)\ncontainer.register(int, instance=3)\n\nclient = container.resolve(Client)\n\nclient.get_numbers() # returns [3, 2, 1]\n```\n\n\n## Decorators\n\nFollows a object orientated decoration pattern, rather than a decoration annotation.\nThe main reason for this was to allow decotation of registered instances\n\n```python\nclass Client\n    def __init__(self, number: int)\n        self.number = number\n\n    def get_number(self):\n        return self.number\n\n\nclass DoubleClientDecorator(Client):\n    def __init__(self, client: Client):\n        self.client = client\n    def get_number(self):\n        return self.client.get_number() * 2\n\ncontainer = Container()\n\ncontainer.register(Client)\ncontainer.register_decorator(Client, DoubleClientDecorator)\ncontainer.register(int, instance=10)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 20\n```\n\n\nDecorators are resolved in order of when first registered. So the first registered decorator is the highest in the class tree\n\n\n```python\n    class Concrete:\n        pass\n\n    class DecoratorOne(Concrete):\n        def __init__(self, child: Concrete):\n            self.child = child\n\n    class DecoratorTwo(Concrete):\n        def __init__(self, child: Concrete):\n            self.child = child\n\n    container = Container()\n\n    container.register(Concrete)\n    container.register_decorator(Concrete, DecoratorOne)\n    container.register_decorator(Concrete, DecoratorTwo)\n\n    root = container.resolve(Concrete)\n\n    type(root) # returns DecoratorOne\n    type(root.child) # returns DecoratorTwo\n    type(root.child.child) # returns Concrete\n```\n\n\n## Subclasses registration\n\nThis feature allows registartion of all subclasses of a giveb type\n\n```python\nclass Client(abc.ABC)\n    @abc.abstractmethod\n    def get_number(self):\n        pass\n\n\nclass TenClient(Client)\n    def get_number(self):\n        return 10\n\nclass TwentyClient(Client)\n    def get_number(self):\n        return 20\n\ncontainer = Container()\n\ncontainer.register_subclasses(Client)\n\nten_client = container.resolve(TenClient)\nten_client.get_number() # returns 10\n\ntwenty_client = container.resolve(TwentyClient)\ntwenty_client.get_number() # returns 20\n\n# Resolve all subsclasses of Client\nclient = container.resolve(list[Client]) ## [TwentyClient(), TenClient()]\n```\n\n\n## Lifespans\nLifespans configure how long and resolved object says alive for\nThere are 4 lifespan types\n\n### transient\nAlways create a new instance\n\n```python\ncontainer.register(Client, lifespan=Lifespan.transient)\n```\n\n\n### once_per_graph (Default behaviour)\nOnly create one instance throughout the resolve call\n\n```python\ncontainer.register(Client, lifespan=Lifespan.once_per_graph)\n```\n\n### scoped\nOnly create a new instance through the life a scope. When not in a scope the behaviour is the same as **once_per_graph**\n\n```python\ncontainer.register(Client, lifespan=Lifespan.scoped)\n```\n\n### singleton\nOnly one instance of the object is created throughout the lifespan of the container\n\n```python\ncontainer.register(Client, lifespan=Lifespan.singleton)\n```\n\n*Note:*\nWhen registering an instance, then the behaviour is always singleton\n\n```python\ncontainer.register(int, instance=10)\n```\n\n## Open Generics\n\nRegisters all generic subclasses of the service type and allows you to resolve with the generic alias\n\n```python\nT = TypeVar("T")\n\nclass HelloCommand:\n    pass\n\nclass GoodbyeCommand:\n    pass\n\nclass CommandHandler(Generic[T]):\n    def handle(self, command: T):\n        pass\n\nclass HelloCommandHandler(CommandHandler[HelloCommand]):\n    def handle(self, command: HelloCommand):\n        print(\'HELLO\')\n\nclass GoodbyeCommandHandler(CommandHandler[GoodbyeCommand]):\n    def handle(self, command: GoodbyeCommand):\n        print(\'GOODBYE\')\n\ncontainer = Container()\ncontainer.register_open_generic(CommandHandler)\n\nh1 = container.resolve(CommandHandler[HelloCommand])\nh2 = container.resolve(CommandHandler[GoodbyeCommand])\n\nh1.handle(HelloCommand()) # prints \'HELLO\'\nh2.handle(GoodbyeCommand()) # prints \'GOODBYE\'\n\n```\n\n## Open Generic Decorators\n\n\nAllows you to add decorators to your open generic registrations\n\n```python\nT = TypeVar("T")\n\nclass HelloCommand:\n    pass\n\nclass GoodbyeCommand:\n    pass\n\nclass CommandHandler(Generic[T]):\n    def handle(self, command: T):\n        pass\n\nclass HelloCommandHandler(CommandHandler[HelloCommand]):\n    def handle(self, command: HelloCommand):\n        print(\'HELLO\')\n\nclass GoodbyeCommandHandler(CommandHandler[GoodbyeCommand]):\n    def handle(self, command: GoodbyeCommand):\n        print(\'GOODBYE\')\n\nclass AVeryBigCommandHandlerDecorator(Generic[T]):\n    def __init__(self, handler: CommandHandler[T]):\n        self.handler = handler\n\n    def handle(self, command: T):\n        print(\'A VERY BIG\')\n        self.handler.handle(command=command)\n\ncontainer = Container()\ncontainer.register_open_generic(CommandHandler)\ncontainer.register_open_generic_decorator(CommandHandler, AVeryBigCommandHandlerDecorator)\nh1 = container.resolve(CommandHandler[HelloCommand])\nh2 = container.resolve(CommandHandler[GoodbyeCommand])\n\nh1.handle(HelloCommand()) # prints \'A VERY BIG\\nHELLO\'\nh2.handle(GoodbyeCommand()) # prints \'A VERY BIG\\nGOODBYE\'\n\n```\n\n## Scopes\n\nScopes are a way to create a sub container that will live for a certain lifespan.\nSome good use cases for scope would be for the lifespan of handling a http request with a web server or a message/event if working on a message based system\n\n\n```python\nclass Client\n    def __init__(self, number: int)\n        return number\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n\nwith container.get_scope() as scope:\n    scope.register(int, instance=10)\n    scoped_client = scope.resolve(Client)\n    scoped_client.get_number() # returns 10\n```\n\n## Named registartions & Registartion filters\n\nBy default the last registration is what the container will return when resolve is called as below.\n\n```python\n\ncontainer = Container()\ncontainer.register(int, instance=1)\ncontainer.register(int, instance=2)\ncontainer.register(int, instance=3)\n\nnumber = container.resolve(int) # returns 3\n\n```\nTo be more selective of what we return we can add a name to the registration and apply a registartion filter when we resolve.\n\nA registartion filter is simply function that receives a **Registartion** and returns a **bool**\n\nFor example if we wanted to get the int named **"One"** we do the following\n\n```python\ncontainer = Container()\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\ncontainer.register(int, instance=3, name="Three")\n\nnumber = container.resolve(int, filter=lambda r: r.name == "One") # returns 1\n```\n\nClean IOC comes with a set of in built registartion filters that can be found [here](./clean_ioc/registration_filters.py)\n\nWe can get the desired behaviour as above\n```python\nfrom clean_ioc.registartion_filters import with_name\n\ncontainer = Container()\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\ncontainer.register(int, instance=3, name="Three")\n\nnumber = container.resolve(int, filter=with_name("One")) # returns 1\n```\n\n## Dependency Settings\n\nDependency settings are defined at registartion and allow you to define the selection or setting dependencies\n\n\n```python\nclass Client\n    def __init__(self, number=10)\n        self.number = number\n\n    def get_number(self):\n        return self.number\n\ncontainer = Container()\n\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\n\ncontainer.register(\n    Client,\n    name="SetsValue",\n    dependency_config={"number": DependencySettings(value=50)}\n)\ncontainer.register(\n    Client,\n    name="UsesDefaultValue"\n)\ncontainer.register(\n    Client,\n    name="IgnoresDefaultParameterValue",\n    dependency_config={"number": DependencySettings(use_default_paramater=False)}\n)\ncontainer.register(\n    Client,\n    name="UsesRegistartionFilter",\n    dependency_config={"number": DependencySettings(use_default_paramater=False, filter=with_name("One"))}\n)\n\nclient1 = container.resolve(Client, filter=with_name("SetsValue"))\nclient2 = container.resolve(Client, filter=with_name("UsesDefaultValue"))\nclient3 = container.resolve(Client, filter=with_name("IgnoresDefaultParameterValue"))\nclient4 = container.resolve(Client, filter=with_name("UsesRegistartionFilter"))\n\n\nclient1.get_number() # returns 50\nclient2.get_number() # returns 10\nclient3.get_number() # returns 2\nclient4.get_number() # returns 1\n```\n\nThe order of a dependant value is as follows\n1. Setting the dependency value explicitly\n    ```python\n    DependencySettings(value=50)\n    ```\n2. Using the default parameter value if it exisis the dependency value explicitly\n    ```python\n    class Client\n    def __init__(self, number=10)\n        self.number = number\n    ```\n    If you don\'t want to use the default parameter value you can set it to false in the dependency setting\n    ```python\n    DependencySettings(use_default_paramater=False)\n    ```\n3. Going to the container registry to find a registartion using the registration filter if, if there is a default value on the dependant paramater you must explicity set.\n\n## Accessing the Container, Scope and Resolver within dependencies\n\nAccessing container directly\n\n```python\nclass Client\n    def __init__(self, container: Container)\n        self.container = container\n\n    def get_number(self):\n        return self.container.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n```\n\nAccessing Resolver also returns the container\n\n```python\n\nclass Client\n    def __init__(self, resolver: Resolver)\n        self.resolver = resolver\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n```\n\nWhen within a scope, Resolver returns the current scope rather than the container\n\n```python\nclass Client\n    def __init__(self, resolver: Resolver)\n        self.resolver = resolver\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n\nwith container.get_scope() as scope:\n    scope.register(int, instance=10)\n    scoped_client = scope.resolve(Client)\n    scoped_client.get_number() # returns 10\n```\n\n\n## Modules (BETA feature)\n\n\nA module is a just a function that accepts a container, it can be used to set up common elements on the container\n\n```python\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\ndef client_module(c: Container):\n    c.register(ClientDependency)\n    c.register(Client)\n\ncontainer.apply_module(client_module)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n```\n\n\n\n## DependencyContext (BETA feature)\n\nYou can inject a special type into your dependants that allows you to inspect the current dependency tree. For instances you can check the parent of the current class you are constructing\nOne example of where this becomes useful is if injecting a logger, you can get information about the loggers parent to add extra context\n\n```python\nclass Logger\n    def __init__(self, module):\n        self.module = module\n\nclass Client\n    def __init__(self, logger: Logger)\n        self.logger = logger\n\ndef logger_fac(context: DependencyContext):\n    module = context.parent.implementation.__module__\n    return Logger(module)\n\n\ncontainer = Container()\ncontainer.register(Client)\ncontainer.register(Logger, factory=logger_fac)\n\nclient = container.resolve(Client)\n\n\n```\n\n\n## Pre-configurations\n\nPre configurations run a side-effect for a type before the type gets resolved.\nThis is useful if some python modules have some sort of module level functions that need to be called before the object get created\n\n```python\nimport logging\n\nclass Client\n    def __init__(self, logger: logging.Logger)\n        self.logger = logger\n\n    def do_a_thing(self):\n        self.logger.info(\'Doing a thing\')\n\ndef logger_fac(context: DependencyContext):\n    module = context.parent.implementation.__module__\n    return logging.getLogger(module)\n\ndef configuring_logging():\n    logging.basicConfig()\n\n\n\n\ncontainer = Container()\ncontainer.register(Client)\ncontainer.register(logging.Logger, factory=logger_fac)\ncontainer.pre_configure(logging.Logger, configuring_logging)\n\nclient = container.resolve(Client)\n\n\n```',
     'author': 'Peter Daly',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/peter-daly/clean_ioc',
```

### Comparing `clean_ioc-0.1.1/PKG-INFO` & `clean_ioc-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-ioc
-Version: 0.1.1
+Version: 0.1.2
 Summary: An IOC Container for Python 3.10+
 Home-page: https://github.com/peter-daly/clean_ioc
 License: MIT
 Author: Peter Daly
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

