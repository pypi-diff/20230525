# Comparing `tmp/captif-slp-0.8.tar.gz` & `tmp/captif-slp-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captif-slp-0.8.tar", max compression
+gzip compressed data, was "captif-slp-0.9.tar", max compression
```

## Comparing `captif-slp-0.8.tar` & `captif-slp-0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1084 2022-06-08 04:18:51.990166 captif-slp-0.8/LICENSE
--rw-r--r--   0        0        0     9601 2022-06-08 04:18:51.990166 captif-slp-0.8/README.md
--rw-r--r--   0        0        0       82 2022-06-08 04:18:51.990166 captif-slp-0.8/captif_slp/__init__.py
--rw-r--r--   0        0        0     2876 2022-06-08 04:18:51.990166 captif-slp-0.8/captif_slp/process.py
--rw-r--r--   0        0        0     2509 2022-06-08 04:18:51.990166 captif-slp-0.8/captif_slp/signal.py
--rw-r--r--   0        0        0    13970 2022-06-08 04:18:51.990166 captif-slp-0.8/captif_slp/slp.py
--rw-r--r--   0        0        0      591 2022-06-08 04:18:51.990166 captif-slp-0.8/pyproject.toml
--rw-r--r--   0        0        0    10537 2022-06-08 04:18:57.322404 captif-slp-0.8/setup.py
--rw-r--r--   0        0        0    10323 2022-06-08 04:18:57.323221 captif-slp-0.8/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-06-08 23:51:25.614740 captif-slp-0.9/LICENSE
+-rw-r--r--   0        0        0     9601 2022-06-08 23:51:25.614740 captif-slp-0.9/README.md
+-rw-r--r--   0        0        0       97 2022-06-08 23:51:25.618740 captif-slp-0.9/captif_slp/__init__.py
+-rw-r--r--   0        0        0     2864 2022-06-08 23:51:25.618740 captif-slp-0.9/captif_slp/process.py
+-rw-r--r--   0        0        0     2602 2022-06-08 23:51:25.618740 captif-slp-0.9/captif_slp/signal.py
+-rw-r--r--   0        0        0    15940 2022-06-08 23:51:25.618740 captif-slp-0.9/captif_slp/slp.py
+-rw-r--r--   0        0        0      614 2022-06-08 23:51:25.618740 captif-slp-0.9/pyproject.toml
+-rw-r--r--   0        0        0    10537 2022-06-08 23:51:29.876893 captif-slp-0.9/setup.py
+-rw-r--r--   0        0        0    10323 2022-06-08 23:51:29.877631 captif-slp-0.9/PKG-INFO
```

### Comparing `captif-slp-0.8/LICENSE` & `captif-slp-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `captif-slp-0.8/README.md` & `captif-slp-0.9/README.md`

 * *Files identical despite different names*

### Comparing `captif-slp-0.8/captif_slp/process.py` & `captif-slp-0.9/captif_slp/process.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import os
 import psutil
 import multiprocessing
 import numpy as np
-import pandas as pd
-import matplotlib.pyplot as plt
 from pathlib import Path
 from platform import system
 from typing import List, Optional, Union
 from unsync import unsync
 
 from .slp import Reading
 
@@ -46,15 +44,17 @@
             parallel=False,
             alpha=alpha,
             start_mm=start_mm,
             end_mm=end_mm,
             detect_plates=detect_plates,
         )
         result, trace = reading.result()
-        result["trace"] = trace  # TODO: fix this for when evaluation_length_m is not None
+        result[
+            "trace"
+        ] = trace  # TODO: fix this for when evaluation_length_m is not None
         results[path] = result
 
     return results
 
 
 def process_generic_files(
     paths: List[Union[str, Path]],
@@ -64,28 +64,29 @@
     alpha: int = 3,
     start_mm: Optional[float] = None,
     end_mm: Optional[float] = None,
     detect_plates: bool = False,
 ):
     try:
         paths = [pp.as_posix() for pp in paths]
