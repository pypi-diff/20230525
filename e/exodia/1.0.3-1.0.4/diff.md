# Comparing `tmp/exodia-1.0.3.tar.gz` & `tmp/exodia-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exodia-1.0.3.tar", last modified: Mon May 22 16:36:33 2023, max compression
+gzip compressed data, was "exodia-1.0.4.tar", last modified: Thu May 25 13:59:53 2023, max compression
```

## Comparing `exodia-1.0.3.tar` & `exodia-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-22 16:36:33.455678 exodia-1.0.3/
--rw-r--r--   0 leondaz    (501) staff       (20)    35148 2023-05-21 21:01:23.000000 exodia-1.0.3/LICENSE
--rw-r--r--   0 leondaz    (501) staff       (20)      226 2023-05-22 16:36:33.455571 exodia-1.0.3/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)     3962 2023-05-22 15:01:07.000000 exodia-1.0.3/README.md
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-22 16:36:33.454757 exodia-1.0.3/exodia/
--rw-r--r--   0 leondaz    (501) staff       (20)      185 2023-05-22 13:06:40.000000 exodia-1.0.3/exodia/__init__.py
--rw-r--r--   0 leondaz    (501) staff       (20)     1396 2023-05-22 13:06:40.000000 exodia-1.0.3/exodia/bases.py
--rw-r--r--   0 leondaz    (501) staff       (20)     1014 2023-05-22 13:06:40.000000 exodia-1.0.3/exodia/exceptions.py
--rw-r--r--   0 leondaz    (501) staff       (20)     4294 2023-05-22 16:30:32.000000 exodia-1.0.3/exodia/fields.py
--rw-r--r--   0 leondaz    (501) staff       (20)      101 2023-05-22 15:04:47.000000 exodia-1.0.3/exodia/utils.py
--rw-r--r--   0 leondaz    (501) staff       (20)     8516 2023-05-22 16:30:32.000000 exodia-1.0.3/exodia/validators.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-22 16:36:33.455180 exodia-1.0.3/exodia.egg-info/
--rw-r--r--   0 leondaz    (501) staff       (20)      226 2023-05-22 16:36:33.000000 exodia-1.0.3/exodia.egg-info/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)      313 2023-05-22 16:36:33.000000 exodia-1.0.3/exodia.egg-info/SOURCES.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-22 16:36:33.000000 exodia-1.0.3/exodia.egg-info/dependency_links.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        7 2023-05-22 16:36:33.000000 exodia-1.0.3/exodia.egg-info/top_level.txt
--rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-22 16:36:33.455711 exodia-1.0.3/setup.cfg
--rw-r--r--   0 leondaz    (501) staff       (20)      284 2023-05-22 16:36:17.000000 exodia-1.0.3/setup.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-22 16:36:33.455416 exodia-1.0.3/tests/
--rw-r--r--   0 leondaz    (501) staff       (20)     1232 2023-05-22 13:06:40.000000 exodia-1.0.3/tests/test_instance_creation.py
--rw-r--r--   0 leondaz    (501) staff       (20)     1629 2023-05-22 16:35:33.000000 exodia-1.0.3/tests/test_validation.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-25 13:59:53.017165 exodia-1.0.4/
+-rw-r--r--   0 leondaz    (501) staff       (20)    35148 2023-05-21 21:01:23.000000 exodia-1.0.4/LICENSE
+-rw-r--r--   0 leondaz    (501) staff       (20)      226 2023-05-25 13:59:53.017057 exodia-1.0.4/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)     4501 2023-05-24 18:30:51.000000 exodia-1.0.4/README.md
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-25 13:59:53.015959 exodia-1.0.4/exodia/
+-rw-r--r--   0 leondaz    (501) staff       (20)      208 2023-05-24 18:30:51.000000 exodia-1.0.4/exodia/__init__.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     1391 2023-05-25 12:15:31.000000 exodia-1.0.4/exodia/bases.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     1014 2023-05-22 13:06:40.000000 exodia-1.0.4/exodia/exceptions.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     6258 2023-05-25 12:52:22.000000 exodia-1.0.4/exodia/fields.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      101 2023-05-22 15:04:47.000000 exodia-1.0.4/exodia/utils.py
+-rw-r--r--   0 leondaz    (501) staff       (20)    10279 2023-05-25 12:53:58.000000 exodia-1.0.4/exodia/validators.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-25 13:59:53.016400 exodia-1.0.4/exodia.egg-info/
+-rw-r--r--   0 leondaz    (501) staff       (20)      226 2023-05-25 13:59:52.000000 exodia-1.0.4/exodia.egg-info/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)      313 2023-05-25 13:59:52.000000 exodia-1.0.4/exodia.egg-info/SOURCES.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-25 13:59:52.000000 exodia-1.0.4/exodia.egg-info/dependency_links.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        7 2023-05-25 13:59:52.000000 exodia-1.0.4/exodia.egg-info/top_level.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-25 13:59:53.017202 exodia-1.0.4/setup.cfg
+-rw-r--r--   0 leondaz    (501) staff       (20)      284 2023-05-25 13:58:47.000000 exodia-1.0.4/setup.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-25 13:59:53.016874 exodia-1.0.4/tests/
+-rw-r--r--   0 leondaz    (501) staff       (20)     1232 2023-05-22 13:06:40.000000 exodia-1.0.4/tests/test_instance_creation.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     2653 2023-05-25 13:59:34.000000 exodia-1.0.4/tests/test_validation.py
```

### Comparing `exodia-1.0.3/LICENSE` & `exodia-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `exodia-1.0.3/README.md` & `exodia-1.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -174,22 +174,39 @@
 
 class ValidatorStack(ex.Validator):
     def __init__(self, validators):
         self.validators = validators
 
     def validate(self, value, field_name=None, instance=None):
         for validator in self.validators:
-            validator.validate(value, field_name, instance)
+            try:
+                validator.validate(value, field_name, instance)
+            except ex.ExodiaException:
+                return False
 
+        return True
 ```
 
 And use it!
