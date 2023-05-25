# Comparing `tmp/lecroyscope-0.0.5.tar.gz` & `tmp/lecroyscope-1.0.0.tar.gz`

## Comparing `lecroyscope-0.0.5.tar` & `lecroyscope-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/.github/workflows/build-test.yml
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/src/lecroyscope/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/src/lecroyscope/version.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/src/lecroyscope/control/__init__.py
--rw-r--r--   0        0        0     5950 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/src/lecroyscope/control/scope.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/src/lecroyscope/reading/__init__.py
--rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/src/lecroyscope/reading/file.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/src/lecroyscope/reading/header.py
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/src/lecroyscope/reading/trace.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/src/lecroyscope/reading/trace_group.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/src/lecroyscope/writing/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/src/lecroyscope/writing/root/__init__.py
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/src/lecroyscope/writing/root/tree.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/tests/test_header.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/tests/test_read.py
--rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/tests/test_trace.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/tests/test_trace_group.py
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/tests/test_writing_root.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/tests/files/header.trc
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/tests/files/pulse.trc
--rw-r--r--   0        0        0    20757 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/tests/files/pulse_sequence.trc
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/LICENSE
--rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/README.md
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 lecroyscope-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/.github/workflows/build-test.yml
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/src/lecroyscope/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/src/lecroyscope/version.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/src/lecroyscope/control/__init__.py
+-rw-r--r--   0        0        0     5950 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/src/lecroyscope/control/scope.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/src/lecroyscope/reading/__init__.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/src/lecroyscope/reading/file.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/src/lecroyscope/reading/header.py
+-rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/src/lecroyscope/reading/trace.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/src/lecroyscope/reading/trace_group.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/src/lecroyscope/writing/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/src/lecroyscope/writing/root/__init__.py
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/src/lecroyscope/writing/root/tree.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/tests/test_header.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/tests/test_read.py
+-rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/tests/test_trace.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/tests/test_trace_group.py
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/tests/test_writing_root.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/tests/files/header.trc
+-rw-r--r--   0        0        0   200361 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/tests/files/issue_1.trc
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/tests/files/pulse.trc
+-rw-r--r--   0        0        0    20757 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/tests/files/pulse_sequence.trc
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/README.md
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 lecroyscope-1.0.0/PKG-INFO
```

### Comparing `lecroyscope-0.0.5/.github/workflows/build-test.yml` & `lecroyscope-1.0.0/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `lecroyscope-0.0.5/.github/workflows/python-publish.yml` & `lecroyscope-1.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `lecroyscope-0.0.5/src/lecroyscope/control/scope.py` & `lecroyscope-1.0.0/src/lecroyscope/control/scope.py`

 * *Files identical despite different names*

### Comparing `lecroyscope-0.0.5/src/lecroyscope/reading/file.py` & `lecroyscope-1.0.0/src/lecroyscope/reading/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 def read(
     filename_or_bytes: str | PathLike[str] | bytes, header_only: bool = False
 ) -> tuple[dict[str, str | int | float], numpy.ndarray, numpy.ndarray]:
     with open(filename_or_bytes, "r+b") if not isinstance(
         filename_or_bytes, bytes
     ) else BytesIO(filename_or_bytes) as f:
-
         wavedesc_bytes = b"WAVEDESC"
         # find "WAVEDESC" and skip those bytes
         if isinstance(filename_or_bytes, bytes):
             f.read(filename_or_bytes.find(wavedesc_bytes))
         else:
             # https://docs.python.org/3/library/mmap.html
             mm = mmap.mmap(f.fileno(), 0)
@@ -108,16 +107,19 @@
                 # skip user text
                 f.read(header["user_text"])
 
             trigger_times = numpy.frombuffer(
                 f.read(int(header["trig_time_array"])), dtype=numpy.float64
             )
 
