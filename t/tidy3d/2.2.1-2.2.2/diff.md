# Comparing `tmp/tidy3d-2.2.1.tar.gz` & `tmp/tidy3d-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidy3d-2.2.1.tar", last modified: Tue May 23 18:01:04 2023, max compression
+gzip compressed data, was "tidy3d-2.2.2.tar", last modified: Thu May 25 16:50:24 2023, max compression
```

## Comparing `tidy3d-2.2.1.tar` & `tidy3d-2.2.2.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.632015 tidy3d-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-23 18:00:43.000000 tidy3d-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-23 18:00:43.000000 tidy3d-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-23 18:01:04.632015 tidy3d-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-23 18:00:43.000000 tidy3d-2.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-23 18:00:43.000000 tidy3d-2.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.600015 tidy3d-2.2.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-23 18:00:43.000000 tidy3d-2.2.1/requirements/basic.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-23 18:00:43.000000 tidy3d-2.2.1/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-23 18:00:43.000000 tidy3d-2.2.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 18:00:43.000000 tidy3d-2.2.1/requirements/gdspy.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 18:00:43.000000 tidy3d-2.2.1/requirements/gdstk.txt
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-23 18:00:43.000000 tidy3d-2.2.1/requirements/jax.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-23 18:00:43.000000 tidy3d-2.2.1/requirements/trimesh.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 18:00:43.000000 tidy3d-2.2.1/requirements/web.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-23 18:00:43.000000 tidy3d-2.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 18:01:04.636015 tidy3d-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-23 18:00:43.000000 tidy3d-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.600015 tidy3d-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.604015 tidy3d-2.2.1/tests/_test_local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/_test_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/_test_local/_test_adjoint_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/_test_local/_test_data_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/_test_local/_test_fit_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/_test_local/_test_plugins_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/_test_local/_test_web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.608015 tidy3d-2.2.1/tests/test_components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_IO.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_boundaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_field_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19253 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_grid_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_medium.py
--rw-r--r--   0 runner    (1001) docker     (123)    23843 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_meshgenerate.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    21134 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_sidewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    53136 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_components/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.608015 tidy3d-2.2.1/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_data/test_data_arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)    19395 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_data/test_monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_data/test_sim_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.608015 tidy3d-2.2.1/tests/test_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_package/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_package/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_package/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_package/test_make_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_package/test_material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_package/test_parametric_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.612015 tidy3d-2.2.1/tests/test_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40386 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_plugins/test_adjoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_plugins/test_component_modeler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_plugins/test_dispersion_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_plugins/test_mode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_plugins/test_polyslab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_plugins/test_resonance_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_plugins/test_waveguide.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.612015 tidy3d-2.2.1/tests/test_web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_web/mock_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_web/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_web/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_web/test_material_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_web/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_web/test_tidy3d_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_web/test_tidy3d_material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_web/test_tidy3d_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/test_web/test_webapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    16947 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.612015 tidy3d-2.2.1/tidy3d/
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.620015 tidy3d-2.2.1/tidy3d/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)    23354 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/boundary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.620015 tidy3d-2.2.1/tidy3d/components/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/data/data_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    14266 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    78767 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/data/monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    28054 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/data/sim_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/field_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)   146570 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.620015 tidy3d-2.2.1/tidy3d/components/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14955 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/grid/grid_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    47556 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/grid/mesher.py
--rw-r--r--   0 runner    (1001) docker     (123)    68574 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    29507 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)   117741 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    33364 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/components/viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.620015 tidy3d-2.2.1/tidy3d/material_library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/material_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62029 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/material_library/material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/material_library/material_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/material_library/parametric_materials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.620015 tidy3d-2.2.1/tidy3d/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.620015 tidy3d-2.2.1/tidy3d/plugins/adjoint/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.624015 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.624015 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/data/data_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/data/monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/data/sim_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    23786 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)    17903 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/components/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    29963 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/adjoint/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.624015 tidy3d-2.2.1/tidy3d/plugins/dispersion/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/dispersion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23663 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/dispersion/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/dispersion/fit_web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.628015 tidy3d-2.2.1/tidy3d/plugins/mode/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/mode/derivatives.py
--rw-r--r--   0 runner    (1001) docker     (123)    25720 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/mode/mode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    27752 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/mode/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/mode/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.628015 tidy3d-2.2.1/tidy3d/plugins/polyslab/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/polyslab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/polyslab/polyslab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.628015 tidy3d-2.2.1/tidy3d/plugins/resonance/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/resonance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/resonance/resonance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.628015 tidy3d-2.2.1/tidy3d/plugins/smatrix/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/smatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19999 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/smatrix/smatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.628015 tidy3d-2.2.1/tidy3d/plugins/waveguide/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/waveguide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35573 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/plugins/waveguide/rectangular_dielectric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/updater.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.632015 tidy3d-2.2.1/tidy3d/web/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)   275233 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.632015 tidy3d-2.2.1/tidy3d/web/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/cli/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20751 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/http_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/httputils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/material_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/material_libray.py
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/s3utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16498 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/simulation_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    24366 2023-05-23 18:00:43.000000 tidy3d-2.2.1/tidy3d/web/webapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:01:04.616015 tidy3d-2.2.1/tidy3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-23 18:01:04.000000 tidy3d-2.2.1/tidy3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-05-23 18:01:04.000000 tidy3d-2.2.1/tidy3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:01:04.000000 tidy3d-2.2.1/tidy3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-23 18:01:04.000000 tidy3d-2.2.1/tidy3d.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-23 18:01:04.000000 tidy3d-2.2.1/tidy3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 18:01:04.000000 tidy3d-2.2.1/tidy3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.078246 tidy3d-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-25 16:50:02.000000 tidy3d-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-25 16:50:02.000000 tidy3d-2.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-25 16:50:24.078246 tidy3d-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-25 16:50:02.000000 tidy3d-2.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-25 16:50:02.000000 tidy3d-2.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.014246 tidy3d-2.2.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-25 16:50:02.000000 tidy3d-2.2.2/requirements/basic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-25 16:50:02.000000 tidy3d-2.2.2/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-25 16:50:02.000000 tidy3d-2.2.2/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-25 16:50:02.000000 tidy3d-2.2.2/requirements/gdspy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-25 16:50:02.000000 tidy3d-2.2.2/requirements/gdstk.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-25 16:50:02.000000 tidy3d-2.2.2/requirements/jax.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-25 16:50:02.000000 tidy3d-2.2.2/requirements/trimesh.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-25 16:50:02.000000 tidy3d-2.2.2/requirements/web.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 16:50:02.000000 tidy3d-2.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 16:50:24.078246 tidy3d-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-25 16:50:02.000000 tidy3d-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.014246 tidy3d-2.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.018246 tidy3d-2.2.2/tests/_test_local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/_test_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/_test_local/_test_adjoint_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/_test_local/_test_data_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/_test_local/_test_fit_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/_test_local/_test_plugins_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/_test_local/_test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.022246 tidy3d-2.2.2/tests/test_components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_components/test_IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_components/test_apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_components/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_components/test_boundaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_components/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_components/test_field_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19253 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_components/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_components/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_components/test_grid_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_components/test_medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23843 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_components/test_meshgenerate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_components/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_components/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21134 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_components/test_sidewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53136 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_components/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_components/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_components/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_components/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.026246 tidy3d-2.2.2/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_data/test_data_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19395 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_data/test_monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_data/test_sim_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.026246 tidy3d-2.2.2/tests/test_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_package/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_package/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_package/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_package/test_make_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_package/test_material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_package/test_parametric_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.030246 tidy3d-2.2.2/tests/test_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41852 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_plugins/test_adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_plugins/test_component_modeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_plugins/test_dispersion_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_plugins/test_mode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_plugins/test_polyslab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_plugins/test_resonance_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_plugins/test_waveguide.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.034246 tidy3d-2.2.2/tests/test_web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_web/mock_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_web/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_web/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_web/test_material_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_web/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_web/test_tidy3d_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_web/test_tidy3d_material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_web/test_tidy3d_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/test_web/test_webapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16947 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.038246 tidy3d-2.2.2/tidy3d/
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tidy3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tidy3d/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.046246 tidy3d-2.2.2/tidy3d/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tidy3d/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tidy3d/components/apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24986 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tidy3d/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tidy3d/components/boundary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.046246 tidy3d-2.2.2/tidy3d/components/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tidy3d/components/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tidy3d/components/data/data_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14266 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tidy3d/components/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78767 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tidy3d/components/data/monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28054 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tidy3d/components/data/sim_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-05-25 16:50:02.000000 tidy3d-2.2.2/tidy3d/components/field_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146570 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/components/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.050246 tidy3d-2.2.2/tidy3d/components/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/components/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14955 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/components/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/components/grid/grid_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47556 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/components/grid/mesher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68574 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/components/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/components/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29507 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/components/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117908 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/components/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33364 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/components/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/components/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/components/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/components/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/components/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/components/viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.050246 tidy3d-2.2.2/tidy3d/material_library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/material_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62029 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/material_library/material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/material_library/material_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/material_library/parametric_materials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.054246 tidy3d-2.2.2/tidy3d/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.054246 tidy3d-2.2.2/tidy3d/plugins/adjoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/adjoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.054246 tidy3d-2.2.2/tidy3d/plugins/adjoint/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/adjoint/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/adjoint/components/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.058246 tidy3d-2.2.2/tidy3d/plugins/adjoint/components/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/adjoint/components/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/adjoint/components/data/data_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/adjoint/components/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/adjoint/components/data/monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/adjoint/components/data/sim_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23786 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/adjoint/components/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/adjoint/components/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17903 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/adjoint/components/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/adjoint/components/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/adjoint/components/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29963 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/adjoint/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.058246 tidy3d-2.2.2/tidy3d/plugins/dispersion/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/dispersion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23663 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/dispersion/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/dispersion/fit_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.062246 tidy3d-2.2.2/tidy3d/plugins/mode/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/mode/derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25720 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/mode/mode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27752 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/mode/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/mode/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.062246 tidy3d-2.2.2/tidy3d/plugins/polyslab/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/polyslab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/polyslab/polyslab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.062246 tidy3d-2.2.2/tidy3d/plugins/resonance/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/resonance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/resonance/resonance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.062246 tidy3d-2.2.2/tidy3d/plugins/smatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/smatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19999 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/smatrix/smatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.062246 tidy3d-2.2.2/tidy3d/plugins/waveguide/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/waveguide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35573 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/plugins/waveguide/rectangular_dielectric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.074247 tidy3d-2.2.2/tidy3d/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/web/asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)   275233 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/web/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/web/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.074247 tidy3d-2.2.2/tidy3d/web/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/web/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/web/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/web/cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/web/cli/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/web/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20751 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/web/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/web/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/web/http_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/web/httputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/web/material_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/web/material_libray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/web/s3utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16498 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/web/simulation_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/web/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/web/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24366 2023-05-25 16:50:03.000000 tidy3d-2.2.2/tidy3d/web/webapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:50:24.038246 tidy3d-2.2.2/tidy3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-25 16:50:23.000000 tidy3d-2.2.2/tidy3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-05-25 16:50:23.000000 tidy3d-2.2.2/tidy3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:50:23.000000 tidy3d-2.2.2/tidy3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-25 16:50:23.000000 tidy3d-2.2.2/tidy3d.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-25 16:50:23.000000 tidy3d-2.2.2/tidy3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 16:50:23.000000 tidy3d-2.2.2/tidy3d.egg-info/top_level.txt
```

### Comparing `tidy3d-2.2.1/LICENSE` & `tidy3d-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/PKG-INFO` & `tidy3d-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy3d
-Version: 2.2.1
+Version: 2.2.2
 Summary: A fast FDTD solver
 Home-page: https://github.com/flexcompute/tidy3d
 Author: Tyler Hughes
 Author-email: tyler@flexcompute.com
 Project-URL: Bug Tracker, https://github.com/flexcompute/tidy3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy3d-2.2.1/README.md` & `tidy3d-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/setup.py` & `tidy3d-2.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/_test_local/_test_adjoint_performance.py` & `tidy3d-2.2.2/tests/_test_local/_test_adjoint_performance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/_test_local/_test_data_performance.py` & `tidy3d-2.2.2/tests/_test_local/_test_data_performance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/_test_local/_test_fit_web.py` & `tidy3d-2.2.2/tests/_test_local/_test_fit_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/_test_local/_test_plugins_web.py` & `tidy3d-2.2.2/tests/_test_local/_test_plugins_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/_test_local/_test_web.py` & `tidy3d-2.2.2/tests/_test_local/_test_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_components/test_IO.py` & `tidy3d-2.2.2/tests/test_components/test_IO.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_components/test_apodization.py` & `tidy3d-2.2.2/tests/test_components/test_apodization.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_components/test_base.py` & `tidy3d-2.2.2/tests/test_components/test_base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_components/test_boundaries.py` & `tidy3d-2.2.2/tests/test_components/test_boundaries.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_components/test_custom.py` & `tidy3d-2.2.2/tests/test_components/test_custom.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_components/test_field_projection.py` & `tidy3d-2.2.2/tests/test_components/test_field_projection.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_components/test_geometry.py` & `tidy3d-2.2.2/tests/test_components/test_geometry.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_components/test_grid.py` & `tidy3d-2.2.2/tests/test_components/test_grid.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_components/test_grid_spec.py` & `tidy3d-2.2.2/tests/test_components/test_grid_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_components/test_medium.py` & `tidy3d-2.2.2/tests/test_components/test_medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_components/test_meshgenerate.py` & `tidy3d-2.2.2/tests/test_components/test_meshgenerate.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_components/test_mode.py` & `tidy3d-2.2.2/tests/test_components/test_mode.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_components/test_monitor.py` & `tidy3d-2.2.2/tests/test_components/test_monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_components/test_sidewall.py` & `tidy3d-2.2.2/tests/test_components/test_sidewall.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_components/test_simulation.py` & `tidy3d-2.2.2/tests/test_components/test_simulation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_components/test_source.py` & `tidy3d-2.2.2/tests/test_components/test_source.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_components/test_types.py` & `tidy3d-2.2.2/tests/test_components/test_types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_data/test_data_arrays.py` & `tidy3d-2.2.2/tests/test_data/test_data_arrays.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_data/test_monitor_data.py` & `tidy3d-2.2.2/tests/test_data/test_monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_data/test_sim_data.py` & `tidy3d-2.2.2/tests/test_data/test_sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_package/test_config.py` & `tidy3d-2.2.2/tests/test_package/test_config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_package/test_log.py` & `tidy3d-2.2.2/tests/test_package/test_log.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_package/test_make_script.py` & `tidy3d-2.2.2/tests/test_package/test_make_script.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_package/test_material_library.py` & `tidy3d-2.2.2/tests/test_package/test_material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_package/test_parametric_variants.py` & `tidy3d-2.2.2/tests/test_package/test_parametric_variants.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_plugins/test_adjoint.py` & `tidy3d-2.2.2/tests/test_plugins/test_adjoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,43 +7,37 @@
 import jax.numpy as jnp
 import numpy as np
 from jax import grad, custom_vjp
 import jax
 from numpy.random import random
 import time
 import matplotlib.pylab as plt
