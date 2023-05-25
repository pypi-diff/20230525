# Comparing `tmp/looseversion-1.1.2.tar.gz` & `tmp/looseversion-1.2.0.tar.gz`

## Comparing `looseversion-1.1.2.tar` & `looseversion-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 looseversion-1.1.2/CHANGES.md
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 looseversion-1.1.2/tests.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 looseversion-1.1.2/tox.ini
--rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 looseversion-1.1.2/src/looseversion/__init__.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 looseversion-1.1.2/src/looseversion/__init__.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 looseversion-1.1.2/src/looseversion/py.typed
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 looseversion-1.1.2/.gitignore
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 looseversion-1.1.2/LICENSE
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 looseversion-1.1.2/README.md
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 looseversion-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 looseversion-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 looseversion-1.2.0/CHANGES.md
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 looseversion-1.2.0/tests.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 looseversion-1.2.0/tox.ini
+-rw-r--r--   0        0        0     8555 2020-02-02 00:00:00.000000 looseversion-1.2.0/src/looseversion/__init__.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 looseversion-1.2.0/src/looseversion/__init__.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 looseversion-1.2.0/src/looseversion/py.typed
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 looseversion-1.2.0/.gitignore
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 looseversion-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 looseversion-1.2.0/README.md
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 looseversion-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 looseversion-1.2.0/PKG-INFO
```

### Comparing `looseversion-1.1.2/CHANGES.md` & `looseversion-1.2.0/CHANGES.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 ## Releases
 
+### 1.2.0 (25 May 2023)
+
+- 2023.05.25
+  - Test on Python 3.12
+  - Enable installation on Python 2+
+  - Ensure consistent semantics between Python 2 and 3
+
 ### 1.1.2 (22 Feb 2023)
 
 - 2023.02.22
   - Revert unintended change in internal version representation
 
 ### 1.1.1 (19 Feb 2023)
```

### Comparing `looseversion-1.1.2/tests.py` & `looseversion-1.2.0/tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,46 +35,72 @@
     assert (orig1 < vend2) == (v1 < v2)
     assert (orig1 > vend2) == (v1 > v2)
     assert (orig1 <= vend2) == (v1 <= v2)
     assert (orig1 >= vend2) == (v1 >= v2)
 
 
 # Adapted from Cpython:Lib/distutils/tests/test_version.py
-@pytest.mark.parametrize("v1,v2,result",
-    [('1.5.1', '1.5.2b2', -1),
-     ('161', '3.10a', 1),
-     ('8.02', '8.02', 0),
-     ('3.4j', '1996.07.12', -1),
-     ('3.2.pl0', '3.1.1.6', 1),
-     ('2g6', '11g', -1),
-     ('0.960923', '2.2beta29', -1),
-     ('1.13++', '5.5.kw', -1)])
+@pytest.mark.parametrize(
+    "v1,v2,result",
+    [
+        ("1.5.1", "1.5.2b2", -1),
+        ("161", "3.10a", 1),
+        ("8.02", "8.02", 0),
+        ("3.4j", "1996.07.12", -1),
+        ("3.2.pl0", "3.1.1.6", 1),
+        ("2g6", "11g", -1),
+        ("0.960923", "2.2beta29", -1),
+        ("1.13++", "5.5.kw", -1),
+    ],
+)
 def test_cmp(v1, v2, result):
     loosev1 = lv.LooseVersion(v1)
     loosev2 = lv.LooseVersion(v2)
     assert loosev1._cmp(loosev2) == result
     assert loosev1._cmp(v2) == result
     assert loosev2._cmp(loosev1) == -result
     assert loosev2._cmp(v1) == -result
     assert loosev1._cmp(object()) == NotImplemented
     assert loosev2._cmp(object()) == NotImplemented
 
 