+            number_of_bytes_to_read = (
+                int(header["wave_array_count"]) * values_type().itemsize
+            )
             values = numpy.frombuffer(
-                f.read(int(header["wave_array_count"])), dtype=values_type
+                f.read(number_of_bytes_to_read), dtype=values_type
             )
         else:
             trigger_times = numpy.array([], dtype=numpy.float64)
             values = numpy.array([], dtype=values_type)
 
         trigger_times = trigger_times.reshape((2, -1), order="F")
         if header["subarray_count"] > 1:
```

### Comparing `lecroyscope-0.0.5/src/lecroyscope/reading/header.py` & `lecroyscope-1.0.0/src/lecroyscope/reading/header.py`

 * *Files identical despite different names*

### Comparing `lecroyscope-0.0.5/src/lecroyscope/reading/trace.py` & `lecroyscope-1.0.0/src/lecroyscope/reading/trace.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,18 @@
 
         # compute time values
         self._time = (
             numpy.arange(self._voltage.shape[-1]) * self.header["horiz_interval"]
             + self.header["horiz_offset"]
         )
 
+        assert (
+            self._voltage.shape[-1] == self._time.shape[-1]
+        ), "Time and voltage arrays must have the same length"
+
     def __len__(self):
         if not self._header.sequence:
             return 1
         return len(self._voltage)
 
     def __iter__(self):
         if len(self) == 1:
```

### Comparing `lecroyscope-0.0.5/src/lecroyscope/reading/trace_group.py` & `lecroyscope-1.0.0/src/lecroyscope/reading/trace_group.py`

 * *Files identical despite different names*

### Comparing `lecroyscope-0.0.5/src/lecroyscope/writing/root/tree.py` & `lecroyscope-1.0.0/src/lecroyscope/writing/root/tree.py`

 * *Files identical despite different names*

### Comparing `lecroyscope-0.0.5/tests/test_header.py` & `lecroyscope-1.0.0/tests/test_header.py`

 * *Files identical despite different names*

### Comparing `lecroyscope-0.0.5/tests/test_read.py` & `lecroyscope-1.0.0/tests/test_read.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,16 +51,20 @@
     assert_array_equal(values_from_file, values_from_bytes)
     assert_array_equal(trigger_times_from_file, trigger_times_from_bytes)
     assert header_from_file == header_from_bytes
 
 
 def test_read_data_from_file():
     for filename, shape in zip(
-        [files_path / "pulse.trc", files_path / "pulse_sequence.trc"],
-        [(251,), (20, 251)],
+        [
+            files_path / "pulse.trc",
+            files_path / "pulse_sequence.trc",
+            files_path / "issue_1.trc",
+        ],
+        [(502,), (20, 502), (100002,)],
     ):
         (
             header_from_file,
             trigger_times_from_file,
             values_from_file,
         ) = lecroyscope.reading.read(filename, header_only=False)
         assert values_from_file.shape == shape
```

### Comparing `lecroyscope-0.0.5/tests/test_trace.py` & `lecroyscope-1.0.0/tests/test_trace.py`

 * *Files 10% similar despite different names*

```diff
@@ -86,28 +86,32 @@
 
         trace = lecroyscope.Trace(tmp_file)
         assert trace.channel == channel
 
 
 def test_read_trace_from_file():
     for filename, shape, length, sequence in zip(
-        [files_path / "pulse.trc", files_path / "pulse_sequence.trc"],
-        [(251,), (20, 251)],
-        [1, 20],
-        [False, True],
+        [
+            files_path / "pulse.trc",
+            files_path / "pulse_sequence.trc",
+            files_path / "issue_1.trc",
+        ],
+        [(502,), (20, 502), (100002,)],
+        [1, 20, 1],
+        [False, True, False],
     ):
         trace = lecroyscope.Trace(filename)
         assert len(trace) == length
         assert trace.header_only is False
         assert trace.sequence == sequence
         assert trace.voltage.shape == shape
