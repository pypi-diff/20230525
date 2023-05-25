# Comparing `tmp/static-frame-1.4.2.tar.gz` & `tmp/static-frame-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static-frame-1.4.2.tar", last modified: Tue May  9 01:49:39 2023, max compression
+gzip compressed data, was "static-frame-1.4.3.tar", last modified: Thu May 25 17:31:23 2023, max compression
```

## Comparing `static-frame-1.4.2.tar` & `static-frame-1.4.3.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-09 01:49:39.262997 static-frame-1.4.2/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1777 2022-09-18 23:42:20.000000 static-frame-1.4.2/LICENSE.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      105 2022-08-07 22:56:47.000000 static-frame-1.4.2/MANIFEST.in
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    22828 2023-05-09 01:49:39.262997 static-frame-1.4.2/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23553 2023-05-09 00:42:47.000000 static-frame-1.4.2/README.rst
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      144 2022-09-18 23:42:20.000000 static-frame-1.4.2/requirements-extras.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      363 2023-05-09 00:42:47.000000 static-frame-1.4.2/requirements-test.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       46 2023-05-09 00:42:47.000000 static-frame-1.4.2/requirements.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       77 2023-05-09 01:49:39.262997 static-frame-1.4.2/setup.cfg
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3777 2023-01-27 15:25:04.000000 static-frame-1.4.2/setup.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-09 01:49:39.254998 static-frame-1.4.2/static_frame/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7660 2023-05-09 01:09:37.000000 static-frame-1.4.2/static_frame/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1573 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/__main__.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-09 01:49:39.258997 static-frame-1.4.2/static_frame/core/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.4.2/static_frame/core/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    44502 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/core/archive_npy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      223 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/assign.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3979 2023-03-31 18:53:08.000000 static-frame-1.4.2/static_frame/core/axis_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    58179 2023-02-23 20:10:49.000000 static-frame-1.4.2/static_frame/core/batch.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    50681 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/core/bus.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    24157 2023-02-27 23:01:10.000000 static-frame-1.4.2/static_frame/core/container.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    70699 2023-04-14 20:39:45.000000 static-frame-1.4.2/static_frame/core/container_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35163 2022-10-01 15:52:09.000000 static-frame-1.4.2/static_frame/core/display.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9232 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/display_color.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17470 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/display_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1599 2022-08-07 22:56:47.000000 static-frame-1.4.2/static_frame/core/display_html_datatables.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15864 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/display_visidata.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    28891 2023-03-28 21:18:03.000000 static-frame-1.4.2/static_frame/core/doc_str.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3524 2023-02-23 22:39:48.000000 static-frame-1.4.2/static_frame/core/exception.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3098 2022-08-07 22:56:47.000000 static-frame-1.4.2/static_frame/core/fill_value_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   378205 2023-05-09 00:42:47.000000 static-frame-1.4.2/static_frame/core/frame.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1141 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/core/hloc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    56830 2023-05-04 22:17:10.000000 static-frame-1.4.2/static_frame/core/index.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6466 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/core/index_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17792 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/core/index_base.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5455 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/index_correspondence.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    21196 2023-05-04 22:17:10.000000 static-frame-1.4.2/static_frame/core/index_datetime.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   107720 2023-05-04 22:17:10.000000 static-frame-1.4.2/static_frame/core/index_hierarchy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    16869 2023-02-01 00:09:42.000000 static-frame-1.4.2/static_frame/core/index_hierarchy_set_utils.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    47042 2023-01-28 23:33:40.000000 static-frame-1.4.2/static_frame/core/interface.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      514 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/interface_meta.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15041 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/core/join.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23859 2023-05-04 22:17:10.000000 static-frame-1.4.2/static_frame/core/loc_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9635 2023-01-28 23:33:40.000000 static-frame-1.4.2/static_frame/core/memory_measure.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35539 2023-03-28 21:18:03.000000 static-frame-1.4.2/static_frame/core/node_dt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    24034 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/node_fill_value.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5312 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/core/node_hashlib.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    31896 2023-05-02 20:46:35.000000 static-frame-1.4.2/static_frame/core/node_iter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14190 2023-03-28 21:18:03.000000 static-frame-1.4.2/static_frame/core/node_re.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    12353 2023-02-28 22:54:13.000000 static-frame-1.4.2/static_frame/core/node_selector.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    34445 2022-11-10 00:09:54.000000 static-frame-1.4.2/static_frame/core/node_str.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15388 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/node_transpose.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    10016 2023-02-27 23:39:36.000000 static-frame-1.4.2/static_frame/core/node_values.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    31469 2022-10-13 03:47:27.000000 static-frame-1.4.2/static_frame/core/pivot.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1623 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/platform.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11771 2022-09-29 04:16:16.000000 static-frame-1.4.2/static_frame/core/protocol_dfi.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17337 2022-09-29 04:16:16.000000 static-frame-1.4.2/static_frame/core/protocol_dfi_abc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    53391 2023-03-31 18:53:08.000000 static-frame-1.4.2/static_frame/core/quilt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4631 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/rank.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   127657 2023-03-31 18:53:08.000000 static-frame-1.4.2/static_frame/core/series.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9996 2023-02-21 22:37:54.000000 static-frame-1.4.2/static_frame/core/store.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6249 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/store_client_mixin.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14881 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/store_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14880 2023-05-08 23:21:40.000000 static-frame-1.4.2/static_frame/core/store_filter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5888 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/store_hdf5.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7057 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/store_sqlite.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    26087 2023-02-03 19:24:20.000000 static-frame-1.4.2/static_frame/core/store_xlsx.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    21183 2023-02-23 22:39:48.000000 static-frame-1.4.2/static_frame/core/store_zip.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5117 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/core/style_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   185709 2023-05-05 18:43:53.000000 static-frame-1.4.2/static_frame/core/type_blocks.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   129022 2023-05-08 23:21:40.000000 static-frame-1.4.2/static_frame/core/util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9952 2022-12-20 03:10:29.000000 static-frame-1.4.2/static_frame/core/www.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    27762 2023-02-28 22:54:13.000000 static-frame-1.4.2/static_frame/core/yarn.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.4.2/static_frame/py.typed
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-09 01:49:39.258997 static-frame-1.4.2/static_frame/test/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.4.2/static_frame/test/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11984 2023-01-30 03:11:00.000000 static-frame-1.4.2/static_frame/test/test_case.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-09 01:49:39.262997 static-frame-1.4.2/static_frame/test/unit/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.4.2/static_frame/test/unit/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    25950 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_archive_npy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7340 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_axis_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   138362 2023-02-23 22:39:48.000000 static-frame-1.4.2/static_frame/test/unit/test_batch.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    81209 2023-02-21 22:37:54.000000 static-frame-1.4.2/static_frame/test/unit/test_bus.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      599 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_container.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35986 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/test/unit/test_container_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    36712 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_display.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_display_color.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      358 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_display_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5247 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/test/unit/test_doc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      937 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_fill_value_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   641433 2023-05-09 00:42:47.000000 static-frame-1.4.2/static_frame/test/unit/test_frame.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2254 2022-08-07 22:56:47.000000 static-frame-1.4.2/static_frame/test/unit/test_frame_he.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    60358 2023-05-02 20:46:35.000000 static-frame-1.4.2/static_frame/test/unit/test_frame_iter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    31756 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/test/unit/test_frame_join.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6644 2022-08-07 22:56:47.000000 static-frame-1.4.2/static_frame/test/unit/test_frame_via_fill_value.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5022 2022-08-07 22:56:47.000000 static-frame-1.4.2/static_frame/test/unit/test_frame_via_re.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2317 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_hloc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    64304 2023-05-04 22:17:10.000000 static-frame-1.4.2/static_frame/test/unit/test_index.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4044 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/test/unit/test_index_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1323 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_index_base.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2023-05-04 22:17:10.000000 static-frame-1.4.2/static_frame/test/unit/test_index_correspondence.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    41844 2023-05-04 22:17:10.000000 static-frame-1.4.2/static_frame/test/unit/test_index_datetime.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   164808 2023-02-28 22:54:13.000000 static-frame-1.4.2/static_frame/test/unit/test_index_hierarchy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3526 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/test/unit/test_index_hierarchy_set_utils.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5856 2023-05-09 00:42:47.000000 static-frame-1.4.2/static_frame/test/unit/test_interface.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    19608 2023-05-04 22:17:10.000000 static-frame-1.4.2/static_frame/test/unit/test_loc_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    16279 2023-05-04 22:17:10.000000 static-frame-1.4.2/static_frame/test/unit/test_memory_measure.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23164 2023-05-05 18:43:53.000000 static-frame-1.4.2/static_frame/test/unit/test_memory_measure_getsizeof.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4455 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_pivot.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      373 2022-08-07 22:56:47.000000 static-frame-1.4.2/static_frame/test/unit/test_platform.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15253 2022-09-29 04:16:16.000000 static-frame-1.4.2/static_frame/test/unit/test_protocol_dfi.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    73785 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/test/unit/test_quilt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11263 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_rank.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   242465 2023-05-02 20:46:35.000000 static-frame-1.4.2/static_frame/test/unit/test_series.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2384 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_series_he.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    13468 2023-02-21 22:37:54.000000 static-frame-1.4.2/static_frame/test/unit/test_store.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14506 2023-05-08 23:21:40.000000 static-frame-1.4.2/static_frame/test/unit/test_store_filter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7409 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_store_hdf5.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     8114 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_store_sqlite.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15968 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_store_xlsx.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17381 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_store_zip.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      884 2022-09-18 23:42:20.000000 static-frame-1.4.2/static_frame/test/unit/test_style_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   162493 2023-01-27 15:25:04.000000 static-frame-1.4.2/static_frame/test/unit/test_type_blocks.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   116937 2023-03-31 18:53:08.000000 static-frame-1.4.2/static_frame/test/unit/test_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    10401 2023-05-09 00:42:47.000000 static-frame-1.4.2/static_frame/test/unit/test_www.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    47732 2023-05-04 22:17:10.000000 static-frame-1.4.2/static_frame/test/unit/test_yarn.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-09 01:49:39.254998 static-frame-1.4.2/static_frame.egg-info/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    22828 2023-05-09 01:49:39.000000 static-frame-1.4.2/static_frame.egg-info/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4328 2023-05-09 01:49:39.000000 static-frame-1.4.2/static_frame.egg-info/SOURCES.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-05-09 01:49:39.000000 static-frame-1.4.2/static_frame.egg-info/dependency_links.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      200 2023-05-09 01:49:39.000000 static-frame-1.4.2/static_frame.egg-info/requires.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       13 2023-05-09 01:49:39.000000 static-frame-1.4.2/static_frame.egg-info/top_level.txt
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-25 17:31:23.212648 static-frame-1.4.3/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1777 2023-03-23 21:26:53.000000 static-frame-1.4.3/LICENSE.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      105 2022-01-11 20:49:28.000000 static-frame-1.4.3/MANIFEST.in
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    22828 2023-05-25 17:31:23.212648 static-frame-1.4.3/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    23553 2023-05-25 17:28:32.000000 static-frame-1.4.3/README.rst
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      144 2023-03-23 21:26:53.000000 static-frame-1.4.3/requirements-extras.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      363 2023-05-25 17:28:32.000000 static-frame-1.4.3/requirements-test.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       46 2023-05-25 17:28:32.000000 static-frame-1.4.3/requirements.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       77 2023-05-25 17:31:23.212648 static-frame-1.4.3/setup.cfg
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3777 2023-03-23 21:26:53.000000 static-frame-1.4.3/setup.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-25 17:31:23.196648 static-frame-1.4.3/static_frame/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7638 2023-05-25 17:28:32.000000 static-frame-1.4.3/static_frame/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1573 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/__main__.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-25 17:31:23.204648 static-frame-1.4.3/static_frame/core/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.3/static_frame/core/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    44502 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/archive_npy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      223 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/assign.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5475 2023-05-16 23:32:31.000000 static-frame-1.4.3/static_frame/core/axis_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    58179 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/batch.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    50681 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/bus.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    24157 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/container.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    70680 2023-05-25 17:28:32.000000 static-frame-1.4.3/static_frame/core/container_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    35163 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/display.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9232 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/display_color.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17470 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/display_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1599 2022-01-11 20:49:28.000000 static-frame-1.4.3/static_frame/core/display_html_datatables.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15864 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/display_visidata.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    28891 2023-04-19 18:21:25.000000 static-frame-1.4.3/static_frame/core/doc_str.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3447 2023-05-25 17:28:32.000000 static-frame-1.4.3/static_frame/core/exception.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3098 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/fill_value_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   378509 2023-05-25 17:28:32.000000 static-frame-1.4.3/static_frame/core/frame.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1141 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/hloc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    56897 2023-05-25 17:28:32.000000 static-frame-1.4.3/static_frame/core/index.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6466 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/index_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17792 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/index_base.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5455 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/index_correspondence.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    21196 2023-05-04 17:09:05.000000 static-frame-1.4.3/static_frame/core/index_datetime.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   107732 2023-05-25 17:28:32.000000 static-frame-1.4.3/static_frame/core/index_hierarchy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    16869 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/index_hierarchy_set_utils.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    47042 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/interface.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      514 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/interface_meta.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15041 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/join.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    23859 2023-05-04 17:09:05.000000 static-frame-1.4.3/static_frame/core/loc_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9635 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/memory_measure.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    35827 2023-05-25 15:11:48.000000 static-frame-1.4.3/static_frame/core/node_dt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    24236 2023-05-25 15:11:48.000000 static-frame-1.4.3/static_frame/core/node_fill_value.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5312 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/node_hashlib.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    31896 2023-04-24 22:32:18.000000 static-frame-1.4.3/static_frame/core/node_iter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14190 2023-04-19 18:21:25.000000 static-frame-1.4.3/static_frame/core/node_re.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    12353 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/node_selector.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    34445 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/node_str.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15388 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/node_transpose.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    10018 2023-05-25 17:28:32.000000 static-frame-1.4.3/static_frame/core/node_values.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    31469 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/pivot.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1623 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/platform.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11771 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/protocol_dfi.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17337 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/protocol_dfi_abc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    53391 2023-04-19 18:21:25.000000 static-frame-1.4.3/static_frame/core/quilt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4631 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/rank.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   127343 2023-05-25 15:11:48.000000 static-frame-1.4.3/static_frame/core/series.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9996 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/store.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6249 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/store_client_mixin.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14881 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/store_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14880 2023-05-12 15:14:12.000000 static-frame-1.4.3/static_frame/core/store_filter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5888 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/store_hdf5.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7057 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/store_sqlite.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    26087 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/store_xlsx.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    21183 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/store_zip.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5117 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/style_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   178010 2023-05-25 17:28:32.000000 static-frame-1.4.3/static_frame/core/type_blocks.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   129082 2023-05-25 17:28:32.000000 static-frame-1.4.3/static_frame/core/util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9952 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/www.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    27762 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/core/yarn.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.3/static_frame/py.typed
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-25 17:31:23.204648 static-frame-1.4.3/static_frame/test/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.3/static_frame/test/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11984 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/test_case.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-25 17:31:23.212648 static-frame-1.4.3/static_frame/test/unit/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.3/static_frame/test/unit/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    25950 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_archive_npy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7340 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_axis_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   138362 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_batch.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    81209 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_bus.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      599 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_container.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    35989 2023-05-25 17:28:32.000000 static-frame-1.4.3/static_frame/test/unit/test_container_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    36712 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_display.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_display_color.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      358 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_display_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5247 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_doc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      937 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_fill_value_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   642225 2023-05-25 17:28:32.000000 static-frame-1.4.3/static_frame/test/unit/test_frame.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2254 2022-03-15 15:56:11.000000 static-frame-1.4.3/static_frame/test/unit/test_frame_he.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    60358 2023-04-24 22:32:18.000000 static-frame-1.4.3/static_frame/test/unit/test_frame_iter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    31756 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_frame_join.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6644 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_frame_via_fill_value.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5022 2022-03-15 15:56:11.000000 static-frame-1.4.3/static_frame/test/unit/test_frame_via_re.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2317 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_hloc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    64304 2023-05-04 17:09:05.000000 static-frame-1.4.3/static_frame/test/unit/test_index.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4044 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_index_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1323 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_index_base.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2023-05-04 17:09:05.000000 static-frame-1.4.3/static_frame/test/unit/test_index_correspondence.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    41844 2023-05-04 17:09:05.000000 static-frame-1.4.3/static_frame/test/unit/test_index_datetime.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   164692 2023-05-16 23:32:31.000000 static-frame-1.4.3/static_frame/test/unit/test_index_hierarchy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3526 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_index_hierarchy_set_utils.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5856 2023-05-12 15:14:12.000000 static-frame-1.4.3/static_frame/test/unit/test_interface.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    19608 2023-05-04 17:09:05.000000 static-frame-1.4.3/static_frame/test/unit/test_loc_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    16279 2023-05-04 17:09:05.000000 static-frame-1.4.3/static_frame/test/unit/test_memory_measure.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    22632 2023-05-25 17:28:32.000000 static-frame-1.4.3/static_frame/test/unit/test_memory_measure_getsizeof.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4455 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_pivot.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      373 2022-03-15 15:56:11.000000 static-frame-1.4.3/static_frame/test/unit/test_platform.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15253 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_protocol_dfi.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    74931 2023-05-16 23:32:31.000000 static-frame-1.4.3/static_frame/test/unit/test_quilt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11263 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_rank.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   244185 2023-05-25 15:11:48.000000 static-frame-1.4.3/static_frame/test/unit/test_series.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2384 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_series_he.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    13468 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_store.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14506 2023-05-12 15:14:12.000000 static-frame-1.4.3/static_frame/test/unit/test_store_filter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7409 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_store_hdf5.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     8114 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_store_sqlite.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15968 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_store_xlsx.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17381 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_store_zip.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      884 2023-03-23 21:26:53.000000 static-frame-1.4.3/static_frame/test/unit/test_style_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   161330 2023-05-25 17:28:32.000000 static-frame-1.4.3/static_frame/test/unit/test_type_blocks.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   114907 2023-05-25 17:28:32.000000 static-frame-1.4.3/static_frame/test/unit/test_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    10401 2023-05-12 15:14:12.000000 static-frame-1.4.3/static_frame/test/unit/test_www.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    47732 2023-05-04 17:09:05.000000 static-frame-1.4.3/static_frame/test/unit/test_yarn.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-05-25 17:31:23.196648 static-frame-1.4.3/static_frame.egg-info/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    22828 2023-05-25 17:31:23.000000 static-frame-1.4.3/static_frame.egg-info/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4328 2023-05-25 17:31:23.000000 static-frame-1.4.3/static_frame.egg-info/SOURCES.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-05-25 17:31:23.000000 static-frame-1.4.3/static_frame.egg-info/dependency_links.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      200 2023-05-25 17:31:23.000000 static-frame-1.4.3/static_frame.egg-info/requires.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       13 2023-05-25 17:31:23.000000 static-frame-1.4.3/static_frame.egg-info/top_level.txt
```

### Comparing `static-frame-1.4.2/LICENSE.txt` & `static-frame-1.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/PKG-INFO` & `static-frame-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame
-Version: 1.4.2
+Version: 1.4.3
 Summary: Immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface.
 Home-page: https://github.com/static-frame/static-frame
 Author: Christopher Ariza
 License: MIT
 Description: A library of immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface. StaticFrame is suitable for applications in data science, data engineering, finance, scientific computing, and related fields where reducing opportunities for error by prohibiting in-place mutation is critical.
         
         While many interfaces are similar to Pandas, StaticFrame deviates from Pandas in many ways: all data is immutable, and all indices are unique; the full range of NumPy data types is preserved, and date-time indices use discrete NumPy units; hierarchical indices are seamlessly integrated; and uniform approaches to element, row, and column iteration and function application are provided. Core StaticFrame depends only on NumPy and two C-extension packages (maintained by the StaticFrame team): Pandas is not a dependency.
