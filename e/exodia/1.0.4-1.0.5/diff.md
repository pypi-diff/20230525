# Comparing `tmp/exodia-1.0.4.tar.gz` & `tmp/exodia-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exodia-1.0.4.tar", last modified: Thu May 25 13:59:53 2023, max compression
+gzip compressed data, was "exodia-1.0.5.tar", last modified: Thu May 25 15:19:54 2023, max compression
```

## Comparing `exodia-1.0.4.tar` & `exodia-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-25 13:59:53.017165 exodia-1.0.4/
--rw-r--r--   0 leondaz    (501) staff       (20)    35148 2023-05-21 21:01:23.000000 exodia-1.0.4/LICENSE
--rw-r--r--   0 leondaz    (501) staff       (20)      226 2023-05-25 13:59:53.017057 exodia-1.0.4/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)     4501 2023-05-24 18:30:51.000000 exodia-1.0.4/README.md
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-25 13:59:53.015959 exodia-1.0.4/exodia/
--rw-r--r--   0 leondaz    (501) staff       (20)      208 2023-05-24 18:30:51.000000 exodia-1.0.4/exodia/__init__.py
--rw-r--r--   0 leondaz    (501) staff       (20)     1391 2023-05-25 12:15:31.000000 exodia-1.0.4/exodia/bases.py
--rw-r--r--   0 leondaz    (501) staff       (20)     1014 2023-05-22 13:06:40.000000 exodia-1.0.4/exodia/exceptions.py
--rw-r--r--   0 leondaz    (501) staff       (20)     6258 2023-05-25 12:52:22.000000 exodia-1.0.4/exodia/fields.py
--rw-r--r--   0 leondaz    (501) staff       (20)      101 2023-05-22 15:04:47.000000 exodia-1.0.4/exodia/utils.py
--rw-r--r--   0 leondaz    (501) staff       (20)    10279 2023-05-25 12:53:58.000000 exodia-1.0.4/exodia/validators.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-25 13:59:53.016400 exodia-1.0.4/exodia.egg-info/
--rw-r--r--   0 leondaz    (501) staff       (20)      226 2023-05-25 13:59:52.000000 exodia-1.0.4/exodia.egg-info/PKG-INFO
--rw-r--r--   0 leondaz    (501) staff       (20)      313 2023-05-25 13:59:52.000000 exodia-1.0.4/exodia.egg-info/SOURCES.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-25 13:59:52.000000 exodia-1.0.4/exodia.egg-info/dependency_links.txt
--rw-r--r--   0 leondaz    (501) staff       (20)        7 2023-05-25 13:59:52.000000 exodia-1.0.4/exodia.egg-info/top_level.txt
--rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-25 13:59:53.017202 exodia-1.0.4/setup.cfg
--rw-r--r--   0 leondaz    (501) staff       (20)      284 2023-05-25 13:58:47.000000 exodia-1.0.4/setup.py
-drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-25 13:59:53.016874 exodia-1.0.4/tests/
--rw-r--r--   0 leondaz    (501) staff       (20)     1232 2023-05-22 13:06:40.000000 exodia-1.0.4/tests/test_instance_creation.py
--rw-r--r--   0 leondaz    (501) staff       (20)     2653 2023-05-25 13:59:34.000000 exodia-1.0.4/tests/test_validation.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-25 15:19:54.799270 exodia-1.0.5/
+-rw-r--r--   0 leondaz    (501) staff       (20)    35148 2023-05-21 21:01:23.000000 exodia-1.0.5/LICENSE
+-rw-r--r--   0 leondaz    (501) staff       (20)      226 2023-05-25 15:19:54.799164 exodia-1.0.5/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)     5743 2023-05-25 15:19:46.000000 exodia-1.0.5/README.md
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-25 15:19:54.798031 exodia-1.0.5/exodia/
+-rw-r--r--   0 leondaz    (501) staff       (20)      208 2023-05-24 18:30:51.000000 exodia-1.0.5/exodia/__init__.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     1836 2023-05-25 15:15:26.000000 exodia-1.0.5/exodia/bases.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     1014 2023-05-22 13:06:40.000000 exodia-1.0.5/exodia/exceptions.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     6258 2023-05-25 12:52:22.000000 exodia-1.0.5/exodia/fields.py
+-rw-r--r--   0 leondaz    (501) staff       (20)      101 2023-05-22 15:04:47.000000 exodia-1.0.5/exodia/utils.py
+-rw-r--r--   0 leondaz    (501) staff       (20)    10279 2023-05-25 12:53:58.000000 exodia-1.0.5/exodia/validators.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-25 15:19:54.798671 exodia-1.0.5/exodia.egg-info/
+-rw-r--r--   0 leondaz    (501) staff       (20)      226 2023-05-25 15:19:54.000000 exodia-1.0.5/exodia.egg-info/PKG-INFO
+-rw-r--r--   0 leondaz    (501) staff       (20)      313 2023-05-25 15:19:54.000000 exodia-1.0.5/exodia.egg-info/SOURCES.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        1 2023-05-25 15:19:54.000000 exodia-1.0.5/exodia.egg-info/dependency_links.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)        7 2023-05-25 15:19:54.000000 exodia-1.0.5/exodia.egg-info/top_level.txt
+-rw-r--r--   0 leondaz    (501) staff       (20)       38 2023-05-25 15:19:54.799306 exodia-1.0.5/setup.cfg
+-rw-r--r--   0 leondaz    (501) staff       (20)      284 2023-05-25 15:19:32.000000 exodia-1.0.5/setup.py
+drwxr-xr-x   0 leondaz    (501) staff       (20)        0 2023-05-25 15:19:54.799021 exodia-1.0.5/tests/
+-rw-r--r--   0 leondaz    (501) staff       (20)     1232 2023-05-22 13:06:40.000000 exodia-1.0.5/tests/test_instance_creation.py
+-rw-r--r--   0 leondaz    (501) staff       (20)     3555 2023-05-25 15:19:46.000000 exodia-1.0.5/tests/test_validation.py
```

### Comparing `exodia-1.0.4/LICENSE` & `exodia-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `exodia-1.0.4/README.md` & `exodia-1.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -202,11 +202,66 @@
 Exodia supports date/time/datetime objects as well with operators working as expected
 
 ```python
 from datetime import datetime, date
 import exodia as ex
 
 ex.Date().before(date(year=3000, month=1, day=1)).validate(date(year=1971, month=1, day=1).isoformat())  # works