-        assert trace.time.shape == (251,)
+        assert trace.time.shape == shape[-1:]
         assert (trace.voltage.shape[-1],) == trace.time.shape
 
-        if not sequence:
+        if filename == files_path / "pulse.trc":
             # check voltage and time scaling is done properly
             # test against signal which consists of ~ 0V baseline + sharp pulse at trigger time
             # first bins should be ~ 0V since we are on the region before pulse
             assert pytest.approx(np.mean(trace.voltage[0:100])) == 0.0057997689768671985
             # time of max voltage value should be very close to trigger time (0 seconds)
             assert (
                 pytest.approx(trace.time[np.argmax(trace.y)]) == 4.254989846811945e-09
```

### Comparing `lecroyscope-0.0.5/tests/test_trace_group.py` & `lecroyscope-1.0.0/tests/test_trace_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
         filenames.append(tmp_file)
 
     # check glob works
     for trace_group in [
         lecroyscope.TraceGroup(*filenames),
         lecroyscope.TraceGroup(tmp_path / "C*Trace00001.trc"),
     ]:
-
         for i, trace in enumerate(trace_group):
             assert isinstance(trace, lecroyscope.Trace)
             # this checks sorting too! (glob order is not the same across platforms)
             assert trace.channel == channels[i]
             np.testing.assert_array_equal(trace.time, trace_group.time)
 
         assert len(trace_group) == len(channels)
```

### Comparing `lecroyscope-0.0.5/tests/test_writing_root.py` & `lecroyscope-1.0.0/tests/test_writing_root.py`

 * *Files identical despite different names*

### Comparing `lecroyscope-0.0.5/tests/files/pulse.trc` & `lecroyscope-1.0.0/tests/files/pulse.trc`

 * *Files identical despite different names*

### Comparing `lecroyscope-0.0.5/tests/files/pulse_sequence.trc` & `lecroyscope-1.0.0/tests/files/pulse_sequence.trc`

 * *Files identical despite different names*

### Comparing `lecroyscope-0.0.5/.gitignore` & `lecroyscope-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lecroyscope-0.0.5/README.md` & `lecroyscope-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `lecroyscope-0.0.5/pyproject.toml` & `lecroyscope-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 [build-system]
 requires = [
     "hatchling",
 ]
 build-backend = "hatchling.build"
 
-
 [project]
 name = "lecroyscope"
 authors = [
     { name = "Luis Antonio Obis Aparicio", email = "luis.antonio.obis@gmail.com" },
 ]
+requires-python = ">=3.8"
 description = "An unofficial Python package 🐍📦 to interface with Teledyne LeCroy oscilloscopes and read binary trace files (.trc)"
 readme = "README.md"
-requires-python = ">=3.8"
+license = "BSD-3-Clause"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
+keywords = [
+    "lecroy",
+    "scope",
+    "oscilloscope",
+    "vxi11",
+    "binary",
+    "trc",
+]
 dependencies = [
     "numpy",
     "python-vxi11",
 ]
 dynamic = [
     "version",
 ]
```

### Comparing `lecroyscope-0.0.5/PKG-INFO` & `lecroyscope-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: lecroyscope
-Version: 0.0.5
+Version: 1.0.0
 Summary: An unofficial Python package 🐍📦 to interface with Teledyne LeCroy oscilloscopes and read binary trace files (.trc)
 Project-URL: Download, https://github.com/lobis/lecroy-scope/releases
 Project-URL: Homepage, https://github.com/lobis/lecroy-scope
 Project-URL: Bug Tracker, https://github.com/lobis/lecroy-scope/issues
 Author-email: Luis Antonio Obis Aparicio <luis.antonio.obis@gmail.com>
+License-Expression: BSD-3-Clause
 License-File: LICENSE
+Keywords: binary,lecroy,oscilloscope,scope,trc,vxi11
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: numpy
 Requires-Dist: python-vxi11
 Provides-Extra: dev
 Requires-Dist: awkward; extra == 'dev'
```