-@pytest.mark.parametrize('vstring,version',
+@pytest.mark.parametrize(
+    "vstring,version",
     [
-        ('1.5.1', [1, 5, 1]),
-        ('1.5.2b2', [1, 5, 2, 'b', 2]),
-        ('161', [161]),
-        ('3.10a', [3, 10, 'a']),
-        ('1.13++', [1, 13, '++']),
+        ("1.5.1", [1, 5, 1]),
+        ("1.5.2b2", [1, 5, 2, "b", 2]),
+        ("161", [161]),
+        ("3.10a", [3, 10, "a"]),
+        ("1.13++", [1, 13, "++"]),
     ],
 )
 def test_split(vstring, version):
     # Regression test to ensure we don't accidentally break parsing (again)
     # This can be changed if the version representation changes
     v = lv.LooseVersion(vstring)
     assert v.vstring == vstring
     assert v.version == version
 
 
-if __name__ == '__main__':
+@pytest.mark.parametrize(
+    "v1,v2,result",
+    [
+        ("0.3@v0.3", "0.3.1@v0.3.1", 1),
+        ("0.3.1@v0.3.1", "0.3@v0.3", -1),
+        ("13.0-beta3", "13.0.1", 1),
+        ("13.0.1", "13.0-beta3", -1),
+    ],
+)
+def test_py2_rules(v1, v2, result):
+    """Python 2 did allow strings and numbers to be compared.
+    Verify consistent, generally unintuitive behavior.
+    """
+    loosev1 = lv.LooseVersion(v1)
+    loosev2 = lv.LooseVersion(v2)
+    assert loosev1._cmp(loosev2) == result
+    assert loosev1._cmp(v2) == result
+    assert loosev2._cmp(loosev1) == -result
+    assert loosev2._cmp(v1) == -result
+
+
+if __name__ == "__main__":
     sys.exit(pytest.main([__file__] + sys.argv[1:]))
```

### Comparing `looseversion-1.1.2/src/looseversion/__init__.py` & `looseversion-1.2.0/src/looseversion/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,14 @@
     an equivalent string -- ie. one that will generate an equivalent
     version number instance)
   * __repr__ generates Python code to recreate the version number instance
   * _cmp compares the current instance with either another instance
     of the same class or a string (which will be parsed to an instance
     of the same class, thus must follow the same rules)
 """
-from __future__ import annotations
-
 import re
 import sys
 
 # The rules according to Greg Stein:
 # 1) a version number has 1 or more numbers separated by a period or by
 #    sequences of letters. If only periods, then these are compared
 #    left-to-right to determine an ordering.
@@ -82,16 +80,34 @@
 # wrong, it's because the simple, obvious design doesn't match my
 # complicated, hairy expectations for real-world version numbers.  It
 # would be a snap to fix the test suite to say, "Yep, LooseVersion does
 # the Right Thing" (ie. the code matches the conception).  But I'd rather
 # have a conception that matches common notions about version numbers.
 
 
-class LooseVersion:
+if sys.version_info >= (3,):
+
+    class _Py2Int(int):
+        """Integer object that compares < any string"""
+
+        def __gt__(self, other):
+            if isinstance(other, str):
+                return False
+            return super().__gt__(other)
+
+        def __lt__(self, other):
+            if isinstance(other, str):
+                return True
+            return super().__lt__(other)
+
+else:
+    _Py2Int = int
+
 
+class LooseVersion(object):
     """Version numbering for anarchists and software realists.
     Implements the standard interface for version number classes as
     described above.  A version number consists of a series of numbers,
     separated by either periods or strings of letters.  When comparing
     version numbers, the numeric components will be compared
     numerically, and the alphabetic components lexically.  The following
     are all valid version numbers, in no particular order:
@@ -115,89 +131,85 @@
 
     In fact, there is no such thing as an invalid version number under
     this scheme; the rules for comparison are simple and predictable,
     but may not always give the results you want (for some definition
     of "want").
     """
 
-    component_re: re.Pattern[str] = re.compile(r"(\d+ | [a-z]+ | \.)", re.VERBOSE)
-    vstring: str
-    version: list[int | str]
+    component_re = re.compile(r"(\d+ | [a-z]+ | \.)", re.VERBOSE)
 
-    def __init__(self, vstring: str | None = None):
+    def __init__(self, vstring=None):
         if vstring:
             self.parse(vstring)
 
-    def __eq__(self, other: object) -> bool:
+    def __eq__(self, other):
         c = self._cmp(other)
         if c is NotImplemented:
             return NotImplemented
         return c == 0
 
-    def __lt__(self, other: object) -> bool:
+    def __lt__(self, other):
         c = self._cmp(other)
         if c is NotImplemented:
             return NotImplemented
         return c < 0
 
-    def __le__(self, other: object) -> bool:
+    def __le__(self, other):
         c = self._cmp(other)
         if c is NotImplemented:
             return NotImplemented
         return c <= 0
 
-    def __gt__(self, other: object) -> bool:
+    def __gt__(self, other):
         c = self._cmp(other)
         if c is NotImplemented:
             return NotImplemented
         return c > 0
 
-    def __ge__(self, other: object) -> bool:
+    def __ge__(self, other):
         c = self._cmp(other)
         if c is NotImplemented:
             return NotImplemented
         return c >= 0
 
-    def parse(self, vstring: str) -> None:
+    def parse(self, vstring):
         # I've given up on thinking I can reconstruct the version string
         # from the parsed tuple -- so I just store the string here for
         # use by __str__
         self.vstring = vstring
-        components: list[str | int] = [
-            x for x in self.component_re.split(vstring) if x and x != "."
-        ]
+        components = [x for x in self.component_re.split(vstring) if x and x != "."]
         for i, obj in enumerate(components):
             try:
-                components[i] = int(obj)
+                components[i] = _Py2Int(obj)
             except ValueError:
                 pass
 
         self.version = components
 
-    def __str__(self) -> str:
+    def __str__(self):
         return self.vstring
 
-    def __repr__(self) -> str:
+    def __repr__(self):
         return "LooseVersion ('%s')" % str(self)
 
-    def _cmp(self, other: object) -> int:
+    def _cmp(self, other):
         other = self._coerce(other)
         if other is NotImplemented:
             return NotImplemented
 
         if self.version == other.version:
             return 0
         if self.version < other.version:
             return -1
         if self.version > other.version:
             return 1
         return NotImplemented
 
     @staticmethod
-    def _coerce(other: object) -> LooseVersion:
+    def _coerce(other):
         if isinstance(other, LooseVersion):
             return other
         elif isinstance(other, str):
             return LooseVersion(other)
         elif "distutils" in sys.modules:
             # Using this check to avoid importing distutils and suppressing the warning
             try:
```

### Comparing `looseversion-1.1.2/.gitignore` & `looseversion-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `looseversion-1.1.2/LICENSE` & `looseversion-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `looseversion-1.1.2/README.md` & `looseversion-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `looseversion-1.1.2/pyproject.toml` & `looseversion-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "looseversion"
 maintainers = [{name = "Chris Markiewicz", email = "effigies@gmail.com"}]
-version = "1.1.2"
+version = "1.2.0"
 description = "Version numbering for anarchists and software realists"
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 6 - Mature",
     "License :: OSI Approved :: Python Software Foundation License",
 ]
 urls = {Homepage = "https://github.com/effigies/looseversion"}
-requires-python = ">=3"
 
 [tool.hatch.build]
 exclude = [".github"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/looseversion"]
```

### Comparing `looseversion-1.1.2/PKG-INFO` & `looseversion-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: looseversion
-Version: 1.1.2
+Version: 1.2.0
 Summary: Version numbering for anarchists and software realists
 Project-URL: Homepage, https://github.com/effigies/looseversion
 Maintainer-email: Chris Markiewicz <effigies@gmail.com>
 License: PYTHON SOFTWARE FOUNDATION LICENSE VERSION 2
         --------------------------------------------
         
         1. This LICENSE AGREEMENT is between the Python Software Foundation
@@ -52,15 +52,14 @@
         8. By copying, installing or otherwise using Python, Licensee
         agrees to be bound by the terms and conditions of this License
         Agreement.
 License-File: LICENSE
 Classifier: Development Status :: 6 - Mature
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # looseversion - Version numbering for anarchists and software realists
 
 A backwards/forwards-compatible fork of `distutils.version.LooseVersion`,
 for times when PEP-440 isn't what you need.
```