-    except:
+    except Exception:
         pass
 
     tasks = [
         _process_files(
             pp.tolist(),
             segment_length_mm=segment_length_mm,
             target_sample_spacing_mm=target_sample_spacing_mm,
             evaluation_length_m=evaluation_length_m,
             alpha=alpha,
             start_mm=start_mm,
             end_mm=end_mm,
             detect_plates=detect_plates,
-        ) for pp in np.array_split(paths, CPU_COUNT)
+        )
+        for pp in np.array_split(paths, CPU_COUNT)
     ]
     results = [tt.result() for tt in tasks]
     results = {kk: vv for rr in results for kk, vv in rr.items()}
     results_ = []
     for kk, vv in results.items():
         pp = Path(kk)
         vv["folder"] = pp.parent.absolute().as_posix()
```

### Comparing `captif-slp-0.8/captif_slp/signal.py` & `captif-slp-0.9/captif_slp/signal.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import numpy as np
 import matplotlib.pyplot as plt
 
 from scipy import signal
 from functools import lru_cache
 
 
@@ -46,46 +45,52 @@
 
 
 def plot_filter_response(sos: np.array, fs: float):
     w, h = signal.sosfreqz(sos, worN=2000)
 
     fig, ax = plt.subplots()
     ax.plot((fs * 0.5 / np.pi) * w, abs(h))
-    ax.plot([0, 0.5 * fs], [np.sqrt(0.5), np.sqrt(0.5)], '--', label='sqrt(0.5)')
+    ax.plot([0, 0.5 * fs], [np.sqrt(0.5), np.sqrt(0.5)], "--", label="sqrt(0.5)")
 
-    ax.set_xlabel('Frequency (mm-1)')
-    ax.set_ylabel('Gain')
+    ax.set_xlabel("Frequency (mm-1)")
+    ax.set_ylabel("Gain")
     ax.grid(True)
-    ax.legend(loc='best')
+    ax.legend(loc="best")
 
     return fig, ax
 
 
 def generate_ba_filter_coefficients(
-    filter_type, sample_spacing_mm, normalise=True,
+    filter_type,
+    sample_spacing_mm,
+    normalise=True,
 ):
     if filter_type == "lowpass":
         b, a = build_lowpass_filter(sample_spacing_mm, "ba")
     if filter_type == "highpass":
         b, a = build_highpass_filter(sample_spacing_mm, "ba")
 
     if normalise:
-        a = a/b[0]
-        b = b/b[0]
+        a = a / b[0]
+        b = b / b[0]
 
     return b, a
 
 
 def generate_reference_filter_coefficients(normalise=True):
     filter_coefficients = []
     for filter_type in ["lowpass", "highpass"]:
         for sample_spacing_mm in [0.5, 1]:
             b, a = generate_ba_filter_coefficients(
-                filter_type, sample_spacing_mm, normalise,
+                filter_type,
+                sample_spacing_mm,
+                normalise,
+            )
+            filter_coefficients.append(
+                {
+                    "filter_type": filter_type,
+                    "sample_spacing_mm": sample_spacing_mm,
+                    "b": b.tolist(),
+                    "a": a.tolist(),
+                }
             )
-            filter_coefficients.append({
-                "filter_type": filter_type,
-                "sample_spacing_mm": sample_spacing_mm,
-                "b": b.tolist(),
-                "a": a.tolist(),
-            })
     return filter_coefficients
```

### Comparing `captif-slp-0.8/captif_slp/slp.py` & `captif-slp-0.9/captif_slp/slp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import pandas as pd
 import numpy as np
 from dataclasses import dataclass
 from pathlib import Path
 from typing import List, Optional, Tuple, Union
 
 from captif_data_structures.readers import TextureReader
@@ -62,109 +61,156 @@
 
 
 @dataclass
 class Reading:
     meta: Optional[dict]
     trace: pd.DataFrame
     resampled_trace: pd.DataFrame
-    segment_length_mm: int
     resampled_sample_spacing_mm: float
     alpha: int