+import h5py
 
 import tidy3d as td
 from typing import Tuple, Any, List
 
 from tidy3d.exceptions import DataError, Tidy3dKeyError, AdjointError
 from tidy3d.plugins.adjoint.components.base import JaxObject
 from tidy3d.plugins.adjoint.components.geometry import JaxBox, JaxPolySlab, MAX_NUM_VERTICES
 from tidy3d.plugins.adjoint.components.medium import JaxMedium, JaxAnisotropicMedium
 from tidy3d.plugins.adjoint.components.medium import JaxCustomMedium, MAX_NUM_CELLS_CUSTOM_MEDIUM
 from tidy3d.plugins.adjoint.components.structure import JaxStructure
 from tidy3d.plugins.adjoint.components.simulation import JaxSimulation, JaxInfo
 from tidy3d.plugins.adjoint.components.data.sim_data import JaxSimulationData
 from tidy3d.plugins.adjoint.components.data.monitor_data import JaxModeData, JaxDiffractionData
-from tidy3d.plugins.adjoint.components.data.data_array import JaxDataArray
+from tidy3d.plugins.adjoint.components.data.data_array import JaxDataArray, JAX_DATA_ARRAY_TAG
 from tidy3d.plugins.adjoint.components.data.dataset import JaxPermittivityDataset
 from tidy3d.plugins.adjoint.web import run, run_async
 from tidy3d.plugins.adjoint.web import run_local, run_async_local
 from tidy3d.plugins.adjoint.components.data.data_array import VALUE_FILTER_THRESHOLD
 from tidy3d.web.container import BatchData
 
