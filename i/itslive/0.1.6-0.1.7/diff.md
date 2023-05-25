# Comparing `tmp/itslive-0.1.6.tar.gz` & `tmp/itslive-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itslive-0.1.6.tar", max compression
+gzip compressed data, was "itslive-0.1.7.tar", max compression
```

## Comparing `itslive-0.1.6.tar` & `itslive-0.1.7.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0    35149 2022-12-29 21:09:11.759936 itslive-0.1.6/LICENSE
--rw-r--r--   0        0        0     1440 2022-12-29 21:09:11.759936 itslive-0.1.6/itslive/__init__.py
--rw-r--r--   0        0        0        0 2022-12-29 21:09:11.759936 itslive-0.1.6/itslive/cli/__init__.py
--rw-r--r--   0        0        0     5269 2022-12-29 21:09:11.759936 itslive-0.1.6/itslive/cli/export.py
--rw-r--r--   0        0        0     5817 2022-12-29 21:09:11.759936 itslive-0.1.6/itslive/cli/plot.py
--rw-r--r--   0        0        0    14822 2022-12-29 21:09:11.759936 itslive-0.1.6/itslive/data_cube.py
--rw-r--r--   0        0        0      115 2022-12-29 21:09:11.759936 itslive-0.1.6/itslive/data_pairs.py
--rw-r--r--   0        0        0     3219 2022-12-29 21:09:11.759936 itslive-0.1.6/itslive/data_viz.py
--rw-r--r--   0        0        0     1047 2022-12-29 21:09:11.763936 itslive-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 itslive-0.1.6/setup.py
--rw-r--r--   0        0        0      870 1970-01-01 00:00:00.000000 itslive-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-25 15:23:33.888923 itslive-0.1.7/LICENSE
+-rw-r--r--   0        0        0      239 2023-05-25 15:23:33.888923 itslive-0.1.7/itslive/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:23:33.888923 itslive-0.1.7/itslive/cli/__init__.py
+-rw-r--r--   0        0        0     5300 2023-05-25 15:23:33.888923 itslive-0.1.7/itslive/cli/export.py
+-rw-r--r--   0        0        0     5861 2023-05-25 15:23:33.888923 itslive-0.1.7/itslive/cli/plot.py
+-rw-r--r--   0        0        0      109 2023-05-25 15:23:33.888923 itslive-0.1.7/itslive/dataviz/__init__.py
+-rw-r--r--   0        0        0     2557 2023-05-25 15:23:33.888923 itslive-0.1.7/itslive/dataviz/_viz.py
+-rw-r--r--   0        0        0      618 2023-05-25 15:23:33.888923 itslive-0.1.7/itslive/velocity_cubes/__init__.py
+-rw-r--r--   0        0        0    14964 2023-05-25 15:23:33.888923 itslive-0.1.7/itslive/velocity_cubes/_cubes.py
+-rw-r--r--   0        0        0       67 2023-05-25 15:23:33.888923 itslive-0.1.7/itslive/velocity_pairs/__init__.py
+-rw-r--r--   0        0        0      115 2023-05-25 15:23:33.888923 itslive-0.1.7/itslive/velocity_pairs/_pairs.py
+-rw-r--r--   0        0        0     1047 2023-05-25 15:23:33.900924 itslive-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      875 1970-01-01 00:00:00.000000 itslive-0.1.7/PKG-INFO
```

### Comparing `itslive-0.1.6/LICENSE` & `itslive-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `itslive-0.1.6/itslive/cli/export.py` & `itslive-0.1.7/itslive/cli/export.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,30 +65,30 @@
             return df
         except Exception:
             raise click.BadParameter("Not a valid CSV file, the format is lon,lat")
 
 
 def export_time_series(points, variables, format, outdir):
     if format == "csv":
-        itslive.cubes.export_csv(points, variables, outdir)
+        itslive.velocity_cubes.export_csv(points, variables, outdir)
     elif format == "netcdf":
-        itslive.cubes.export_netcdf(points, variables, outdir)
+        itslive.velocity_cubes.export_netcdf(points, variables, outdir)
     else:
-        itslive.cubes.export_stdout(points, variables)
+        itslive.velocity_cubes.export_stdout(points, variables)
     return None
 
 
 def plot_time_series(points, variable, label_by, outdir, stdout):
     if stdout is not None:
         # experimental
-        itslive.cubes._plot_time_series_terminal(points, variable)
+        itslive.velocity_cubes._plot_time_series_terminal(points, variable)
     else:
         pass
         # TODO: save plot on outdir
-        # plot = itslive.cubes.plot_time_series(points, variable, label_by)
+        # plot = itslive.velocity_cubes.plot_time_series(points, variable, label_by)
         # plot.save()
     return None
 
 
 @click.command()
 @click.option(
     "--itslive-catalog",
@@ -127,15 +127,14 @@
     multiple=True,
     default=["v"],
     help=(
         "v: velocity"
         "v_error: error in v"
         "vx: Velocity x component"
         "vy: Velocity y component"
-        "for a full list visit"
     ),
 )
 @click.option(
     "--outdir",
     type=str,
     help="output directory",
 )
@@ -156,18 +155,18 @@
     ITS_LIVE Global Glacier Veolocity
 
     [i]You can try using --help at the top level and also for
     specific group subcommands.[/]
     """
 
     points = []
-    itslive.cubes.load_catalog(itslive_catalog)
+    itslive.velocity_cubes.load_catalog(itslive_catalog)
     if debug:
         rprint("Debug mode is [red]on[/]")
-        rprint(f"Using: {itslive.cubes._current_catalog_url}")
+        rprint(f"Using: {itslive.velocity_cubes._current_catalog_url}")
     if input_coordinates is not None:
         # rprint(f"input file head: {input.head}")
         for index, row in input_coordinates.iterrows():
             points.append((row["lon"], row["lat"]))
     else:
         if lat and lon:
             points.append((lon, lat))
```

