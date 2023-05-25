# Comparing `tmp/pyg_nightly-2.4.0.dev20230524.tar.gz` & `tmp/pyg_nightly-2.4.0.dev20230525.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyg_nightly-2.4.0.dev20230524.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyg_nightly-2.4.0.dev20230525.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyg_nightly-2.4.0.dev20230524.tar` & `pyg_nightly-2.4.0.dev20230525.tar`

### file list

```diff
@@ -1,550 +1,551 @@
--rw-r--r--   0        0        0    60889 2023-05-24 06:05:41.012045 pyg_nightly-2.4.0.dev20230524/README.md
--rw-r--r--   0        0        0     4073 2023-05-24 06:05:41.392044 pyg_nightly-2.4.0.dev20230524/pyproject.toml
--rw-r--r--   0        0        0     1055 2023-05-24 06:05:41.388044 pyg_nightly-2.4.0.dev20230524/torch_geometric/__init__.py
--rw-r--r--   0        0        0     3392 2023-05-24 06:05:41.048045 pyg_nightly-2.4.0.dev20230524/torch_geometric/compile.py
--rw-r--r--   0        0        0      352 2023-05-24 06:05:41.048045 pyg_nightly-2.4.0.dev20230524/torch_geometric/contrib/__init__.py
--rw-r--r--   0        0        0       23 2023-05-24 06:05:41.048045 pyg_nightly-2.4.0.dev20230524/torch_geometric/contrib/datasets/__init__.py
--rw-r--r--   0        0        0      163 2023-05-24 06:05:41.048045 pyg_nightly-2.4.0.dev20230524/torch_geometric/contrib/explain/__init__.py
--rw-r--r--   0        0        0    20540 2023-05-24 06:05:41.048045 pyg_nightly-2.4.0.dev20230524/torch_geometric/contrib/explain/graphmask_explainer.py
--rw-r--r--   0        0        0    16627 2023-05-24 06:05:41.048045 pyg_nightly-2.4.0.dev20230524/torch_geometric/contrib/explain/pgm_explainer.py
--rw-r--r--   0        0        0       72 2023-05-24 06:05:41.048045 pyg_nightly-2.4.0.dev20230524/torch_geometric/contrib/nn/__init__.py
--rw-r--r--   0        0        0       23 2023-05-24 06:05:41.048045 pyg_nightly-2.4.0.dev20230524/torch_geometric/contrib/nn/conv/__init__.py
--rw-r--r--   0        0        0      113 2023-05-24 06:05:41.048045 pyg_nightly-2.4.0.dev20230524/torch_geometric/contrib/nn/models/__init__.py
--rw-r--r--   0        0        0    33261 2023-05-24 06:05:41.048045 pyg_nightly-2.4.0.dev20230524/torch_geometric/contrib/nn/models/rbcd_attack.py
--rw-r--r--   0        0        0       23 2023-05-24 06:05:41.048045 pyg_nightly-2.4.0.dev20230524/torch_geometric/contrib/transforms/__init__.py
--rw-r--r--   0        0        0     3383 2023-05-24 06:05:41.048045 pyg_nightly-2.4.0.dev20230524/torch_geometric/data/__init__.py
--rw-r--r--   0        0        0     7428 2023-05-24 06:05:41.048045 pyg_nightly-2.4.0.dev20230524/torch_geometric/data/batch.py
--rw-r--r--   0        0        0    10658 2023-05-24 06:05:41.048045 pyg_nightly-2.4.0.dev20230524/torch_geometric/data/collate.py
--rw-r--r--   0        0        0    37655 2023-05-24 06:05:41.048045 pyg_nightly-2.4.0.dev20230524/torch_geometric/data/data.py
--rw-r--r--   0        0        0     2922 2023-05-24 06:05:41.048045 pyg_nightly-2.4.0.dev20230524/torch_geometric/data/datapipes.py
--rw-r--r--   0        0        0    14850 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/data/dataset.py
--rw-r--r--   0        0        0     1359 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/data/download.py
--rw-r--r--   0        0        0     2252 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/data/extract.py
--rw-r--r--   0        0        0    21075 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/data/feature_store.py
--rw-r--r--   0        0        0    13495 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/data/graph_store.py
--rw-r--r--   0        0        0    44236 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/data/hetero_data.py
--rw-r--r--   0        0        0     7750 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/data/in_memory_dataset.py
--rw-r--r--   0        0        0      178 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/data/lightning/__init__.py
--rw-r--r--   0        0        0    28490 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/data/lightning/datamodule.py
--rw-r--r--   0        0        0      338 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/data/makedirs.py
--rw-r--r--   0        0        0     3962 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/data/remote_backend_utils.py
--rw-r--r--   0        0        0     4360 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/data/separate.py
--rw-r--r--   0        0        0    25245 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/data/storage.py
--rw-r--r--   0        0        0     5219 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/data/summary.py
--rw-r--r--   0        0        0     9354 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/data/temporal.py
--rw-r--r--   0        0        0     1038 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/data/view.py
--rw-r--r--   0        0        0     5051 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/__init__.py
--rw-r--r--   0        0        0     4220 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/actor.py
--rw-r--r--   0        0        0     5584 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/airfrans.py
--rw-r--r--   0        0        0     3711 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/airports.py
--rw-r--r--   0        0        0     3050 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/amazon.py
--rw-r--r--   0        0        0     4099 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/amazon_products.py
--rw-r--r--   0        0        0     4942 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/aminer.py
--rw-r--r--   0        0        0     5266 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/aqsol.py
--rw-r--r--   0        0        0     5735 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/attributed_graph_dataset.py
--rw-r--r--   0        0        0     4063 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/ba2motif_dataset.py
--rw-r--r--   0        0        0     3518 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/ba_multi_shapes.py
--rw-r--r--   0        0        0     3824 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/ba_shapes.py
--rw-r--r--   0        0        0     4137 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/bitcoin_otc.py
--rw-r--r--   0        0        0     4205 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/citation_full.py
--rw-r--r--   0        0        0     3009 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/coauthor.py
--rw-r--r--   0        0        0     4564 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/coma.py
--rw-r--r--   0        0        0     5192 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/dblp.py
--rw-r--r--   0        0        0     5608 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/dbp15k.py
--rw-r--r--   0        0        0     2308 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/deezer_europe.py
--rw-r--r--   0        0        0     3862 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/dgraph.py
--rw-r--r--   0        0        0     5865 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/dynamic_faust.py
--rw-r--r--   0        0        0     4498 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/elliptic.py
--rw-r--r--   0        0        0     2990 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/elliptic_temporal.py
--rw-r--r--   0        0        0     2631 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/email_eu_core.py
--rw-r--r--   0        0        0     7001 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/entities.py
--rw-r--r--   0        0        0     5817 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/explainer_dataset.py
--rw-r--r--   0        0        0     2228 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/facebook.py
--rw-r--r--   0        0        0    10215 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/fake.py
--rw-r--r--   0        0        0     3924 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/faust.py
--rw-r--r--   0        0        0     4099 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/flickr.py
--rw-r--r--   0        0        0     3815 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/freebase.py
--rw-r--r--   0        0        0     3416 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/gdelt.py
--rw-r--r--   0        0        0     9261 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/ged_dataset.py
--rw-r--r--   0        0        0     2626 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/gemsec.py
--rw-r--r--   0        0        0     3954 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/geometry.py
--rw-r--r--   0        0        0     2484 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/github.py
--rw-r--r--   0        0        0     6762 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/gnn_benchmark_dataset.py
--rw-r--r--   0        0        0      221 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/graph_generator/__init__.py
--rw-r--r--   0        0        0      965 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/graph_generator/ba_graph.py
--rw-r--r--   0        0        0      949 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/graph_generator/base.py
--rw-r--r--   0        0        0      918 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/graph_generator/er_graph.py
--rw-r--r--   0        0        0     1159 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/graph_generator/grid_graph.py
--rw-r--r--   0        0        0     4043 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/heterophilous_graph_dataset.py
--rw-r--r--   0        0        0     8467 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/hgb_dataset.py
--rw-r--r--   0        0        0    11053 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/hydro_net.py
--rw-r--r--   0        0        0     4447 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/icews.py
--rw-r--r--   0        0        0     4000 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/imdb.py
--rw-r--r--   0        0        0     7169 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/infection_dataset.py
--rw-r--r--   0        0        0     3439 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/jodie.py
--rw-r--r--   0        0        0     3444 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/karate.py
--rw-r--r--   0        0        0     4349 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/last_fm.py
--rw-r--r--   0        0        0     2283 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/lastfm_asia.py
--rw-r--r--   0        0        0     6582 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/linkx_dataset.py
--rw-r--r--   0        0        0    11559 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/lrgb.py
--rw-r--r--   0        0        0     5044 2023-05-24 06:05:41.052045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/malnet_tiny.py
--rw-r--r--   0        0        0    16482 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/md17.py
--rw-r--r--   0        0        0     3770 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/mixhop_synthetic_dataset.py
--rw-r--r--   0        0        0     3136 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/mnist_superpixels.py
--rw-r--r--   0        0        0     5251 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/modelnet.py
--rw-r--r--   0        0        0     6593 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/molecule_net.py
--rw-r--r--   0        0        0      227 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/motif_generator/__init__.py
--rw-r--r--   0        0        0      910 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/motif_generator/base.py
--rw-r--r--   0        0        0     1203 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/motif_generator/custom.py
--rw-r--r--   0        0        0      984 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/motif_generator/cycle.py
--rw-r--r--   0        0        0      801 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/motif_generator/house.py
--rw-r--r--   0        0        0     3787 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/movie_lens.py
--rw-r--r--   0        0        0     6005 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/movie_lens_100k.py
--rw-r--r--   0        0        0     2889 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/nell.py
--rw-r--r--   0        0        0     7190 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/ogb_mag.py
--rw-r--r--   0        0        0     3415 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/omdb.py
--rw-r--r--   0        0        0     3964 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/particle.py
--rw-r--r--   0        0        0    10699 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/pascal.py
--rw-r--r--   0        0        0     4602 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/pascal_pf.py
--rw-r--r--   0        0        0     5716 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/pcpnet_dataset.py
--rw-r--r--   0        0        0     6975 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/planetoid.py
--rw-r--r--   0        0        0     2842 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/polblogs.py
--rw-r--r--   0        0        0     4866 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/ppi.py
--rw-r--r--   0        0        0     3182 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/qm7.py
--rw-r--r--   0        0        0    16813 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/qm9.py
--rw-r--r--   0        0        0     2941 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/reddit.py
--rw-r--r--   0        0        0     4439 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/reddit2.py
--rw-r--r--   0        0        0     4345 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/rel_link_pred_dataset.py
--rw-r--r--   0        0        0     4173 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/s3dis.py
--rw-r--r--   0        0        0     8140 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/sbm_dataset.py
--rw-r--r--   0        0        0     8088 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/shapenet.py
--rw-r--r--   0        0        0     6150 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/shrec2016.py
--rw-r--r--   0        0        0     9283 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/snap_dataset.py
--rw-r--r--   0        0        0     3031 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/suite_sparse.py
--rw-r--r--   0        0        0     3959 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/taobao.py
--rw-r--r--   0        0        0     4451 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/tosca.py
--rw-r--r--   0        0        0     7302 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/tu_dataset.py
--rw-r--r--   0        0        0     3464 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/twitch.py
--rw-r--r--   0        0        0     6929 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/upfd.py
--rw-r--r--   0        0        0      182 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/utils/__init__.py
--rw-r--r--   0        0        0     1732 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/utils/cheatsheet.py
--rw-r--r--   0        0        0     4615 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/webkb.py
--rw-r--r--   0        0        0     3674 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/wikics.py
--rw-r--r--   0        0        0     6083 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/wikipedia_network.py
--rw-r--r--   0        0        0     6322 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/willow_object_class.py
--rw-r--r--   0        0        0     7857 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/word_net.py
--rw-r--r--   0        0        0     4116 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/yelp.py
--rw-r--r--   0        0        0     6171 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/zinc.py
--rw-r--r--   0        0        0     1197 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/debug.py
--rw-r--r--   0        0        0      748 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/deprecation.py
--rw-r--r--   0        0        0     2466 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/experimental.py
--rw-r--r--   0        0        0      359 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/__init__.py
--rw-r--r--   0        0        0      418 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/algorithm/__init__.py
--rw-r--r--   0        0        0     4491 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/algorithm/attention_explainer.py
--rw-r--r--   0        0        0     6899 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/algorithm/base.py
--rw-r--r--   0        0        0    12489 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/algorithm/captum.py
--rw-r--r--   0        0        0     6530 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/algorithm/captum_explainer.py
--rw-r--r--   0        0        0     2867 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/algorithm/dummy_explainer.py
--rw-r--r--   0        0        0    11149 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/algorithm/gnn_explainer.py
--rw-r--r--   0        0        0    10370 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/algorithm/pg_explainer.py
--rw-r--r--   0        0        0     2308 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/algorithm/utils.py
--rw-r--r--   0        0        0     7834 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/config.py
--rw-r--r--   0        0        0    10375 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/explainer.py
--rw-r--r--   0        0        0    14842 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/explanation.py
--rw-r--r--   0        0        0      301 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/metric/__init__.py
--rw-r--r--   0        0        0     1888 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/metric/basic.py
--rw-r--r--   0        0        0     3063 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/metric/faithfulness.py
--rw-r--r--   0        0        0     6157 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/metric/fidelity.py
--rw-r--r--   0        0        0     2045 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/__init__.py
--rw-r--r--   0        0        0      510 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/benchmark.py
--rw-r--r--   0        0        0     2371 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/checkpoint.py
--rw-r--r--   0        0        0      738 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/cmd_args.py
--rw-r--r--   0        0        0    17221 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/config.py
--rw-r--r--   0        0        0    14575 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/config_store.py
--rw-r--r--   0        0        0      389 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/contrib/__init__.py
--rw-r--r--   0        0        0      221 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/contrib/act/__init__.py
--rw-r--r--   0        0        0      221 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/contrib/config/__init__.py
--rw-r--r--   0        0        0      221 2023-05-24 06:05:41.056045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/contrib/encoder/__init__.py
--rw-r--r--   0        0        0      221 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/contrib/head/__init__.py
--rw-r--r--   0        0        0      221 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/contrib/layer/__init__.py
--rw-r--r--   0        0        0     8304 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/contrib/layer/generalconv.py
--rw-r--r--   0        0        0      221 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/contrib/loader/__init__.py
--rw-r--r--   0        0        0      221 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/contrib/loss/__init__.py
--rw-r--r--   0        0        0      221 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/contrib/network/__init__.py
--rw-r--r--   0        0        0      221 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/contrib/optimizer/__init__.py
--rw-r--r--   0        0        0      221 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/contrib/pooling/__init__.py
--rw-r--r--   0        0        0      221 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/contrib/stage/__init__.py
--rw-r--r--   0        0        0      221 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/contrib/train/__init__.py
--rw-r--r--   0        0        0      221 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/contrib/transform/__init__.py
--rw-r--r--   0        0        0      375 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/imports.py
--rw-r--r--   0        0        0      490 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/init.py
--rw-r--r--   0        0        0    11763 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/loader.py
--rw-r--r--   0        0        0    11329 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/logger.py
--rw-r--r--   0        0        0     1474 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/loss.py
--rw-r--r--   0        0        0     3110 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/model_builder.py
--rw-r--r--   0        0        0     1121 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/models/__init__.py
--rw-r--r--   0        0        0      822 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/models/act.py
--rw-r--r--   0        0        0     2546 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/models/encoder.py
--rw-r--r--   0        0        0     5133 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/models/gnn.py
--rw-r--r--   0        0        0     4434 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/models/head.py
--rw-r--r--   0        0        0    12486 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/models/layer.py
--rw-r--r--   0        0        0      288 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/models/pooling.py
--rw-r--r--   0        0        0     1391 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/models/transform.py
--rw-r--r--   0        0        0     2544 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/optim.py
--rw-r--r--   0        0        0     3944 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/register.py
--rw-r--r--   0        0        0     1887 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/train.py
--rw-r--r--   0        0        0        0 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/utils/LICENSE
--rw-r--r--   0        0        0      641 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/utils/__init__.py
--rw-r--r--   0        0        0     9513 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/utils/agg_runs.py
--rw-r--r--   0        0        0     3056 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/utils/comp_budget.py
--rw-r--r--   0        0        0     1352 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/utils/device.py
--rw-r--r--   0        0        0      690 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/utils/epoch.py
--rw-r--r--   0        0        0     2050 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/utils/io.py
--rw-r--r--   0        0        0      606 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/utils/plot.py
--rw-r--r--   0        0        0      198 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/utils/tools.py
--rw-r--r--   0        0        0      830 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/home.py
--rw-r--r--   0        0        0      528 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/io/__init__.py
--rw-r--r--   0        0        0     1148 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/io/npz.py
--rw-r--r--   0        0        0      957 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/io/obj.py
--rw-r--r--   0        0        0     2586 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/io/off.py
--rw-r--r--   0        0        0     4211 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/io/planetoid.py
--rw-r--r--   0        0        0      476 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/io/ply.py
--rw-r--r--   0        0        0     1136 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/io/sdf.py
--rw-r--r--   0        0        0     4733 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/io/tu.py
--rw-r--r--   0        0        0      562 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/io/txt_array.py
--rw-r--r--   0        0        0      768 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/lazy_loader.py
--rw-r--r--   0        0        0     1675 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/__init__.py
--rw-r--r--   0        0        0     1433 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/base.py
--rw-r--r--   0        0        0     6910 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/cluster.py
--rw-r--r--   0        0        0     1449 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/data_list_loader.py
--rw-r--r--   0        0        0     3222 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/dataloader.py
--rw-r--r--   0        0        0     1683 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/dense_data_loader.py
--rw-r--r--   0        0        0     4285 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/dynamic_batch_sampler.py
--rw-r--r--   0        0        0     8448 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/graph_saint.py
--rw-r--r--   0        0        0     6012 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/hgt_loader.py
--rw-r--r--   0        0        0     3754 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/imbalanced_sampler.py
--rw-r--r--   0        0        0    13948 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/link_loader.py
--rw-r--r--   0        0        0    12513 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/link_neighbor_loader.py
--rw-r--r--   0        0        0     6317 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/mixin.py
--rw-r--r--   0        0        0    11382 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/neighbor_loader.py
--rw-r--r--   0        0        0     8513 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/neighbor_sampler.py
--rw-r--r--   0        0        0     9365 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/node_loader.py
--rw-r--r--   0        0        0     2141 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/prefetch.py
--rw-r--r--   0        0        0     2196 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/random_node_loader.py
--rw-r--r--   0        0        0     4173 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/shadow.py
--rw-r--r--   0        0        0     1319 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/temporal_dataloader.py
--rw-r--r--   0        0        0    12273 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/utils.py
--rw-r--r--   0        0        0     3518 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/zip_loader.py
--rw-r--r--   0        0        0      832 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/logging.py
--rw-r--r--   0        0        0      911 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/__init__.py
--rw-r--r--   0        0        0     1397 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/__init__.py
--rw-r--r--   0        0        0     2395 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/attention.py
--rw-r--r--   0        0        0     7106 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/base.py
--rw-r--r--   0        0        0    11000 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/basic.py
--rw-r--r--   0        0        0     2064 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/deep_sets.py
--rw-r--r--   0        0        0     6881 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/equilibrium.py
--rw-r--r--   0        0        0    12229 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/fused.py
--rw-r--r--   0        0        0     3062 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/gmt.py
--rw-r--r--   0        0        0     1464 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/gru.py
--rw-r--r--   0        0        0     1484 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/lstm.py
--rw-r--r--   0        0        0     1995 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/mlp.py
--rw-r--r--   0        0        0     8163 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/multi.py
--rw-r--r--   0        0        0     6098 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/quantile.py
--rw-r--r--   0        0        0     4642 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/scaler.py
--rw-r--r--   0        0        0     2517 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/set2set.py
--rw-r--r--   0        0        0     3439 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/set_transformer.py
--rw-r--r--   0        0        0     1921 2023-05-24 06:05:41.060045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/sort.py
--rw-r--r--   0        0        0     8322 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/utils.py
--rw-r--r--   0        0        0     3360 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/__init__.py
--rw-r--r--   0        0        0     3088 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/agnn_conv.py
--rw-r--r--   0        0        0     4388 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/antisymmetric_conv.py
--rw-r--r--   0        0        0     6010 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/appnp.py
--rw-r--r--   0        0        0     6637 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/arma_conv.py
--rw-r--r--   0        0        0     4036 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/cg_conv.py
--rw-r--r--   0        0        0     6444 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/cheb_conv.py
--rw-r--r--   0        0        0     5303 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/cluster_gcn_conv.py
--rw-r--r--   0        0        0      251 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/cugraph/__init__.py
--rw-r--r--   0        0        0     8195 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/cugraph/base.py
--rw-r--r--   0        0        0     2849 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/cugraph/gat_conv.py
--rw-r--r--   0        0        0     4218 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/cugraph/rgcn_conv.py
--rw-r--r--   0        0        0     2802 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/cugraph/sage_conv.py
--rw-r--r--   0        0        0    12105 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/dna_conv.py
--rw-r--r--   0        0        0     5550 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/edge_conv.py
--rw-r--r--   0        0        0    10482 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/eg_conv.py
--rw-r--r--   0        0        0     7927 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/fa_conv.py
--rw-r--r--   0        0        0     4453 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/feast_conv.py
--rw-r--r--   0        0        0     6332 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/film_conv.py
--rw-r--r--   0        0        0     4242 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/fused_gat_conv.py
--rw-r--r--   0        0        0    13610 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/gat_conv.py
--rw-r--r--   0        0        0     3582 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/gated_graph_conv.py
--rw-r--r--   0        0        0    12423 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/gatv2_conv.py
--rw-r--r--   0        0        0     7022 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/gcn2_conv.py
--rw-r--r--   0        0        0     9333 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/gcn_conv.py
--rw-r--r--   0        0        0     9992 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/gen_conv.py
--rw-r--r--   0        0        0     7512 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/general_conv.py
--rw-r--r--   0        0        0     7444 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/gin_conv.py
--rw-r--r--   0        0        0     8320 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/gmm_conv.py
--rw-r--r--   0        0        0     5764 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/gps_conv.py
--rw-r--r--   0        0        0     3547 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/graph_conv.py
--rw-r--r--   0        0        0     5023 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/gravnet_conv.py
--rw-r--r--   0        0        0     7354 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/han_conv.py
--rw-r--r--   0        0        0     6063 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/heat_conv.py
--rw-r--r--   0        0        0     6470 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/hetero_conv.py
--rw-r--r--   0        0        0     9282 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/hgt_conv.py
--rw-r--r--   0        0        0     7580 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/hypergraph_conv.py
--rw-r--r--   0        0        0     3523 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/le_conv.py
--rw-r--r--   0        0        0     2418 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/lg_conv.py
--rw-r--r--   0        0        0    11524 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/message_passing.jinja
--rw-r--r--   0        0        0    39859 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/message_passing.py
--rw-r--r--   0        0        0     4321 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/mf_conv.py
--rw-r--r--   0        0        0     4743 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/nn_conv.py
--rw-r--r--   0        0        0     4928 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/pan_conv.py
--rw-r--r--   0        0        0     4916 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/pdn_conv.py
--rw-r--r--   0        0        0     8242 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/pna_conv.py
--rw-r--r--   0        0        0     4522 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/point_conv.py
--rw-r--r--   0        0        0     3288 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/point_gnn_conv.py
--rw-r--r--   0        0        0     5889 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/point_transformer_conv.py
--rw-r--r--   0        0        0     5422 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/ppf_conv.py
--rw-r--r--   0        0        0     4180 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/res_gated_graph_conv.py
--rw-r--r--   0        0        0    22785 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/rgat_conv.py
--rw-r--r--   0        0        0    14977 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/rgcn_conv.py
--rw-r--r--   0        0        0     5813 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/sage_conv.py
--rw-r--r--   0        0        0     4597 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/sg_conv.py
--rw-r--r--   0        0        0     6283 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/signed_conv.py
--rw-r--r--   0        0        0     3899 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/simple_conv.py
--rw-r--r--   0        0        0     6330 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/spline_conv.py
--rw-r--r--   0        0        0     5185 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/ssg_conv.py
--rw-r--r--   0        0        0    11980 2023-05-24 06:05:41.064045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/supergat_conv.py
--rw-r--r--   0        0        0     4215 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/tag_conv.py
--rw-r--r--   0        0        0     9425 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/transformer_conv.py
--rw-r--r--   0        0        0      823 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/utils/__init__.py
--rw-r--r--   0        0        0     2692 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/utils/cheatsheet.py
--rw-r--r--   0        0        0      186 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/utils/helpers.py
--rw-r--r--   0        0        0     3259 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/utils/inspector.py
--rw-r--r--   0        0        0      679 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/utils/jit.py
--rw-r--r--   0        0        0     3859 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/utils/typing.py
--rw-r--r--   0        0        0     3103 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/wl_conv.py
--rw-r--r--   0        0        0     2349 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/wl_conv_continuous.py
--rw-r--r--   0        0        0     5955 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/x_conv.py
--rw-r--r--   0        0        0     3960 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/data_parallel.py
--rw-r--r--   0        0        0      712 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/dense/__init__.py
--rw-r--r--   0        0        0     4228 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/dense/dense_gat_conv.py
--rw-r--r--   0        0        0     2989 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/dense/dense_gcn_conv.py
--rw-r--r--   0        0        0     2357 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/dense/dense_gin_conv.py
--rw-r--r--   0        0        0     2737 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/dense/dense_graph_conv.py
--rw-r--r--   0        0        0     2658 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/dense/dense_sage_conv.py
--rw-r--r--   0        0        0     3050 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/dense/diff_pool.py
--rw-r--r--   0        0        0     5671 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/dense/dmon_pool.py
--rw-r--r--   0        0        0    15505 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/dense/linear.py
--rw-r--r--   0        0        0     4111 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/dense/mincut_pool.py
--rw-r--r--   0        0        0     3125 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/encoding.py
--rw-r--r--   0        0        0       92 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/functional/__init__.py
--rw-r--r--   0        0        0     1549 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/functional/bro.py
--rw-r--r--   0        0        0      863 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/functional/gini.py
--rw-r--r--   0        0        0    15551 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/fx.py
--rw-r--r--   0        0        0     1088 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/glob.py
--rw-r--r--   0        0        0     2457 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/inits.py
--rw-r--r--   0        0        0      241 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/kge/__init__.py
--rw-r--r--   0        0        0     5739 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/kge/base.py
--rw-r--r--   0        0        0     3234 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/kge/complex.py
--rw-r--r--   0        0        0     2462 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/kge/distmult.py
--rw-r--r--   0        0        0      771 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/kge/loader.py
--rw-r--r--   0        0        0     3208 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/kge/rotate.py
--rw-r--r--   0        0        0     3088 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/kge/transe.py
--rw-r--r--   0        0        0     8937 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/lr_scheduler.py
--rw-r--r--   0        0        0     9464 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/model_hub.py
--rw-r--r--   0        0        0     1647 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/__init__.py
--rw-r--r--   0        0        0     6591 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/attentive_fp.py
--rw-r--r--   0        0        0    10656 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/autoencoder.py
--rw-r--r--   0        0        0    27754 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/basic_gnn.py
--rw-r--r--   0        0        0     4138 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/captum.py
--rw-r--r--   0        0        0     6799 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/correct_and_smooth.py
--rw-r--r--   0        0        0     3972 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/deep_graph_infomax.py
--rw-r--r--   0        0        0     4223 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/deepgcn.py
--rw-r--r--   0        0        0    34432 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/dimenet.py
--rw-r--r--   0        0        0     4611 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/dimenet_utils.py
--rw-r--r--   0        0        0     7859 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/gnnff.py
--rw-r--r--   0        0        0     5381 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/graph_unet.py
--rw-r--r--   0        0        0     3397 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/jumping_knowledge.py
--rw-r--r--   0        0        0     3937 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/label_prop.py
--rw-r--r--   0        0        0    11282 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/lightgcn.py
--rw-r--r--   0        0        0     7901 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/linkx.py
--rw-r--r--   0        0        0     2566 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/mask_label.py
--rw-r--r--   0        0        0     6529 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/meta.py
--rw-r--r--   0        0        0    10318 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/metapath2vec.py
--rw-r--r--   0        0        0     8980 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/mlp.py
--rw-r--r--   0        0        0     7641 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/node2vec.py
--rw-r--r--   0        0        0     3257 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/pmlp.py
--rw-r--r--   0        0        0     8979 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/re_net.py
--rw-r--r--   0        0        0     5789 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/rect.py
--rw-r--r--   0        0        0    11818 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/rev_gnn.py
--rw-r--r--   0        0        0    16599 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/schnet.py
--rw-r--r--   0        0        0     9840 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/signed_gcn.py
--rw-r--r--   0        0        0    11579 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/tgn.py
--rw-r--r--   0        0        0     1957 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/module_dict.py
--rw-r--r--   0        0        0      638 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/norm/__init__.py
--rw-r--r--   0        0        0     8258 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/norm/batch_norm.py
--rw-r--r--   0        0        0     4706 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/norm/diff_group_norm.py
--rw-r--r--   0        0        0     2715 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/norm/graph_norm.py
--rw-r--r--   0        0        0     1492 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/norm/graph_size_norm.py
--rw-r--r--   0        0        0     4670 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/norm/instance_norm.py
--rw-r--r--   0        0        0     7806 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/norm/layer_norm.py
--rw-r--r--   0        0        0     1311 2023-05-24 06:05:41.068045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/norm/mean_subtraction_norm.py
--rw-r--r--   0        0        0     1654 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/norm/msg_norm.py
--rw-r--r--   0        0        0     2809 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/norm/pair_norm.py
--rw-r--r--   0        0        0     1982 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/parameter_dict.py
--rw-r--r--   0        0        0    12699 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/__init__.py
--rw-r--r--   0        0        0     6870 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/asap.py
--rw-r--r--   0        0        0     3966 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/avg_pool.py
--rw-r--r--   0        0        0       92 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/connect/__init__.py
--rw-r--r--   0        0        0     4001 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/connect/base.py
--rw-r--r--   0        0        0      273 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/consecutive.py
--rw-r--r--   0        0        0     1600 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/decimation.py
--rw-r--r--   0        0        0     8567 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/edge_pool.py
--rw-r--r--   0        0        0     3510 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/glob.py
--rw-r--r--   0        0        0     1292 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/graclus.py
--rw-r--r--   0        0        0     4262 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/max_pool.py
--rw-r--r--   0        0        0     5362 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/mem_pool.py
--rw-r--r--   0        0        0     4400 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/pan_pool.py
--rw-r--r--   0        0        0      631 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/pool.py
--rw-r--r--   0        0        0     5966 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/sag_pool.py
--rw-r--r--   0        0        0      135 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/select/__init__.py
--rw-r--r--   0        0        0     3208 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/select/base.py
--rw-r--r--   0        0        0     6262 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/select/topk.py
--rw-r--r--   0        0        0     5760 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/topk_pool.py
--rw-r--r--   0        0        0     2727 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/voxel_grid.py
--rw-r--r--   0        0        0      412 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/reshape.py
--rw-r--r--   0        0        0     6155 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/resolver.py
--rw-r--r--   0        0        0     1071 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/sequential.jinja
--rw-r--r--   0        0        0     4577 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/sequential.py
--rw-r--r--   0        0        0     5616 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/summary.py
--rw-r--r--   0        0        0     1282 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/to_fixed_size_transformer.py
--rw-r--r--   0        0        0     6486 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/to_hetero_module.py
--rw-r--r--   0        0        0    18407 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/to_hetero_transformer.py
--rw-r--r--   0        0        0    23103 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/to_hetero_with_bases_transformer.py
--rw-r--r--   0        0        0      102 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/unpool/__init__.py
--rw-r--r--   0        0        0     2586 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/unpool/knn_interpolate.py
--rw-r--r--   0        0        0      803 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/profile/__init__.py
--rw-r--r--   0        0        0     4363 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/profile/benchmark.py
--rw-r--r--   0        0        0    10364 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/profile/profile.py
--rw-r--r--   0        0        0    16665 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/profile/profiler.py
--rw-r--r--   0        0        0     4563 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/profile/utils.py
--rw-r--r--   0        0        0     1251 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/resolver.py
--rw-r--r--   0        0        0      481 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/sampler/__init__.py
--rw-r--r--   0        0        0    22762 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/sampler/base.py
--rw-r--r--   0        0        0     2734 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/sampler/hgt_sampler.py
--rw-r--r--   0        0        0    26144 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/sampler/neighbor_sampler.py
--rw-r--r--   0        0        0     5252 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/sampler/utils.py
--rw-r--r--   0        0        0      354 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/seed.py
--rw-r--r--   0        0        0      710 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/testing/__init__.py
--rw-r--r--   0        0        0     4368 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/testing/asserts.py
--rw-r--r--   0        0        0     1933 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/testing/data.py
--rw-r--r--   0        0        0     3842 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/testing/decorators.py
--rw-r--r--   0        0        0     1847 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/testing/feature_store.py
--rw-r--r--   0        0        0     1009 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/testing/graph_store.py
--rw-r--r--   0        0        0     4136 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/__init__.py
--rw-r--r--   0        0        0    13966 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/add_metapaths.py
--rw-r--r--   0        0        0     4838 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/add_positional_encoding.py
--rw-r--r--   0        0        0     2088 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/add_remaining_self_loops.py
--rw-r--r--   0        0        0     2019 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/add_self_loops.py
--rw-r--r--   0        0        0     1141 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/base_transform.py
--rw-r--r--   0        0        0     1937 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/cartesian.py
--rw-r--r--   0        0        0      641 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/center.py
--rw-r--r--   0        0        0     1659 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/compose.py
--rw-r--r--   0        0        0     1961 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/constant.py
--rw-r--r--   0        0        0     1223 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/delaunay.py
--rw-r--r--   0        0        0     1810 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/distance.py
--rw-r--r--   0        0        0     1035 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/face_to_edge.py
--rw-r--r--   0        0        0     2953 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/feature_propagation.py
--rw-r--r--   0        0        0     2368 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/fixed_points.py
--rw-r--r--   0        0        0     1398 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/gcn_norm.py
--rw-r--r--   0        0        0    24216 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/gdc.py
--rw-r--r--   0        0        0     1019 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/generate_mesh_normals.py
--rw-r--r--   0        0        0     2512 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/grid_sampling.py
--rw-r--r--   0        0        0     2544 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/knn_graph.py
--rw-r--r--   0        0        0     2466 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/laplacian_lambda_max.py
--rw-r--r--   0        0        0     2001 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/largest_connected_components.py
--rw-r--r--   0        0        0     3724 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/line_graph.py
--rw-r--r--   0        0        0     1998 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/linear_transformation.py
--rw-r--r--   0        0        0     1699 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/local_cartesian.py
--rw-r--r--   0        0        0     1405 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/local_degree_profile.py
--rw-r--r--   0        0        0     4600 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/mask.py
--rw-r--r--   0        0        0     6093 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/node_property_split.py
--rw-r--r--   0        0        0     1029 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/normalize_features.py
--rw-r--r--   0        0        0     1739 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/normalize_rotation.py
--rw-r--r--   0        0        0      621 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/normalize_scale.py
--rw-r--r--   0        0        0     1534 2023-05-24 06:05:41.072045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/one_hot_degree.py
--rw-r--r--   0        0        0    21976 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/pad.py
--rw-r--r--   0        0        0     1794 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/point_pair_features.py
--rw-r--r--   0        0        0     2127 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/polar.py
--rw-r--r--   0        0        0     2051 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/radius_graph.py
--rw-r--r--   0        0        0      989 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/random_flip.py
--rw-r--r--   0        0        0     1511 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/random_jitter.py
--rw-r--r--   0        0        0    14298 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/random_link_split.py
--rw-r--r--   0        0        0     5769 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/random_node_split.py
--rw-r--r--   0        0        0     1904 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/random_rotate.py
--rw-r--r--   0        0        0     1216 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/random_scale.py
--rw-r--r--   0        0        0     1320 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/random_shear.py
--rw-r--r--   0        0        0     1806 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/remove_duplicated_edges.py
--rw-r--r--   0        0        0     2284 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/remove_isolated_nodes.py
--rw-r--r--   0        0        0      960 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/remove_training_classes.py
--rw-r--r--   0        0        0     6112 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/rooted_subgraph.py
--rw-r--r--   0        0        0     2141 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/sample_points.py
--rw-r--r--   0        0        0     2129 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/sign.py
--rw-r--r--   0        0        0     2242 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/spherical.py
--rw-r--r--   0        0        0     1003 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/svd_feature_reduction.py
--rw-r--r--   0        0        0     1608 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/target_indegree.py
--rw-r--r--   0        0        0     2328 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/to_dense.py
--rw-r--r--   0        0        0     1456 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/to_device.py
--rw-r--r--   0        0        0     5354 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/to_sparse_tensor.py
--rw-r--r--   0        0        0     2622 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/to_superpixels.py
--rw-r--r--   0        0        0     2973 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/to_undirected.py
--rw-r--r--   0        0        0     1215 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/two_hop.py
--rw-r--r--   0        0        0     2784 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/virtual_node.py
--rw-r--r--   0        0        0     9288 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/typing.py
--rw-r--r--   0        0        0     4549 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/__init__.py
--rw-r--r--   0        0        0     2347 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/assortativity.py
--rw-r--r--   0        0        0     9080 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/augmentation.py
--rw-r--r--   0        0        0     5037 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/coalesce.py
--rw-r--r--   0        0        0    19630 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/convert.py
--rw-r--r--   0        0        0     1018 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/degree.py
--rw-r--r--   0        0        0    11323 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/dropout.py
--rw-r--r--   0        0        0     1657 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/embedding.py
--rw-r--r--   0        0        0     4042 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/geodesic.py
--rw-r--r--   0        0        0     3755 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/get_laplacian.py
--rw-r--r--   0        0        0     4424 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/get_mesh_laplacian.py
--rw-r--r--   0        0        0     2536 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/grid.py
--rw-r--r--   0        0        0     9798 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/hetero.py
--rw-r--r--   0        0        0     4818 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/homophily.py
--rw-r--r--   0        0        0     3574 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/isolated.py
--rw-r--r--   0        0        0    15855 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/loop.py
--rw-r--r--   0        0        0     1884 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/mask.py
--rw-r--r--   0        0        0      608 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/mixin.py
--rw-r--r--   0        0        0    14643 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/negative_sampling.py
--rw-r--r--   0        0        0     3344 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/nested.py
--rw-r--r--   0        0        0     1169 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/normalized_cut.py
--rw-r--r--   0        0        0     1917 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/num_nodes.py
--rw-r--r--   0        0        0     1404 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/one_hot.py
--rw-r--r--   0        0        0     5154 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/random.py
--rw-r--r--   0        0        0      361 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/repeat.py
--rw-r--r--   0        0        0     7525 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/scatter.py
--rw-r--r--   0        0        0     1110 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/segment.py
--rw-r--r--   0        0        0     2149 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/select.py
--rw-r--r--   0        0        0     6016 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/smiles.py
--rw-r--r--   0        0        0     2718 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/softmax.py
--rw-r--r--   0        0        0     1017 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/sort.py
--rw-r--r--   0        0        0     3066 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/sort_edge_index.py
--rw-r--r--   0        0        0    14860 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/sparse.py
--rw-r--r--   0        0        0     5547 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/spmm.py
--rw-r--r--   0        0        0    12370 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/subgraph.py
--rw-r--r--   0        0        0     3439 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/to_dense_adj.py
--rw-r--r--   0        0        0     4313 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/to_dense_batch.py
--rw-r--r--   0        0        0     3489 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/train_test_split_edges.py
--rw-r--r--   0        0        0     4867 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/tree_decomposition.py
--rw-r--r--   0        0        0     6350 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/trim_to_layer.py
--rw-r--r--   0        0        0     2125 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/unbatch.py
--rw-r--r--   0        0        0     5770 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/undirected.py
--rw-r--r--   0        0        0      123 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/visualization/__init__.py
--rw-r--r--   0        0        0     4149 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/visualization/graph.py
--rw-r--r--   0        0        0      388 2023-05-24 06:05:41.076045 pyg_nightly-2.4.0.dev20230524/torch_geometric/visualization/influence.py
--rw-r--r--   0        0        0    63898 1970-01-01 00:00:00.000000 pyg_nightly-2.4.0.dev20230524/PKG-INFO
+-rw-r--r--   0        0        0    60889 2023-05-25 06:05:58.118297 pyg_nightly-2.4.0.dev20230525/README.md
+-rw-r--r--   0        0        0     4073 2023-05-25 06:05:58.682332 pyg_nightly-2.4.0.dev20230525/pyproject.toml
+-rw-r--r--   0        0        0     1055 2023-05-25 06:05:58.678331 pyg_nightly-2.4.0.dev20230525/torch_geometric/__init__.py
+-rw-r--r--   0        0        0     3392 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/compile.py
+-rw-r--r--   0        0        0      352 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/contrib/__init__.py
+-rw-r--r--   0        0        0       23 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/contrib/datasets/__init__.py
+-rw-r--r--   0        0        0      163 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/contrib/explain/__init__.py
+-rw-r--r--   0        0        0    20540 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/contrib/explain/graphmask_explainer.py
+-rw-r--r--   0        0        0    16627 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/contrib/explain/pgm_explainer.py
+-rw-r--r--   0        0        0       72 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/contrib/nn/__init__.py
+-rw-r--r--   0        0        0       23 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/contrib/nn/conv/__init__.py
+-rw-r--r--   0        0        0      113 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/contrib/nn/models/__init__.py
+-rw-r--r--   0        0        0    33261 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/contrib/nn/models/rbcd_attack.py
+-rw-r--r--   0        0        0       23 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/contrib/transforms/__init__.py
+-rw-r--r--   0        0        0     3383 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/data/__init__.py
+-rw-r--r--   0        0        0     7428 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/data/batch.py
+-rw-r--r--   0        0        0    10658 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/data/collate.py
+-rw-r--r--   0        0        0    37598 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/data/data.py
+-rw-r--r--   0        0        0     2922 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/data/datapipes.py
+-rw-r--r--   0        0        0    14850 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/data/dataset.py
+-rw-r--r--   0        0        0     1359 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/data/download.py
+-rw-r--r--   0        0        0     2252 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/data/extract.py
+-rw-r--r--   0        0        0    21075 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/data/feature_store.py
+-rw-r--r--   0        0        0    13495 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/data/graph_store.py
+-rw-r--r--   0        0        0    44133 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/data/hetero_data.py
+-rw-r--r--   0        0        0     7805 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/data/in_memory_dataset.py
+-rw-r--r--   0        0        0      178 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/data/lightning/__init__.py
+-rw-r--r--   0        0        0    28490 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/data/lightning/datamodule.py
+-rw-r--r--   0        0        0      338 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/data/makedirs.py
+-rw-r--r--   0        0        0     3962 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/data/remote_backend_utils.py
+-rw-r--r--   0        0        0     4360 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/data/separate.py
+-rw-r--r--   0        0        0    25245 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/data/storage.py
+-rw-r--r--   0        0        0     5219 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/data/summary.py
+-rw-r--r--   0        0        0     9354 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/data/temporal.py
+-rw-r--r--   0        0        0     1038 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/data/view.py
+-rw-r--r--   0        0        0     5051 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/__init__.py
+-rw-r--r--   0        0        0     4220 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/actor.py
+-rw-r--r--   0        0        0     5584 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/airfrans.py
+-rw-r--r--   0        0        0     3711 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/airports.py
+-rw-r--r--   0        0        0     3050 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/amazon.py
+-rw-r--r--   0        0        0     4099 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/amazon_products.py
+-rw-r--r--   0        0        0     4942 2023-05-25 06:05:58.166300 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/aminer.py
+-rw-r--r--   0        0        0     5266 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/aqsol.py
+-rw-r--r--   0        0        0     5735 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/attributed_graph_dataset.py
+-rw-r--r--   0        0        0     4063 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/ba2motif_dataset.py
+-rw-r--r--   0        0        0     3518 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/ba_multi_shapes.py
+-rw-r--r--   0        0        0     3824 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/ba_shapes.py
+-rw-r--r--   0        0        0     4137 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/bitcoin_otc.py
+-rw-r--r--   0        0        0     4205 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/citation_full.py
+-rw-r--r--   0        0        0     3009 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/coauthor.py
+-rw-r--r--   0        0        0     4564 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/coma.py
+-rw-r--r--   0        0        0     5192 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/dblp.py
+-rw-r--r--   0        0        0     5608 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/dbp15k.py
+-rw-r--r--   0        0        0     2308 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/deezer_europe.py
+-rw-r--r--   0        0        0     3862 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/dgraph.py
+-rw-r--r--   0        0        0     5865 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/dynamic_faust.py
+-rw-r--r--   0        0        0     4498 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/elliptic.py
+-rw-r--r--   0        0        0     2990 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/elliptic_temporal.py
+-rw-r--r--   0        0        0     2631 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/email_eu_core.py
+-rw-r--r--   0        0        0     7001 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/entities.py
+-rw-r--r--   0        0        0     5817 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/explainer_dataset.py
+-rw-r--r--   0        0        0     2228 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/facebook.py
+-rw-r--r--   0        0        0    10215 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/fake.py
+-rw-r--r--   0        0        0     3924 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/faust.py
+-rw-r--r--   0        0        0     4099 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/flickr.py
+-rw-r--r--   0        0        0     3815 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/freebase.py
+-rw-r--r--   0        0        0     3416 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/gdelt.py
+-rw-r--r--   0        0        0     9261 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/ged_dataset.py
+-rw-r--r--   0        0        0     2626 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/gemsec.py
+-rw-r--r--   0        0        0     3954 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/geometry.py
+-rw-r--r--   0        0        0     2484 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/github.py
+-rw-r--r--   0        0        0     6762 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/gnn_benchmark_dataset.py
+-rw-r--r--   0        0        0      221 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/graph_generator/__init__.py
+-rw-r--r--   0        0        0      965 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/graph_generator/ba_graph.py
+-rw-r--r--   0        0        0      949 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/graph_generator/base.py
+-rw-r--r--   0        0        0      918 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/graph_generator/er_graph.py
+-rw-r--r--   0        0        0     1159 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/graph_generator/grid_graph.py
+-rw-r--r--   0        0        0     4043 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/heterophilous_graph_dataset.py
+-rw-r--r--   0        0        0     8467 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/hgb_dataset.py
+-rw-r--r--   0        0        0    11053 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/hydro_net.py
+-rw-r--r--   0        0        0     4447 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/icews.py
+-rw-r--r--   0        0        0     4000 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/imdb.py
+-rw-r--r--   0        0        0     7169 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/infection_dataset.py
+-rw-r--r--   0        0        0     3439 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/jodie.py
+-rw-r--r--   0        0        0     3444 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/karate.py
+-rw-r--r--   0        0        0     4349 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/last_fm.py
+-rw-r--r--   0        0        0     2283 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/lastfm_asia.py
+-rw-r--r--   0        0        0     6582 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/linkx_dataset.py
+-rw-r--r--   0        0        0    11559 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/lrgb.py
+-rw-r--r--   0        0        0     5044 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/malnet_tiny.py
+-rw-r--r--   0        0        0    16482 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/md17.py
+-rw-r--r--   0        0        0     3770 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/mixhop_synthetic_dataset.py
+-rw-r--r--   0        0        0     3136 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/mnist_superpixels.py
+-rw-r--r--   0        0        0     5251 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/modelnet.py
+-rw-r--r--   0        0        0     6593 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/molecule_net.py
+-rw-r--r--   0        0        0      227 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/motif_generator/__init__.py
+-rw-r--r--   0        0        0      910 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/motif_generator/base.py
+-rw-r--r--   0        0        0     1203 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/motif_generator/custom.py
+-rw-r--r--   0        0        0      984 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/motif_generator/cycle.py
+-rw-r--r--   0        0        0      801 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/motif_generator/house.py
+-rw-r--r--   0        0        0     3787 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/movie_lens.py
+-rw-r--r--   0        0        0     6005 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/movie_lens_100k.py
+-rw-r--r--   0        0        0     2889 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/nell.py
+-rw-r--r--   0        0        0     7190 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/ogb_mag.py
+-rw-r--r--   0        0        0     3415 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/omdb.py
+-rw-r--r--   0        0        0     3964 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/particle.py
+-rw-r--r--   0        0        0    10699 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/pascal.py
+-rw-r--r--   0        0        0     4602 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/pascal_pf.py
+-rw-r--r--   0        0        0     5716 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/pcpnet_dataset.py
+-rw-r--r--   0        0        0     6975 2023-05-25 06:05:58.170301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/planetoid.py
+-rw-r--r--   0        0        0     2842 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/polblogs.py
+-rw-r--r--   0        0        0     4866 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/ppi.py
+-rw-r--r--   0        0        0     3182 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/qm7.py
+-rw-r--r--   0        0        0    16813 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/qm9.py
+-rw-r--r--   0        0        0     2941 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/reddit.py
+-rw-r--r--   0        0        0     4439 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/reddit2.py
+-rw-r--r--   0        0        0     4345 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/rel_link_pred_dataset.py
+-rw-r--r--   0        0        0     4173 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/s3dis.py
+-rw-r--r--   0        0        0     8140 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/sbm_dataset.py
+-rw-r--r--   0        0        0     8088 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/shapenet.py
+-rw-r--r--   0        0        0     6150 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/shrec2016.py
+-rw-r--r--   0        0        0     9283 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/snap_dataset.py
+-rw-r--r--   0        0        0     3031 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/suite_sparse.py
+-rw-r--r--   0        0        0     3959 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/taobao.py
+-rw-r--r--   0        0        0     4451 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/tosca.py
+-rw-r--r--   0        0        0     7302 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/tu_dataset.py
+-rw-r--r--   0        0        0     3464 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/twitch.py
+-rw-r--r--   0        0        0     6929 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/upfd.py
+-rw-r--r--   0        0        0      182 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/utils/__init__.py
+-rw-r--r--   0        0        0     1732 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/utils/cheatsheet.py
+-rw-r--r--   0        0        0     4615 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/webkb.py
+-rw-r--r--   0        0        0     3674 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/wikics.py
+-rw-r--r--   0        0        0     6083 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/wikipedia_network.py
+-rw-r--r--   0        0        0     6322 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/willow_object_class.py
+-rw-r--r--   0        0        0     7857 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/word_net.py
+-rw-r--r--   0        0        0     4116 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/yelp.py
+-rw-r--r--   0        0        0     6171 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/zinc.py
+-rw-r--r--   0        0        0     1197 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/debug.py
+-rw-r--r--   0        0        0      748 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/deprecation.py
+-rw-r--r--   0        0        0     2466 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/experimental.py
+-rw-r--r--   0        0        0      359 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/__init__.py
+-rw-r--r--   0        0        0      418 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/algorithm/__init__.py
+-rw-r--r--   0        0        0     4491 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/algorithm/attention_explainer.py
+-rw-r--r--   0        0        0     6899 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/algorithm/base.py
+-rw-r--r--   0        0        0    12489 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/algorithm/captum.py
+-rw-r--r--   0        0        0     6530 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/algorithm/captum_explainer.py
+-rw-r--r--   0        0        0     2867 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/algorithm/dummy_explainer.py
+-rw-r--r--   0        0        0    11149 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/algorithm/gnn_explainer.py
+-rw-r--r--   0        0        0    10370 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/algorithm/pg_explainer.py
+-rw-r--r--   0        0        0     2308 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/algorithm/utils.py
+-rw-r--r--   0        0        0     7834 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/config.py
+-rw-r--r--   0        0        0    10375 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/explainer.py
+-rw-r--r--   0        0        0    14842 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/explanation.py
+-rw-r--r--   0        0        0      301 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/metric/__init__.py
+-rw-r--r--   0        0        0     1888 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/metric/basic.py
+-rw-r--r--   0        0        0     3063 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/metric/faithfulness.py
+-rw-r--r--   0        0        0     6157 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/metric/fidelity.py
+-rw-r--r--   0        0        0     2045 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/__init__.py
+-rw-r--r--   0        0        0      510 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/benchmark.py
+-rw-r--r--   0        0        0     2371 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/checkpoint.py
+-rw-r--r--   0        0        0      738 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/cmd_args.py
+-rw-r--r--   0        0        0    17221 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/config.py
+-rw-r--r--   0        0        0    14575 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/config_store.py
+-rw-r--r--   0        0        0      389 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/contrib/__init__.py
+-rw-r--r--   0        0        0      221 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/contrib/act/__init__.py
+-rw-r--r--   0        0        0      221 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/contrib/config/__init__.py
+-rw-r--r--   0        0        0      221 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/contrib/encoder/__init__.py
+-rw-r--r--   0        0        0      221 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/contrib/head/__init__.py
+-rw-r--r--   0        0        0      221 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/contrib/layer/__init__.py
+-rw-r--r--   0        0        0     8304 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/contrib/layer/generalconv.py
+-rw-r--r--   0        0        0      221 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/contrib/loader/__init__.py
+-rw-r--r--   0        0        0      221 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/contrib/loss/__init__.py
+-rw-r--r--   0        0        0      221 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/contrib/network/__init__.py
+-rw-r--r--   0        0        0      221 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/contrib/optimizer/__init__.py
+-rw-r--r--   0        0        0      221 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/contrib/pooling/__init__.py
+-rw-r--r--   0        0        0      221 2023-05-25 06:05:58.174301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/contrib/stage/__init__.py
+-rw-r--r--   0        0        0      221 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/contrib/train/__init__.py
+-rw-r--r--   0        0        0      221 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/contrib/transform/__init__.py
+-rw-r--r--   0        0        0      375 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/imports.py
+-rw-r--r--   0        0        0      490 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/init.py
+-rw-r--r--   0        0        0    11763 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/loader.py
+-rw-r--r--   0        0        0    11329 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/logger.py
+-rw-r--r--   0        0        0     1474 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/loss.py
+-rw-r--r--   0        0        0     3110 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/model_builder.py
+-rw-r--r--   0        0        0     1121 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/models/__init__.py
+-rw-r--r--   0        0        0      822 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/models/act.py
+-rw-r--r--   0        0        0     2546 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/models/encoder.py
+-rw-r--r--   0        0        0     5133 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/models/gnn.py
+-rw-r--r--   0        0        0     4434 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/models/head.py
+-rw-r--r--   0        0        0    12486 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/models/layer.py
+-rw-r--r--   0        0        0      288 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/models/pooling.py
+-rw-r--r--   0        0        0     1391 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/models/transform.py
+-rw-r--r--   0        0        0     2544 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/optim.py
+-rw-r--r--   0        0        0     3944 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/register.py
+-rw-r--r--   0        0        0     1887 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/train.py
+-rw-r--r--   0        0        0        0 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/utils/LICENSE
+-rw-r--r--   0        0        0      641 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/utils/__init__.py
+-rw-r--r--   0        0        0     9513 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/utils/agg_runs.py
+-rw-r--r--   0        0        0     3056 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/utils/comp_budget.py
+-rw-r--r--   0        0        0     1352 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/utils/device.py
+-rw-r--r--   0        0        0      690 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/utils/epoch.py
+-rw-r--r--   0        0        0     2050 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/utils/io.py
+-rw-r--r--   0        0        0      606 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/utils/plot.py
+-rw-r--r--   0        0        0      198 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/utils/tools.py
+-rw-r--r--   0        0        0      830 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/home.py
+-rw-r--r--   0        0        0      528 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/io/__init__.py
+-rw-r--r--   0        0        0     1148 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/io/npz.py
+-rw-r--r--   0        0        0      957 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/io/obj.py
+-rw-r--r--   0        0        0     2586 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/io/off.py
+-rw-r--r--   0        0        0     4211 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/io/planetoid.py
+-rw-r--r--   0        0        0      476 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/io/ply.py
+-rw-r--r--   0        0        0     1136 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/io/sdf.py
+-rw-r--r--   0        0        0     4733 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/io/tu.py
+-rw-r--r--   0        0        0      562 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/io/txt_array.py
+-rw-r--r--   0        0        0      768 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/lazy_loader.py
+-rw-r--r--   0        0        0     1675 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/__init__.py
+-rw-r--r--   0        0        0     1433 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/base.py
+-rw-r--r--   0        0        0    11349 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/cluster.py
+-rw-r--r--   0        0        0     1449 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/data_list_loader.py
+-rw-r--r--   0        0        0     3222 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/dataloader.py
+-rw-r--r--   0        0        0     1683 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/dense_data_loader.py
+-rw-r--r--   0        0        0     4285 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/dynamic_batch_sampler.py
+-rw-r--r--   0        0        0     8448 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/graph_saint.py
+-rw-r--r--   0        0        0     6012 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/hgt_loader.py
+-rw-r--r--   0        0        0     3754 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/imbalanced_sampler.py
+-rw-r--r--   0        0        0    13948 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/link_loader.py
+-rw-r--r--   0        0        0    12513 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/link_neighbor_loader.py
+-rw-r--r--   0        0        0     6317 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/mixin.py
+-rw-r--r--   0        0        0    11382 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/neighbor_loader.py
+-rw-r--r--   0        0        0     8513 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/neighbor_sampler.py
+-rw-r--r--   0        0        0     9365 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/node_loader.py
+-rw-r--r--   0        0        0     2141 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/prefetch.py
+-rw-r--r--   0        0        0     2196 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/random_node_loader.py
+-rw-r--r--   0        0        0     4173 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/shadow.py
+-rw-r--r--   0        0        0     1319 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/temporal_dataloader.py
+-rw-r--r--   0        0        0    12273 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/utils.py
+-rw-r--r--   0        0        0     3518 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/zip_loader.py
+-rw-r--r--   0        0        0      832 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/logging.py
+-rw-r--r--   0        0        0      911 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/__init__.py
+-rw-r--r--   0        0        0     1397 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/__init__.py
+-rw-r--r--   0        0        0     2395 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/attention.py
+-rw-r--r--   0        0        0     7106 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/base.py
+-rw-r--r--   0        0        0    11000 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/basic.py
+-rw-r--r--   0        0        0     2064 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/deep_sets.py
+-rw-r--r--   0        0        0     6881 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/equilibrium.py
+-rw-r--r--   0        0        0    12229 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/fused.py
+-rw-r--r--   0        0        0     3062 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/gmt.py
+-rw-r--r--   0        0        0     1464 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/gru.py
+-rw-r--r--   0        0        0     1484 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/lstm.py
+-rw-r--r--   0        0        0     1995 2023-05-25 06:05:58.178301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/mlp.py
+-rw-r--r--   0        0        0     8163 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/multi.py
+-rw-r--r--   0        0        0     6174 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/quantile.py
+-rw-r--r--   0        0        0     4642 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/scaler.py
+-rw-r--r--   0        0        0     2517 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/set2set.py
+-rw-r--r--   0        0        0     3439 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/set_transformer.py
+-rw-r--r--   0        0        0     1921 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/sort.py
+-rw-r--r--   0        0        0     8322 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/utils.py
+-rw-r--r--   0        0        0     3360 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/__init__.py
+-rw-r--r--   0        0        0     3088 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/agnn_conv.py
+-rw-r--r--   0        0        0     4388 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/antisymmetric_conv.py
+-rw-r--r--   0        0        0     6010 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/appnp.py
+-rw-r--r--   0        0        0     6637 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/arma_conv.py
+-rw-r--r--   0        0        0     4036 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/cg_conv.py
+-rw-r--r--   0        0        0     6444 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/cheb_conv.py
+-rw-r--r--   0        0        0     5303 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/cluster_gcn_conv.py
+-rw-r--r--   0        0        0      251 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/cugraph/__init__.py
+-rw-r--r--   0        0        0     8195 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/cugraph/base.py
+-rw-r--r--   0        0        0     2849 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/cugraph/gat_conv.py
+-rw-r--r--   0        0        0     4218 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/cugraph/rgcn_conv.py
+-rw-r--r--   0        0        0     2802 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/cugraph/sage_conv.py
+-rw-r--r--   0        0        0    12105 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/dna_conv.py
+-rw-r--r--   0        0        0     5550 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/edge_conv.py
+-rw-r--r--   0        0        0    10482 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/eg_conv.py
+-rw-r--r--   0        0        0     7927 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/fa_conv.py
+-rw-r--r--   0        0        0     4453 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/feast_conv.py
+-rw-r--r--   0        0        0     6332 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/film_conv.py
+-rw-r--r--   0        0        0     4242 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/fused_gat_conv.py
+-rw-r--r--   0        0        0    13610 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/gat_conv.py
+-rw-r--r--   0        0        0     3582 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/gated_graph_conv.py
+-rw-r--r--   0        0        0    12423 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/gatv2_conv.py
+-rw-r--r--   0        0        0     7022 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/gcn2_conv.py
+-rw-r--r--   0        0        0     9333 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/gcn_conv.py
+-rw-r--r--   0        0        0     9992 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/gen_conv.py
+-rw-r--r--   0        0        0     7512 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/general_conv.py
+-rw-r--r--   0        0        0     7444 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/gin_conv.py
+-rw-r--r--   0        0        0     8320 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/gmm_conv.py
+-rw-r--r--   0        0        0     5764 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/gps_conv.py
+-rw-r--r--   0        0        0     3547 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/graph_conv.py
+-rw-r--r--   0        0        0     5023 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/gravnet_conv.py
+-rw-r--r--   0        0        0     7354 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/han_conv.py
+-rw-r--r--   0        0        0     6063 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/heat_conv.py
+-rw-r--r--   0        0        0     6470 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/hetero_conv.py
+-rw-r--r--   0        0        0     9282 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/hgt_conv.py
+-rw-r--r--   0        0        0     7580 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/hypergraph_conv.py
+-rw-r--r--   0        0        0     3523 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/le_conv.py
+-rw-r--r--   0        0        0     2418 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/lg_conv.py
+-rw-r--r--   0        0        0    11524 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/message_passing.jinja
+-rw-r--r--   0        0        0    39859 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/message_passing.py
+-rw-r--r--   0        0        0     4321 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/mf_conv.py
+-rw-r--r--   0        0        0     4743 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/nn_conv.py
+-rw-r--r--   0        0        0     4928 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/pan_conv.py
+-rw-r--r--   0        0        0     4916 2023-05-25 06:05:58.182301 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/pdn_conv.py
+-rw-r--r--   0        0        0     8242 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/pna_conv.py
+-rw-r--r--   0        0        0     4522 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/point_conv.py
+-rw-r--r--   0        0        0     3288 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/point_gnn_conv.py
+-rw-r--r--   0        0        0     5889 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/point_transformer_conv.py
+-rw-r--r--   0        0        0     5422 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/ppf_conv.py
+-rw-r--r--   0        0        0     4180 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/res_gated_graph_conv.py
+-rw-r--r--   0        0        0    22785 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/rgat_conv.py
+-rw-r--r--   0        0        0    14977 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/rgcn_conv.py
+-rw-r--r--   0        0        0     5813 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/sage_conv.py
+-rw-r--r--   0        0        0     4597 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/sg_conv.py
+-rw-r--r--   0        0        0     6283 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/signed_conv.py
+-rw-r--r--   0        0        0     3899 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/simple_conv.py
+-rw-r--r--   0        0        0     6330 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/spline_conv.py
+-rw-r--r--   0        0        0     5185 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/ssg_conv.py
+-rw-r--r--   0        0        0    11980 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/supergat_conv.py
+-rw-r--r--   0        0        0     4215 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/tag_conv.py
+-rw-r--r--   0        0        0     9425 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/transformer_conv.py
+-rw-r--r--   0        0        0      823 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/utils/__init__.py
+-rw-r--r--   0        0        0     2692 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/utils/cheatsheet.py
+-rw-r--r--   0        0        0      186 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/utils/helpers.py
+-rw-r--r--   0        0        0     3259 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/utils/inspector.py
+-rw-r--r--   0        0        0      679 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/utils/jit.py
+-rw-r--r--   0        0        0     3859 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/utils/typing.py
+-rw-r--r--   0        0        0     3103 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/wl_conv.py
+-rw-r--r--   0        0        0     2349 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/wl_conv_continuous.py
+-rw-r--r--   0        0        0     5955 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/x_conv.py
+-rw-r--r--   0        0        0     3960 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/data_parallel.py
+-rw-r--r--   0        0        0      712 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/dense/__init__.py
+-rw-r--r--   0        0        0     4228 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/dense/dense_gat_conv.py
+-rw-r--r--   0        0        0     2989 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/dense/dense_gcn_conv.py
+-rw-r--r--   0        0        0     2357 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/dense/dense_gin_conv.py
+-rw-r--r--   0        0        0     2737 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/dense/dense_graph_conv.py
+-rw-r--r--   0        0        0     2658 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/dense/dense_sage_conv.py
+-rw-r--r--   0        0        0     3050 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/dense/diff_pool.py
+-rw-r--r--   0        0        0     5671 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/dense/dmon_pool.py
+-rw-r--r--   0        0        0    15505 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/dense/linear.py
+-rw-r--r--   0        0        0     4111 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/dense/mincut_pool.py
+-rw-r--r--   0        0        0     3125 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/encoding.py
+-rw-r--r--   0        0        0       92 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/functional/__init__.py
+-rw-r--r--   0        0        0     1549 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/functional/bro.py
+-rw-r--r--   0        0        0      863 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/functional/gini.py
+-rw-r--r--   0        0        0    15551 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/fx.py
+-rw-r--r--   0        0        0     1088 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/glob.py
+-rw-r--r--   0        0        0     2457 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/inits.py
+-rw-r--r--   0        0        0      241 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/kge/__init__.py
+-rw-r--r--   0        0        0     5739 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/kge/base.py
+-rw-r--r--   0        0        0     3234 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/kge/complex.py
+-rw-r--r--   0        0        0     2462 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/kge/distmult.py
+-rw-r--r--   0        0        0      771 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/kge/loader.py
+-rw-r--r--   0        0        0     3208 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/kge/rotate.py
+-rw-r--r--   0        0        0     3088 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/kge/transe.py
+-rw-r--r--   0        0        0     8937 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/lr_scheduler.py
+-rw-r--r--   0        0        0     9464 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/model_hub.py
+-rw-r--r--   0        0        0     1647 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/__init__.py
+-rw-r--r--   0        0        0     6591 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/attentive_fp.py
+-rw-r--r--   0        0        0    10656 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/autoencoder.py
+-rw-r--r--   0        0        0    27754 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/basic_gnn.py
+-rw-r--r--   0        0        0     4138 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/captum.py
+-rw-r--r--   0        0        0     6799 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/correct_and_smooth.py
+-rw-r--r--   0        0        0     3972 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/deep_graph_infomax.py
+-rw-r--r--   0        0        0     4223 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/deepgcn.py
+-rw-r--r--   0        0        0    34432 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/dimenet.py
+-rw-r--r--   0        0        0     4611 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/dimenet_utils.py
+-rw-r--r--   0        0        0     7859 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/gnnff.py
+-rw-r--r--   0        0        0     5381 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/graph_unet.py
+-rw-r--r--   0        0        0     3397 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/jumping_knowledge.py
+-rw-r--r--   0        0        0     3937 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/label_prop.py
+-rw-r--r--   0        0        0    11282 2023-05-25 06:05:58.186302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/lightgcn.py
+-rw-r--r--   0        0        0     7901 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/linkx.py
+-rw-r--r--   0        0        0     2566 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/mask_label.py
+-rw-r--r--   0        0        0     6529 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/meta.py
+-rw-r--r--   0        0        0    10318 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/metapath2vec.py
+-rw-r--r--   0        0        0     8980 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/mlp.py
+-rw-r--r--   0        0        0     7641 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/node2vec.py
+-rw-r--r--   0        0        0     3257 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/pmlp.py
+-rw-r--r--   0        0        0     8979 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/re_net.py
+-rw-r--r--   0        0        0     5789 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/rect.py
+-rw-r--r--   0        0        0    11818 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/rev_gnn.py
+-rw-r--r--   0        0        0    16599 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/schnet.py
+-rw-r--r--   0        0        0     9840 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/signed_gcn.py
+-rw-r--r--   0        0        0    11579 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/tgn.py
+-rw-r--r--   0        0        0     1957 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/module_dict.py
+-rw-r--r--   0        0        0      638 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/norm/__init__.py
+-rw-r--r--   0        0        0     8258 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/norm/batch_norm.py
+-rw-r--r--   0        0        0     4706 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/norm/diff_group_norm.py
+-rw-r--r--   0        0        0     2715 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/norm/graph_norm.py
+-rw-r--r--   0        0        0     1492 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/norm/graph_size_norm.py
+-rw-r--r--   0        0        0     4670 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/norm/instance_norm.py
+-rw-r--r--   0        0        0     7806 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/norm/layer_norm.py
+-rw-r--r--   0        0        0     1311 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/norm/mean_subtraction_norm.py
+-rw-r--r--   0        0        0     1654 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/norm/msg_norm.py
+-rw-r--r--   0        0        0     2809 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/norm/pair_norm.py
+-rw-r--r--   0        0        0     1982 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/parameter_dict.py
+-rw-r--r--   0        0        0    12699 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/__init__.py
+-rw-r--r--   0        0        0     6870 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/asap.py
+-rw-r--r--   0        0        0     3966 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/avg_pool.py
+-rw-r--r--   0        0        0       92 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/connect/__init__.py
+-rw-r--r--   0        0        0     4001 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/connect/base.py
+-rw-r--r--   0        0        0      273 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/consecutive.py
+-rw-r--r--   0        0        0     1600 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/decimation.py
+-rw-r--r--   0        0        0     8567 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/edge_pool.py
+-rw-r--r--   0        0        0     3510 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/glob.py
+-rw-r--r--   0        0        0     1292 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/graclus.py
+-rw-r--r--   0        0        0     4262 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/max_pool.py
+-rw-r--r--   0        0        0     5362 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/mem_pool.py
+-rw-r--r--   0        0        0     4400 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/pan_pool.py
+-rw-r--r--   0        0        0      631 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/pool.py
+-rw-r--r--   0        0        0     5966 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/sag_pool.py
+-rw-r--r--   0        0        0      135 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/select/__init__.py
+-rw-r--r--   0        0        0     3208 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/select/base.py
+-rw-r--r--   0        0        0     6262 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/select/topk.py
+-rw-r--r--   0        0        0     5760 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/topk_pool.py
+-rw-r--r--   0        0        0     2727 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/voxel_grid.py
+-rw-r--r--   0        0        0      412 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/reshape.py
+-rw-r--r--   0        0        0     6155 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/resolver.py
+-rw-r--r--   0        0        0     1071 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/sequential.jinja
+-rw-r--r--   0        0        0     4577 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/sequential.py
+-rw-r--r--   0        0        0     5616 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/summary.py
+-rw-r--r--   0        0        0     1282 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/to_fixed_size_transformer.py
+-rw-r--r--   0        0        0     6486 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/to_hetero_module.py
+-rw-r--r--   0        0        0    18407 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/to_hetero_transformer.py
+-rw-r--r--   0        0        0    23103 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/to_hetero_with_bases_transformer.py
+-rw-r--r--   0        0        0      102 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/unpool/__init__.py
+-rw-r--r--   0        0        0     2586 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/unpool/knn_interpolate.py
+-rw-r--r--   0        0        0      803 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/profile/__init__.py
+-rw-r--r--   0        0        0     4363 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/profile/benchmark.py
+-rw-r--r--   0        0        0    10364 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/profile/profile.py
+-rw-r--r--   0        0        0    16665 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/profile/profiler.py
+-rw-r--r--   0        0        0     4563 2023-05-25 06:05:58.190302 pyg_nightly-2.4.0.dev20230525/torch_geometric/profile/utils.py
+-rw-r--r--   0        0        0     1251 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/resolver.py
+-rw-r--r--   0        0        0      481 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/sampler/__init__.py
+-rw-r--r--   0        0        0    22762 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/sampler/base.py
+-rw-r--r--   0        0        0     2734 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/sampler/hgt_sampler.py
+-rw-r--r--   0        0        0    26144 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/sampler/neighbor_sampler.py
+-rw-r--r--   0        0        0     5252 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/sampler/utils.py
+-rw-r--r--   0        0        0      354 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/seed.py
+-rw-r--r--   0        0        0      710 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/testing/__init__.py
+-rw-r--r--   0        0        0     4368 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/testing/asserts.py
+-rw-r--r--   0        0        0     1933 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/testing/data.py
+-rw-r--r--   0        0        0     3842 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/testing/decorators.py
+-rw-r--r--   0        0        0     1847 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/testing/feature_store.py
+-rw-r--r--   0        0        0     1009 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/testing/graph_store.py
+-rw-r--r--   0        0        0     4136 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/__init__.py
+-rw-r--r--   0        0        0    13964 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/add_metapaths.py
+-rw-r--r--   0        0        0     4836 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/add_positional_encoding.py
+-rw-r--r--   0        0        0     2087 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/add_remaining_self_loops.py
+-rw-r--r--   0        0        0     2018 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/add_self_loops.py
+-rw-r--r--   0        0        0     1255 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/base_transform.py
+-rw-r--r--   0        0        0     1936 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/cartesian.py
+-rw-r--r--   0        0        0      640 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/center.py
+-rw-r--r--   0        0        0     1658 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/compose.py
+-rw-r--r--   0        0        0     1960 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/constant.py
+-rw-r--r--   0        0        0     1222 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/delaunay.py
+-rw-r--r--   0        0        0     1809 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/distance.py
+-rw-r--r--   0        0        0     1034 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/face_to_edge.py
+-rw-r--r--   0        0        0     2952 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/feature_propagation.py
+-rw-r--r--   0        0        0     2367 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/fixed_points.py
+-rw-r--r--   0        0        0     1397 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/gcn_norm.py
+-rw-r--r--   0        0        0    24215 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/gdc.py
+-rw-r--r--   0        0        0     1018 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/generate_mesh_normals.py
+-rw-r--r--   0        0        0     2511 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/grid_sampling.py
+-rw-r--r--   0        0        0     2543 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/knn_graph.py
+-rw-r--r--   0        0        0     2465 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/laplacian_lambda_max.py
+-rw-r--r--   0        0        0     2000 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/largest_connected_components.py
+-rw-r--r--   0        0        0     3723 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/line_graph.py
+-rw-r--r--   0        0        0     1996 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/linear_transformation.py
+-rw-r--r--   0        0        0     1698 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/local_cartesian.py
+-rw-r--r--   0        0        0     1404 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/local_degree_profile.py
+-rw-r--r--   0        0        0     4598 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/mask.py
+-rw-r--r--   0        0        0     6091 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/node_property_split.py
+-rw-r--r--   0        0        0     1028 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/normalize_features.py
+-rw-r--r--   0        0        0     1738 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/normalize_rotation.py
+-rw-r--r--   0        0        0      620 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/normalize_scale.py
+-rw-r--r--   0        0        0     1533 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/one_hot_degree.py
+-rw-r--r--   0        0        0    21975 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/pad.py
+-rw-r--r--   0        0        0     1793 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/point_pair_features.py
+-rw-r--r--   0        0        0     2126 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/polar.py
+-rw-r--r--   0        0        0     2050 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/radius_graph.py
+-rw-r--r--   0        0        0      988 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/random_flip.py
+-rw-r--r--   0        0        0     1510 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/random_jitter.py
+-rw-r--r--   0        0        0    14297 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/random_link_split.py
+-rw-r--r--   0        0        0     5768 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/random_node_split.py
+-rw-r--r--   0        0        0     1903 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/random_rotate.py
+-rw-r--r--   0        0        0     1215 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/random_scale.py
+-rw-r--r--   0        0        0     1319 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/random_shear.py
+-rw-r--r--   0        0        0     1805 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/remove_duplicated_edges.py
+-rw-r--r--   0        0        0     2283 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/remove_isolated_nodes.py
+-rw-r--r--   0        0        0      959 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/remove_training_classes.py
+-rw-r--r--   0        0        0     6111 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/rooted_subgraph.py
+-rw-r--r--   0        0        0     2140 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/sample_points.py
+-rw-r--r--   0        0        0     2128 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/sign.py
+-rw-r--r--   0        0        0     2241 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/spherical.py
+-rw-r--r--   0        0        0     1002 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/svd_feature_reduction.py
+-rw-r--r--   0        0        0     1607 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/target_indegree.py
+-rw-r--r--   0        0        0     2327 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/to_dense.py
+-rw-r--r--   0        0        0     1455 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/to_device.py
+-rw-r--r--   0        0        0     5353 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/to_sparse_tensor.py
+-rw-r--r--   0        0        0     2621 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/to_superpixels.py
+-rw-r--r--   0        0        0     2972 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/to_undirected.py
+-rw-r--r--   0        0        0     1214 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/two_hop.py
+-rw-r--r--   0        0        0     2783 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/virtual_node.py
+-rw-r--r--   0        0        0     9472 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/typing.py
+-rw-r--r--   0        0        0     4549 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/__init__.py
+-rw-r--r--   0        0        0     2347 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/assortativity.py
+-rw-r--r--   0        0        0     9080 2023-05-25 06:05:58.194302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/augmentation.py
+-rw-r--r--   0        0        0     5037 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/coalesce.py
+-rw-r--r--   0        0        0    19630 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/convert.py
+-rw-r--r--   0        0        0     1018 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/degree.py
+-rw-r--r--   0        0        0    11323 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/dropout.py
+-rw-r--r--   0        0        0     1657 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/embedding.py
+-rw-r--r--   0        0        0     4042 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/geodesic.py
+-rw-r--r--   0        0        0     3755 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/get_laplacian.py
+-rw-r--r--   0        0        0     4424 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/get_mesh_laplacian.py
+-rw-r--r--   0        0        0     2536 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/grid.py
+-rw-r--r--   0        0        0     9798 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/hetero.py
+-rw-r--r--   0        0        0     4818 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/homophily.py
+-rw-r--r--   0        0        0     3574 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/isolated.py
+-rw-r--r--   0        0        0    15855 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/loop.py
+-rw-r--r--   0        0        0     1597 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/map.py
+-rw-r--r--   0        0        0     1884 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/mask.py
+-rw-r--r--   0        0        0      608 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/mixin.py
+-rw-r--r--   0        0        0    14643 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/negative_sampling.py
+-rw-r--r--   0        0        0     3344 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/nested.py
+-rw-r--r--   0        0        0     1169 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/normalized_cut.py
+-rw-r--r--   0        0        0     1917 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/num_nodes.py
+-rw-r--r--   0        0        0     1404 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/one_hot.py
+-rw-r--r--   0        0        0     5154 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/random.py
+-rw-r--r--   0        0        0      361 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/repeat.py
+-rw-r--r--   0        0        0     7525 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/scatter.py
+-rw-r--r--   0        0        0     1110 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/segment.py
+-rw-r--r--   0        0        0     2149 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/select.py
+-rw-r--r--   0        0        0     6016 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/smiles.py
+-rw-r--r--   0        0        0     2718 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/softmax.py
+-rw-r--r--   0        0        0     1017 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/sort.py
+-rw-r--r--   0        0        0     3066 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/sort_edge_index.py
+-rw-r--r--   0        0        0    14860 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/sparse.py
+-rw-r--r--   0        0        0     5587 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/spmm.py
+-rw-r--r--   0        0        0    12370 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/subgraph.py
+-rw-r--r--   0        0        0     3439 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/to_dense_adj.py
+-rw-r--r--   0        0        0     4313 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/to_dense_batch.py
+-rw-r--r--   0        0        0     3489 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/train_test_split_edges.py
+-rw-r--r--   0        0        0     4867 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/tree_decomposition.py
+-rw-r--r--   0        0        0     6350 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/trim_to_layer.py
+-rw-r--r--   0        0        0     2125 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/unbatch.py
+-rw-r--r--   0        0        0     5770 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/undirected.py
+-rw-r--r--   0        0        0      123 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/visualization/__init__.py
+-rw-r--r--   0        0        0     4149 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/visualization/graph.py
+-rw-r--r--   0        0        0      388 2023-05-25 06:05:58.198302 pyg_nightly-2.4.0.dev20230525/torch_geometric/visualization/influence.py
+-rw-r--r--   0        0        0    63898 1970-01-01 00:00:00.000000 pyg_nightly-2.4.0.dev20230525/PKG-INFO
```