-from ..utils import (
-    run_emulated,
-    assert_log_level,
-    log_capture,
-    run_async_emulated,
-    SIM_DATA_PATH,
-    SIM_FULL,
-    TMP_DIR,
-)
+from ..utils import run_emulated, assert_log_level, log_capture, run_async_emulated
+from ..utils import SIM_DATA_PATH, SIM_FULL, TMP_DIR
 
 FWD_SIM_DATA_FILE = TMP_DIR + "adjoint_grad_data_fwd.hdf5"
 SIM_VJP_FILE = TMP_DIR + "adjoint_sim_vjp_file.hdf5"
 RUN_PATH = TMP_DIR + "simulation.hdf5"
 
 EPS = 2.0
 SIZE = (1.0, 2.0, 3.0)
@@ -1213,7 +1207,55 @@
         jax_eps_dataset = JaxPermittivityDataset(**field_components)
         return JaxCustomMedium(eps_dataset=jax_eps_dataset)
 
     make_custom_medium(num_cells=1)
     make_custom_medium(num_cells=MAX_NUM_CELLS_CUSTOM_MEDIUM)
     with pytest.raises(pydantic.ValidationError):
         make_custom_medium(num_cells=MAX_NUM_CELLS_CUSTOM_MEDIUM + 1)
+
+
+def test_jax_sim_io():
+
+    jax_box = JaxBox(size=(1, 1, 1), center=(0, 0, 0))
+
+    def make_custom_medium(num_cells: int) -> JaxCustomMedium:
+
+        n = int(np.sqrt(num_cells))
+        Nx = n
+        Ny = n
+        Nz = 1
+
+        # custom medium
+        (xmin, ymin, zmin), (xmax, ymax, zmax) = jax_box.bounds
+        coords = dict(
+            x=np.linspace(xmin, xmax, Nx).tolist(),
+            y=np.linspace(ymin, ymax, Ny).tolist(),
+            z=np.linspace(zmin, zmax, Nz).tolist(),
+            f=[FREQ0],
+        )
+
+        values = np.random.random((Nx, Ny, Nz, 1)) + 1.0
+        eps_ii = JaxDataArray(values=values, coords=coords)
+        field_components = {f"eps_{dim}{dim}": eps_ii for dim in "xyz"}
+        jax_eps_dataset = JaxPermittivityDataset(**field_components)
+        return JaxCustomMedium(eps_dataset=jax_eps_dataset)
+
+    num_cells = 200 * 200
+    struct = JaxStructure(geometry=jax_box, medium=make_custom_medium(num_cells=num_cells))
+    sim = JaxSimulation(
+        size=(2, 2, 2),
+        input_structures=[struct],
+        run_time=1e-12,
+        grid_spec=td.GridSpec.auto(wavelength=1.0),
+    )
+
+    fname = "tests/tmp/jax_sim_io_tmp.hdf5"
+    sim.to_file(fname)
+
+    with h5py.File(fname, "r") as f:
+        assert "input_structures" in f.keys()
+        json_string = str(f["JSON_STRING"][()])
+        assert JAX_DATA_ARRAY_TAG in json_string
+
+    sim2 = JaxSimulation.from_file(fname)
+
+    assert sim == sim2
```

### Comparing `tidy3d-2.2.1/tests/test_plugins/test_component_modeler.py` & `tidy3d-2.2.2/tests/test_plugins/test_component_modeler.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_plugins/test_dispersion_fitter.py` & `tidy3d-2.2.2/tests/test_plugins/test_dispersion_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_plugins/test_mode_solver.py` & `tidy3d-2.2.2/tests/test_plugins/test_mode_solver.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_plugins/test_polyslab.py` & `tidy3d-2.2.2/tests/test_plugins/test_polyslab.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_plugins/test_resonance_finder.py` & `tidy3d-2.2.2/tests/test_plugins/test_resonance_finder.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_plugins/test_waveguide.py` & `tidy3d-2.2.2/tests/test_plugins/test_waveguide.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_web/test_auth.py` & `tidy3d-2.2.2/tests/test_web/test_auth.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_web/test_cli.py` & `tidy3d-2.2.2/tests/test_web/test_cli.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_web/test_material_fitter.py` & `tidy3d-2.2.2/tests/test_web/test_material_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_web/test_tidy3d_folder.py` & `tidy3d-2.2.2/tests/test_web/test_tidy3d_folder.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_web/test_tidy3d_material_library.py` & `tidy3d-2.2.2/tests/test_web/test_tidy3d_material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_web/test_tidy3d_task.py` & `tidy3d-2.2.2/tests/test_web/test_tidy3d_task.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/test_web/test_webapi.py` & `tidy3d-2.2.2/tests/test_web/test_webapi.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tests/utils.py` & `tidy3d-2.2.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/__init__.py` & `tidy3d-2.2.2/tidy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/__main__.py` & `tidy3d-2.2.2/tidy3d/__main__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/components/apodization.py` & `tidy3d-2.2.2/tidy3d/components/apodization.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/components/base.py` & `tidy3d-2.2.2/tidy3d/components/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # pylint:disable=too-many-public-methods
 """global configuration / base class for pydantic models used to make simulation."""
 from __future__ import annotations
 
 import json
 from functools import wraps
