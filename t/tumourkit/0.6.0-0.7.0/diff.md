# Comparing `tmp/tumourkit-0.6.0.tar.gz` & `tmp/tumourkit-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tumourkit-0.6.0.tar", last modified: Thu May  4 18:22:57 2023, max compression
+gzip compressed data, was "tumourkit-0.7.0.tar", last modified: Thu May 25 07:57:36 2023, max compression
```

## Comparing `tumourkit-0.6.0.tar` & `tumourkit-0.7.0.tar`

### file list

```diff
@@ -1,156 +1,157 @@
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.163659 tumourkit-0.6.0/
--rw-r--r--   0 joseperezcano   (501) staff       (20)    34523 2022-12-31 13:00:33.000000 tumourkit-0.6.0/LICENSE
--rw-r--r--   0 joseperezcano   (501) staff       (20)    42041 2023-05-04 18:22:57.163143 tumourkit-0.6.0/PKG-INFO
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1269 2023-03-25 17:22:23.000000 tumourkit-0.6.0/README.md
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.039022 tumourkit-0.6.0/docs/
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.038843 tumourkit-0.6.0/docs/buildenv/
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.053707 tumourkit-0.6.0/docs/buildenv/bin/
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      675 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rst2html.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      795 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rst2html4.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1163 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rst2html5.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      872 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rst2latex.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      680 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rst2man.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      845 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rst2odt.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1807 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      682 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      718 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rst2s5.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      952 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rst2xetex.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      683 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rst2xml.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)      751 2023-03-25 16:44:11.000000 tumourkit-0.6.0/docs/buildenv/bin/rstpep2html.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.054458 tumourkit-0.6.0/docs/source/
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1151 2023-04-11 15:21:40.000000 tumourkit-0.6.0/docs/source/conf.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2226 2023-05-04 05:50:12.000000 tumourkit-0.6.0/pyproject.toml
--rw-r--r--   0 joseperezcano   (501) staff       (20)      856 2023-05-04 18:20:19.000000 tumourkit-0.6.0/requirements.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)       38 2023-05-04 18:22:57.163807 tumourkit-0.6.0/setup.cfg
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.075620 tumourkit-0.6.0/tests/
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1596 2023-03-20 09:45:58.000000 tumourkit-0.6.0/tests/centroidspng2csv_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1871 2023-03-06 07:41:04.000000 tumourkit-0.6.0/tests/conf_matrix_sum_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2043 2023-03-06 07:25:02.000000 tumourkit-0.6.0/tests/cpairs_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)      805 2023-03-06 07:25:20.000000 tumourkit-0.6.0/tests/example_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3927 2022-12-31 13:06:14.000000 tumourkit-0.6.0/tests/generate_centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3403 2022-12-31 13:06:04.000000 tumourkit-0.6.0/tests/generate_rswoosh.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1517 2023-03-06 07:25:59.000000 tumourkit-0.6.0/tests/get_conn_comp_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1827 2023-03-28 15:20:41.000000 tumourkit-0.6.0/tests/graph2centroids_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1707 2023-03-20 10:39:44.000000 tumourkit-0.6.0/tests/graph_idx_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2199 2023-03-23 19:39:56.000000 tumourkit-0.6.0/tests/hov_prob_pipe_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2098 2023-03-06 07:27:57.000000 tumourkit-0.6.0/tests/hov_prob_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2503 2023-03-23 07:08:34.000000 tumourkit-0.6.0/tests/hovernet_patches_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1844 2023-03-06 07:41:02.000000 tumourkit-0.6.0/tests/metrics_pairs_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1974 2023-03-06 07:41:00.000000 tumourkit-0.6.0/tests/metrics_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1898 2023-03-20 10:58:10.000000 tumourkit-0.6.0/tests/png2graph_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2240 2023-03-06 07:30:23.000000 tumourkit-0.6.0/tests/pngcsv2geojson_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1829 2023-03-20 10:39:00.000000 tumourkit-0.6.0/tests/pngcsv2graph_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1978 2023-04-12 10:40:07.000000 tumourkit-0.6.0/tests/read_nodes_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1374 2023-03-06 07:31:03.000000 tumourkit-0.6.0/tests/remove_idx_test.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1577 2023-03-06 07:31:28.000000 tumourkit-0.6.0/tests/rswoosh_test.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.083781 tumourkit-0.6.0/tumourkit/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      154 2023-04-30 10:24:02.000000 tumourkit-0.6.0/tumourkit/__init__.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.089478 tumourkit-0.6.0/tumourkit/classification/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      155 2023-04-11 15:25:33.000000 tumourkit-0.6.0/tumourkit/classification/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1349 2023-04-12 10:40:08.000000 tumourkit-0.6.0/tumourkit/classification/compute_imbalance.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     6072 2023-04-12 10:38:57.000000 tumourkit-0.6.0/tumourkit/classification/evaluate.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5318 2023-04-11 18:31:20.000000 tumourkit-0.6.0/tumourkit/classification/infer.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.091791 tumourkit-0.6.0/tumourkit/classification/models/
--rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-11-28 08:50:03.000000 tumourkit-0.6.0/tumourkit/classification/models/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2532 2023-03-23 17:44:30.000000 tumourkit-0.6.0/tumourkit/classification/models/gat.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2008 2022-12-31 13:10:31.000000 tumourkit-0.6.0/tumourkit/classification/models/gcn.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7769 2022-12-31 13:10:48.000000 tumourkit-0.6.0/tumourkit/classification/models/hgao.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2840 2022-12-19 09:14:00.000000 tumourkit-0.6.0/tumourkit/classification/models/norm.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7489 2023-04-12 10:40:12.000000 tumourkit-0.6.0/tumourkit/classification/read_graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    20584 2023-05-01 12:03:44.000000 tumourkit-0.6.0/tumourkit/classification/train_graphs.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    10352 2023-04-12 10:40:17.000000 tumourkit-0.6.0/tumourkit/classification/train_xgboost.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.092350 tumourkit-0.6.0/tumourkit/demo/
--rw-r--r--   0 joseperezcano   (501) staff       (20)    12908 2023-05-04 15:31:12.000000 tumourkit-0.6.0/tumourkit/demo/app.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5613 2023-05-01 12:07:14.000000 tumourkit-0.6.0/tumourkit/eval_pipe.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7511 2023-04-17 15:24:46.000000 tumourkit-0.6.0/tumourkit/infer_pipe.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3151 2023-03-20 14:38:24.000000 tumourkit-0.6.0/tumourkit/make_dirs.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.095546 tumourkit-0.6.0/tumourkit/postprocessing/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      180 2023-05-03 07:48:49.000000 tumourkit-0.6.0/tumourkit/postprocessing/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2601 2023-05-04 07:23:47.000000 tumourkit-0.6.0/tumourkit/postprocessing/draw_cells.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3619 2023-03-09 07:58:38.000000 tumourkit-0.6.0/tumourkit/postprocessing/join_graph_gt.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5469 2023-03-22 15:42:53.000000 tumourkit-0.6.0/tumourkit/postprocessing/join_hovprob_graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5332 2023-04-02 17:54:39.000000 tumourkit-0.6.0/tumourkit/postprocessing/merge_cells.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1623 2023-01-14 21:36:24.000000 tumourkit-0.6.0/tumourkit/postprocessing/rswoosh.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.100141 tumourkit-0.6.0/tumourkit/preprocessing/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      616 2023-03-20 11:26:08.000000 tumourkit-0.6.0/tumourkit/preprocessing/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2298 2023-03-23 19:01:53.000000 tumourkit-0.6.0/tumourkit/preprocessing/centroids2png.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4659 2023-03-25 16:07:13.000000 tumourkit-0.6.0/tumourkit/preprocessing/centroidspng2csv.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3894 2023-04-30 09:54:10.000000 tumourkit-0.6.0/tumourkit/preprocessing/geojson2pngcsv.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3288 2023-03-28 09:36:18.000000 tumourkit-0.6.0/tumourkit/preprocessing/graph2centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2844 2023-03-23 19:09:28.000000 tumourkit-0.6.0/tumourkit/preprocessing/hovernet2centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3723 2023-03-23 19:11:32.000000 tumourkit-0.6.0/tumourkit/preprocessing/hovernet2geojson.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4731 2023-03-23 19:32:48.000000 tumourkit-0.6.0/tumourkit/preprocessing/png2graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2775 2023-03-25 16:11:44.000000 tumourkit-0.6.0/tumourkit/preprocessing/pngcsv2centroids.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5043 2023-04-30 09:55:47.000000 tumourkit-0.6.0/tumourkit/preprocessing/pngcsv2geojson.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3935 2023-03-23 19:32:30.000000 tumourkit-0.6.0/tumourkit/preprocessing/pngcsv2graph.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1075 2023-04-30 10:05:05.000000 tumourkit-0.6.0/tumourkit/preprocessing/remove_uncertain.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.101134 tumourkit-0.6.0/tumourkit/profiling/
--rw-r--r--   0 joseperezcano   (501) staff       (20)     2824 2022-12-31 13:07:35.000000 tumourkit-0.6.0/tumourkit/profiling/cpairs_profile.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1946 2022-12-31 13:07:42.000000 tumourkit-0.6.0/tumourkit/profiling/rswoosh_profile.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    14757 2023-05-03 12:46:59.000000 tumourkit-0.6.0/tumourkit/research_pipe.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.102479 tumourkit-0.6.0/tumourkit/segmentation/
--rw-r--r--   0 joseperezcano   (501) staff       (20)      182 2023-03-08 12:07:32.000000 tumourkit-0.6.0/tumourkit/segmentation/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    12265 2023-04-27 10:59:55.000000 tumourkit-0.6.0/tumourkit/segmentation/evaluate.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.105024 tumourkit-0.6.0/tumourkit/segmentation/hovernet/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2023-03-08 08:02:19.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     2380 2023-03-20 14:44:06.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/config.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.108209 tumourkit-0.6.0/tumourkit/segmentation/hovernet/dataloader/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:49.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/dataloader/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     3322 2023-04-13 06:48:37.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/dataloader/augs.py
--rwx------   0 joseperezcano   (501) staff       (20)     3608 2023-01-26 12:04:04.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/dataloader/infer_loader.py
--rwxr-xr-x   0 joseperezcano   (501) staff       (20)     6632 2023-03-15 12:03:08.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/dataloader/train_loader.py
--rwx------   0 joseperezcano   (501) staff       (20)     8251 2023-03-08 08:12:38.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/extract_patches.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.115379 tumourkit-0.6.0/tumourkit/segmentation/hovernet/infer/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/infer/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     3497 2023-05-03 12:16:27.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/infer/base.py
--rwx------   0 joseperezcano   (501) staff       (20)    14233 2023-03-08 12:23:40.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/infer/tile.py
--rwx------   0 joseperezcano   (501) staff       (20)    30145 2023-03-23 17:33:09.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/infer/wsi.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.119873 tumourkit-0.6.0/tumourkit/segmentation/hovernet/metrics/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/metrics/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)    16129 2023-01-10 14:25:36.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/metrics/stats_utils.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.131029 tumourkit-0.6.0/tumourkit/segmentation/hovernet/misc/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/misc/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     5473 2023-01-10 14:24:57.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/misc/patch_extractor.py
--rwx------   0 joseperezcano   (501) staff       (20)     4951 2023-01-10 14:25:05.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/misc/utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     5727 2023-01-10 14:25:12.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/misc/viz_utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     7419 2023-01-10 14:25:19.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/misc/wsi_handler.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.131735 tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/__init__.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.144098 tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     5421 2023-01-10 14:23:15.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py
--rwx------   0 joseperezcano   (501) staff       (20)     9731 2023-01-10 14:23:26.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     6130 2023-03-15 07:07:22.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/opt.py
--rwx------   0 joseperezcano   (501) staff       (20)     7784 2023-03-22 08:36:42.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py
--rwx------   0 joseperezcano   (501) staff       (20)    13296 2023-03-13 19:48:31.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py
--rwx------   0 joseperezcano   (501) staff       (20)     5117 2023-04-25 06:50:35.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/targets.py
--rwx------   0 joseperezcano   (501) staff       (20)     4903 2023-01-10 16:18:24.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/utils.py
--rwx------   0 joseperezcano   (501) staff       (20)     8325 2023-05-03 12:12:19.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_infer.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.146149 tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/__init__.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.151752 tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/callbacks/
--rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/callbacks/__init__.py
--rwx------   0 joseperezcano   (501) staff       (20)     6991 2023-01-11 07:50:22.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py
--rwx------   0 joseperezcano   (501) staff       (20)     6145 2022-09-15 10:27:54.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py
--rwx------   0 joseperezcano   (501) staff       (20)     5955 2023-01-13 16:18:56.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py
--rwx------   0 joseperezcano   (501) staff       (20)     7482 2023-04-13 06:55:55.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/engine.py
--rwx------   0 joseperezcano   (501) staff       (20)     6834 2023-01-10 14:22:13.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/utils.py
--rwx------   0 joseperezcano   (501) staff       (20)    10663 2023-03-23 18:07:29.000000 tumourkit-0.6.0/tumourkit/segmentation/hovernet/train.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     9861 2023-04-17 15:13:33.000000 tumourkit-0.6.0/tumourkit/train_pipe.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.162298 tumourkit-0.6.0/tumourkit/utils/
--rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-09-26 11:04:45.000000 tumourkit-0.6.0/tumourkit/utils/__init__.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5932 2023-03-23 17:37:13.000000 tumourkit-0.6.0/tumourkit/utils/calibration_error.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5649 2023-05-01 12:06:57.000000 tumourkit-0.6.0/tumourkit/utils/classification.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3606 2023-03-23 18:25:35.000000 tumourkit-0.6.0/tumourkit/utils/folder2txt.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5254 2023-03-23 18:29:29.000000 tumourkit-0.6.0/tumourkit/utils/nearest.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     3094 2023-04-22 10:28:27.000000 tumourkit-0.6.0/tumourkit/utils/pipes.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     7022 2023-03-23 18:35:15.000000 tumourkit-0.6.0/tumourkit/utils/postprocessing.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)    21866 2023-04-30 10:04:39.000000 tumourkit-0.6.0/tumourkit/utils/preprocessing.py
--rw-r--r--   0 joseperezcano   (501) staff       (20)     5714 2023-05-04 05:48:41.000000 tumourkit-0.6.0/tumourkit/utils/read_nodes.py
-drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-04 18:22:57.086899 tumourkit-0.6.0/tumourkit.egg-info/
--rw-r--r--   0 joseperezcano   (501) staff       (20)    42041 2023-05-04 18:22:57.000000 tumourkit-0.6.0/tumourkit.egg-info/PKG-INFO
--rw-r--r--   0 joseperezcano   (501) staff       (20)     4909 2023-05-04 18:22:57.000000 tumourkit-0.6.0/tumourkit.egg-info/SOURCES.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)        1 2023-05-04 18:22:57.000000 tumourkit-0.6.0/tumourkit.egg-info/dependency_links.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)     1000 2023-05-04 18:22:57.000000 tumourkit-0.6.0/tumourkit.egg-info/entry_points.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)      856 2023-05-04 18:22:57.000000 tumourkit-0.6.0/tumourkit.egg-info/requires.txt
--rw-r--r--   0 joseperezcano   (501) staff       (20)       34 2023-05-04 18:22:57.000000 tumourkit-0.6.0/tumourkit.egg-info/top_level.txt
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.458661 tumourkit-0.7.0/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    34523 2022-12-31 13:00:33.000000 tumourkit-0.7.0/LICENSE
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    42041 2023-05-25 07:57:36.458279 tumourkit-0.7.0/PKG-INFO
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1269 2023-03-25 17:22:23.000000 tumourkit-0.7.0/README.md
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.349341 tumourkit-0.7.0/docs/
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.349161 tumourkit-0.7.0/docs/buildenv/
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.364651 tumourkit-0.7.0/docs/buildenv/bin/
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      675 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rst2html.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      795 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rst2html4.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1163 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rst2html5.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      872 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rst2latex.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      680 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rst2man.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      845 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rst2odt.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)     1807 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      682 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      718 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rst2s5.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      952 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rst2xetex.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      683 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rst2xml.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)      751 2023-03-25 16:44:11.000000 tumourkit-0.7.0/docs/buildenv/bin/rstpep2html.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.365470 tumourkit-0.7.0/docs/source/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1151 2023-04-11 15:21:40.000000 tumourkit-0.7.0/docs/source/conf.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2282 2023-05-25 06:24:46.000000 tumourkit-0.7.0/pyproject.toml
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      856 2023-05-04 18:20:19.000000 tumourkit-0.7.0/requirements.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)       38 2023-05-25 07:57:36.458820 tumourkit-0.7.0/setup.cfg
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.383471 tumourkit-0.7.0/tests/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1596 2023-03-20 09:45:58.000000 tumourkit-0.7.0/tests/centroidspng2csv_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1871 2023-03-06 07:41:04.000000 tumourkit-0.7.0/tests/conf_matrix_sum_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2043 2023-03-06 07:25:02.000000 tumourkit-0.7.0/tests/cpairs_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      805 2023-03-06 07:25:20.000000 tumourkit-0.7.0/tests/example_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3927 2022-12-31 13:06:14.000000 tumourkit-0.7.0/tests/generate_centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3403 2022-12-31 13:06:04.000000 tumourkit-0.7.0/tests/generate_rswoosh.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1517 2023-03-06 07:25:59.000000 tumourkit-0.7.0/tests/get_conn_comp_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1827 2023-03-28 15:20:41.000000 tumourkit-0.7.0/tests/graph2centroids_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1707 2023-03-20 10:39:44.000000 tumourkit-0.7.0/tests/graph_idx_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2199 2023-03-23 19:39:56.000000 tumourkit-0.7.0/tests/hov_prob_pipe_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2098 2023-03-06 07:27:57.000000 tumourkit-0.7.0/tests/hov_prob_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2503 2023-03-23 07:08:34.000000 tumourkit-0.7.0/tests/hovernet_patches_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1844 2023-03-06 07:41:02.000000 tumourkit-0.7.0/tests/metrics_pairs_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1974 2023-03-06 07:41:00.000000 tumourkit-0.7.0/tests/metrics_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1898 2023-03-20 10:58:10.000000 tumourkit-0.7.0/tests/png2graph_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2240 2023-03-06 07:30:23.000000 tumourkit-0.7.0/tests/pngcsv2geojson_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1829 2023-03-20 10:39:00.000000 tumourkit-0.7.0/tests/pngcsv2graph_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1978 2023-04-12 10:40:07.000000 tumourkit-0.7.0/tests/read_nodes_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1374 2023-03-06 07:31:03.000000 tumourkit-0.7.0/tests/remove_idx_test.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1577 2023-03-06 07:31:28.000000 tumourkit-0.7.0/tests/rswoosh_test.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.389875 tumourkit-0.7.0/tumourkit/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      154 2023-05-25 06:25:28.000000 tumourkit-0.7.0/tumourkit/__init__.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.398324 tumourkit-0.7.0/tumourkit/classification/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      155 2023-04-11 15:25:33.000000 tumourkit-0.7.0/tumourkit/classification/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1356 2023-05-18 07:19:54.000000 tumourkit-0.7.0/tumourkit/classification/compute_imbalance.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     6104 2023-05-18 07:21:56.000000 tumourkit-0.7.0/tumourkit/classification/evaluate.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5305 2023-05-18 07:22:57.000000 tumourkit-0.7.0/tumourkit/classification/infer.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.402069 tumourkit-0.7.0/tumourkit/classification/models/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-11-28 08:50:03.000000 tumourkit-0.7.0/tumourkit/classification/models/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2532 2023-03-23 17:44:30.000000 tumourkit-0.7.0/tumourkit/classification/models/gat.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2008 2022-12-31 13:10:31.000000 tumourkit-0.7.0/tumourkit/classification/models/gcn.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7769 2022-12-31 13:10:48.000000 tumourkit-0.7.0/tumourkit/classification/models/hgao.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2840 2022-12-19 09:14:00.000000 tumourkit-0.7.0/tumourkit/classification/models/norm.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7575 2023-05-18 07:24:15.000000 tumourkit-0.7.0/tumourkit/classification/read_graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    20658 2023-05-18 07:28:33.000000 tumourkit-0.7.0/tumourkit/classification/train_graphs.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    10426 2023-05-18 07:32:33.000000 tumourkit-0.7.0/tumourkit/classification/train_xgboost.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.403464 tumourkit-0.7.0/tumourkit/demo/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    12884 2023-05-18 07:16:15.000000 tumourkit-0.7.0/tumourkit/demo/app.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     6349 2023-05-18 07:55:33.000000 tumourkit-0.7.0/tumourkit/eval_pipe.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     8197 2023-05-18 07:55:46.000000 tumourkit-0.7.0/tumourkit/infer_pipe.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3924 2023-05-18 07:56:05.000000 tumourkit-0.7.0/tumourkit/make_dirs.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.408799 tumourkit-0.7.0/tumourkit/postprocessing/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      180 2023-05-03 07:48:49.000000 tumourkit-0.7.0/tumourkit/postprocessing/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2591 2023-05-25 07:56:12.000000 tumourkit-0.7.0/tumourkit/postprocessing/draw_cells.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5344 2023-05-25 07:55:08.000000 tumourkit-0.7.0/tumourkit/postprocessing/draw_graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3623 2023-05-18 07:05:34.000000 tumourkit-0.7.0/tumourkit/postprocessing/join_graph_gt.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5472 2023-05-18 07:06:54.000000 tumourkit-0.7.0/tumourkit/postprocessing/join_hovprob_graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5407 2023-05-18 07:10:02.000000 tumourkit-0.7.0/tumourkit/postprocessing/merge_cells.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1660 2023-05-18 07:11:45.000000 tumourkit-0.7.0/tumourkit/postprocessing/rswoosh.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.418893 tumourkit-0.7.0/tumourkit/preprocessing/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      616 2023-03-20 11:26:08.000000 tumourkit-0.7.0/tumourkit/preprocessing/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2307 2023-05-18 06:57:47.000000 tumourkit-0.7.0/tumourkit/preprocessing/centroids2png.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4660 2023-05-18 06:58:20.000000 tumourkit-0.7.0/tumourkit/preprocessing/centroidspng2csv.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3892 2023-05-18 07:00:03.000000 tumourkit-0.7.0/tumourkit/preprocessing/geojson2pngcsv.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3289 2023-05-18 07:00:16.000000 tumourkit-0.7.0/tumourkit/preprocessing/graph2centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2825 2023-05-18 07:00:48.000000 tumourkit-0.7.0/tumourkit/preprocessing/hovernet2centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3720 2023-05-18 07:01:18.000000 tumourkit-0.7.0/tumourkit/preprocessing/hovernet2geojson.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4731 2023-05-18 07:02:17.000000 tumourkit-0.7.0/tumourkit/preprocessing/png2graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2777 2023-05-18 07:02:32.000000 tumourkit-0.7.0/tumourkit/preprocessing/pngcsv2centroids.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5041 2023-05-18 07:02:55.000000 tumourkit-0.7.0/tumourkit/preprocessing/pngcsv2geojson.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3945 2023-05-18 07:03:41.000000 tumourkit-0.7.0/tumourkit/preprocessing/pngcsv2graph.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1861 2023-05-18 07:42:25.000000 tumourkit-0.7.0/tumourkit/preprocessing/remove_uncertain.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.420685 tumourkit-0.7.0/tumourkit/profiling/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     2747 2023-05-18 07:35:28.000000 tumourkit-0.7.0/tumourkit/profiling/cpairs_profile.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1915 2023-05-18 07:36:50.000000 tumourkit-0.7.0/tumourkit/profiling/rswoosh_profile.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    15312 2023-05-18 07:56:19.000000 tumourkit-0.7.0/tumourkit/research_pipe.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.422293 tumourkit-0.7.0/tumourkit/segmentation/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      182 2023-03-08 12:07:32.000000 tumourkit-0.7.0/tumourkit/segmentation/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    12362 2023-05-18 07:40:19.000000 tumourkit-0.7.0/tumourkit/segmentation/evaluate.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.426797 tumourkit-0.7.0/tumourkit/segmentation/hovernet/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2023-03-08 08:02:19.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     2380 2023-03-20 14:44:06.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/config.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.429271 tumourkit-0.7.0/tumourkit/segmentation/hovernet/dataloader/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:49.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/dataloader/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     3322 2023-04-13 06:48:37.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/dataloader/augs.py
+-rwx------   0 joseperezcano   (501) staff       (20)     3608 2023-01-26 12:04:04.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/dataloader/infer_loader.py
+-rwxr-xr-x   0 joseperezcano   (501) staff       (20)     6632 2023-03-15 12:03:08.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/dataloader/train_loader.py
+-rwx------   0 joseperezcano   (501) staff       (20)     8251 2023-03-08 08:12:38.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/extract_patches.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.431527 tumourkit-0.7.0/tumourkit/segmentation/hovernet/infer/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/infer/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     3497 2023-05-03 12:16:27.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/infer/base.py
+-rwx------   0 joseperezcano   (501) staff       (20)    14233 2023-03-08 12:23:40.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/infer/tile.py
+-rwx------   0 joseperezcano   (501) staff       (20)    30145 2023-03-23 17:33:09.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/infer/wsi.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.433636 tumourkit-0.7.0/tumourkit/segmentation/hovernet/metrics/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/metrics/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)    16129 2023-01-10 14:25:36.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/metrics/stats_utils.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.437934 tumourkit-0.7.0/tumourkit/segmentation/hovernet/misc/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/misc/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5473 2023-01-10 14:24:57.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/misc/patch_extractor.py
+-rwx------   0 joseperezcano   (501) staff       (20)     4951 2023-01-10 14:25:05.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/misc/utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5727 2023-01-10 14:25:12.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/misc/viz_utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     7419 2023-01-10 14:25:19.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/misc/wsi_handler.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.438793 tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/__init__.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.444226 tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:53.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5421 2023-01-10 14:23:15.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py
+-rwx------   0 joseperezcano   (501) staff       (20)     9731 2023-01-10 14:23:26.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6130 2023-03-15 07:07:22.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/opt.py
+-rwx------   0 joseperezcano   (501) staff       (20)     7784 2023-03-22 08:36:42.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py
+-rwx------   0 joseperezcano   (501) staff       (20)    13296 2023-03-13 19:48:31.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5117 2023-04-25 06:50:35.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/targets.py
+-rwx------   0 joseperezcano   (501) staff       (20)     4903 2023-01-10 16:18:24.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)     8325 2023-05-03 12:12:19.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_infer.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.446066 tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/__init__.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.448182 tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/callbacks/
+-rwx------   0 joseperezcano   (501) staff       (20)        0 2022-09-15 10:27:54.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/callbacks/__init__.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6991 2023-01-11 07:50:22.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6145 2022-09-15 10:27:54.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py
+-rwx------   0 joseperezcano   (501) staff       (20)     5955 2023-01-13 16:18:56.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py
+-rwx------   0 joseperezcano   (501) staff       (20)     7482 2023-04-13 06:55:55.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/engine.py
+-rwx------   0 joseperezcano   (501) staff       (20)     6834 2023-01-10 14:22:13.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/utils.py
+-rwx------   0 joseperezcano   (501) staff       (20)    10663 2023-03-23 18:07:29.000000 tumourkit-0.7.0/tumourkit/segmentation/hovernet/train.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    10454 2023-05-18 07:56:27.000000 tumourkit-0.7.0/tumourkit/train_pipe.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.457319 tumourkit-0.7.0/tumourkit/utils/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)        0 2022-09-26 11:04:45.000000 tumourkit-0.7.0/tumourkit/utils/__init__.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5934 2023-05-18 06:31:59.000000 tumourkit-0.7.0/tumourkit/utils/calibration_error.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5658 2023-05-18 06:37:18.000000 tumourkit-0.7.0/tumourkit/utils/classification.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3611 2023-05-18 06:39:27.000000 tumourkit-0.7.0/tumourkit/utils/folder2txt.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5321 2023-05-18 06:43:10.000000 tumourkit-0.7.0/tumourkit/utils/nearest.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     3074 2023-05-18 06:43:40.000000 tumourkit-0.7.0/tumourkit/utils/pipes.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     7053 2023-05-18 06:46:21.000000 tumourkit-0.7.0/tumourkit/utils/postprocessing.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    21855 2023-05-18 06:54:22.000000 tumourkit-0.7.0/tumourkit/utils/preprocessing.py
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     5798 2023-05-18 06:56:50.000000 tumourkit-0.7.0/tumourkit/utils/read_nodes.py
+drwxr-xr-x   0 joseperezcano   (501) staff       (20)        0 2023-05-25 07:57:36.392578 tumourkit-0.7.0/tumourkit.egg-info/
+-rw-r--r--   0 joseperezcano   (501) staff       (20)    42041 2023-05-25 07:57:36.000000 tumourkit-0.7.0/tumourkit.egg-info/PKG-INFO
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     4948 2023-05-25 07:57:36.000000 tumourkit-0.7.0/tumourkit.egg-info/SOURCES.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)        1 2023-05-25 07:57:36.000000 tumourkit-0.7.0/tumourkit.egg-info/dependency_links.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)     1054 2023-05-25 07:57:36.000000 tumourkit-0.7.0/tumourkit.egg-info/entry_points.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)      856 2023-05-25 07:57:36.000000 tumourkit-0.7.0/tumourkit.egg-info/requires.txt
+-rw-r--r--   0 joseperezcano   (501) staff       (20)       38 2023-05-25 07:57:36.000000 tumourkit-0.7.0/tumourkit.egg-info/top_level.txt
```

### Comparing `tumourkit-0.6.0/LICENSE` & `tumourkit-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/PKG-INFO` & `tumourkit-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumourkit
-Version: 0.6.0
+Version: 0.7.0
 Summary: A SDK for tumour study
 Author-email: Jose Pérez Cano <joseperez2000@hotmail.es>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `tumourkit-0.6.0/README.md` & `tumourkit-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/docs/buildenv/bin/rst2html.py` & `tumourkit-0.7.0/docs/buildenv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/docs/buildenv/bin/rst2html4.py` & `tumourkit-0.7.0/docs/buildenv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/docs/buildenv/bin/rst2html5.py` & `tumourkit-0.7.0/docs/buildenv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/docs/buildenv/bin/rst2latex.py` & `tumourkit-0.7.0/docs/buildenv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/docs/buildenv/bin/rst2man.py` & `tumourkit-0.7.0/docs/buildenv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/docs/buildenv/bin/rst2odt.py` & `tumourkit-0.7.0/docs/buildenv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/docs/buildenv/bin/rst2odt_prepstyles.py` & `tumourkit-0.7.0/docs/buildenv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/docs/buildenv/bin/rst2pseudoxml.py` & `tumourkit-0.7.0/docs/buildenv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/docs/buildenv/bin/rst2s5.py` & `tumourkit-0.7.0/docs/buildenv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/docs/buildenv/bin/rst2xetex.py` & `tumourkit-0.7.0/docs/buildenv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/docs/buildenv/bin/rst2xml.py` & `tumourkit-0.7.0/docs/buildenv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/docs/buildenv/bin/rstpep2html.py` & `tumourkit-0.7.0/docs/buildenv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/docs/source/conf.py` & `tumourkit-0.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/pyproject.toml` & `tumourkit-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -51,8 +51,9 @@
 run_training = "tumourkit.train_pipe:main"
 run_inference = "tumourkit.infer_pipe:main"
 run_research = "tumourkit.research_pipe:main"
 run_evaluation = "tumourkit.eval_pipe:main"
 merge_cells = "tumourkit.postprocessing.merge_cells:main"
 remove_uncertain = "tumourkit.preprocessing.remove_uncertain:main"
 draw_cells = "tumourkit.postprocessing.draw_cells:main"
-start_app = "tumourkit.demo.app:main"
+start_app = "tumourkit.demo.app:main"
+draw_graph = "tumourkit.postprocessing.draw_graph:main"
```