@@ -46,15 +46,15 @@
         --------------
         
         Core StaticFrame requires the following:
         
         - Python>=3.7
         - NumPy>=1.18.5
         - arraymap==0.1.8
-        - arraykit==0.3.4
+        - arraykit==0.4.8
         
         For extended input and output, the following packages are required:
         
         - pandas>=0.24.2
         - xlsxwriter>=1.1.2
         - openpyxl>=3.0.9
         - xarray>=0.13.0
```

### Comparing `static-frame-1.4.2/README.rst` & `static-frame-1.4.3/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 --------------
 
 Core StaticFrame requires the following:
 
 - Python>=3.7
 - NumPy>=1.18.5
 - arraymap==0.1.8
-- arraykit==0.3.4
+- arraykit==0.4.8
 
 For extended input and output, the following packages are required:
 
 - pandas>=0.24.2
 - xlsxwriter>=1.1.2
 - openpyxl>=3.0.9
 - xarray>=0.13.0
```

### Comparing `static-frame-1.4.2/setup.py` & `static-frame-1.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/__init__.py` & `static-frame-1.4.3/static_frame/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #pylint: disable=W0611
 #pylint: disable=C0414
 
 # We import the names "as" themselves here (and here only) to tell linting tools
 # that they are explicitly being exported here (and not just unused).
+from arraykit import ErrorInitTypeBlocks
 from arraykit import isna_element as isna_element
 from arraykit import mloc as mloc
 
 from static_frame.core.archive_npy import NPY as NPY
 from static_frame.core.archive_npy import NPZ as NPZ
 from static_frame.core.batch import Batch as Batch
 from static_frame.core.bus import Bus as Bus
@@ -14,21 +15,20 @@
 from static_frame.core.display import DisplayActive as DisplayActive
 from static_frame.core.display_config import DisplayConfig as DisplayConfig
 from static_frame.core.display_config import DisplayConfigs as DisplayConfigs
 from static_frame.core.display_config import DisplayFormats as DisplayFormats
 from static_frame.core.exception import AxisInvalid
 from static_frame.core.exception import ErrorInit
 from static_frame.core.exception import ErrorInitBus
+from static_frame.core.exception import ErrorInitColumns
 from static_frame.core.exception import ErrorInitFrame
 from static_frame.core.exception import ErrorInitIndex
-from static_frame.core.exception import ErrorInitIndexLevel
 from static_frame.core.exception import ErrorInitSeries
 from static_frame.core.exception import ErrorInitStore
 from static_frame.core.exception import ErrorInitStoreConfig
-from static_frame.core.exception import ErrorInitTypeBlocks
 from static_frame.core.exception import LocEmpty
 from static_frame.core.exception import LocInvalid
 from static_frame.core.exception import StoreFileMutation
 from static_frame.core.fill_value_auto import FillValueAuto as FillValueAuto
 from static_frame.core.frame import Frame as Frame
 from static_frame.core.frame import FrameAssign as FrameAssign
 from static_frame.core.frame import FrameAssignBLoc as FrameAssignBLoc
@@ -115,8 +115,8 @@
 from static_frame.core.util import IndexSpecifier as IndexSpecifier
 from static_frame.core.util import KeyOrKeys as KeyOrKeys
 from static_frame.core.util import PathSpecifierOrFileLike as PathSpecifierOrFileLike
 from static_frame.core.util import SeriesInitializer as SeriesInitializer
 from static_frame.core.www import WWW
 from static_frame.core.yarn import Yarn as Yarn
 
-__version__ = '1.4.2'
+__version__ = '1.4.3'
```

### Comparing `static-frame-1.4.2/static_frame/__main__.py` & `static-frame-1.4.3/static_frame/__main__.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/archive_npy.py` & `static-frame-1.4.3/static_frame/core/archive_npy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/axis_map.py` & `static-frame-1.4.3/static_frame/core/axis_map.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 from copy import deepcopy
 from functools import partial
 
 from arraykit import array_deepcopy
 
 from static_frame.core.bus import Bus
 from static_frame.core.exception import AxisInvalid
+from static_frame.core.frame import Frame
 from static_frame.core.index_auto import IndexAutoConstructorFactory
 from static_frame.core.index_base import IndexBase
 from static_frame.core.index_hierarchy import IndexHierarchy
+from static_frame.core.index_hierarchy import IndexHierarchyGO
 from static_frame.core.index_hierarchy import TreeNodeT
 from static_frame.core.util import AnyCallable
 
 if tp.TYPE_CHECKING:
     from static_frame.core.yarn import Yarn  # pylint: disable=W0611 #pragma: no cover
 
 
@@ -29,45 +31,86 @@
         memo: tp.Optional[tp.Dict[int, tp.Any]] = None if not memo_active else {}
         if is_array:
             return partial(array_deepcopy, memo=memo)
         return partial(deepcopy, memo=memo)
     return lambda x: x
 
 
+def _bus_to_hierarchy_inner_hierarchies(
+        bus: tp.Union[Bus, 'Yarn'],
+        axis: int,
+        extractor: tp.Callable[[IndexBase], IndexBase],
+        init_exception_cls: tp.Type[Exception],
+        ) -> tp.Tuple[IndexHierarchy, IndexBase]:
+    '''
+    Specialized version of :func:`bus_to_hierarchy` for the case where Bus's frames contains only hierarchical indices on the axis of concatentation
+    '''
+    opposite: tp.Optional[IndexBase] = None
+
+    def level_add(pair: tp.Tuple[tp.Hashable, Frame]) -> IndexHierarchy:
+        nonlocal opposite
+        label, frame = pair
+
+        if axis == 0:
+            axis0, axis1 = extractor(frame.index), frame.columns
+        else:
+            assert axis == 1
+            axis0, axis1 = extractor(frame.columns), frame.index
+
+        if opposite is None:
+            opposite = extractor(axis1)
+        else:
+            if not opposite.equals(axis1):
+                raise init_exception_cls('opposite axis must have equivalent indices')
+
+        assert isinstance(axis0, IndexHierarchy) # true assert
+        return axis0.level_add(label)
+
+    items_iter = iter(bus.items())
+
+    primary = IndexHierarchyGO(level_add(next(items_iter)))
+
+    for level in items_iter:
+        primary.extend(level_add(level))
+
+    return IndexHierarchy(primary), opposite # type: ignore
+
+
 def bus_to_hierarchy(
         bus: tp.Union[Bus, 'Yarn'],
         axis: int,
         deepcopy_from_bus: bool,
         init_exception_cls: tp.Type[Exception],
         ) -> tp.Tuple[IndexHierarchy, IndexBase]:
     '''
     Given a :obj:`Bus` and an axis, derive a :obj:`IndexHierarchy`; also return and validate the :obj:`Index` of the opposite axis.
     '''
     # NOTE: need to extract just axis labels, not the full Frame; need new Store/Bus loaders just for label data
     extractor = get_extractor(deepcopy_from_bus, is_array=False, memo_active=False)
 
-    def tree_extractor(index: IndexBase) -> tp.Union[IndexBase, TreeNodeT]:
-        index = extractor(index)
-        if isinstance(index, IndexHierarchy):
-            return index.to_tree()
-        return index
+    first = tp.cast(Frame, bus.iloc[0])
+    if (
+        (axis == 0 and isinstance(first.index, IndexHierarchy)) or
+        (axis == 1 and isinstance(first.columns, IndexHierarchy))
+    ):
+        return _bus_to_hierarchy_inner_hierarchies(bus, axis, extractor, init_exception_cls)
 
     tree: TreeNodeT = {}
     opposite: tp.Optional[IndexBase] = None
 
     for label, f in bus.items():
         if axis == 0:
-            tree[label] = tree_extractor(f.index)
+            tree[label] = extractor(f.index)
             if opposite is None:
                 opposite = extractor(f.columns)
             else:
                 if not opposite.equals(f.columns):
                     raise init_exception_cls('opposite axis must have equivalent indices')
         elif axis == 1:
-            tree[label] = tree_extractor(f.columns)
+            tree[label] = extractor(f.columns)
             if opposite is None:
                 opposite = extractor(f.index)
             else:
                 if not opposite.equals(f.index):
                     raise init_exception_cls('opposite axis must have equivalent indices')
         else:
             raise AxisInvalid(f'invalid axis {axis}')
```

### Comparing `static-frame-1.4.2/static_frame/core/batch.py` & `static-frame-1.4.3/static_frame/core/batch.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/bus.py` & `static-frame-1.4.3/static_frame/core/bus.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/container.py` & `static-frame-1.4.3/static_frame/core/container.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/container_util.py` & `static-frame-1.4.3/static_frame/core/container_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from fractions import Fraction
 from functools import partial
 from itertools import zip_longest
 
 import numpy as np
 from arraykit import column_2d_filter
 from arraykit import resolve_dtype_iter
+from arraykit import slice_to_ascending_slice
 from numpy import char as npc
 
 from static_frame.core.container import ContainerBase
 from static_frame.core.container import ContainerOperand
 from static_frame.core.exception import AxisInvalid
 from static_frame.core.exception import ErrorInitIndex
 from static_frame.core.fill_value_auto import FillValueAuto
@@ -46,15 +47,14 @@
 from static_frame.core.util import UFunc
 from static_frame.core.util import WarningsSilent
 from static_frame.core.util import concat_resolved
 from static_frame.core.util import is_dtype_specifier
 from static_frame.core.util import is_mapping
 from static_frame.core.util import iterable_to_array_1d
 from static_frame.core.util import iterable_to_array_2d
-from static_frame.core.util import slice_to_ascending_slice
 from static_frame.core.util import ufunc_set_iter
 from static_frame.core.util import ufunc_unique1d
 from static_frame.core.util import ufunc_unique2d
 from static_frame.core.util import validate_dtype_specifier
 
 if tp.TYPE_CHECKING:
     import pandas as pd  # pylint: disable=W0611 #pragma: no cover
@@ -934,15 +934,15 @@
     Args:
         size: the length of the container on this axis
     '''
     from static_frame.core.frame import Frame
     from static_frame.core.series import Series
 
     if key.__class__ is slice:
-        return slice_to_ascending_slice(key, size=size) #type: ignore
+        return slice_to_ascending_slice(key, size) #type: ignore
 
     if isinstance(key, str) or not hasattr(key, '__len__'):
         return key
 
     if key.__class__ is np.ndarray:
         # array first as not truthy
         if key.dtype == DTYPE_BOOL: #type: ignore
```

### Comparing `static-frame-1.4.2/static_frame/core/display.py` & `static-frame-1.4.3/static_frame/core/display.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/display_color.py` & `static-frame-1.4.3/static_frame/core/display_color.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/display_config.py` & `static-frame-1.4.3/static_frame/core/display_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/display_html_datatables.py` & `static-frame-1.4.3/static_frame/core/display_html_datatables.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/display_visidata.py` & `static-frame-1.4.3/static_frame/core/display_visidata.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/doc_str.py` & `static-frame-1.4.3/static_frame/core/doc_str.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/exception.py` & `static-frame-1.4.3/static_frame/core/exception.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,36 +2,32 @@
 import warnings
 
 
 class ErrorInit(RuntimeError):
     '''Error in Container initialization.
     '''
 
-class ErrorInitTypeBlocks(ErrorInit):
-    '''Error in TypeBlocks initialization.
-    '''
-
 class ErrorInitSeries(ErrorInit):
     '''Error in Series initialization.
     '''
 
 class ErrorInitFrame(ErrorInit):
     '''Error in Frame (and derived Frame) initialization.
     '''
 
 class ErrorInitIndex(ErrorInit):
     '''Error in IndexBase (and derived Index) initialization.
     '''
 
-class ErrorInitIndexNonUnique(ErrorInitIndex):
-    '''Error in IndexBase initialization due to non-unique values.
+class ErrorInitColumns(ErrorInitIndex):
+    '''Error in IndexBase (and derived Index) initialization of columns.
     '''
 