### Comparing `itslive-0.1.6/itslive/cli/plot.py` & `itslive-0.1.7/itslive/cli/plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,30 +65,30 @@
             return df
         except Exception:
             raise click.BadParameter("Not a valid CSV file, the format is lon,lat")
 
 
 def export_time_series(points, variables, format, outdir):
     if format == "csv":
-        itslive.cubes.export_csv(points, variables, outdir)
+        itslive.velocity_cubes.export_csv(points, variables, outdir)
     elif format == "netcdf":
-        itslive.cubes.export_netcdf(points, variables, outdir)
+        itslive.velocity_cubes.export_netcdf(points, variables, outdir)
     else:
-        itslive.cubes.export_stdout(points, variables)
+        itslive.velocity_cubes.export_stdout(points, variables)
     return None
 
 
 def plot_time_series(points, variable, operation, freq, outdir, stdout):
     if stdout is not None:
         # experimental
-        itslive.cubes._plot_time_series_terminal(points, variable, operation, freq)
+        itslive.velocity_cubes.plot_time_series_terminal(points, variable)
     else:
         pass
         # TODO: save plot on outdir
-        # plot = itslive.cubes.plot_time_series(points, variable, label_by)
+        # plot = itslive.velocity_cubes.plot_time_series(points, variable, label_by)
         # plot.save()
     return None
 
 
 def list_variables():
     itslive.cubes.list_variables()
 