+
 ```python
 validate_multiple_of_5_and_25 = ValidatorStack(validators=[
     ex.validators.MultipleOf(5),
     ex.validators.MultipleOf(25),
 ])
 
 validate_multiple_of_5_and_25(30)  # everything explodes
 ```
 
+However, we do have this included as `ex.Stack`
+
+Exodia supports date/time/datetime objects as well with operators working as expected
+
+```python
+from datetime import datetime, date
+import exodia as ex
+
+ex.Date().before(date(year=3000, month=1, day=1)).validate(date(year=1971, month=1, day=1).isoformat())  # works
+ex.DateTime().validate(datetime(year=1971, month=1, day=1, hour=1, minute=1, second=1).isoformat()) # works
+```
+
 More is coming, actually more is still undocumented!
```

### Comparing `exodia-1.0.3/exodia/exceptions.py` & `exodia-1.0.4/exodia/exceptions.py`

 * *Files identical despite different names*

### Comparing `exodia-1.0.3/exodia/fields.py` & `exodia-1.0.4/exodia/fields.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 from collections.abc import Callable, Mapping
 from exodia import validators, ExodiaException
+from datetime import date, datetime
 
 
 class Field:
+    """
+    Represents a Field
+
+    class Person:
+        name = ex.Field()
+
+    except that you don't create Field instances, you create subclasses only.
+
+    :param of_type: represents the allowed types to be worked with during validation process
+    """
+
     of_type = None
 
     def __init__(self, *args, **kwargs):
         self._name = None
         self.args = args
         self.kwargs = kwargs
 
@@ -56,20 +68,27 @@
                 raise ExodiaException(
                     "Can't have validators [{v1}, {v2}] at the same time".format(
                         v1=validator.__class__.__name__,
                         v2=v.__name__,
                     )
                 )
 
+    def prepare_for_validation(self, v):
+        return v
+
     def validate(self, value):