+from typing import List, Callable
 
 import rich
 import pydantic
 from pydantic.fields import ModelField
 import yaml
 import numpy as np
 import h5py
@@ -406,23 +407,29 @@
                     tuple_index = cls.get_tuple_index(key_name=key)
                     model_dict = model_dict[tuple_index]
                 else:
                     model_dict = model_dict[key]
         return model_dict
 
     @classmethod
-    def dict_from_hdf5(cls, fname: str, group_path: str = "") -> dict:
+    def dict_from_hdf5(
+        cls, fname: str, group_path: str = "", custom_decoders: List[Callable] = None
+    ) -> dict:
         """Loads a dictionary containing the model contents from a .hdf5 file.
 
         Parameters
         ----------
         fname : str
             Full path to the .hdf5 file to load the :class:`Tidy3dBaseModel` from.
         group_path : str, optional
             Path to a group inside the file to selectively load a sub-element of the model only.
+        custom_decoders : List[Callable]
+            List of functions accepting
+            (fname: str, group_path: str, model_dict: dict, key: str, value: Any) that store the
+            value in the model dict after a custom decoding.
 
         Returns
         -------
         dict
             Dictionary containing the model.
 
         Example
@@ -433,14 +440,25 @@
         def load_data_from_file(model_dict: dict, group_path: str = "") -> None:
             """For every DataArray item in dictionary, load path of hdf5 group as value."""
 
             for key, value in model_dict.items():
 
                 subpath = f"{group_path}/{key}"
 
+                # apply custom validation to the key value pair and modify model_dict
+                if custom_decoders:
+                    for custom_decoder in custom_decoders:
+                        custom_decoder(
+                            fname=fname,
+                            group_path=subpath,
+                            model_dict=model_dict,
+                            key=key,
+                            value=value,
+                        )
+
                 # write the path to the element of the json dict where the data_array should be
                 if isinstance(value, str) and value in DATA_ARRAY_MAP:
                     data_array_type = DATA_ARRAY_MAP[value]
                     model_dict[key] = data_array_type.from_hdf5(fname=fname, group_path=subpath)
                     continue
 
                 # if a list, assign each element a unique key, recurse
@@ -458,43 +476,58 @@
 
         group_path = cls._construct_group_path(group_path)
         model_dict = cls.get_sub_model(group_path=group_path, model_dict=model_dict)
         load_data_from_file(model_dict=model_dict, group_path=group_path)
         return model_dict
 
     @classmethod
-    def from_hdf5(cls, fname: str, group_path: str = "", **parse_obj_kwargs) -> Tidy3dBaseModel:
+    def from_hdf5(
+        cls,
+        fname: str,
+        group_path: str = "",
+        custom_decoders: List[Callable] = None,
+        **parse_obj_kwargs,
+    ) -> Tidy3dBaseModel:
         """Loads :class:`Tidy3dBaseModel` instance to .hdf5 file.
 
         Parameters
         ----------
         fname : str
             Full path to the .hdf5 file to load the :class:`Tidy3dBaseModel` from.
         group_path : str, optional
             Path to a group inside the file to selectively load a sub-element of the model only.
             Starting `/` is optional.