@@ -167,16 +167,16 @@
     ITS_LIVE Global Glacier Veolocity
 
     [i]You can try using --help at the top level and also for
     specific group subcommands.[/]
     """
 
     points = []
-    itslive.cubes.load_catalog(itslive_catalog)
-    rprint(f"Using: {itslive.cubes._current_catalog_url}")
+    catalog, current_catalog = itslive.velocity_cubes.load_catalog(itslive_catalog)
+    rprint(f"Using: {current_catalog}")
     if input_coordinates is not None:
         # rprint(f"input file head: {input.head}")
         for index, row in input_coordinates.iterrows():
             points.append((row["lon"], row["lat"]))
     else:
         if lat and lon:
             points.append((lon, lat))
```

### Comparing `itslive-0.1.6/itslive/data_cube.py` & `itslive-0.1.7/itslive/velocity_cubes/_cubes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,83 @@
 # to get and use geojson datacube catalog
 # for timing data access
+import json
+import pathlib
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 from uuid import uuid4
 
+import numpy as np
 import pyproj
 import requests
 # for datacube xarray/zarr access
 import xarray as xr
-from matplotlib import pyplot as plt
+from itslive.dataviz import plot_terminal
 from rich import print as rprint
 from rich.progress import track
 from shapely import geometry
 
-import itslive
-
-from .data_viz import plot_terminal, plot_variable
-
 
 # class to throw time series lookup errors
 class timeseriesException(Exception):
     pass
 
 
 DEFAULT_CATALOG_URL = (
     "https://its-live-data.s3.amazonaws.com/datacubes/catalog_v02.json"
 )
 
+DEFAULT_CATALOG_CACHE_PATH = pathlib.Path.home() / ".itslive_catalog.json"
+
+
+def load_catalog(url: str = DEFAULT_CATALOG_URL, reload: bool = False):
+    """Loads a geojson catalog containing all the zarr cube urls and metadata,
+    if url is not provided will load the default location on S3
+        returns catalog,catalog_url
+    """
+    if DEFAULT_CATALOG_CACHE_PATH.exists() and not reload:
+        _current_catalog_url = DEFAULT_CATALOG_URL
+        with open(DEFAULT_CATALOG_CACHE_PATH, "r") as f:
+            _catalog = json.load(f)
+    else:
+        try:
+            _current_catalog_url = url
+            _catalog = requests.get(_current_catalog_url).json()
+            with open(DEFAULT_CATALOG_CACHE_PATH, "w") as f:
+                json.dump(_catalog, f)
+        except Exception:
+            raise Exception
+    return _catalog, _current_catalog_url
+
 
-# keep track of open cubes so that we don't re-read xarray metadata
-# and dimension vectors
+# keep track of open cubes so that we don't re-open (it is slow to re-read xarray metadata
+# and dimension vectors)
 _open_cubes = {}
-_catalog = requests.get(DEFAULT_CATALOG_URL).json()
-_current_catalog_url = DEFAULT_CATALOG_URL
+
+_catalog, _current_catalog_url = load_catalog(url=DEFAULT_CATALOG_URL)
 
 
 def _get_projected_xy_point(lon: float, lat: float, projection: str) -> geometry.Point:
     reprojection = pyproj.Transformer.from_proj(
         "epsg:4326", f"epsg:{projection}", always_xy=True
     )
     point = geometry.Point(*reprojection.transform(lon, lat))
     return point
 
 
+def _get_geographic_point_from_projected(
+    x: float, y: float, from_projection: str
+) -> geometry.Point:
+    to_ll_reprojection = pyproj.Transformer.from_proj(
+        f"epsg:{from_projection}", "epsg:4326", always_xy=True
+    )
+    point = geometry.Point(*to_ll_reprojection.transform(x, y))
+    return point
+
+
 def _merge_default_variables(variables: List[str]) -> set[str]:
     _default_variables = [
         "v",
         "v_error",
         "vx",
         "vx_error",
         "vy",
@@ -58,20 +89,14 @@
     query_variables = set(_default_variables)
     query_variables.update(variables)
     return query_variables
 
     return []
 
 
-def list_variables() -> None:
-    variables = itslive.__variables__
-    for v in variables:
-        rprint(f"[red on black] {v} [/]")
-
-
 def find(
     points: List[tuple[float, float]],
 ) -> List[Dict[str, Any]]:
     """Find the zarr cube information for a given geometry, if 2 values are passed
     it will use the point geometry, if 3 or more values are passed it will
     search using a polygon.
 
@@ -87,28 +112,14 @@
         point = points[0]
         cubes = find_by_point(lon=point[0], lat=point[1])
     if len(points) > 1:
         cubes = find_by_polygon(points)
     return cubes
 
 
-def load_catalog(
-    url: str = "https://its-live-data.s3.amazonaws.com/datacubes/catalog_v02.json",
-):
-    """Loads a geojson catalog containing all the zarr cube urls and metadata,
-    if url is not provided will load the default location on S3
-    """
-    try:
-        _current_catalog_url = url
-        _catalog = requests.get(_current_catalog_url).json()
-    except Exception:
-        raise Exception
-    return _catalog
-
-
 def find_by_bbox(
     lower_left_lon: float,
     lower_left_lat: float,
     upper_right_lon: float,
     upper_right_lat: float,
 ) -> List[Dict[str, Any]]:
     """
@@ -177,21 +188,24 @@
     return cubes
 
 
 def get_time_series(
     points: List[tuple[float, float]], variables: List[str] = ["v"]
 ) -> List[Dict[str, Any]]:
     """
-    Returns an xarray DataArray (time series) for each variable on the list for each of the lon lat points.
+    For the points in the list, returns a list of dictionaries - each one containing:
+        an xarray DataArray (time series) for each variable on the list for each of the lon lat points.
 