-ex.DateTime().validate(datetime(year=1971, month=1, day=1, hour=1, minute=1, second=1).isoformat()) # works
+ex.DateTime().validate(datetime(year=1971, month=1, day=1, hour=1, minute=1, second=1).isoformat())  # works
 ```
 
-More is coming, actually more is still undocumented!
+### What if you have dependant fields?
+
+```python
+import exodia as ex
+
+
+class Person(ex.Base):
+    age = ex.Integer().required()
+    younger_brother_age = ex.Integer().required()
+
+    def validate(self, attrs):
+        # no need to check if age in attrs, you can't get into this step
+        # without providing both because both are required
+        # any assertion errors are transformed into ex.ExodiaException instances
+        assert attrs['age'] > attrs['younger_brother_age'], "PUT IN YOUR MESSAGE"
+```
+
+However, that's not the only way to do it
+
+```python
+import exodia as ex
+
+
+class Person(ex.Base):
+    age = ex.Integer().required()
+    younger_brother_age = (
+        ex.Integer()
+            .ref(
+            age,
+            lambda me, my_bro: my_bro > me, "younger brother can't be older!"
+        )
+    )
+```
+
+### OR
+
+```python
+import exodia as ex
+
+
+class Person(ex.Base):
+    younger_brother_age = (
+        ex.Integer()
+            .ref(
+            'age',
+            lambda me, my_bro: my_bro > me, "younger brother can't be older!"
+        )
+    )
+    age = ex.Integer().required()
+```
+
+Notice the quotes, we need to respect python lexing order, `age` is defined after `younger_brother_age`,
+so we can't reference it
+
+
+More is coming, actually more is still undocumented!
```

### Comparing `exodia-1.0.4/exodia/bases.py` & `exodia-1.0.5/exodia/bases.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,42 +10,57 @@
         if cls == Base:
             raise ex.ExodiaException(
                 "Can't instantiate Base directly, You must subclass it"
             )
 
         return super().__new__(cls)
 