-class ErrorInitIndexLevel(ErrorInit):
-    '''Error in IndexBase (and derived Index) initialization.
+class ErrorInitIndexNonUnique(ErrorInitIndex):
+    '''Error in IndexBase initialization due to non-unique values.
     '''
 
 class ErrorInitBus(ErrorInit):
     '''Error in Bus initialization.
     '''
 
 class ErrorInitQuilt(ErrorInit):
```

### Comparing `static-frame-1.4.2/static_frame/core/fill_value_auto.py` & `static-frame-1.4.3/static_frame/core/fill_value_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/frame.py` & `static-frame-1.4.3/static_frame/core/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,17 @@
 from static_frame.core.display import Display
 from static_frame.core.display import DisplayActive
 from static_frame.core.display import DisplayHeader
 from static_frame.core.display_config import DisplayConfig
 from static_frame.core.display_config import DisplayFormats
 from static_frame.core.doc_str import doc_inject
 from static_frame.core.exception import AxisInvalid
+from static_frame.core.exception import ErrorInitColumns
 from static_frame.core.exception import ErrorInitFrame
+from static_frame.core.exception import ErrorInitIndex
 from static_frame.core.exception import ErrorInitIndexNonUnique
 from static_frame.core.exception import InvalidFillValue
 from static_frame.core.exception import RelabelInvalid
 from static_frame.core.index import Index
 from static_frame.core.index import IndexGO
 from static_frame.core.index import _index_initializer_needs_init
 from static_frame.core.index import immutable_index_filter
@@ -731,15 +733,15 @@
 
         fill_arrays = {} # NOTE: we will hash to NaN and NaT, but can assume we are using the same instance
 
         containers_iter = iter(containers)
         container = next(containers_iter)
 
         if fill_value is FILL_VALUE_DEFAULT:
-            fill_value_reindex = dtype_kind_to_na(container._blocks._row_dtype.kind)
+            fill_value_reindex = dtype_kind_to_na(container._blocks._index.dtype.kind)
         else:
             fill_value_reindex = fill_value # just pass along even if FillValueAuto
 
         # get the first container
         post = frame_to_frame(container, cls).reindex(
                 index=index,
                 columns=columns,
@@ -3281,15 +3283,15 @@
             raise ErrorInitFrame('use Frame.from_dict to create a Frame from a mapping.')
         elif isinstance(data, Series):
             raise ErrorInitFrame('use Frame.from_series to create a Frame from a Series.')
         else:
             raise ErrorInitFrame('use Frame.from_element, Frame.from_elements, or Frame.from_records to create a Frame from 0, 1, or 2 dimensional untyped data (respectively).')
 
         # counts can be zero (not None) if _block was created but is empty
-        row_count, col_count = (self._blocks._shape
+        row_count, col_count = (self._blocks.shape
                 if not blocks_constructor else (None, None))
 
         self._name = None if name is NAME_DEFAULT else name_filter(name)
 
         #-----------------------------------------------------------------------
         # columns assignment
 
@@ -3300,22 +3302,26 @@
             col_count = 0 if col_count is None else col_count
             self._columns = IndexAutoFactory.from_optional_constructor(
                     col_count,
                     default_constructor=self._COLUMNS_CONSTRUCTOR,
                     explicit_constructor=columns_constructor
                     )
         else:
-            self._columns = index_from_optional_constructor(columns,
-                    default_constructor=self._COLUMNS_CONSTRUCTOR,
-                    explicit_constructor=columns_constructor
-                    )
+            try:
+                self._columns = index_from_optional_constructor(columns,
+                        default_constructor=self._COLUMNS_CONSTRUCTOR,
+                        explicit_constructor=columns_constructor
+                        )
+            except ErrorInitIndex as e: # show this as a column exception
+                raise ErrorInitColumns(str(e)) from None
+
             col_count = len(self._columns)
         # check after creation, as we cannot determine from the constructor (it might be a method on a class)
         if self._COLUMNS_CONSTRUCTOR.STATIC != self._columns.STATIC:
-            raise ErrorInitFrame(f'supplied column constructor does not match required static attribute: {self._COLUMNS_CONSTRUCTOR.STATIC}')
+            raise ErrorInitFrame(f'Supplied `columns_constructor` does not match required static attribute: {self._COLUMNS_CONSTRUCTOR.STATIC}')
 
         #-----------------------------------------------------------------------
         # index assignment
 
         if own_index:
             self._index = index # type: ignore
             row_count = len(self._index)
@@ -4616,15 +4622,15 @@
                 name=self._name,
                 own_index=True,
                 own_columns=self.STATIC,
                 own_data=True,
                 )
         # NOTE: we branch based on value type to use more efficient TypeBlock methods when we know we have an element or a 2D array
         if isinstance(value, Frame):
-            fill_value = dtype_to_fill_value(value._blocks._row_dtype)
+            fill_value = dtype_to_fill_value(value._blocks._index.dtype)
             fill = value.reindex(
                     index=self.index,
                     columns=self.columns,
                     fill_value=fill_value
                     ).values
             # produce a Boolean array that shows True only for labels (index, columns) found in the original `value` argument (before reindexing) and also in the target; this will be used to not set a NA when the value to fill was produced by reindexing.
             fill_valid = self._blocks.extract_iloc_mask((
@@ -4819,15 +4825,15 @@
                 own_data=True)
 
     #---------------------------------------------------------------------------
 
     def __len__(self) -> int:
         '''Length of rows in values.
         '''
-        return self._blocks._shape[0]
+        return self._blocks._index.rows
 
     @doc_inject()
     def display(self,
             config: tp.Optional[DisplayConfig] = None,
             *,
             style_config: tp.Optional[StyleConfig] = None,
             ) -> Display:
@@ -4899,15 +4905,15 @@
     def shape(self) -> tp.Tuple[int, int]:
         '''
         Return a tuple describing the shape of the underlying NumPy array.
 
         Returns:
             :obj:`tp.Tuple[int, int]`
         '''
-        return self._blocks._shape
+        return self._blocks._index.shape
 
     @property
     def ndim(self) -> int:
         '''
         Return the number of dimensions, which for a `Frame` is always 2.
 
         Returns:
@@ -4996,15 +5002,15 @@
             columns = self._columns._extract_iloc(column_key) # type: ignore
             own_columns = True
             if not column_key_is_slice and isinstance(column_key, INT_TYPES):
                 name_column = self._columns._extract_iloc_by_int(column_key)
 
         # determine if an axis is not multi; if one axis is not multi, we return a Series instead of a Frame
         axis_nm = self._extract_axis_not_multi(row_key, column_key)
-        blocks_shape = blocks._shape
+        blocks_shape = blocks.shape
 
         if blocks_shape[0] == 0 or blocks_shape[1] == 0:
             # return a 0-sized Series, `blocks` is already extracted
             array = column_1d_filter(blocks._blocks[0]) if blocks._blocks else EMPTY_ARRAY
             if axis_nm[0]: # if row not multi
                 return Series(array,
                         index=immutable_index_filter(columns),
@@ -5591,15 +5597,15 @@
 
         Args:
             as_array: if True, return arrays instead of ``Frame``
         '''
         blocks = self._blocks
 
         if drop:
-            shape = blocks._shape[1] if axis == 0 else blocks._shape[0]
+            shape = blocks._index.columns if axis == 0 else blocks._index.rows
             drop_mask = np.full(shape, True, dtype=DTYPE_BOOL)
             drop_mask[key] = False
 
         # NOTE: in limited studies using stable does not show significant overhead
         kind = DEFAULT_STABLE_SORT_KIND if stable else DEFAULT_FAST_SORT_KIND
         try:
             blocks, ordering = blocks.sort(key=key, axis=not axis, kind=kind)
@@ -6834,15 +6840,15 @@
             start: int = 0,
             fill_value: tp.Any = np.nan,
     ) -> 'Frame':
 
         if axis == 1 and is_fill_value_factory_initializer(fill_value):
             raise InvalidFillValue(fill_value, 'axis==1')
 
-        shape = self._blocks._shape
+        shape = self._blocks.shape
         asc_is_element = isinstance(ascending, BOOL_TYPES)
 
         if not asc_is_element:
             ascending = tuple(ascending)
             opposite_axis = int(not axis)
             if len(ascending) != shape[opposite_axis]:
                 raise RuntimeError(f'Multiple ascending values must match length of axis {opposite_axis}.')
@@ -7078,15 +7084,15 @@
         if not skipna and skipfalsy:
             raise RuntimeError('Cannot skipfalsy and not skipna.')
 
         labels = self._columns if axis == 0 else self._index
 
         if not skipna and not skipfalsy and not unique:
             array = np.full(len(labels),
-                    self._blocks._shape[axis],
+                    self._blocks.shape[axis],
                     dtype=DTYPE_INT_DEFAULT,
                     )
         else:
             array = np.empty(len(labels), dtype=DTYPE_INT_DEFAULT)
             for i, values in enumerate(self._blocks.axis_values(axis=axis)):
                 valid: tp.Optional[np.ndarray] = None
 
@@ -8461,15 +8467,15 @@
         else:
             columns_tuples = tuple((l,) for l in self._columns.values)
 
         # immutability should be preserved
         array = self._blocks.values.reshape(self._blocks.size)
 
         def labels() -> tp.Iterator[tp.Hashable]:
-            for row, col in np.ndindex(self._blocks._shape):
+            for row, col in np.ndindex(self._blocks.shape):
                 yield index_tuples[row] + columns_tuples[col]
 
         index = index_constructor(labels())
         name = name if name is not NAME_DEFAULT else self._name
 
         return Series(array, index=index, own_index=True, name=name)
 
@@ -8591,15 +8597,15 @@
                 # write the rest of the line
                 if store_filter:
                     row.extend(f'{filter_func(x)}' for x in columns_row)
                 else:
                     row.extend(f'{x}' for x in columns_row)
                 yield row
 
-        col_idx_last = self._blocks._shape[1] - 1
+        col_idx_last = self._blocks._index.columns - 1
         # avoid row creation to avoid joining types; avoide creating a list for each row
         row_current_idx: tp.Optional[int] = None
 
         for (row_idx, col_idx), element in self._iter_element_iloc_items():
             if row_idx != row_current_idx: # each new row
                 if row_current_idx is not None: # if not the first
                     yield row
@@ -9166,15 +9172,15 @@
             self._columns.extend(container.keys())
             self._blocks.extend(container._blocks)
         elif isinstance(container, Series):
             self._columns.append(container.name)
             self._blocks.append(container.values)
 
         # this should never happen, and is hard to test!
-        assert len(self._columns) == self._blocks._shape[1] #pragma: no cover
+        assert len(self._columns) == self._blocks._index.columns #pragma: no cover
 
     #---------------------------------------------------------------------------
     def via_fill_value(self,
             fill_value: object = np.nan,
             ) -> InterfaceFillValueGO['Frame']:
         '''
         Interface for using binary operators and methods with a pre-defined fill value.
```

### Comparing `static-frame-1.4.2/static_frame/core/hloc.py` & `static-frame-1.4.3/static_frame/core/hloc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/index.py` & `static-frame-1.4.3/static_frame/core/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,20 +355,20 @@
             size = len(self._map)
 
         # this might be NP array, or a list, depending on if static or grow only; if an array, dtype will be compared with passed dtype_extract
         self._labels = self._extract_labels(self._map, labels, dtype_extract)
         self._positions = self._extract_positions(size, positions)
 
         if self._DTYPE and self._labels.dtype != self._DTYPE:
-            raise ErrorInitIndex('Invalid label dtype for this Index', #pragma: no cover
+            raise ErrorInitIndex('Invalid label dtype for this Index.', #pragma: no cover
                     self._labels.dtype, self._DTYPE)
 
         # NOTE: to implement GH # 374; do this after final self._labels creation as user may pass a dtype argument
         if not is_typed and self._labels.dtype.kind == DTYPE_DATETIME_KIND:
-            raise ErrorInitIndex('Cannot create an Index with a datetime64 array; use an Index subclass (e.g. IndexDate) or supply an `index_constructors` argument')
+            raise ErrorInitIndex(f'Cannot create an `Index` with a `datetime64` array (with `dtype` {self._labels.dtype} and including {self._labels[:10]}); use a subclass (e.g. `IndexDate`) directly or as a constructor argument.')
 
     #---------------------------------------------------------------------------
 
     def __setstate__(self, state: tp.Tuple[None, tp.Dict[str, tp.Any]]) -> None:
         '''
         Ensure that reanimated NP arrays are set not writeable.
         '''
```

### Comparing `static-frame-1.4.2/static_frame/core/index_auto.py` & `static-frame-1.4.3/static_frame/core/index_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/index_base.py` & `static-frame-1.4.3/static_frame/core/index_base.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/index_correspondence.py` & `static-frame-1.4.3/static_frame/core/index_correspondence.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/index_datetime.py` & `static-frame-1.4.3/static_frame/core/index_datetime.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/index_hierarchy.py` & `static-frame-1.4.3/static_frame/core/index_hierarchy.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,15 +297,14 @@
         Builds the IndexHierarchy name from the names of `indices`. If one is not specified, the name is None
         '''
         name: SingleLabelType = tuple(index.name for index in indices)
         if any(n is None for n in name):
             return None
         return name
 
-
     @classmethod
     def from_pandas(cls: tp.Type[IH],
             value: 'pandas.MultiIndex',
             ) -> IH:
         '''
         Given a Pandas index, return the appropriate IndexBase derived class.
         '''
@@ -1310,15 +1309,15 @@
 
         Returns:
             :obj:`tp.Tuple[int]`
         '''
         if self._recache:
             return self.__len__(), self.depth
 
-        return self._blocks._shape
+        return self._blocks.shape
 
     @property
     def ndim(self: IH) -> int:
         '''
         Return the number of dimensions.
 
         Returns:
@@ -1527,15 +1526,14 @@
         if self._recache:
             self._update_array_cache()
 
         validate_depth_selection(depth_level)
 
         return self._indexers[depth_level]
 
-
     @doc_inject()
     def label_widths_at_depth(self: IH,
             depth_level: DepthLevelSpecifier = 0
             ) -> tp.Iterator[tp.Tuple[tp.Hashable, int]]:
         '''
         {}
         '''
@@ -1562,16 +1560,14 @@
         indexer = self._indexers[pos]
         index = self._indices[pos]
 
         ilocs, widths = run_length_1d(indexer)
 
         yield from zip(map(index._extract_iloc_by_int, ilocs), widths)
 
-
-
     @property
     def index_types(self: IH) -> 'Series':
         '''
         Return a Series of Index classes for each index depth.
 
         Returns:
             :obj:`Series`
@@ -2780,28 +2776,26 @@
             ) -> IH:
         '''
         Return an IndexHierarchy with a new root (outer) level added.
         '''
         if self._recache:
             self._update_array_cache()
 
-        index_cls = self._INDEX_CONSTRUCTOR if index_constructor is None else index_constructor._MUTABLE_CONSTRUCTOR # type: ignore
+        if index_constructor is None:
+            index_cls = self._INDEX_CONSTRUCTOR
+        else:
+            index_cls = index_constructor._IMMUTABLE_CONSTRUCTOR if self.STATIC else index_constructor._MUTABLE_CONSTRUCTOR # type: ignore
 
         if self.STATIC:
             indices = [index_cls((level,)), *self._indices]
         else:
             indices = [index_cls((level,)), *(idx.copy() for idx in self._indices)]
 
-        indexers = np.array(
-                [
-                    np.zeros(self.__len__(), dtype=DTYPE_INT_DEFAULT),
-                    *self._indexers
-                ],
-                dtype=DTYPE_INT_DEFAULT,
-        )
+        indexers = np.zeros((len(self._indexers) + 1, self.__len__()), dtype=DTYPE_INT_DEFAULT)
+        indexers[1:] = self._indexers
         indexers.flags.writeable = False
 
         def gen_blocks() -> tp.Iterator[np.ndarray]:
             # First index only has one value. Extract from array (instead of using `level`) since the constructor might have modified its type
             yield np.full(self.__len__(), indices[0][0])
             yield from self._blocks._blocks
```

### Comparing `static-frame-1.4.2/static_frame/core/index_hierarchy_set_utils.py` & `static-frame-1.4.3/static_frame/core/index_hierarchy_set_utils.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/interface.py` & `static-frame-1.4.3/static_frame/core/interface.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/interface_meta.py` & `static-frame-1.4.3/static_frame/core/interface_meta.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/join.py` & `static-frame-1.4.3/static_frame/core/join.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/loc_map.py` & `static-frame-1.4.3/static_frame/core/loc_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/memory_measure.py` & `static-frame-1.4.3/static_frame/core/memory_measure.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/node_dt.py` & `static-frame-1.4.3/static_frame/core/node_dt.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,17 +164,19 @@
 
     def _fill_missing_dt64(self, array_src: np.ndarray, array_dst: np.ndarray) -> np.ndarray:
         '''
         Args:
             array_src: The raw array, before any dytpe conversions; used to identify missing values.
             array_dst: The array post any conversions, to be filled with missing values.
         '''
-        if self._fill_value is not FILL_VALUE_DEFAULT:
-            targets = isna_array(array_src)
-            if targets.any():
+        targets = isna_array(array_src)
+        if targets.any():
+            if self._fill_value is FILL_VALUE_DEFAULT:
+                raise RuntimeError('Cannot convert NaT: provide a `fill_value` to `via_dt()`.')
+            else:
                 dt = resolve_dtype(array_dst.dtype, self._fill_value_dtype)
                 if dt != array_dst.dtype:
                     array_dst = array_dst.astype(dt)
                 array_dst[targets] = self._fill_value
 
         array_dst.flags.writeable = False
         return array_dst
@@ -183,14 +185,17 @@
             array: np.ndarray,
             *,
             method_name: str,
             args: tp.Tuple[tp.Any, ...],
             dtype: np.dtype,
             ) -> np.ndarray:
         if self._fill_value is FILL_VALUE_DEFAULT:
+            if isna_array(array).any():
+                raise RuntimeError('Cannot convert NaT: provide a `fill_value` to `via_dt()`.')
+
             array = array_from_element_method(
                     array=array,
                     method_name=method_name,
                     args=args,
                     dtype=dtype,
                     )
         else:
@@ -204,24 +209,26 @@
                 return getattr(e, method_name)(*args)
 
             array = array_from_element_apply(
                     array=array,
                     func=func,
                     dtype=dt,
                     )
-        assert array.flags.writeable is False
         return array
 
     def _fill_missing_element_attr(self,
             array: np.ndarray,
             *,
             attr_name: str,
             dtype: np.dtype,
             ) -> np.ndarray:
         if self._fill_value is FILL_VALUE_DEFAULT:
+            if isna_array(array).any():
+                raise RuntimeError('Cannot convert NaT: provide a `fill_value` to `via_dt()`.')
+
             array = array_from_element_attr(
                     array=array,
                     attr_name=attr_name,
                     dtype=dtype,
                     )
         else:
             dt = resolve_dtype(dtype, self._fill_value_dtype)
@@ -233,15 +240,14 @@
                 return getattr(e, attr_name)
 
             array = array_from_element_apply(
                     array=array,
                     func=func,
                     dtype=dt,
                     )
-        assert array.flags.writeable is False
         return array
 
     #---------------------------------------------------------------------------
     # date, datetime attributes
 
     @property
     def year(self) -> TContainer:
```

### Comparing `static-frame-1.4.2/static_frame/core/node_fill_value.py` & `static-frame-1.4.3/static_frame/core/node_fill_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,20 +97,25 @@
 
     #---------------------------------------------------------------------------
     @staticmethod
     def _extract_key_attrs(
             key: GetItemKeyType,
             index: 'IndexBase',
             ) -> tp.Tuple[GetItemKeyType, bool, bool]:
+        from static_frame.core.container_util import key_from_container_key
+
+        key = key_from_container_key(index, key, expand_iloc=True)
         key_is_multiple = isinstance(key, KEY_MULTIPLE_TYPES)
+
         if key.__class__ is slice:
             key_is_null_slice = key == NULL_SLICE
             key = index._extract_loc(key) #type: ignore
         else:
             key_is_null_slice = False
+
         return key, key_is_multiple, key_is_null_slice
 
     def _extract_loc1d(self,
             key: GetItemKeyType = NULL_SLICE,
             ) -> 'Series':
         '''This is only called if container is 1D
         '''
@@ -123,15 +128,15 @@
         fill_value = self._fill_value
         container = self._container
 
         if is_multiple:
             return container.reindex(key if not is_null_slice else None, #type: ignore
                     fill_value=fill_value,
                     )
-
+        # if a single value, return it or the fill value
         fv = get_col_fill_value_factory(fill_value, None)(0, container.dtype) #type: ignore
         return container.get(key, fv) #type: ignore
 
     def _extract_loc2d(self,
             row_key: GetItemKeyType = NULL_SLICE,
             column_key: GetItemKeyType = NULL_SLICE,
             ) -> tp.Union['Frame', 'Series']:
```

### Comparing `static-frame-1.4.2/static_frame/core/node_hashlib.py` & `static-frame-1.4.3/static_frame/core/node_hashlib.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/node_iter.py` & `static-frame-1.4.3/static_frame/core/node_iter.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/node_re.py` & `static-frame-1.4.3/static_frame/core/node_re.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/node_selector.py` & `static-frame-1.4.3/static_frame/core/node_selector.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/node_str.py` & `static-frame-1.4.3/static_frame/core/node_str.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/node_transpose.py` & `static-frame-1.4.3/static_frame/core/node_transpose.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/node_values.py` & `static-frame-1.4.3/static_frame/core/node_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             array.flags.writeable = False
             return array
 
         if self._container._NDIM == 2:
             blocks: tp.Iterable[np.ndarray] = self._container._blocks._blocks #type: ignore
 
             if self._unify_blocks:
-                dtype = self._container._blocks._row_dtype if self._dtype is None else self._dtype #type: ignore
+                dtype = self._container._blocks._index.dtype if self._dtype is None else self._dtype #type: ignore
                 tb = TypeBlocks.from_blocks(func(blocks_to_array_2d(
                         blocks=blocks,
                         shape=self._container.shape,
                         dtype=dtype,
                         )))
             elif self._consolidate_blocks:
                 if self._dtype is not None:
```

### Comparing `static-frame-1.4.2/static_frame/core/pivot.py` & `static-frame-1.4.3/static_frame/core/pivot.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/platform.py` & `static-frame-1.4.3/static_frame/core/platform.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/protocol_dfi.py` & `static-frame-1.4.3/static_frame/core/protocol_dfi.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/protocol_dfi_abc.py` & `static-frame-1.4.3/static_frame/core/protocol_dfi_abc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/quilt.py` & `static-frame-1.4.3/static_frame/core/quilt.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/rank.py` & `static-frame-1.4.3/static_frame/core/rank.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/series.py` & `static-frame-1.4.3/static_frame/core/series.py`

 * *Files 0% similar despite different names*

```diff
@@ -1894,19 +1894,14 @@
             Pandas supports taking in iterables of keys, where some keys are not found in the index; a Series is returned as if a reindex operation was performed. This is undesirable. Better instead is to use reindex()
         '''
         iloc_key = self._index._loc_to_iloc(key)
         values = self.values[iloc_key]
 
         if isinstance(iloc_key, INT_TYPES): # if we have a single element
             # NOTE: cannot check if we have an array as an array might be an element
-            # NOTE: this branch is not encountered and may not be necessary
-            # if isinstance(key, HLoc) and key.has_key_multiple():
-            #     # must return a Series, even though we do not have an array
-            #     values = np.array(values)
-            #     values.flags.writeable = False
             return values #type: ignore
 
         return self.__class__(values,
                 index=self._index.iloc[iloc_key],
                 own_index=True,
                 name=self._name)
```

### Comparing `static-frame-1.4.2/static_frame/core/store.py` & `static-frame-1.4.3/static_frame/core/store.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/store_client_mixin.py` & `static-frame-1.4.3/static_frame/core/store_client_mixin.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/store_config.py` & `static-frame-1.4.3/static_frame/core/store_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/store_filter.py` & `static-frame-1.4.3/static_frame/core/store_filter.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/store_hdf5.py` & `static-frame-1.4.3/static_frame/core/store_hdf5.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/store_sqlite.py` & `static-frame-1.4.3/static_frame/core/store_sqlite.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/store_xlsx.py` & `static-frame-1.4.3/static_frame/core/store_xlsx.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/store_zip.py` & `static-frame-1.4.3/static_frame/core/store_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/style_config.py` & `static-frame-1.4.3/static_frame/core/style_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/type_blocks.py` & `static-frame-1.4.3/static_frame/core/type_blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import typing as tp
-from copy import deepcopy
 from functools import partial
 from itertools import chain
 from itertools import repeat
 from itertools import zip_longest
 
 import numpy as np
+from arraykit import BlockIndex
+from arraykit import ErrorInitTypeBlocks
 from arraykit import array_deepcopy
 from arraykit import column_1d_filter
 from arraykit import column_2d_filter
 from arraykit import first_true_1d
 from arraykit import immutable_filter
 from arraykit import mloc
 from arraykit import resolve_dtype
@@ -22,22 +23,20 @@
 from static_frame.core.container_util import apply_binary_operator_blocks_columnar
 from static_frame.core.container_util import get_block_match
 from static_frame.core.display import Display
 from static_frame.core.display import DisplayActive
 from static_frame.core.display_config import DisplayConfig
 from static_frame.core.doc_str import doc_inject
 from static_frame.core.exception import AxisInvalid
-from static_frame.core.exception import ErrorInitTypeBlocks
 from static_frame.core.index_correspondence import IndexCorrespondence
 from static_frame.core.node_selector import InterfaceGetItem
 from static_frame.core.style_config import StyleConfig
 from static_frame.core.util import DEFAULT_FAST_SORT_KIND
 from static_frame.core.util import DEFAULT_SORT_KIND
 from static_frame.core.util import DTYPE_BOOL
-from static_frame.core.util import DTYPE_FLOAT_DEFAULT
 from static_frame.core.util import DTYPE_OBJECT
 from static_frame.core.util import EMPTY_ARRAY
 from static_frame.core.util import EMPTY_ARRAY_OBJECT
 from static_frame.core.util import FILL_VALUE_DEFAULT
 from static_frame.core.util import INT_TYPES
 from static_frame.core.util import KEY_ITERABLE_TYPES
 from static_frame.core.util import KEY_MULTIPLE_TYPES
@@ -64,15 +63,14 @@
 from static_frame.core.util import full_for_fill
 from static_frame.core.util import isfalsy_array
 from static_frame.core.util import isin_array
 from static_frame.core.util import isna_array
 from static_frame.core.util import iterable_to_array_1d
 from static_frame.core.util import iterable_to_array_nd
 from static_frame.core.util import roll_1d
-from static_frame.core.util import slice_to_ascending_slice
 from static_frame.core.util import slices_from_targets
 from static_frame.core.util import ufunc_dtype_to_dtype
 from static_frame.core.util import validate_dtype_specifier
 from static_frame.core.util import view_2d_as_1d
 
 #---------------------------------------------------------------------------
 
@@ -92,15 +90,15 @@
         drop: Optionally drop the target of the grouping as specified by ``key``.
         extract: if provided, will be used to select from the group on the opposite axis
 
     Returns:
         Generator of group, selection pairs, where selection is an np.ndarray. Returned is as an np.ndarray if key is more than one column.
     '''
     # NOTE: in axis_values we determine zero size by looking for empty _blocks; not sure if that is appropriate here.
-    if blocks._shape[0] == 0 or blocks._shape[1] == 0: # zero sized
+    if blocks._index.shape[0] == 0 or blocks._index.shape[1] == 0: # zero sized
         return
 
     unique_axis = None
 
     if group_source is not None:
         pass
     elif axis == 0:
@@ -123,15 +121,15 @@
         if axis == 0:
             groups = array2d_to_tuples(groups)
         else:
             groups = array2d_to_tuples(groups.T)
 
     if drop:
         # axis 0 means we return row groups; key is a column key
-        shape = blocks._shape[1] if axis == 0 else blocks._shape[0]
+        shape = blocks._index.shape[1] if axis == 0 else blocks._index.shape[0]
         drop_mask = np.full(shape, True, dtype=DTYPE_BOOL)
         drop_mask[key] = False
 
     column_key: tp.Union[int, np.ndarray, None]
     row_key: tp.Union[int, np.ndarray, None]
     # this key is used to select which components are returned per group selection (where that group selection is on the opposite axis)
 
@@ -191,15 +189,15 @@
     Returns:
         Generator of group, selection pairs, where selection is an np.ndarray. Returned is as an np.ndarray if key is more than one column.
     '''
     # if extract is not None drop must be False
     # assert extract is not None and drop is False
 
     # NOTE: in axis_values we determine zero size by looking for empty _blocks; not sure if that is appropriate here.
-    if blocks._shape[0] == 0 or blocks._shape[1] == 0: # zero sized
+    if blocks._index.shape[0] == 0 or blocks._index.shape[1] == 0: # zero sized
         return
 
     if group_source is not None:
         pass
         # NOTE: axis 1 transposition is not required as group_source is already prepared by h-stacking 1D arrays
     elif axis == 0:
         # axis 0 means we return row groups; key is a column key
@@ -210,15 +208,15 @@
         # for ndim==2, must present values from top to bottom
         group_source = group_source.T
     else:
         raise AxisInvalid(f'invalid axis: {axis}')
 
     if drop:
         # axis 0 means we return row groups; key is a column key
-        shape = blocks._shape[1] if axis == 0 else blocks._shape[0]
+        shape = blocks._index.shape[1] if axis == 0 else blocks._index.shape[0]
         drop_mask = np.full(shape, True, dtype=DTYPE_BOOL)
         drop_mask[key] = False
 
     column_key: tp.Union[int, np.ndarray, None]
     row_key: tp.Union[int, np.ndarray, None]
 
     func = blocks._extract_array if as_array else blocks._extract
@@ -417,16 +415,14 @@
 
     A TypeBlocks instance can have a zero size shape (where the length of one axis is zero). Internally, when axis 0 (rows) is of size 0, we store similarly sized arrays. When axis 1 (columns) is of size 0, we do not store arrays, as such arrays do not define a type (as types are defined by columns).
     '''
 
     __slots__ = (
             '_blocks',
             '_index',
-            '_shape',
-            '_row_dtype',
             )
 
     STATIC = False
 
     #---------------------------------------------------------------------------
     # constructors
 
@@ -442,79 +438,35 @@
 
         Args:
             raw_blocks: iterable (generator compatible) of NDArrays, or a single NDArray.
             shape_reference: optional argument to support cases where no blocks are found in the ``raw_blocks`` iterable, but the outer context is one with rows but no columns, or columns and no rows.
 
         '''
         blocks: tp.List[np.ndarray] = [] # ordered blocks
-        index: tp.List[tp.Tuple[int, int]] = [] # columns position to blocks key
-        block_count = 0
-
-        row_count: tp.Optional[int]
+        index = BlockIndex()
 
         # if a single block, no need to loop
         if raw_blocks.__class__ is np.ndarray:
-            if raw_blocks.ndim > 2: #type: ignore
-                raise ErrorInitTypeBlocks('arrays of dimensionality greater than 2 cannot be used to create TypeBlocks')
-
-            row_count, column_count = shape_filter(raw_blocks)
-            if column_count == 0:
-                # set shape but do not store array
-                return cls(blocks=blocks,
-                        index=index,
-                        shape=(row_count, column_count) #type: ignore
-                        )
-            blocks.append(immutable_filter(raw_blocks))
-            for i in range(column_count):
-                index.append((block_count, i))
-
+            if index.register(raw_blocks):
+                blocks.append(immutable_filter(raw_blocks))
         else: # an iterable of blocks
-            row_count = None
-            column_count = 0
-
             for block in raw_blocks:
-                if not block.__class__ is np.ndarray:
-                    raise ErrorInitTypeBlocks(f'found non array block: {block}')
-
-                if block.ndim > 2:
-                    raise ErrorInitTypeBlocks(f'cannot include array with {block.ndim} dimensions')
-
-                r, c = shape_filter(block)
-
-                # check number of rows is the same for all blocks
-                if row_count is not None and r != row_count: #type: ignore [unreachable]
-                    raise ErrorInitTypeBlocks(f'mismatched row count: {r}: {row_count}')
-                else: # assign on first
-                    row_count = r
-
                 # we keep array with 0 rows but > 0 columns, as they take type space in the TypeBlocks object; arrays with 0 columns do not take type space and thus can be skipped entirely
-                if c == 0:
-                    continue
-
-                blocks.append(immutable_filter(block))
-
-                # store position to key of block, block columns
-                for i in range(c):
-                    index.append((block_count, i))
-
-                column_count += c
-                block_count += 1
-
-        # blocks can be empty
-        if row_count is None:
-            if shape_reference is not None:
-                # if columns have gone to zero, and this was created from a TB that had rows, continue to represent those rows
-                row_count = shape_reference[0]
-            else:
-                raise ErrorInitTypeBlocks('cannot derive a row_count from blocks; provide a shape reference')
+                if index.register(block):
+                    blocks.append(immutable_filter(block))
 
+            # blocks can be empty, and index with no registration has rows as -1
+            if index.rows < 0:
+                if shape_reference is not None:
+                    index.register(EMPTY_ARRAY.reshape(shape_reference[0], 0))
+                else:
+                    raise ErrorInitTypeBlocks('cannot derive a row_count from blocks; provide a shape reference')
         return cls(
                 blocks=blocks,
                 index=index,
-                shape=(row_count, column_count),
                 )
 
     @classmethod
     def from_element_items(cls,
             items: tp.Iterable[tp.Tuple[tp.Tuple[int, ...], object]],
             shape: tp.Tuple[int, ...],
             dtype: np.dtype,
@@ -549,16 +501,16 @@
             if get_col_dtype is None:
                 blocks = np.empty(shape)
                 blocks.flags.writeable = False
             else:
                 blocks = (np.empty(rows, dtype=get_col_dtype(i)) for i in range(columns))
             return cls.from_blocks(blocks)
 
-        # for arrays with no width, favor storing shape alone and not creating an array object; the shape will be binding for future appending
-        return cls(blocks=list(), index=list(), shape=shape)
+        # for arrays with 0 columns, favor storing shape alone and not creating an array object; the shape will be binding for future appending
+        return cls.from_blocks((), shape_reference=shape)
 
     @staticmethod
     def vstack_blocks_to_blocks(
             type_blocks: tp.Sequence['TypeBlocks'],
             block_compatible: tp.Optional[bool] = None,
             reblock_compatible: tp.Optional[bool] = None,
             ) -> tp.Iterator[np.ndarray]:
@@ -599,34 +551,25 @@
                 yield concat_resolved(block_parts)
 
 
     #---------------------------------------------------------------------------
 
     def __init__(self, *,
             blocks: tp.List[np.ndarray],
-            index: tp.List[tp.Tuple[int, int]],
-            shape: tp.Tuple[int, int],
+            index: BlockIndex,
             ) -> None:
         '''
         Default constructor. We own all lists passed in to this constructor. This instance takes ownership of all lists passed to it.
 
         Args:
             blocks: A list of one or two-dimensional NumPy arrays. The list is owned by this instance.