-    :params points: List of lon lat coordinates (i.e. some points laong the center line of a glacier)
-    :params variables: list of variables included in the Dataset: v, vx, vy etc.
-    :returns List[Dict]: list of tuples with coordinates and xarray Datasets for the matching Zarr cubes
+    :params points: List of (lon, lat) coordinates (EPSG:4326) (e.g. points along the center line of a glacier)
+    :params variables: list of variables to be included in the Dataset: v, vx, vy etc.
+    :returns: list of dictionaries with coordinates and xarray time series Datasets for the nearest neighbors to the points
+                ITS_LIVE processes on a 120 m grid, so nearest points will be close to requested points
     """
     velocity_ts: List = []
+    variables = _merge_default_variables(variables)
     for point in points:
         lon = point[0]
         lat = point[1]
         results = find_by_point(lon, lat)
         if len(results):
             cube = results[0]
             projection = cube["properties"]["epsg"]
@@ -208,46 +222,63 @@
                 xr_da = xr.open_dataset(
                     cube_s3_url, engine="zarr", storage_options={"anon": True}
                 )
                 _open_cubes[cube_s3_url] = xr_da
             time_series = xr_da[variables].sel(
                 x=projected_point.x, y=projected_point.y, method="nearest"
             )
+
             if time_series is not None and isinstance(time_series, xr.Dataset):
+                x_off = time_series.x.values - projected_point.x
+                y_off = time_series.y.values - projected_point.y
+                ll_pt = _get_geographic_point_from_projected(
+                    time_series.x.values, time_series.y.values, projection
+                )
+                actual_lon = ll_pt.x
+                actual_lat = ll_pt.y
+
                 velocity_ts.append(
-                    {"coordinates": (lon, lat), "time_series": time_series}
+                    {
+                        "requested_point_geographic_coordinates": (lon, lat),
+                        "returned_point_geographic_coordinates": (
+                            actual_lon,
+                            actual_lat,
+                        ),
+                        "returned_point_projected_coordinates": {
+                            "epsg": projection,
+                            "coords": (time_series.x.values, time_series.y.values),
+                        },
+                        "returned_point_offset_from_requested_in_projection_meters": np.sqrt(
+                            x_off**2 + y_off**2
+                        ),
+                        "time_series": time_series,
+                    }
                 )
 
     return velocity_ts
 
 
 def export_csv(
     points: List[tuple[float, float]],
     variables: List[str] = ["v"],
     outdir: Optional[str] = None,
 ) -> None:
-    """Exports a list of ITS_LIVE glacier velocity variables to csv files
-
-    :params points: List of lon lat coordinates (i.e. some points laong the center line of a glacier)
-    :params variables: list of variables included in the Dataset: v, vx, vy etc.
-    :params outdir: directory to place the CSV files
-    """
+    """Exports a list of ITS_LIVE glacier velocity variables to csv files"""
 
     query_variables = _merge_default_variables(variables)
 
     outdir = f"./itslive-{uuid4()}" if outdir is None else outdir
 
     Path(outdir).mkdir(parents=True, exist_ok=True)
 
     for point in track(
         points,
         description=f"Processing {len(points)} coordinates...",
         total=len(points),
     ):
-
         lon = round(point[0], 4)
         lat = round(point[1], 4)
         result_series = get_time_series([(lon, lat)], query_variables)
         if len(result_series):
             series = result_series[0]["time_series"]
 
             df = series.to_dataframe()
@@ -293,32 +324,26 @@
 
 
 def export_netcdf(
     points: List[tuple[float, float]],
     variables: List[str] = ["v"],
     outdir: Optional[str] = None,
 ) -> None:
-    """Exports a list of ITS_LIVE glacier velocity variables to netcdf files
-
-    :params points: List of lon lat coordinates (i.e. some points laong the center line of a glacier)
-    :params variables: list of variables included in the Dataset: v, vx, vy etc.
-    :params outdir: directory to place the CSV files
-    """
+    """Exports a list of ITS_LIVE glacier velocity variables to netcdf files"""
 
     query_variables = _merge_default_variables(variables)
 
     outdir = f"./itslive-{uuid4()}" if outdir is None else outdir
     Path(outdir).mkdir(parents=True, exist_ok=True)
 
     for point in track(
         points,
         description=f"Processing {len(points)} coordinates...",
         total=len(points),
     ):
-
         lon = round(point[0], 4)
         lat = round(point[1], 4)
 
         file_name = f"LON{lon}--LAT{lat}"
         result_series = get_time_series([(lon, lat)], query_variables)
         if len(result_series):
             series = result_series[0]["time_series"]
@@ -327,28 +352,23 @@
             rprint(f"[red on black]No data found at[/] lon:{lon}, lat: {lat}")
 
 
 def export_stdout(
     points: List[tuple[float, float]],
     variables: List[str] = ["v"],
 ) -> None:
-    """Exports a list of ITS_LIVE glacier velocity variables to stdout
-
-    :params points: List of lon lat coordinates (i.e. some points laong the center line of a glacier)
-    :params variables: list of variables included in the Dataset: v, vx, vy etc.
-    """
+    """Exports a list of ITS_LIVE glacier velocity variables to stdout"""
 
     query_variables = _merge_default_variables(variables)
 
     for point in track(
         points,
         description=f"Processing {len(points)} coordinates...",
         total=len(points),
     ):
-
         lon = round(point[0], 4)
         lat = round(point[1], 4)
 
         result_series = get_time_series([(lon, lat)], query_variables)
         if len(result_series):
             series = result_series[0]["time_series"]
             df = series.to_dataframe()
@@ -377,66 +397,37 @@
             rprint(f"[red on black] No data found at [/] lon: {lon}, lat: {lat}")
 
 
 def plot_time_series(
     points: List[tuple[float, float]],
     variable: str = "v",
     label_by: str = "location",
+    outdir: Optional[str] = None,
 ) -> Any:
-    """Plots velocity time series for a list of lon, lat locations. Color coding
-    can be by location or satellite, satellite is better suited for single points.
+    return None
 