-    def _get_valid_attrs(self):
+    def __init__(self, **kwargs):
+        self._validate_kwargs(kwargs)
+
+    def _get_valid_fields(self):
         result = {}
 
         for key, value in self.__class__.__dict__.items():
             if isinstance(value, ex.Field):
                 result[key] = value
 
         return result
 
     def _validate_kwargs(self, kwargs):
         errors = []
         unknown_attrs = []
-        valid_attrs = self._get_valid_attrs()
+        valid_fields = self._get_valid_fields()
+        valid_attrs = {key: kwargs.get(key) for key in valid_fields.keys()}
 
         for key, value in kwargs.items():
-            if not valid_attrs.get(key):
+            if not valid_fields.get(key):
                 unknown_attrs.append(key)
 
-        for arg in unknown_attrs:
-            error = ex.ExodiaException("unexpected argument {arg}".format(arg=arg))
+        for attr in unknown_attrs:
+            error = ex.ExodiaException("unexpected attribute {attr}".format(attr=attr))
             errors.append(error)
 
+        for key, field in valid_fields.items():
+            value = valid_attrs.get(key)
+            try:
+                field._run_validators(value, key, self)
+            except ex.ExodiaException as e:
+                errors += [e]
+
+            self.post_field_validation(key, value)
+
+        try:
+            self.validate(valid_attrs)
+        except AssertionError as e:
+            errors.append(ex.ExodiaException(*e.args))
+        except ex.ExodiaException as e:
+            errors.append(e)
+
         if errors:
             raise ex.ExodiaException(errors)
 
-        for key, field in valid_attrs.items():
-            value = kwargs.get(key)
-            field._run_validators(value, key, self)
-            self.post_field_validation(key, value)
+    def validate(self, attrs):
+        pass
 
     def post_field_validation(self, field, value):
         setattr(self, field, value)
-
-    def __init__(self, **kwargs):
-        self._validate_kwargs(kwargs)
```

### Comparing `exodia-1.0.4/exodia/exceptions.py` & `exodia-1.0.5/exodia/exceptions.py`

 * *Files identical despite different names*

### Comparing `exodia-1.0.4/exodia/fields.py` & `exodia-1.0.5/exodia/fields.py`

 * *Files identical despite different names*

### Comparing `exodia-1.0.4/exodia/validators.py` & `exodia-1.0.5/exodia/validators.py`

 * *Files identical despite different names*

### Comparing `exodia-1.0.4/tests/test_instance_creation.py` & `exodia-1.0.5/tests/test_instance_creation.py`

 * *Files identical despite different names*

### Comparing `exodia-1.0.4/tests/test_validation.py` & `exodia-1.0.5/tests/test_validation.py`

 * *Files 20% similar despite different names*

```diff
@@ -90,17 +90,45 @@
 def test_ref():
     class Person(ex.Base):
         age = ex.Integer().required()
         younger_brother_age = (
             ex.Integer()
             .ref(
                 age,
-                lambda my_age, brother_age: my_age > brother_age,
+                lambda younger_age, age: age > younger_age,
                 "younger_brother can't be older!",
             )
             .required()
         )
 
-    Person(age=25, younger_brother_age=90)
+    Person(age=25, younger_brother_age=20)
 
     with pytest.raises(ex.ExodiaException):
-        Person(age=25, younger_brother_age=20)
+        Person(age=25, younger_brother_age=90)
+
+
+def test_ref_with_string_field():
+    class Person(ex.Base):
+        age = ex.Integer().required()
+        younger_brother = (
+            ex.Integer()
+            .ref("age", lambda younger_age, age: age > younger_age)
+            .required()
+        )
+
+    with pytest.raises(ex.ExodiaException):
+        Person(age=25, younger_brother=30)
+
+
+def test_validate_method():
+    class Person(ex.Base):
+        age = ex.Integer().required()
+        younger_brother_age = ex.Integer().required()
+
+        def validate(self, attrs):
+            # no need to check if age in attrs, you can't get into this step
+            # without providing both because both are required
+            # any assertion errors are transfored into ex.ExodiaException instances
+            assert attrs["age"] > attrs["younger_brother_age"]
+
+    with pytest.raises(ex.ExodiaException):
+        Person(age=25, younger_brother_age=30)
```