-            index: list of pairs, where the first element is the block index, the second elemetns is the intra-block column
-            shape: two-element tuple defining row and column count. A (0, 0) shape is permitted for empty TypeBlocks.
+            index: BlockIndex
         '''
         self._blocks = blocks
-        self._index = index # list where index, as column, gets block, offset
-        self._shape = shape
-
-        if self._blocks:
-            self._row_dtype = resolve_dtype_iter(b.dtype for b in self._blocks)
-        else:
-            # NOTE: this violates the type; however, this is desirable when appending such that this value does not force an undesirable type resolution
-            self._row_dtype = None
+        self._index = index
 
     #---------------------------------------------------------------------------
     def __setstate__(self,
             state: tp.Tuple[object, tp.Mapping[str, tp.Any]],
             ) -> None:
         '''
         Ensure that reanimated NP arrays are set not writeable.
@@ -637,27 +580,24 @@
         for b in self._blocks:
             b.flags.writeable = False
 
     def __deepcopy__(self, memo: tp.Dict[int, tp.Any]) -> 'TypeBlocks':
         obj = self.__class__.__new__(self.__class__)
         obj._blocks = [array_deepcopy(b, memo) for b in self._blocks]
         obj._index = self._index.copy() # list of tuples of ints
-        obj._shape = self._shape # immutable, no copy necessary
-        obj._row_dtype = deepcopy(self._row_dtype, memo)
         memo[id(self)] = obj
         return obj
 
     def __copy__(self) -> 'TypeBlocks':
         '''
         Return shallow copy of this TypeBlocks. Underlying arrays are not copied.
         '''
         return self.__class__(
                 blocks=[b for b in self._blocks],
                 index=self._index.copy(), # list
-                shape=self._shape,
                 )
 
     def copy(self) -> 'TypeBlocks':
         '''
         Return shallow copy of this TypeBlocks. Underlying arrays are not copied.
         '''
         return self.__copy__()
@@ -675,15 +615,15 @@
 
     @property
     def dtypes(self) -> np.ndarray:
         '''
         Return an immutable array that, for each realizable column (not each block), the dtype is given.
         '''
         # this creates a new array every time it is called; could cache
-        a = np.empty(self._shape[1], dtype=DTYPE_OBJECT)
+        a = np.empty(self._index.columns, dtype=DTYPE_OBJECT)
         a[NULL_SLICE] = list(self._iter_dtypes())
         a.flags.writeable = False
         return a
 
     @property
     def shapes(self) -> np.ndarray:
         '''
@@ -714,14 +654,15 @@
     def unified_dtypes(self) -> bool:
         '''Return True if all blocks have the same dtype.
         '''
         # use blocks to iterate over fewer things
         if len(self._blocks) <= 1:
             return True
         dtypes = iter(d.dtype for d in self._blocks)
+        # NOTE: could compare to index.dtype
         d_first = next(dtypes)
         for d in dtypes:
             if d != d_first:
                 return False
         return True
 
     #---------------------------------------------------------------------------
@@ -732,16 +673,15 @@
         return InterfaceGetItem(self._extract_iloc)
 
     #---------------------------------------------------------------------------
     # common NP-style properties
 
     @property
     def shape(self) -> tp.Tuple[int, int]:
-        # make this a property so as to be immutable
-        return self._shape
+        return self._index.shape
 
     @property
     def ndim(self) -> int:
         return 2
 
     @property
     def size(self) -> int:
@@ -755,20 +695,19 @@
     # value extraction
 
     @property
     def values(self) -> np.ndarray:
         '''Returns a consolidated NP array of the all blocks.
         '''
         # provide a default dtype if one has not yet been set (an empty TypeBlocks, for example)
-        row_dtype = self._row_dtype if self._row_dtype is not None else DTYPE_FLOAT_DEFAULT
         # always return a 2D array
         return blocks_to_array_2d(
                 blocks=self._blocks,
-                shape=self._shape,
-                dtype=row_dtype,
+                shape=self._index.shape,
+                dtype=self._index.dtype,
                 )
 
     def axis_values(self,
             axis: int = 0,
             reverse: bool = False,
             ) -> tp.Iterator[np.ndarray]:
         '''Generator of arrays produced along an axis. Clients can expect to get an immutable array.
@@ -778,16 +717,16 @@
         '''
         # NOTE: might be renamed iter_arrays_by_axis
 
         if axis == 1: # iterate over rows
             zero_size = not bool(self._blocks)
             unified = self.unified
             # key: tp.Union[int, slice]
-            row_dtype= self._row_dtype if self._row_dtype is not None else DTYPE_FLOAT_DEFAULT
-            row_length = self._shape[0]
+            row_dtype = self._index.dtype
+            row_length = self._index.rows
 
             if not reverse:
                 row_idx_iter = range(row_length)
             else:
                 row_idx_iter = range(row_length - 1, -1, -1)
 
             if zero_size:
@@ -801,23 +740,23 @@
                     else: # 2d array
                         yield b[i]
             else:
                 # PERF: only creating and yielding one array at a time is shown to be slower; performance optimized: consolidate into a single array and then take slices
                 # NOTE: this might force unnecessary type coercion if going to a tuple, but if going to an array, the type consolidation is necessary
                 b = blocks_to_array_2d(
                         blocks=self._blocks,
-                        shape=self._shape,
+                        shape=self._index.shape,
                         dtype=row_dtype,
                         )
                 for i in row_idx_iter:
                     yield b[i]
 
         elif axis == 0: # iterate over columns
             if not reverse:
-                block_column_iter: tp.Iterable[tp.Tuple[int, int]] = self._index
+                block_column_iter = iter(self._index)
             else:
                 block_column_iter = reversed(self._index)
 
             for block_idx, column in block_column_iter:
                 b = self._blocks[block_idx]
                 if b.ndim == 1:
                     yield b
@@ -832,16 +771,15 @@
             ) -> tp.Iterator[tp.Tuple[tp.Tuple[int, int], tp.Any]]:
         '''
         Generator of pairs of iloc locations, values across entire TypeBlock. Used in creating a IndexHierarchy instance from a TypeBlocks.
 
         Args:
             axis: if 0, use row major iteration,  vary fastest along row.
         '''
-
-        shape = self._shape if axis == 0 else (self._shape[1], self._shape[0])
+        shape = self._index.shape if axis == 0 else (self._index.columns, self._index.rows)
 
         for iloc in np.ndindex(shape):
             if axis != 0: # invert
                 iloc = (iloc[1], iloc[0])
 
             block_idx, column = self._index[iloc[1]]
             b = self._blocks[block_idx]
@@ -1366,56 +1304,55 @@
             result.flags.writeable = False
             return result
 
         shape: ShapeType
 
         if axis == 0:
             # reduce all rows to 1d with column width
-            shape = self._shape[1]
+            shape = self._index.columns
             pos = 0 # used below undex axis 0
         elif composable: # axis 1
             # reduce all columns to 2d blocks with 1 column
-            shape = (self._shape[0], len(self._blocks))
+            shape = (self._index.rows, len(self._blocks))
         else: # axis 1, not block composable
             # Cannot do block-wise processing, must resolve to single array and return
-            row_dtype = self._row_dtype if self._row_dtype is not None else DTYPE_FLOAT_DEFAULT
-
             array = blocks_to_array_2d(
                     blocks=self._blocks,
-                    shape=self._shape,
-                    dtype=row_dtype,
+                    shape=self._index.shape,
+                    dtype=self._index.dtype,
                     )
             result = func(array=array, axis=axis)
             result.flags.writeable = False
             return result
 
         if dtypes:
             # If dtypes were specified, we know we have specific targets in mind for output
-            # Favor self._row_dtype's kind if it is in dtypes, else take first of passed dtypes
+            # Favor row_dtype's kind if it is in dtypes, else take first of passed dtypes
+            row_dtype = self._index.dtype
             for dt in dtypes:
-                if self._row_dtype.kind == dt.kind:
-                    dtype = self._row_dtype
+                if row_dtype == dt.kind:
+                    dtype = row_dtype
                     break
             else: # no break encountered
                 dtype = dtypes[0]
         else:
-            # _row_dtype gives us the compatible dtype for all blocks, whether we are reducing vertically (axis 0) or horizontall (axis 1)
+            # row_dtype gives us the compatible dtype for all blocks, whether we are reducing vertically (axis 0) or horizontall (axis 1)
             ufunc_selected = ufunc_skipna if skipna else ufunc
-            dtype = ufunc_dtype_to_dtype(ufunc_selected, self._row_dtype)
+            dtype = ufunc_dtype_to_dtype(ufunc_selected, self._index.dtype)
             if dtype is None:
                 # if we do not have a mapping for this function and row dtype, try to get a compatible type for the result of the function applied to each block
                 block_dtypes = []
                 for b in self._blocks:
                     dt = ufunc_dtype_to_dtype(ufunc_selected, b.dtype)
                     if dt is not None:
                         block_dtypes.append(dt)
                 if len(block_dtypes) == len(self._blocks): # if all resolved
                     dtype = resolve_dtype_iter(block_dtypes)
                 else: # assume row_dtype is appropriate
-                    dtype = self._row_dtype
+                    dtype = self._index.dtype
 
         out = np.empty(shape, dtype=dtype)
         for idx, b in enumerate(self._blocks):
             if axis == 0: # Combine rows, end with columns shape.
                 if size_one_unity and b.size == 1 and not skipna:
                     # No function call is necessary; if skipna could turn NaN to zero.
                     end = pos + 1
@@ -1461,21 +1398,20 @@
         Return a TypeBlocks rounded to the given decimals. Negative decimals round to the left of the decimal point.
         '''
         func = partial(np.round, decimals=decimals)
         # for now, we do not expose application of rounding on a subset of blocks, but is doable by setting the column_key
         return self.__class__(
                 blocks=list(self._ufunc_blocks(column_key=NULL_SLICE, func=func)),
                 index=self._index.copy(),
-                shape=self._shape
                 )
 
     def __len__(self) -> int:
         '''Length, as with NumPy and Pandas, is the number of rows. Note that A shape of (3, 0) will return a length of 3, even though there is no data.
         '''
-        return self._shape[0]
+        return self._index.rows
 
     @doc_inject()
     def display(self,
             config: tp.Optional[DisplayConfig] = None,
             *,
             style_config: tp.Optional[StyleConfig] = None,
             ) -> Display:
@@ -1515,104 +1451,35 @@
                     outermost=outermost)
         return d
 
 
     #---------------------------------------------------------------------------
     # extraction utilities
 
-    @staticmethod
-    def _cols_to_slice(indices: tp.Sequence[int]) -> slice:
-        '''Translate an iterable of contiguous integers into a slice. Integers are assumed to be intentionally ordered and contiguous.
-        '''
-        start_idx = indices[0]
-        # single column as a single slice
-        if len(indices) == 1:
-            return slice(start_idx, start_idx + 1)
-
-        stop_idx = indices[-1]
-        if stop_idx > start_idx: # ascending indices
-            return slice(start_idx, stop_idx + 1)
-
-        if stop_idx == 0:
-            return slice(start_idx, None, -1)
-        # stop is less than start, need to reduce by 1 to cover range
-        return slice(start_idx, stop_idx - 1, -1)
-
-
-    @classmethod
-    def _indices_to_contiguous_pairs(cls, indices: tp.Iterable[tp.Tuple[int, int]]
-        ) -> tp.Iterator[tp.Tuple[int, slice]]:
-        '''Indices are pairs of (block_idx, value); convert these to pairs of (block_idx, slice) when we identify contiguous indices within a block (these are block slices)
-
-        Args:
-            indices: can be a generator
-        '''
-        # store pairs of block idx, ascending col list
-        last: tp.Optional[tp.Tuple[int, int]] = None
-
-        for block_idx, col in indices:
-            if not last:
-                last = (block_idx, col)
-                bundle = [col]
-                continue
-            if last[0] == block_idx and abs(col - last[1]) == 1:
-                # if contiguous, update last, add to bundle
-                last = (block_idx, col)
-                # do not need to store all col, only the last, however probably easier to just accumulate all
-                bundle.append(col)
-                continue
-            # either new block, or not contiguous on same block
-            yield (last[0], cls._cols_to_slice(bundle))
-            # start a new bundle
-            bundle = [col]
-            last = (block_idx, col)
-
-        # last can be None
-        if last and bundle:
-            yield (last[0], cls._cols_to_slice(bundle))
-
-    # NOTE: this might cache its results as it might be frequently called with the same arguments in some scenarios (group)
     def _key_to_block_slices(self,
             key: GetItemKeyTypeCompound,
             retain_key_order: bool = True
             ) -> tp.Iterator[tp.Tuple[int, tp.Union[slice, int]]]:
         '''
         For a column key (an integer, slice, iterable, Boolean array), generate pairs of (block_idx, slice or integer) to cover all extractions. First, get the relevant index values (pairs of block id, column id), then convert those to contiguous slices. NOTE: integers are only returned when the input key is itself an integer.
 
         Args:
             retain_key_order: if False, returned slices will be in ascending order.
 
         Returns:
             A generator iterable of pairs, where values are pairs of either a block index and slice or, a block index and column index.
         '''
         if key is None or (key.__class__ is slice and key == NULL_SLICE):
+            # NOTE: this might be internalized in BlockIndex
             yield from ((i, NULL_SLICE) for i in range(len(self._blocks)))
-        else:
-            if isinstance(key, INT_TYPES):
-                # the index has the pair block, column integer
-                yield self._index[key]
-            else: # all cases where we try to get contiguous slices
-                if key.__class__ is slice:
-                    #  slice the index; null slice already handled
-                    if not retain_key_order:
-                        key = slice_to_ascending_slice(key, self._shape[1])
-                    indices: tp.Iterable[tp.Tuple[int, int]] = self._index[key] #type: ignore
-                elif key.__class__ is np.ndarray and key.dtype == bool: #type: ignore
-                    # NOTE: if self._index was an array we could use Boolean selection directly
-                    indices = (self._index[idx] for idx, v in enumerate(key) if v)
-                elif isinstance(key, KEY_ITERABLE_TYPES):
-                    # an iterable of keys, may not have contiguous regions; provide in the order given; set as a generator; self._index is a list, not an np.array, so cannot slice self._index; requires iteration in passed generator so probably this is as fast as it can be.
-                    # NOTE: we assume key is a list of integers: if key is a list of Booleans, we will not get the same elementwise selection as if we selected from an array
-                    if retain_key_order:
-                        indices = (self._index[x] for x in key)
-                    else:
-                        indices = (self._index[x] for x in sorted(key))
-                else:
-                    raise KeyError(key)
-                yield from self._indices_to_contiguous_pairs(indices)
+        elif isinstance(key, INT_TYPES):
+            # the index has the pair block, column integer
+            yield self._index[key]
+        else: # all cases where we try to get contiguous slices
+            yield from self._index.iter_contiguous(key, ascending=not retain_key_order)
 
     #---------------------------------------------------------------------------
     def _mask_blocks(self,
             row_key: tp.Optional[GetItemKeyTypeCompound] = None,
             column_key: tp.Optional[GetItemKeyTypeCompound] = None) -> tp.Iterator[np.ndarray]:
         '''Return Boolean blocks of the same size and shape, where key selection sets values to True.
         '''