### Comparing `tumourkit-0.6.0/requirements.txt` & `tumourkit-0.7.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tests/centroidspng2csv_test.py` & `tumourkit-0.7.0/tests/centroidspng2csv_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tests/conf_matrix_sum_test.py` & `tumourkit-0.7.0/tests/conf_matrix_sum_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tests/cpairs_test.py` & `tumourkit-0.7.0/tests/cpairs_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tests/example_test.py` & `tumourkit-0.7.0/tests/example_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tests/generate_centroids.py` & `tumourkit-0.7.0/tests/generate_centroids.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tests/generate_rswoosh.py` & `tumourkit-0.7.0/tests/generate_rswoosh.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tests/get_conn_comp_test.py` & `tumourkit-0.7.0/tests/get_conn_comp_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tests/graph2centroids_test.py` & `tumourkit-0.7.0/tests/graph2centroids_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tests/graph_idx_test.py` & `tumourkit-0.7.0/tests/graph_idx_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tests/hov_prob_pipe_test.py` & `tumourkit-0.7.0/tests/hov_prob_pipe_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tests/hov_prob_test.py` & `tumourkit-0.7.0/tests/hov_prob_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tests/hovernet_patches_test.py` & `tumourkit-0.7.0/tests/hovernet_patches_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tests/metrics_pairs_test.py` & `tumourkit-0.7.0/tests/metrics_pairs_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tests/metrics_test.py` & `tumourkit-0.7.0/tests/metrics_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tests/png2graph_test.py` & `tumourkit-0.7.0/tests/png2graph_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tests/pngcsv2geojson_test.py` & `tumourkit-0.7.0/tests/pngcsv2geojson_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tests/pngcsv2graph_test.py` & `tumourkit-0.7.0/tests/pngcsv2graph_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tests/read_nodes_test.py` & `tumourkit-0.7.0/tests/read_nodes_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tests/remove_idx_test.py` & `tumourkit-0.7.0/tests/remove_idx_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tests/rswoosh_test.py` & `tumourkit-0.7.0/tests/rswoosh_test.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/classification/compute_imbalance.py` & `tumourkit-0.7.0/tumourkit/classification/compute_imbalance.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,16 +23,17 @@
 import os
 import numpy as np
 
 FILE_DIR = os.path.dirname(os.path.abspath(__file__))
 
 parser = argparse.ArgumentParser()
 parser.add_argument('--graph-dir', type=str, required=True,
-                     help='Folder containing .graph.csv files.')
+                    help='Folder containing .graph.csv files.')
 
-if __name__=='__main__':
+
+if __name__ == '__main__':
     args = parser.parse_args()
     GRAPH_DIR = args.graph_dir
 
     X, y = read_all_nodes(GRAPH_DIR, os.listdir(GRAPH_DIR))
-    print('Number of tumoral cells:', np.sum(y==1))
-    print('Number of non-tumoral cells:', np.sum(y==0))
+    print('Number of tumoral cells:', np.sum(y == 1))
+    print('Number of non-tumoral cells:', np.sum(y == 0))
```

### Comparing `tumourkit-0.6.0/tumourkit/classification/evaluate.py` & `tumourkit-0.7.0/tumourkit/classification/evaluate.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,32 +34,33 @@
     """
     Plot a line from slope and intercept on current axis.
     """
     x_vals = np.array(axes.get_xlim())
     y_vals = intercept + slope * x_vals
     axes.plot(x_vals, y_vals, linestyle='dotted', color='k')
 
+
 def draw_reliability_diagram(
-    y_true: np.ndarray, 
-    y_probs: np.ndarray, 
-    save_path: str, 
-    method_name: str
-    ) -> None:
+        y_true: np.ndarray,
+        y_probs: np.ndarray,
+        save_path: str,
+        method_name: str
+        ) -> None:
     """
     Draws reliability diagram into save_path.
     save_path must not contain extension.
     """
     prob_true, prob_pred = calibration_curve(y_true, y_probs, n_bins=20)
 
-    fig, ax = plt.subplots(1,2, figsize=(16,6))
+    fig, ax = plt.subplots(1, 2, figsize=(16, 6))
     ax[0].plot(prob_pred, prob_true, marker='s', color='forestgreen')
     abline(1, 0, ax[0])
     ax[0].set(
-        title='Reliability diagram', 
-        xlabel='Mean predicted probability', 
+        title='Reliability diagram',
+        xlabel='Mean predicted probability',
         ylabel='Fraction of positives'
     )
     ax[0].legend([method_name, 'Perfectly calibrated'])
 
     ax[1].hist(
         y_probs,
         range=(0, 1),
@@ -68,42 +69,45 @@
         color='forestgreen',
     )
     ax[1].set(title=method_name, xlabel="Mean predicted probability", ylabel="Count")
 
     fig.savefig(save_path + '.png')
     plt.close(fig)
 
+
 def compute_metrics(
-    nodes_df: pd.DataFrame, 
-    draw_on: Optional[str] = None, 
-    method_name: Optional[str] = 'Method'
-    ) -> Dict[str, float]:
+        nodes_df: pd.DataFrame,
+        draw_on: Optional[str] = None,
+        method_name: Optional[str] = 'Method'
+        ) -> Dict[str, float]:
     """
     Computes F1-score, Accuracy, ROC AUC, Expected Calibration Error and percentage error.
     Dataframe must contain columns class and prob1.
     Class columns must have 1 for negative and 2 for positive.
     """
-    labels = nodes_df['class'].to_numpy()-1
+    labels = nodes_df['class'].to_numpy() - 1
     probs = nodes_df['prob1'].to_numpy()
     preds = (probs > 0.5) * 1
 
     acc, f1, auc, perc_error, ece = metrics_from_predictions(labels, preds, probs, 2)
 
     if draw_on is not None:
         draw_reliability_diagram(labels, probs, draw_on, method_name)
 
     return {'Accuracy': acc, 'F1-score': f1, 'ROC AUC': auc, 'Error percentage': perc_error, 'ECE': ece}
 
+
 def save_metrics(metrics: Dict[str, float], save_name):
     """
     Saves metrics into csv file.
     """
     metrics_df = pd.DataFrame(metrics)
     metrics_df.to_csv(save_name + '.csv', index=False)
-    
+
+
 def join_dictionaries(dict1: Dict[str, List[float]], dict2: Dict[str, float]) -> None:
     """
     Joins dict2 into dict1, modifying dict1.
     For each key it adds the value in dict2 to the list in dict1,
     if dict1 doesn't have such key, it is created.
     """
     for key in dict2.keys():
@@ -118,17 +122,17 @@
                         help='Folder with .nodes.csv prediction files.')
     parser.add_argument('--save-file', type=str, required=True,
                         help='Name to file where to save the results. Must not contain extension.')
     parser.add_argument('--by-img', action='store_true',
                         help='Whether to evaluate images separately or totally.')
     parser.add_argument('--draw', action='store_true',
                         help='Whether to draw reliability diagrams.')