-    evaluation_length_m: Optional[float] = None,
-    start_mm: Optional[float] = None,
-    end_mm: Optional[float] = None,
-    detect_plates: bool = False,
+    segment_length_mm: Optional[int] = None
+    segment_bins: Optional[list] = None
+    evaluation_length_m: Optional[float] = None
+    start_mm: Optional[float] = None
+    end_mm: Optional[float] = None
+    detect_plates: bool = False
 
     @classmethod
     def from_trace(
         cls,
         trace,
         meta=None,
         segment_length_mm: int = 100,
+        segment_bins: Optional[list] = None,
         target_sample_spacing_mm: float = 0.5,
         evaluation_length_m: Optional[float] = None,
         alpha: int = 3,
         start_mm: Optional[float] = None,
         end_mm: Optional[float] = None,
         detect_plates: bool = False,
     ):
+        if segment_bins is not None:
+            segment_length_mm = None
+
         if detect_plates and (start_mm is None) and (end_mm is None):
             start_mm, end_mm = find_plates(trace)
 
         trace = trim_trace(trace, start_mm, end_mm)
         trace["relative_height_mm_raw_trace"] = trace["relative_height_mm"]
 
         trace = append_dropout_column(trace)
         trace = apply_dropout_correction(trace)
 
         resampled_trace = build_resampled_trace(trace, target_sample_spacing_mm)
 
-        resampled_trace["relative_height_mm_no_spike_correction"] = resampled_trace["relative_height_mm"]
+        resampled_trace["relative_height_mm_no_spike_correction"] = resampled_trace[
+            "relative_height_mm"
+        ]
         resampled_trace = apply_spike_removal(resampled_trace, alpha=alpha)
 
-        resampled_trace["relative_height_mm_no_highpass_filter"] = resampled_trace["relative_height_mm"]
+        resampled_trace["relative_height_mm_no_highpass_filter"] = resampled_trace[
+            "relative_height_mm"
+        ]
         if evaluation_length_m is not None:
-            resampled_trace = apply_highpass_filter(resampled_trace, target_sample_spacing_mm)
+            resampled_trace = apply_highpass_filter(
+                resampled_trace, target_sample_spacing_mm
+            )
 
-        resampled_trace["relative_height_mm_no_lowpass_filter"] = resampled_trace["relative_height_mm"]
-        resampled_trace = apply_lowpass_filter(resampled_trace, target_sample_spacing_mm)
+        resampled_trace["relative_height_mm_no_lowpass_filter"] = resampled_trace[
+            "relative_height_mm"
+        ]
+        resampled_trace = apply_lowpass_filter(
+            resampled_trace, target_sample_spacing_mm
+        )
 
         return Reading(
-            meta, trace, resampled_trace, segment_length_mm, target_sample_spacing_mm,
-            alpha, evaluation_length_m, start_mm, end_mm, detect_plates
+            meta=meta,
+            trace=trace,
+            resampled_trace=resampled_trace,
+            resampled_sample_spacing_mm=target_sample_spacing_mm,
+            alpha=alpha,
+            segment_length_mm=segment_length_mm,
+            segment_bins=segment_bins,
+            evaluation_length_m=evaluation_length_m,
+            start_mm=start_mm,
+            end_mm=end_mm,
+            detect_plates=detect_plates,
         )
 
     @classmethod
     def from_file(
         cls,
         path: Union[str, Path],
         segment_length_mm: int = 100,
+        segment_bins: Optional[list] = None,
         target_sample_spacing_mm: float = 0.5,
         evaluation_length_m: Optional[float] = None,
         parallel: bool = True,
         alpha: int = 3,
         start_mm: Optional[float] = None,
         end_mm: Optional[float] = None,
         detect_plates: bool = False,
     ):
         meta, trace = load_reading(path, parallel=parallel)
         return cls.from_trace(
-            trace, meta, segment_length_mm, target_sample_spacing_mm,
-            evaluation_length_m, alpha, start_mm, end_mm, detect_plates,
+            trace=trace,
+            meta=meta,
+            segment_length_mm=segment_length_mm,
+            segment_bins=segment_bins,
+            target_sample_spacing_mm=target_sample_spacing_mm,
+            evaluation_length_m=evaluation_length_m,
+            alpha=alpha,
+            start_mm=start_mm,
+            end_mm=end_mm,
+            detect_plates=detect_plates,
         )
 
     @property
     def segments(self):