-        self._run_validators(value)
+        self._run_validators(self.prepare_for_validation(value))
+        return self.to_repr(value)
 
     def get_type_validator(self):
         return validators.Type(self.of_type)
 
+    def to_repr(self, v):
+        return v
+
     def optional(self):
         self._no_validator_of_type(validators.Required)
         self._add_validator(validators.Optional())
 
         # generate an optional self.of_type validator
         current_type_validator = self._pop_validator(self.get_type_validator())
         OptionalTypeValidator = current_type_validator.merge(validators.Type(None))
@@ -86,20 +105,24 @@
         self._add_validator(validators.Function(f, message))
         return self
 
     def enum(self, options):
         self._add_validator(validators.Enum(options))
         return self
 
+    def ref(self, field, expr, message=None):
+        self._add_validator(validators.Ref(field, expr, message))
+        return self
+
     def __set__(self, instance, value):
-        self._run_validators(value, self._name, instance)
-        instance.__dict__[self._name] = value
+        self._run_validators(self.prepare_for_validation(value), self._name, instance)
+        instance.__dict__[self._name] = self.to_repr(value)
 
     def __get__(self, instance, owner):
-        return self.of_type(instance.__dict__[self._name])
+        return instance.__dict__[self._name]
 
 
 class String(Field):
     of_type = str
 
     def __init__(self, length=None, **kwargs):
         super().__init__(length, **kwargs)
@@ -119,19 +142,35 @@
         self._add_validator(validators.NotEmpty())
 
 
 class Integer(Field):
     of_type = int
 
     def min(self, value: int):
-        self._add_validator(validators.MinValue(value))
+        self._add_validator(
+            validators.Stack(
+                [
+                    validators.GreaterThan(value),
+                    validators.Equal(value),
+                ]
+            )
+        )
+
         return self
 
     def max(self, value: int):
-        self._add_validator(validators.MaxValue(value))
+        self._add_validator(
+            validators.Stack(
+                [
+                    validators.LessThan(value),
+                    validators.Equal(value),
+                ]
+            )
+        )
+
         return self
 
     def between(self, min: int, max: int):
         self._add_validator(validators.Between(min, max))
         return self
 
     def multiple_of(self, n):