-    parser.add_argument('--draw-dir', type=str, 
+    parser.add_argument('--draw-dir', type=str,
                         help='Folder to save reliability diagram on by-img mode.')
-    parser.add_argument('--name', type=str, default='Method', 
+    parser.add_argument('--name', type=str, default='Method',
                         help='The name of the model used. Default: Method.')
     return parser
 
 
 def main_with_args(args):
     node_files = os.listdir(args.node_dir)
     node_paths = [parse_path(args.node_dir) + x for x in node_files]
@@ -145,15 +149,15 @@
                 aux_metrics = compute_metrics(nodes_df)
             aux_metrics['name'] = node_file[:-10]
             join_dictionaries(metrics, aux_metrics)
     else:
         total_nodes_df = pd.DataFrame()
         for node_path in node_paths:
             nodes_df = pd.read_csv(node_path)
-            total_nodes_df = pd.concat([total_nodes_df,nodes_df])
+            total_nodes_df = pd.concat([total_nodes_df, nodes_df])
         total_nodes_df.reset_index(inplace=True)
         total_nodes_df.drop('index', axis=1, inplace=True)
         if args.draw:
             aux_metrics = compute_metrics(total_nodes_df, draw_on=args.save_file, method_name=args.name)
         else:
             aux_metrics = compute_metrics(total_nodes_df)
         join_dictionaries(metrics, aux_metrics)
```

### Comparing `tumourkit-0.6.0/tumourkit/classification/infer.py` & `tumourkit-0.7.0/tumourkit/classification/infer.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,56 +29,59 @@
 from dgl.dataloading import GraphDataLoader
 import json
 import pickle
 import numpy as np
 import pandas as pd
 import argparse
 import os
-                  
+
 
 def load_saved_model(weights_path: str, conf_path: str, num_classes: int, num_feats: int) -> nn.Module:
     """
     Loads state_dict into a torch module.
     Configuration file must match with state_dict.
     """
     state_dict = torch.load(weights_path, map_location='cpu')
     with open(conf_path, 'r') as f:
         conf = json.load(f)
     model = load_model(conf, num_classes, num_feats)
     model.load_state_dict(state_dict)
     return model
 
+
 def load_normalizer(norm_path: str) -> Tuple[Any]:
     """
     Returns normalizers used in training save at norm_path.
     """
     with open(norm_path, 'rb') as f:
         normalizers = pickle.load(f)
     return normalizers
 
+
 def run_inference(model: nn.Module, loader: GraphDataLoader, device: str, num_classes: int) -> Dict[str, np.ndarray]:
     """
     Computes probabilities for all the nodes.
     """
     probs = {}
     for g, name in loader:
         # self-loops
         g = dgl.remove_self_loop(g)
         g = dgl.add_self_loop(g)
         # data
         features = g.ndata['X'].to(device)
         # Forward
         logits = model(g, features)
         if num_classes == 2:
-            prob = F.softmax(logits, dim=1).detach().numpy()[:,1].reshape(-1,1)
+            prob = F.softmax(logits, dim=1).detach().numpy()[:, 1].reshape(-1, 1)
         else:
             prob = F.softmax(logits, dim=1).detach().numpy()
         probs[name[0]] = prob
     return probs
 
+
 def save_probs(probs: Dict[str, np.ndarray], node_dir: str, output_dir: str, num_classes: int) -> None:
     """
     Saves probabilities in .nodes.csv files.
     It appends a column to original .nodes.csv file.
     """
     for name, prob in probs.items():
         orig = pd.read_csv(os.path.join(node_dir, name))
@@ -93,15 +96,15 @@
 def _create_parser():
     parser = argparse.ArgumentParser()
     parser.add_argument('--node-dir', type=str, required=True,
                         help='Folder containing .nodes.csv')
     parser.add_argument('--output-dir', type=str, required=True,
                         help='Folder to save .nodes.csv containing probabilities.')
     parser.add_argument('--weights', type=str, required=True,
-                        help='Path to model weights.')  
+                        help='Path to model weights.')
     parser.add_argument('--conf', type=str, required=True,
                         help='Configuration file for the model.')
     parser.add_argument('--normalizers', type=str, required=True,
                         help='Path to normalizer objects for the model.')
     parser.add_argument('--num-classes', type=int, default=2, help='Number of classes to consider for classification (background not included).')
     parser.add_argument('--disable-prior', action='store_true', help='If True, remove hovernet probabilities from node features.')
     parser.add_argument('--disable-morph-feats', action='store_true', help='If True, remove morphological features from node features.')
@@ -126,11 +129,12 @@
     if num_feats == 0:
         num_feats = 1
     model = load_saved_model(args.weights, args.conf, args.num_classes, num_feats)
     model.eval()
     probs = run_inference(model, eval_dataloader, 'cpu', args.num_classes)
     save_probs(probs, node_dir, output_dir, args.num_classes)
 
+
 def main():
     parser = _create_parser()
     args = parser.parse_args()
-    main(args)
+    main(args)
```

### Comparing `tumourkit-0.6.0/tumourkit/classification/models/gat.py` & `tumourkit-0.7.0/tumourkit/classification/models/gat.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/classification/models/gcn.py` & `tumourkit-0.7.0/tumourkit/classification/models/gcn.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/classification/models/hgao.py` & `tumourkit-0.7.0/tumourkit/classification/models/hgao.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/classification/models/norm.py` & `tumourkit-0.7.0/tumourkit/classification/models/norm.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/classification/read_graph.py` & `tumourkit-0.7.0/tumourkit/classification/read_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,34 +27,36 @@
 from ..utils.classification import fit_column_normalizer
 from ..utils.read_nodes import read_node_matrix
 import torch
 from torch.utils.data import Dataset
 import dgl
 from sklearn.preprocessing import Normalizer
 
+
 class GraphDataset(Dataset):
     """
     Torch Dataset to load graphs from .nodes.csv files.
 
     Generated graph is in DGL format, with node attributes in .ndata
     and edge attributes in .edata.
 
     Graph edges are generated on the fly.
     """
-    def __init__(self, node_dir: str, max_dist: float, max_degree: int,
-        files: Optional[List[str]] = None,
-        transform: Optional[Callable[[np.ndarray], np.ndarray]] = None,
-        column_normalize: Optional[bool] = False,
-        row_normalize: Optional[bool] = False,
-        normalizers: Optional[Tuple[Any]] = None,
-        return_names: Optional[bool] = False,
-        is_inference: Optional[bool] = False,
-        remove_prior: Optional[bool] = False,
-        remove_morph: Optional[bool] = False,
-        ):
+    def __init__(
+            self, node_dir: str, max_dist: float, max_degree: int,
+            files: Optional[List[str]] = None,
+            transform: Optional[Callable[[np.ndarray], np.ndarray]] = None,
+            column_normalize: Optional[bool] = False,
+            row_normalize: Optional[bool] = False,
+            normalizers: Optional[Tuple[Any]] = None,
+            return_names: Optional[bool] = False,
+            is_inference: Optional[bool] = False,
+            remove_prior: Optional[bool] = False,
+            remove_morph: Optional[bool] = False,
+            ):
         """
         node_dir: Path to .nodes.csv files.
         max_dist: Maximum distance to consider two nodes as neighbours.
         max_degree: Maximum degree for each node.
         files: List of names to include in the dataset. If None all names are included.
         column_normalize: Whether to subtract mean and divide by standard deviation each feature.
         row_normalize: Whether to apply row normalization. Reference: https://pytorch-geometric.readthedocs.io/en/latest/_modules/torch_geometric/transforms/normalize_features.html#NormalizeFeatures
@@ -95,25 +97,27 @@
         if self.transform is not None:
             X = self.transform(X)
         source, dest, dists = GraphDataset.create_edges(xx, yy, self.max_degree, self.max_dist)
         g = dgl.graph((source, dest), num_nodes=len(X))
         g.ndata['X'] = torch.tensor(X, dtype=torch.float32)
         if not self.is_inference:
             g.ndata['y'] = torch.tensor(y, dtype=torch.long)
-        g.edata['dist'] = torch.tensor(dists, dtype=torch.float32).reshape((-1,1))
+        g.edata['dist'] = torch.tensor(dists, dtype=torch.float32).reshape((-1, 1))
         if self.return_names:
             return g, file_name
         return g
 
     def __len__(self):
         return len(self.node_names)
 
     @staticmethod
-    def create_edges(xx: List[float], yy: List[float],
-        max_degree: int, threshold: float) -> Tuple[List[int], List[int]]:
+    def create_edges(
+            xx: List[float], yy: List[float],
+            max_degree: int, threshold: float
+            ) -> Tuple[List[int], List[int]]:
         """
         Creates edges between nearby nodes.
 
         xx: X coordinates of nodes.
         yy: Y coordinates of nodes.
         max_degree: Maximum degree for each node.
         threshold: Maximum distance to look at.
@@ -122,15 +126,15 @@
         source: List of source nodes id.
         dest: List of destination nodes id.
         distances: Distances between nodes in edges.
         """
         tree = generate_tree(zip(xx, yy))
         source, dest, distances = [], [], []
         for i, (x, y) in enumerate(zip(xx, yy)):
-            dists, idx = tree.query((x,y), k=max_degree, distance_upper_bound=threshold)
+            dists, idx = tree.query((x, y), k=max_degree, distance_upper_bound=threshold)
             tmp = list(filter(lambda x: x[0] > 1e-10 and x[1] < len(xx), zip(dists, idx)))
             tmp1, tmp2 = tee(tmp)
             dists, idx = list(x[0] for x in tmp1), list(x[1] for x in tmp2)
             source.extend([i for _ in range(len(idx))])
             dest.extend(idx)
             distances.extend(dists)
         return source, dest, distances
@@ -142,19 +146,19 @@
         if self.normalizers is not None:
             for normalizer in self.normalizers:
                 assert callable(getattr(normalizer, "transform", None)), \
                     'Normalizers provided must have transform method.'
         if self.column_normalize:
             self.col_sc = fit_column_normalizer(self.node_dir, self.node_names, remove_morph=self.remove_morph, remove_prior=self.remove_prior)
             assert callable(getattr(self.col_sc, "transform", None)), \
-            'Error loading column normalizer.'
+                'Error loading column normalizer.'
         if self.row_normalize:
             self.row_sc = Normalizer(norm='l1')
             assert callable(getattr(self.row_sc, "transform", None)), \
-            'Error loading row normalizer.'
+                'Error loading row normalizer.'
 
     def get_normalizers(self) -> Tuple[Any]:
         """
         Returns a tuple with all the normalizers in the order they are used.
         """
         if self.column_normalize and self.row_normalize and self.normalizers is not None:
             return [self.col_sc, self.row_sc, *self.normalizers]
@@ -166,8 +170,7 @@
             return [self.row_sc, *self.normalizers]
         if self.column_normalize:
             return [self.col_sc]
         if self.row_normalize and self.normalizers is not None:
             return [self.row_sc, *self.normalizers]
         if self.normalizers is not None:
             return self.normalizers
-
```

### Comparing `tumourkit-0.6.0/tumourkit/classification/train_graphs.py` & `tumourkit-0.7.0/tumourkit/classification/train_graphs.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 from concurrent.futures import ThreadPoolExecutor
 import json
 import pickle
 from ..utils.preprocessing import parse_path, create_dir
 from ..utils.classification import metrics_from_predictions
 warnings.filterwarnings('ignore')
 
+
 def evaluate(
         loader: GraphDataLoader,
         model: nn.Module,
         device: str,
         writer: Optional[SummaryWriter] = None,
         epoch: Optional[int] = None,
         log_suffix: Optional[str] = None,
@@ -55,39 +56,39 @@
         ) -> List[float]:
     """
     Evaluates model in loader.
     Logs to tensorboard with suffix log_suffix.
     Returns the model in evaluation mode.
     """
     model.eval()
-    preds, labels, probs = np.array([]).reshape(0,1), np.array([]).reshape(0,1), np.array([]).reshape(0,1 if num_classes == 2 else num_classes)
+    preds, labels, probs = np.array([]).reshape(0, 1), np.array([]).reshape(0, 1), np.array([]).reshape(0, 1 if num_classes == 2 else num_classes)
     for g in loader:
         g = g.to(device)
         # self-loops
         g = dgl.remove_self_loop(g)
         g = dgl.add_self_loop(g)
         # data
         features = g.ndata['X']
         # Forward
         logits = model(g, features)
-        pred = logits.argmax(1).detach().cpu().numpy().reshape(-1,1)
+        pred = logits.argmax(1).detach().cpu().numpy().reshape(-1, 1)
         preds = np.vstack((preds, pred))
         if num_classes == 2:
-            prob = F.softmax(logits, dim=1).detach().cpu().numpy()[:,1].reshape(-1,1)
+            prob = F.softmax(logits, dim=1).detach().cpu().numpy()[:, 1].reshape(-1, 1)
         else:
             prob = F.softmax(logits, dim=1).detach().cpu().numpy()
         probs = np.vstack((probs, prob))
-        label = g.ndata['y'].detach().cpu().numpy().reshape(-1,1)
+        label = g.ndata['y'].detach().cpu().numpy().reshape(-1, 1)
         labels = np.vstack((labels, label))
-    # Compute metrics on validation  
+    # Compute metrics on validation
     if num_classes == 2:
         acc, f1, auc, perc_err, ece = metrics_from_predictions(labels, preds, probs, 2)
         # Tensorboard
         if writer is not None:
-            assert(log_suffix is not None and epoch is not None)
+            assert (log_suffix is not None and epoch is not None)
             writer.add_scalar('Accuracy/' + log_suffix, acc, epoch)
             writer.add_scalar('F1/' + log_suffix, f1, epoch)
             writer.add_scalar('ROC_AUC/' + log_suffix, auc, epoch)
             writer.add_scalar('Percentage Error/' + log_suffix, perc_err, epoch)
             writer.add_scalar('ECE/' + log_suffix, ece, epoch)
         return f1, acc, auc, perc_err, ece
     else:
@@ -95,15 +96,15 @@
         # Tensorboard
         if writer is not None:
             writer.add_scalar('Accuracy/' + log_suffix, micro, epoch)
             writer.add_scalar('Macro F1/' + log_suffix, macro, epoch)
             writer.add_scalar('Weighted F1/' + log_suffix, weighted, epoch)
             writer.add_scalar('ECE/' + log_suffix, ece, epoch)
         return micro, macro, weighted, ece
-    
+
 
 def train_one_iter(
         tr_loader: GraphDataLoader,
         model: nn.Module,
         device: str,
         optimizer: Optimizer,
         epoch: int,
@@ -129,43 +130,44 @@
         optimizer.zero_grad()
         loss.backward()
         optimizer.step()
         # Compute metrics on training
         preds = logits.argmax(1).detach().cpu().numpy()
         labels = labels.detach().cpu().numpy()
         if num_classes == 2:
-            probs = F.softmax(logits, dim=1).detach().cpu().numpy()[:,1]
+            probs = F.softmax(logits, dim=1).detach().cpu().numpy()[:, 1]
             train_acc, train_f1, train_auc, train_perc_err, train_ece = metrics_from_predictions(labels, preds, probs, 2)
             # Tensorboard
-            writer.add_scalar('Accuracy/train', train_acc, step+len(tr_loader)*epoch)
-            writer.add_scalar('F1/train', train_f1, step+len(tr_loader)*epoch)
-            writer.add_scalar('ROC_AUC/train', train_auc, step+len(tr_loader)*epoch)
-            writer.add_scalar('ECE/train', train_ece, step+len(tr_loader)*epoch)
-            writer.add_scalar('Percentage Error/train', train_perc_err, step+len(tr_loader)*epoch)
+            writer.add_scalar('Accuracy/train', train_acc, step + len(tr_loader) * epoch)
+            writer.add_scalar('F1/train', train_f1, step + len(tr_loader) * epoch)
+            writer.add_scalar('ROC_AUC/train', train_auc, step + len(tr_loader) * epoch)
+            writer.add_scalar('ECE/train', train_ece, step + len(tr_loader) * epoch)
+            writer.add_scalar('Percentage Error/train', train_perc_err, step + len(tr_loader) * epoch)
         else:
             probs = F.softmax(logits, dim=1).detach().cpu().numpy()
             train_micro, train_macro, train_weighted, train_ece = metrics_from_predictions(labels, preds, probs, num_classes)
             # Tensorboard
-            writer.add_scalar('Accuracy/train', train_micro, step+len(tr_loader)*epoch)
-            writer.add_scalar('Macro F1/train', train_macro, step+len(tr_loader)*epoch)
-            writer.add_scalar('Weighted F1/train', train_weighted, step+len(tr_loader)*epoch)
-            writer.add_scalar('ECE/train', train_ece, step+len(tr_loader)*epoch)
+            writer.add_scalar('Accuracy/train', train_micro, step + len(tr_loader) * epoch)
+            writer.add_scalar('Macro F1/train', train_macro, step + len(tr_loader) * epoch)
+            writer.add_scalar('Weighted F1/train', train_weighted, step + len(tr_loader) * epoch)
+            writer.add_scalar('ECE/train', train_ece, step + len(tr_loader) * epoch)
+
 
 def train(
         save_dir: str,
         save_weights: bool,
-        tr_loader: GraphDataLoader, 
-        val_loader: GraphDataLoader, 
+        tr_loader: GraphDataLoader,
+        val_loader: GraphDataLoader,
         model: nn.Module,
         optimizer: Optimizer,
         writer: SummaryWriter,
         n_early: int,
         device: Optional[str] = 'cpu',
         check_iters: Optional[int] = -1,
-        conf: Optional[Dict[str,Any]] = None,
+        conf: Optional[Dict[str, Any]] = None,
         normalizers: Optional[Tuple[Normalizer]] = None,
         num_classes: Optional[int] = 2,
         ) -> None:
     """
     Train the model with early stopping on F1 score (weighted) or until 1000 iterations.
     """
     model = model.to(device)
@@ -188,26 +190,26 @@
             early_stop_rounds = 0
             if save_weights:
                 save_model(save_dir, model, conf, normalizers, prefix='best_')
         elif early_stop_rounds < n_early:
             early_stop_rounds += 1
         else:
             return
-        
+
 
 def load_dataset(
         train_node_dir: str,
         val_node_dir: str,
         test_node_dir: str,
         bsize: int,
         remove_prior: Optional[bool] = False,
         remove_morph: Optional[bool] = False,
         ) -> Tuple[GraphDataLoader, GraphDataLoader, GraphDataLoader]:
     """
-    Creates Torch dataloaders for training. 
+    Creates Torch dataloaders for training.
     Folder structure:
     node_dir:
      - train
       - graphs
        - file1.nodes.csv
        ...
      - validation
@@ -229,27 +231,28 @@
     val_dataloader = GraphDataLoader(val_dataset, batch_size=1, shuffle=False)
     test_dataset = GraphDataset(
         node_dir=test_node_dir, remove_morph=remove_morph, remove_prior=remove_prior,
         max_dist=200, max_degree=10, normalizers=train_dataset.get_normalizers())
     test_dataloader = GraphDataLoader(test_dataset, batch_size=1, shuffle=False)
     return train_dataloader, val_dataloader, test_dataloader
 
+
 def generate_configurations(max_confs: int, model_name: str) -> List[Dict[str, int]]:
     """
     Generates a grid in the search space with no more than max_confs configurations.
     Parameters changed: NUM_LAYERS, DROPOUT, NORM_TYPE
     """
     num_layers_confs = int(math.sqrt(max_confs / 2))
     num_dropout_confs = int(max_confs // (2 * num_layers_confs))
-    assert(2 * num_layers_confs * num_dropout_confs <= max_confs)
+    assert (2 * num_layers_confs * num_dropout_confs <= max_confs)
     assert num_layers_confs <= 15, 'Too many layers'
     confs = []
-    for num_layers in np.linspace(1,15, num_layers_confs):
+    for num_layers in np.linspace(1, 15, num_layers_confs):
         num_layers = int(num_layers)
-        for dropout in np.linspace(0,0.9, num_dropout_confs):
+        for dropout in np.linspace(0, 0.9, num_dropout_confs):
             conf = {}
             conf['MODEL_NAME'] = model_name
             conf['NUM_LAYERS'] = num_layers
             conf['DROPOUT'] = dropout
             conf['NORM_TYPE'] = 'bn'
             confs.append(conf)
 
@@ -257,15 +260,16 @@
             conf['MODEL_NAME'] = model_name
             conf['NUM_LAYERS'] = num_layers
             conf['DROPOUT'] = dropout
             conf['NORM_TYPE'] = None
             confs.append(conf)
     return confs
 
-def load_model(conf: Dict[str,Any], num_classes: int, num_feats: int) -> nn.Module:
+
+def load_model(conf: Dict[str, Any], num_classes: int, num_feats: int) -> nn.Module:
     """
     Available models: GCN, ATT, HATT, SAGE, BOOST
     Configuration space: NUM_LAYERS, DROPOUT, NORM_TYPE
     """
     hidden_feats = 100
     if conf['MODEL_NAME'] == 'GCN':
         return GCN(num_feats, hidden_feats, num_classes, conf['NUM_LAYERS'], conf['DROPOUT'], conf['NORM_TYPE'])
@@ -274,45 +278,52 @@
         num_out_heads = 1
         heads = ([num_heads] * conf['NUM_LAYERS']) + [num_out_heads]
         if conf['MODEL_NAME'] == 'ATT':
             return GAT(num_feats, hidden_feats, num_classes, heads, conf['NUM_LAYERS'], conf['DROPOUT'], conf['NORM_TYPE'])
         return HardGAT(num_feats, hidden_feats, num_classes, heads, conf['NUM_LAYERS'], conf['DROPOUT'], conf['NORM_TYPE'])
     assert False, 'Model not implemented.'
 
+
 def create_results_file(filename: str, num_classes: int) -> None:
     """
     Creates header of .csv result file to append results.
     filename must not contain extension.
     """
     if num_classes == 2:
         with open(filename + '.csv', 'w') as f:
             print('F1 Score,Accuracy,ROC AUC,PERC ERR,ECE,NUM_LAYERS,DROPOUT,NORM_TYPE', file=f)
     else:
         with open(filename + '.csv', 'w') as f:
             print('Micro F1,Macro F1,Weighted F1,ECE,NUM_LAYERS,DROPOUT,NORM_TYPE', file=f)
 
+
 def append_results(
-    filename: str, f1: float, acc: float, auc: float, num_layers: int, dropout: float, bn_type: str, ece: float, perc_err: Optional[float] = None
-) -> None:
+        filename: str,
+        f1: float, acc: float, auc: float,
+        num_layers: int, dropout: float, bn_type: str,
+        ece: float, perc_err: Optional[float] = None
+        ) -> None:
     """
     Appends result to given filename.
     filename must not contain extension.
     """
     with open(filename + '.csv', 'a') as f:
         if perc_err is not None:
             print(f1, acc, auc, perc_err, ece, num_layers, dropout, bn_type, file=f, sep=',')
         else:
             print(f1, acc, auc, ece, num_layers, dropout, bn_type, file=f, sep=',')
 
+
 def name_from_conf(conf: Dict[str, Any]) -> str:
     """
     Generates a name from the configuration object.
     """
     return conf['MODEL_NAME'] + '_' + str(conf['NUM_LAYERS']) + '_' \
-        + str(conf['DROPOUT']) + '_' + str(conf['NORM_TYPE']) 
+        + str(conf['DROPOUT']) + '_' + str(conf['NORM_TYPE'])
+
 
 def save_model(
         save_dir: str,
         model: nn.Module,
         conf: Dict[str, Any],
         normalizers: Tuple[Normalizer],
         prefix: Optional[str] = ''
@@ -324,14 +335,15 @@
     state_dict = model.state_dict()
     torch.save(state_dict, os.path.join(save_dir, 'weights', name + '.pth'))
     with open(os.path.join(save_dir, 'confs', name + '.json'), 'w') as f:
         json.dump(conf, f)
     with open(os.path.join(save_dir, 'normalizers', name + '.pkl'), 'wb') as f:
         pickle.dump(normalizers, f)
 
+
 def train_one_conf(
         args: Namespace,
         conf: Dict[str, Any],
         train_dataloader: GraphDataLoader,
         val_dataloader: GraphDataLoader,
         test_dataloader: GraphDataLoader,
         log_dir: str,
@@ -382,17 +394,17 @@
                         help='Name to file where to save the results. Must not contain extension.')
     parser.add_argument('--num-confs', type=int, default=50,
                         help='Upper bound on the number of configurations to try.')
     parser.add_argument('--save-dir', type=str,
                         help='Folder to save models weights and confs.')
     parser.add_argument('--device', type=str, choices=['cpu', 'cuda'], default='cpu',
                         help='Device to execute. Either cpu or cuda. Default: cpu.')
-    parser.add_argument('--num-workers', type=int, default=1, 
+    parser.add_argument('--num-workers', type=int, default=1,
                         help='Number of processors to use. Default: 1.')
-    parser.add_argument('--checkpoint-iters', type=int, default=-1, 
+    parser.add_argument('--checkpoint-iters', type=int, default=-1,
                         help='Number of iterations at which to save model periodically while training. Set to -1 for no checkpointing. Default: -1.')
     parser.add_argument('--num-classes', type=int, default=2, help='Number of classes to consider for classification (background not included).')
     parser.add_argument('--disable-prior', action='store_true', help='If True, remove hovernet probabilities from node features.')
     parser.add_argument('--disable-morph-feats', action='store_true', help='If True, remove morphological features from node features.')
     return parser
 
 
@@ -460,8 +472,7 @@
                 save_model(save_dir, model, conf, train_dataloader.dataset.get_normalizers(), 'last_')
 
 
 def main():
     parser = _create_parser()
     args = parser.parse_args()
     main(args)
-
```

### Comparing `tumourkit-0.6.0/tumourkit/classification/train_xgboost.py` & `tumourkit-0.7.0/tumourkit/classification/train_xgboost.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 from sklearn.model_selection import StratifiedKFold
 import pandas as pd
 from concurrent.futures import ThreadPoolExecutor
 from ..utils.classification import metrics_from_predictions
 
 
 def train(
-        conf: Dict[str, Any], 
-        X_tr: np.ndarray, 
-        y_tr: np.ndarray, 
+        conf: Dict[str, Any],
+        X_tr: np.ndarray,
+        y_tr: np.ndarray,
         val_size: float,
         seed: int,
         num_classes: Optional[int] = 2
         ) -> XGBClassifier:
     X_tr, X_val, y_tr, y_val = train_test_split(
         X_tr, y_tr, test_size=val_size, stratify=y_tr, random_state=seed
     )
@@ -69,99 +69,109 @@
         X_tr, y_tr,
         eval_set=[(X_val, y_val)], verbose=False
     )
     return model
 
 
 def evaluate(
-        model: XGBClassifier, 
+        model: XGBClassifier,
         X_val: np.ndarray,
         y_val: np.ndarray,
         num_classes: Optional[int] = 2
         ) -> Tuple[float, float, float]:
     preds = model.predict(X_val)
     if num_classes == 2:
-        probs = model.predict_proba(X_val)[:,1]
+        probs = model.predict_proba(X_val)[:, 1]
         acc, f1, auc, perc_err, ece = metrics_from_predictions(y_val, preds, probs, 2)
         return f1, acc, auc, perc_err, ece
     else:
         probs = model.predict_proba(X_val)
         micro, macro, weighted, ece = metrics_from_predictions(y_val, preds, probs, num_classes)
         return micro, macro, weighted, ece
 
 
-def save(metrics: Dict[str,Tuple[float,float,float]], path: str) -> None:
+def save(metrics: Dict[str, Tuple[float, float, float]], path: str) -> None:
     metrics.to_csv(path, index=False)
 
 
 def cross_validate(args, conf, skf, X, y):
     if args.num_classes == 2:
         f1_mean, acc_mean, auc_mean, perc_err_mean, ece_mean = 0, 0, 0, 0, 0
     else:
         micro_mean, macro_mean, weighted_mean, ece_mean = 0, 0, 0, 0
     for train_index, val_index in skf.split(X, y):
         X_train, X_cval = X[train_index], X[val_index]
         y_train, y_cval = y[train_index], y[val_index]
-        ## Train
+        # Train
         model = train(conf, X_train, y_train, args.val_size, args.seed, args.num_classes)
-        ## Save metrics
+        # Save metrics
         val_metrics = evaluate(model, X_cval, y_cval, args.num_classes)
         if args.num_classes == 2:
             f1, acc, auc, perc_err, ece = val_metrics
-            f1_mean += f1; acc_mean += acc; auc_mean += auc
-            perc_err_mean += perc_err; ece_mean += ece
+            f1_mean += f1
+            acc_mean += acc
+            auc_mean += auc
+            perc_err_mean += perc_err
+            ece_mean += ece
         else:
             micro, macro, weighted, ece = val_metrics
-            micro_mean += micro; macro_mean += macro; weighted_mean += weighted
+            micro_mean += micro
+            macro_mean += macro
+            weighted_mean += weighted
             ece_mean += ece
     if args.num_classes == 2:
-        f1_mean /= args.cv_folds; acc_mean /= args.cv_folds; auc_mean /= args.cv_folds
-        perc_err_mean /= args.cv_folds; ece_mean /= args.cv_folds
+        f1_mean /= args.cv_folds
+        acc_mean /= args.cv_folds
+        auc_mean /= args.cv_folds
+        perc_err_mean /= args.cv_folds
+        ece_mean /= args.cv_folds
         tmp = pd.DataFrame(
-            [(*conf.values(), f1_mean, acc_mean, auc_mean, perc_err_mean, ece_mean)], 
+            [(*conf.values(), f1_mean, acc_mean, auc_mean, perc_err_mean, ece_mean)],
             columns=[
                 'n_estimators', 'learning_rate', 'max_depth', 'colsample_bytree',
                 'f1', 'accuracy', 'auc', 'perc_err', 'ece'
                 ]
         )
     else:
-        micro_mean /= args.cv_folds; macro_mean /= args.cv_folds; weighted_mean /= args.cv_folds
+        micro_mean /= args.cv_folds
+        macro_mean /= args.cv_folds
+        weighted_mean /= args.cv_folds
         ece_mean /= args.cv_folds
         tmp = pd.DataFrame(
-            [(*conf.values(), micro_mean, macro_mean, weighted_mean, ece_mean)], 
+            [(*conf.values(), micro_mean, macro_mean, weighted_mean, ece_mean)],
             columns=[
                 'n_estimators', 'learning_rate', 'max_depth', 'colsample_bytree',
                 'micro', 'macro', 'weighted', 'ece'
                 ]
         )
     return tmp
 
 
 def create_confs():
-    confs = [{'n_estimators': n, 'learning_rate': l, 'max_depth': d, 'colsample_bytree': c}
-            for n in [500] 
-            for l in [0.05, 0.005] 
-            for d in [8, 16] 
-            for c in [0, 0.5]]
+    confs = [{'n_estimators': n, 'learning_rate': lr, 'max_depth': d, 'colsample_bytree': c}
+             for n in [500]
+             for lr in [0.05, 0.005]
+             for d in [8, 16]
+             for c in [1, 0.5]]
     return confs
 
 
 def _create_parser():
     parser = argparse.ArgumentParser()
     parser.add_argument('--graph-dir', type=str, required=True,
                         help='Folder containing .graph.csv files.')
     parser.add_argument('--test-graph-dir', type=str, required=True,
                         help='Folder containing .graph.csv files to evaluate at the end.')
     parser.add_argument('--val-size', type=float, default=0.2,
                         help='Validation size used for early stopping. Default: 0.2')
     parser.add_argument('--seed', type=int, default=None,
                         help='Seed for random split. Default: None')
-    parser.add_argument('--num-workers', type=int, default=1, 
+    parser.add_argument('--num-workers', type=int, default=1,
                         help='Number of processors to use. Default: 1.')
-    parser.add_argument('--cv-folds', type=int, default=10, 
+    parser.add_argument('--cv-folds', type=int, default=10,
                         help='Number of CV folds. Default: 10.')
     parser.add_argument('--save-name', type=str, required=True,
                         help='Name to save the result, without file type.')
     parser.add_argument('--num-classes', type=int, default=2,
                         help='Number of classes to consider for classification (background not included).')
     return parser
 
@@ -170,23 +180,23 @@
     X, y = read_all_nodes(args.graph_dir)
     y = np.array(y, dtype=np.int32)
     skf = StratifiedKFold(n_splits=args.cv_folds)
     skf.get_n_splits(X, y)
 
     if args.num_classes == 2:
         metrics = pd.DataFrame(
-            {}, 
+            {},
             columns=[
                 'n_estimators', 'learning_rate', 'max_depth', 'colsample_bytree',
                 'f1', 'accuracy', 'auc', 'perc_err', 'ece'
             ]
         )
     else:
         metrics = pd.DataFrame(
-            {}, 
+            {},
             columns=[
                 'n_estimators', 'learning_rate', 'max_depth', 'colsample_bytree',
                 'micro', 'macro', 'weighted', 'ece'
             ]
         )
     confs = create_confs()
     logger.info('Training various XGBoost configurations')
@@ -225,24 +235,24 @@
     logger.info('Computing test metrics.')
     X_test, y_test = read_all_nodes(args.test_graph_dir)
     y_test = np.array(y_test, dtype=np.int32)
     test_metrics = evaluate(model, X_test, y_test, args.num_classes)
     if args.num_classes == 2:
         f1, acc, auc, perc_err, ece = test_metrics
         test_metrics = pd.DataFrame(
-            [(*best_conf.values(), f1, acc, auc, perc_err, ece)], 
+            [(*best_conf.values(), f1, acc, auc, perc_err, ece)],
             columns=[
                 'n_estimators', 'learning_rate', 'max_depth', 'colsample_bytree',
                 'f1', 'accuracy', 'auc', 'perc_err', 'ece'
                 ]
         )
     else:
         micro, macro, weighted, ece = test_metrics
         test_metrics = pd.DataFrame(
-            [(*best_conf.values(), micro, macro, weighted, ece)], 
+            [(*best_conf.values(), micro, macro, weighted, ece)],
             columns=[
                 'n_estimators', 'learning_rate', 'max_depth', 'colsample_bytree',
                 'micro', 'macro', 'weighted', 'ece'
                 ]
         )
     save(test_metrics, args.save_name + '_test.csv')
 
@@ -256,9 +266,7 @@
     ch = logging.StreamHandler()
     ch.setLevel(logging.DEBUG)
     formatter = logging.Formatter('%(name)s - %(levelname)s - %(message)s')
     ch.setFormatter(formatter)
     logger.addHandler(ch)
 
     main_with_args(args, logger)
-    
-
```

### Comparing `tumourkit-0.6.0/tumourkit/demo/app.py` & `tumourkit-0.7.0/tumourkit/demo/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         download_file(url, filename)
     if not os.path.exists(os.path.join(weights_dir, hov_dataset, 'type_info.json')):
         os.makedirs(os.path.join(weights_dir, hov_dataset), exist_ok=True)
         url = f'https://huggingface.co/Jerry-Master/Hovernet-plus-Graphs/resolve/main/{hov_dataset}/hovernet/type_info.json'
         filename = os.path.join(weights_dir, hov_dataset, 'type_info.json')
         download_file(url, filename)
     if not os.path.exists(os.path.join(weights_dir, hov_dataset, gnn_model)) \
-        or len(os.listdir(os.path.join(weights_dir, hov_dataset, gnn_model))) < 3:
+       or len(os.listdir(os.path.join(weights_dir, hov_dataset, gnn_model))) < 3:
         os.makedirs(os.path.join(weights_dir, hov_dataset, gnn_model), exist_ok=True)
         url_folder = f'https://huggingface.co/Jerry-Master/Hovernet-plus-Graphs/tree/main/{hov_dataset}/gnn/{gnn_model}/'
         url_files = f'https://huggingface.co/Jerry-Master/Hovernet-plus-Graphs/resolve/main/{hov_dataset}/gnn/{gnn_model}/'
         dirname = os.path.join(weights_dir, hov_dataset, gnn_model)
         download_folder(url_folder, url_files, dirname)
 
 
@@ -105,79 +105,79 @@
         'mem_usage': '0.2'
     }
     hov_infer(newargs, newsubargs, 'tile')
 
 
 def run_posthov(num_classes: int, logger: Logger):
     newargs = Namespace(
-        json_dir = os.path.join(APP_DIR, 'tmp', 'tmp_hov', 'json'),
-        gson_dir = os.path.join(APP_DIR, 'tmp', 'gson_hov'),
-        num_classes = num_classes
+        json_dir=os.path.join(APP_DIR, 'tmp', 'tmp_hov', 'json'),
+        gson_dir=os.path.join(APP_DIR, 'tmp', 'gson_hov'),
+        num_classes=num_classes
     )
     hovernet2geojson(newargs)
     newargs = Namespace(
-        gson_dir = os.path.join(APP_DIR, 'tmp', 'gson_hov'),
-        png_dir = os.path.join(APP_DIR, 'tmp', 'png_hov'),
-        csv_dir = os.path.join(APP_DIR, 'tmp', 'csv_hov'),
-        num_classes = num_classes
+        gson_dir=os.path.join(APP_DIR, 'tmp', 'gson_hov'),
+        png_dir=os.path.join(APP_DIR, 'tmp', 'png_hov'),
+        csv_dir=os.path.join(APP_DIR, 'tmp', 'csv_hov'),
+        num_classes=num_classes
     )
     geojson2pngcsv(newargs)
     create_dir(os.path.join(APP_DIR, 'tmp', 'graphs'))
     newargs = Namespace(
-        png_dir = os.path.join(APP_DIR, 'tmp', 'png_hov'),
-        orig_dir = os.path.join(APP_DIR, 'tmp', 'input'),
-        output_path = os.path.join(APP_DIR, 'tmp', 'graphs', 'raw'),
-        num_workers = 0
+        png_dir=os.path.join(APP_DIR, 'tmp', 'png_hov'),
+        orig_dir=os.path.join(APP_DIR, 'tmp', 'input'),
+        output_path=os.path.join(APP_DIR, 'tmp', 'graphs', 'raw'),
+        num_workers=0
     )
     png2graph(newargs)
     newargs = Namespace(
-        json_dir = os.path.join(APP_DIR, 'tmp', 'tmp_hov', 'json'),
-        graph_dir = os.path.join(APP_DIR, 'tmp', 'graphs', 'raw'),
-        output_dir = os.path.join(APP_DIR, 'tmp', 'graphs', 'hovpreds'),
-        num_classes = num_classes
+        json_dir=os.path.join(APP_DIR, 'tmp', 'tmp_hov', 'json'),
+        graph_dir=os.path.join(APP_DIR, 'tmp', 'graphs', 'raw'),
+        output_dir=os.path.join(APP_DIR, 'tmp', 'graphs', 'hovpreds'),
+        num_classes=num_classes
     )
     join_hovprob_graph(newargs, logger)
 
 
 def run_graphs(gnn_dataset: str, gnn_model: str, num_classes: int, weights_dir: str):
     disable_prior = 'no-prior' in gnn_model or 'void' in gnn_model
     disable_morph_feats = 'no-morph' in gnn_model or 'void' in gnn_model
     model_name = os.listdir(os.path.join(weights_dir, gnn_dataset, gnn_model))[0]
     model_name, ext = os.path.splitext(model_name)
     newargs = Namespace(
-        node_dir = os.path.join(APP_DIR, 'tmp', 'graphs', 'hovpreds'),
-        output_dir = os.path.join(APP_DIR, 'tmp', 'gnn_preds'),
-        weights = os.path.join(weights_dir, gnn_dataset, gnn_model, model_name + '.pth'),
-        conf = os.path.join(weights_dir, gnn_dataset, gnn_model, model_name + '.json'),
-        normalizers = os.path.join(weights_dir, gnn_dataset, gnn_model, model_name + '.pkl'),
-        num_classes = num_classes,
-        disable_prior = disable_prior,
-        disable_morph_feats = disable_morph_feats,
+        node_dir=os.path.join(APP_DIR, 'tmp', 'graphs', 'hovpreds'),
+        output_dir=os.path.join(APP_DIR, 'tmp', 'gnn_preds'),
+        weights=os.path.join(weights_dir, gnn_dataset, gnn_model, model_name + '.pth'),
+        conf=os.path.join(weights_dir, gnn_dataset, gnn_model, model_name + '.json'),
+        normalizers=os.path.join(weights_dir, gnn_dataset, gnn_model, model_name + '.pkl'),
+        num_classes=num_classes,
+        disable_prior=disable_prior,
+        disable_morph_feats=disable_morph_feats,
     )
     infer_gnn(newargs)
 
 
 def run_postgraphs(num_classes: int):
     newargs = Namespace(
-        graph_dir = os.path.join(APP_DIR, 'tmp', 'gnn_preds'),
-        centroids_dir = os.path.join(APP_DIR, 'tmp', 'centroids'),
-        num_classes = num_classes,
+        graph_dir=os.path.join(APP_DIR, 'tmp', 'gnn_preds'),
+        centroids_dir=os.path.join(APP_DIR, 'tmp', 'centroids'),
+        num_classes=num_classes,
     )
     graph2centroids(newargs)
     newargs = Namespace(
-        centroids_dir = os.path.join(APP_DIR, 'tmp', 'centroids'),
-        png_dir = os.path.join(APP_DIR, 'tmp', 'png_hov'),
-        csv_dir = os.path.join(APP_DIR, 'tmp', 'csv_gnn'),
+        centroids_dir=os.path.join(APP_DIR, 'tmp', 'centroids'),
+        png_dir=os.path.join(APP_DIR, 'tmp', 'png_hov'),
+        csv_dir=os.path.join(APP_DIR, 'tmp', 'csv_gnn'),
     )
     centroidspng2csv(newargs)
     newargs = Namespace(
-        png_dir = os.path.join(APP_DIR, 'tmp', 'png_hov'),
-        csv_dir = os.path.join(APP_DIR, 'tmp', 'csv_gnn'),
-        gson_dir = os.path.join(APP_DIR, 'tmp', 'gson_gnn'),
-        num_classes = num_classes
+        png_dir=os.path.join(APP_DIR, 'tmp', 'png_hov'),
+        csv_dir=os.path.join(APP_DIR, 'tmp', 'csv_gnn'),
+        gson_dir=os.path.join(APP_DIR, 'tmp', 'gson_gnn'),
+        num_classes=num_classes
     )
     pngcsv2geojson(newargs)
 
 
 def create_logger():
     logger = logging.getLogger('gradio')
     logger.setLevel(logging.DEBUG)
@@ -190,64 +190,67 @@
 
 
 def overlay_outputs(hov_dataset: str, use_gnn: bool):
     """
     Returns the output images.
     """
     newargs = Namespace(
-        orig_dir = os.path.join(APP_DIR, 'tmp', 'input'),
-        png_dir = os.path.join(APP_DIR, 'tmp', 'png_hov'),
-        csv_dir = os.path.join(APP_DIR, 'tmp', 'csv_hov'),
-        output_dir = os.path.join(APP_DIR, 'tmp', 'overlay_hov'),
-        type_info = os.path.join(APP_DIR, 'weights', hov_dataset, 'type_info.json'),
+        orig_dir=os.path.join(APP_DIR, 'tmp', 'input'),
+        png_dir=os.path.join(APP_DIR, 'tmp', 'png_hov'),
+        csv_dir=os.path.join(APP_DIR, 'tmp', 'csv_hov'),
+        output_dir=os.path.join(APP_DIR, 'tmp', 'overlay_hov'),
+        type_info=os.path.join(APP_DIR, 'weights', hov_dataset, 'type_info.json'),
     )
     draw_cells(newargs)
     hov_dir = os.path.join(APP_DIR, 'tmp', 'overlay_hov')
     hov_file = os.listdir(hov_dir)[0]
     hov = cv2.imread(os.path.join(hov_dir, hov_file), -1)[:, :, ::-1]
     if use_gnn:
         newargs = Namespace(
-            orig_dir = os.path.join(APP_DIR, 'tmp', 'input'),
-            png_dir = os.path.join(APP_DIR, 'tmp', 'png_hov'),
-            csv_dir = os.path.join(APP_DIR, 'tmp', 'csv_gnn'),
-            output_dir = os.path.join(APP_DIR, 'tmp', 'overlay_gnn'),
-            type_info = os.path.join(APP_DIR, 'weights', hov_dataset, 'type_info.json'),
+            orig_dir=os.path.join(APP_DIR, 'tmp', 'input'),
+            png_dir=os.path.join(APP_DIR, 'tmp', 'png_hov'),
+            csv_dir=os.path.join(APP_DIR, 'tmp', 'csv_gnn'),
+            output_dir=os.path.join(APP_DIR, 'tmp', 'overlay_gnn'),
+            type_info=os.path.join(APP_DIR, 'weights', hov_dataset, 'type_info.json'),
         )
         draw_cells(newargs)
         gnn_dir = os.path.join(APP_DIR, 'tmp', 'overlay_gnn')
         gnn_file = os.listdir(gnn_dir)[0]
         gnn = cv2.imread(os.path.join(gnn_dir, gnn_file), -1)[:, :, ::-1]
     else:
         gnn = None
     return hov, gnn
 
 
 LAST_HOV_MODEL = None
 LAST_HOV_DATASET = None
 LAST_IMG_HASH = None
+
+
 def process_image(weights_dir: str, input_image: np.ndarray, hov_dataset: str, hov_model: str, gnn_model: str):
     # Cache information when possible
     global LAST_HOV_MODEL
     global LAST_IMG_HASH
+    global LAST_HOV_DATASET
     input_hash = hash(str(input_image))
     if LAST_IMG_HASH is None:
         LAST_IMG_HASH = input_hash
     if LAST_HOV_MODEL is None or LAST_IMG_HASH is None or LAST_HOV_DATASET is None \
-         or LAST_HOV_MODEL != hov_model or LAST_IMG_HASH != input_hash or LAST_HOV_DATASET != hov_dataset:
+       or LAST_HOV_MODEL != hov_model or LAST_IMG_HASH != input_hash or LAST_HOV_DATASET != hov_dataset:
         LAST_HOV_MODEL = hov_model
         LAST_IMG_HASH = input_hash
         LAST_HOV_DATASET = hov_dataset
         delete_prev = True
     else:
         delete_prev = False
 
     # Monusac doesn't have graph attention
     if hov_dataset == 'monusac' and gnn_model == 'gat-full':
         gnn_model = 'None'
-    
+
     if weights_dir is None:
         weights_dir = os.path.join(APP_DIR, 'weights')
     logger = create_logger()
     download_models_if_needed(hov_dataset, hov_model, gnn_model, weights_dir)
     with open(os.path.join(APP_DIR, 'weights', hov_dataset, 'type_info.json'), 'r') as f:
         type_info = json.load(f)
         num_classes = len(type_info.keys()) - 1
@@ -274,15 +277,17 @@
     gnn_model = gr.Dropdown(choices=[
         'gcn-full', 'gat-full',
         'gcn-no-morph', 'gcn-no-prior', 'gcn-void',
         'None'
         ], label='Select GNN model')
     out1 = gr.Image(label='Hovernet')
     out2 = gr.Image(label='GNN')
-    func = lambda a,b,c,d: process_image(weights_dir, a,b,c,d)
+
+    def func(a: np.ndarray, b: str, c: str, d: str):
+        process_image(weights_dir, a, b, c, d)
     ui = gr.Interface(
         fn=func,
         inputs=[image_input, hov_dataset, hov_model, gnn_model],
         outputs=[out1, out2],
         title="CNN+GNN Demo",
         description="Upload an image to see the output of the algorithm.",
         examples=[[os.path.join(APP_DIR, 'examples', x), 'breast', '518FT', 'gcn-full'] for x in os.listdir(os.path.join(APP_DIR, 'examples'))]
@@ -303,8 +308,8 @@
     parser = _create_parser()
     args = parser.parse_args()
     ui = create_ui(args.weights_dir)
     ui.launch(server_name=args.ip, server_port=args.port, share=args.share)
 
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `tumourkit-0.6.0/tumourkit/eval_pipe.py` & `tumourkit-0.7.0/tumourkit/eval_pipe.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,68 +1,88 @@
+"""
+Pipeline for evaluation of models.
+
+Copyright (C) 2023  Jose Pérez Cano
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU Affero General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU Affero General Public License for more details.
+
+You should have received a copy of the GNU Affero General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Contact information: joseperez2000@hotmail.es
+"""
 import argparse
 from argparse import Namespace
 import logging
 from logging import Logger
 import numpy as np
 import pandas as pd
 from . import eval_segment
 import os
 from .preprocessing import hovernet2centroids, geojson2pngcsv, pngcsv2centroids
 from .utils.preprocessing import get_names
 from .utils.pipes import HovernetNotFoundError, check_void
 from .utils.classification import metrics_from_predictions
 
 
-def run_preprocessing(args: Namespace, logger : Logger) -> None:
+def run_preprocessing(args: Namespace, logger: Logger) -> None:
     """
     Converts the gson format to the rest of formats.
     """
     logger.info('Extracting Hovernet centroids from training output.')
     if not os.path.isdir(os.path.join(args.root_dir, 'data', 'tmp_hov', 'json')):
         raise HovernetNotFoundError('Please, train again or extract hovernet outputs.')
     newargs = Namespace(
-        json_dir = os.path.join(args.root_dir, 'data', 'tmp_hov', 'json'),
-        output_path = os.path.join(args.root_dir, 'data', 'tmp_hov', 'centroids_hov'),
+        json_dir=os.path.join(args.root_dir, 'data', 'tmp_hov', 'json'),
+        output_path=os.path.join(args.root_dir, 'data', 'tmp_hov', 'centroids_hov'),
     )
     hovernet2centroids(newargs)
     for split in ['train', 'validation', 'test']:
         if check_void(os.path.join(args.root_dir, 'data', split, 'names.txt')):
             logger.info(f'Preprocessing split {split}.')
             split_names = get_names(os.path.join(args.root_dir, 'data', split, 'gson'), '.geojson')
             with open(os.path.join(args.root_dir, 'data', split, 'names.txt'), 'w') as f:
                 for name in split_names:
                     print(name, file=f)
         if check_void(os.path.join(args.root_dir, 'data', split, 'png')) or check_void(os.path.join(args.root_dir, 'data', split, 'csv')):
             logger.info('   From geojson to pngcsv.')
             newargs = Namespace(
-                gson_dir = os.path.join(args.root_dir, 'data', split, 'gson'),
-                png_dir = os.path.join(args.root_dir, 'data', split, 'png'),
-                csv_dir = os.path.join(args.root_dir, 'data', split, 'csv'),
-                num_classes = args.num_classes,
+                gson_dir=os.path.join(args.root_dir, 'data', split, 'gson'),
+                png_dir=os.path.join(args.root_dir, 'data', split, 'png'),
+                csv_dir=os.path.join(args.root_dir, 'data', split, 'csv'),
+                num_classes=args.num_classes,
             )
             geojson2pngcsv(newargs)
         if check_void(os.path.join(args.root_dir, 'data', split, 'centroids')):
             logger.info('   Extracting centroids from GT.')
             newargs = Namespace(
-                png_dir = os.path.join(args.root_dir, 'data', split, 'png'),
-                csv_dir = os.path.join(args.root_dir, 'data', split, 'csv'),
-                output_path = os.path.join(args.root_dir, 'data', split, 'centroids')
+                png_dir=os.path.join(args.root_dir, 'data', split, 'png'),
+                csv_dir=os.path.join(args.root_dir, 'data', split, 'csv'),
+                output_path=os.path.join(args.root_dir, 'data', split, 'centroids')
             )
             pngcsv2centroids(newargs)
     return
 
 
 def compute_ece(args: Namespace, logger: Logger, split: str) -> None:
     folder = os.path.join(args.root_dir, 'data', split, 'graphs', 'preds')
     trues, probs = None, None
     for file in os.listdir(folder):
         df = pd.read_csv(os.path.join(folder, file))
-        _trues = df['class'].to_numpy()-1
+        _trues = df['class'].to_numpy() - 1
         if trues is None:
-            trues = _trues.reshape((-1,1))
+            trues = _trues.reshape((-1, 1))
         else:
             trues = np.vstack((trues, _trues.reshape((-1, 1))))
         if args.num_classes == 2:
             _probs = df['prob1'].to_numpy().reshape((-1, 1))
             _probs = np.hstack((1 - _probs, _probs))
         else:
             cols = ['prob' + str(k) for k in range(1, args.num_classes + 1)]
@@ -88,20 +108,20 @@
 
 
 def run_evaluation(args: Namespace, logger: Logger) -> None:
     logger.info('Starting evaluation of Hovernet output.')
     for split in ['train', 'validation', 'test']:
         logger.info(f'    Evaluating {split} split')
         newargs = Namespace(
-            names = os.path.join(args.root_dir, 'data', split, 'names.txt'),
-            gt_path = os.path.join(args.root_dir, 'data', split, 'centroids'),
-            pred_path = os.path.join(args.root_dir, 'data', 'tmp_hov', 'centroids_hov'),
-            save_name = args.save_name + '_' + split,
-            debug_path = None,
-            num_classes = args.num_classes
+            names=os.path.join(args.root_dir, 'data', split, 'names.txt'),
+            gt_path=os.path.join(args.root_dir, 'data', split, 'centroids'),
+            pred_path=os.path.join(args.root_dir, 'data', 'tmp_hov', 'centroids_hov'),
+            save_name=args.save_name + '_' + split,
+            debug_path=None,
+            num_classes=args.num_classes
         )
         eval_segment(newargs, logger)
 
         compute_ece(args, logger, split)
     return
 
 
@@ -122,8 +142,8 @@
     ch = logging.StreamHandler()
     ch.setLevel(logging.DEBUG)
     formatter = logging.Formatter('%(name)s - %(levelname)s - %(message)s')
     ch.setFormatter(formatter)
     logger.addHandler(ch)
 
     run_preprocessing(args, logger)
-    run_evaluation(args, logger)
+    run_evaluation(args, logger)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tumourkit-0.6.0/tumourkit/infer_pipe.py` & `tumourkit-0.7.0/tumourkit/infer_pipe.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+"""
+Pipeline for inference.
+
+Copyright (C) 2023  Jose Pérez Cano
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU Affero General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU Affero General Public License for more details.
+
+You should have received a copy of the GNU Affero General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Contact information: joseperez2000@hotmail.es
+"""
 import argparse
 from argparse import Namespace
 import logging
 from logging import Logger
 from .segmentation import hov_infer
 import os
 from .preprocessing import geojson2pngcsv, png2graph, hovernet2geojson, graph2centroids, centroidspng2csv, pngcsv2geojson
@@ -53,90 +73,90 @@
         'mem_usage': '0.2'
     }
     hov_infer(newargs, newsubargs, 'tile')
     return
 
 
 def run_posthov(args: Namespace, logger: Logger) -> None:
-    logger.info(f'Parsing Hovernet output')
+    logger.info('Parsing Hovernet output')
     logger.info('   From json to geojson.')
     newargs = Namespace(
-        json_dir = os.path.join(args.output_dir, 'tmp_hov', 'json'),
-        gson_dir = os.path.join(args.output_dir, 'gson_hov'),
-        num_classes = args.num_classes
+        json_dir=os.path.join(args.output_dir, 'tmp_hov', 'json'),
+        gson_dir=os.path.join(args.output_dir, 'gson_hov'),
+        num_classes=args.num_classes
     )
     hovernet2geojson(newargs)
     logger.info('   From geojson to pngcsv.')
     newargs = Namespace(
-        gson_dir = os.path.join(args.output_dir, 'gson_hov'),
-        png_dir = os.path.join(args.output_dir, 'png_hov'),
-        csv_dir = os.path.join(args.output_dir, 'csv_hov'),
-        num_classes = args.num_classes
+        gson_dir=os.path.join(args.output_dir, 'gson_hov'),
+        png_dir=os.path.join(args.output_dir, 'png_hov'),
+        csv_dir=os.path.join(args.output_dir, 'csv_hov'),
+        num_classes=args.num_classes
     )
     geojson2pngcsv(newargs)
     logger.info('   From pngcsv to nodes.csv.')
     create_dir(os.path.join(args.output_dir, 'graphs'))
     newargs = Namespace(
-        png_dir = os.path.join(args.output_dir, 'png_hov'),
-        orig_dir = args.input_dir,
-        output_path = os.path.join(args.output_dir, 'graphs', 'raw'),
-        num_workers = args.num_workers
+        png_dir=os.path.join(args.output_dir, 'png_hov'),
+        orig_dir=args.input_dir,
+        output_path=os.path.join(args.output_dir, 'graphs', 'raw'),
+        num_workers=args.num_workers
     )
     png2graph(newargs)
     logger.info('   Adding hovernet predictions to .nodes.csv.')
     newargs = Namespace(
-        json_dir = os.path.join(args.output_dir, 'tmp_hov', 'json'),
-        graph_dir = os.path.join(args.output_dir, 'graphs', 'raw'),
-        output_dir = os.path.join(args.output_dir, 'graphs', 'hovpreds'),
-        num_classes = args.num_classes
+        json_dir=os.path.join(args.output_dir, 'tmp_hov', 'json'),
+        graph_dir=os.path.join(args.output_dir, 'graphs', 'raw'),
+        output_dir=os.path.join(args.output_dir, 'graphs', 'hovpreds'),
+        num_classes=args.num_classes
     )
     join_hovprob_graph(newargs, logger)
     return
 
 
 def run_graphs(args: Namespace, logger: Logger) -> None:
     logger.info('Starting graph inference.')
     model_name = 'best_' + args.best_arch + '_' + args.best_num_layers + '_' \
         + args.best_dropout + '_' + args.best_norm_type
     newargs = Namespace(
-        node_dir = os.path.join(args.output_dir, 'graphs', 'hovpreds'),
-        output_dir = os.path.join(args.output_dir, 'gnn_preds'),
-        weights = os.path.join(args.root_dir, 'weights', 'classification', 'gnn', 'weights', model_name + '.pth'),
-        conf = os.path.join(args.root_dir, 'weights', 'classification', 'gnn', 'confs', model_name + '.json'),
-        normalizers = os.path.join(args.root_dir, 'weights', 'classification', 'gnn', 'normalizers', model_name + '.pkl'),
-        num_classes = args.num_classes,
-        disable_prior = False,
-        disable_morph_feats = False,
+        node_dir=os.path.join(args.output_dir, 'graphs', 'hovpreds'),
+        output_dir=os.path.join(args.output_dir, 'gnn_preds'),
+        weights=os.path.join(args.root_dir, 'weights', 'classification', 'gnn', 'weights', model_name + '.pth'),
+        conf=os.path.join(args.root_dir, 'weights', 'classification', 'gnn', 'confs', model_name + '.json'),
+        normalizers=os.path.join(args.root_dir, 'weights', 'classification', 'gnn', 'normalizers', model_name + '.pkl'),
+        num_classes=args.num_classes,
+        disable_prior=False,
+        disable_morph_feats=False,
     )
     infer_gnn(newargs)
     return
 
 
 def run_postgraphs(args: Namespace, logger: Logger) -> None:
     logger.info('Parsing gnn output.')
     logger.info('   Converting .nodes.csv to .centroids.csv.')
     newargs = Namespace(
-        graph_dir = os.path.join(args.output_dir, 'gnn_preds'),
-        centroids_dir = os.path.join(args.output_dir, 'centroids'),
-        num_classes = args.num_classes,
+        graph_dir=os.path.join(args.output_dir, 'gnn_preds'),
+        centroids_dir=os.path.join(args.output_dir, 'centroids'),
+        num_classes=args.num_classes,
     )
     graph2centroids(newargs)
     logger.info('   Converting .centroids.csv and .GT_cells.png to .class.csv.')
     newargs = Namespace(
-        centroids_dir = os.path.join(args.output_dir, 'centroids'),
-        png_dir = os.path.join(args.output_dir, 'png_hov'),
-        csv_dir = os.path.join(args.output_dir, 'csv_gnn'),
+        centroids_dir=os.path.join(args.output_dir, 'centroids'),
+        png_dir=os.path.join(args.output_dir, 'png_hov'),
+        csv_dir=os.path.join(args.output_dir, 'csv_gnn'),
     )
     centroidspng2csv(newargs)
     logger.info('   Converting png/csv to geojson.')
     newargs = Namespace(
-        png_dir = os.path.join(args.output_dir, 'png_hov'),
-        csv_dir = os.path.join(args.output_dir, 'csv_gnn'),
-        gson_dir = os.path.join(args.output_dir, 'gson_gnn'),
-        num_classes = args.num_classes
+        png_dir=os.path.join(args.output_dir, 'png_hov'),
+        csv_dir=os.path.join(args.output_dir, 'csv_gnn'),
+        gson_dir=os.path.join(args.output_dir, 'gson_gnn'),
+        num_classes=args.num_classes
     )
     pngcsv2geojson(newargs)
     return
 
 
 def _create_parser():
     parser = argparse.ArgumentParser()
@@ -167,8 +187,8 @@
     logger.addHandler(ch)
 
     if args.best_num_layers is None or args.best_dropout is None or args.best_norm_type is None:
         set_best_configuration(args, logger)
     run_hovernet(args, logger)
     run_posthov(args, logger)
     run_graphs(args, logger)
-    run_postgraphs(args, logger)
+    run_postgraphs(args, logger)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tumourkit-0.6.0/tumourkit/postprocessing/draw_cells.py` & `tumourkit-0.7.0/tumourkit/postprocessing/draw_cells.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 from typing import Dict, Tuple, List
 from ..utils.preprocessing import get_names, read_labels
 
 
 def draw_cells(orig: np.ndarray, png: np.ndarray, csv: pd.DataFrame, type_info: Dict[str, Tuple[str, List[int]]]) -> np.ndarray:
     blend = orig.copy()
     for i, (idx, cell_label) in csv.iterrows():
-        blend[png==idx] = 0.3 * np.array(type_info[str(cell_label)][1]) \
-                       + 0.7 * blend[png==idx]
+        blend[png == idx] = 0.3 * np.array(type_info[str(cell_label)][1]) \
+            + 0.7 * blend[png == idx]
     return blend
 
 
 def _create_parser():
     parser = argparse.ArgumentParser()
     parser.add_argument('--orig-dir', type=str, help='Path to base images folder. Must be in .png format.')
     parser.add_argument('--png-dir', type=str, help='Path to folder with png of the labels.')
@@ -49,21 +49,21 @@
     parser.add_argument('--type-info', type=str, help='Path to type_info.json.')
     return parser
 
 
 def main_with_args(args: Namespace) -> None:
     os.makedirs(args.output_dir, exist_ok=True)
     names = get_names(args.orig_dir, '.png')
+    with open(args.type_info, 'r') as f:
+            type_info = json.load(f)
     for name in tqdm(names):
         orig = cv2.imread(os.path.join(args.orig_dir, name + '.png'), cv2.IMREAD_COLOR)[:, :, ::-1]
         png, csv = read_labels(name, args.png_dir, args.csv_dir)
-        with open(args.type_info, 'r') as f:
-            type_info = json.load(f)
         out = draw_cells(orig, png, csv, type_info)
         cv2.imwrite(os.path.join(args.output_dir, name + '.overlay.png'), out[:, :, ::-1])
     return
 
 
 def main():
     parser = _create_parser()
     args = parser.parse_args()
-    main_with_args(args)
+    main_with_args(args)
```

### Comparing `tumourkit-0.6.0/tumourkit/postprocessing/join_graph_gt.py` & `tumourkit-0.7.0/tumourkit/postprocessing/join_graph_gt.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,31 +33,31 @@
     """
     Finds 1-1 matchings of nodes and substitutes labels in graph
     by those in centroids. Internally uses KD-trees.
     """
     assert len(centroids) > 0, 'GT must contain at least one cell.'
     graph = graph.copy()
     graph['prob1'] = graph['class'] - 1
-    gt_tree = generate_tree(centroids[:,:2])
+    gt_tree = generate_tree(centroids[:, :2])
     pred_centroids = graph[['X', 'Y']].to_numpy(dtype=int)
     pred_tree = generate_tree(pred_centroids)
     for point_id, point in enumerate(centroids):
         if point[2] == -1:
             continue
         closest_id = find_nearest(point[:2], pred_tree)
         closest = graph.loc[closest_id, ['X', 'Y', 'class']]
         if closest[2] == -1:
             continue
         if point_id == find_nearest(closest[:2], gt_tree):
-            graph.loc[closest_id, 'class'] = point[2] # 1-1 matchings
+            graph.loc[closest_id, 'class'] = point[2]  # 1-1 matchings
     for point_id, point in enumerate(pred_centroids):
         closest_id = find_nearest(point[:2], gt_tree)
         closest = centroids[closest_id]
         if point_id != find_nearest(closest[:2], pred_tree):
-            graph.drop(point_id, inplace=True) # Remove prediction not matched in GT
+            graph.drop(point_id, inplace=True)  # Remove prediction not matched in GT
     return graph
 
 
 def _create_parser():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         '--graph-dir', type=str, required=True,
@@ -90,8 +90,8 @@
             continue
     return
 
 
 def main():
     parser = _create_parser()
     args = parser.parse_args()
-    main_with_args(args)
+    main_with_args(args)
```

### Comparing `tumourkit-0.6.0/tumourkit/postprocessing/join_hovprob_graph.py` & `tumourkit-0.7.0/tumourkit/postprocessing/join_hovprob_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import os
 from ..utils.preprocessing import create_dir, parse_path, get_names, read_json, save_graph
 from ..utils.nearest import generate_tree, find_nearest
 import logging
 from logging import Logger
 
 
-def parse_centroids_probs(nuc: Dict[str, Any], logger: Optional[Logger] = None, num_classes: Optional[int] = 2) -> List[Tuple[int,int,int]]:
+def parse_centroids_probs(nuc: Dict[str, Any], logger: Optional[Logger] = None, num_classes: Optional[int] = 2) -> List[Tuple[int, int, int]]:
     """
     Input: Hovernet json nuclei dictionary as given by modified run_infer.py.
     Output: List of (X,Y,prob1) tuples representing centroids.
     """
     centroids_ = []
     for inst in nuc:
         inst_info = nuc[inst]
@@ -50,52 +50,52 @@
         if inst_type == 0:
             if logger is None:
                 logging.warning('Found cell with class 0, removing it.')
             else:
                 logger.warning('Found cell with class 0, removing it.')
         else:
             if num_classes == 2:
-                centroids_.append((inst_centroid[1], inst_centroid[0], inst_prob1)) 
+                centroids_.append((inst_centroid[1], inst_centroid[0], inst_prob1))
             else:
-                centroids_.append((inst_centroid[1], inst_centroid[0], *inst_probs)) 
+                centroids_.append((inst_centroid[1], inst_centroid[0], *inst_probs))
     return centroids_
 
 
 def add_probability(graph: pd.DataFrame, hov_json: Dict[str, Any], logger: Optional[Logger] = None, num_classes: Optional[int] = 2) -> pd.DataFrame:
     """
     Extracts type_prob from json and adds it as column prob1.
     Makes the join based on id.
     """
     centroids = parse_centroids_probs(hov_json, logger, num_classes)
     centroids = np.array(centroids)
     assert len(centroids) > 0, 'Hov json must contain at least one cell.'
     graph = graph.copy()
-    if not 'prob1' in graph.columns:
+    if 'prob1' not in graph.columns:
         n_cols = len(graph.columns)
         graph.insert(n_cols, 'prob1', [-1] * len(graph))
     else:
         graph['prob1'] = -1
     if num_classes > 2:
         for k in range(2, num_classes + 1):
             if not 'prob' + str(k) in graph.columns:
                 n_cols = len(graph.columns)
                 graph.insert(n_cols, 'prob' + str(k), [-1] * len(graph))
             else:
                 graph['prob' + str(k)] = -1
-    gt_tree = generate_tree(centroids[:,:2])
+    gt_tree = generate_tree(centroids[:, :2])
     pred_centroids = graph[['X', 'Y']].to_numpy(dtype=int)
     pred_tree = generate_tree(pred_centroids)
     for point_id, point in enumerate(centroids):
         closest_id = find_nearest(point[:2], pred_tree)
         closest = graph.loc[closest_id, ['X', 'Y', 'prob1']]
         if point_id == find_nearest(closest[:2], gt_tree):
-            graph.loc[closest_id, 'prob1'] = point[2] # 1-1 matchings
+            graph.loc[closest_id, 'prob1'] = point[2]  # 1-1 matchings
             if num_classes > 2:
                 for k in range(2, num_classes + 1):
-                    graph.loc[closest_id, 'prob' + str(k)] = point[k + 1] # 1-1 matchings
+                    graph.loc[closest_id, 'prob' + str(k)] = point[k + 1]  # 1-1 matchings
     graph.drop(graph[graph['prob1'] == -1].index, inplace=True)
     return graph
 
 
 def _create_parser():
     parser = argparse.ArgumentParser()
     parser.add_argument(
```

### Comparing `tumourkit-0.6.0/tumourkit/postprocessing/merge_cells.py` & `tumourkit-0.7.0/tumourkit/postprocessing/merge_cells.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Merge broken cells using a morphological algorithm 
+Merge broken cells using a morphological algorithm
 to detect touching frontiers.
 
 Copyright (C) 2023  Jose Pérez Cano
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU Affero General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
@@ -29,78 +29,83 @@
 )
 import argparse
 from tqdm import tqdm
 
 
 MAX_CELLS = 1500
 
-def create_id_map() -> Tuple[Callable[[np.ndarray], np.ndarray], Dict[int, Tuple[int,int]]]:
+
+def create_id_map() -> Tuple[Callable[[np.ndarray], np.ndarray], Dict[int, Tuple[int, int]]]:
     """
     Map index to some function so that difference is unique per pair.
-    Also returns the inverse mapping of the differences and the 
+    Also returns the inverse mapping of the differences and the
     inverse mapping of the function itself.
     Extra information: https://math.stackexchange.com/questions/4565014/injectivity-of-given-integer-function/4567383#4567383
     """
-    f = lambda x: x**5
+    def f(x: int) -> int:
+        return x**5
     sq_dif = []
     inv_diff_mapping = {}
     for i in range(MAX_CELLS):
-        for j in range(i+1,MAX_CELLS):
-            sq_dif.append(f(j)-f(i))
-            inv_diff_mapping[f(j)-f(i)] = [j,i]
-    assert (len(sq_dif) - len(set(sq_dif)))==0, 'Defined function is not injective.'
+        for j in range(i + 1, MAX_CELLS):
+            sq_dif.append(f(j) - f(i))
+            inv_diff_mapping[f(j) - f(i)] = [j, i]
+    assert (len(sq_dif) - len(set(sq_dif))) == 0, 'Defined function is not injective.'
 
     vec_mapping = np.vectorize(f)
     return vec_mapping, inv_diff_mapping
 
+
 def get_gradient(png: np.ndarray) -> np.ndarray:
     """
     Apply a dilation, subtract the image and remove pixels in background.
     """
     mask = png.copy()
-    mask[mask>0] = 1
-    dilation = skimage.morphology.dilation(png, np.ones((3,3)))
+    mask[mask > 0] = 1
+    dilation = skimage.morphology.dilation(png, np.ones((3, 3)))
     grad = dilation - png
     grad_bkgr = grad * mask
     return grad_bkgr
 
+
 def merge_cells(
-    png: np.ndarray, 
-    vec_mapping: Callable[[np.ndarray], np.ndarray], 
-    inv_diff_mapping: Dict[int, Tuple[int,int]]
-    ) -> np.ndarray:
+        png: np.ndarray,
+        vec_mapping: Callable[[np.ndarray], np.ndarray],
+        inv_diff_mapping: Dict[int, Tuple[int, int]]
+        ) -> np.ndarray:
     """
     Merges all the cells that share a frontier of more than 13 pixels.
     """
     png_cp = png.copy()
-    png_cp = vec_mapping(png_cp) # Indices mapping
-    grad_bkgr = get_gradient(png_cp) # Morphological gradient
+    png_cp = vec_mapping(png_cp)  # Indices mapping
+    grad_bkgr = get_gradient(png_cp)  # Morphological gradient
     # Select pairs with long frontier
     unique, counts = np.unique(grad_bkgr, return_counts=True)
     component = [-1 for _ in range(MAX_CELLS)]
     for el, freq in zip(unique, counts):
-        if el > 0 and freq > 13: # More than 13 points in frontier
+        if el > 0 and freq > 13:  # More than 13 points in frontier
             pair = inv_diff_mapping[el]
             # Get component of each index
             if component[pair[0]] != -1:
                 pair[0] = component[pair[0]]
             if component[pair[1]] != -1:
                 pair[1] = component[pair[1]]
-            M = min(*pair) # Merge operation is to set both indices to the minimum
+            M = min(*pair)  # Merge operation is to set both indices to the minimum
             # Update component of each index
             for k, el in enumerate(component):
                 if el == pair[0] or el == pair[1]:
                     component[k] = M
             component[pair[0]] = M
             component[pair[1]] = M
             # Map indices to new component
-            png[png==pair[0]] = M
-            png[png==pair[1]] = M
+            png[png == pair[0]] = M
+            png[png == pair[1]] = M
     return png
 
+
 def remove_lost_ids(png: np.ndarray, csv: pd.DataFrame) -> pd.DataFrame:
     """
     Removes identifiers in csv that are not in png.
     """
     next_ids = set(np.unique(png))
     curr_ids = set(csv.id)
     assert next_ids.difference(curr_ids) == set([0]), "Indices doesn't match"
@@ -134,12 +139,13 @@
     create_dir(png_out_path)
     create_dir(csv_out_path)
 
     names = get_names(png_dir, '.GT_cells.png')
     vec_mapping, inv_diff_mapping = create_id_map()
     for k, name in tqdm(enumerate(names)):
         png, csv = read_labels(name, png_dir, csv_dir)
-        if png is None or csv is None: continue
-        assert(np.max(csv.id) < MAX_CELLS), "Exceeded maximum number of cells."
+        if png is None or csv is None:
+            continue
+        assert (np.max(csv.id) < MAX_CELLS), "Exceeded maximum number of cells."
         png = merge_cells(png, vec_mapping, inv_diff_mapping)
         csv = remove_lost_ids(png, csv)
         save_pngcsv(png, csv, png_out_path, csv_out_path, name)
```

### Comparing `tumourkit-0.6.0/tumourkit/postprocessing/rswoosh.py` & `tumourkit-0.7.0/tumourkit/postprocessing/rswoosh.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,33 +14,35 @@
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Contact information: joseperez2000@hotmail.es
 """
 from typing import Callable, Tuple, List
 
-Point = Tuple[float,float]
+
+Point = Tuple[float, float]
 Contour = List[Point]
-Cell = Tuple[int, int, Contour] # id, class
+Cell = Tuple[int, int, Contour]  # id, class
+
 
 def rswoosh(
-    I: List[Cell], 
-    isEqual: Callable[[Contour,Contour], bool], 
-    merge: Callable[[Cell, Cell], Cell]
-    ) -> List[Cell]:
+        I: List[Cell],
+        isEqual: Callable[[Contour, Contour], bool],
+        merge: Callable[[Cell, Cell], Cell]
+        ) -> List[Cell]:
     """
     Given a list of cells, returns the same list without duplicates.
     Must provide a function to check equality and another to merge cells.
     """
-    O = {} # Hash Table
-    while(len(I) > 0):
-        key_r, class_r, r = I.pop() # O(1)
+    out = {}  # Hash Table
+    while (len(I) > 0):
+        key_r, class_r, r = I.pop()  # O(1)
         exist_equal = False
-        for key_s, (class_s, s) in O.items():
-            if isEqual(r,s):
-                del O[key_s] # O(1)
-                I.append(merge((key_r, class_r, r),(key_s, class_s, s))) # O(1)
+        for key_s, (class_s, s) in out.items():
+            if isEqual(r, s):
+                del out[key_s]  # O(1)
+                I.append(merge((key_r, class_r, r), (key_s, class_s, s)))  # O(1)
                 exist_equal = True
                 break
         if not exist_equal:
-            O[key_r] = (class_r, r) # O(1)
-    return O.items()
+            out[key_r] = (class_r, r)  # O(1)
+    return out.items()
```

### Comparing `tumourkit-0.6.0/tumourkit/preprocessing/__init__.py` & `tumourkit-0.7.0/tumourkit/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/preprocessing/centroids2png.py` & `tumourkit-0.7.0/tumourkit/preprocessing/centroids2png.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,26 +22,26 @@
 import numpy as np
 import cv2
 from ..utils.preprocessing import parse_path, create_dir, get_names, read_centroids
 import argparse
 from tqdm import tqdm
 
 
-def centroids2png(centroids: List[Tuple[int,int,int]]) -> np.ndarray:
+def centroids2png(centroids: List[Tuple[int, int, int]]) -> np.ndarray:
     """
     Generates a blank image with pixel value 255 at the coordinates of each centroid.
 
     :param centroids: A list of centroids represented as (X, Y, class) tuples.
-    :type centroids: List[Tuple[int,int,int]]
+    :type centroids: List[Tuple[int, int, int]]
     :return: A NumPy array representing the generated image.
     :rtype: np.ndarray
     """
-    png = np.zeros((1024,1024))
-    for x,y,cls in centroids:
-        png[x,y] = 255
+    png = np.zeros((1024, 1024))
+    for x, y, cls in centroids:
+        png[x, y] = 255
     return png
 
 
 def _create_parser():
     parser = argparse.ArgumentParser()
     parser.add_argument('--centroids-path', type=str, required=True,
                         help='Path to centroid files.')
@@ -60,8 +60,8 @@
         png = centroids2png(centroids)
         cv2.imwrite(output_path + name + '.points.png', png)
 
 
 def main():
     parser = _create_parser()
     args = parser.parse_args()
-    main_with_args(args)
+    main_with_args(args)
```

### Comparing `tumourkit-0.6.0/tumourkit/preprocessing/centroidspng2csv.py` & `tumourkit-0.7.0/tumourkit/preprocessing/centroidspng2csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from argparse import Namespace
 from ..utils.preprocessing import get_names, parse_path, create_dir, read_png, save_csv, read_centroids, get_centroid_by_id
 import pandas as pd
 import numpy as np
 from ..utils.nearest import generate_tree, find_nearest
 from tqdm import tqdm
 
+
 def extract_centroids(img: np.ndarray) -> List[Tuple[int, int, int]]:
     """
     Extracts the centroids of cells from a labeled image. The third coordinates is the index.
 
     :param img: A 2D NumPy array representing the labeled image. Each unique non-zero value represents a different cell.
     :type img: np.ndarray
     :return: A list of tuples containing the x and y coordinates of the centroid, and the cell index.
@@ -45,15 +46,15 @@
             centroids.append((x, y, idx))
     return centroids
 
 
 def centroidspng2csv(centroids_file: np.ndarray, png_file: np.ndarray) -> pd.DataFrame:
     """
     Converts a PNG file with cell labels and a CSV file with cell centroids into a CSV file
-    associating each cell label with the closest centroid. 
+    associating each cell label with the closest centroid.
 
     :param centroids_file: A NumPy array with three columns, representing the X and Y coordinates
                            and class of each centroid.
     :type centroids_file: np.ndarray
     :param png_file: A NumPy array with the same dimensions as the corresponding image file,
                      where each pixel is labeled with an integer representing the cell it belongs to.
     :type png_file: np.ndarray
@@ -101,8 +102,8 @@
         save_csv(csv_file, csv_dir, name)
     return
 
 
 def main():
     parser = _create_parser()
     args = parser.parse_args()
-    main_with_args(args)
+    main_with_args(args)
```

### Comparing `tumourkit-0.6.0/tumourkit/preprocessing/geojson2pngcsv.py` & `tumourkit-0.7.0/tumourkit/preprocessing/geojson2pngcsv.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,53 +33,52 @@
 
     :param gson: A list of GeoJSON features.
     :type gson: List[Dict[str, Any]]
     :param num_classes: The number of classes to use in the output CSV. If not provided, it defaults to 2 (tumour and non-tumour).
     :type num_classes: Optional[int]
     :return: A tuple containing the PNG image array and the Pandas DataFrame of the CSV file.
     :rtype: Tuple[np.ndarray, pd.DataFrame]
-    
+
     This function takes a list of GeoJSON features and generates PNG and CSV labels from them.
     The width and height of the PNG image are assumed to be 1024.
     The function expects the GeoJSON to have specific format, with the geometry stored as a list of coordinates.
     If a feature has a label that is not "tumour" or "non-tumour", the label will be replaced with "ClassN", where N is the class number.
     """
-    png = np.zeros((1024,1024), dtype=np.uint16)
+    png = np.zeros((1024, 1024), dtype=np.uint16)
     csv = pd.DataFrame([], columns=['id', 'label'])
     label_parser = {'tumour': 2, 'non-tumour': 1}
     if num_classes != 2:
-        label_parser = {"Class"+str(k): k for k in range(1, num_classes+1)}
+        label_parser = {"Class" + str(k): k for k in range(1, num_classes + 1)}
     for k, feature in enumerate(gson):
         # Draw filled contour
         contour = feature['geometry']['coordinates'][0]
         if len(contour) <= 1:
             continue
-        assert(contour[0] == contour[-1])
+        assert (contour[0] == contour[-1])
         poly = np.array(contour[:-1])
-        rr, cc = polygon(poly[:,0], poly[:,1], png.shape)
-        png[cc,rr] = k+1
+        rr, cc = polygon(poly[:, 0], poly[:, 1], png.shape)
+        png[cc, rr] = k + 1
 
         # Save row to csv
         label = feature['properties']['classification']['name']
         label = label_parser[label]
-        csv = pd.concat([csv, pd.DataFrame([[k+1,label]], columns=['id', 'label'])])
-        
+        csv = pd.concat([csv, pd.DataFrame([[k + 1, label]], columns=['id', 'label'])])
     return png, csv
 
 
 def _create_parser():
     parser = argparse.ArgumentParser()
-    parser.add_argument('--gson-dir', type=str, required=True, 
+    parser.add_argument('--gson-dir', type=str, required=True,
                         help='Path to the geojson files.')
     parser.add_argument('--png-dir', type=str, required=True,
-                        help='Path to save the png files.')  
+                        help='Path to save the png files.')
     parser.add_argument('--csv-dir', type=str, required=True,
                         help='Path to save the csv files.')
     parser.add_argument('--num-classes', type=int, default=2)
-    return parser 
+    return parser
 
 
 def main_with_args(args):
     gson_dir = parse_path(args.gson_dir)
     png_dir = parse_path(args.png_dir)
     csv_dir = parse_path(args.csv_dir)
 
@@ -88,11 +87,12 @@
 
     names = get_names(gson_dir, '.geojson')
     for name in tqdm(names):
         gson = read_gson(name, gson_dir)
         png, csv = geojson2pngcsv(gson, args.num_classes)
         save_pngcsv(png, csv, png_dir, csv_dir, name)
 
+
 def main():
     parser = _create_parser()
     args = parser.parse_args()
     main_with_args(args)
```

### Comparing `tumourkit-0.6.0/tumourkit/preprocessing/graph2centroids.py` & `tumourkit-0.7.0/tumourkit/preprocessing/graph2centroids.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -71,8 +71,8 @@
         save_centroids(centroids_file, centroids_dir, name)
     return
 
 
 def main():
     parser = _create_parser()
     args = parser.parse_args()
-    main_with_args(args)
+    main_with_args(args)
```

### Comparing `tumourkit-0.6.0/tumourkit/preprocessing/hovernet2centroids.py` & `tumourkit-0.7.0/tumourkit/preprocessing/hovernet2centroids.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,22 +17,21 @@
 
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Contact information: joseperez2000@hotmail.es
 """
 from typing import Dict, Any, List, Tuple
-import pandas as pd
 import argparse
 import logging
 from tqdm import tqdm
 from ..utils.preprocessing import create_dir, read_json, parse_path, get_names, save_centroids
 
 
-def parse_centroids(nuc: Dict[str, Any]) -> List[Tuple[int,int,int]]:
+def parse_centroids(nuc: Dict[str, Any]) -> List[Tuple[int, int, int]]:
     """
     Extracts centroids from a HoverNet JSON dictionary and returns them as a list of (X,Y,class) tuples.
 
     :param nuc: The HoverNet JSON dictionary containing nuclei information.
     :type nuc: Dict[str, Any]
     :return: A list of (X,Y,class) tuples representing centroids.
     :rtype: List[Tuple[int,int,int]]
@@ -44,15 +43,15 @@
     for inst in nuc:
         inst_info = nuc[inst]
         inst_centroid = inst_info['centroid']
         inst_type = inst_info['type']
         if inst_type == 0:
             logging.warning('Found cell with class 0, removing it.')
         else:
-            centroids_.append((inst_centroid[1], inst_centroid[0], inst_type)) 
+            centroids_.append((inst_centroid[1], inst_centroid[0], inst_type))
     return centroids_
 
 
 def _create_parser():
     parser = argparse.ArgumentParser()
     parser.add_argument('--json-dir', type=str, required=True,
                         help='Path to json files.')
```

### Comparing `tumourkit-0.6.0/tumourkit/preprocessing/hovernet2geojson.py` & `tumourkit-0.7.0/tumourkit/preprocessing/hovernet2geojson.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,18 @@
 from typing import Dict, Any, Tuple, List, Optional
 import argparse
 import geojson
 from tqdm import tqdm
 from ..utils.preprocessing import parse_path, get_names, create_dir, read_json, create_geojson
 
 
-Point = Tuple[float,float]
+Point = Tuple[float, float]
 Contour = List[Point]
+
+
 def parse_contours(nuc: Dict[str, Any], num_classes: Optional[int] = 2) -> List[Contour]:
     """
     Parses contours of cells from the given HoverNet JSON dictionary.
 
     :param nuc: A dictionary containing HoverNet nuclei information.
     :type nuc: Dict[str, Any]
     :param num_classes: The number of classes (default 2).
@@ -44,26 +46,26 @@
     contours_ = []
     for inst in nuc:
         inst_info = nuc[inst]
         inst_type = inst_info['type']
         if inst_type >= 1 and inst_type <= num_classes:
             inst_contour = inst_info['contour']
             inst_contour.append(inst_contour[0])
-            contours_.append((inst_contour, inst_type)) 
+            contours_.append((inst_contour, inst_type))
         elif inst_type is None:
             inst_contour = inst_info['contour']
             inst_contour.append(inst_contour[0])
-            contours_.append((inst_contour, 3)) 
+            contours_.append((inst_contour, 3))
     return contours_
 
 
 def save_contours(out_dir: str, name: str, contours: List[Contour]) -> None:
     """
     Save geojson in a file with given name in out_dir.
-    
+
     :param out_dir: The directory where the file will be saved.
     :type out_dir: str
     :param name: The name of the file.
     :type name: str
     :param contours: The list of contours in the GeoJSON format.
     :type contours: List[Contour]
     """
```

### Comparing `tumourkit-0.6.0/tumourkit/preprocessing/png2graph.py` & `tumourkit-0.7.0/tumourkit/preprocessing/png2graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,45 +24,42 @@
 import os
 from concurrent.futures import ThreadPoolExecutor
 import logging
 from tqdm import tqdm
 from ..utils.preprocessing import read_png, save_graph, parse_path, create_dir, get_names, get_mask, apply_mask, add_node, extract_features, read_image
 
 
-
-
-
 def png2graph(img: np.ndarray, png: np.ndarray) -> pd.DataFrame:
     """
     Given an original image and a segmentation mask in PNG format, this function extracts the nodes and their attributes
     and returns them in a pandas DataFrame. The following attributes are computed for each node:
-    
+
     * X: The X-coordinate of the centroid.
     * Y: The Y-coordinate of the centroid.
     * Area: The area of the cell.
     * Perimeter: The perimeter of the cell.
     * Variance: The variance of the grayscale values inside the cell.
     * Histogram: The normalized histogram of the grayscale values inside the cell (5 bins).
-    
+
     :param img: The original image as a numpy array.
     :type img: np.ndarray
     :param png: The segmentation mask in PNG format as a numpy array.
     :type png: np.ndarray
     :return: A pandas DataFrame containing the extracted nodes and their attributes.
     :rtype: pd.DataFrame
     """
     graph = {}
     for idx in np.unique(png):
         if idx == 0:
             continue
         mask = get_mask(png, idx)
-        msk_img, msk, X, Y  = apply_mask(img, mask)
+        msk_img, msk, X, Y = apply_mask(img, mask)
         try:
             feats = extract_features(msk_img, msk)
-        except:
+        except Exception:
             feats = extract_features(msk_img, msk, debug=True)
         if len(feats) > 0:
             feats['id'] = idx
             feats['X'] = X
             feats['Y'] = Y
         add_node(graph, feats)
     return pd.DataFrame(graph)
@@ -82,15 +79,15 @@
 
 def main_subthread(
         name: str,
         png_dir: str,
         orig_dir: str,
         output_path: str,
         pbar: tqdm,
-        )-> None:
+        ) -> None:
     """
     A wrapper function to use multiprocessing.
 
     :param name: The name of the image file (without extension).
     :type name: str
     :param png_dir: The directory path containing PNG segmentation masks.
     :type png_dir: str
@@ -101,15 +98,15 @@
     :param pbar: A progress bar object to track the progress of the computation.
     :type pbar: tqdm.tqdm
     """
     try:
         png = read_png(name, png_dir)
         img = read_image(name, orig_dir)
         graph = png2graph(img, png)
-        save_graph(graph, os.path.join(output_path, name+'.nodes.csv'))
+        save_graph(graph, os.path.join(output_path, name + '.nodes.csv'))
     except Exception as e:
         logging.warning(e)
         logging.warning('Failed at:', name)
     finally:
         pbar.update(1)
 
 
@@ -120,15 +117,15 @@
     create_dir(output_path)
 
     names = get_names(png_dir, '.GT_cells.png')
     pbar = tqdm(total=len(names))
     if args.num_workers > 0:
         with ThreadPoolExecutor(max_workers=args.num_workers) as executor:
             for name in names:
-                executor.submit(main_subthread, name, png_dir, orig_dir, output_path, pbar) 
+                executor.submit(main_subthread, name, png_dir, orig_dir, output_path, pbar)
     else:
         for name in names:
             main_subthread(name, png_dir, orig_dir, output_path, pbar)
 
 
 def main():
     parser = _create_parser()
```

### Comparing `tumourkit-0.6.0/tumourkit/preprocessing/pngcsv2centroids.py` & `tumourkit-0.7.0/tumourkit/preprocessing/pngcsv2centroids.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from tqdm import tqdm
 from ..utils.preprocessing import read_labels, parse_path, create_dir, get_names, save_centroids, get_centroid_by_id
 import numpy as np
 import pandas as pd
 from typing import List, Tuple
 
 
-def extract_centroids(img: np.ndarray, csv: pd.DataFrame) -> List[Tuple[int,int,int]]:
+def extract_centroids(img: np.ndarray, csv: pd.DataFrame) -> List[Tuple[int, int, int]]:
     """
     Extracts the centroids of cells from a labeled image. The third coordinate is the class.
 
     :param img: A 2D NumPy array representing the labeled image. Each unique non-zero value represents a different cell.
     :type img: np.ndarray
     :param csv: A pandas DataFrame representing the labels. Just two colums, one for id and another for the class.
     :type csv: pd.DataFrame
```

### Comparing `tumourkit-0.6.0/tumourkit/preprocessing/pngcsv2geojson.py` & `tumourkit-0.7.0/tumourkit/preprocessing/pngcsv2geojson.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,28 +30,28 @@
     save_geojson
 )
 
 
 def create_mask(png: np.ndarray, csv: pd.DataFrame, label: int) -> np.ndarray:
     """
     Returns an image with only the pixels of the class given in the label.
-    
+
     :param png: Segmentation mask with indices as pixel values.
     :type png: np.ndarray
     :param csv: DataFrame containing the class labels for each cell in the image.
     :type csv: pd.DataFrame
     :param label: Class label to extract from the image.
     :type label: int
     :return: Binary mask where pixels of the specified class have value 1 and all others have value 0.
     :rtype: np.ndarray
     """
     mask = png.copy()
     for i, (idx, cell_label) in csv.iterrows():
         if cell_label != label:
-            mask[mask==idx] = 0
+            mask[mask == idx] = 0
     return np.array(mask, dtype=np.uint8)
 
 
 def pngcsv2features(png: np.ndarray, csv: pd.DataFrame, label: int, num_classes: Optional[int] = 2) -> List[Dict[str, Any]]:
     """
     Computes geojson features of contours of a given class.
```

### Comparing `tumourkit-0.6.0/tumourkit/preprocessing/pngcsv2graph.py` & `tumourkit-0.7.0/tumourkit/preprocessing/pngcsv2graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,31 +26,31 @@
 import logging
 from tqdm import tqdm
 from ..utils.preprocessing import get_mask, read_labels, parse_path, create_dir, save_graph, get_names, apply_mask, extract_features, add_node, read_image
 
 
 def pngcsv2graph(img: np.ndarray, png: np.ndarray, csv: pd.DataFrame) -> pd.DataFrame:
     """
-    Given original image and pngcsv labels, 
+    Given original image and pngcsv labels,
     returns nodes with extracted attributes in a DataFrame.
     Current attributes are:
         - X, Y of centroid
         - Area
         - Perimeter
         - Variance
         - Regularity (not yet)
         - Histogram (5 bins)
     """
     graph = {}
     for idx, cls in csv.itertuples(index=False, name=None):
         mask = get_mask(png, idx)
-        msk_img, msk, X, Y  = apply_mask(img, mask)
+        msk_img, msk, X, Y = apply_mask(img, mask)
         try:
             feats = extract_features(msk_img, msk)
-        except:
+        except Exception:
             feats = extract_features(msk_img, msk, debug=True)
         if len(feats) > 0:
             feats['class'] = cls
             feats['id'] = idx
             feats['X'] = X
             feats['Y'] = Y
         add_node(graph, feats)
@@ -74,23 +74,23 @@
 def main_subthread(
         name: str,
         png_dir: str,
         csv_dir: str,
         orig_dir: str,
         output_path: str,
         pbar: tqdm,
-        )-> None:
+        ) -> None:
     """
     Wrapper to use multiprocessing
     """
     try:
         png, csv = read_labels(name, png_dir, csv_dir)
         img = read_image(name, orig_dir)
         graph = pngcsv2graph(img, png, csv)
-        save_graph(graph, os.path.join(output_path, name+'.nodes.csv'))
+        save_graph(graph, os.path.join(output_path, name + '.nodes.csv'))
     except Exception as e:
         logging.warning(e)
         logging.warning('Failed at:', name)
     finally:
         pbar.update(1)
 
 
@@ -102,15 +102,15 @@
     create_dir(output_path)
 
     names = get_names(png_dir, '.GT_cells.png')
     pbar = tqdm(total=len(names))
     if args.num_workers > 0:
         with ThreadPoolExecutor(max_workers=args.num_workers) as executor:
             for name in names:
-                executor.submit(main_subthread, name, png_dir, csv_dir, orig_dir, output_path, pbar) 
+                executor.submit(main_subthread, name, png_dir, csv_dir, orig_dir, output_path, pbar)
     else:
         for name in names:
             main_subthread(name, png_dir, csv_dir, orig_dir, output_path, pbar)
 
 
 def main():
     parser = _create_parser()
```

### Comparing `tumourkit-0.6.0/tumourkit/profiling/cpairs_profile.py` & `tumourkit-0.7.0/tumourkit/profiling/cpairs_profile.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,71 +12,67 @@
 GNU Affero General Public License for more details.
 
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Contact information: joseperez2000@hotmail.es
 """
-import sys
-import os
 import numpy as np
 import cProfile
 import io
 import pstats
-
-TEST_DIR = os.path.dirname(os.path.abspath(__file__))
-PKG_DIR = os.path.dirname(TEST_DIR)
-sys.path.append(PKG_DIR)
-
-from utils.postprocessing import get_N_closest_pairs_dists
+from ..utils.postprocessing import get_N_closest_pairs_dists
 
 
 THRESHOLD = 0.001
 tests = [
     (
-        np.hstack((np.linspace(0,30,100).reshape(-1,1), np.ones((100,1)))),
-        np.hstack((np.linspace(0,30,100).reshape(-1,1), np.ones((100,1))*2)), 
+        np.hstack((np.linspace(0, 30, 100).reshape(-1, 1), np.ones((100, 1)))),
+        np.hstack((np.linspace(0, 30, 100).reshape(-1, 1), np.ones((100, 1)) * 2)),
         np.ones((10,))
     ),
     (
-        np.hstack((np.linspace(0,300,101).reshape(-1,1), np.ones((101,1))))+np.array([[1,0]]),
-        np.hstack((np.linspace(0,300,101).reshape(-1,1), np.ones((101,1))*2)), 
+        np.hstack((np.linspace(0, 300, 101).reshape(-1, 1), np.ones((101, 1)))) + np.array([[1, 0]]),
+        np.hstack((np.linspace(0, 300, 101).reshape(-1, 1), np.ones((101, 1)) * 2)),
         np.ones((20,)) * np.sqrt(2)
     ),
     (
-        np.hstack((np.linspace(0,30,11).reshape(-1,1)**2, np.ones((11,1)))),
-        np.hstack((np.linspace(0,30,11).reshape(-1,1), np.ones((11,1))*2)), 
-        np.array([1, 1, np.sqrt(3**2+1), np.sqrt(3**2+1), np.sqrt(3**2+1), np.sqrt(6**2+1), np.sqrt(6**2+1)])
+        np.hstack((np.linspace(0, 30, 11).reshape(-1, 1)**2, np.ones((11, 1)))),
+        np.hstack((np.linspace(0, 30, 11).reshape(-1, 1), np.ones((11, 1)) * 2)),
+        np.array([1, 1, np.sqrt(3**2 + 1), np.sqrt(3**2 + 1), np.sqrt(3**2 + 1), np.sqrt(6**2 + 1), np.sqrt(6**2 + 1)])
     ),
     (
-        np.hstack((np.linspace(0,300000,100001).reshape(-1,1), np.ones((100001,1))))+np.array([[1,0]]),
-        np.hstack((np.linspace(0,300,101).reshape(-1,1), np.ones((101,1))*2)), 
+        np.hstack((np.linspace(0, 300000, 100001).reshape(-1, 1), np.ones((100001, 1)))) + np.array([[1, 0]]),
+        np.hstack((np.linspace(0, 300, 101).reshape(-1, 1), np.ones((101, 1)) * 2)),
         np.ones((20,)) * np.sqrt(2)
     )
 ]
-def exec_conversion(A,B, result):
+
+
+def exec_conversion(A, B, result):
     pred = get_N_closest_pairs_dists(A, B, len(result))
     pred = sorted(pred)
     if len(pred) != len(result):
         return False
     for i in range(len(pred)):
         if abs(pred[i] - result[i]) > THRESHOLD:
             return False
     return True
 
 # cProfile.runctx('exec_conversion(*tests[0])', None, locals(), filename='prof1.txt')
 # cProfile.runctx('exec_conversion(*tests[1])', None, locals(), filename='prof2.txt')
 # cProfile.runctx('exec_conversion(*tests[2])', None, locals(), filename='prof3.txt')
 
+
 for i in range(len(tests)):
     pr = cProfile.Profile()
     pr.enable()
 
     my_result = exec_conversion(*tests[i])
 
     pr.disable()
     s = io.StringIO()
     ps = pstats.Stats(pr, stream=s).sort_stats('tottime')
     ps.print_stats()
 
-    with open('cpairs/cpairs_profile' + str(i+1) + '.txt', 'w+') as f:
-        f.write(s.getvalue())
+    with open('cpairs/cpairs_profile' + str(i + 1) + '.txt', 'w+') as f:
+        f.write(s.getvalue())
```

### Comparing `tumourkit-0.6.0/tumourkit/profiling/rswoosh_profile.py` & `tumourkit-0.7.0/tumourkit/profiling/rswoosh_profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,42 +15,41 @@
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Contact information: joseperez2000@hotmail.es
 """
 import cProfile
 import io
 import pstats
-import sys
 import os
 import json
+from postprocessing.rswoosh import rswoosh
+from ..utils.preprocessing import get_names, parse_path
+from ..utils.postprocessing import create_comparator, merge_cells
+
 
 PROF_DIR = os.path.dirname(os.path.abspath(__file__))
 PKG_DIR = os.path.dirname(PROF_DIR)
-sys.path.append(PKG_DIR)
-
-from postprocessing.rswoosh import rswoosh
-from utils.preprocessing import get_names, parse_path
-from utils.postprocessing import create_comparator, merge_cells
-
 RSWOOSH_DIR = parse_path(PKG_DIR) + 'tests/rswoosh/'
 THRESHOLD = 1
 NUM_FRONTIER = 15
-
 names = get_names(RSWOOSH_DIR, '.input.json')
+
+
 def exec_conversion(name):
     with open(RSWOOSH_DIR + name + '.input.json', 'r') as f:
         inp = json.load(f)
     with open(RSWOOSH_DIR + name + '.output.json', 'r') as f:
         expected_out = json.load(f)
     predicted_out = rswoosh(inp, create_comparator(THRESHOLD, NUM_FRONTIER), merge_cells)
     if not len(predicted_out) == len(expected_out):
         print(name)
         return False
     return True
 
+
 for name in names:
     pr = cProfile.Profile()
     pr.enable()
 
     my_result = exec_conversion(name)
 
     pr.disable()
```

### Comparing `tumourkit-0.6.0/tumourkit/research_pipe.py` & `tumourkit-0.7.0/tumourkit/research_pipe.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,33 @@
+"""
+Pipeline to ease experiment replication.
+
+Copyright (C) 2023  Jose Pérez Cano
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU Affero General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU Affero General Public License for more details.
+
+You should have received a copy of the GNU Affero General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Contact information: joseperez2000@hotmail.es
+"""
 import shutil
 import argparse
 from argparse import Namespace
 import logging
 from logging import Logger
 import os
-import pandas as pd
 from .segmentation import hov_train, hov_infer
 from .utils.pipes import check_training, WrongConfigurationError, HovernetNotFoundError, check_void
 from .preprocessing import hovernet2centroids, geojson2pngcsv, pngcsv2centroids
 from .segmentation import pngcsv2npy
 from .utils.preprocessing import get_names
 from . import eval_segment
 from .classification import train_xgb, train_gnn
@@ -20,60 +39,60 @@
     os.makedirs(args.output_dir, exist_ok=True)
     if args.experiment == 'scaling':
         if args.pretrained_path is None:
             raise WrongConfigurationError('You must provide a path to pretrained Hovernet weights for the scaling experiment.')
     return
 
 
-def hovernet_preproc_with_shape(shape: str, args: Namespace, logger : Logger) -> None:
+def hovernet_preproc_with_shape(shape: str, args: Namespace, logger: Logger) -> None:
     """
     Converts the gson format to the rest of formats.
     """
     real_shape = shape[:-2] if 'FT' in shape else shape
     os.makedirs(os.path.join(args.output_dir, 'hovernet', 'data', real_shape), exist_ok=True)
     for split in ['train', 'validation', 'test']:
         logger.info(f'Parsing {split} split')
         if check_void(os.path.join(args.root_dir, 'data', split, 'png')) or check_void(os.path.join(args.root_dir, 'data', split, 'csv')):
             logger.info('   From geojson to pngcsv.')
             newargs = Namespace(
-                gson_dir = os.path.join(args.root_dir, 'data', split, 'gson'),
-                png_dir = os.path.join(args.root_dir, 'data', split, 'png'),
-                csv_dir = os.path.join(args.root_dir, 'data', split, 'csv'),
-                num_classes = args.num_classes,
+                gson_dir=os.path.join(args.root_dir, 'data', split, 'gson'),
+                png_dir=os.path.join(args.root_dir, 'data', split, 'png'),
+                csv_dir=os.path.join(args.root_dir, 'data', split, 'csv'),
+                num_classes=args.num_classes,
             )
             geojson2pngcsv(newargs)
         os.makedirs(os.path.join(args.output_dir, 'hovernet', 'data', real_shape, split), exist_ok=True)
         os.makedirs(os.path.join(args.output_dir, 'hovernet', 'data', real_shape, split, 'npy'), exist_ok=True)
         if check_void(os.path.join(args.output_dir, 'hovernet', 'data', real_shape, split, 'npy')):
             newargs = Namespace(
-                orig_dir = os.path.join(args.root_dir, 'data', 'orig'),
-                png_dir = os.path.join(args.root_dir, 'data', split, 'png'),
-                csv_dir = os.path.join(args.root_dir, 'data', split, 'csv'),
-                out_dir = os.path.join(args.output_dir, 'hovernet', 'data', real_shape, split, 'npy'),
-                save_example = False, use_labels = True, split = False,
-                shape = real_shape
+                orig_dir=os.path.join(args.root_dir, 'data', 'orig'),
+                png_dir=os.path.join(args.root_dir, 'data', split, 'png'),
+                csv_dir=os.path.join(args.root_dir, 'data', split, 'csv'),
+                out_dir=os.path.join(args.output_dir, 'hovernet', 'data', real_shape, split, 'npy'),
+                save_example=False, use_labels=True, split=False,
+                shape=real_shape
             )
             pngcsv2npy(newargs)
     return
 
 
 def train_hovernet_with_shape(shape: str, args: Namespace, logger: Logger) -> None:
     logger.info(f'Starting hovernet preprocessing of {shape}.')
     hovernet_preproc_with_shape(shape, args, logger)
     logger.info(f'Starting training of {shape}.')
     os.makedirs(os.path.join(args.output_dir, 'hovernet', 'weights', shape), exist_ok=True)
     real_shape = shape[:-2] if 'FT' in shape else shape
     newargs = Namespace(
-        gpu = args.gpu, view = None, save_name = None,
-        log_dir = os.path.join(args.output_dir, 'hovernet', 'weights', shape),
-        train_dir = os.path.join(args.output_dir, 'hovernet', 'data', real_shape, 'train', 'npy'),
-        valid_dir = os.path.join(args.output_dir, 'hovernet', 'data', real_shape, 'validation', 'npy'),
-        pretrained_path = args.pretrained_path if 'FT' in shape else None,
-        shape = real_shape,
-        num_classes = args.num_classes,
+        gpu=args.gpu, view=None, save_name=None,
+        log_dir=os.path.join(args.output_dir, 'hovernet', 'weights', shape),
+        train_dir=os.path.join(args.output_dir, 'hovernet', 'data', real_shape, 'train', 'npy'),
+        valid_dir=os.path.join(args.output_dir, 'hovernet', 'data', real_shape, 'validation', 'npy'),
+        pretrained_path=args.pretrained_path if 'FT' in shape else None,
+        shape=real_shape,
+        num_classes=args.num_classes,
     )
     hov_train(newargs)
 
 
 def infer_hovernet_with_shape(shape: str, args: Namespace, logger: Logger) -> None:
     logger.info(f'Starting inference of {shape}.')
     newargs = {
@@ -96,67 +115,67 @@
         'save_qupath': False,
         'save_raw_map': False,
         'mem_usage': '0.2'
     }
     hov_infer(newargs, newsubargs, 'tile')
 
 
-def run_postprocessing_with_shape(shape: str, args: Namespace, logger : Logger) -> None:
+def run_postprocessing_with_shape(shape: str, args: Namespace, logger: Logger) -> None:
     """
     Converts the gson format to the rest of formats.
     """
     logger.info('Extracting Hovernet centroids from training output.')
     if not os.path.isdir(os.path.join(args.output_dir, 'hovernet', 'output', shape, 'json')):
         raise HovernetNotFoundError('Please, train again or extract hovernet outputs.')
     newargs = Namespace(
-        json_dir = os.path.join(args.output_dir, 'hovernet', 'output', shape, 'json'),
-        output_path = os.path.join(args.output_dir, 'hovernet', 'output', shape, 'centroids_hov'),
+        json_dir=os.path.join(args.output_dir, 'hovernet', 'output', shape, 'json'),
+        output_path=os.path.join(args.output_dir, 'hovernet', 'output', shape, 'centroids_hov'),
     )
     hovernet2centroids(newargs)
     for split in ['train', 'validation', 'test']:
         if check_void(os.path.join(args.root_dir, 'data', split, 'names.txt')):
             logger.info(f'Preprocessing split {split}.')
             split_names = get_names(os.path.join(args.root_dir, 'data', split, 'gson'), '.geojson')
             with open(os.path.join(args.root_dir, 'data', split, 'names.txt'), 'w') as f:
                 for name in split_names:
                     print(name, file=f)
         if check_void(os.path.join(args.root_dir, 'data', split, 'png')) or check_void(os.path.join(args.root_dir, 'data', split, 'csv')):
             logger.info('   From geojson to pngcsv.')
             newargs = Namespace(
-                gson_dir = os.path.join(args.root_dir, 'data', split, 'gson'),
-                png_dir = os.path.join(args.root_dir, 'data', split, 'png'),
-                csv_dir = os.path.join(args.root_dir, 'data', split, 'csv'),
-                num_classes = args.num_classes,
+                gson_dir=os.path.join(args.root_dir, 'data', split, 'gson'),
+                png_dir=os.path.join(args.root_dir, 'data', split, 'png'),
+                csv_dir=os.path.join(args.root_dir, 'data', split, 'csv'),
+                num_classes=args.num_classes,
             )
             geojson2pngcsv(newargs)
         if check_void(os.path.join(args.root_dir, 'data', split, 'centroids')):
             logger.info('   Extracting centroids from GT.')
             newargs = Namespace(
-                png_dir = os.path.join(args.root_dir, 'data', split, 'png'),
-                csv_dir = os.path.join(args.root_dir, 'data', split, 'csv'),
-                output_path = os.path.join(args.root_dir, 'data', split, 'centroids')
+                png_dir=os.path.join(args.root_dir, 'data', split, 'png'),
+                csv_dir=os.path.join(args.root_dir, 'data', split, 'csv'),
+                output_path=os.path.join(args.root_dir, 'data', split, 'centroids')
             )
             pngcsv2centroids(newargs)
 
 
 def evaluate_hovernet_with_shape(shape: str, args: Namespace, logger: Logger) -> None:
     logger.info(f'Starting evaluation of {shape}.')
     os.makedirs(os.path.join(args.output_dir, 'hovernet', 'output', shape, 'results'), exist_ok=True)
     for split in ['train', 'validation', 'test']:
         logger.info(f'    Evaluating {split} split')
         newargs = Namespace(
-            names = os.path.join(args.root_dir, 'data', split, 'names.txt'),
-            gt_path = os.path.join(args.root_dir, 'data', split, 'centroids'),
-            pred_path = os.path.join(args.output_dir, 'hovernet', 'output', shape, 'centroids_hov'),
-            save_name = os.path.join(args.output_dir, 'hovernet', 'output', shape, 'results', shape + '_' + split),
-            debug_path = None,
-            num_classes = args.num_classes
+            names=os.path.join(args.root_dir, 'data', split, 'names.txt'),
+            gt_path=os.path.join(args.root_dir, 'data', split, 'centroids'),
+            pred_path=os.path.join(args.output_dir, 'hovernet', 'output', shape, 'centroids_hov'),
+            save_name=os.path.join(args.output_dir, 'hovernet', 'output', shape, 'results', shape + '_' + split),
+            debug_path=None,
+            num_classes=args.num_classes
         )
         eval_segment(newargs, logger)
-    
+
 
 def run_scaling(args: Namespace, logger: Logger) -> None:
     os.makedirs(os.path.join(args.output_dir, 'hovernet'), exist_ok=True)
     os.makedirs(os.path.join(args.output_dir, 'hovernet', 'weights'), exist_ok=True)
     os.makedirs(os.path.join(args.output_dir, 'hovernet', 'data'), exist_ok=True)
     train_hovernet_with_shape('270', args, logger)
     train_hovernet_with_shape('270FT', args, logger)
@@ -189,87 +208,87 @@
     files = [os.path.join(tr_graphs_dir, f) for f in os.listdir(tr_graphs_dir)] + \
             [os.path.join(val_graphs_dir, f) for f in os.listdir(val_graphs_dir)]
     for file in files:
         shutil.copy(file, all_graphs_dir)
     logger.info('Starting XGBoost training.')
     os.makedirs(os.path.join(args.output_dir, 'xgb'), exist_ok=True)
     newargs = Namespace(
-        graph_dir = all_graphs_dir,
-        test_graph_dir = os.path.join(args.root_dir, 'data', 'test', 'graphs', 'preds'),
-        val_size = 0.2,
-        seed = 0,
-        num_workers = args.num_workers,
-        cv_folds = 5,
-        save_name = os.path.join(args.output_dir, 'xgb', 'cv_results'),
-        num_classes = args.num_classes,
+        graph_dir=all_graphs_dir,
+        test_graph_dir=os.path.join(args.root_dir, 'data', 'test', 'graphs', 'preds'),
+        val_size=0.2,
+        seed=0,
+        num_workers=args.num_workers,
+        cv_folds=5,
+        save_name=os.path.join(args.output_dir, 'xgb', 'cv_results'),
+        num_classes=args.num_classes,
     )
     train_xgb(newargs, logger)
 
 
 def run_void(args: Namespace, logger: Logger) -> None:
     logger.info('Training GNN without prior.')
     newargs = Namespace(
-        train_node_dir = os.path.join(args.root_dir, 'data', 'train', 'graphs', 'preds'),
-        validation_node_dir = os.path.join(args.root_dir, 'data', 'validation', 'graphs', 'preds'),
-        test_node_dir = os.path.join(args.root_dir, 'data', 'test', 'graphs', 'preds'),
-        log_dir = os.path.join(args.output_dir, 'gnn_no_prior_logs'),
-        early_stopping_rounds = 10,
-        batch_size = 10,
-        model_name = 'GCN',
-        save_file = os.path.join(args.output_dir, 'gnn_no_prior_logs', 'gnn_results'),
-        num_confs = 32,
-        save_dir = os.path.join(args.root_dir, 'weights', 'classification', 'gnn_no_prior'),
-        device = 'cpu' if args.gpu == '' else 'cuda',
-        num_workers = args.num_workers,
-        checkpoint_iters = -1,
-        num_classes = args.num_classes,
-        disable_prior = True,
-        disable_morph_feats = False,
+        train_node_dir=os.path.join(args.root_dir, 'data', 'train', 'graphs', 'preds'),
+        validation_node_dir=os.path.join(args.root_dir, 'data', 'validation', 'graphs', 'preds'),
+        test_node_dir=os.path.join(args.root_dir, 'data', 'test', 'graphs', 'preds'),
+        log_dir=os.path.join(args.output_dir, 'gnn_no_prior_logs'),
+        early_stopping_rounds=10,
+        batch_size=10,
+        model_name='GCN',
+        save_file=os.path.join(args.output_dir, 'gnn_no_prior_logs', 'gnn_results'),
+        num_confs=32,
+        save_dir=os.path.join(args.root_dir, 'weights', 'classification', 'gnn_no_prior'),
+        device='cpu' if args.gpu == '' else 'cuda',
+        num_workers=args.num_workers,
+        checkpoint_iters=-1,
+        num_classes=args.num_classes,
+        disable_prior=True,
+        disable_morph_feats=False,
     )
     train_gnn(newargs)
 
     logger.info('Training GNN without morphological features.')
     newargs = Namespace(
-        train_node_dir = os.path.join(args.root_dir, 'data', 'train', 'graphs', 'preds'),
-        validation_node_dir = os.path.join(args.root_dir, 'data', 'validation', 'graphs', 'preds'),
-        test_node_dir = os.path.join(args.root_dir, 'data', 'test', 'graphs', 'preds'),
-        log_dir = os.path.join(args.output_dir, 'gnn_no_morph_logs'),
-        early_stopping_rounds = 10,
-        batch_size = 10,
-        model_name = 'GCN',
-        save_file = os.path.join(args.output_dir, 'gnn_no_morph_logs', 'gnn_results'),
-        num_confs = 32,
-        save_dir = os.path.join(args.root_dir, 'weights', 'classification', 'gnn_no_morph'),
-        device = 'cpu' if args.gpu == '' else 'cuda',
-        num_workers = args.num_workers,
-        checkpoint_iters = -1,
-        num_classes = args.num_classes,
-        disable_prior = False,
-        disable_morph_feats = True,
+        train_node_dir=os.path.join(args.root_dir, 'data', 'train', 'graphs', 'preds'),
+        validation_node_dir=os.path.join(args.root_dir, 'data', 'validation', 'graphs', 'preds'),
+        test_node_dir=os.path.join(args.root_dir, 'data', 'test', 'graphs', 'preds'),
+        log_dir=os.path.join(args.output_dir, 'gnn_no_morph_logs'),
+        early_stopping_rounds=10,
+        batch_size=10,
+        model_name='GCN',
+        save_file=os.path.join(args.output_dir, 'gnn_no_morph_logs', 'gnn_results'),
+        num_confs=32,
+        save_dir=os.path.join(args.root_dir, 'weights', 'classification', 'gnn_no_morph'),
+        device='cpu' if args.gpu == '' else 'cuda',
+        num_workers=args.num_workers,
+        checkpoint_iters=-1,
+        num_classes=args.num_classes,
+        disable_prior=False,
+        disable_morph_feats=True,
     )
     train_gnn(newargs)
 
     logger.info('Training void GNN.')
     newargs = Namespace(
-        train_node_dir = os.path.join(args.root_dir, 'data', 'train', 'graphs', 'preds'),
-        validation_node_dir = os.path.join(args.root_dir, 'data', 'validation', 'graphs', 'preds'),
-        test_node_dir = os.path.join(args.root_dir, 'data', 'test', 'graphs', 'preds'),
-        log_dir = os.path.join(args.output_dir, 'gnn_void_logs'),
-        early_stopping_rounds = 10,
-        batch_size = 10,
-        model_name = 'GCN',
-        save_file = os.path.join(args.output_dir, 'gnn_void_logs', 'gnn_results'),
-        num_confs = 32,
-        save_dir = os.path.join(args.root_dir, 'weights', 'classification', 'gnn_void'),
-        device = 'cpu' if args.gpu == '' else 'cuda',
-        num_workers = args.num_workers,
-        checkpoint_iters = -1,
-        num_classes = args.num_classes,
-        disable_prior = True,
-        disable_morph_feats = True,
+        train_node_dir=os.path.join(args.root_dir, 'data', 'train', 'graphs', 'preds'),
+        validation_node_dir=os.path.join(args.root_dir, 'data', 'validation', 'graphs', 'preds'),
+        test_node_dir=os.path.join(args.root_dir, 'data', 'test', 'graphs', 'preds'),
+        log_dir=os.path.join(args.output_dir, 'gnn_void_logs'),
+        early_stopping_rounds=10,
+        batch_size=10,
+        model_name='GCN',
+        save_file=os.path.join(args.output_dir, 'gnn_void_logs', 'gnn_results'),
+        num_confs=32,
+        save_dir=os.path.join(args.root_dir, 'weights', 'classification', 'gnn_void'),
+        device='cpu' if args.gpu == '' else 'cuda',
+        num_workers=args.num_workers,
+        checkpoint_iters=-1,
+        num_classes=args.num_classes,
+        disable_prior=True,
+        disable_morph_feats=True,
     )
     train_gnn(newargs)
 
 
 def run_cnn(args: Namespace, logger: Logger) -> None:
     raise NotImplementedError
 
@@ -285,15 +304,15 @@
     parser.add_argument('--num-workers', type=int, default=0)
     return parser
 
 
 def main():
     parser = _create_parser()
     args = parser.parse_args()
-    
+
     logger = logging.getLogger('research_pipe')
     logger.setLevel(logging.DEBUG)
     ch = logging.StreamHandler()
     ch.setLevel(logging.DEBUG)
     formatter = logging.Formatter('%(name)s - %(levelname)s - %(message)s')
     ch.setFormatter(formatter)
     logger.addHandler(ch)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/evaluate.py` & `tumourkit-0.7.0/tumourkit/segmentation/evaluate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Evaluating script for cell predictions. 
+Evaluating script for cell predictions.
 
 Input format
 ------------
 Centroids in a csv with columns X,Y and class. Both for prediction and GT.
 
 Output
 ------
@@ -37,81 +37,82 @@
 import argparse
 from argparse import Namespace
 import logging
 from logging import Logger
 
 
 def get_confusion_matrix(
-    gt_centroids: List[Tuple[int,int,int]], 
-    pred_centroids: List[Tuple[int,int,int]]
-    ) -> np.ndarray:
+        gt_centroids: List[Tuple[int, int, int]],
+        pred_centroids: List[Tuple[int, int, int]]
+        ) -> np.ndarray:
     """
     Each centroid is represented by a 3-tuple with (X, Y, class).
     Matrix has (N+1)x(N+1) entries, one more for background when no match is found.
     N is the maximum value encountered for class.
     """
     if len(gt_centroids) == 0 and len(pred_centroids) == 0:
         return np.array([[0]])
     if len(gt_centroids) == 0:
-        N = np.max(pred_centroids[:,2])
-        M = np.zeros((N+1,N+1))
-        classes, freqs = np.unique(pred_centroids[:,2], return_counts=True)
+        N = np.max(pred_centroids[:, 2])
+        M = np.zeros((N + 1, N + 1))
+        classes, freqs = np.unique(pred_centroids[:, 2], return_counts=True)
         M[0, classes] += freqs
         return M
     if len(pred_centroids) == 0:
-        N = np.max(gt_centroids[:,2])
-        M = np.zeros((N+1,N+1))
-        classes, freqs = np.unique(gt_centroids[:,2], return_counts=True)
+        N = np.max(gt_centroids[:, 2])
+        M = np.zeros((N + 1, N + 1))
+        classes, freqs = np.unique(gt_centroids[:, 2], return_counts=True)
         M[classes, 0] += freqs
         return M
     if type(gt_centroids) == list:
         gt_centroids = np.array(gt_centroids)
     if type(pred_centroids) == list:
         pred_centroids = np.array(pred_centroids)
-    N = int(max(np.max(gt_centroids[:,2]), np.max(pred_centroids[:,2])))
-    assert min(np.min(gt_centroids[:,2]), np.min(pred_centroids[:,2])) > 0, 'Zero should not be a class.'
-    gt_tree = generate_tree(gt_centroids[:,:2])
-    pred_tree = generate_tree(pred_centroids[:,:2])
-    M = np.zeros((N+1,N+1)) 
+    N = int(max(np.max(gt_centroids[:, 2]), np.max(pred_centroids[:, 2])))
+    assert min(np.min(gt_centroids[:, 2]), np.min(pred_centroids[:, 2])) > 0, 'Zero should not be a class.'
+    gt_tree = generate_tree(gt_centroids[:, :2])
+    pred_tree = generate_tree(pred_centroids[:, :2])
+    M = np.zeros((N + 1, N + 1))
     for point_id, point in enumerate(gt_centroids):
         closest_id = find_nearest(point[:2], pred_tree)
         closest = pred_centroids[closest_id]
         if point_id == find_nearest(closest[:2], gt_tree):
-            M[int(point[2])][int(closest[2])] += 1 # 1-1 matchings
+            M[int(point[2])][int(closest[2])] += 1  # 1-1 matchings
         else:
-            M[int(point[2])][0] += 1 # GT not matched in prediction
+            M[int(point[2])][0] += 1  # GT not matched in prediction
     for point_id, point in enumerate(pred_centroids):
         closest_id = find_nearest(point[:2], gt_tree)
         closest = gt_centroids[closest_id]
         if point_id != find_nearest(closest[:2], pred_tree):
-            M[0][int(point[2])] += 1 # Prediction not matched in GT
+            M[0][int(point[2])] += 1  # Prediction not matched in GT
     return M
 
+
 def get_pairs(
-    gt_centroids: List[Tuple[int,int,int]], 
-    pred_centroids: List[Tuple[int,int,int]]
-    ) -> Tuple[np.ndarray, np.ndarray]:
+        gt_centroids: List[Tuple[int, int, int]],
+        pred_centroids: List[Tuple[int, int, int]]
+        ) -> Tuple[np.ndarray, np.ndarray]:
     """
     Each centroid is represented by a 3-tuple with (X, Y, class).
     Class is 1=non-tumour, 2=tumour.
     Returns true and predicted labels ordered by their correspondences.
     Returned labels start at 0.
     """
     if len(gt_centroids) == 0:
         return None, None
 
-    gt_tree = generate_tree(gt_centroids[:,:2])
-    pred_tree = generate_tree(pred_centroids[:,:2])
+    gt_tree = generate_tree(gt_centroids[:, :2])
+    pred_tree = generate_tree(pred_centroids[:, :2])
     true_labels, pred_labels = [], []
     for point_id, point in enumerate(gt_centroids):
         closest_id = find_nearest(point[:2], pred_tree)
         closest = pred_centroids[closest_id]
         if closest[2] != -1 and point[2] != -1 and point_id == find_nearest(closest[:2], gt_tree):
-            true_labels.append(point[2]-1)
-            pred_labels.append(closest[2]-1)
+            true_labels.append(point[2] - 1)
+            pred_labels.append(closest[2] - 1)
     return np.array(true_labels), np.array(pred_labels)
 
 
 def compute_f1_score_from_matrix(conf_mat: np.ndarray, cls: int) -> float:
     """
     Returns f1 score of given class against the rest.
     If no positive or predictive positive classes are found, None is returned.
@@ -127,28 +128,29 @@
         return None
     precision = TP / PP
     recall = TP / P
     if TP == 0:
         return 0
     return 2 * precision * recall / (precision + recall)
 
+
 def compute_metrics_from_matrix(conf_mat: np.ndarray) -> Tuple[float, float, float, float]:
     """
     Given confusion matrix,
     returns F1 score, Accuracy, ROC AUC and percentage error.
     """
     total = np.sum(conf_mat)
     acc = np.matrix.trace(conf_mat) / total
     n_classes = len(conf_mat)
     macro, weighted = 0, 0
     real_n_classes = n_classes
     adjust_weighted = 1
     for k in range(n_classes):
         f1_class = compute_f1_score_from_matrix(conf_mat, cls=k)
-        cls_supp = conf_mat[k,:].sum() / total
+        cls_supp = conf_mat[k, :].sum() / total
         if f1_class is not None:
             macro += f1_class
             weighted += f1_class * cls_supp
         else:
             real_n_classes -= 1
             adjust_weighted -= cls_supp
     macro /= real_n_classes
@@ -162,39 +164,40 @@
     If B is bigger than A, A is enlarged with zeros.
     And vice versa.
     """
     if A.shape == B.shape:
         return A + B
     n, m = A.shape[0], B.shape[0]
     if m > n:
-        res = np.zeros((m,m))
-        res[:n,:n] += A
+        res = np.zeros((m, m))
+        res[:n, :n] += A
         res += B
     else:
-        res = np.zeros((n,n))
-        res[:m,:m] += B
+        res = np.zeros((n, n))
+        res[:m, :m] += B
         res += A
     return res
 
 
 def save_csv(
-    metrics: Dict[str, List[float]], 
-    save_path: str
-    ) -> None:
+        metrics: Dict[str, List[float]],
+        save_path: str
+        ) -> None:
     """
     Saves metrics in csv format for later use.
     Columns depend on dictionary keys.
     """
     metrics_df = pd.DataFrame(metrics)
     metrics_df.to_csv(save_path + '.csv', index=False)
 
+
 def save_debug_matrix(
-    mat: np.ndarray,
-    save_path: str
-    ) -> None:
+        mat: np.ndarray,
+        save_path: str
+        ) -> None:
     """
     Saves confusion matrices for debug purposes.
     """
     conf_mat_df = pd.DataFrame(mat)
     conf_mat_df.to_csv(save_path + '.csv')
 
 
@@ -225,15 +228,15 @@
         metrics = {
             'Name': [], 'Macro F1': [], 'Weighted F1': [], 'Micro F1': [], 'ECE': [],
             'Macro F1 (bkgr)': [], 'Weighted F1 (bkgr)': [], 'Micro F1 (bkgr)': []
         }
     global_conf_mat = None
     global_pred, global_true = [], []
     for k, name in enumerate(names):
-        logger.info('Progress: {:2d}/{}'.format(k+1, len(names)))
+        logger.info('Progress: {:2d}/{}'.format(k + 1, len(names)))
         metrics['Name'].append(name)
         # Read
         gt_centroids = read_centroids(name, args.gt_path)
         pred_centroids = read_centroids(name, args.pred_path)
         # Compute pairs and confusion matrix
         conf_mat = get_confusion_matrix(gt_centroids, pred_centroids)
         if args.debug_path is not None:
@@ -298,20 +301,21 @@
         micro, macro, weighted, ece = _global_metrics
         global_metrics = {
             'Name': ['All'], 'Macro F1': [macro], 'Weighted F1': [weighted], 'Micro F1': [micro], 'ECE': [ece],
             'Macro F1 (bkgr)': [macro_bkgr], 'Weighted F1 (bkgr)': [weighted_bkgr], 'Micro F1 (bkgr)': [micro_bkgr]
         }
     save_csv(global_metrics, args.save_name + '_all')
 
+
 def main():
     parser = _create_parser()
     args = parser.parse_args()
 
     logger = logging.getLogger('eval_segment')
     logger.setLevel(logging.DEBUG)
     ch = logging.StreamHandler()
     ch.setLevel(logging.DEBUG)
     formatter = logging.Formatter('%(name)s - %(levelname)s - %(message)s')
     ch.setFormatter(formatter)
     logger.addHandler(ch)
 
-    main(args, logger)
+    main(args, logger)
```

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/config.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/config.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/dataloader/augs.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/dataloader/augs.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/dataloader/infer_loader.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/dataloader/infer_loader.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/dataloader/train_loader.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/dataloader/train_loader.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/extract_patches.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/extract_patches.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/infer/base.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/infer/base.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/infer/tile.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/infer/tile.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/infer/wsi.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/infer/wsi.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/metrics/stats_utils.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/metrics/stats_utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/misc/patch_extractor.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/misc/patch_extractor.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/misc/utils.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/misc/utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/misc/viz_utils.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/misc/viz_utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/misc/wsi_handler.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/misc/wsi_handler.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/net_desc.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/net_utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/opt.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/opt.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/post_proc.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/run_desc.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/targets.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/targets.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/models/hovernet/utils.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/models/hovernet/utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_infer.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_infer.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/callbacks/logging.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/callbacks/serialize.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/engine.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/engine.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/run_utils/utils.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/run_utils/utils.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/segmentation/hovernet/train.py` & `tumourkit-0.7.0/tumourkit/segmentation/hovernet/train.py`

 * *Files identical despite different names*

### Comparing `tumourkit-0.6.0/tumourkit/train_pipe.py` & `tumourkit-0.7.0/tumourkit/train_pipe.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,59 +1,79 @@
+"""
+Training pipeline.
+
+Copyright (C) 2023  Jose Pérez Cano
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU Affero General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU Affero General Public License for more details.
+
+You should have received a copy of the GNU Affero General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Contact information: joseperez2000@hotmail.es
+"""
 import argparse
 from argparse import Namespace
 from .preprocessing import geojson2pngcsv, pngcsv2graph, hovernet2geojson, pngcsv2centroids
 from .segmentation import pngcsv2npy
 import os
 import logging
 from logging import Logger
 from .segmentation import hov_train, hov_infer
 from .utils.preprocessing import get_names
 import shutil
 from .postprocessing import join_graph_gt, join_hovprob_graph
 from .classification import train_gnn
 
 
-def run_preproc_pipe(args: Namespace, logger : Logger) -> None:
+def run_preproc_pipe(args: Namespace, logger: Logger) -> None:
     """
     Converts the gson format to the rest of formats.
     """
     for split in ['train', 'validation', 'test']:
         logger.info(f'Parsing {split} split')
         newargs = Namespace(
-            gson_dir = os.path.join(args.root_dir, 'data', split, 'gson'),
-            png_dir = os.path.join(args.root_dir, 'data', split, 'png'),
-            csv_dir = os.path.join(args.root_dir, 'data', split, 'csv'),
-            num_classes = args.num_classes,
+            gson_dir=os.path.join(args.root_dir, 'data', split, 'gson'),
+            png_dir=os.path.join(args.root_dir, 'data', split, 'png'),
+            csv_dir=os.path.join(args.root_dir, 'data', split, 'csv'),
+            num_classes=args.num_classes,
         )
         geojson2pngcsv(newargs)
         newargs = Namespace(
-            orig_dir = os.path.join(args.root_dir, 'data', 'orig'),
-            png_dir = os.path.join(args.root_dir, 'data', split, 'png'),
-            csv_dir = os.path.join(args.root_dir, 'data', split, 'csv'),
-            out_dir = os.path.join(args.root_dir, 'data', split, 'npy'),
-            save_example = False, use_labels = True, split = False,
-            shape = '518'
+            orig_dir=os.path.join(args.root_dir, 'data', 'orig'),
+            png_dir=os.path.join(args.root_dir, 'data', split, 'png'),
+            csv_dir=os.path.join(args.root_dir, 'data', split, 'csv'),
+            out_dir=os.path.join(args.root_dir, 'data', split, 'npy'),
+            save_example=False, use_labels=True, split=False,
+            shape='518'
         )
         pngcsv2npy(newargs)
     return
 
 
-def run_hov_pipe(args: Namespace, logger : Logger) -> None:
+def run_hov_pipe(args: Namespace, logger: Logger) -> None:
     """
     Trains hovernet and predicts cell contours on json format.
     """
     logger.info('Starting training.')
     newargs = Namespace(
-        gpu = args.gpu, view = None, save_name = None,
-        log_dir = os.path.join(args.root_dir, 'weights', 'segmentation', 'hovernet'),
-        train_dir = os.path.join(args.root_dir, 'data', 'train', 'npy'),
-        valid_dir = os.path.join(args.root_dir, 'data', 'validation', 'npy'),
-        pretrained_path = args.pretrained_path,
-        shape = '518',
-        num_classes = args.num_classes,
+        gpu=args.gpu, view=None, save_name=None,
+        log_dir=os.path.join(args.root_dir, 'weights', 'segmentation', 'hovernet'),
+        train_dir=os.path.join(args.root_dir, 'data', 'train', 'npy'),
+        valid_dir=os.path.join(args.root_dir, 'data', 'validation', 'npy'),
+        pretrained_path=args.pretrained_path,
+        shape='518',
+        num_classes=args.num_classes,
     )
     hov_train(newargs)
     logger.info('Starting inference.')
     newargs = {
         'nr_types': str(args.num_classes + 1),
         'type_info_path': os.path.join(args.root_dir, 'weights', 'segmentation', 'hovernet', 'type_info.json'),
         'gpu': args.gpu,
@@ -73,15 +93,15 @@
         'save_raw_map': False,
         'mem_usage': '0.2'
     }
     hov_infer(newargs, newsubargs, 'tile')
     return
 
 
-def run_postproc_pipe(args: Namespace, logger : Logger) -> None:
+def run_postproc_pipe(args: Namespace, logger: Logger) -> None:
     """
     Converts the json format to the graph format containing GT and preds.
     """
     logger.info('Moving json files to corresponding folders.')
     tr_files = set(get_names(os.path.join(args.root_dir, 'data', 'train', 'gson'), '.geojson'))
     val_files = set(get_names(os.path.join(args.root_dir, 'data', 'validation', 'gson'), '.geojson'))
     ts_files = set(get_names(os.path.join(args.root_dir, 'data', 'test', 'gson'), '.geojson'))
@@ -92,101 +112,101 @@
                 os.path.join(args.root_dir, 'data', 'tmp_hov', 'json', file + '.json'),
                 os.path.join(args.root_dir, 'data', folder_name, 'json')
             )
     for split in ['train', 'validation', 'test']:
         logger.info(f'Parsing {split} split')
         logger.info('   From json to geojson.')
         newargs = Namespace(
-            json_dir = os.path.join(args.root_dir, 'data', split, 'json'),
-            gson_dir = os.path.join(args.root_dir, 'data', split, 'gson_hov'),
-            num_classes = args.num_classes
+            json_dir=os.path.join(args.root_dir, 'data', split, 'json'),
+            gson_dir=os.path.join(args.root_dir, 'data', split, 'gson_hov'),
+            num_classes=args.num_classes
         )
         hovernet2geojson(newargs)
         logger.info('   From geojson to pngcsv.')
         newargs = Namespace(
-            gson_dir = os.path.join(args.root_dir, 'data', split, 'gson_hov'),
-            png_dir = os.path.join(args.root_dir, 'data', split, 'png_hov'),
-            csv_dir = os.path.join(args.root_dir, 'data', split, 'csv_hov'),
-            num_classes = args.num_classes,
+            gson_dir=os.path.join(args.root_dir, 'data', split, 'gson_hov'),
+            png_dir=os.path.join(args.root_dir, 'data', split, 'png_hov'),
+            csv_dir=os.path.join(args.root_dir, 'data', split, 'csv_hov'),
+            num_classes=args.num_classes,
         )
         geojson2pngcsv(newargs)
         logger.info('   From pngcsv to nodes.csv.')
         newargs = Namespace(
-            png_dir = os.path.join(args.root_dir, 'data', split, 'png_hov'),
-            csv_dir = os.path.join(args.root_dir, 'data', split, 'csv_hov'),
-            orig_dir = os.path.join(args.root_dir, 'data', 'orig'),
-            output_path = os.path.join(args.root_dir, 'data', split, 'graphs', 'raw'),
-            num_workers = args.num_workers
+            png_dir=os.path.join(args.root_dir, 'data', split, 'png_hov'),
+            csv_dir=os.path.join(args.root_dir, 'data', split, 'csv_hov'),
+            orig_dir=os.path.join(args.root_dir, 'data', 'orig'),
+            output_path=os.path.join(args.root_dir, 'data', split, 'graphs', 'raw'),
+            num_workers=args.num_workers
         )
         pngcsv2graph(newargs)
         logger.info('   Extracting centroids from GT.')
         newargs = Namespace(
-            png_dir = os.path.join(args.root_dir, 'data', split, 'png'),
-            csv_dir = os.path.join(args.root_dir, 'data', split, 'csv'),
-            output_path = os.path.join(args.root_dir, 'data', split, 'centroids')
+            png_dir=os.path.join(args.root_dir, 'data', split, 'png'),
+            csv_dir=os.path.join(args.root_dir, 'data', split, 'csv'),
+            output_path=os.path.join(args.root_dir, 'data', split, 'centroids')
         )
         pngcsv2centroids(newargs)
         logger.info('   Adding GT labels to .nodes.csv.')
         newargs = Namespace(
-            graph_dir = os.path.join(args.root_dir, 'data', split, 'graphs', 'raw'),
-            centroids_dir = os.path.join(args.root_dir, 'data', split, 'centroids'),
-            output_dir = os.path.join(args.root_dir, 'data', split, 'graphs', 'GT')
+            graph_dir=os.path.join(args.root_dir, 'data', split, 'graphs', 'raw'),
+            centroids_dir=os.path.join(args.root_dir, 'data', split, 'centroids'),
+            output_dir=os.path.join(args.root_dir, 'data', split, 'graphs', 'GT')
         )
         join_graph_gt(newargs)
         logger.info('   Adding hovernet predictions to .nodes.csv.')
         newargs = Namespace(
-            json_dir = os.path.join(args.root_dir, 'data', split, 'json'),
-            graph_dir = os.path.join(args.root_dir, 'data', split, 'graphs', 'GT'),
-            output_dir = os.path.join(args.root_dir, 'data', split, 'graphs', 'preds'),
-            num_classes = args.num_classes,
+            json_dir=os.path.join(args.root_dir, 'data', split, 'json'),
+            graph_dir=os.path.join(args.root_dir, 'data', split, 'graphs', 'GT'),
+            output_dir=os.path.join(args.root_dir, 'data', split, 'graphs', 'preds'),
+            num_classes=args.num_classes,
         )
         join_hovprob_graph(newargs, logger)
     return
 
 
-def run_graph_pipe(args: Namespace, logger : Logger) -> None:
+def run_graph_pipe(args: Namespace, logger: Logger) -> None:
     """
     Trains the graph models.
     """
     newargs = Namespace(
-        train_node_dir = os.path.join(args.root_dir, 'data', 'train', 'graphs', 'preds'),
-        validation_node_dir = os.path.join(args.root_dir, 'data', 'validation', 'graphs', 'preds'),
-        test_node_dir = os.path.join(args.root_dir, 'data', 'test', 'graphs', 'preds'),
-        log_dir = os.path.join(args.root_dir, 'gnn_logs'),
-        early_stopping_rounds = 10,
-        batch_size = 20,
-        model_name = 'GCN',
-        save_file = os.path.join(args.root_dir, 'gnn_logs', 'gcn_results'),
-        num_confs = 32,
-        save_dir = os.path.join(args.root_dir, 'weights', 'classification', 'gnn'),
-        device = 'cpu' if args.gpu == '' else 'cuda',
-        num_workers = args.num_workers,
-        checkpoint_iters = -1,
-        num_classes = args.num_classes,
-        disable_prior = False,
-        disable_morph_feats = False,
+        train_node_dir=os.path.join(args.root_dir, 'data', 'train', 'graphs', 'preds'),
+        validation_node_dir=os.path.join(args.root_dir, 'data', 'validation', 'graphs', 'preds'),
+        test_node_dir=os.path.join(args.root_dir, 'data', 'test', 'graphs', 'preds'),
+        log_dir=os.path.join(args.root_dir, 'gnn_logs'),
+        early_stopping_rounds=10,
+        batch_size=20,
+        model_name='GCN',
+        save_file=os.path.join(args.root_dir, 'gnn_logs', 'gcn_results'),
+        num_confs=32,
+        save_dir=os.path.join(args.root_dir, 'weights', 'classification', 'gnn'),
+        device='cpu' if args.gpu == '' else 'cuda',
+        num_workers=args.num_workers,
+        checkpoint_iters=-1,
+        num_classes=args.num_classes,
+        disable_prior=False,
+        disable_morph_feats=False,
     )
     train_gnn(newargs)
     newargs = Namespace(
-        train_node_dir = os.path.join(args.root_dir, 'data', 'train', 'graphs', 'preds'),
-        validation_node_dir = os.path.join(args.root_dir, 'data', 'validation', 'graphs', 'preds'),
-        test_node_dir = os.path.join(args.root_dir, 'data', 'test', 'graphs', 'preds'),
-        log_dir = os.path.join(args.root_dir, 'gnn_logs'),
-        early_stopping_rounds = 10,
-        batch_size = 20,
-        model_name = 'ATT',
-        save_file = os.path.join(args.root_dir, 'gnn_logs', 'gat_results'),
-        num_confs = 32,
-        save_dir = os.path.join(args.root_dir, 'weights', 'classification', 'gnn'),
-        device = 'cpu' if args.gpu == '' else 'cuda',
-        num_workers = args.num_workers,
-        checkpoint_iters = -1,
-        num_classes = args.num_classes,
-        disable_prior = False,
-        disable_morph_feats = False,
+        train_node_dir=os.path.join(args.root_dir, 'data', 'train', 'graphs', 'preds'),
+        validation_node_dir=os.path.join(args.root_dir, 'data', 'validation', 'graphs', 'preds'),
+        test_node_dir=os.path.join(args.root_dir, 'data', 'test', 'graphs', 'preds'),
+        log_dir=os.path.join(args.root_dir, 'gnn_logs'),
+        early_stopping_rounds=10,
+        batch_size=20,
+        model_name='ATT',
+        save_file=os.path.join(args.root_dir, 'gnn_logs', 'gat_results'),
+        num_confs=32,
+        save_dir=os.path.join(args.root_dir, 'weights', 'classification', 'gnn'),
+        device='cpu' if args.gpu == '' else 'cuda',
+        num_workers=args.num_workers,
+        checkpoint_iters=-1,
+        num_classes=args.num_classes,
+        disable_prior=False,
+        disable_morph_feats=False,
     )
     train_gnn(newargs)
     return
 
 
 def _create_parser():
     parser = argparse.ArgumentParser()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tumourkit-0.6.0/tumourkit/utils/calibration_error.py` & `tumourkit-0.7.0/tumourkit/utils/calibration_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 import numpy as np
 
 from sklearn.utils import assert_all_finite
 from sklearn.utils import check_consistent_length
 from sklearn.utils import column_or_1d
 
+
 def calibration_error(y_true, y_prob, sample_weight=None, norm='l2',
                       n_bins=10, strategy='uniform', pos_label=None,
                       reduce_bias=True):
     """Compute calibration error of a binary classifier.
     Across all items in a set of N predictions, the calibration error measures
     the aggregated difference between (1) the average predicted probabilities
     assigned to the positive class, and (2) the frequencies
@@ -147,8 +148,8 @@
         loss = np.sum(delta_loss) / count
     elif norm == "l2":
         delta_loss = (avg_pred_true - bin_centroid)**2 * delta_count
         loss = np.sum(delta_loss) / count
         if reduce_bias:
             loss += np.sum(debias)
         loss = np.sqrt(max(loss, 0.))
-    return loss
+    return loss
```

### Comparing `tumourkit-0.6.0/tumourkit/utils/classification.py` & `tumourkit-0.7.0/tumourkit/utils/classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import numpy as np
 from sklearn.preprocessing import StandardScaler
 from typing import Tuple, List, Optional
 from sklearn.metrics import roc_auc_score, f1_score, accuracy_score
 from .read_nodes import _read_all_nodes
 from .calibration_error import calibration_error
 
+
 def normalize(X_train: np.ndarray, X_val: np.ndarray, X_test: np.ndarray) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
     """
     Normalizes the input data using the mean and standard deviation of the training dataset.
 
     :param X_train: The input training data with shape (n_samples, n_features).
     :type X_train: numpy.ndarray
     :param X_val: The input validation data with shape (n_samples, n_features).
@@ -41,14 +42,15 @@
              - The normalized X_test with shape (n_samples, n_features).
     :rtype: tuple(numpy.ndarray, numpy.ndarray, numpy.ndarray)
     """
     sc = StandardScaler()
     sc.fit(X_train)
     return sc.transform(X_train), sc.transform(X_val), sc.transform(X_test)
 
+
 def fit_column_normalizer(
         node_dir: str,
         names: List[str],
         remove_prior: Optional[bool] = False,
         remove_morph: Optional[bool] = False,
         ) -> StandardScaler:
     """
@@ -61,15 +63,15 @@
     :param remove_prior: If True, hovernet probabilites are ignored.
     :type remove_prior: Optional[bool]
     :param remove_morph: If True, morphological features are removed.
     :type remove_morph: Optional[bool]
     :return: A StandardScaler object fitted to the input data.
     :rtype: StandardScaler
     """
-    X, y = _read_all_nodes(node_dir, [x+'.nodes.csv' for x in names], remove_morph=remove_morph, remove_prior=remove_prior)
+    X, y = _read_all_nodes(node_dir, [x + '.nodes.csv' for x in names], remove_morph=remove_morph, remove_prior=remove_prior)
     sc = StandardScaler()
     sc.fit(X)
     return sc
 
 
 def check_imbalance(y_true: np.ndarray) -> bool:
     """
@@ -78,16 +80,16 @@
     return len(np.unique(y_true)) > 1
 
 
 def percentage_error(y_true: np.ndarray, y_pred: np.ndarray) -> float:
     """
     Computes the deviation in the percentage of tumoral cells.
     """
-    gt_perc = (y_true==1).sum() / len(y_true)
-    pred_perc = (y_pred==1).sum() / len(y_pred)
+    gt_perc = (y_true == 1).sum() / len(y_true)
+    pred_perc = (y_pred == 1).sum() / len(y_pred)
     return abs(gt_perc - pred_perc)
 
 
 def metrics_from_predictions(
         y_true: np.ndarray,
         y_pred: np.ndarray,
         y_prob: Optional[np.ndarray] = None,
@@ -135,8 +137,8 @@
                 y_true_i = (y_true == i) * 1
                 y_prob_i = y_prob[:, i]
                 ece_i = calibration_error(y_true_i, y_prob_i, norm='l1', reduce_bias=False)
                 ece += ece_i
             ece /= num_classes
         else:
             ece = -1
-        return micro, macro, weighted, ece
+        return micro, macro, weighted, ece
```

### Comparing `tumourkit-0.6.0/tumourkit/utils/folder2txt.py` & `tumourkit-0.7.0/tumourkit/utils/folder2txt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """
-
-Script to generate txt files with the names of the files in the 
+Script to generate txt files with the names of the files in the
 train, validation, test split folders.
 
 Input
 -----
 The path to the folders.
 
 Output
 ------
-Txt files with one name per line, the names don't contain the 
+Txt files with one name per line, the names don't contain the
 (x,y).npy at the end.
 
 Copyright (C) 2023  Jose Pérez Cano
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU Affero General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
@@ -41,29 +40,31 @@
 parser.add_argument('--validation', type=str,
                     help='Path to validation folder as created by my_extract_patches.py')
 parser.add_argument('--test', type=str,
                     help='Path to test folder as created by my_extract_patches.py')
 parser.add_argument('--out-dir', type=str,
                     help='Path to save the txt files.')
 
+
 def remove_coordinates(name: str) -> str:
     """
     Removes the (number, number) pattern and '.npy' extension from the input string.
 
     :param name: The input string with a (number, number) pattern and '.npy' extension.
     :type name: str
     :return: The input string with the (number, number) pattern and '.npy' extension removed.
     :rtype: str
     """
-    regex = '\([0-9]{1,3},[0-9]{1,3}\)'
+    regex = r'\([0-9]{1,3},[0-9]{1,3}\)'
     parenthesis = re.findall(regex, name)
     par_len = len(parenthesis[0])
     npy_len = len('.npy')
     return name[:-(par_len + npy_len)]
 
+
 def read_files(path: str) -> List[str]:
     """
     Returns a list of file names without the (number, number).npy pattern at the end.
 
     :param path: The path to the directory containing the files.
     :type path: str
     :return: A list of file names without the (number, number).npy pattern at the end.
@@ -72,14 +73,15 @@
     files = os.listdir(path)
     file_list = []
     for file_name in files:
         file_list.append(remove_coordinates(file_name))
     file_list = list(set(file_list))
     return file_list
 
+
 def save_txt(file_list: List[str], path: str, name: str) -> None:
     """
     Saves a list of file names to a text file with one name per line.
 
     :param file_list: The list of file names to save.
     :type file_list: list[str]
     :param path: The path to the directory where the text file will be saved.
@@ -88,19 +90,20 @@
     :type name: str
     :return: None
     """
     with open(path + name, 'a') as f:
         for file_name in file_list:
             print(file_name, file=f)
 
-if __name__=='__main__':
+
+if __name__ == '__main__':
     args = parser.parse_args()
     train_files = read_files(args.train)
     val_files = read_files(args.validation)
     test_files = read_files(args.test)
 
     OUT_DIR = parse_path(args.out_dir)
     create_dir(OUT_DIR)
 
     save_txt(train_files, OUT_DIR, 'train.txt')
     save_txt(val_files, OUT_DIR, 'validation.txt')
-    save_txt(test_files, OUT_DIR, 'test.txt')
+    save_txt(test_files, OUT_DIR, 'test.txt')
```

### Comparing `tumourkit-0.6.0/tumourkit/utils/nearest.py` & `tumourkit-0.7.0/tumourkit/utils/nearest.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,62 +18,67 @@
 
 Contact information: joseperez2000@hotmail.es
 """
 from scipy.spatial import KDTree
 import numpy as np
 from typing import List, Tuple, Optional
 
-def generate_tree(centroids: List[Tuple[int,int,int]]) -> KDTree:
+
+def generate_tree(centroids: List[Tuple[int, int, int]]) -> KDTree:
     """
     Returns a KDTree object from a list of (x, y, class) tuples.
 
     :param centroids: A list of (x, y, class) tuples representing the centroids.
     :type centroids: list[tuple(int, int, int)]
     :return: A KDTree object created from the x and y coordinates of the centroids.
     :rtype: KDTree
     """
     centroids_ = np.array(list(map(lambda x: (x[0], x[1]), centroids)))
     return KDTree(centroids_)
 
-def find_nearest(a: Tuple[int,int,int], B: KDTree) -> int:
+
+def find_nearest(a: Tuple[int, int, int], B: KDTree) -> int:
     """
     Finds the index of the nearest point in a KDTree to a given (x, y, class) tuple.
 
     :param a: The (x, y, class) tuple to search for the nearest point.
     :type a: tuple(int, int, int)
     :param B: The KDTree to search for the nearest point.
     :type B: KDTree
     :return: The index of the nearest point in the KDTree to the given tuple.
     :rtype: int
     """
     x, y = a[0], a[1]
-    dist, idx = B.query([x,y], k=1)
+    dist, idx = B.query([x, y], k=1)
     return idx
 
-def find_nearest_dist_idx(a: Tuple[int,int,int], B: KDTree) -> Tuple[float, int]:
+
+def find_nearest_dist_idx(a: Tuple[int, int, int], B: KDTree) -> Tuple[float, int]:
     """
     Finds the distance and index of the nearest point in a KDTree to a given (x, y, class) tuple.
 
     :param a: The (x, y, class) tuple to search for the nearest point.
     :type a: tuple(int, int, int)
     :param B: The KDTree to search for the nearest point.
     :type B: KDTree
     :return: A tuple containing the distance and index of the nearest point in the KDTree to the given tuple.
     :rtype: tuple(float, int)
     """
     x, y = a[0], a[1]
-    dist, idx = B.query([x,y], k=1)
+    dist, idx = B.query([x, y], k=1)
     return dist, idx
 
-Point = Tuple[float,float]
+
+Point = Tuple[float, float]
 Contour = List[Point]
-Cell = Tuple[int, int, Contour] # id, class
+Cell = Tuple[int, int, Contour]  # id, class
+
 
 def get_N_closest_pairs_dists(a: Contour, b: Contour, N: int,
-    threshold: Optional[float] = np.inf) -> List[float]:
+                              threshold: Optional[float] = np.inf) -> List[float]:
     """
     Returns the N closest pairs distances between two sets of points.
 
     :param a: The first set of points as a list of (x, y) tuples.
     :type a: Contour
     :param b: The second set of points as a list of (x, y) tuples.
     :type b: Contour
@@ -96,16 +101,17 @@
     for point in query_set:
         dist, idx = tree.query(point, k=N, distance_upper_bound=threshold)
         cpairs.extend(dist)
         cpairs.sort()
         cpairs = cpairs[:N]
     return cpairs
 
+
 def get_N_closest_pairs_idx(a: Contour, b: Contour, N: int,
-    threshold: Optional[float] = np.inf) -> Tuple[List[int],List[int]]:
+                            threshold: Optional[float] = np.inf) -> Tuple[List[int], List[int]]:
     """
     Returns the indices of the N closest pairs of points between two sets of points.
 
     :param a: The first set of points as a list of (x, y) tuples.
     :type a: Contour
     :param b: The second set of points as a list of (x, y) tuples.
     :type b: Contour
@@ -130,8 +136,8 @@
         dist, idx = tree.query(point, k=N, distance_upper_bound=threshold)
         cpairs.extend(zip(dist, idx, [idx2 for _ in range(len(idx))]))
         cpairs.sort()
         cpairs = cpairs[:N]
     dists, idxa, idxb = list(zip(*cpairs))
     if not is_a_tree:
         idxa, idxb = idxb, idxa
-    return list(idxa), list(idxb)
+    return list(idxa), list(idxb)
```

### Comparing `tumourkit-0.6.0/tumourkit/utils/pipes.py` & `tumourkit-0.7.0/tumourkit/utils/pipes.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,18 +56,17 @@
     for element in graph_check_list:
         if not check_void(element):
             exist_result_file = True
             graph_result_file = element
     if not exist_result_file:
         graph_folder = os.path.join(args.root_dir, 'gnn_logs')
         raise WrongConfigurationError(f'There is not graph result csv file under {graph_folder}')
-        
+
     dir_list = [os.path.join(args.root_dir, 'weights', 'classification', 'gnn', dir) for dir in ['confs', 'normalizers', 'weights']]
     if not check_same_num(dir_list):
         raise WrongConfigurationError('Graph weights folders contain different number of files. Try running the training pipeline again')
-    
+
     results = pd.read_csv(graph_result_file)
     if 'F1 Score' in results.columns and args.num_classes != 2:
         raise WrongConfigurationError('You have trained the GNN models for binary problem but are asking to run research for multiclass.')
     elif 'Micro F1' in results.columns and args.num_classes == 2:
         raise WrongConfigurationError('You have trained the GNN models for multiclass problem but are asking to run research for binary.')
-
```

### Comparing `tumourkit-0.6.0/tumourkit/utils/postprocessing.py` & `tumourkit-0.7.0/tumourkit/utils/postprocessing.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,23 +14,24 @@
 GNU Affero General Public License for more details.
 
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Contact information: joseperez2000@hotmail.es
 """
-
 from typing import Callable, Tuple, List
 from .nearest import get_N_closest_pairs_dists, get_N_closest_pairs_idx
 
-Point = Tuple[float,float]
+
+Point = Tuple[float, float]
 Contour = List[Point]
-Cell = Tuple[int, int, Contour] # id, class
+Cell = Tuple[int, int, Contour]  # id, class
 
-def create_comparator(threshold: float, num_frontier: int) -> Callable[[Contour,Contour], bool]:
+
+def create_comparator(threshold: float, num_frontier: int) -> Callable[[Contour, Contour], bool]:
     """
     Returns a comparator function between two contours.
 
     :param threshold: The maximum distance allowed between the num_frontier closest pairs of points to consider two contours equal.
     :type threshold: float
     :param num_frontier: The number of closest pairs of points to consider when comparing contours.
     :type num_frontier: int
@@ -40,25 +41,26 @@
     This function returns a comparator function between two contours.
     The comparator function takes two contours as input and returns True if the two contours are equal and False otherwise.
     Two contours are considered equal if their num_frontier closest pairs of points are at a distance lower than the specified threshold.
     The function returns the comparator function as a callable object.
     """
     def is_equal(a: Contour, b: Contour) -> bool:
         """
-        Two contours are equal if their num_frontier closest pairs 
+        Two contours are equal if their num_frontier closest pairs
         are at a distance lower than threshold.
         """
         cpairs_dists = get_N_closest_pairs_dists(a, b, num_frontier)
         for dist in cpairs_dists:
             if dist > threshold:
                 return False
         return True
     return is_equal
 
-def get_greatest_connected_component(idx: List[int], max_idx: int) -> Tuple[int,int]:
+
+def get_greatest_connected_component(idx: List[int], max_idx: int) -> Tuple[int, int]:
     """
     Given a list of indices, returns the left and right value of the greatest connected component.
 
     :param idx: A list of indices.
     :type idx: list[int]
     :param max_idx: The maximum index value.
     :type max_idx: int
@@ -71,39 +73,40 @@
     When a gap between indices is found, the function checks if the current component is greater than the previous greatest component and updates the left and right indices if it is.
     If the list of indices is circular (i.e., the first and last indices are connected), the function handles this case separately.
     The function returns a tuple containing the left and right values of the greatest connected component.
     """
     idx.sort()
     l_final, l_aux, r_final, r_aux = 0, 0, 0, 0
     found_comp = False
-    for k in range(1,len(idx)):
-        if idx[k-1]+1 != idx[k]:
+    for k in range(1, len(idx)):
+        if idx[k - 1] + 1 != idx[k]:
             found_comp = True
             # End of component
-            r_aux = k-1
-            if  r_aux - l_aux > r_final - l_final:
+            r_aux = k - 1
+            if r_aux - l_aux > r_final - l_final:
                 # Save greatest component
                 r_final, l_final = r_aux, l_aux
             # Restart left auxiliary index
             l_aux = k
     if not found_comp:
         return idx[0], idx[-1]
     if idx[0] == 0 and idx[-1] == max_idx:
         # Circular case
         r_aux = 1
-        while r_aux < len(idx) and idx[r_aux-1] + 1 == idx[r_aux]:
+        while r_aux < len(idx) and idx[r_aux - 1] + 1 == idx[r_aux]:
             r_aux += 1
         r_aux -= 1
-        l_aux = len(idx)-1
-        while l_aux >= 0 and idx[l_aux-1] + 1 == idx[l_aux]:
+        l_aux = len(idx) - 1
+        while l_aux >= 0 and idx[l_aux - 1] + 1 == idx[l_aux]:
             l_aux -= 1
-        if (r_aux-0) + (len(idx)-l_aux) > r_final - l_final:
+        if (r_aux - 0) + (len(idx) - l_aux) > r_final - l_final:
             r_final, l_final = r_aux, l_aux
     return idx[l_final], idx[r_final]
 
+
 def remove_idx(a: Cell, a_idx: List[int]) -> Cell:
     """
     Removes all the indices in a's contour that are included in a_idx's greatest connected component.
 
     :param a: The cell containing the contour to modify.
     :type a: Cell
     :param a_idx: A list of indices.
@@ -112,31 +115,33 @@
     :rtype: Cell
 
     This function takes a cell `a` and a list of indices `a_idx` as input and removes from the contour in `a` all indices that are included in the greatest connected component of `a_idx`.
     The function calls the `get_greatest_connected_component()` function to determine the left and right indices of the greatest connected component.
     The function then creates a new list of indices that includes all the indices in the contour of `a` that are not in the greatest connected component of `a_idx`.
     The function returns a new cell containing the original cell's first two elements and the modified list of indices as the third element.
     """
-    left, right = get_greatest_connected_component(a_idx, len(a[2])-1)
+    left, right = get_greatest_connected_component(a_idx, len(a[2]) - 1)
     res = []
-    if left > right: # Contour is in third position
-        res.extend(a[2][right+1:left])
+    if left > right:  # Contour is in third position
+        res.extend(a[2][right + 1:left])
     elif left <= right:
-        res.extend(a[2][right+1:])
-        res.extend(a[2][0:left]) 
+        res.extend(a[2][right + 1:])
+        res.extend(a[2][0:left])
     return (a[0], a[1], res)
 
+
 def check_order(a: Cell, b: Cell) -> Cell:
     """
     THIS FUNCTION IS NOT IMPLEMENTED YET.
 
     This function is intended to check whether joining two cells `a` and `b` creates a cross in the middle.
     """
     return True
 
+
 def join(a: Cell, b: Cell) -> Cell:
     """
     Joins two cells by appending all the points in `b`'s contour to `a`'s contour.
 
     :param a: The first cell to join.
     :type a: Cell
     :param b: The second cell to join.
@@ -146,14 +151,15 @@
     """
     good_order = check_order(a, b)
     if not good_order:
         b[2].reverse()
     a[2].extend(b[2])
     return a
 
+
 def merge_cells(a: Cell, b: Cell) -> Cell:
     """
     Merges two cells by removing their 30 closest pairs and connecting the endpoints.
 
     :param a: The first cell to merge.
     :type a: Cell
     :param b: The second cell to merge.
@@ -161,8 +167,8 @@
     :return: A new cell containing the merged contours.
     :rtype: Cell
     """
     a_idx, b_idx = get_N_closest_pairs_idx(a[2], b[2], 30)
     a = remove_idx(a, a_idx)
     b = remove_idx(b, b_idx)
     c = join(a, b)
-    return c
+    return c
```

### Comparing `tumourkit-0.6.0/tumourkit/utils/preprocessing.py` & `tumourkit-0.7.0/tumourkit/utils/preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """
-
 Module with utility functions for preprocessing.
 
 Copyright (C) 2023  Jose Pérez Cano
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU Affero General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
@@ -39,24 +38,26 @@
     :return: The parsed file path with a trailing slash.
     :rtype: str
     """
     if path[-1] != '/':
         return path + '/'
     return path
 
+
 def create_dir(path: str) -> None:
     """
     Creates a directory at the specified path if it does not already exist.
 
     :param path: The path of the directory to create.
     :type path: str
     """
     if not os.path.isdir(path):
         os.mkdir(path)
 
+
 def get_names(path: str, pattern: str) -> List[str]:
     """
     This function returns a list of all files in a directory located at <path> that contain the substring <pattern> in their name. The <pattern> substring is then removed from the names and the resulting list is returned.
 
     :param path: The path of the directory to search in.
     :type path: str
     :param pattern: The substring to search for in file names.
@@ -67,14 +68,15 @@
     names_raw = os.listdir(path)
     names = []
     for name in names_raw:
         if pattern in name:
             names.append(name[:-len(pattern)])
     return names
 
+
 def read_names(file_path: str) -> List[str]:
     """
     Returns a list of file names in the specified path that contain the given pattern.
 
     :param path: The path to search for files.
     :type path: str
     :param pattern: The pattern to search for in file names.
@@ -102,15 +104,15 @@
     This function reads a PNG file from the specified directory and returns its image data as a NumPy array.
     The function expects the PNG file to have a specific filename format: '<name>.GT_cells.png'.
     If the function is unable to read the PNG file or encounters an error, it returns `None`.
     """
     try:
         img = cv2.imread(os.path.join(png_dir, name + '.GT_cells.png'), -1)
         return img
-    except:
+    except Exception:
         return None
 
 
 def read_csv(name: str, csv_dir: str) -> Tuple[np.ndarray, pd.DataFrame]:
     """
     Reads a CSV file from the specified directory and returns its contents as a Pandas DataFrame.
 
@@ -125,33 +127,33 @@
     The function expects the CSV file to have a specific filename format: '<name>.class.csv'.
     If the function is unable to read the CSV file or encounters an error, it returns `None`.
     """
     try:
         csv = pd.read_csv(os.path.join(csv_dir, name + '.class.csv'), header=None)
         csv.columns = ['id', 'label']
         return csv
-    except:
+    except Exception:
         return None
-    
 
-def read_gson(name: str, path: str) -> List[Dict[str,Any]]:
+
+def read_gson(name: str, path: str) -> List[Dict[str, Any]]:
     """
     Reads the GeoJSON file at the specified path with the given name.
 
     :param name: The base name of the file (without extension).
     :type name: str
     :param path: The path to the directory containing the file.
     :type path: str
     :return: The contents of the GeoJSON file as a list of dictionaries.
     :rtype: List[Dict[str, Any]]
     """
     with open(os.path.join(path, name + '.geojson'), 'r') as f:
         gson = geojson.load(f)
     return gson
-    
+
 
 def read_labels(name: str, png_dir: str, csv_dir: str) -> Tuple[np.ndarray, pd.DataFrame]:
     """
     Reads a PNG and CSV file from the specified directories and returns their contents as a tuple.
 
     :param name: The base name of the files (without extensions).
     :type name: str
@@ -166,15 +168,15 @@
     The function expects the PNG and CSV files to have specific filename formats: '<name>.GT_cells.png' and '<name>.class.csv'.
     If the function is unable to read either file or encounters an error, it returns (`None`,`None`).
     """
     try:
         img = read_png(name, png_dir)
         csv = read_csv(name, csv_dir)
         return img, csv
-    except:
+    except Exception:
         return None, None
 
 
 def read_json(json_path: str) -> Dict[str, Any]:
     """
     Reads a Hovernet JSON file from the specified path and returns the nuclei information as a dictionary.
 
@@ -188,14 +190,15 @@
     The function expects the JSON file to contain a 'nuc' key with the nuclei information.
     """
     with open(json_path) as json_file:
         data = json.load(json_file)
         nuc_info = data['nuc']
     return nuc_info
 
+
 def read_centroids(name: str, path: str) -> np.ndarray:
     """
     Reads a CSV file from the specified directory containing centroids and returns their contents as a NumPy array.
 
     :param name: The base name of the CSV file (without extension).
     :type name: str
     :param path: The directory containing the CSV file.
@@ -204,15 +207,15 @@
     :rtype: np.ndarray
 
     This function reads a CSV file from the specified directory containing centroids and returns their contents as a NumPy array.
     The function expects the CSV file to have specific column names: 'X', 'Y', and 'class'.
     Centroids with class -1 are dropped and the coordinates are converted to integers.
     """
     centroid_csv = pd.read_csv(os.path.join(path, name + '.centroids.csv'))
-    centroid_csv = centroid_csv.drop(centroid_csv[centroid_csv['class']==-1].index)
+    centroid_csv = centroid_csv.drop(centroid_csv[centroid_csv['class'] == -1].index)
     return centroid_csv.to_numpy(dtype=int)
 
 
 def read_graph(name: str, graph_dir: str) -> pd.DataFrame:
     """
     Reads a graph in CSV format from the specified directory and returns it as a Pandas DataFrame.
 
@@ -227,88 +230,91 @@
     The function expects the graph file to have a specific filename format: '<name>.nodes.csv'.
     If the function is unable to read the file or encounters an error, it returns `None`.
     """
     df = pd.read_csv(os.path.join(graph_dir, name + '.nodes.csv'))
     return df
 
 
-Point = Tuple[float,float]
+Point = Tuple[float, float]
 Contour = List[Point]
+
+
 def format_contour(contour: Contour) -> Contour:
     """
     Formats a contour in cv2.findContours format to an array of shape (N,2).
     Additionally, the first point is added to the end to close the contour.
 
     :param contour: The contour to be formatted.
     :type contour: Contour
     :return: The formatted contour.
     :rtype: Contour
     """
-    new_contour = np.reshape(contour, (-1,2)).tolist()
+    new_contour = np.reshape(contour, (-1, 2)).tolist()
     new_contour.append(new_contour[0])
     return new_contour
 
-def create_geojson(contours: List[Tuple[int,int]], num_classes: Optional[int] = 2) -> List[Dict[str, Any]]:
+
+def create_geojson(contours: List[Tuple[int, int]], num_classes: Optional[int] = 2) -> List[Dict[str, Any]]:
     """
-    Converts a list of contours and their labels to a list of dictionaries 
+    Converts a list of contours and their labels to a list of dictionaries
     containing GeoJSON-formatted data.
 
-    :param contours: A list of pairs (contour, label) where contour is a list of points starting 
-        and finishing in the same point and label is an integer representing the class of the 
+    :param contours: A list of pairs (contour, label) where contour is a list of points starting
+        and finishing in the same point and label is an integer representing the class of the
         cell (1: non-tumour, 2: tumour).
     :type contours: List[Tuple[int, int]]
     :param num_classes: The number of classes in the data. Defaults to 2.
     :type num_classes: Optional[int]
     :return: A list of dictionaries with the GeoJSON format of QuPath.
     :rtype: List[Dict[str, Any]]
 
-    This function converts a list of contours and their labels to a list of dictionaries 
-    containing GeoJSON-formatted data. The function expects the contours to be a list of 
-    pairs (contour, label), where contour is a list of points starting and finishing in the 
-    same point, and label is an integer representing the class of the cell (1: non-tumour, 
-    2: tumour). 
-
-    The function returns a list of dictionaries with the GeoJSON format of QuPath. The 
-    number of classes can be specified with the num_classes parameter. By default, it is set 
-    to 2, but it can be set to any integer greater than or equal to 1. 
-
-    The function uses a list of labels and colour codes to create the classification data for 
-    the output dictionaries. The labels and colour codes are stored in the label_dict and 
-    colour_dict lists, respectively. The label_dict list contains the names of the labels and 
-    the colour_dict list contains the corresponding RGB colour codes for each label. By default, 
-    the label_dict list contains the values ["background", "non-tumour", "tumour", "segmented"] 
-    and the colour_dict list contains the value [-9408287, -9408287, -9408287, -9408287]. If 
-    the num_classes parameter is set to a value other than 2, the label_dict list is updated 
-    to contain the values ["background", "Class1", "Class2", ..., "ClassN"], where N is the 
-    number of classes, and the colour_dict list is updated to contain the value 
+    This function converts a list of contours and their labels to a list of dictionaries
+    containing GeoJSON-formatted data. The function expects the contours to be a list of
+    pairs (contour, label), where contour is a list of points starting and finishing in the
+    same point, and label is an integer representing the class of the cell (1: non-tumour,
+    2: tumour).
+
+    The function returns a list of dictionaries with the GeoJSON format of QuPath. The
+    number of classes can be specified with the num_classes parameter. By default, it is set
+    to 2, but it can be set to any integer greater than or equal to 1.
+
+    The function uses a list of labels and colour codes to create the classification data for
+    the output dictionaries. The labels and colour codes are stored in the label_dict and
+    colour_dict lists, respectively. The label_dict list contains the names of the labels and
+    the colour_dict list contains the corresponding RGB colour codes for each label. By default,
+    the label_dict list contains the values ["background", "non-tumour", "tumour", "segmented"]
+    and the colour_dict list contains the value [-9408287, -9408287, -9408287, -9408287]. If
+    the num_classes parameter is set to a value other than 2, the label_dict list is updated
+    to contain the values ["background", "Class1", "Class2", ..., "ClassN"], where N is the
+    number of classes, and the colour_dict list is updated to contain the value
     [-9408287, ..., -9408287] where the length of the list is N+1. Although this list is
     superfluous and not used by QuPath.
 
-    Each dictionary in the output list represents a cell contour and contains a Polygon 
-    object with the contour points, a classification object with the name and colour of the 
-    label, and a boolean indicating whether the object is locked. The dictionary is in the 
+    Each dictionary in the output list represents a cell contour and contains a Polygon
+    object with the contour points, a classification object with the name and colour of the
+    label, and a boolean indicating whether the object is locked. The dictionary is in the
     format expected by QuPath for reading annotations.
     """
     label_dict = ["background", "non-tumour", "tumour", "segmented"]
     colour_dict = [-9408287, -9408287, -9408287, -9408287]
     if num_classes != 2:
-        label_dict = ["background"] + ["Class" + str(i) for i in range(1, num_classes+1)]
+        label_dict = ["background"] + ["Class" + str(i) for i in range(1, num_classes + 1)]
     colour_dict = [-9408287] * (num_classes + 1)
     features = []
     for contour, label in contours:
-        assert(label > 0)
+        assert (label > 0)
         points = Polygon([contour])
         properties = {
-                    "object_type": "annotation",
-                    "classification": {
-                        "name": label_dict[label],
-                        "colorRGB": colour_dict[label]
-                    },
-                    "isLocked": False
-                    }
+            "object_type": "annotation",
+            "classification": {
+                "name": label_dict[label],
+                "colorRGB": colour_dict[label]
+            },
+            "isLocked": False
+        }
         feat = Feature(geometry=points, properties=properties)
         features.append(feat)
     return features
 
 
 def save_png(png: np.ndarray, png_path: str, name: str) -> None:
     """
@@ -369,15 +375,15 @@
     :param centroids: The centroids to save.
     :type centroids: np.ndarray
     :param centroids_dir: The directory to save the centroids in.
     :type centroids_dir: str
     :param name: The base name for the file (without extensions).
     :type name: str
     """
-    df = pd.DataFrame(centroids, columns=['X','Y','class'])
+    df = pd.DataFrame(centroids, columns=['X', 'Y', 'class'])
     df.to_csv(os.path.join(centroids_dir, name + '.centroids.csv'), index=False)
 
 
 def save_graph(graph: pd.DataFrame, path: str) -> None:
     """
     Saves the given graph as a CSV file to the specified path.
 
@@ -407,15 +413,15 @@
         geojson.dump(gson, f, sort_keys=True, indent=2)
 
 
 def get_centroid_by_id(img: np.ndarray, idx: int) -> Tuple[int, int]:
     """
     Given an image and an id representing a component, returns the centroid
     of the component as a tuple (x, y).
-    
+
     :param img: A NumPy array representing the image.
     :type img: np.ndarray
     :param idx: An integer representing the id of the component.
     :type idx: int
     :return: A tuple representing the centroid of the component.
     :rtype: Tuple[int, int]
 
@@ -436,16 +442,16 @@
     :type png: np.ndarray
     :param idx: Index of the mask to retrieve.
     :type idx: int
     :return: The mask corresponding to the given index.
     :rtype: np.ndarray
     """
     png_aux = png.copy()
-    png_aux[png_aux!=idx] = 0
-    png_aux[png_aux!=0] = 1
+    png_aux[png_aux != idx] = 0
+    png_aux[png_aux != 0] = 1
     return png_aux
 
 
 def apply_mask(img: np.ndarray, mask: np.ndarray) -> Tuple[np.ndarray, int, int]:
     """
     Apply a binary mask to an RGB image.
 
@@ -457,36 +463,36 @@
     :rtype: Tuple[np.ndarray, np.ndarray, int, int]
 
     For efficiency only the bounded box of the mask is returned, together with the center of the box.
     Coordinates are indices of array.
     """
     img_aux = img.copy()
     img_aux = img_aux * mask.reshape(*mask.shape, 1)
-    x,y,w,h = cv2.boundingRect((mask * 255).astype(np.uint8))
+    x, y, w, h = cv2.boundingRect((mask * 255).astype(np.uint8))
     X, Y = np.where(mask == 1)
     if len(X) == 0 or len(Y) == 0:
         cx, cy = -1, -1
     else:
         cx, cy = X.mean(), Y.mean()
-    return img_aux[y:y+h, x:x+w].copy(), mask[y:y+h, x:x+w].copy(), cx, cy
+    return img_aux[y:y + h, x:x + w].copy(), mask[y:y + h, x:x + w].copy(), cx, cy
 
 
 def read_image(name: str, path: str) -> np.array:
     """
     Given name image (without extension) and folder path,
     returns array with pixel values (RGB).
 
     :param name: Name of the image (without extension).
     :type name: str
     :param path: Path to the folder where the image is located.
     :type path: str
     :return: Array with pixel values (RGB).
     :rtype: np.array
     """
-    aux = cv2.imread(os.path.join(path, name+'.png'))
+    aux = cv2.imread(os.path.join(path, name + '.png'))
     return cv2.cvtColor(aux, cv2.COLOR_BGR2RGB)
 
 
 def compute_perimeter(c: Contour) -> float:
     """
     Compute the perimeter of a given contour.
     Prerequisites: First and last point must be the same.
@@ -494,15 +500,15 @@
     :param c: Contour represented as a list of points (x,y).
               The first and last point must be the same.
     :type c: List[Tuple[float, float]]
     :return: The perimeter of the contour.
     :rtype: float
     """
     diff = np.diff(c, axis=0)
-    dists = np.hypot(diff[:,0], diff[:,1])
+    dists = np.hypot(diff[:, 0], diff[:, 1])
     return dists.sum()
 
 
 def extract_features(msk_img: np.ndarray, bin_msk: np.ndarray, debug=False) -> Dict[str, np.ndarray]:
     """
     Extracts features from a given RGB bounding box of a cell and its mask.
 
@@ -518,37 +524,39 @@
     if len(msk_img) == 0 or msk_img.max() == 0:
         return {}
     gray_msk = cv2.cvtColor(msk_img, cv2.COLOR_RGB2GRAY)
     # bin_msk = (gray_msk > 0) * 1
     feats = {}
     feats['area'] = bin_msk.sum()
 
-    if debug: import pdb; pdb.set_trace()
+    if debug:
+        import pdb
+        pdb.set_trace()
     contours, _ = cv2.findContours(
-        (bin_msk * 255).astype(np.uint8), 
+        (bin_msk * 255).astype(np.uint8),
         mode=cv2.RETR_TREE, method=cv2.CHAIN_APPROX_SIMPLE
     )
     contour = format_contour(contours[0])
     feats['perimeter'] = compute_perimeter(contour)
-    
+
     gray_msk = ma.masked_array(
-        gray_msk, mask=1-bin_msk
+        gray_msk, mask=1 - bin_msk
     )
     feats['std'] = gray_msk.std()
 
     msk_img = ma.masked_array(
-        msk_img, mask=1-np.repeat(bin_msk.reshape((*bin_msk.shape,1)), 3, axis=2)
+        msk_img, mask=1 - np.repeat(bin_msk.reshape((*bin_msk.shape, 1)), 3, axis=2)
     )
-    red = msk_img[:,:,0].compressed()
+    red = msk_img[:, :, 0].compressed()
     red_bins, _ = np.histogram(red, bins=5, density=True)
     feats['red'] = red_bins
-    green = msk_img[:,:,1].compressed()
+    green = msk_img[:, :, 1].compressed()
     green_bins, _ = np.histogram(green, bins=5, density=True)
     feats['green'] = green_bins
-    blue = msk_img[:,:,2].compressed()
+    blue = msk_img[:, :, 2].compressed()
     blue_bins, _ = np.histogram(blue, bins=5, density=True)
     feats['blue'] = blue_bins
     return feats
 
 
 def add_node(graph: Dict[str, float], feats: Dict[str, np.ndarray]) -> None:
     """
@@ -556,19 +564,19 @@
     converts them into one column per dimension
     and add them into the global dictionary.
 
     :param graph: Dictionary with graph node data.
     :type graph: Dict[str, float]
     :param feats: Dictionary with vectorial features of a graph node.
     :type feats: Dict[str, np.ndarray]
-    :return: None. The graph dictionary is modified in place.    
+    :return: None. The graph dictionary is modified in place.
     """
     for k, v in feats.items():
         if hasattr(v, '__len__'):
             for i, coord in enumerate(v):
                 if k + str(i) not in graph:
                     graph[k + str(i)] = []
                 graph[k + str(i)].append(coord)
         else:
             if k not in graph:
                 graph[k] = []
-            graph[k].append(v)
+            graph[k].append(v)
```

### Comparing `tumourkit-0.6.0/tumourkit/utils/read_nodes.py` & `tumourkit-0.7.0/tumourkit/utils/read_nodes.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,15 +40,18 @@
     Centroids coordinates are removed.
     Labels are subtracted 1 to be in 0-1 range.
     """
     df = pd.read_csv(file)
     remove_vars = ['id', 'class', 'X', 'Y']
     if remove_morph:
         remove_vars.extend([
-            'area','perimeter','std','red0','red1','red2','red3','red4','green0','green1','green2','green3','green4','blue0','blue1','blue2','blue3','blue4'
+            'area', 'perimeter', 'std',
+            'red0', 'red1', 'red2', 'red3', 'red4',
+            'green0', 'green1', 'green2', 'green3', 'green4',
+            'blue0', 'blue1', 'blue2', 'blue3', 'blue4'
         ])
     if remove_prior:
         remove_vars.extend(list(filter(lambda x: 'prob' in x, df.columns)))
     if return_class:
         y = df['class'].to_numpy() - 1
         X = df.drop(remove_vars, axis=1).to_numpy()
         if remove_morph and remove_prior:
@@ -67,14 +70,15 @@
         if not return_coordinates:
             return X, None
         else:
             xx = df['X'].to_numpy()
             yy = df['Y'].to_numpy()
             return X, None, xx, yy
 
+
 def _read_all_nodes(
         node_dir: str,
         names: List[str],
         remove_prior: Optional[bool] = False,
         remove_morph: Optional[bool] = False,
         ) -> List[np.ndarray]:
     """
@@ -84,17 +88,17 @@
     Output
       X: Input data in array format.
       y: Labels in array format.
     """
     X, y = None, None
     for name in names:
         X_, y_ = read_node_matrix(os.path.join(node_dir, name), remove_morph=remove_morph, remove_prior=remove_prior)
-        if X is None: 
-            X = X_ # Shape (n_samples, n_features)
-            y = y_ # Shape (n_samples,)
+        if X is None:
+            X = X_  # Shape (n_samples, n_features)
+            y = y_  # Shape (n_samples,)
         else:
             X = np.vstack([X, X_])
             y = np.hstack([y, y_])
     return X, y
 
 
 def read_all_nodes(
@@ -107,55 +111,56 @@
       node_dir: Path to folder with csv files containing node features.
     Output
       X: Input data in array format.
       y: Labels in array format.
     """
     ext = '.nodes.csv'
     names = get_names(node_dir, ext)
-    names = [x+ext for x in names]
+    names = [x + ext for x in names]
     X, y = _read_all_nodes(node_dir, names, remove_morph=remove_morph, remove_prior=remove_prior)
     return X, y
 
 
 def create_node_splits(
-    node_dir: str, val_size: float, test_size: float, 
-    seed: Optional[int] = None,
-    mode: Optional[str] = 'total') -> List[np.ndarray]:
+        node_dir: str, val_size: float, test_size: float,
+        seed: Optional[int] = None,
+        mode: Optional[str] = 'total'
+        ) -> List[np.ndarray]:
     """
     Input
       node_dir: Path to folder with csv files containing node features.
       val_size: Percentage of data to use as validation.
       test_size: Percentage of data to use as test.
       seed: Seed for the random split.
-      mode: Whether to mix images in the splits or not. It can be 'total' or 'by_img'. 
+      mode: Whether to mix images in the splits or not. It can be 'total' or 'by_img'.
     Output
       X_train, X_val, X_test, y_train, y_val, y_test: Node features and labels.
     """
     ext = '.nodes.csv'
     names = get_names(node_dir, ext)