-        traces = zip(
-            extract_segment_traces_from_trace(self.trace, self.segment_length_mm),
-            extract_segment_traces_from_trace(self.resampled_trace, self.segment_length_mm),
+        segment_data = extract_segment_data(
+            trace=self.trace,
+            resampled_trace=self.resampled_trace,
+            segment_length_mm=self.segment_length_mm,
+            segment_bins=self.segment_bins,
         )
+
         segments_ = []
-        for ii, (segment_trace, resampled_segment_trace) in enumerate(traces):
-            segment_length = len(resampled_segment_trace) * self.resampled_sample_spacing_mm
-            if segment_length < (0.9 * self.segment_length_mm):
+        for ii, (
+            segment_trace,
+            resampled_segment_trace,
+            segment_length_mm,
+        ) in enumerate(segment_data):
+            n_points = len(resampled_segment_trace)
+            max_points = segment_length_mm / self.resampled_sample_spacing_mm
+            if (n_points / max_points) < 0.9:
                 continue
 
             # Apply slope correction if "spot" measurement:
-            resampled_segment_trace["relative_height_mm_no_slope_correction"] = \
-                resampled_segment_trace["relative_height_mm"]
+            resampled_segment_trace[
+                "relative_height_mm_no_slope_correction"
+            ] = resampled_segment_trace["relative_height_mm"]
             if self.evaluation_length_m is None:
-                resampled_segment_trace = apply_slope_correction(resampled_segment_trace)
+                resampled_segment_trace = apply_slope_correction(
+                    resampled_segment_trace
+                )
 
             evaluation_length_position_m = calculate_evaluation_length_position(
-                segment_trace["distance_mm"].min(), self.evaluation_length_m)
+                segment_trace["distance_mm"].min(), self.evaluation_length_m
+            )
 