-    :params points: List of lon lat coordinates (i.e. some points laong the center line of a glacier)
-    :params variables: list of variables included in the Dataset: v, vx, vy etc.
-    """
-    fig, ax = plt.subplots(1, 1)
-    for point in track(
-        points,
-        description=f"Processing {len(points)} coordinates...",
-        total=len(points),
-    ):
-        lon = round(point[0], 4)
-        lat = round(point[1], 4)
 
-        query_variables = _merge_default_variables(variable)
-
-        series = get_time_series([(lon, lat)], variables=query_variables)
-        if series is not None and len(series) > 0:
-            ts = series[0]["time_series"]
-            plot_variable(lon, lat, ax, ts, variable, label_by)
-
-    return ax
-
-
-def _plot_time_series_terminal(
+def plot_time_series_terminal(
     points: List[tuple[float, float]],
     variable: List[str] = ["v"],
-    operation: str = "median",
-    freq: str = "m",
+    label_by: str = "location",
+    outdir: Optional[str] = None,
 ):
-    """
-    A bit of an easter egg. Plots velocity time series directly on the terminal.
-    only used by the CLI via the itslive-plot command.
-    """
     for point in track(
         points,
         description=f"Processing {len(points)} coordinates...",
         total=len(points),
     ):
         lon = round(point[0], 4)
         lat = round(point[1], 4)
 
-        query_variables = _merge_default_variables(variable)
-
-        series = get_time_series([(lon, lat)], variables=query_variables)
+        series = get_time_series([(lon, lat)], variables=variable)
         if series is not None and len(series) > 0:
             ts = series[0]["time_series"]
-
-            plot_terminal(lon, lat, ts, variable, operation, freq)
-
+            plot_terminal(lon, lat, ts, variable)
             max_variable = (
                 ts[variable]
                 .where(ts[variable] == ts[variable].max(), drop=True)
                 .squeeze()
             )
             min_variable = (
                 ts[variable]
```

### Comparing `itslive-0.1.6/itslive/data_viz.py` & `itslive-0.1.7/itslive/dataviz/_viz.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,43 @@
 from typing import Any
 
-import matplotlib
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import plotext as plt
+import plotext
 import xarray as xr
 
+# import itslive
+
 
 def plot_terminal(
     lon: float,
     lat: float,
     dataset: xr.Dataset,
     variable: str = "v",
     operation: str = "median",
     freq: str = "m",
 ) -> None:
-    """Plots a variable from an already located xarray dataset in the terminal"""
-    plt.date_form("Y-m-d")
-    sat = np.unique(dataset["satellite_img1"].values)
-    sats = set([str(s[0]) for s in sat])
-    g_ts = dataset.to_pandas().sort_index()
-
-    for satellite in sats:
-        ts = getattr(
-            (
-                g_ts.where(g_ts["satellite_img1"].str[:1] == satellite)[
-                    variable
-                ].groupby(pd.Grouper(freq=freq))
-            ),
-            operation,
-        )()
-
-        dates = [
-            d.to_pydatetime().strftime("%Y-%m-%d")
-            for d in pd.date_range(start=ts.index.min(), end=ts.index.max(), freq=freq)
-        ]
-
-        values = [float(v[0]) for v in ts.values]
-        if satellite in ["1", "2"]:
-            label = f"Sentinel {satellite}"
-        else:
-            label = f"Landsat {satellite}"
-        plt.plot(dates, values, label=label)
-
-        xticks, xlabels = list(dates[::6]), list(dates[::6])
-        plt.xticks(xticks, xlabels)
-    plt.xlabel("Date")
-    # TODO: add lat, lon in plot
-    plt.ylabel(variable)
-    plt.show()
+    """Plots a variable from a given lon, lat in the terminal"""
+    plotext.date_form("Y-m-d")
+    # the beauty of pandas + xarray
+    ts = dataset[variable].to_pandas().sort_index()
+    dates = [d for d in ts.index.to_pydatetime()]
+    values = [float(v[0]) for v in ts.values]
+    xticks = [i for i in range(0, len(dates))]
+    xlabels = [d.strftime("%Y/%m") for d in dates]
+    plotext.xticks(xticks, xlabels)
+    plotext.plot(values)
+    plotext.show()
 
 
 def _plot_by_location(
     lon: float,
     lat: float,
-    ax: matplotlib.axes.Axes,
+    ax: plt.Axes,
     dataset: xr.Dataset,
     variable: str = "v",
 ) -> None:
     dt = dataset["date_dt"].values
     dt = dt.astype(float) * 1.15741e-14
 
     ax.plot(
@@ -69,19 +48,18 @@
 
     return ax
 
 
 def _plot_by_sensor(
     lon: float,
     lat: float,
-    ax: matplotlib.axes.Axes,
+    ax: plt.Axes,
     dataset: xr.Dataset,
     variable: str = "v",
 ) -> None:
-
     sats = np.unique(dataset["satellite_img1"].values)
     sat_plotsym_dict = {
         "1": "r+",
         "2": "bo",
         "4": "y+",
         "5": "y+",
         "7": "c+",
@@ -117,15 +95,15 @@
 
     return ax
 
 
 def plot_variable(
     lon: float,
     lat: float,
-    ax: matplotlib.axes.Axes,
+    ax: plt.Axes,
     dataset: xr.Dataset,
     variable: str = "v",
     label_by: str = "location",
 ) -> Any:
     """ """
     if label_by == "location":
         return _plot_by_location(lon, lat, ax, dataset, variable)
```

### Comparing `itslive-0.1.6/pyproject.toml` & `itslive-0.1.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "itslive"
 homepage = "https://github.com/nasa-jpl/itslive-vortex"
-version = "0.1.6"
+version = "0.1.7"
 description = "Python client for ITSLIVE gralcier velocity data"
 authors = ["Luis Lopez <luis.lopez@nsidc.org>"]
 license = "GNUL V3"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 zarr = ">=2.11"
 s3fs = ">=2022.3"
 xarray = ">=2022.3"
 Shapely = ">=1.8"
 pyproj = ">=3.3"
-matplotlib = ">=3.5"
+matplotlib = "~=3.6"
 rich-click = ">=1.5"
 plotext=">=0"
 tabulate = ">=0.9.0"
 pandas = "1.5.1"
 requests = "^2.28.1"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `itslive-0.1.6/PKG-INFO` & `itslive-0.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: itslive
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python client for ITSLIVE gralcier velocity data
 Home-page: https://github.com/nasa-jpl/itslive-vortex
 License: GNUL V3
 Author: Luis Lopez
 Author-email: luis.lopez@nsidc.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Shapely (>=1.8)
-Requires-Dist: matplotlib (>=3.5)
+Requires-Dist: matplotlib (>=3.6,<4.0)
 Requires-Dist: pandas (==1.5.1)
 Requires-Dist: plotext (>=0)
 Requires-Dist: pyproj (>=3.3)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: rich-click (>=1.5)
 Requires-Dist: s3fs (>=2022.3)
 Requires-Dist: tabulate (>=0.9.0)
```