@@ -2028,15 +1895,16 @@
             ) -> tp.Iterator[np.ndarray]:
         '''
         Shift type blocks independently on rows or columns. When ``wrap`` is True, the operation is a roll-style shift; when ``wrap`` is False, shifted-out values are not replaced and are filled with ``fill_value``.
 
         Args:
             column_shift: a positive value moves column data to the right.
         '''
-        row_count, column_count = self._shape
+        row_count = self._index.rows
+        column_count = self._index.columns
 
         # new start index is the opposite of the shift; if shifting by 2, the new start is the second from the end
         index_start_pos = -(column_shift % column_count)
         row_start_pos = -(row_shift % row_count)
 
         block_head_iter: tp.Iterable[np.ndarray]
         block_tail_iter: tp.Iterable[np.ndarray]
@@ -2101,15 +1969,16 @@
             column_shift: int,
             wrap: bool,
             get_col_fill_value: tp.Callable[[int, np.dtype], tp.Any],
             ) -> tp.Iterator[np.ndarray]:
         '''
         Shift type blocks independently on rows or columns. When ``wrap`` is True, the operation is a roll-style shift; when ``wrap`` is False, shifted-out values are not replaced and are filled with ``get_col_fill_value``.
         '''
-        row_count, column_count = self._shape
+        row_count = self._index.rows
+        column_count = self._index.columns
 
         # new start index is the opposite of the shift; if shifting by 2, the new start is the second from the end
         index_start_pos = -(column_shift % column_count)
         row_start_pos = -(row_shift % row_count)
 
         block_head_iter: tp.Iterable[np.ndarray]
         block_tail_iter: tp.Iterable[np.ndarray]
@@ -2750,38 +2619,38 @@
         Generator of sliced blocks, given row and column key selectors.
         The result is suitable for passing to TypeBlocks constructor.
         '''
         row_key_null = (row_key is None or
                 (row_key.__class__ is slice and row_key == NULL_SLICE))
 
         single_row = False
-        if row_key_null and self._shape[0] == 1:
+        if row_key_null and self._index.rows == 1:
             # this codition used to only hold if the arg is a null slice; now if None too and shape has one row
             single_row = True
         elif isinstance(row_key, INT_TYPES):
             single_row = True
         elif row_key.__class__ is slice:
             # NOTE: NULL_SLICE already handled above
             # need to determine if there is only one index returned by range (after getting indices from the slice); do this without creating a list/tuple, or walking through the entire range; get constant time look-up of range length after uses slice.indicies
-            if len(range(*row_key.indices(self._shape[0]))) == 1: #type: ignore
+            if len(range(*row_key.indices(self._index.rows))) == 1: #type: ignore
                 single_row = True
         elif row_key.__class__ is np.ndarray and row_key.dtype == DTYPE_BOOL: #type: ignore
             # must check this case before general iterables, below
             if row_key.sum() == 1: #type: ignore
                 single_row = True
         elif isinstance(row_key, KEY_ITERABLE_TYPES) and len(row_key) == 1:
             # an iterable of index integers is expected here
             single_row = True
 
         # if column_key_null
         if column_key is None or (
                 column_key.__class__ is slice and column_key == NULL_SLICE
                 ):
-            if self._shape[1] == 0:
-                yield EMPTY_ARRAY.reshape(self._shape)[row_key]
+            if self._index.columns == 0:
+                yield EMPTY_ARRAY.reshape(self._index.shape)[row_key]
             elif row_key_null: # when column_key is full
                 yield from self._blocks
             else:
                 for b in self._blocks:
                     # selection works for both 1D (to an element) and 2D (two a 1D array)
                     b_row = b[row_key] # PERF: most time from line profiler
                     if b_row.__class__ is np.ndarray:
@@ -2934,15 +2803,15 @@
         else:
             def chainer(i: int) -> tp.Any:
                 for a in arrays:
                     if a.ndim > 1:
                         yield from a[i]
                     else:
                         yield a[i]
-            for i in range(self._shape[0]):
+            for i in range(self._index.rows):
                 yield constructor(chainer(i))
 
     def iter_columns_tuples(self,
             key: tp.Optional[GetItemKeyTypeCompound],
             *,
             constructor: tp.Type[tp.Tuple[tp.Any, ...]] = tuple,
             ) -> tp.Iterator[tp.Tuple[tp.Any, ...]]:
@@ -3003,15 +2872,15 @@
             return TypeBlocks.from_blocks(b[row_key, column])
 
         # pass a generator to from_block; will return a TypeBlocks or a single element
         return self.from_blocks(
                 self._slice_blocks(
                         row_key=row_key,
                         column_key=column_key),
-                shape_reference=self._shape
+                shape_reference=self._index.shape
                 )
 
     def _extract_iloc(self,
             key: GetItemKeyTypeCompound
             ) -> 'TypeBlocks':
         if isinstance(key, tuple):
             return self._extract(*key)
@@ -3171,19 +3040,19 @@
         Args:
             key: if a single value, treated as a row key; if a tuple, treated as a pair of row, column keys.
         '''
         if isinstance(key, tuple):
             # column dropping can leed to a TB with generator that yields nothing;
             return TypeBlocks.from_blocks(
                     self._drop_blocks(*key),
-                    shape_reference=self._shape
+                    shape_reference=self._index.shape
                     )
         return TypeBlocks.from_blocks(
                 self._drop_blocks(row_key=key),
-                shape_reference=self._shape
+                shape_reference=self._index.shape
                 )
 
     def __iter__(self) -> tp.Iterator['TypeBlocks']:
         raise NotImplementedError('Amibigous whether or not to return np array or TypeBlocks')
 
     def __getitem__(self, key: GetItemKeyTypeCompound) -> 'TypeBlocks':
         '''
@@ -3240,15 +3109,15 @@
         if isinstance(other, TypeBlocks):
             apply_column_2d_filter = True
 
             if self.block_compatible(other, axis=None):
                 # this means that the blocks are the same shape; we do not check types
                 self_operands = self._blocks
                 other_operands = other._blocks
-            elif self._shape == other._shape:
+            elif self.shape == other.shape:
                 # if the result of reblock does not result in compatible shapes, we have to use .values as operands; the dtypes can be different so we only have to check that they columns sizes, the second element of the signature, all match.
                 if not self.reblock_compatible(other):
                     self_operands = (self.values,)
                     other_operands = (other.values,)
                 else:
                     self_operands = self._reblock()
                     other_operands = other._reblock()
@@ -3261,27 +3130,27 @@
 
             # handle dimensions
             if other.ndim == 0 or (other.ndim == 1 and len(other) == 1): #type: ignore
                 # a scalar: reference same value for each block position
                 apply_column_2d_filter = False
                 other_operands = (other for _ in range(len(self._blocks)))
             elif other.ndim == 1: #type: ignore
-                if axis == 0 and len(other) == self._shape[1]: #type: ignore
+                if axis == 0 and len(other) == self._index.columns: #type: ignore
                     # 1d array applied to the rows: chop to block width
                     apply_column_2d_filter = False
                     other_operands = (other[s] for s in self._block_shape_slices()) #type: ignore
-                elif axis == 1 and len(other) == self._shape[0]: #type: ignore
+                elif axis == 1 and len(other) == self._index.rows: #type: ignore
                     columnar = True
                 else:
-                    raise NotImplementedError(f'cannot apply binary operators with a 1D array along axis {axis}: {self._shape}, {other.shape}.') #type: ignore
-            elif other.ndim == 2 and other.shape == self._shape: #type: ignore
+                    raise NotImplementedError(f'cannot apply binary operators with a 1D array along axis {axis}: {self.shape}, {other.shape}.') #type: ignore
+            elif other.ndim == 2 and other.shape == self._index.shape: #type: ignore
                 apply_column_2d_filter = True
                 other_operands = (other[NULL_SLICE, s] for s in self._block_shape_slices()) #type: ignore
             else:
-                raise NotImplementedError(f'cannot apply binary operators to arrays without alignable shapes: {self._shape}, {other.shape}.') #type: ignore
+                raise NotImplementedError(f'cannot apply binary operators to arrays without alignable shapes: {self._index.shape}, {other.shape}.') #type: ignore
 
         if columnar:
             return self.from_blocks(apply_binary_operator_blocks_columnar(
                     values=self_operands,
                     other=other,
                     operator=operator,
                     ))
@@ -3296,15 +3165,15 @@
     #---------------------------------------------------------------------------
     # transformations resulting in the same dimensionality
 
     def isin(self, other: tp.Any) -> 'TypeBlocks':
         '''Return a new Boolean TypeBlocks that returns True if an element is in `other`.
         '''
         if hasattr(other, '__len__') and len(other) == 0:
-            array = np.full(self._shape, False, dtype=bool)
+            array = np.full(self._index.shape, False, dtype=bool)
             array.flags.writeable = False
             return self.from_blocks(array)
 
         other, other_is_unique = iterable_to_array_1d(other)
 
         def blocks() -> tp.Iterator[np.ndarray]:
             for b in self._blocks:
@@ -3317,23 +3186,23 @@
 
         return self.from_blocks(blocks())
 
 
     def transpose(self) -> 'TypeBlocks':
         '''Return a new TypeBlocks that transposes and concatenates all blocks.
         '''
-        dtype = self._row_dtype
+        dtype = self._index.dtype
         blocks = []
         for b in self._blocks:
             b = column_2d_filter(b).transpose()
             if b.dtype != dtype:
                 b = b.astype(dtype)
             blocks.append(b)
 
-        array = np.empty((self._shape[1], self._shape[0]), dtype=dtype)
+        array = np.empty((self._index.columns, self._index.rows), dtype=dtype)
         np.concatenate(blocks, axis=0, out=array)
         array.flags.writeable = False
         return self.from_blocks(array)
 
     #---------------------------------------------------------------------------
     #
     def boolean_apply_any(self, func: tp.Callable[[np.ndarray], np.ndarray]) -> bool:
@@ -4178,15 +4047,15 @@
 
     def iter_block_signatures(self) -> tp.Iterator[ArraySignature]:
         '''
         Yields:
             a hashable key that will match array that share the same data, or share slices from the same underlying data and have the same shape and strides.
         '''
         yield from (array_signature(self._extract_array_column(i))
-                for i in range(self._shape[1]))
+                for i in range(self._index.columns))
 
     @doc_inject()
     def equals(self,
             other: tp.Any,
             *,
             compare_dtype: bool = False,
             compare_class: bool = False,
@@ -4206,83 +4075,47 @@
         # NOTE: there is only one TypeBlocks class, but better to be consistent
         if compare_class and self.__class__ != other.__class__:
             return False
         elif not isinstance(other, TypeBlocks):
             return False
 
         # same type from here
-        if self._shape != other._shape:
+        if self._index.shape != other.shape:
             return False
 
         if compare_dtype:
             for d_self, d_other in zip(self._iter_dtypes(), other._iter_dtypes()):
                 # have already validated shape
                 if d_self != d_other:
                     return False
 
         # NOTE: cannot directly compare blocks as we cannot assume the same number of blocks means that the blocks are consolidated in the same way
 
-        for i in range(self._shape[1]):
+        for i in range(self._index.columns):
             if not arrays_equal(
                     self._extract_array_column(i),
                     other._extract_array_column(i),
                     skipna=skipna,
                     ):
                 return False
         return True
 
     #---------------------------------------------------------------------------
     # mutate
 
     def append(self, block: np.ndarray) -> None:
         '''Add a block; an array copy will not be made unless the passed in block is not immutable'''
         # NOTE: shape can be 0, 0 if empty, or any one dimension can be 0. if columns is 0 and rows is non-zero, that row count is binding for appending (though the array need no tbe appended); if columns is > 0 and rows is zero, that row is binding for appending (and the array should be appended).
+        if self._index.register(block):
+            self._blocks.append(immutable_filter(block))
 
-        row_count = self._shape[0]
-
-        # update shape
-        if block.shape[0] != row_count:
-            raise RuntimeError(f'appended block shape {block.shape} does not align with shape {self._shape}')
-
-        # get ref to append
-        block_idx = len(self._blocks) # next block
-        if block.ndim == 1:
-            # length already confirmed to match row count; even if this is a zero length 1D array, we keep it as it (by definition) defines a column (if the existing row_count is zero). said another way, a zero length, 1D array always has a shape of (0, 1)
-            block_columns = 1
-        else:
-            block_columns = block.shape[1]
-            if block_columns == 0:
-                # do not append 0 width arrays
-                return
-
-        # extend shape, or define it if not yet set
-        self._shape = (row_count, self._shape[1] + block_columns)
-
-        # add block, dtypes, index
-        for i in range(block_columns):
-            self._index.append((block_idx, i))
-
-        # make immutable copy if necessary before appending
-        self._blocks.append(immutable_filter(block))
-
-        # if already aligned, nothing to do
-        if not self._row_dtype: # if never set as shape is empty
-            self._row_dtype = block.dtype
-        elif block.dtype != self._row_dtype:
-            # we do not use resolve_dtype here as we want to preserve types, not safely cooerce them (i.e., int to float)
-            self._row_dtype = DTYPE_OBJECT
 
     def extend(self,
             other: tp.Union['TypeBlocks', tp.Iterable[np.ndarray]]
             ) -> None:
         '''Extend this TypeBlock with the contents of another TypeBlocks instance, or an iterable of arrays. Note that an iterable of TypeBlocks is not currently supported.
         '''
-        if isinstance(other, TypeBlocks):
-            if self._shape[0]:
-                if self._shape[0] != other._shape[0]:
-                    raise RuntimeError('cannot extend unaligned shapes')
-            blocks: tp.Iterable[np.ndarray] = other._blocks
-        else: # accept iterables of np.arrays
-            blocks = other
-        # row count must be the same
+        # accept iterables of np.arrays
+        blocks = other._blocks if isinstance(other, TypeBlocks) else other
         for block in blocks:
-            self.append(block)
+            if self._index.register(block):
+                self._blocks.append(immutable_filter(block))
```

### Comparing `static-frame-1.4.2/static_frame/core/util.py` & `static-frame-1.4.3/static_frame/core/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1748,52 +1748,52 @@
         array, _ = iterable_to_array_1d(chain((first,), values))
         return array
     # its an element
     return np.array(values)
 
 #-------------------------------------------------------------------------------
 
-def slice_to_ascending_slice(
-        key: slice,
-        size: int
-        ) -> slice:
-    '''
-    Given a slice, return a slice that, with ascending integers, covers the same values.
-
-    Args:
-        size: the length of the container on this axis
-    '''
-    key_step = key.step
-    key_start = key.start
-    key_stop = key.stop
-
-    if key_step is None or key_step > 0:
-        return key
-
-    # will get rid of all negative values greater than the size; but will replace None with an appropriate number for usage in range
-    norm_key_start, norm_key_stop, norm_key_step = key.indices(size)
-
-    # everything else should be descending, but we might have non-descending start, stop
-    if key_start is not None and key_stop is not None:
-        if norm_key_start <= norm_key_stop: # an ascending range
-            return EMPTY_SLICE
-
-    norm_range = range(norm_key_start, norm_key_stop, norm_key_step)
-
-    # derive stop
-    if key_start is None:
-        stop = None
-    else:
-        stop = norm_range[0] + 1
-
-    if key_step == -1:
-        # gets last realized value, not last range value
-        return slice(None if key_stop is None else norm_range[-1], stop, 1)
+# def slice_to_ascending_slice(
+#         key: slice,
+#         size: int
+#         ) -> slice:
+#     '''
+#     Given a slice, return a slice that, with ascending integers, covers the same values.
+
+#     Args:
+#         size: the length of the container on this axis
+#     '''
+#     key_step = key.step
+#     key_start = key.start
+#     key_stop = key.stop
+
+#     if key_step is None or key_step > 0:
+#         return key
+
+#     # will get rid of all negative values greater than the size; but will replace None with an appropriate number for usage in range
+#     norm_key_start, norm_key_stop, norm_key_step = key.indices(size)
+
+#     # everything else should be descending, but we might have non-descending start, stop
+#     if key_start is not None and key_stop is not None:
+#         if norm_key_start <= norm_key_stop: # an ascending range
+#             return EMPTY_SLICE
+
+#     norm_range = range(norm_key_start, norm_key_stop, norm_key_step)
+
+#     # derive stop
+#     if key_start is None:
+#         stop = None
+#     else:
+#         stop = norm_range[0] + 1
+
+#     if key_step == -1:
+#         # gets last realized value, not last range value
+#         return slice(None if key_stop is None else norm_range[-1], stop, 1)
 