+        custom_decoders : List[Callable]
+            List of functions accepting
+            (fname: str, group_path: str, model_dict: dict, key: str, value: Any) that store the
+            value in the model dict after a custom decoding.
         **parse_obj_kwargs
             Keyword arguments passed to pydantic's ``parse_obj`` method.
 
         Example
         -------
         >>> simulation = Simulation.from_file(fname='folder/sim.hdf5') # doctest: +SKIP
         """
 
         group_path = cls._construct_group_path(group_path)
-        model_dict = cls.dict_from_hdf5(fname=fname, group_path=group_path)
+        model_dict = cls.dict_from_hdf5(
+            fname=fname, group_path=group_path, custom_decoders=custom_decoders
+        )
         return cls.parse_obj(model_dict, **parse_obj_kwargs)
 
-    def to_hdf5(self, fname: str) -> None:
+    def to_hdf5(self, fname: str, custom_encoders: List[Callable] = None) -> None:
         """Exports :class:`Tidy3dBaseModel` instance to .hdf5 file.
 
         Parameters
         ----------
         fname : str
             Full path to the .hdf5 file to save the :class:`Tidy3dBaseModel` to.
+        custom_encoders : List[Callable]
+            List of functions accepting (fname: str, group_path: str, value: Any) that take
+            the ``value`` supplied and write it to the hdf5 ``fname`` at ``group_path``.
 
         Example
         -------
         >>> simulation.to_hdf5(fname='folder/sim.hdf5') # doctest: +SKIP
         """
 
         with h5py.File(fname, "w") as f_handle:
@@ -505,14 +538,18 @@
                 """For every DataArray item in dictionary, write path of hdf5 group as value."""
 
                 for key, value in data_dict.items():
 
                     # append the key to the path
                     subpath = f"{group_path}/{key}"
 
+                    if custom_encoders:
+                        for custom_encoder in custom_encoders:
+                            custom_encoder(fname=f_handle, group_path=subpath, value=value)
+
                     # write the path to the element of the json dict where the data_array should be
                     if isinstance(value, xr.DataArray):
                         value.to_hdf5(fname=f_handle, group_path=subpath)
 
                     # if a tuple, assign each element a unique key
                     if isinstance(value, (list, tuple)):
                         value_dict = self.tuple_to_dict(tuple_values=value)
```

### Comparing `tidy3d-2.2.1/tidy3d/components/boundary.py` & `tidy3d-2.2.2/tidy3d/components/boundary.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/components/data/data_array.py` & `tidy3d-2.2.2/tidy3d/components/data/data_array.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/components/data/dataset.py` & `tidy3d-2.2.2/tidy3d/components/data/dataset.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/components/data/monitor_data.py` & `tidy3d-2.2.2/tidy3d/components/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/components/data/sim_data.py` & `tidy3d-2.2.2/tidy3d/components/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/components/field_projection.py` & `tidy3d-2.2.2/tidy3d/components/field_projection.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/components/geometry.py` & `tidy3d-2.2.2/tidy3d/components/geometry.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/components/grid/grid.py` & `tidy3d-2.2.2/tidy3d/components/grid/grid.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/components/grid/grid_spec.py` & `tidy3d-2.2.2/tidy3d/components/grid/grid_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/components/grid/mesher.py` & `tidy3d-2.2.2/tidy3d/components/grid/mesher.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/components/medium.py` & `tidy3d-2.2.2/tidy3d/components/medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/components/mode.py` & `tidy3d-2.2.2/tidy3d/components/mode.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/components/monitor.py` & `tidy3d-2.2.2/tidy3d/components/monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/components/simulation.py` & `tidy3d-2.2.2/tidy3d/components/simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -971,14 +971,18 @@
             tfsf_surfaces = Source.surfaces(
                 center=source.center, size=source.size, source_time=source.source_time
             )
             sidewall_surfaces = []
             sidewall_structs = []
             # get the structures that intersect each sidewall
             for surface in tfsf_surfaces:
+                # ignore the sidewall surface if it falls outside the simulation domain
+                if not self.intersects(surface):
+                    continue
+
                 if surface.name[-2] != "xyz"[source.injection_axis]:
                     sidewall_surfaces.append(surface)
                     intersecting_structs = self.intersecting_structures(
                         test_object=surface, structures=self.structures
                     )
 
                     if any(
```

### Comparing `tidy3d-2.2.1/tidy3d/components/source.py` & `tidy3d-2.2.2/tidy3d/components/source.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/components/structure.py` & `tidy3d-2.2.2/tidy3d/components/structure.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/components/transformation.py` & `tidy3d-2.2.2/tidy3d/components/transformation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/components/types.py` & `tidy3d-2.2.2/tidy3d/components/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/components/validators.py` & `tidy3d-2.2.2/tidy3d/components/validators.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/components/viz.py` & `tidy3d-2.2.2/tidy3d/components/viz.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/config.py` & `tidy3d-2.2.2/tidy3d/config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/constants.py` & `tidy3d-2.2.2/tidy3d/constants.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/exceptions.py` & `tidy3d-2.2.2/tidy3d/exceptions.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/log.py` & `tidy3d-2.2.2/tidy3d/log.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/material_library/material_library.py` & `tidy3d-2.2.2/tidy3d/material_library/material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/material_library/material_reference.py` & `tidy3d-2.2.2/tidy3d/material_library/material_reference.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/material_library/parametric_materials.py` & `tidy3d-2.2.2/tidy3d/material_library/parametric_materials.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/plugins/adjoint/__init__.py` & `tidy3d-2.2.2/tidy3d/plugins/adjoint/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/plugins/adjoint/components/data/data_array.py` & `tidy3d-2.2.2/tidy3d/plugins/adjoint/components/data/data_array.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 """Defines jax-compatible DataArrays."""
 from __future__ import annotations
 
 from typing import Tuple, Any, Dict, List
 
+import h5py
 import pydantic as pd
 import numpy as np
 import jax.numpy as jnp
 from jax.tree_util import register_pytree_node_class
+
 from .....components.base import Tidy3dBaseModel, cached_property
 from .....exceptions import DataError, Tidy3dKeyError, AdjointError
 
 
 # condition setting when to set value in DataArray to zero:
 # if abs(val) <= VALUE_FILTER_THRESHOLD * max(abs(val))
 VALUE_FILTER_THRESHOLD = 1e-6
 
+# JaxDataArrays are written to json as JAX_DATA_ARRAY_TAG
+JAX_DATA_ARRAY_TAG = "<<JaxDataArray>>"
+
 
 @register_pytree_node_class
 class JaxDataArray(Tidy3dBaseModel):
     """A :class:`.DataArray`-like class that only wraps xarray for jax compability."""
 
     values: Any = pd.Field(
         ...,
@@ -71,14 +76,50 @@
     #             raise AdjointError(
     #                 f"coordinate '{coord_name}' has '{len(coord_list)}' elements, "
     #                 f"expected '{len_dim}' to match number of 'values' along this dimension."
     #             )
 
     #     return val
 
+    # pylint: disable=arguments-differ, arguments-renamed
+    def to_hdf5(self, fname: str, group_path: str) -> None:
+        """Save an xr.DataArray to the hdf5 file with a given path to the group."""
+        sub_group = fname.create_group(group_path)
+        sub_group["values"] = self.values
+        dims = []
+        for key, val in self.coords.items():
+            # sub_group[key] = val
+            dims.append(key)
+            val = np.array(val)
+            if val.dtype == "<U1":
+                sub_group[key] = val.tolist()
+            else:
+                sub_group[key] = val
+        sub_group["dims"] = dims
+
+    # pylint: disable=arguments-differ
+    @classmethod
+    def from_hdf5(cls, fname: str, group_path: str) -> JaxDataArray:
+        """Load an DataArray from an hdf5 file with a given path to the group."""
+        with h5py.File(fname, "r") as f:
+            sub_group = f[group_path]
+            values = np.array(sub_group["values"])
+            dims = sub_group["dims"]
+            coords = {dim: np.array(sub_group[dim]) for dim in dims}
+            for key, val in coords.items():
+                val = np.array(val)
+                if val.dtype == "O":
+                    coords[key] = [byte_string.decode() for byte_string in val.tolist()]
+
+            coords = {
+                key: val.tolist() if isinstance(val, np.ndarray) else val
+                for key, val in coords.items()
+            }
+            return cls(values=values, coords=coords)
+
     @cached_property
     def as_ndarray(self) -> np.ndarray:
         """``self.values`` as a numpy array."""
         if not isinstance(self.values, np.ndarray):
             return np.array(self.values)
         return self.values
```

### Comparing `tidy3d-2.2.1/tidy3d/plugins/adjoint/components/data/dataset.py` & `tidy3d-2.2.2/tidy3d/plugins/adjoint/components/data/dataset.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/plugins/adjoint/components/data/monitor_data.py` & `tidy3d-2.2.2/tidy3d/plugins/adjoint/components/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/plugins/adjoint/components/data/sim_data.py` & `tidy3d-2.2.2/tidy3d/plugins/adjoint/components/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/plugins/adjoint/components/geometry.py` & `tidy3d-2.2.2/tidy3d/plugins/adjoint/components/geometry.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/plugins/adjoint/components/medium.py` & `tidy3d-2.2.2/tidy3d/plugins/adjoint/components/medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/plugins/adjoint/components/simulation.py` & `tidy3d-2.2.2/tidy3d/plugins/adjoint/components/simulation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/plugins/adjoint/components/structure.py` & `tidy3d-2.2.2/tidy3d/plugins/adjoint/components/structure.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/plugins/adjoint/components/types.py` & `tidy3d-2.2.2/tidy3d/plugins/adjoint/components/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/plugins/adjoint/web.py` & `tidy3d-2.2.2/tidy3d/plugins/adjoint/web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/plugins/dispersion/fit.py` & `tidy3d-2.2.2/tidy3d/plugins/dispersion/fit.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/plugins/dispersion/fit_web.py` & `tidy3d-2.2.2/tidy3d/plugins/dispersion/fit_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/plugins/mode/derivatives.py` & `tidy3d-2.2.2/tidy3d/plugins/mode/derivatives.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/plugins/mode/mode_solver.py` & `tidy3d-2.2.2/tidy3d/plugins/mode/mode_solver.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/plugins/mode/solver.py` & `tidy3d-2.2.2/tidy3d/plugins/mode/solver.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/plugins/mode/transforms.py` & `tidy3d-2.2.2/tidy3d/plugins/mode/transforms.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/plugins/polyslab/polyslab.py` & `tidy3d-2.2.2/tidy3d/plugins/polyslab/polyslab.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/plugins/resonance/resonance.py` & `tidy3d-2.2.2/tidy3d/plugins/resonance/resonance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/plugins/smatrix/smatrix.py` & `tidy3d-2.2.2/tidy3d/plugins/smatrix/smatrix.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/plugins/waveguide/rectangular_dielectric.py` & `tidy3d-2.2.2/tidy3d/plugins/waveguide/rectangular_dielectric.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/updater.py` & `tidy3d-2.2.2/tidy3d/updater.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/web/__init__.py` & `tidy3d-2.2.2/tidy3d/web/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/web/asynchronous.py` & `tidy3d-2.2.2/tidy3d/web/asynchronous.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/web/auth.py` & `tidy3d-2.2.2/tidy3d/web/auth.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/web/cacert.pem` & `tidy3d-2.2.2/tidy3d/web/cacert.pem`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/web/cli/app.py` & `tidy3d-2.2.2/tidy3d/web/cli/app.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/web/cli/migrate.py` & `tidy3d-2.2.2/tidy3d/web/cli/migrate.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/web/config.py` & `tidy3d-2.2.2/tidy3d/web/config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/web/container.py` & `tidy3d-2.2.2/tidy3d/web/container.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/web/environment.py` & `tidy3d-2.2.2/tidy3d/web/environment.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/web/http_management.py` & `tidy3d-2.2.2/tidy3d/web/http_management.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/web/httputils.py` & `tidy3d-2.2.2/tidy3d/web/httputils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/web/material_fitter.py` & `tidy3d-2.2.2/tidy3d/web/material_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/web/material_libray.py` & `tidy3d-2.2.2/tidy3d/web/material_libray.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/web/s3utils.py` & `tidy3d-2.2.2/tidy3d/web/s3utils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/web/simulation_task.py` & `tidy3d-2.2.2/tidy3d/web/simulation_task.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/web/task.py` & `tidy3d-2.2.2/tidy3d/web/task.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/web/types.py` & `tidy3d-2.2.2/tidy3d/web/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d/web/webapi.py` & `tidy3d-2.2.2/tidy3d/web/webapi.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d.egg-info/PKG-INFO` & `tidy3d-2.2.2/tidy3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy3d
-Version: 2.2.1
+Version: 2.2.2
 Summary: A fast FDTD solver
 Home-page: https://github.com/flexcompute/tidy3d
 Author: Tyler Hughes
 Author-email: tyler@flexcompute.com
 Project-URL: Bug Tracker, https://github.com/flexcompute/tidy3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy3d-2.2.1/tidy3d.egg-info/SOURCES.txt` & `tidy3d-2.2.2/tidy3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tidy3d-2.2.1/tidy3d.egg-info/requires.txt` & `tidy3d-2.2.2/tidy3d.egg-info/requires.txt`

 * *Files identical despite different names*