-    names = [x+ext for x in names]
+    names = [x + ext for x in names]
     if mode == 'total':
         X, y = _read_all_nodes(node_dir, names)
         X_tr_val, X_test, y_tr_val, y_test = train_test_split(
             X, y, test_size=test_size, stratify=y, random_state=seed
         )
         X_train, X_val, y_train, y_val = train_test_split(
-            X_tr_val, y_tr_val, test_size=val_size / (1-test_size), 
+            X_tr_val, y_tr_val, test_size=val_size / (1 - test_size),
             stratify=y_tr_val, random_state=seed
         )
         return X_train, X_val, X_test, y_train, y_val, y_test
     elif mode == 'by_img':
         random.seed(seed)
         random.shuffle(names)
         N = len(names)
         N_ts = int(N * test_size)
         N_val = int(N * val_size)
         N_tr = N - N_val - N_ts
         train_names = names[:N_tr]
-        val_names = names[N_tr:N_val+N_tr]
-        test_names = names[N_val+N_tr:]
+        val_names = names[N_tr:N_val + N_tr]
+        test_names = names[N_val + N_tr:]
         X_train, y_train = _read_all_nodes(node_dir, train_names)
         X_val, y_val = _read_all_nodes(node_dir, val_names)
         X_test, y_test = _read_all_nodes(node_dir, test_names)
         return X_train, X_val, X_test, y_train, y_val, y_test
     else:
-        assert False, 'Wrong mode.'
+        assert False, 'Wrong mode.'
```

### Comparing `tumourkit-0.6.0/tumourkit.egg-info/PKG-INFO` & `tumourkit-0.7.0/tumourkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumourkit
-Version: 0.6.0
+Version: 0.7.0
 Summary: A SDK for tumour study
 Author-email: Jose Pérez Cano <joseperez2000@hotmail.es>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `tumourkit-0.6.0/tumourkit.egg-info/SOURCES.txt` & `tumourkit-0.7.0/tumourkit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 tumourkit/classification/models/gat.py
 tumourkit/classification/models/gcn.py
 tumourkit/classification/models/hgao.py
 tumourkit/classification/models/norm.py
 tumourkit/demo/app.py
 tumourkit/postprocessing/__init__.py
 tumourkit/postprocessing/draw_cells.py
+tumourkit/postprocessing/draw_graph.py
 tumourkit/postprocessing/join_graph_gt.py
 tumourkit/postprocessing/join_hovprob_graph.py
 tumourkit/postprocessing/merge_cells.py
 tumourkit/postprocessing/rswoosh.py
 tumourkit/preprocessing/__init__.py
 tumourkit/preprocessing/centroids2png.py
 tumourkit/preprocessing/centroidspng2csv.py
```

### Comparing `tumourkit-0.6.0/tumourkit.egg-info/entry_points.txt` & `tumourkit-0.7.0/tumourkit.egg-info/entry_points.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [console_scripts]
 centroids2png = tumourkit.preprocessing.centroids2png:main
 centroidspng2csv = tumourkit.preprocessing.centroidspng2csv:main
 draw_cells = tumourkit.postprocessing.draw_cells:main
+draw_graph = tumourkit.postprocessing.draw_graph:main
 geojson2pngcsv = tumourkit.preprocessing.geojson2pngcsv:main
 graph2centroids = tumourkit.preprocessing.graph2centroids:main
 hovernet2centroids = tumourkit.preprocessing.hovernet2centroids:main
 hovernet2geojson = tumourkit.preprocessing.hovernet2geojson:main
 make_dirs = tumourkit.make_dirs:main
 merge_cells = tumourkit.postprocessing.merge_cells:main
 pngcsv2centroids = tumourkit.preprocessing.pngcsv2centroids:main
```

### Comparing `tumourkit-0.6.0/tumourkit.egg-info/requires.txt` & `tumourkit-0.7.0/tumourkit.egg-info/requires.txt`

 * *Files identical despite different names*