-    return slice(norm_range[-1], stop, key_step * -1)
+#     return slice(norm_range[-1], stop, key_step * -1)
 
 def pos_loc_slice_to_iloc_slice(
         key: slice,
         length: int,
         ) -> slice:
     '''Make a positional (integer) exclusive stop key inclusive by adding one to the stop value.
     '''
```

### Comparing `static-frame-1.4.2/static_frame/core/www.py` & `static-frame-1.4.3/static_frame/core/www.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/core/yarn.py` & `static-frame-1.4.3/static_frame/core/yarn.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/test_case.py` & `static-frame-1.4.3/static_frame/test/test_case.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_archive_npy.py` & `static-frame-1.4.3/static_frame/test/unit/test_archive_npy.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_axis_map.py` & `static-frame-1.4.3/static_frame/test/unit/test_axis_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_batch.py` & `static-frame-1.4.3/static_frame/test/unit/test_batch.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_bus.py` & `static-frame-1.4.3/static_frame/test/unit/test_bus.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_container.py` & `static-frame-1.4.3/static_frame/test/unit/test_container.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_container_util.py` & `static-frame-1.4.3/static_frame/test/unit/test_container_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,15 +265,15 @@
 
     #---------------------------------------------------------------------------
 
     def test_key_to_ascending_key_a(self) -> None:
         self.assertEqual(key_to_ascending_key([9, 5, 1], 3), [1, 5, 9])
         self.assertEqual(key_to_ascending_key(np.array([9, 5, 1]), 3).tolist(), [1, 5, 9]) # type: ignore
 