@@ -149,7 +188,48 @@
 
 class Exodia(Field):
     of_type = Mapping
 
     def __init__(self, schema, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._add_validator(validators.Exodia(schema))
+
+
+class Date(Field):
+    of_type = [str, date]
+
+    def prepare_for_validation(self, v):
+        return date.fromisoformat(v)
+
+    def to_repr(self, v):
+        return date.fromisoformat(v)
+
+    def between(self, start: date, end: date):
+        self._add_validator(validators.Between(start, end))
+        return self
+
+    def before(self, d: date):
+        self._add_validator(validators.LessThan(d))
+        return self
+
+    def after(self, d: date):
+        self._add_validator(validators.GreaterThan(d))
+        return self
+
+
+class DateTime(Date):
+    of_type = [str, datetime]
+
+    def prepare_for_validation(self, v: str):
+        return datetime.fromisoformat(v)
+
+    def before(self, d: datetime):
+        self._add_validator(validators.LessThan(d))
+        return self
+
+    def after(self, d: datetime):
+        self._add_validator(validators.GreaterThan(d))
+        return self
+
+    def between(self, start: datetime, end: datetime):
+        self._add_validator(validators.Between(start, end))
+        return self
```

### Comparing `exodia-1.0.3/exodia/validators.py` & `exodia-1.0.4/exodia/validators.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from collections.abc import Mapping, Iterable
+from collections.abc import Mapping, Iterable, Callable
+from datetime import date, datetime, time
+from typing import Union, List
+
 from exodia import ExodiaException
 
 from exodia.utils import get_callable_params
 
 
 class Validator:
     field_message = "You've forgot to include a message for validator {class_name}"
@@ -92,43 +95,40 @@
         return len(value) == 0
 
 
 class Between(Validator):
     field_message = "{field_name} must be between ({min}, {max})"
     generic_message = "{value} is not between ({min}, {max})"
 
-    def __init__(self, min: int, max: int):
-        assert isinstance(min, int), "{}.min must be an instance of int".format(
-            self.__class__.__name__
-        )
-        assert isinstance(max, int), "{}.max must be an instance of int".format(
-            self.__class__.__name__
-        )
-
+    def __init__(self, min, max):
         super().__init__()
         self.min = min
         self.max = max
 
     def validate(self, value, field_name=None, instance=None):
         return self.min <= value <= self.max
 
 
 class Type(Validator):
-    generic_message = "{value} is of type {actual_type}, expected types {expected_types}"
+    generic_message = (
+        "{value} is of type {actual_type}, expected types {expected_types}"
+    )
     field_message = (
         "{field_name}={value} is of type {actual_type}, expected types {expected_types}"
     )
 
     def __init__(self, ts):
         if not isinstance(ts, Iterable):
             ts = [ts]
 
         # a hack to support "None" as a type instead of an instance of NoneType, just for convenience
         for i, t in enumerate(ts):
-            assert isinstance(t, type) or t is None, "{}.t must be a class".format(self.__class__.__name__)
+            assert isinstance(t, type) or t is None, "{}.t must be a class".format(
+                self.__class__.__name__
+            )
 
             if t is None:
                 ts[i] = type(None)
 
         self.ts = ts
         super().__init__()
 
@@ -138,24 +138,26 @@
     def validate(self, value, field_name=None, instance=None):
         return isinstance(value, tuple(self.ts))
 
     def get_format_params(self, value):
         return dict(
             **super().get_format_params(value),
             actual_type=type(value).__name__,
-            expected_types=", ".join(item.__class__.__name__ for item in self.ts),
+            expected_types=", ".join(item.__name__ for item in self.ts),
         )
 
 
 class MultipleOf(Validator):
     generic_message = "{value} is not a multiple of {n}"
     field_message = "{field_name}={value} is not a multiple of {n}"
 
     def __init__(self, n):
-        assert isinstance(n, int), "{}.n must be an instance of integer".format(self.__class__.__name__)
+        assert isinstance(n, int), "{}.n must be an instance of integer".format(
+            self.__class__.__name__
+        )
 
         super().__init__()
         self.n = n
 
     def validate(self, value, field_name=None, instance=None):
         return value % self.n == 0
 
@@ -166,17 +168,17 @@
 class Enum(Validator):
     field_message = (
         "{value} is not a valid choice for {field_name}, choices are {options}"
     )
     generic_message = "{value} is not a valid choice, choices are {options}"
 
     def __init__(self, options):
-        assert isinstance(options, Iterable) and not isinstance(options, Mapping), (
-            "{}.options must be a tuple-like object"
-        )
+        assert isinstance(options, Iterable) and not isinstance(
+            options, Mapping
+        ), "{}.options must be a tuple-like object"
 
         self.options = options
         super().__init__()
 
     def validate(self, value, field_name=None, instance=None):
         return value in self.options
 
@@ -184,70 +186,82 @@
 class MinLength(Validator):
     field_message = (
         "{class_name}.{field_name}={value} must have length greater than {length}"
     )
     generic_message = "{value} must have length greater than {length}"
 
     def __init__(self, length):
-        assert isinstance(length, int), "{}.length must be an instance of int".format(self.__class__.__name__)
+        assert isinstance(length, int), "{}.length must be an instance of str".format(
+            self.__class__.__name__
+        )
 
         super().__init__()
         self.length = length
 
     def validate(self, value, field_name=None, instance=None):
         return len(value) >= self.length
 
 
 class MaxLength(Validator):
     field_message = "{class_name}{field_name}={value} must have length less than {l}"
     generic_message = "{value} must have length less than {l}"
 
     def __init__(self, length):
-        assert isinstance(length, int), "{}.length must be an instance of int".format(self.__class__.__name__)
+        assert isinstance(length, int), "{}.length must be an instance of str".format(
+            self.__class__.__name__
+        )
 
         super().__init__()
         self.length = length
 
     def validate(self, value, field_name=None, instance=None):
         return len(value) <= self.length
 
 
-class MinValue(Validator):
-    field_message = (
-        "{class_name}.{field_name}={value} must have length greater than {v}"
-    )
-    generic_message = "{value} must have length greater than {v}"
+class LessThan(Validator):
+    field_message = "{class_name}.{field_name}={value} must be less than {v}"
+    generic_message = "{value} must be less than {v}"
 
     def __init__(self, v):
-        assert isinstance(v, int), "{}.length must be an instance of int".format(self.__class__.__name__)
-
         super().__init__()
         self.v = v
 
     def validate(self, value, field_name=None, instance=None):
-        return value >= self.v
+        return value < self.v
 
 
-class MaxValue(Validator):
-    generic_message = "{value} must have length greater than {v}"
-    field_message = "{class_name}{field_name}={value} must have length less than {v}"
+class Equal(Validator):
+    field_message = "{class_name}.{field_name}={value} must be equal to {v}"
+    generic_message = "{value} must be equal to {v}"
 
     def __init__(self, v):
-        assert isinstance(v, int), "{}.length must be an instance of int".format(self.__class__.__name__)
+        super().__init__()
+        self.v = v
 
+    def validate(self, value, field_name=None, instance=None):
+        return value == self.v
+
+
+class GreaterThan(Validator):
+    field_message = "{class_name}.{field_name}={value} must be greater than {v}"
+    generic_message = "{value} must be greater than {v}"
+
+    def __init__(self, v):
         super().__init__()
         self.v = v
 
     def validate(self, value, field_name=None, instance=None):
-        return self.v > value
+        return value > self.v
 
 
 class Exodia(Validator):
     def __init__(self, schema):
-        assert isinstance(schema, Mapping), "{}.length must be an instance of Mapping".format(self.__class__.__name__)
+        assert isinstance(
+            schema, Mapping
+        ), "{}.length must be an instance of Mapping".format(self.__class__.__name__)
 
         super().__init__()
         self.schema = schema
 
     def _recursive_validate_schema(self, data, field_name, instance):
         for key, v in self.schema.items():
             item = data.get(key) if data else None
@@ -268,7 +282,61 @@
         super().__init__()
 
     def get_message(self, field_name):
         return self.message
 
     def validate(self, value, field_name=None, instance=None):
         return self.f(value)
+
+
+class Stack(Validator):
+    def __init__(self, validators: List[Validator]):
+        for i, validator in enumerate(validators):
+            assert isinstance(
+                validator, Validator
+            ), "validators[{}] is not ex.validators.Validator instance".format(str(i))
+
+        self.validators = validators
+        self.validator_names = list(map(lambda v: v.__class__.__name__, validators))
+
+    def validate(self, value, field_name=None, instance=None):
+        for validator in self.validators:
+            try:
+                validator(value, field_name, instance)
+            except ExodiaException:
+                return False
+
+        return True
+
+
+class Ref(Validator):
+    def __init__(self, field, expr, message=None):
+        assert isinstance(expr, Callable), "Ref.expr must be a callable"
+
+        self.message = message or "ref expression for {} returned False".format(field)
+        self.field = field
+        self.expr = expr
+
+        super().__init__()
+
+    def get_message(self, field_name):
+        return self.message
+
+    def validate(self, value, field_name=None, instance=None):
+        if instance is None:
+            raise ExodiaException("can't use Field.ref without an instance context")
+
+        if isinstance(self.field, str):
+            field_name = self.field
+        else:
+            field_name = self.field._name
+
+        if not hasattr(instance, field_name):
+            raise ExodiaException(
+                "{class_name}.{field} does not exist".format(
+                    class_name=instance.__class__.__name__,
+                    field=self.field,
+                )
+            )
+
+        # no __dict__ because validation is still running
+        return self.expr(value, instance.__dict__[field_name])
```

### Comparing `exodia-1.0.3/tests/test_instance_creation.py` & `exodia-1.0.4/tests/test_instance_creation.py`

 * *Files identical despite different names*