### Comparing `pyg_nightly-2.4.0.dev20230524/README.md` & `pyg_nightly-2.4.0.dev20230525/README.md`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/pyproject.toml` & `pyg_nightly-2.4.0.dev20230525/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires=["flit_core >=3.2,<4"]
 build-backend="flit_core.buildapi"
 
 [project]
 name="pyg-nightly"
-version="2.4.0.dev20230524"
+version="2.4.0.dev20230525"
 authors=[
     {name="Matthias Fey", email="matthias@pyg.org"},
 ]
 description="Graph Neural Network Library for PyTorch"
 readme="README.md"
 requires-python=">=3.7"
 keywords=[
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/__init__.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from .experimental import (is_experimental_mode_enabled, experimental_mode,
                            set_experimental_mode)
 from .lazy_loader import LazyLoader
 
 contrib = LazyLoader('contrib', globals(), 'torch_geometric.contrib')
 graphgym = LazyLoader('graphgym', globals(), 'torch_geometric.graphgym')
 
-__version__ = '2.4.0.dev20230524'
+__version__ = '2.4.0.dev20230525'
 
 __all__ = [
     'seed_everything',
     'get_home_dir',
     'set_home_dir',
     'compile',
     'is_debug_enabled',
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/compile.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/compile.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/contrib/explain/graphmask_explainer.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/contrib/explain/graphmask_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/contrib/explain/pgm_explainer.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/contrib/explain/pgm_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/contrib/nn/models/rbcd_attack.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/contrib/nn/models/rbcd_attack.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/data/__init__.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/data/batch.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/data/batch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/data/collate.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/data/collate.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/data/data.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/data/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -585,31 +585,28 @@
     def subgraph(self, subset: Tensor) -> 'Data':
         r"""Returns the induced subgraph given by the node indices
         :obj:`subset`.
 
         Args:
             subset (LongTensor or BoolTensor): The nodes to keep.
         """
-        if subset.dtype == torch.bool:
-            num_nodes = int(subset.sum())
-        else:
-            num_nodes = subset.size(0)
-            subset = torch.unique(subset, sorted=True)
-
         out = subgraph(subset, self.edge_index, relabel_nodes=True,
                        num_nodes=self.num_nodes, return_edge_mask=True)
         edge_index, _, edge_mask = out
 
         data = copy.copy(self)
 
         for key, value in self:
             if key == 'edge_index':
                 data.edge_index = edge_index
             elif key == 'num_nodes':
-                data.num_nodes = num_nodes
+                if subset.dtype == torch.bool:
+                    data.num_nodes = int(subset.sum())
+                else:
+                    data.num_nodes = subset.size(0)
             elif self.is_node_attr(key):
                 cat_dim = self.__cat_dim__(key, value)
                 data[key] = select(value, subset, dim=cat_dim)
             elif self.is_edge_attr(key):
                 cat_dim = self.__cat_dim__(key, value)
                 data[key] = select(value, edge_mask, dim=cat_dim)
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/data/datapipes.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/data/datapipes.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/data/dataset.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/data/dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/data/download.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/data/download.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/data/extract.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/data/extract.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/data/feature_store.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/data/feature_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/data/graph_store.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/data/graph_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/data/hetero_data.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/data/hetero_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -634,25 +634,20 @@
             subset_dict (Dict[str, LongTensor or BoolTensor]): A dictionary
                 holding the nodes to keep for each node type.
         """
         data = copy.copy(self)
         subset_dict = copy.copy(subset_dict)
 
         for node_type, subset in subset_dict.items():
-
-            if subset.dtype == torch.bool:
-                num_nodes = int(subset.sum())
-            else:
-                num_nodes = subset.size(0)
-                subset = torch.unique(subset, sorted=True)
-                subset_dict[node_type] = subset
-
             for key, value in self[node_type].items():
                 if key == 'num_nodes':
-                    data[node_type].num_nodes = num_nodes
+                    if subset.dtype == torch.bool:
+                        data[node_type].num_nodes = int(subset.sum())
+                    else:
+                        data[node_type].num_nodes = subset.size(0)
                 elif self[node_type].is_node_attr(key):
                     data[node_type][key] = value[subset]
                 else:
                     data[node_type][key] = value
 
         for edge_type in self.edge_types:
             src, _, dst = edge_type
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/data/in_memory_dataset.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/data/in_memory_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
         if self.slices is None:
             return 1
         for _, value in nested_iter(self.slices):
             return len(value) - 1
         return 0
 
     def get(self, idx: int) -> Data:
+        # TODO (matthias) Avoid unnecessary copy here.
         if self.len() == 1:
             return copy.copy(self._data)
 
         if not hasattr(self, '_data_list') or self._data_list is None:
             self._data_list = self.len() * [None]
         elif self._data_list[idx] is not None:
             return copy.copy(self._data_list[idx])
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/data/lightning/datamodule.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/data/lightning/datamodule.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/data/remote_backend_utils.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/data/remote_backend_utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/data/separate.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/data/separate.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/data/storage.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/data/storage.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/data/summary.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/data/summary.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/data/temporal.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/data/temporal.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/data/view.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/data/view.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/__init__.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/actor.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/actor.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/airfrans.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/airfrans.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/airports.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/airports.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/amazon.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/amazon.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/amazon_products.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/amazon_products.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/aminer.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/aminer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/aqsol.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/aqsol.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/attributed_graph_dataset.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/attributed_graph_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/ba2motif_dataset.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/ba2motif_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/ba_multi_shapes.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/ba_multi_shapes.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/ba_shapes.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/ba_shapes.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/bitcoin_otc.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/bitcoin_otc.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/citation_full.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/citation_full.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/coauthor.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/coauthor.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/coma.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/coma.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/dblp.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/dblp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/dbp15k.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/dbp15k.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/deezer_europe.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/deezer_europe.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/dgraph.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/dgraph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/dynamic_faust.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/dynamic_faust.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/elliptic.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/elliptic.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/elliptic_temporal.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/elliptic_temporal.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/email_eu_core.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/email_eu_core.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/entities.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/entities.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/explainer_dataset.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/explainer_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/facebook.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/facebook.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/fake.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/fake.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/faust.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/faust.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/flickr.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/flickr.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/freebase.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/freebase.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/gdelt.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/gdelt.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/ged_dataset.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/ged_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/gemsec.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/gemsec.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/geometry.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/geometry.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/github.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/github.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/gnn_benchmark_dataset.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/gnn_benchmark_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/graph_generator/ba_graph.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/graph_generator/ba_graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/graph_generator/base.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/graph_generator/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/graph_generator/er_graph.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/graph_generator/er_graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/graph_generator/grid_graph.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/graph_generator/grid_graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/heterophilous_graph_dataset.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/heterophilous_graph_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/hgb_dataset.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/hgb_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/hydro_net.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/hydro_net.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/icews.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/icews.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/imdb.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/infection_dataset.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/infection_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/jodie.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/jodie.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/karate.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/karate.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/last_fm.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/last_fm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/lastfm_asia.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/lastfm_asia.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/linkx_dataset.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/linkx_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/lrgb.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/lrgb.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/malnet_tiny.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/malnet_tiny.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/md17.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/md17.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/mixhop_synthetic_dataset.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/mixhop_synthetic_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/mnist_superpixels.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/mnist_superpixels.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/modelnet.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/modelnet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/molecule_net.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/molecule_net.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/motif_generator/base.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/motif_generator/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/motif_generator/custom.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/motif_generator/custom.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/motif_generator/cycle.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/motif_generator/cycle.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/motif_generator/house.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/motif_generator/house.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/movie_lens.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/movie_lens.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/movie_lens_100k.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/movie_lens_100k.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/nell.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/nell.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/ogb_mag.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/ogb_mag.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/omdb.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/omdb.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/particle.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/particle.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/pascal.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/pascal.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/pascal_pf.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/pascal_pf.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/pcpnet_dataset.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/pcpnet_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/planetoid.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/planetoid.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/polblogs.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/polblogs.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/ppi.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/ppi.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/qm7.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/qm7.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/qm9.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/qm9.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/reddit.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/reddit.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/reddit2.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/reddit2.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/rel_link_pred_dataset.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/rel_link_pred_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/s3dis.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/s3dis.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/sbm_dataset.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/sbm_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/shapenet.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/shapenet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/shrec2016.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/shrec2016.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/snap_dataset.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/snap_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/suite_sparse.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/suite_sparse.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/taobao.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/taobao.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/tosca.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/tosca.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/tu_dataset.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/tu_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/twitch.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/twitch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/upfd.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/upfd.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/utils/cheatsheet.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/utils/cheatsheet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/webkb.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/webkb.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/wikics.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/wikics.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/wikipedia_network.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/wikipedia_network.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/willow_object_class.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/willow_object_class.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/word_net.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/word_net.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/yelp.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/yelp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/datasets/zinc.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/datasets/zinc.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/debug.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/debug.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/deprecation.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/deprecation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/experimental.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/experimental.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/algorithm/attention_explainer.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/algorithm/attention_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/algorithm/base.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/algorithm/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/algorithm/captum.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/algorithm/captum.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/algorithm/captum_explainer.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/algorithm/captum_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/algorithm/dummy_explainer.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/algorithm/dummy_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/algorithm/gnn_explainer.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/algorithm/gnn_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/algorithm/pg_explainer.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/algorithm/pg_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/algorithm/utils.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/algorithm/utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/config.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/config.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/explainer.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/explanation.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/explanation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/metric/basic.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/metric/basic.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/metric/faithfulness.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/metric/faithfulness.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/explain/metric/fidelity.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/explain/metric/fidelity.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/__init__.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/checkpoint.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/checkpoint.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/cmd_args.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/cmd_args.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/config.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/config.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/config_store.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/config_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/contrib/layer/generalconv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/contrib/layer/generalconv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/loader.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/logger.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/logger.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/loss.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/loss.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/model_builder.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/model_builder.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/models/__init__.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/models/act.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/models/act.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/models/encoder.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/models/encoder.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/models/gnn.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/models/gnn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/models/head.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/models/head.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/models/layer.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/models/layer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/models/transform.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/models/transform.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/optim.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/optim.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/register.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/register.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/train.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/train.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/utils/__init__.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/utils/agg_runs.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/utils/agg_runs.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/utils/comp_budget.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/utils/comp_budget.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/utils/device.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/utils/device.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/utils/epoch.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/utils/epoch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/utils/io.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/utils/io.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/graphgym/utils/plot.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/graphgym/utils/plot.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/home.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/home.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/io/__init__.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/io/npz.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/io/npz.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/io/obj.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/io/obj.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/io/off.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/io/off.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/io/planetoid.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/io/planetoid.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/io/sdf.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/io/sdf.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/io/tu.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/io/tu.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/io/txt_array.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/io/txt_array.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/lazy_loader.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/__init__.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/base.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/data_list_loader.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/data_list_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/dataloader.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/dataloader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/dense_data_loader.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/dense_data_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/dynamic_batch_sampler.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/dynamic_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/graph_saint.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/graph_saint.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/hgt_loader.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/hgt_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/imbalanced_sampler.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/imbalanced_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/link_loader.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/link_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/link_neighbor_loader.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/link_neighbor_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/mixin.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/mixin.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/neighbor_loader.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/neighbor_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/neighbor_sampler.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/neighbor_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/node_loader.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/node_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/prefetch.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/prefetch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/random_node_loader.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/random_node_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/shadow.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/shadow.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/temporal_dataloader.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/temporal_dataloader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/utils.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/loader/zip_loader.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/loader/zip_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/logging.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/logging.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/__init__.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/__init__.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/attention.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/attention.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/base.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/basic.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/basic.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/deep_sets.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/deep_sets.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/equilibrium.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/equilibrium.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/fused.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/fused.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/gmt.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/gmt.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/gru.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/gru.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/lstm.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/lstm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/mlp.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/mlp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/multi.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/multi.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/quantile.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/quantile.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,17 @@
             if self.interpolation == 'linear':
                 q_frac = q_point.frac().view(shape)
                 quantile = l_quant + (r_quant - l_quant) * q_frac
             else:  # 'midpoint'
                 quantile = 0.5 * l_quant + 0.5 * r_quant
 
         # If the number of elements is zero, fill with pre-defined value:
-        mask = (count == 0).repeat_interleave(self.q.numel()).view(shape)
+        repeats = self.q.numel()
+        mask = (count == 0).repeat_interleave(
+            repeats, output_size=repeats * count.numel()).view(shape)
         out = quantile.masked_fill(mask, self.fill_value)
 
         if self.q.numel() > 1:
             shape = list(out.shape)
             shape = (shape[:dim] + [shape[dim] // self.q.numel(), -1] +
                      shape[dim + 2:])
             out = out.view(shape)
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/scaler.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/scaler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/set2set.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/set2set.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/set_transformer.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/set_transformer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/sort.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/sort.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/aggr/utils.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/aggr/utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/__init__.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/agnn_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/agnn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/antisymmetric_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/antisymmetric_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/appnp.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/appnp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/arma_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/arma_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/cg_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/cg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/cheb_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/cheb_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/cluster_gcn_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/cluster_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/cugraph/base.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/cugraph/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/cugraph/gat_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/cugraph/gat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/cugraph/rgcn_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/cugraph/rgcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/cugraph/sage_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/cugraph/sage_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/dna_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/dna_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/edge_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/edge_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/eg_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/eg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/fa_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/fa_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/feast_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/feast_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/film_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/film_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/fused_gat_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/fused_gat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/gat_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/gat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/gated_graph_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/gated_graph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/gatv2_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/gatv2_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/gcn2_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/gcn2_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/gcn_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/gcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/gen_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/gen_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/general_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/general_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/gin_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/gin_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/gmm_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/gmm_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/gps_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/gps_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/graph_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/graph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/gravnet_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/gravnet_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/han_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/han_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/heat_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/heat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/hetero_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/hetero_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/hgt_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/hgt_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/hypergraph_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/hypergraph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/le_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/le_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/lg_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/lg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/message_passing.jinja` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/message_passing.jinja`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/message_passing.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/message_passing.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/mf_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/mf_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/nn_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/nn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/pan_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/pan_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/pdn_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/pdn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/pna_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/pna_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/point_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/point_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/point_gnn_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/point_gnn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/point_transformer_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/point_transformer_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/ppf_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/ppf_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/res_gated_graph_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/res_gated_graph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/rgat_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/rgat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/rgcn_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/rgcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/sage_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/sage_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/sg_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/sg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/signed_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/signed_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/simple_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/simple_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/spline_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/spline_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/ssg_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/ssg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/supergat_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/supergat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/tag_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/tag_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/transformer_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/transformer_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/utils/__init__.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/utils/cheatsheet.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/utils/cheatsheet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/utils/inspector.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/utils/inspector.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/utils/jit.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/utils/jit.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/utils/typing.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/utils/typing.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/wl_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/wl_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/wl_conv_continuous.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/wl_conv_continuous.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/conv/x_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/conv/x_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/data_parallel.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/data_parallel.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/dense/__init__.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/dense/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/dense/dense_gat_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/dense/dense_gat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/dense/dense_gcn_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/dense/dense_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/dense/dense_gin_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/dense/dense_gin_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/dense/dense_graph_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/dense/dense_graph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/dense/dense_sage_conv.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/dense/dense_sage_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/dense/diff_pool.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/dense/diff_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/dense/dmon_pool.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/dense/dmon_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/dense/linear.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/dense/linear.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/dense/mincut_pool.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/dense/mincut_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/encoding.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/encoding.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/functional/bro.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/functional/bro.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/functional/gini.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/functional/gini.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/fx.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/fx.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/glob.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/glob.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/inits.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/inits.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/kge/base.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/kge/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/kge/complex.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/kge/complex.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/kge/distmult.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/kge/distmult.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/kge/loader.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/kge/loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/kge/rotate.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/kge/rotate.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/kge/transe.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/kge/transe.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/lr_scheduler.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/model_hub.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/model_hub.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/__init__.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/attentive_fp.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/attentive_fp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/autoencoder.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/basic_gnn.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/basic_gnn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/captum.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/captum.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/correct_and_smooth.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/correct_and_smooth.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/deep_graph_infomax.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/deep_graph_infomax.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/deepgcn.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/deepgcn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/dimenet.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/dimenet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/dimenet_utils.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/dimenet_utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/gnnff.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/gnnff.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/graph_unet.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/graph_unet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/jumping_knowledge.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/jumping_knowledge.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/label_prop.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/label_prop.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/lightgcn.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/lightgcn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/linkx.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/linkx.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/mask_label.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/mask_label.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/meta.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/meta.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/metapath2vec.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/metapath2vec.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/mlp.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/mlp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/node2vec.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/node2vec.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/pmlp.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/pmlp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/re_net.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/re_net.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/rect.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/rect.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/rev_gnn.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/rev_gnn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/schnet.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/schnet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/signed_gcn.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/signed_gcn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/models/tgn.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/models/tgn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/module_dict.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/module_dict.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/norm/__init__.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/norm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/norm/batch_norm.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/norm/batch_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/norm/diff_group_norm.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/norm/diff_group_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/norm/graph_norm.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/norm/graph_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/norm/graph_size_norm.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/norm/graph_size_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/norm/instance_norm.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/norm/instance_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/norm/layer_norm.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/norm/layer_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/norm/mean_subtraction_norm.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/norm/mean_subtraction_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/norm/msg_norm.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/norm/msg_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/norm/pair_norm.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/norm/pair_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/parameter_dict.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/parameter_dict.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/__init__.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/asap.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/asap.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/avg_pool.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/avg_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/connect/base.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/connect/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/decimation.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/decimation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/edge_pool.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/edge_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/glob.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/glob.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/graclus.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/graclus.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/max_pool.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/max_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/mem_pool.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/mem_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/pan_pool.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/pan_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/pool.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/sag_pool.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/sag_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/select/base.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/select/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/select/topk.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/select/topk.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/topk_pool.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/topk_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/pool/voxel_grid.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/pool/voxel_grid.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/resolver.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/resolver.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/sequential.jinja` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/sequential.jinja`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/sequential.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/sequential.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/summary.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/summary.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/to_fixed_size_transformer.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/to_fixed_size_transformer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/to_hetero_module.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/to_hetero_module.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/to_hetero_transformer.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/to_hetero_transformer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/to_hetero_with_bases_transformer.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/to_hetero_with_bases_transformer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/nn/unpool/knn_interpolate.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/nn/unpool/knn_interpolate.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/profile/__init__.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/profile/benchmark.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/profile/benchmark.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/profile/profile.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/profile/profile.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/profile/profiler.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/profile/profiler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/profile/utils.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/profile/utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/resolver.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/resolver.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/sampler/base.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/sampler/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/sampler/hgt_sampler.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/sampler/hgt_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/sampler/neighbor_sampler.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/sampler/neighbor_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/sampler/utils.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/sampler/utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/testing/__init__.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/testing/asserts.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/testing/asserts.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/testing/data.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/testing/data.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/testing/decorators.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/testing/decorators.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/testing/feature_store.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/testing/feature_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/testing/graph_store.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/testing/graph_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/__init__.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/add_metapaths.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/add_metapaths.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         self.metapaths = metapaths
         self.drop_orig_edge_types = drop_orig_edge_types
         self.keep_same_node_type = keep_same_node_type
         self.drop_unconnected_node_types = drop_unconnected_node_types
         self.max_sample = max_sample
         self.weighted = weighted
 
-    def __call__(self, data: HeteroData) -> HeteroData:
+    def forward(self, data: HeteroData) -> HeteroData:
         edge_types = data.edge_types  # save original edge types
         data.metapath_dict = {}
 
         for j, metapath in enumerate(self.metapaths):
             for edge_type in metapath:
                 assert data._to_canonical(
                     edge_type) in edge_types, f"'{edge_type}' not present"
@@ -240,15 +240,15 @@
         self.drop_unconnected_node_types = drop_unconnected_node_types
         self.sample_ratio = sample_ratio
         if isinstance(walks_per_node, int):
             walks_per_node = [walks_per_node] * len(metapaths)
         assert len(walks_per_node) == len(metapaths)
         self.walks_per_node = walks_per_node
 
-    def __call__(self, data: HeteroData) -> HeteroData:
+    def forward(self, data: HeteroData) -> HeteroData:
         edge_types = data.edge_types  # save original edge types
         data.metapath_dict = {}
 
         for j, metapath in enumerate(self.metapaths):
             for edge_type in metapath:
                 assert data._to_canonical(
                     edge_type) in edge_types, f"'{edge_type}' not present"
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/add_positional_encoding.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/add_positional_encoding.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         **kwargs,
     ):
         self.k = k
         self.attr_name = attr_name
         self.is_undirected = is_undirected
         self.kwargs = kwargs
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         from scipy.sparse.linalg import eigs, eigsh
         eig_fn = eigs if not self.is_undirected else eigsh
 
         num_nodes = data.num_nodes
         edge_index, edge_weight = get_laplacian(
             data.edge_index,
             data.edge_weight,
@@ -113,15 +113,15 @@
         self,
         walk_length: int,
         attr_name: Optional[str] = 'random_walk_pe',
     ):
         self.walk_length = walk_length
         self.attr_name = attr_name
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         row, col = data.edge_index
         N = data.num_nodes
 
         value = data.edge_weight
         if value is None:
             value = torch.ones(data.num_edges, device=row.device)
         value = scatter(value, row, dim_size=N, reduce='sum').clamp(min=1)[row]
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/add_remaining_self_loops.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/add_remaining_self_loops.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             :obj:`"min"`, :obj:`"max"`, :obj:`"mul"`). (default: :obj:`1.`)
     """
     def __init__(self, attr: Optional[str] = 'edge_weight',
                  fill_value: Union[float, Tensor, str] = 1.0):
         self.attr = attr
         self.fill_value = fill_value
 
-    def __call__(
+    def forward(
         self,
         data: Union[Data, HeteroData],
     ) -> Union[Data, HeteroData]:
         for store in data.edge_stores:
             if store.is_bipartite() or 'edge_index' not in store:
                 continue
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/add_self_loops.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/add_self_loops.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             :obj:`"min"`, :obj:`"max"`, :obj:`"mul"`). (default: :obj:`1.`)
     """
     def __init__(self, attr: Optional[str] = 'edge_weight',
                  fill_value: Union[float, Tensor, str] = 1.0):
         self.attr = attr
         self.fill_value = fill_value
 
-    def __call__(
+    def forward(
         self,
         data: Union[Data, HeteroData],
     ) -> Union[Data, HeteroData]:
         for store in data.edge_stores:
             if store.is_bipartite() or 'edge_index' not in store:
                 continue
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/base_transform.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/base_transform.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from abc import ABC
+import copy
+from abc import ABC, abstractmethod
 from typing import Any
 
 
 class BaseTransform(ABC):
     r"""An abstract base class for writing transforms.
 
     Transforms are a general way to modify and customize
@@ -23,11 +24,15 @@
         dataset = TUDataset(path, name='MUTAG', transform=transform)
         data = dataset[0]  # Implicitly transform data on every access.
 
         data = TUDataset(path, name='MUTAG')[0]
         data = transform(data)  # Explicitly transform data.
     """
     def __call__(self, data: Any) -> Any:
-        raise NotImplementedError
+        return self.forward(copy.copy(data))
+
+    @abstractmethod
+    def forward(self, data: Any) -> Any:
+        pass
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}()'
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/cartesian.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/cartesian.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         max_value: Optional[float] = None,
         cat: bool = True,
     ):
         self.norm = norm
         self.max = max_value
         self.cat = cat
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         (row, col), pos, pseudo = data.edge_index, data.pos, data.edge_attr
 
         cart = pos[row] - pos[col]
         cart = cart.view(-1, 1) if cart.dim() == 1 else cart
 
         if self.norm and cart.numel() > 0:
             max_value = cart.abs().max() if self.max is None else self.max
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/center.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/center.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from torch_geometric.transforms import BaseTransform
 
 
 @functional_transform('center')
 class Center(BaseTransform):
     r"""Centers node positions :obj:`data.pos` around the origin
     (functional name: :obj:`center`)."""
-    def __call__(
+    def forward(
         self,
         data: Union[Data, HeteroData],
     ) -> Union[Data, HeteroData]:
         for store in data.node_stores:
             if hasattr(store, 'pos'):
                 store.pos = store.pos - store.pos.mean(dim=-2, keepdim=True)
         return data
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/compose.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/compose.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     Args:
         transforms (List[Callable]): List of transforms to compose.
     """
     def __init__(self, transforms: List[Callable]):
         self.transforms = transforms
 
-    def __call__(
+    def forward(
         self,
         data: Union[Data, HeteroData],
     ) -> Union[Data, HeteroData]:
         for transform in self.transforms:
             if isinstance(data, (list, tuple)):
                 data = [transform(d) for d in data]
             else:
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/constant.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/constant.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         if isinstance(node_types, str):
             node_types = [node_types]
 
         self.value = value
         self.cat = cat
         self.node_types = node_types
 
-    def __call__(
+    def forward(
         self,
         data: Union[Data, HeteroData],
     ) -> Union[Data, HeteroData]:
 
         for store in data.node_stores:
             if self.node_types is None or store._key in self.node_types:
                 num_nodes = store.num_nodes
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/delaunay.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/delaunay.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from torch_geometric.transforms import BaseTransform
 
 
 @functional_transform('delaunay')
 class Delaunay(BaseTransform):
     r"""Computes the delaunay triangulation of a set of points
     (functional name: :obj:`delaunay`)."""
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         if data.pos.size(0) < 2:
             data.edge_index = torch.tensor([], dtype=torch.long,
                                            device=data.pos.device).view(2, 0)
         if data.pos.size(0) == 2:
             data.edge_index = torch.tensor([[0, 1], [1, 0]], dtype=torch.long,
                                            device=data.pos.device)
         elif data.pos.size(0) == 3:
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/distance.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/distance.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     """
     def __init__(self, norm: bool = True, max_value: Optional[float] = None,
                  cat: bool = True):
         self.norm = norm
         self.max = max_value
         self.cat = cat
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         (row, col), pos, pseudo = data.edge_index, data.pos, data.edge_attr
 
         dist = torch.norm(pos[col] - pos[row], p=2, dim=-1).view(-1, 1)
 
         if self.norm and dist.numel() > 0:
             dist = dist / (dist.max() if self.max is None else self.max)
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/face_to_edge.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/face_to_edge.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Args:
         remove_faces (bool, optional): If set to :obj:`False`, the face tensor
             will not be removed.
     """
     def __init__(self, remove_faces: bool = True):
         self.remove_faces = remove_faces
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         if hasattr(data, 'face'):
             face = data.face
             edge_index = torch.cat([face[:2], face[1:], face[::2]], dim=1)
             edge_index = to_undirected(edge_index, num_nodes=data.num_nodes)
 
             data.edge_index = edge_index
             if self.remove_faces:
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/feature_propagation.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/feature_propagation.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         num_iterations (int, optional): The number of propagations.
             (default: :obj:`40`)
     """
     def __init__(self, missing_mask: Tensor, num_iterations: int = 40):
         self.missing_mask = missing_mask
         self.num_iterations = num_iterations
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         assert 'edge_index' in data or 'adj_t' in data
         assert data.x.size() == self.missing_mask.size()
 
         missing_mask = self.missing_mask.to(data.x.device)
         known_mask = ~missing_mask
 
         if 'edge_index' in data:
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/fixed_points.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/fixed_points.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         replace: bool = True,
         allow_duplicates: bool = False,
     ):
         self.num = num
         self.replace = replace
         self.allow_duplicates = allow_duplicates
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         num_nodes = data.num_nodes
 
         if self.replace:
             choice = np.random.choice(num_nodes, self.num, replace=True)
             choice = torch.from_numpy(choice).to(torch.long)
         elif not self.allow_duplicates:
             choice = torch.randperm(num_nodes)[:self.num]
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/gcn_norm.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/gcn_norm.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         \mathbf{\hat{D}}^{-1/2}
 
     where :math:`\hat{D}_{ii} = \sum_{j=0} \hat{A}_{ij} + 1`.
     """
     def __init__(self, add_self_loops: bool = True):
         self.add_self_loops = add_self_loops
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         gcn_norm = torch_geometric.nn.conv.gcn_conv.gcn_norm
         assert 'edge_index' in data or 'adj_t' in data
 
         if 'edge_index' in data:
             data.edge_index, data.edge_weight = gcn_norm(
                 data.edge_index, data.edge_weight, data.num_nodes,
                 add_self_loops=self.add_self_loops)
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/gdc.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/gdc.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         self.sparsification_kwargs = sparsification_kwargs
         self.exact = exact
 
         if self_loop_weight:
             assert exact or self_loop_weight == 1
 
     @torch.no_grad()
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         N = data.num_nodes
         edge_index = data.edge_index
         if data.edge_attr is None:
             edge_weight = torch.ones(edge_index.size(1),
                                      device=edge_index.device)
         else:
             edge_weight = data.edge_attr
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/generate_mesh_normals.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/generate_mesh_normals.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from torch_geometric.utils import scatter
 
 
 @functional_transform('generate_mesh_normals')
 class GenerateMeshNormals(BaseTransform):
     r"""Generate normal vectors for each mesh node based on neighboring
     faces (functional name: :obj:`generate_mesh_normals`)."""
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         assert 'face' in data
         pos, face = data.pos, data.face
 
         vec1 = pos[face[1]] - pos[face[0]]
         vec2 = pos[face[2]] - pos[face[0]]
         face_norm = F.normalize(vec1.cross(vec2), p=2, dim=-1)  # [F, 3]
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/grid_sampling.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/grid_sampling.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def __init__(self, size: Union[float, List[float], Tensor],
                  start: Optional[Union[float, List[float], Tensor]] = None,
                  end: Optional[Union[float, List[float], Tensor]] = None):
         self.size = size
         self.start = start
         self.end = end
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         num_nodes = data.num_nodes
 
         batch = data.get('batch', None)
 
         c = torch_geometric.nn.voxel_grid(data.pos, self.size, batch,
                                           self.start, self.end)
         c, perm = torch_geometric.nn.pool.consecutive.consecutive_cluster(c)
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/knn_graph.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/knn_graph.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self.k = k
         self.loop = loop
         self.force_undirected = force_undirected
         self.flow = flow
         self.cosine = cosine
         self.num_workers = num_workers
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         data.edge_attr = None
         batch = data.batch if 'batch' in data else None
 
         edge_index = torch_geometric.nn.knn_graph(
             data.pos,
             self.k,
             batch,
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/laplacian_lambda_max.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/laplacian_lambda_max.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         normalization: Optional[str] = None,
         is_undirected: bool = False,
     ):
         assert normalization in [None, 'sym', 'rw'], 'Invalid normalization'
         self.normalization = normalization
         self.is_undirected = is_undirected
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         edge_weight = data.edge_attr
         if edge_weight is not None and edge_weight.numel() != data.num_edges:
             edge_weight = None
 
         edge_index, edge_weight = get_laplacian(data.edge_index, edge_weight,
                                                 self.normalization,
                                                 num_nodes=data.num_nodes)
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/largest_connected_components.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/largest_connected_components.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             (default: :obj:`'weak'`)
     """
     def __init__(self, num_components: int = 1, connection: str = 'weak'):
         assert connection in ['strong', 'weak'], 'Unknown connection type'
         self.num_components = num_components
         self.connection = connection
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         import numpy as np
         import scipy.sparse as sp
 
         adj = to_scipy_sparse_matrix(data.edge_index, num_nodes=data.num_nodes)
 
         num_components, component = sp.csgraph.connected_components(
             adj, connection=self.connection)
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/line_graph.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/line_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     Args:
         force_directed (bool, optional): If set to :obj:`True`, the graph will
             be always treated as a directed graph. (default: :obj:`False`)
     """
     def __init__(self, force_directed: bool = False):
         self.force_directed = force_directed
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         N = data.num_nodes
         edge_index, edge_attr = data.edge_index, data.edge_attr
         edge_index, edge_attr = coalesce(edge_index, edge_attr, num_nodes=N)
         row, col = edge_index
 
         if self.force_directed or data.is_directed():
             i = torch.arange(row.size(0), dtype=torch.long, device=row.device)
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/linear_transformation.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/linear_transformation.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,18 +22,18 @@
             matrix = torch.tensor(matrix)
         assert matrix.dim() == 2, (
             'Transformation matrix should be two-dimensional.')
         assert matrix.size(0) == matrix.size(1), (
             f'Transformation matrix should be square (got {matrix.size()})')
 
         # Store the matrix as its transpose.
-        # We do this to enable post-multiplication in `__call__`.
+        # We do this to enable post-multiplication in `forward`.
         self.matrix = matrix.t()
 
-    def __call__(
+    def forward(
         self,
         data: Union[Data, HeteroData],
     ) -> Union[Data, HeteroData]:
         for store in data.node_stores:
             if not hasattr(store, 'pos'):
                 continue
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/local_cartesian.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/local_cartesian.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         cat (bool, optional): If set to :obj:`False`, all existing edge
             attributes will be replaced. (default: :obj:`True`)
     """
     def __init__(self, norm: bool = True, cat: bool = True):
         self.norm = norm
         self.cat = cat
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         (row, col), pos, pseudo = data.edge_index, data.pos, data.edge_attr
 
         cart = pos[row] - pos[col]
         cart = cart.view(-1, 1) if cart.dim() == 1 else cart
 
         max_value = scatter(cart.abs(), col, 0, pos.size(0), reduce='max')
         max_value = max_value.max(dim=-1, keepdim=True)[0]
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/local_degree_profile.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/local_degree_profile.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     to the node features, where :math:`DN(i) = \{ \deg(j) \mid j \in
     \mathcal{N}(i) \}`.
     """
     def __init__(self):
         from torch_geometric.nn.aggr.fused import FusedAggregation
         self.aggr = FusedAggregation(['min', 'max', 'mean', 'std'])
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         row, col = data.edge_index
         N = data.num_nodes
 
         deg = degree(row, N, dtype=torch.float).view(-1, 1)
         xs = [deg] + self.aggr(deg[col], row, dim_size=N)
 
         if data.x is not None:
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/mask.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/mask.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         sizes: Optional[Union[int, List[int]]] = None,
         replace: bool = False,
     ):
         self.attrs = [attrs] if isinstance(attrs, str) else attrs
         self.sizes = sizes
         self.replace = replace
 
-    def __call__(
+    def forward(
         self,
         data: Union[Data, HeteroData],
     ) -> Union[Data, HeteroData]:
         for store in data.stores:
             attrs = get_attrs_with_suffix(self.attrs, store, '_index')
 
             sizes = self.sizes or ([None] * len(attrs))
@@ -102,15 +102,15 @@
         self,
         attrs: Optional[Union[str, List[str]]] = None,
         replace: bool = False,
     ):
         self.attrs = [attrs] if isinstance(attrs, str) else attrs
         self.replace = replace
 
-    def __call__(
+    def forward(
         self,
         data: Union[Data, HeteroData],
     ) -> Union[Data, HeteroData]:
         for store in data.stores:
             attrs = get_attrs_with_suffix(self.attrs, store, '_mask')
 
             for attr in attrs:
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/node_property_split.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/node_property_split.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,16 +77,15 @@
             raise ValueError(f"'ratios' must sum to 1.0 (got {sum(ratios)})")
 
         self.property_name = property_name
         self.compute_fn = _property_name_to_compute_fn[property_name]
         self.ratios = ratios
         self.ascending = ascending
 
-    def __call__(self, data: Data) -> Data:
-
+    def forward(self, data: Data) -> Data:
         G = to_networkx(data, to_undirected=True, remove_self_loops=True)
         property_values = self.compute_fn(G, self.ascending)
         mask_dict = self._mask_nodes_by_property(property_values, self.ratios)
 
         for key, mask in mask_dict.items():
             data[key] = mask
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/normalize_features.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/normalize_features.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Args:
         attrs (List[str]): The names of attributes to normalize.
             (default: :obj:`["x"]`)
     """
     def __init__(self, attrs: List[str] = ["x"]):
         self.attrs = attrs
 
-    def __call__(
+    def forward(
         self,
         data: Union[Data, HeteroData],
     ) -> Union[Data, HeteroData]:
         for store in data.stores:
             for key, value in store.items(*self.attrs):
                 if value.numel() > 0:
                     value = value - value.min()
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/normalize_rotation.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/normalize_rotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         sort (bool, optional): If set to :obj:`True`, will sort eigenvectors
             according to their eigenvalues. (default: :obj:`False`)
     """
     def __init__(self, max_points: int = -1, sort: bool = False):
         self.max_points = max_points
         self.sort = sort
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         pos = data.pos
 
         if self.max_points > 0 and pos.size(0) > self.max_points:
             perm = torch.randperm(pos.size(0))
             pos = pos[perm[:self.max_points]]
 
         pos = pos - pos.mean(dim=0, keepdim=True)
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/normalize_scale.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/normalize_scale.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 class NormalizeScale(BaseTransform):
     r"""Centers and normalizes node positions to the interval :math:`(-1, 1)`
     (functional name: :obj:`normalize_scale`).
     """
     def __init__(self):
         self.center = Center()
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         data = self.center(data)
 
         scale = (1 / data.pos.abs().max()) * 0.999999
         data.pos = data.pos * scale
 
         return data
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/one_hot_degree.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/one_hot_degree.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         in_degree: bool = False,
         cat: bool = True,
     ):
         self.max_degree = max_degree
         self.in_degree = in_degree
         self.cat = cat
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         idx, x = data.edge_index[1 if self.in_degree else 0], data.x
         deg = degree(idx, data.num_nodes, dtype=torch.long)
         deg = one_hot(deg, num_classes=self.max_degree + 1)
 
         if x is not None and self.cat:
             x = x.view(-1, 1) if x.dim() == 1 else x
             data.x = torch.cat([x, deg.to(x.dtype)], dim=-1)
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/pad.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/pad.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,15 +395,15 @@
         return self.node_pad.get_value(node_type, attr_name)
 
     def __get_edge_padding(
             self, attr_name: str,
             edge_type: Optional[EdgeType] = None) -> Union[int, float]:
         return self.edge_pad.get_value(edge_type, attr_name)
 
-    def __call__(
+    def forward(
         self,
         data: Union[Data, HeteroData],
     ) -> Union[Data, HeteroData]:
 
         if isinstance(data, Data):
             assert isinstance(self.node_pad, (UniformPadding, AttrNamePadding))
             assert isinstance(self.edge_pad, (UniformPadding, AttrNamePadding))
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/point_pair_features.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/point_pair_features.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Args:
         cat (bool, optional): If set to :obj:`False`, all existing edge
             attributes will be replaced. (default: :obj:`True`)
     """
     def __init__(self, cat: bool = True):
         self.cat = cat
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         ppf_func = torch_geometric.nn.conv.ppf_conv.point_pair_features
 
         assert data.edge_index is not None
         assert data.pos is not None and data.norm is not None
         assert data.pos.size(-1) == 3
         assert data.pos.size() == data.norm.size()
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/polar.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/polar.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         max_value: Optional[float] = None,
         cat: bool = True,
     ):
         self.norm = norm
         self.max = max_value
         self.cat = cat
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         (row, col), pos, pseudo = data.edge_index, data.pos, data.edge_attr
         assert pos.dim() == 2 and pos.size(1) == 2
 
         cart = pos[col] - pos[row]
 
         rho = torch.norm(cart, p=2, dim=-1).view(-1, 1)
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/radius_graph.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/radius_graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     ):
         self.r = r
         self.loop = loop
         self.max_num_neighbors = max_num_neighbors
         self.flow = flow
         self.num_workers = num_workers
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         data.edge_attr = None
         batch = data.batch if 'batch' in data else None
 
         data.edge_index = torch_geometric.nn.radius_graph(
             data.pos,
             self.r,
             batch,
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/random_flip.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/random_flip.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         p (float, optional): Probability that node positions will be flipped.
             (default: :obj:`0.5`)
     """
     def __init__(self, axis: int, p: float = 0.5):
         self.axis = axis
         self.p = p
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         if random.random() < self.p:
             pos = data.pos.clone()
             pos[..., self.axis] = -pos[..., self.axis]
             data.pos = pos
         return data
 
     def __repr__(self) -> str:
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/random_jitter.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/random_jitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             :math:`(-\mathrm{translate}, +\mathrm{translate})` to sample from.
             If :obj:`translate` is a number instead of a sequence, the same
             range is used for each dimension.
     """
     def __init__(self, translate: Union[float, int, Sequence]):
         self.translate = translate
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         (n, dim), t = data.pos.size(), self.translate
         if isinstance(t, numbers.Number):
             t = list(repeat(t, times=dim))
         assert len(t) == dim
 
         ts = []
         for d in range(dim):
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/random_link_split.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/random_link_split.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         self.split_labels = split_labels
         self.add_negative_train_samples = add_negative_train_samples
         self.neg_sampling_ratio = neg_sampling_ratio
         self.disjoint_train_ratio = disjoint_train_ratio
         self.edge_types = edge_types
         self.rev_edge_types = rev_edge_types
 
-    def __call__(
+    def forward(
         self,
         data: Union[Data, HeteroData],
     ) -> Union[Data, HeteroData]:
         edge_types = self.edge_types
         rev_edge_types = self.rev_edge_types
 
         train_data, val_data, test_data = copy(data), copy(data), copy(data)
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/random_node_split.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/random_node_split.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         self.split = split
         self.num_splits = num_splits
         self.num_train_per_class = num_train_per_class
         self.num_val = num_val
         self.num_test = num_test
         self.key = key
 
-    def __call__(
+    def forward(
         self,
         data: Union[Data, HeteroData],
     ) -> Union[Data, HeteroData]:
         for store in data.node_stores:
             if self.key is not None and not hasattr(store, self.key):
                 continue
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/random_rotate.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/random_rotate.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                  axis: int = 0):
         if isinstance(degrees, numbers.Number):
             degrees = (-abs(degrees), abs(degrees))
         assert isinstance(degrees, (tuple, list)) and len(degrees) == 2
         self.degrees = degrees
         self.axis = axis
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         degree = math.pi * random.uniform(*self.degrees) / 180.0
         sin, cos = math.sin(degree), math.cos(degree)
 
         if data.pos.size(-1) == 2:
             matrix = [[cos, sin], [-sin, cos]]
         else:
             if self.axis == 0:
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/random_scale.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/random_scale.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,14 @@
             is randomly sampled from the range
             :math:`a \leq \mathrm{scale} \leq b`.
     """
     def __init__(self, scales: Tuple[float, float]):
         assert isinstance(scales, (tuple, list)) and len(scales) == 2
         self.scales = scales
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         scale = random.uniform(*self.scales)
         data.pos = data.pos * scale
         return data
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}({self.scales})'
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/random_shear.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/random_shear.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     Args:
         shear (float or int): maximum shearing factor defining the range
             :math:`(-\mathrm{shear}, +\mathrm{shear})` to sample from.
     """
     def __init__(self, shear: Union[float, int]):
         self.shear = abs(shear)
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         dim = data.pos.size(-1)
 
         matrix = data.pos.new_empty(dim, dim).uniform_(-self.shear, self.shear)
         eye = torch.arange(dim, dtype=torch.long)
         matrix[eye, eye] = 1
 
         return LinearTransformation(matrix)(data)
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/remove_duplicated_edges.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/remove_duplicated_edges.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     ):
         if isinstance(key, str):
             key = [key]
 
         self.keys = key
         self.reduce = reduce
 
-    def __call__(
+    def forward(
         self,
         data: Union[Data, HeteroData],
     ) -> Union[Data, HeteroData]:
 
         for store in data.edge_stores:
             keys = [key for key in self.keys if key in store]
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/remove_isolated_nodes.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/remove_isolated_nodes.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from torch_geometric.transforms import BaseTransform
 
 
 @functional_transform('remove_isolated_nodes')
 class RemoveIsolatedNodes(BaseTransform):
     r"""Removes isolated nodes from the graph
     (functional name: :obj:`remove_isolated_nodes`)."""
-    def __call__(
+    def forward(
         self,
         data: Union[Data, HeteroData],
     ) -> Union[Data, HeteroData]:
         # Gather all nodes that occur in at least one edge (across all types):
         n_id_dict = defaultdict(list)
         for store in data.edge_stores:
             if 'edge_index' not in store:
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/remove_training_classes.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/remove_training_classes.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     Args:
         classes (List[int]): The classes to remove from the training set.
     """
     def __init__(self, classes: List[int]):
         self.classes = classes
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         data.train_mask = data.train_mask.clone()
         for i in self.classes:
             data.train_mask[data.y == i] = False
         return data
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}({self.classes})'
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/rooted_subgraph.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/rooted_subgraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         node_map = data.edge_index.new_ones(data.num_nodes, data.num_nodes)
         node_map[n_sub_batch, n_id] = arange
         sub_edge_index += (arange * data.num_nodes)[e_sub_batch]
         sub_edge_index = node_map.view(-1)[sub_edge_index]
 
         return sub_edge_index, n_id, e_id, n_sub_batch, e_sub_batch
 
-    def __call__(self, data: Data) -> RootedSubgraphData:
+    def forward(self, data: Data) -> RootedSubgraphData:
         out = self.extract(data)
         d = RootedSubgraphData.from_dict(data.to_dict())
         d.sub_edge_index, d.n_id, d.e_id, d.n_sub_batch, d.e_sub_batch = out
         return d
 
 
 class RootedEgoNets(RootedSubgraph):
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/sample_points.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/sample_points.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         remove_faces: bool = True,
         include_normals: bool = False,
     ):
         self.num = num
         self.remove_faces = remove_faces
         self.include_normals = include_normals
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         pos, face = data.pos, data.face
         assert pos.size(1) == 3 and face.size(0) == 3
 
         pos_max = pos.abs().max()
         pos = pos / pos_max
 
         area = (pos[face[1]] - pos[face[0]]).cross(pos[face[2]] - pos[face[0]])
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/sign.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/sign.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     Args:
         K (int): The number of hops/layer.
     """
     def __init__(self, K: int):
         self.K = K
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         assert data.edge_index is not None
         row, col = data.edge_index
         N = data.num_nodes
 
         edge_weight = data.edge_weight
         if edge_weight is None:
             edge_weight = torch.ones(data.num_edges, device=row.device)
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/spherical.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/spherical.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         max_value: Optional[float] = None,
         cat: bool = True,
     ):
         self.norm = norm
         self.max = max_value
         self.cat = cat
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         (row, col), pos, pseudo = data.edge_index, data.pos, data.edge_attr
         assert pos.dim() == 2 and pos.size(1) == 3
 
         cart = pos[col] - pos[row]
 
         rho = torch.norm(cart, p=2, dim=-1).view(-1, 1)
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/svd_feature_reduction.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/svd_feature_reduction.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Args:
         out_channels (int): The dimensionlity of node features after
             reduction.
     """
     def __init__(self, out_channels: int):
         self.out_channels = out_channels
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         if data.x.size(-1) > self.out_channels:
             U, S, _ = torch.linalg.svd(data.x)
             data.x = torch.mm(U[:, :self.out_channels],
                               torch.diag(S[:self.out_channels]))
         return data
 
     def __repr__(self) -> str:
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/target_indegree.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/target_indegree.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         max_value: Optional[float] = None,
         cat: bool = True,
     ):
         self.norm = norm
         self.max = max_value
         self.cat = cat
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         col, pseudo = data.edge_index[1], data.edge_attr
 
         deg = degree(col, data.num_nodes)
 
         if self.norm:
             deg = deg / (deg.max() if self.max is None else self.max)
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/to_dense.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/to_dense.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         num_nodes (int, optional): The number of nodes. If set to :obj:`None`,
             the number of nodes will get automatically inferred.
             (default: :obj:`None`)
     """
     def __init__(self, num_nodes: Optional[int] = None):
         self.num_nodes = num_nodes
 
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         assert data.edge_index is not None
 
         orig_num_nodes = data.num_nodes
         if self.num_nodes is None:
             num_nodes = orig_num_nodes
         else:
             assert orig_num_nodes <= self.num_nodes
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/to_device.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/to_device.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         attrs: Optional[List[str]] = None,
         non_blocking: bool = False,
     ):
         self.device = device
         self.attrs = attrs or []
         self.non_blocking = non_blocking
 
-    def __call__(
+    def forward(
         self,
         data: Union[Data, HeteroData],
     ) -> Union[Data, HeteroData]:
         return data.to(self.device, *self.attrs,
                        non_blocking=self.non_blocking)
 
     def __repr__(self):
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/to_sparse_tensor.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/to_sparse_tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                              f"(got '{layout}')")
 
         self.attr = attr
         self.remove_edge_index = remove_edge_index
         self.fill_cache = fill_cache
         self.layout = layout
 
-    def __call__(
+    def forward(
         self,
         data: Union[Data, HeteroData],
     ) -> Union[Data, HeteroData]:
 
         for store in data.edge_stores:
             if 'edge_index' not in store:
                 continue
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/to_superpixels.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/to_superpixels.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             #skimage.segmentation.slic>`_ for an overview.
     """
     def __init__(self, add_seg: bool = False, add_img: bool = False, **kwargs):
         self.add_seg = add_seg
         self.add_img = add_img
         self.kwargs = kwargs
 
-    def __call__(self, img: Tensor) -> Data:
+    def forward(self, img: Tensor) -> Data:
         from skimage.segmentation import slic
 
         img = img.permute(1, 2, 0)
         h, w, c = img.size()
 
         seg = slic(img.to(torch.double).numpy(), start_label=0, **self.kwargs)
         seg = torch.from_numpy(seg)
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/to_undirected.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/to_undirected.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             :class:`~torch_geometric.data.HeteroData` graph data.
             (default: :obj:`True`)
     """
     def __init__(self, reduce: str = "add", merge: bool = True):
         self.reduce = reduce
         self.merge = merge
 
-    def __call__(
+    def forward(
         self,
         data: Union[Data, HeteroData],
     ) -> Union[Data, HeteroData]:
         for store in data.edge_stores:
             if 'edge_index' not in store:
                 continue
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/two_hop.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/two_hop.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 )
 
 
 @functional_transform('two_hop')
 class TwoHop(BaseTransform):
     r"""Adds the two hop edges to the edge indices
     (functional name: :obj:`two_hop`)."""
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         edge_index, edge_attr = data.edge_index, data.edge_attr
         N = data.num_nodes
 
         adj = to_torch_csr_tensor(edge_index, size=(N, N))
         edge_index2, _ = to_edge_index(adj @ adj)
         edge_index2, _ = remove_self_loops(edge_index2)
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/transforms/virtual_node.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/transforms/virtual_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     phase.
 
     Node and edge features of the virtual node are added as zero-filled input
     features.
     Furthermore, special edge types will be added both for in-coming and
     out-going information to and from the virtual node.
     """
-    def __call__(self, data: Data) -> Data:
+    def forward(self, data: Data) -> Data:
         num_nodes, (row, col) = data.num_nodes, data.edge_index
         edge_type = data.get('edge_type', torch.zeros_like(row))
 
         arange = torch.arange(num_nodes, device=row.device)
         full = row.new_full((num_nodes, ), num_nodes)
         row = torch.cat([row, arange, full], dim=0)
         col = torch.cat([col, full, arange], dim=0)
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/typing.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 
 try:
     import pyg_lib  # noqa
     WITH_PYG_LIB = True
     WITH_GMM = WITH_PT2 and hasattr(pyg_lib.ops, 'grouped_matmul')
     WITH_SAMPLED_OP = hasattr(pyg_lib.ops, 'sampled_add')
     WITH_INDEX_SORT = hasattr(pyg_lib.ops, 'index_sort')
+    WITH_METIS = hasattr(pyg_lib, 'partition')
 except (ImportError, OSError) as e:
     if isinstance(e, OSError):
         warnings.warn(f"An issue occurred while importing 'pyg-lib'. "
                       f"Disabling its usage. Stacktrace: {e}")
     pyg_lib = object
     WITH_PYG_LIB = False
     WITH_GMM = False
     WITH_SAMPLED_OP = False
     WITH_INDEX_SORT = False
+    WITH_METIS = False
 
 try:
     import torch_scatter  # noqa
     WITH_TORCH_SCATTER = True
 except (ImportError, OSError) as e:
     if isinstance(e, OSError):
         warnings.warn(f"An issue occurred while importing 'torch-scatter'. "
@@ -129,14 +131,17 @@
 
         def coo(self) -> Tuple[Tensor, Tensor, Optional[Tensor]]:
             raise ImportError("'SparseTensor' requires 'torch-sparse'")
 
         def csr(self) -> Tuple[Tensor, Tensor, Optional[Tensor]]:
             raise ImportError("'SparseTensor' requires 'torch-sparse'")
 
+        def requires_grad(self) -> bool:
+            raise ImportError("'SparseTensor' requires 'torch-sparse'")
+
         def to_torch_sparse_csr_tensor(
             self,
             dtype: Optional[torch.dtype] = None,
         ) -> Tensor:
             raise ImportError("'SparseTensor' requires 'torch-sparse'")
 
     class torch_sparse:
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/__init__.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/assortativity.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/assortativity.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/augmentation.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/coalesce.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/coalesce.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/convert.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/convert.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/degree.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/degree.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/dropout.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/dropout.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/embedding.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/embedding.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/geodesic.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/geodesic.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/get_laplacian.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/get_laplacian.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/get_mesh_laplacian.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/get_mesh_laplacian.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/grid.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/grid.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/hetero.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/hetero.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/homophily.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/homophily.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/isolated.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/isolated.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/loop.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/loop.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/mask.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/mask.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/mixin.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/mixin.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/negative_sampling.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/negative_sampling.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/nested.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/nested.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/normalized_cut.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/normalized_cut.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/num_nodes.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/num_nodes.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/one_hot.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/one_hot.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/random.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/random.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/scatter.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/scatter.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/segment.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/segment.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/select.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/select.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/smiles.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/smiles.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/softmax.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/softmax.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/sort.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/sort.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/sort_edge_index.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/sort_edge_index.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/sparse.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/sparse.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/spmm.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/spmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,32 +20,32 @@
     pass
 
 
 def spmm(src: Adj, other: Tensor, reduce: str = "sum") -> Tensor:
     """Matrix product of sparse matrix with dense matrix.
 
     Args:
-        src (Tensor or torch_sparse.SparseTensor): The input sparse matrix,
-            either a :pyg:`PyG` :class:`torch_sparse.SparseTensor` or a
+        src (torch.Tensor or torch_sparse.SparseTensor): The input sparse
+            matrix, either a :pyg:`PyG` :class:`torch_sparse.SparseTensor` or a
             :pytorch:`PyTorch` :class:`torch.sparse.Tensor`.
-        other (Tensor): The input dense matrix.
+        other (torch.Tensor): The input dense matrix.
         reduce (str, optional): The reduce operation to use
             (:obj:`"sum"`, :obj:`"mean"`, :obj:`"min"`, :obj:`"max"`).
             (default: :obj:`"sum"`)
 
     :rtype: :class:`Tensor`
     """
     reduce = 'sum' if reduce == 'add' else reduce
 
     if reduce not in ['sum', 'mean', 'min', 'max']:
         raise ValueError(f"`reduce` argument '{reduce}' not supported")
 
     if isinstance(src, SparseTensor):
         if (torch_geometric.typing.WITH_PT2 and other.dim() == 2
-                and not src.is_cuda()):
+                and not src.is_cuda() and not src.requires_grad()):
             # Use optimized PyTorch `torch.sparse.mm` path:
             csr = src.to_torch_sparse_csr_tensor()
             return torch.sparse.mm(csr, other, reduce)
         return torch_sparse.matmul(src, other, reduce)
 
     if not is_torch_sparse_tensor(src):
         raise ValueError("`src` must be a `torch_sparse.SparseTensor` "
```

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/subgraph.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/subgraph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/to_dense_adj.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/to_dense_adj.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/to_dense_batch.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/to_dense_batch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/train_test_split_edges.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/train_test_split_edges.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/tree_decomposition.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/tree_decomposition.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/trim_to_layer.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/trim_to_layer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/unbatch.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/unbatch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/utils/undirected.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/utils/undirected.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/torch_geometric/visualization/graph.py` & `pyg_nightly-2.4.0.dev20230525/torch_geometric/visualization/graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.4.0.dev20230524/PKG-INFO` & `pyg_nightly-2.4.0.dev20230525/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyg-nightly
-Version: 2.4.0.dev20230524
+Version: 2.4.0.dev20230525
 Summary: Graph Neural Network Library for PyTorch
 Keywords: deep-learning,pytorch,geometric-deep-learning,graph-neural-networks,graph-convolutional-networks
 Author-email: Matthias Fey <matthias@pyg.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