-        self.assertEqual(key_to_ascending_key(slice(3, 0, -1), 3), slice(1, 3, 1))
+        self.assertEqual(key_to_ascending_key(slice(3, 0, -1), 3), slice(1, 3, None))
 
         self.assertEqual(key_to_ascending_key(100, 3), 100)
 
         self.assertEqual(key_to_ascending_key([], 3), [])
 
         self.assertEqual(key_to_ascending_key( # type: ignore
                 Series(('a', 'b', 'c'), index=(9, 5, 1)), 3).values.tolist(),
```

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_display.py` & `static-frame-1.4.3/static_frame/test/unit/test_display.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_display_color.py` & `static-frame-1.4.3/static_frame/test/unit/test_display_color.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_doc.py` & `static-frame-1.4.3/static_frame/test/unit/test_doc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_fill_value_auto.py` & `static-frame-1.4.3/static_frame/test/unit/test_fill_value_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_frame.py` & `static-frame-1.4.3/static_frame/test/unit/test_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 from static_frame import IndexYearGO
 from static_frame import IndexYearMonth
 from static_frame import Series
 from static_frame import TypeBlocks
 from static_frame import isna_element
 from static_frame import mloc
 from static_frame.core.exception import AxisInvalid
+from static_frame.core.exception import ErrorInitColumns
 from static_frame.core.exception import ErrorInitFrame
 from static_frame.core.exception import ErrorInitIndex
 from static_frame.core.exception import ErrorNPYEncode
 from static_frame.core.exception import InvalidDatetime64Initializer
 from static_frame.core.exception import InvalidFillValue
 from static_frame.core.fill_value_auto import FillValueAuto
 from static_frame.core.frame import FrameAssignBLoc
@@ -9177,14 +9178,28 @@
         s1 = Series([1, 2, 3]) # happens implicitly, but here we make it explicit
         s2 = s1.rename(np.datetime64('2022-01-01'))
 
         with self.assertRaises(InvalidDatetime64Initializer):
             _ = Frame.from_concat((s1, s2), axis=1, columns_constructor=sf.IndexDate)
 
 
+    def test_frame_from_concat_hh(self) -> None:
+        a = sf.Series([1, 2, 3], name='2000-01-01')
+        b = sf.Series([4, 5, 6], name=np.datetime64('2000-01-02'))
+        # for axis 1, name will become column label, index will remains
+        # this fails as we end up using default index constructor on dt64 name, which raises
+        f1 = Frame.from_concat((a, b), axis=1, columns_constructor=IndexDate)
+        self.assertEqual(f1.to_pairs(),
+            ((np.datetime64('2000-01-01'), ((0, 1), (1, 2), (2, 3))),
+            (np.datetime64('2000-01-02'), ((0, 4), (1, 5), (2, 6))))
+            )
+
+        with self.assertRaises(ErrorInitColumns):
+            _ = Frame.from_concat((a, b), axis=1, index_constructor=IndexDate)
+
 
     #---------------------------------------------------------------------------
 
     def test_frame_from_concat_error_init_a(self) -> None:
         f1 = Frame.from_element(10,
                 columns=('p', 'q',),
                 index=('x', 'z'))
```

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_frame_he.py` & `static-frame-1.4.3/static_frame/test/unit/test_frame_he.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_frame_iter.py` & `static-frame-1.4.3/static_frame/test/unit/test_frame_iter.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_frame_join.py` & `static-frame-1.4.3/static_frame/test/unit/test_frame_join.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_frame_via_fill_value.py` & `static-frame-1.4.3/static_frame/test/unit/test_frame_via_fill_value.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_frame_via_re.py` & `static-frame-1.4.3/static_frame/test/unit/test_frame_via_re.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_hloc.py` & `static-frame-1.4.3/static_frame/test/unit/test_hloc.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_index.py` & `static-frame-1.4.3/static_frame/test/unit/test_index.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_index_auto.py` & `static-frame-1.4.3/static_frame/test/unit/test_index_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_index_base.py` & `static-frame-1.4.3/static_frame/test/unit/test_index_base.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_index_correspondence.py` & `static-frame-1.4.3/static_frame/test/unit/test_index_correspondence.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_index_datetime.py` & `static-frame-1.4.3/static_frame/test/unit/test_index_datetime.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_index_hierarchy.py` & `static-frame-1.4.3/static_frame/test/unit/test_index_hierarchy.py`

 * *Files 0% similar despite different names*

```diff
@@ -921,15 +921,14 @@
         ih2.append(('c', 'c')) #type: ignore
         self.assertEqual(ih1.values.tolist(),
                 [['a', 'a'], ['b', 'b']])
 
         self.assertEqual(ih2.values.tolist(), #type: ignore
                 [['a', 'a'], ['b', 'b'], ['c', 'c']])
 
-
     #---------------------------------------------------------------------------
 
     def test_hierarchy_extract_getitem_astype_a(self) -> None:
 
         labels = (
                 ('I', 'A', 1),
                 ('I', 'B', 1),
@@ -1614,17 +1613,14 @@
         self.assertIn((True, False), ih)
         with self.assertRaises(IndexError):
             np.array((True, False)) in ih
 
         with self.assertRaises(RuntimeError):
             (True, False, True, False) in ih #pylint: disable=W0104
 
-        # TODO: This behavior is incorrect!
-        # self.assertNotIn(np.array((True, False, True, False)), ih)
-
     def test_hierarchy_contains_d(self) -> None:
         labels = ((True, 'A'), ('I', 'B'))
         ih = IndexHierarchy.from_labels(labels)
 
         key = HLoc[:, 'A']
 
         ih2 = ih.loc[key]
@@ -4536,15 +4532,14 @@
 
         original = copy.deepcopy(ihgo)
         ihgo.append((5, 302))
         post19 = str(ihgo)
         self.assertNotEqual(post19, str(original))
         self.assertEqual(post19, str(ihgo))
 
-
     #---------------------------------------------------------------------------
 
     def test_hierarchy_iloc_a(self) -> None:
 
         f = ff.parse('f(Fg)|v(int,bool,str)|i((IY,ID),(dtY,dtD))|c(ISg,dts)|s(6,2)')
 
         post = f.loc[HLoc[f.index.iloc[0]]]
```

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_index_hierarchy_set_utils.py` & `static-frame-1.4.3/static_frame/test/unit/test_index_hierarchy_set_utils.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_interface.py` & `static-frame-1.4.3/static_frame/test/unit/test_interface.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_loc_map.py` & `static-frame-1.4.3/static_frame/test/unit/test_loc_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_memory_measure.py` & `static-frame-1.4.3/static_frame/test/unit/test_memory_measure.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_memory_measure_getsizeof.py` & `static-frame-1.4.3/static_frame/test/unit/test_memory_measure_getsizeof.py`

 * *Files 4% similar despite different names*

```diff
@@ -452,57 +452,37 @@
         self.assertTrue(memory_total(tb), sum(getsizeof(e) for e in (
             np.array([1, 2, 3]),
             tb._blocks, # [np.array([1, 2, 3])],
             0,
             (0, 0),
             tb._index, # [(0, 0)],
             3, 1,
-            tb._shape, # (3, 1),
-            np.dtype('int64'),
             # _row_dtype, # np.dtype('int64') is already included
             tb
         )))
 
     def test_getsizeof_total_type_blocks_list_of_1d_arrays(self) -> None:
         tb = TypeBlocks.from_blocks([
             np.array([1, 2, 3]),
             np.array([4, 5, 6])
         ])
         self.assertEqual(memory_total(tb), sum(getsizeof(e) for e in (
             np.array([1, 2, 3]),
             np.array([4, 5, 6]),
             tb._blocks, # [np.array([1, 2, 3]), np.array([4, 5, 6])],
-            0,
-            (0, 0),
-            1,
-            (1, 0),
             tb._index, # [(0, 0), (1, 0)],
-            3, 2,
-            tb._shape, # (3, 2),
-            np.dtype('int64'),
-            # _row_dtype, # np.dtype('int64') is already included
             tb
         )))
 
     def test_getsizeof_total_type_blocks_2d_array(self) -> None:
         tb = TypeBlocks.from_blocks(np.array([[1, 2, 3], [4, 5, 6]]))
         self.assertEqual(memory_total(tb), sum(getsizeof(e) for e in (
             np.array([[1, 2, 3],[4, 5, 6]]),
             tb._blocks, # [np.array([[1, 2, 3],[4, 5, 6]])],
-            0,
-            (0, 0),
-            1,
-            (0, 1),
-            2,
-            (0, 2),
             tb._index, # [(0, 0), (0, 1), (0, 2)],
-            3,
-            tb._shape, # (2, 3),
-            np.dtype('int64'),
-            # _row_dtype, # np.dtype('int64') is already included
             tb
         )))
 
     #---------------------------------------------------------------------------
     # IndexHierarchy
 
     def test_getsizeof_total_index_hierarchy_simple(self) -> None:
```

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_pivot.py` & `static-frame-1.4.3/static_frame/test/unit/test_pivot.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_protocol_dfi.py` & `static-frame-1.4.3/static_frame/test/unit/test_protocol_dfi.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_quilt.py` & `static-frame-1.4.3/static_frame/test/unit/test_quilt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1695,12 +1695,41 @@
         f1 = ff.parse('s(20,4)|v(int)|i(I,str)|c(I,str)')
         q1 = Quilt.from_frame(f1, chunksize=5, axis=0, retain_labels=True)
         b1 = q1.bus
 
         self.assertEqual(b1.index.values.tolist(),
             ['zZbu', 'z2Oo', 'zOyq', 'zjZQ'])
 
+    #------------------------------------------------------------------
+
+    def test_quilt_from_index_hierarchy_bus_consistent_index_a(self) -> None:
+        frame = ff.parse('f(Fg)|v(int,bool,str)|i((I,I),(str,int))|s(12,2)')
+        frame = frame.iloc[np.array([11, 0, 4, 9, 1, 10, 5, 2, 6, 3, 7, 8])]
+
+        f1 = frame.iloc[:6].rename("f1")
+        f2 = frame.iloc[6:].rename("f2")
+
+        bus = Bus.from_frames((f1, f2))
+        quilt = Quilt(bus, retain_labels=False, axis=0)
+
+        selected_index = quilt.loc[HLoc["ztsv"]].index
+
+        assert set(selected_index.values_at_depth(0)) == {"ztsv"}
+
+    def test_quilt_from_index_hierarchy_bus_consistent_index_b(self) -> None:
+        frame = ff.parse('f(Fg)|v(int,bool,str)|i((I,I),(str,int))|s(12,2)')
+        frame = frame.iloc[np.array([11, 0, 4, 9, 1, 10, 5, 2, 6, 3, 7, 8])]
+
+        f1 = frame.iloc[:6].rename("f1").T
+        f2 = frame.iloc[6:].rename("f2").T
+
+        bus = Bus.from_frames((f1, f2))
+        quilt = Quilt(bus, retain_labels=False, axis=1)
+
+        selected_index = quilt[HLoc["ztsv"]].columns
+
+        assert set(selected_index.values_at_depth(0)) == {"ztsv"}
 
 
 if __name__ == '__main__':
     import unittest
     unittest.main()
```

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_rank.py` & `static-frame-1.4.3/static_frame/test/unit/test_rank.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_series.py` & `static-frame-1.4.3/static_frame/test/unit/test_series.py`

 * *Files 1% similar despite different names*

```diff
@@ -4346,14 +4346,21 @@
         s1 = Series(('2014', '', '2013'), index=('x', 'y', 'z'), dtype=dt64)
         s2 = s1.via_dt(fill_value=-1).year
         self.assertEqual(s2.to_pairs(), (('x', 2014), ('y', -1), ('z', 2013)))
         self.assertEqual(s1.astype(object).via_dt(fill_value=-1).year.to_pairs(),
                 (('x', 2014), ('y', -1), ('z', 2013))
                 )
 
+    def test_series_via_dt_year_c(self) -> None:
+        dt64 = np.datetime64
+
+        s1 = Series(('2014', '', '2013'), index=('x', 'y', 'z'), dtype=dt64)
+        with self.assertRaises(RuntimeError):
+            _ = s1.via_dt.year
+
     #---------------------------------------------------------------------------
 
     def test_series_via_dt_month_a(self) -> None:
         dt64 = np.datetime64
 
         s1 = Series(('2014-04', '', '2013-08'), index=('x', 'y', 'z'), dtype=dt64)
         s2 = s1.via_dt(fill_value=-1).month
@@ -4398,14 +4405,20 @@
         s1 = Series(('2010-01-01', '2010-01-02', '', '2013-04-01', '2013-04-02'),
                 index=('a', 'b', 'c', 'd', 'e'),
                 dtype=np.datetime64).astype(object)
         post = s1.via_dt(fill_value='x').year_month
         self.assertEqual(post.to_pairs(),
                 (('a', '2010-01'), ('b', '2010-01'), ('c', 'x'), ('d', '2013-04'), ('e', '2013-04')))
 
+    def test_series_via_dt_year_month_c3(self) -> None:
+        s1 = Series(('2010-01-01', '2010-01-02', '', '2013-04-01', '2013-04-02'),
+                index=('a', 'b', 'c', 'd', 'e'),
+                dtype=np.datetime64).astype(object)
+        with self.assertRaises(RuntimeError):
+            _ = s1.via_dt.year_month
 
     #---------------------------------------------------------------------------
 
     def test_series_via_dt_day_a(self) -> None:
         dt64 = np.datetime64
 
         s1 = Series(('2014', '2013'), index=('x', 'y'))
@@ -4439,14 +4452,25 @@
         dt64 = np.datetime64
         s1 = Series((dt64('2014-02-12'), '', dt64('2013-11-28')), index=('x', 'y', 'z'), dtype=dt64)
         s2 = s1.via_dt(fill_value=-1).day
         self.assertEqual(s2.to_pairs(), (('x', 12), ('y', -1), ('z', 28)))
         self.assertEqual(s1.astype(object).via_dt(fill_value=0).day.to_pairs(), (('x', 12), ('y', 0), ('z', 28)))
 
 
+    def test_series_via_dt_day_c(self) -> None:
+        def todt(date_str: str) -> datetime.date:
+            return datetime.date(*(int(x) for x in date_str.split('-')))
+
+        s1 = Series((todt('2014-02-12'), None, todt('2013-11-28')), index=('x', 'y', 'z'))
+        with self.assertRaises(RuntimeError):
+            _ = s1.via_dt.day
+        self.assertEqual(s1.via_dt(fill_value=-1).day.to_pairs(),
+                (('x', 12), ('y', -1), ('z', 28))
+                )
+
     #---------------------------------------------------------------------------
 
 
     def test_series_via_dt_isoformat_a(self) -> None:
 
         s1 = Series(('2014-01-02T05:02', '2013-02-05T16:55'),
                 index=('x', 'y'),
@@ -5555,14 +5579,33 @@
 
         s1 = Series(range(3), index=tuple('abc'))
         s2 = Series(range(5), index=tuple('abcde'))
 
         with self.assertRaises(NotImplementedError):
             s2.via_fill_value(0).via_T * s2
 
+
+    def test_series_via_fill_value_k(self) -> None:
+        s1 = sf.Series(range(4))
+        s2 = s1.via_fill_value(-1).loc[s1.index]
+        self.assertEqual(s2.to_pairs(), ((0, 0), (1, 1), (2, 2), (3, 3)))
+
+        s3 = s1.via_fill_value(-1).loc[s1]
+        self.assertEqual(s3.to_pairs(), ((0, 0), (1, 1), (2, 2), (3, 3)))
+
+
+    def test_series_via_fill_value_l(self) -> None:
+        s1 = sf.Series(range(4), index=tuple('abcd'))
+        s2 = s1.via_fill_value(-1).loc[s1.index]
+        self.assertEqual(s2.to_pairs(), (('a', 0), ('b', 1), ('c', 2), ('d', 3)))
+
+        s3 = s1.via_fill_value(-1).loc[s1]
+        self.assertEqual(s3.to_pairs(), ((0, -1), (1, -1), (2, -1), (3, -1)))
+
+
     #---------------------------------------------------------------------------
 
     def test_series_via_re_search_a(self) -> None:
 
         s1 = sf.Series(('aaa', 'aab', 'cab'))
 
         s2 = s1.via_re('ab').search()
```

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_series_he.py` & `static-frame-1.4.3/static_frame/test/unit/test_series_he.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_store.py` & `static-frame-1.4.3/static_frame/test/unit/test_store.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_store_filter.py` & `static-frame-1.4.3/static_frame/test/unit/test_store_filter.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_store_hdf5.py` & `static-frame-1.4.3/static_frame/test/unit/test_store_hdf5.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_store_sqlite.py` & `static-frame-1.4.3/static_frame/test/unit/test_store_sqlite.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_store_xlsx.py` & `static-frame-1.4.3/static_frame/test/unit/test_store_xlsx.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_store_zip.py` & `static-frame-1.4.3/static_frame/test/unit/test_store_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_style_config.py` & `static-frame-1.4.3/static_frame/test/unit/test_style_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_type_blocks.py` & `static-frame-1.4.3/static_frame/test/unit/test_type_blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import copy
 import pickle
 from itertools import zip_longest
 
 import frame_fixtures as ff
 import numpy as np
+from arraykit import ErrorInitTypeBlocks
 from arraykit import immutable_filter
 
 from static_frame import TypeBlocks
 from static_frame import mloc
 from static_frame.core.container_util import get_col_dtype_factory
 from static_frame.core.container_util import get_col_fill_value_factory
 from static_frame.core.display_config import DisplayConfig
 from static_frame.core.exception import AxisInvalid
-from static_frame.core.exception import ErrorInitTypeBlocks
 from static_frame.core.fill_value_auto import FillValueAuto
 from static_frame.core.frame import Frame
 from static_frame.core.index_correspondence import IndexCorrespondence
 from static_frame.core.type_blocks import group_match
 from static_frame.core.type_blocks import group_sorted
 from static_frame.core.util import NULL_SLICE
 from static_frame.core.util import isna_array
@@ -56,33 +56,14 @@
         a3 = np.array([['a', 'b'], ['c', 'd'], ['oe', 'od']])
         tb3 = TypeBlocks.from_blocks((a1, a2, a3))
 
         # showing that slices keep the same memory location
         # self.assertTrue((tb1[0:2].mloc == tb1.mloc[:2]).all())
         # self.assertTrue((tb1.mloc[:2] == tb1.iloc[0:2, 0:2].mloc).all())
 
-    def test_type_blocks_contiguous_pairs(self) -> None:
-
-        a = [(0, 1), (0, 2), (2, 3), (2, 1)]
-        post = list(TypeBlocks._indices_to_contiguous_pairs(a))
-        self.assertEqual(post, [
-                (0, slice(1, 3)),
-                (2, slice(3, 4)),
-                (2, slice(1, 2)),
-                ])
-
-        a = [(0, 0), (0, 1), (0, 2), (1, 4), (2, 1), (2, 3)]
-        post = list(TypeBlocks._indices_to_contiguous_pairs(a))
-        self.assertEqual(post, [
-                (0, slice(0, 3)),
-                (1, slice(4, 5)),
-                (2, slice(1, 2)),
-                (2, slice(3, 4)),
-            ])
-
     def test_type_blocks_b(self) -> None:
 
         # given naturally of a list of rows; this corresponds to what we get with iloc, where we select a row first, then a column
         a1 = np.array([[1, 2, 3], [4, 5, 6]])
         # shape is given as rows, columns
         self.assertEqual(a1.shape, (2, 3))
 
@@ -96,15 +77,15 @@
         self.assertTypeBlocksArrayEqual(tb1[4], [[0.5], [0.6]])
 
         self.assertEqual(list(tb1[7].values), ['b', 'd'])
 
         self.assertEqual(tb1.shape, (2, 8))
 
         self.assertEqual(len(tb1), 2)
-        self.assertEqual(tb1._row_dtype, np.object_)
+        self.assertEqual(tb1._index.dtype, np.object_)
 
         slice1 = tb1[2:5]
         self.assertEqual(slice1.shape, (2, 3))
 
         slice2 = tb1[0:5]
         self.assertEqual(slice2.shape, (2, 5))
 
@@ -172,28 +153,14 @@
         self.assertEqual(list(tb1._key_to_block_slices(6)), [(2, 0)])
         self.assertEqual(list(tb1._key_to_block_slices([3,5,6])),
             [(1, slice(0, 1, None)), (1, slice(2, 3, None)), (2, slice(0, 1, None))]
             )
 
     #---------------------------------------------------------------------------
 
-    def test_type_blocks_key_to_block_slices_a(self) -> None:
-        a1 = np.array([1, 2, -1])
-        a2 = np.array([[False, True], [True, True], [False, True]])
-        tb1 = TypeBlocks.from_blocks((a1, a2))
-
-        self.assertEqual(list(tb1._key_to_block_slices(None)),
-                [(0, NULL_SLICE), (1, NULL_SLICE)]
-                )
-
-        with self.assertRaises(KeyError):
-            list(tb1._key_to_block_slices('a'))
-
-    #---------------------------------------------------------------------------
-
     def test_type_blocks_extract_a(self) -> None:
 
         a1 = np.array([1, 2, 3])
         a2 = np.array([False, True, False])
         a3 = np.array(['b', 'c', 'd'])
         a4 = np.array(['gd', 'cd', 'dd'])
         tb1 = TypeBlocks.from_blocks((a1, a2, a3, a4))
@@ -679,15 +646,15 @@
         a2 = np.array([[False, False, True], [True, False, True], [True, False, True]])
         a3 = np.array([['a', 'b'], ['c', 'd'], ['oe', 'od']])
         a4 = np.array([None, None, None])
         tb = TypeBlocks.from_blocks((a1, a2, a4, a3))
 
         post1 = [x for x in tb.element_items()]
 
-        tb2 = TypeBlocks.from_element_items(post1, tb.shape, tb._row_dtype)
+        tb2 = TypeBlocks.from_element_items(post1, tb.shape, tb._index.dtype)
         self.assertTrue((tb.values == tb2.values).all())
 
         post2 = tb == tb2
         self.assertEqual(post2.values.tolist(),
                 [[True, True, True, True, True, True, True, True, True], [True, True, True, True, True, True, True, True, True], [True, True, True, True, True, True, True, True, True]])
 
     def test_type_blocks_binary_operator_f(self) -> None:
@@ -1806,15 +1773,15 @@
 
         post = [x for x in tb.element_items()]
 
         self.assertEqual(post,
                 [((0, 0), 1), ((0, 1), 2), ((0, 2), 3), ((0, 3), False), ((0, 4), False), ((0, 5), True), ((0, 6), None), ((0, 7), 'a'), ((0, 8), 'b'), ((1, 0), 4), ((1, 1), 5), ((1, 2), 6), ((1, 3), True), ((1, 4), False), ((1, 5), True), ((1, 6), None), ((1, 7), 'c'), ((1, 8), 'd'), ((2, 0), 0), ((2, 1), 0), ((2, 2), 1), ((2, 3), True), ((2, 4), False), ((2, 5), True), ((2, 6), None), ((2, 7), 'oe'), ((2, 8), 'od')]
                 )
 
-        tb2 = TypeBlocks.from_element_items(post, tb.shape, tb._row_dtype)
+        tb2 = TypeBlocks.from_element_items(post, tb.shape, tb._index.dtype)
         self.assertTrue((tb.values == tb2.values).all())
 
     def test_type_blocks_elements_items_b(self) -> None:
         a1 = np.array([[1, 2, 3], [4, 5, 6], [0, 0, 1]])
         a2 = np.array([None, None, None])
         tb = TypeBlocks.from_blocks((a1, a2))
 
@@ -3431,15 +3398,14 @@
         a2 = np.full((3, 4), 'x')
         tb = TypeBlocks.from_blocks((a1, a2))
         self.assertEqual(tb.shape, (3, 4))
         self.assertEqual(tb.values.tolist(),
             [['x', 'x', 'x', 'x'],
             ['x', 'x', 'x', 'x'],
             ['x', 'x', 'x', 'x']])
-
         a3 = next(tb.axis_values(0))
         self.assertEqual(a3.tolist(),
             ['x', 'x', 'x']
             )
 
     def test_type_blocks_from_blocks_b(self) -> None:
 
@@ -4151,15 +4117,15 @@
         a1 = np.array([False, True, False])
         tb1 = TypeBlocks.from_blocks((a1, ))
         self.assertTrue(tb1.unified_dtypes)
 
     #---------------------------------------------------------------------------
     def test_type_blocks_key_to_block_slices_exception(self) -> None:
         # as this is an loc-is-iloc index, the key gets passed directly to type blocks
-        with self.assertRaises(KeyError):
+        with self.assertRaises(TypeError):
             ff.parse('v(bool,str,bool,float)|s(4,8)')["foo"]
 
 
     def test_type_blocks_consolidate_select_a1(self) -> None:
 
         a1 = np.array([1, 2, 3])
         a2 = np.array([4, 5, 6])
```

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_util.py` & `static-frame-1.4.3/static_frame/test/unit/test_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,14 @@
 from static_frame.core.util import key_to_datetime_key
 from static_frame.core.util import prepare_iter_for_array
 from static_frame.core.util import roll_1d
 from static_frame.core.util import roll_2d
 from static_frame.core.util import run_length_1d
 from static_frame.core.util import setdiff1d
 from static_frame.core.util import setdiff2d
-from static_frame.core.util import slice_to_ascending_slice
 from static_frame.core.util import slices_from_targets
 from static_frame.core.util import to_datetime64
 from static_frame.core.util import to_timedelta64
 from static_frame.core.util import ufunc_all
 from static_frame.core.util import ufunc_any
 from static_frame.core.util import ufunc_dtype_to_dtype
 from static_frame.core.util import ufunc_nanall
@@ -992,77 +991,14 @@
         self.assertTrue(np.array_equal(expected, _isin_2d(arr_2d, s3)))
 
         arr_1d = np.array([1, 2, 3, 4, 5])
         with self.assertRaises(ValueError):
             _isin_2d(arr_1d, s3)
     #---------------------------------------------------------------------------
 
-    def test_slice_to_ascending_slice_a(self) -> None:
-
-        a1 = np.arange(10)
-
-        def compare(slc: slice) -> None:
-            slc_asc = slice_to_ascending_slice(slc, len(a1))
-            self.assertEqual(sorted(a1[slc]), list(a1[slc_asc]))
-
-        compare(slice(4,))
-        compare(slice(6, 1, -1))
-        compare(slice(6, 1, -2))
-        compare(slice(6, None, -3))
-        compare(slice(6, 2, -2))
-        compare(slice(None, 1, -1))
-
-    def test_slice_to_ascending_slice_b(self) -> None:
-        self.assertEqual(
-            slice_to_ascending_slice(slice(3, None, -1), 10),
-            slice(None, 4, 1)
-            )
-        self.assertEqual(
-            slice_to_ascending_slice(slice(3, None, -3), 10),
-            slice(0, 4, 3)
-            )
-        self.assertEqual(
-            slice_to_ascending_slice(slice(-3, 0, -1), 10),
-            slice(1, 8, 1)
-            )
-        self.assertEqual(
-            slice_to_ascending_slice(slice(-3, None, -1), 10),
-            slice(None, 8, 1)
-            )
-        self.assertEqual(
-            slice_to_ascending_slice(slice(-3, 0, -2), 10),
-            slice(1, 8, 2)
-            )
-        self.assertEqual(
-            slice_to_ascending_slice(slice(-3, None, -2), 10),
-            slice(1, 8, 2)
-            )
-        self.assertEqual(
-            slice_to_ascending_slice(slice(-3, None, -6), 10),
-            slice(1, 8, 6)
-            )
-
-    def test_slice_to_ascending_slice_c(self) -> None:
-        self.assertEqual(
-            slice_to_ascending_slice(slice(-9, -1, 1), 10),
-            slice(-9, -1, 1) # ascenidng
-            )
-        self.assertEqual(
-            slice_to_ascending_slice(slice(-9, -1, -1), 10),
-            slice(0, 0, None) # ascending start stop, descending
-            )
-
-    def test_slice_to_ascending_slice_d(self) -> None:
-        self.assertEqual(
-            slice_to_ascending_slice(slice(1, -10, -1), 10), # [1]
-            slice(1, 2, 1)
-            )
-
-
-
     def test_array_shift_a(self) -> None:
         a1 = np.arange(6)
 
 
         self.assertEqual(array_shift(array=a1, shift=2, axis=0, wrap=True).tolist(),
                 [4, 5, 0, 1, 2, 3])
         self.assertEqual(array_shift(array=a1, shift=-2, axis=0, wrap=True).tolist(),
```

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_www.py` & `static-frame-1.4.3/static_frame/test/unit/test_www.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame/test/unit/test_yarn.py` & `static-frame-1.4.3/static_frame/test/unit/test_yarn.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.2/static_frame.egg-info/PKG-INFO` & `static-frame-1.4.3/static_frame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame
-Version: 1.4.2
+Version: 1.4.3
 Summary: Immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface.
 Home-page: https://github.com/static-frame/static-frame
 Author: Christopher Ariza
 License: MIT
 Description: A library of immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface. StaticFrame is suitable for applications in data science, data engineering, finance, scientific computing, and related fields where reducing opportunities for error by prohibiting in-place mutation is critical.
         
         While many interfaces are similar to Pandas, StaticFrame deviates from Pandas in many ways: all data is immutable, and all indices are unique; the full range of NumPy data types is preserved, and date-time indices use discrete NumPy units; hierarchical indices are seamlessly integrated; and uniform approaches to element, row, and column iteration and function application are provided. Core StaticFrame depends only on NumPy and two C-extension packages (maintained by the StaticFrame team): Pandas is not a dependency.
@@ -46,15 +46,15 @@
         --------------
         
         Core StaticFrame requires the following:
         
         - Python>=3.7
         - NumPy>=1.18.5
         - arraymap==0.1.8
-        - arraykit==0.3.4
+        - arraykit==0.4.8
         
         For extended input and output, the following packages are required:
         
         - pandas>=0.24.2
         - xlsxwriter>=1.1.2
         - openpyxl>=3.0.9
         - xarray>=0.13.0
```

### Comparing `static-frame-1.4.2/static_frame.egg-info/SOURCES.txt` & `static-frame-1.4.3/static_frame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