-            segments_.append(Segment(
-                segment_no=ii,
-                trace=segment_trace,
-                resampled_trace=resampled_segment_trace,
-                segment_length_mm=self.segment_length_mm,
-                resampled_sample_spacing_mm=self.resampled_sample_spacing_mm,
-                evaluation_length_position_m=evaluation_length_position_m,
-            ))
+            segments_.append(
+                Segment(
+                    segment_no=ii,
+                    trace=segment_trace,
+                    resampled_trace=resampled_segment_trace,
+                    segment_length_mm=segment_length_mm,
+                    resampled_sample_spacing_mm=self.resampled_sample_spacing_mm,
+                    evaluation_length_position_m=evaluation_length_position_m,
+                )
+            )
         return segments_
 
     def msd(self) -> List[dict]:
         """Mean segment depths (MSD) for the segments making up the profile."""
         return [
             {
                 "segment_no": ss.segment_no,
@@ -201,15 +247,17 @@
         """
         Returns the Mean profile depth (MPD) results for each evaluation length as either
         a dict (if no evaluation length) or a DataFrame (if evaluation length provided),
         and the resampled trace as a list of dicts.
         """
         return (
             self.mpd(include_meta=True),
-            self.resampled_trace[["distance_mm", "relative_height_mm"]].to_dict("records"),
+            self.resampled_trace[["distance_mm", "relative_height_mm"]].to_dict(
+                "records"
+            ),
         )
 
 
 def append_meta(result, meta):
     for kk, vv in meta.items():
         result[kk] = vv
     return result
@@ -223,15 +271,15 @@
     if end_mm:
         trace = trace.loc[trace["distance_mm"] < end_mm]
 
     if start_mm:
         trace = trace.loc[trace["distance_mm"] >= start_mm]
         trace["distance_mm"] -= start_mm
         trace.reset_index(drop=True, inplace=True)
-    
+
     return trace
 
 
 def find_plates(trace: pd.DataFrame):
     yy = trace["relative_height_mm"].interpolate("pad")
     is_plate = yy > PLATE_THRESHOLD
 
@@ -241,41 +289,62 @@
     diff = is_plate.diff()
     diff.iloc[0] = False
 
     i_midpoint = int(np.ceil(len(trace) / 2))
 
     start_mm, end_mm = None, None
     try:
-        ii_start = trace.loc[:i_midpoint].loc[
-                diff.loc[:i_midpoint]
-            ].iloc[-1].name
+        ii_start = trace.loc[:i_midpoint].loc[diff.loc[:i_midpoint]].iloc[-1].name
         start_mm = trace.loc[ii_start, "distance_mm"] + PLATE_BUFFER
-    except:
+    except Exception:
         pass
 
     try:
-        ii_end = trace.loc[i_midpoint:].loc[
-                diff.loc[i_midpoint:]
-            ].iloc[0].name - 1
+        ii_end = trace.loc[i_midpoint:].loc[diff.loc[i_midpoint:]].iloc[0].name - 1
         end_mm = trace.loc[ii_end, "distance_mm"] - PLATE_BUFFER
-    except:
+    except Exception:
         pass
 
     return start_mm, end_mm
 
 
-def extract_segment_traces_from_trace(trace: pd.DataFrame, segment_length_mm: int):
-    bins = generate_trace_bins(trace, segment_length_mm)
+def extract_segment_traces_from_trace(trace: pd.DataFrame, segment_bins: list):
     yield from (
-        tt for _, tt in trace.groupby(
-            pd.cut(trace["distance_mm"], bins, include_lowest=True)
+        tt
+        for _, tt in trace.groupby(
+            pd.cut(trace["distance_mm"], segment_bins, include_lowest=True)
         )
     )
 
 
+def extract_segment_data(
+    trace: pd.DataFrame,
+    resampled_trace: pd.DataFrame,
+    segment_length_mm: Optional[int] = None,
+    segment_bins: Optional[list] = None,
+):
+    """
+    Extracts segment traces (original and resampled) from the reading and calculated the
+    resulting segment length of each segment. The segment data is zipped with each
+    element containing (trace, resampled_trace, segment_length_mm) for one segment.
+
+    """
+    if segment_bins is None and segment_length_mm is None:
+        raise ValueError("at least one of segment_length_m or segment_bins must be set")
+
+    if segment_bins is None:
+        segment_bins = generate_trace_bins(trace, segment_length_mm)
+
+    return zip(
+        extract_segment_traces_from_trace(trace, segment_bins),
+        extract_segment_traces_from_trace(resampled_trace, segment_bins),
+        np.diff(segment_bins),  # segment_length_m of each segment
+    )
+
+
 def generate_trace_bins(trace: pd.DataFrame, bin_width_mm: float):
     return np.arange(0, trace["distance_mm"].max() + bin_width_mm, bin_width_mm)
 
 
 def build_resampled_trace(trace: pd.DataFrame, target_sample_spacing_mm: float):
     if calculate_trace_sample_spacing(trace) == target_sample_spacing_mm:
         return trace.copy()
@@ -285,15 +354,17 @@
     trace.loc[0, "group"] = 1 if g0 == 0 else g0
 
     resampled_trace = trace[["group", "relative_height_mm"]].groupby("group").mean()
     resampled_trace["distance_mm"] = resampled_trace.index * target_sample_spacing_mm
     resampled_trace.reset_index(drop=True, inplace=True)
     trace.drop(columns=["group"], inplace=True)
 
-    resampled_trace["relative_height_mm"] = resampled_trace["relative_height_mm"].round(6)
+    resampled_trace["relative_height_mm"] = resampled_trace["relative_height_mm"].round(
+        6
+    )
     return resampled_trace
 
 
 def load_reading(path: Union[str, Path], parallel: bool = True):
     meta, table_rows, _ = TextureReader.load(path, parallel=parallel)
     trace = pd.DataFrame(table_rows).sort_values("distance_mm").reset_index(drop=True)
     return meta, trace
@@ -316,18 +387,17 @@
 def calculate_trace_sample_spacing(trace: pd.DataFrame) -> float:
     return trace["distance_mm"].diff().mean()
 
 
 def append_spike_column(trace: pd.DataFrame, alpha: float = 3):
     threshold = round(alpha * calculate_trace_sample_spacing(trace), 6)
     ss = (trace["relative_height_mm"].diff().abs() >= threshold).to_numpy()[1:]
-    trace["spike"] = (
-        np.insert(ss, 0, False) |  # spikes in forward direction
-        np.append(ss, False)  # spikes in reverse direction
-    )
+    trace["spike"] = np.insert(ss, 0, False) | np.append(  # spikes in forward direction
+        ss, False
+    )  # spikes in reverse direction
     return trace
 
 
 def apply_spike_removal(trace: pd.DataFrame, alpha: float = 3):
     trace = append_spike_column(trace, alpha)
     trace.loc[trace["spike"], "relative_height_mm"] = None
     return apply_dropout_correction(trace)
@@ -355,27 +425,29 @@
 
 def dropout_correction_start_end(trace: pd.DataFrame):
     yy = trace["relative_height_mm"].copy()
     valid_index = yy.loc[~yy.isna()].index
 
     # Fill start of trace if it contains dropouts:
     if np.isnan(yy.iloc[0]):
-        yy.loc[:valid_index[0]] = yy.loc[valid_index[0]]
+        yy.loc[: valid_index[0]] = yy.loc[valid_index[0]]
 
     # Fill end of trace if it contains dropouts:
     if np.isnan(yy.iloc[-1]):
-        yy.loc[valid_index[-1]:] = yy.loc[valid_index[-1]]
+        yy.loc[valid_index[-1] :] = yy.loc[valid_index[-1]]
 
     trace["relative_height_mm"] = yy
     return trace
 
 
 def dropout_correction_interpolate(trace: pd.DataFrame):
-    return (trace
-        .set_index("distance_mm", drop=True)  # so distance weighing can be used in interpolation
+    return (
+        trace.set_index(
+            "distance_mm", drop=True
+        )  # so distance weighing can be used in interpolation
         .interpolate(method="index", limit_area="inside")
         .reset_index(drop=False)  # move distance back to a column
     )
 
 
 def calculate_msd(trace: pd.DataFrame) -> float:
     n_samples = len(trace)
@@ -384,15 +456,16 @@
     peak2 = trace.iloc[i_midpoint:]["relative_height_mm"].max()
     peak_average = (peak1 + peak2) / 2
     profile_average = trace["relative_height_mm"].mean()
     return peak_average - profile_average
 
 
 def calculate_evaluation_length_position(
-    segment_start_position_mm: float,
-    evaluation_length_m: Optional[float] = None
+    segment_start_position_mm: float, evaluation_length_m: Optional[float] = None
 ) -> float:
     if evaluation_length_m is None:
         return None
 
-    position_no = int(np.floor(segment_start_position_mm / (evaluation_length_m * 1000)))
+    position_no = int(
+        np.floor(segment_start_position_mm / (evaluation_length_m * 1000))
+    )
     return (position_no + 1) * evaluation_length_m
```

### Comparing `captif-slp-0.8/pyproject.toml` & `captif-slp-0.9/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "captif-slp"
-version = "0.8"
+version = "0.9"
 description = ""
 authors = ["John Bull"]
 homepage = "https://github.com/captif-nz/captif-slp"
 license = "MIT"
 readme = "README.md"
 keywords = ["CAPTIF"]
 
@@ -18,11 +18,12 @@
 matplotlib = "^3.4.3"
 psutil = "^5.8.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
 pytest-randomly = "^3.10.1"
+pre-commit = "^2.19.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `captif-slp-0.8/setup.py` & `captif-slp-0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'pandas>=1.3.3,<2.0.0',
  'psutil>=5.8.0,<6.0.0',
  'pydantic>=1.8.2,<2.0.0',
  'scipy>=1.7.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'captif-slp',
-    'version': '0.8',
+    'version': '0.9',
     'description': '',
     'long_description': '# captif-slp\n\nThe *captif-slp* Python package can be used to calculate the Mean Profile Depth (MPD) of a road surface according to *[ISO 13473-1:2019](https://www.iso.org/standard/45111.html) Characterization of pavement texture by use of surface profiles — Part 1: Determination of mean profile depth*.\n\nThe software has been developed at the Waka Kotahi NZ Transport Agency *[CAPTIF Road Research Centre](https://www.nzta.govt.nz/roads-and-rail/road-composition/road-pavements/captif/)* for use with the CAPTIF in-house Stationary Laser Profilometer (SLP). While some methods are specific to data captured using the CAPTIF SLP instrument the software can also be used to calculate MPD of other road surface profiles provided the data is converted to a valid format before processing.\n\nRefer to the *[European Road Profile Users\' Group](https://www.erpug.org/index.php?contentID=239)* website for further information on ISO 13473-1 including a MATLAB implementation and a set of reference profiles and results.\n\nAlso refer to *[Transfund New Zealand Research Report 84](https://www.nzta.govt.nz/resources/research/reports/84/)* for details of the original Stationary Laser Profilometer developed in 1997 for use by Transit New Zealand. This instrument was based on the VTI stationary laser profilometer.\n\n## Installation\n\n*captif-slp* can be installed by running `pip install captif-slp`.\n\nThe package requires Python 3.9 to run.\n\n## Usage\n\n### The Reading object\n\nThe *Reading* class provides a mechanism to interact with an individual road surface profile and can be imported using `from captif_slp import Reading`.\n\nA new *Reading* object must be created using one of the following class methods.\n\n1. From a DataFrame containing `distance_mm` and `relative_height_mm` columns:\n\n    ```python\n    reading = Reading.from_trace(\n        trace: DataFrame,\n        meta: Optional[dict] = None,\n        ...\n    )\n    ```\n\n    The `meta` keyword argument provides a mechanism for attaching meta data to a *Reading* object. This can be used to include information such as a file name, reading number or measurement date. The data can be accessed later from the *meta* attribute.\n\n2. Or from a valid *texture* data file capable of being read using the *[captif-data-structures](https://github.com/captif-nz/captif-data-structures)* package (i.e. a CAPTIF in-house file format):\n\n    ```python\n    reading = Reading.from_file(\n        path: Union[str, Path],\n        parallel: bool = True,\n        ...\n    )\n    ```\n\n    The `parallel` keyword argument allows the file to be read using the Python *multiprocessing* module. This can significantly speed up load times for large files. Note that where several files are being processed it is more efficient to pass individual files to each CPU core for processing in which case *parallel* **must be set to False** to allow the multiprocessing module to be used by a higher level function.\n\nThe remaining keyword arguments are common for `Reading.from_trace()` and `Reading.from_file()`:\n\n```python\nreading = Reading.from_...(\n    ...\n    segment_length_mm: int = 100,\n    target_sample_spacing_mm: float = 0.5,\n    evaluation_length_m: Optional[float] = None,\n    alpha: int = 3,\n    start_mm: Optional[float] = None,\n    end_mm: Optional[float] = None,\n    detect_plates: bool = False,\n)\n```\n\nThe keyword arguments have the following meanings:\n\n- `segment_lenght_mm` -- *default: 100*\n\\\nLength of the segments (in millimetres) that the profile is split into for processing. Note that this should generally be left as the default value of 100 mm as this is the required segment length in ISO 13473-1.\n\n- `target_sample_spacing_mm` -- *default: 0.5*\n\\\nThe sample spacing (in millimetres) used by the resampling process. ISO 13473-1:2019 calls for a road surface profile to be resampled to either 0.5 mm or 1.0 mm depending on the sample spacing in the original profile. In general 0.5 mm should be used where the original sample spacing is less than or equal to 0.5 mm.\n\n- `evaluation_length_m` -- *default: None*\n\\\nThe evaluation length (in metres) over which the mean profile depth is reported. The default behaviour is to calculate MPD for the entire road surface profile. For spot measurements taken using a Stationary Laser Profilometer (SLP) the default behaviour is appropriate. For continuous measurements it is usually more useful to report MPD over shorter sections in which case the evaluation length could be set to 10 or 20 metres.\n\n- `alpha` -- *default: 3*\n\\\nThe constant used in the spike detection criterion (Eqn E.1, ISO 13473-1:2019). The default value of 3 is the value suggested in the standard. Note that a value of 3 used with profiles taken using the CAPTIF SLP results in a large number of false positives when analysing highly texture surfaces in New Zealand (e.g. chipseals). A value of 6 has been found to yield good results on profiles taken using the CAPTIF SLP instrument.\n\n- `start_mm` -- *default: None*\n\\\nUsed to remove a section from the beginning of the profile before processing. The default is use the full profile. The value is ignored if the *detect_plates* is set to True.\n\n- `end_mm` -- *default: None*\n\\\nUsed to remove a section from the end of the profile before processing. The default is use the full profile. The value is ignored if the *detect_plates* is set to True.\n\n- `detect_plates` -- *default: False*\n\\\nUsed to detect reference plates at the start and/or end of the profile and trim the profile accordingly. For historical reasons reference plates are present on the CAPTIF SLP instrument to signal the start and end of the section of interest; these reference plates (along with the sections of profile outside of them) need to be removed from the profile before processing. The default behaviour is to not preform this step as it is unique to the CAPTIF SLP instrument.\n\n#### Accessing the results\n\nOnce a profile has been successfully loaded into a *Reading* object the following instance methods can be used to access the results.\n\n`reading.msd()` -- Mean Segment Depth (MSD)\n\\\nReturns a list of dictionaries containing MSD values for each segment (usually 100 mm long) in the profile. Each *dict* element in the list has the following keys:\n\n- `segment_no: int` - segment position number (int).\n- `msd: float` - mean segment depth.\n- `valid: bool` - segment validity (i.e. meets the maximum dropouts and spikes requirement).\n- `evaluation_length_position_m: Optional[float]` - evaluation length position.\n\n`reading.mpd(include_meta: bool = False)` -- Mean Profile Depth (MPD)\n\\\nReturns either a single dictionary if evaluation length is not set, or a list of dictionaries if evaluation length is set. The *dict* element(s) have the following keys:\n\n- `distance_m` - evaluation length position (*None* if evaluation length is not set).\n- `mpd` - mean profile depth (average MSD across all valid segments).\n- `stdev` - standard deviation (standard deviation of MSD from all valid segments).\n- `valid_segments` - number of valid segments in the profile.\n- `proportion_valid_segments` - proportion of valid segments in the profile.\n- `is_valid` - result validity (i.e. whether or not valid_segment_ration >= 0.5).\n- (meta data fields) - the meta data fields if *include_meta* is set to True.\n\n### Bulk processing\n\nIn order to provide efficient processing the Python *multiprocessing* module is used to process batches of valid data files meeting the CAPTIF in-house *texture* file format. The processing function can be imported using `from captif_slp import process_files`.\n\nThe function takes the path of a folder containing the files to be processed and returns a list of results as per `Reading.mpd(include_meta=True)` with the addition of a `filename` and `folder` field.\n\n```python\nresults = process_files(path: Union[str, Path])\n```\n\n`process_files` uses the following settings under the hood as these are the settings relevant to profiles taken using the CAPTIF SLP instrument:\n\n- `segment_lenght_mm = 100`\n- `target_sample_spacing_mm = 0.5`\n- `evaluation_length_m = None`\n- `alpha = 6`\n- `detect_plates = True`\n\nTo access all attributes from `Reading.from_file` (except the *parallel* attribute which is set to False internally to allow the *multiprocessing* module to be used by a higher level) use `captif_slp.process.process_generic_files`.\n\n## Issues\n\nPlease submit an issue if you find a bug or have an idea for an improvement.\n\n## License\n\nThe software is provided under the following license.\n\n*MIT License*\n\n*Copyright (c) 2021 CAPTIF Road Research Centre*\n\n*Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:*\n\n*The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.*\n\n*THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.*\n',
     'author': 'John Bull',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/captif-nz/captif-slp',
```

### Comparing `captif-slp-0.8/PKG-INFO` & `captif-slp-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captif-slp
-Version: 0.8
+Version: 0.9
 Summary: 
 Home-page: https://github.com/captif-nz/captif-slp
 License: MIT
 Keywords: CAPTIF
 Author: John Bull
 Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: MIT License
```

