# Comparing `tmp/scgenome-0.0.8.tar.gz` & `tmp/scgenome-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scgenome-0.0.8.tar", last modified: Thu Oct  6 02:16:13 2022, max compression
+gzip compressed data, was "scgenome-0.0.9.tar", last modified: Sat Dec  3 12:49:00 2022, max compression
```

## Comparing `scgenome-0.0.8.tar` & `scgenome-0.0.9.tar`

### file list

```diff
@@ -1,72 +1,71 @@
-drwxr-xr-x   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)        0 2022-10-06 02:16:13.000000 scgenome-0.0.8/
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)       51 2022-07-14 17:06:38.000000 scgenome-0.0.8/MANIFEST.in
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)      252 2022-10-06 02:16:13.000000 scgenome-0.0.8/PKG-INFO
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     1104 2022-09-10 17:05:09.000000 scgenome-0.0.8/README.md
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)      802 2022-09-22 11:32:22.000000 scgenome-0.0.8/pyproject.toml
-drwxr-xr-x   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)        0 2022-10-06 02:16:13.000000 scgenome-0.0.8/scgenome/
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)      216 2022-10-06 01:34:18.000000 scgenome-0.0.8/scgenome/__init__.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)      497 2022-10-06 02:16:13.000000 scgenome-0.0.8/scgenome/_version.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)    13131 2022-02-03 21:13:25.000000 scgenome-0.0.8/scgenome/breakpointdata.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)    18495 2021-08-09 21:24:41.000000 scgenome-0.0.8/scgenome/cnclones.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     6376 2022-02-17 14:48:58.000000 scgenome-0.0.8/scgenome/cncluster.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     3575 2019-11-05 01:01:50.000000 scgenome-0.0.8/scgenome/cnfilter.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)    14553 2022-02-17 14:48:58.000000 scgenome-0.0.8/scgenome/cnplot.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     3884 2021-08-02 11:23:15.000000 scgenome-0.0.8/scgenome/cntransitions.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)    17916 2020-03-06 20:35:12.000000 scgenome-0.0.8/scgenome/csvutils.py
-drwxr-xr-x   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)        0 2022-10-06 02:16:13.000000 scgenome-0.0.8/scgenome/data/
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     2746 2019-01-30 05:13:04.000000 scgenome-0.0.8/scgenome/data/GRCh37-lite.fa.fai
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     2139 2022-02-17 14:48:58.000000 scgenome-0.0.8/scgenome/data/mm10.fa.fai
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     3120 2019-10-28 23:45:26.000000 scgenome-0.0.8/scgenome/jointcnmodels.py
-drwxr-xr-x   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)        0 2022-10-06 02:16:13.000000 scgenome-0.0.8/scgenome/loaders/
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)        0 2019-08-14 01:05:21.000000 scgenome-0.0.8/scgenome/loaders/__init__.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     1677 2022-05-25 17:57:59.000000 scgenome-0.0.8/scgenome/loaders/align.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)      930 2021-08-17 18:38:48.000000 scgenome-0.0.8/scgenome/loaders/allele.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     1301 2022-02-03 21:13:26.000000 scgenome-0.0.8/scgenome/loaders/annotation.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     7017 2021-08-17 18:38:48.000000 scgenome-0.0.8/scgenome/loaders/breakpoint.py
-drwxr-xr-x   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)        0 2022-10-06 02:16:13.000000 scgenome-0.0.8/scgenome/loaders/dtypes/
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     2847 2019-10-28 23:45:26.000000 scgenome-0.0.8/scgenome/loaders/dtypes/alignment_gc_metrics_defs.yaml
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)      587 2019-10-28 23:45:26.000000 scgenome-0.0.8/scgenome/loaders/dtypes/hmmcopy_params_defs.yaml
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)      531 2019-10-28 23:45:26.000000 scgenome-0.0.8/scgenome/loaders/dtypes/hmmcopy_reads_defs.yaml
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)      194 2019-10-28 23:45:26.000000 scgenome-0.0.8/scgenome/loaders/dtypes/hmmcopy_segments_defs.yaml
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     6642 2019-10-28 23:45:26.000000 scgenome-0.0.8/scgenome/loaders/dtypes/metrics_column_defs.yaml
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     2483 2022-03-23 15:12:31.000000 scgenome-0.0.8/scgenome/loaders/hmmcopy.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     3197 2022-02-10 21:27:17.000000 scgenome-0.0.8/scgenome/loaders/qc.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)    14719 2022-04-01 11:32:12.000000 scgenome-0.0.8/scgenome/loaders/snv.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     6667 2022-02-10 21:27:17.000000 scgenome-0.0.8/scgenome/loaders/utils.py
-drwxr-xr-x   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)        0 2022-10-06 02:16:13.000000 scgenome-0.0.8/scgenome/plotting/
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)      170 2022-07-14 17:06:38.000000 scgenome-0.0.8/scgenome/plotting/__init__.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     1920 2022-10-06 01:34:18.000000 scgenome-0.0.8/scgenome/plotting/cn.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     4068 2022-10-06 01:34:18.000000 scgenome-0.0.8/scgenome/plotting/heatmap.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     4291 2022-10-04 18:34:33.000000 scgenome-0.0.8/scgenome/plotting/phylo.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)      241 2022-02-10 21:27:17.000000 scgenome-0.0.8/scgenome/plotting/qc.py
-drwxr-xr-x   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)        0 2022-10-06 02:16:13.000000 scgenome-0.0.8/scgenome/preprocessing/
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)      225 2022-10-06 01:34:19.000000 scgenome-0.0.8/scgenome/preprocessing/__init__.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     4060 2022-10-06 01:34:18.000000 scgenome-0.0.8/scgenome/preprocessing/filtering.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)    10568 2022-10-06 01:34:20.000000 scgenome-0.0.8/scgenome/preprocessing/load_cn.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     1791 2022-06-14 14:28:10.000000 scgenome-0.0.8/scgenome/preprocessing/load_snv.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)      698 2022-02-10 21:27:17.000000 scgenome-0.0.8/scgenome/preprocessing/transform.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     2149 2022-10-06 02:15:07.000000 scgenome-0.0.8/scgenome/refgenome.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)    11819 2021-08-09 21:24:41.000000 scgenome-0.0.8/scgenome/snpdata.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     7618 2021-04-20 11:27:07.000000 scgenome-0.0.8/scgenome/snvdata.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     7971 2021-08-03 18:18:35.000000 scgenome-0.0.8/scgenome/snvphylo.py
-drwxr-xr-x   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)        0 2022-10-06 02:16:13.000000 scgenome-0.0.8/scgenome/tests/
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)        0 2019-10-28 23:45:26.000000 scgenome-0.0.8/scgenome/tests/__init__.py
-drwxr-xr-x   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)        0 2022-10-06 02:16:13.000000 scgenome-0.0.8/scgenome/tools/
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)      386 2022-10-03 23:20:01.000000 scgenome-0.0.8/scgenome/tools/__init__.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     3466 2022-02-10 21:27:17.000000 scgenome-0.0.8/scgenome/tools/binfeat.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     6367 2022-09-10 17:58:01.000000 scgenome-0.0.8/scgenome/tools/cluster.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)      597 2022-04-03 17:02:32.000000 scgenome-0.0.8/scgenome/tools/concat.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     3761 2022-08-15 23:41:43.000000 scgenome-0.0.8/scgenome/tools/genes.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     2189 2022-02-10 21:27:17.000000 scgenome-0.0.8/scgenome/tools/pca.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)      492 2022-07-14 17:06:38.000000 scgenome-0.0.8/scgenome/tools/phylo.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     1076 2022-02-10 21:27:17.000000 scgenome-0.0.8/scgenome/tools/sorting.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     2610 2021-11-10 20:10:28.000000 scgenome-0.0.8/scgenome/utils.py
-drwxr-xr-x   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)        0 2022-10-06 02:16:13.000000 scgenome-0.0.8/scgenome.egg-info/
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)      252 2022-10-06 02:16:13.000000 scgenome-0.0.8/scgenome.egg-info/PKG-INFO
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     1647 2022-10-06 02:16:13.000000 scgenome-0.0.8/scgenome.egg-info/SOURCES.txt
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)        1 2022-10-06 02:16:13.000000 scgenome-0.0.8/scgenome.egg-info/dependency_links.txt
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)      259 2022-10-06 02:16:13.000000 scgenome-0.0.8/scgenome.egg-info/requires.txt
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)        9 2022-10-06 02:16:13.000000 scgenome-0.0.8/scgenome.egg-info/top_level.txt
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)      233 2022-10-06 02:16:13.000000 scgenome-0.0.8/setup.cfg
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)     1128 2022-10-06 01:34:18.000000 scgenome-0.0.8/setup.py
--rw-r--r--   0 mcphera1 (1715532355) MSKCC\Domain Users (9696963)    81180 2022-07-14 17:06:38.000000 scgenome-0.0.8/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 12:49:00.328926 scgenome-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)       51 2022-12-03 12:48:32.000000 scgenome-0.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      174 2022-12-03 12:49:00.328926 scgenome-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1622 2022-12-03 12:48:32.000000 scgenome-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 12:49:00.328926 scgenome-0.0.9/scgenome/
+-rw-r--r--   0 root         (0) root         (0)      407 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2022-12-03 12:49:00.328926 scgenome-0.0.9/scgenome/_version.py
+-rw-r--r--   0 root         (0) root         (0)    13131 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/breakpointdata.py
+-rw-r--r--   0 root         (0) root         (0)    18495 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/cnclones.py
+-rw-r--r--   0 root         (0) root         (0)     6376 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/cncluster.py
+-rw-r--r--   0 root         (0) root         (0)     3575 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/cnfilter.py
+-rw-r--r--   0 root         (0) root         (0)    14693 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/cnplot.py
+-rw-r--r--   0 root         (0) root         (0)     3884 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/cntransitions.py
+-rw-r--r--   0 root         (0) root         (0)    17916 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/csvutils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 12:49:00.320926 scgenome-0.0.9/scgenome/data/
+-rw-r--r--   0 root         (0) root         (0)      790 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/data/grch38.fa.fai
+-rw-r--r--   0 root         (0) root         (0)     2746 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/data/hg19.fa.fai
+-rw-r--r--   0 root         (0) root         (0)     2139 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/data/mm10.fa.fai
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 12:49:00.320926 scgenome-0.0.9/scgenome/datasets/
+-rw-r--r--   0 root         (0) root         (0)       55 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      395 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/datasets/_datasets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 12:49:00.320926 scgenome-0.0.9/scgenome/datasets/data/
+-rw-r--r--   0 root         (0) root         (0)  4946742 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/datasets/data/OV2295_HMMCopy_reduced.h5ad
+-rw-r--r--   0 root         (0) root         (0)     3120 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/jointcnmodels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 12:49:00.324926 scgenome-0.0.9/scgenome/loaders/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/loaders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/loaders/align.py
+-rw-r--r--   0 root         (0) root         (0)      930 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/loaders/allele.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/loaders/annotation.py
+-rw-r--r--   0 root         (0) root         (0)     7017 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/loaders/breakpoint.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/loaders/hmmcopy.py
+-rw-r--r--   0 root         (0) root         (0)     3197 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/loaders/qc.py
+-rw-r--r--   0 root         (0) root         (0)    14719 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/loaders/snv.py
+-rw-r--r--   0 root         (0) root         (0)     6667 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/loaders/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 12:49:00.324926 scgenome-0.0.9/scgenome/plotting/
+-rw-r--r--   0 root         (0) root         (0)      170 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/plotting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/plotting/cn.py
+-rw-r--r--   0 root         (0) root         (0)    10139 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/plotting/heatmap.py
+-rw-r--r--   0 root         (0) root         (0)     4291 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/plotting/phylo.py
+-rw-r--r--   0 root         (0) root         (0)      241 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/plotting/qc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 12:49:00.324926 scgenome-0.0.9/scgenome/preprocessing/
+-rw-r--r--   0 root         (0) root         (0)      225 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/preprocessing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4089 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/preprocessing/filtering.py
+-rw-r--r--   0 root         (0) root         (0)    11108 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/preprocessing/load_cn.py
+-rw-r--r--   0 root         (0) root         (0)     1791 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/preprocessing/load_snv.py
+-rw-r--r--   0 root         (0) root         (0)      698 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/preprocessing/transform.py
+-rw-r--r--   0 root         (0) root         (0)     2486 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/refgenome.py
+-rw-r--r--   0 root         (0) root         (0)    11819 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/snpdata.py
+-rw-r--r--   0 root         (0) root         (0)     7618 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/snvdata.py
+-rw-r--r--   0 root         (0) root         (0)     7971 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/snvphylo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 12:49:00.324926 scgenome-0.0.9/scgenome/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 12:49:00.328926 scgenome-0.0.9/scgenome/tools/
+-rw-r--r--   0 root         (0) root         (0)      386 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3466 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/tools/binfeat.py
+-rw-r--r--   0 root         (0) root         (0)     6890 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/tools/cluster.py
+-rw-r--r--   0 root         (0) root         (0)      597 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/tools/concat.py
+-rw-r--r--   0 root         (0) root         (0)     3761 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/tools/genes.py
+-rw-r--r--   0 root         (0) root         (0)     2189 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/tools/pca.py
+-rw-r--r--   0 root         (0) root         (0)      492 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/tools/phylo.py
+-rw-r--r--   0 root         (0) root         (0)     1076 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/tools/sorting.py
+-rw-r--r--   0 root         (0) root         (0)     2610 2022-12-03 12:48:34.000000 scgenome-0.0.9/scgenome/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-03 12:49:00.320926 scgenome-0.0.9/scgenome.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      174 2022-12-03 12:48:59.000000 scgenome-0.0.9/scgenome.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1513 2022-12-03 12:49:00.000000 scgenome-0.0.9/scgenome.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-03 12:48:59.000000 scgenome-0.0.9/scgenome.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      319 2022-12-03 12:49:00.000000 scgenome-0.0.9/scgenome.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2022-12-03 12:49:00.000000 scgenome-0.0.9/scgenome.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      233 2022-12-03 12:49:00.328926 scgenome-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1223 2022-12-03 12:48:34.000000 scgenome-0.0.9/setup.py
+-rw-r--r--   0 root         (0) root         (0)    81180 2022-12-03 12:48:34.000000 scgenome-0.0.9/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scgenome-0.0.8/README.md` & `scgenome-0.0.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # scgenome: single cell whole genome analysis in python
 
+![codebuild](https://codebuild.us-east-1.amazonaws.com/badges?uuid=eyJlbmNyeXB0ZWREYXRhIjoiSTVXZ3NyZWVSejMrd2JRd25GUTJnUmMwclFqd0t0ajNzbWk4dWlld3N4UHVYZzUzUzJkVUVPQmloZUZzbWNGM2lwWUlVN1hDMnBmandJZWdENU5GUjlrPSIsIml2UGFyYW1ldGVyU3BlYyI6IjM2UTFWbjRyUmx0VXlMWUgiLCJtYXRlcmlhbFNldFNlcmlhbCI6MX0%3D&branch=main)
+
+![Documentation Status](https://readthedocs.org/projects/scgenome/badge/?version=latest)
+
 scgenome is scalable python toolkit for analyzing single-cell whole genome
 data built on [anndata](https://anndata.readthedocs.io) and inspired by
 [scanpy](https://scanpy.readthedocs.io).  scgenome includes preprocessing,
 visualization, and clustering functionality and can be used to analyze
 copy number, allele specific copy number, SNV and breakpoint features.
 
 ## Installation
@@ -37,11 +41,20 @@
 
 Coming Soon
 
 ## Pip build
 
 To build with pip and distribute to pypi, use the following commands:
 
-    python setup.py build_ext --force sdist
-    twine upload --repository pypi dist/*
+```
+python setup.py build_ext --force sdist
+twine upload --repository pypi dist/*
+```
 
+## Build documentation
 
+```
+pip install -r docs/requirements/requirements.txt
+pip install scgenome
+cd docs
+make html
+```
```

### Comparing `scgenome-0.0.8/scgenome/breakpointdata.py` & `scgenome-0.0.9/scgenome/breakpointdata.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/cnclones.py` & `scgenome-0.0.9/scgenome/cnclones.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/cncluster.py` & `scgenome-0.0.9/scgenome/cncluster.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/cnfilter.py` & `scgenome-0.0.9/scgenome/cnfilter.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/cnplot.py` & `scgenome-0.0.9/scgenome/cnplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,23 +53,23 @@
     idx = np.array(Z['leaves'])
     ordering = np.zeros(idx.shape[0], dtype=int)
     ordering[idx] = np.arange(idx.shape[0])
     return ordering
 
 
 def plot_clustered_cell_cn_matrix(ax, cn_data, cn_field_name, cluster_field_name='cluster_id', secondary_field_name=None, raw=False, max_cn=13, cmap=None):
-    plot_data = cn_data.merge(refgenome.info.chrom_idxs)
+    plot_data = cn_data.merge(refgenome.info.chromosome_info[['chr', 'chr_index']])
 
     if secondary_field_name is not None:
         plot_data = plot_data.set_index(['chr_index', 'start', 'cell_id', cluster_field_name])
         plot_data = plot_data[[secondary_field_name, cn_field_name]]
         plot_data = plot_data.unstack(level=['cell_id', cluster_field_name]).fillna(0)
         ordering = plot_data[secondary_field_name].values[0]
 
-        plot_data = cn_data.merge(refgenome.info.chrom_idxs)
+        plot_data = cn_data.merge(refgenome.info.chromosome_info[['chr', 'chr_index']])
         plot_data = plot_data.set_index(['chr_index', 'start', 'cell_id', cluster_field_name])[cn_field_name].unstack(level=['cell_id', cluster_field_name]).fillna(0)
     else:
         plot_data = plot_data.set_index(['chr_index', 'start', 'cell_id', cluster_field_name])[cn_field_name].unstack(level=['cell_id', cluster_field_name]).fillna(0)
         ordering = _secondary_clustering(plot_data.values)
     ordering = pd.Series(ordering, index=plot_data.columns, name='cell_order')
     plot_data = plot_data.T.set_index(ordering, append=True).T
 
@@ -78,15 +78,15 @@
         plot_data[plot_data > max_cn] = max_cn
 
     mat_chrom_idxs = plot_data.index.get_level_values(0).values
     chrom_boundaries = np.array([0] + list(np.where(mat_chrom_idxs[1:] != mat_chrom_idxs[:-1])[0]) + [plot_data.shape[0] - 1])
     chrom_sizes = chrom_boundaries[1:] - chrom_boundaries[:-1]
     chrom_mids = chrom_boundaries[:-1] + chrom_sizes / 2
     ordered_mat_chrom_idxs = mat_chrom_idxs[np.where(np.array([1] + list(np.diff(mat_chrom_idxs))) != 0)]
-    chrom_names = np.array(refgenome.info.chromosomes)[ordered_mat_chrom_idxs]
+    chrom_names = np.array(refgenome.info.plot_chromosomes)[ordered_mat_chrom_idxs]
 
     mat_cluster_ids = plot_data.columns.get_level_values(1).values
     cluster_boundaries = np.array([0] + list(np.where(mat_cluster_ids[1:] != mat_cluster_ids[:-1])[0]) + [plot_data.shape[1] - 1])
     cluster_sizes = cluster_boundaries[1:] - cluster_boundaries[:-1]
     cluster_mids = cluster_boundaries[:-1] + cluster_sizes / 2
 
     if not raw and cmap is None:
@@ -182,22 +182,22 @@
         ax.set_xticks(xticks + chromosome_start)
         ax.set_xticklabels(xticklabels)
         ax.xaxis.set_minor_locator(matplotlib.ticker.FixedLocator(xminorticks + chromosome_start))
         ax.xaxis.set_minor_formatter(matplotlib.ticker.NullFormatter())
         ax.set_xlim((chromosome_start, chromosome_end))
 
     else:
-        ax.set_xlim((-0.5, refgenome.info.chromosome_end.max()))
+        ax.set_xlim((-0.5, refgenome.info.chromosome_info['chromosome_end'].max()))
         ax.set_xlabel('chromosome')
-        ax.set_xticks([0] + list(refgenome.info.chromosome_end.values))
+        ax.set_xticks([0] + list(refgenome.info.chromosome_info['chromosome_end'].values))
         ax.set_xticklabels([])
         ax.xaxis.tick_bottom()
         ax.yaxis.tick_left()
-        ax.xaxis.set_minor_locator(matplotlib.ticker.FixedLocator(refgenome.info.chromosome_mid))
-        ax.xaxis.set_minor_formatter(matplotlib.ticker.FixedFormatter(refgenome.info.chromosomes))
+        ax.xaxis.set_minor_locator(matplotlib.ticker.FixedLocator(refgenome.info.chromosome_info['chromosome_mid']))
+        ax.xaxis.set_minor_formatter(matplotlib.ticker.FixedFormatter(refgenome.info.plot_chromosomes))
 
     if squashy and not rawy:
         yticks = np.array([0, 2, 4, 7, 20])
         yticks_squashed = squash_f(yticks)
         ytick_labels = [str(a) for a in yticks]
         ax.set_yticks(yticks_squashed)
         ax.set_yticklabels(ytick_labels)
@@ -280,15 +280,15 @@
         color = prediction_colors[prediction_id]
         ax.plot(pos, spl(pos), ls='-', lw=lw, color=color)
 
     ax.set_ylim((ylim[0], ylim[1] + 5))
 
 
 def plot_cluster_cn_matrix(fig, cn_data, cn_field_name, cluster_field_name='cluster_id'):
-    plot_data = cn_data.merge(refgenome.info.chrom_idxs)
+    plot_data = cn_data.merge(refgenome.info.chromosome_info[['chr', 'chr_index']])
     plot_data = plot_data.groupby(['chr_index', 'start', cluster_field_name], observed=True)[cn_field_name].median().astype(int)
     plot_data = plot_data.unstack(level=[cluster_field_name]).fillna(0)
     plot_data = plot_data.sort_index(axis=1, level=1)
 
     logging.info(f'matrix with size {plot_data.T.shape}')
 
     ax = fig.add_axes([0.0,1.,0.1,1.])
@@ -305,15 +305,15 @@
         ax.spines['right'].set_visible(False)
         plot_data = plot_data.iloc[:, idx]
 
     mat_chrom_idxs = plot_data.index.get_level_values(0).values
     chrom_boundaries = np.array([0] + list(np.where(mat_chrom_idxs[1:] != mat_chrom_idxs[:-1])[0]) + [plot_data.shape[0] - 1])
     chrom_sizes = chrom_boundaries[1:] - chrom_boundaries[:-1]
     chrom_mids = chrom_boundaries[:-1] + chrom_sizes / 2
-    chromosomes = refgenome.info.chrom_idxs.loc[refgenome.info.chrom_idxs['chr_index'].isin(mat_chrom_idxs), 'chr'].values
+    chromosomes = refgenome.info.chromosome_info.set_index('chr_index').loc[np.unique(mat_chrom_idxs), 'chr_plot']
 
     ax = fig.add_axes([0.125,1.,0.875,1.])
     im = ax.imshow(plot_data.T, aspect='auto', cmap=get_cn_cmap(plot_data.values), interpolation='none')
 
     ax.set(xticks=chrom_mids)
     ax.set(xticklabels=chromosomes)
     ax.set(yticks=list(range(len(plot_data.columns.values))))
```

### Comparing `scgenome-0.0.8/scgenome/cntransitions.py` & `scgenome-0.0.9/scgenome/cntransitions.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/csvutils.py` & `scgenome-0.0.9/scgenome/csvutils.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/data/GRCh37-lite.fa.fai` & `scgenome-0.0.9/scgenome/data/hg19.fa.fai`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/data/mm10.fa.fai` & `scgenome-0.0.9/scgenome/data/mm10.fa.fai`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/jointcnmodels.py` & `scgenome-0.0.9/scgenome/jointcnmodels.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/loaders/align.py` & `scgenome-0.0.9/scgenome/loaders/align.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/loaders/allele.py` & `scgenome-0.0.9/scgenome/loaders/allele.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/loaders/annotation.py` & `scgenome-0.0.9/scgenome/loaders/annotation.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/loaders/breakpoint.py` & `scgenome-0.0.9/scgenome/loaders/breakpoint.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/loaders/hmmcopy.py` & `scgenome-0.0.9/scgenome/loaders/hmmcopy.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/loaders/qc.py` & `scgenome-0.0.9/scgenome/loaders/qc.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/loaders/snv.py` & `scgenome-0.0.9/scgenome/loaders/snv.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/loaders/utils.py` & `scgenome-0.0.9/scgenome/loaders/utils.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/plotting/cn.py` & `scgenome-0.0.9/scgenome/plotting/cn.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import matplotlib.pyplot as plt
 import pandas as pd
+import numpy as np
 
 from anndata import AnnData
 
 import scgenome.cnplot
 
 
 def plot_cn_profile(
@@ -39,27 +40,37 @@
     s : int, optional
         size of scatter points, by default 5
     squashy : bool, optional
         compress y axis, by default False
     rawy : bool, optional
         raw data on y axis, by default False
 
+    Examples
+    -------
+
+    .. plot::
+        :context: close-figs
+
+        import scgenome
+        adata = scgenome.datasets.OV2295_HMMCopy_reduced()
+        scgenome.pl.plot_cn_profile(adata, 'SA922-A90554B-R27-C43', value_layer_name='copy', state_layer_name='state')
+
     TODO: missing return
     """
 
     cn_data = adata.var.copy()
 
     if value_layer_name is not None:
-        cn_data['value'] = adata[[obs_id], :].layers[value_layer_name][0]
+        cn_data['value'] = np.array(adata[[obs_id], :].layers[value_layer_name][0])
     else:
-        cn_data['value'] = adata[[obs_id], :].X[0]
+        cn_data['value'] = np.array(adata[[obs_id], :].X[0])
 
     cn_field_name = None
     if state_layer_name is not None:
-        cn_data['state'] = adata[[obs_id], :].layers[state_layer_name][0]
+        cn_data['state'] = np.array(adata[[obs_id], :].layers[state_layer_name][0])
         cn_field_name = 'state'
 
     if ax is None:
         ax = plt.gca()
 
     cn_data = cn_data.dropna(subset=['value'])
```

### Comparing `scgenome-0.0.8/scgenome/plotting/heatmap.py` & `scgenome-0.0.9/scgenome/plotting/phylo.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,128 +1,137 @@
-import anndata as ad
-import matplotlib.pyplot as plt
+import Bio.Phylo
 import numpy as np
-
-from anndata import AnnData
-
-import scgenome.cnplot
-import scgenome.refgenome
-
-
-def plot_cell_cn_matrix(adata: AnnData, layer_name='state', cell_order_fields=None, ax=None, raw=False, max_cn=13):
-    """ Plot a copy number matrix
+import matplotlib.pyplot as plt
+import matplotlib.patches as mpatches
+from matplotlib import gridspec
+import seaborn as sns
+
+import scgenome.plotting.heatmap
+
+
+def map_annotations_to_colors(annotation, cmap):
+    num_colors = len(np.unique(annotation))
+
+    color_map = {}
+    for idx, value in enumerate(np.unique(annotation)):
+        color_map[value] = cmap(float(idx) / float(max(1, num_colors - 1)))
+
+    color_mat = []
+    for value in annotation:
+        color_mat.append(color_map[value])
+        
+    return color_mat, color_map
+
+
+def plot_tree_cn(
+        tree,
+        adata,
+        chrom_segments=True,
+        layer_name=None,
+        obs_annotation=None,
+        obs_cmap=None,
+        var_label=None,
+        fig=None,
+        raw=False,
+        max_cn=13):
+    """ Plot a tree aligned to a CN values matrix heatmap
 
     Parameters
     ----------
+    tree : Bio.Phylo.BaseTree.Tree
+        phylogenetic tree
     adata : AnnData
-        copy number data
+        Copy number data, either genes or segments
+    chrom_segments : bool, optional
+        whether adata is genes or segments, by default True
     layer_name : str, optional
-        layer with copy number data to plot, None for X, by default 'state'
-    cell_order_fields : list, optional
-        columns of obs on which to sort cells, by default None
-    ax : matplotlib.axes.Axes, optional
-        existing axis to plot into, by default None
+        layer to plot for copy number heatmap, by default None
+    obs_annotation : str, optional
+        column of adata.obs to annotate cells, by default None
+    obs_cmap : matplotlib.colors.ListedColormap, optional
+        color map for cell annotations, by default None
+    var_label : str, optional
+        column of adata.var to use for heatmap var labels, by default None use index
+    fig : matplotlib.figure.Figure, optional
+        existing figure to plot into, by default None
     raw : bool, optional
         raw plotting, no integer color map, by default False
     max_cn : int, optional
         clip cn at max value, by default 13
-
-    TODO: missing return
     """    
+    
+    if fig is None:
+        fig = plt.figure(figsize=(16, 12), dpi=150)
 
-    if ax is None:
-        ax = plt.gca()
+    # Add phylogenetic ordering to anndata obs
+    cell_ids = []
+    for a in tree.get_terminals():
+        cell_ids.append(a.name)
+
+    adata.obs['phylo_order'] = None
+    for idx, _ in adata.obs.iterrows():
+        adata.obs.loc[idx, 'phylo_order'] = cell_ids.index(idx)
+
+    gs = gridspec.GridSpec(1, 3, width_ratios=(0.4, 0.58, 0.02))
+
+    # Plot phylogenetic tree
+    ax = fig.add_subplot(gs[0, 0])
+    ax.spines['top'].set_visible(False)
+    ax.spines['right'].set_visible(False)
+    ax.spines['bottom'].set_visible(True)
+    ax.spines['left'].set_visible(False)
+    ax.get_yaxis().set_ticks([])
+    Bio.Phylo.draw(tree, label_func=lambda a: '', axes=ax, do_show=False)
+
+    # Plot copy number heatmap
+    ax = fig.add_subplot(gs[0, 1])
+
+    if chrom_segments:
+        scgenome.plotting.heatmap.plot_cell_cn_matrix(
+            adata,
+            layer_name=layer_name,
+            cell_order_fields=('phylo_order',),
+            ax=ax,
+            raw=raw,
+            max_cn=max_cn,
+        )
 
-    if layer_name is not None:
-        X = adata.layers[layer_name].copy()
     else:
-        X = adata.X.copy()
-
-    X = np.nan_to_num(X, nan=0)
-
-    if max_cn is not None:
-        X[X > max_cn] = max_cn
-
-    # Order the chromosomes
-    chr_start = adata.var.reset_index().merge(scgenome.refgenome.info.chrom_idxs, how='left')[['start', 'chr_index']].values
-    genome_ordering = np.lexsort(chr_start.transpose())
+        if layer_name is not None:
+            X = adata.layers[layer_name]
+        else:
+            X = adata.X
 
-    # Order the cells if requested
-    if cell_order_fields is not None:
-        cell_order_fields = reversed(list(cell_order_fields))
-        cell_order_values = adata.obs[cell_order_fields].values.transpose()
+        # Order the cells according to the phylogeny
+        cell_order_values = adata.obs[['phylo_order']].values.transpose()
         cell_ordering = np.lexsort(cell_order_values)
 
-    else:
-        cell_ordering = range(X.shape[0])
-
-    X = X[cell_ordering, :][:, genome_ordering]
-
-    cmap = None
-    if not raw:
-        cmap = scgenome.cnplot.get_cn_cmap(X)
-
-    im = ax.imshow(X, aspect='auto', cmap=cmap, interpolation='none')
-
-    mat_chrom_idxs = chr_start[genome_ordering][:, 1]
-    chrom_boundaries = np.array([0] + list(np.where(mat_chrom_idxs[1:] != mat_chrom_idxs[:-1])[0]) + [mat_chrom_idxs.shape[0] - 1])
-    chrom_sizes = chrom_boundaries[1:] - chrom_boundaries[:-1]
-    chrom_mids = chrom_boundaries[:-1] + chrom_sizes / 2
-    ordered_mat_chrom_idxs = mat_chrom_idxs[np.where(np.array([1] + list(np.diff(mat_chrom_idxs))) != 0)]
-    chrom_names = np.array(scgenome.refgenome.info.chromosomes)[ordered_mat_chrom_idxs]
+        X = X[cell_ordering, :]
 
-    ax.set(xticks=chrom_mids)
-    ax.set(xticklabels=chrom_names)
+        mat = adata[cell_ordering, :].to_df(layer=layer_name)
+        if var_label is not None:
+            mat = mat.rename(columns=adata.var[var_label])
+        
+        cbar_ax = fig.add_axes([0.45, 0.0, 0.2, 0.01])
+        sns.heatmap(mat, ax=ax, cbar_ax=cbar_ax, cbar_kws={'orientation': 'horizontal'})
 
-    for val in chrom_boundaries[:-1]:
-        ax.axvline(x=val, linewidth=1, color='black', zorder=100)
-
-    return ax
-
-
-def plot_cell_cn_matrix_clusters_fig(
-        adata: AnnData,
-        layer_name='state',
-        cell_order_fields=None,
-        annotation_field='cluster_id',
-        fig=None,
-        raw=False,
-        max_cn=13):
-    """ Plot a copy number matrix
-
-    Parameters
-    ----------
-    adata : AnnData
-        copy number data
-    layer_name : str, optional
-        layer with copy number data to plot, None for X, by default 'state'
-    cell_order_fields : list, optional
-        columns of obs on which to sort cells, by default None
-    annotation_field : str
-        column of obs to use as an annotation colorbar, by default 'cluster_id'
-    fig : matplotlib.figure.Figure, optional
-        existing figure to plot into, by default None
-    raw : bool, optional
-        raw plotting, no integer color map, by default False
-    max_cn : int, optional
-        clip cn at max value, by default 13
-    """    
+    ax.set_yticks([])
 
-    if fig is None:
-        fig = plt.figure()
+    # Plot obs annotation
+    if obs_annotation is not None:
+        ax = fig.add_subplot(gs[0, 2])
+
+        color_mat, color_map = map_annotations_to_colors(adata.obs[obs_annotation], obs_cmap)
+        color_mat = np.swapaxes(np.array([color_mat]), 0, 1)
+
+        ax.imshow(color_mat[::-1, :, :], aspect='auto', origin='lower', interpolation='none')
+        ax.set_xticks([])
+        ax.set_yticks([])
+
+        patches = []
+        for label, color in color_map.items():
+            patches.append(mpatches.Patch(color=color, label=label))
+        ax.legend(handles=patches, loc='upper left', bbox_to_anchor=(1.05, 1.))
 
-    ax = fig.add_axes([0.1,0.0,0.9,1.])
-    plot_cell_cn_matrix(
-        adata, layer_name=layer_name,
-        cell_order_fields=cell_order_fields,
-        ax=ax, raw=raw, max_cn=max_cn)
-
-    cluster_ids = adata.obs.sort_values(cell_order_fields)[annotation_field].values
-    color_mat = scgenome.cncluster.get_cluster_colors(cluster_ids)
-
-    ax = fig.add_axes([0.0,0.0,0.05,1.])
-    ax.imshow(np.array(color_mat)[::-1, np.newaxis], aspect='auto', origin='lower', interpolation='none')
-    ax.grid(False)
-    ax.set_xticks([])
-    ax.set_yticks([])
+    plt.subplots_adjust(left=0.065, right=0.97, top=0.96, bottom=0.065, wspace=0.01)
 
     return fig
```

### Comparing `scgenome-0.0.8/scgenome/preprocessing/filtering.py` & `scgenome-0.0.9/scgenome/preprocessing/filtering.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,20 +35,22 @@
     inplace : bool, optional
         Whether to modify passed in AnnData, by default False
 
     Returns
     -------
     AnnData
         AnnData with modified obs if not inplace, otherise, None
-    
-    Properties Changed
-    ------
-    AnnData.obs.filter_quality
-    AnnData.obs.filter_reads
-    AnnData.obs.filter_copy_state_diff
+
+    Note
+    ----
+
+    The following properties are changed:
+    - AnnData.obs.filter_quality
+    - AnnData.obs.filter_reads
+    - AnnData.obs.filter_copy_state_diff
     
     If is_s_phase is a property of AnnData
         AnnData.obs.filter_is_s_phase
         
     AnnData.obs.copy_state_diff
     AnnData.obs.copy_state_diff_mean
     """
```

### Comparing `scgenome-0.0.8/scgenome/preprocessing/load_cn.py` & `scgenome-0.0.9/scgenome/preprocessing/load_cn.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,32 +13,33 @@
 from pandas import DataFrame
 
 
 def read_dlp_hmmcopy(alignment_results_dir, hmmcopy_results_dir, annotation_results_dir, sample_ids=None, additional_hmmcopy_reads_cols=None) -> AnnData:
     """ Read hmmcopy results from the DLP pipeline.
 
     Parameters
-    ------
-    alignment_results_dir (str):
+    ----------
+    alignment_results_dir : str
         dlp pipeline alignment results directory
-    hmmcopy_results_dir (str):
+    hmmcopy_results_dir : str
         dlp pipeline hmmcopy results directory
-    annotation_results_dir (str):
+    annotation_results_dir : str
         dlp pipeline annotation results directory
-    sample_ids (list):
+    sample_ids : list
         sample ids to load
-    additional_hmmcopy_reads_cols (list):
+    additional_hmmcopy_reads_cols : list
         per bin metrics to load
 
     Returns
-    ------
+    -------
     AnnData
         An instantiated AnnData Object.
     """
 
+
     results = scgenome.loaders.qc.load_qc_results(
         alignment_results_dir,
         hmmcopy_results_dir,
         annotation_results_dir,
         sample_ids=sample_ids,
         additional_hmmcopy_reads_cols=additional_hmmcopy_reads_cols,
     )
@@ -49,24 +50,24 @@
     return convert_dlp_hmmcopy(metrics_data, cn_data)
 
 
 def read_dlp_hmmcopy2(reads_filename, metrics_filename, sample_ids=None) -> AnnData:
     """ Read hmmcopy results from the DLP pipeline.
 
     Parameters
-    ------
+    ----------
     reads_filename (str):
         dlp pipeline reads filename
     metrics_filename (str):
         dlp pipeline metrics filename
     sample_ids (list):
         sample ids to load
 
     Returns
-    ------
+    -------
     AnnData
         An instantiated AnnData Object.
     """
 
     cn_data = csverve.read_csv(
         reads_filename,
         dtype={
@@ -130,43 +131,58 @@
     duplicate_cell_ids = cn_data.loc[cn_data[['chr', 'start', 'end', 'cell_id']].duplicated(keep=False), 'cell_id'].unique()
     if len(duplicate_cell_ids) > 0:
         raise ValueError(f'cell {duplicate_cell_ids[0]} is duplicated, and {len(duplicate_cell_ids)} others')
 
     assert not cell_metrics_data.duplicated(subset=['cell_id']).any()
     assert not bin_metrics_data.duplicated(subset=['chr', 'start', 'end']).any()
 
-    cn_matrix = (
+    X = (
         cn_data
-            .set_index(['chr', 'start', 'end', 'cell_id'])[layers_columns + [X_column]]
+            .set_index(['chr', 'start', 'end', 'cell_id'])[X_column]
             .unstack(level='cell_id')
             .transpose())
+    X.index = X.index.astype(str)
+
+    chr_start_end_index = X.columns
+    bin_index = (
+        X.columns.get_level_values('chr').astype(str) + ':' +
+        X.columns.get_level_values('start').astype(str) + '-' +
+        X.columns.get_level_values('end').astype(str))
+
+    X = X.set_axis(bin_index, axis=1, copy=False)
+
+    layers = {}
+    for layer_name in layers_columns:
+        layers[layer_name] = (
+            cn_data
+                .set_index(['chr', 'start', 'end', 'cell_id'])[layer_name]
+                .unstack(level='cell_id')
+                .transpose()
+                .reindex(index=X.index, columns=chr_start_end_index)
+                .set_axis(bin_index, axis=1, copy=False))
+        layers[layer_name].index = layers[layer_name].index.astype(str)
 
     bin_data = (
         bin_metrics_data
             .set_index(['chr', 'start', 'end'], drop=False)
-            .reindex(cn_matrix.loc[X_column].columns))
+            .reindex(index=chr_start_end_index)
+            .set_axis(bin_index, axis=0))
 
     cell_data = (
         cell_metrics_data
             .set_index(['cell_id'])
-            .reindex(cn_matrix.loc[X_column].index))
-
-    bin_index = (
-        cn_matrix.columns.get_level_values('chr').astype(str) + ':' +
-        cn_matrix.columns.get_level_values('start').astype(str) + '-' +
-        cn_matrix.columns.get_level_values('end').astype(str))
-
-    cn_matrix.set_axis(bin_index, axis=1, inplace=True)
-    bin_data.set_axis(bin_index, axis=0, inplace=True)
+            .reindex(X.index))
+    cell_data.index = cell_data.index.astype(str)
 
     adata = ad.AnnData(
-        cn_matrix.loc[X_column],
+        X,
+        dtype=X.dtypes[0],
         obs=cell_data,
         var=bin_data,
-        layers={a: cn_matrix.loc[a] for a in layers_columns},
+        layers=layers,
     )
 
     return adata
 
 
 def convert_dlp_hmmcopy(metrics_data: DataFrame, cn_data: DataFrame) -> AnnData:
     """ Convert hmmcopy pandas dataframes to anndata
@@ -242,15 +258,15 @@
 def read_bam_bin_counts(bins: PyRanges, bams: Dict[str, str], excluded: PyRanges = None, **kwargs) -> AnnData:
     """ Count reads in bins from bams
 
     Parameters
     ----------
     bins : pyranges.PyRanges
         bins in which to count reads
-    bams : Dict[Str]
+    bams : Dict[str]
         bam filenames with cell ids as keys
     excluded: PyRanges
         excluded genomic regions to filter reads
 
     Returns
     -------
     ad.AnnData
@@ -273,17 +289,19 @@
         logging.info(f"count overlaps")
         bam_data = bam_data.intersect(bins, how='containment')
         read_counts = bins.count_overlaps(bam_data, overlap_col='reads')
 
         read_counts = _convert_pyranges(read_counts)
         read_counts = _add_bin_index(read_counts)
 
-        cn_matrix[cell_id] = read_counts['reads']
+        assert (read_counts.index == bin_data.index).all()
+
+        cn_matrix[cell_id] = read_counts['reads'].values.copy()
 
-    cn_matrix = pd.DataFrame(cn_matrix)
+    cn_matrix = pd.DataFrame(cn_matrix, index=bin_data.index)
 
     cell_data = pd.DataFrame({'cell_id': cn_matrix.columns.values}).set_index('cell_id')
 
     adata = ad.AnnData(
         cn_matrix.T,
         obs=cell_data,
         var=bin_data,
```

### Comparing `scgenome-0.0.8/scgenome/preprocessing/load_snv.py` & `scgenome-0.0.9/scgenome/preprocessing/load_snv.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/preprocessing/transform.py` & `scgenome-0.0.9/scgenome/preprocessing/transform.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/snpdata.py` & `scgenome-0.0.9/scgenome/snpdata.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/snvdata.py` & `scgenome-0.0.9/scgenome/snvdata.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/snvphylo.py` & `scgenome-0.0.9/scgenome/snvphylo.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/tools/binfeat.py` & `scgenome-0.0.9/scgenome/tools/binfeat.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/tools/cluster.py` & `scgenome-0.0.9/scgenome/tools/cluster.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,36 @@
     max_k : int, optional
         maximum number of clusters, by default 100
 
     Returns
     -------
     AnnData
         copy number data with additional `cluster_id` column
+
+    Examples
+    -------
+
+    >>> import scgenome
+    >>> import anndata as ad
+    >>> import numpy as np
+    >>> adata = ad.AnnData(np.array([
+    ...    [3, 3, 3, 6, 6],
+    ...    [1, 1, 1, 2, 2],
+    ...    [1, 22, 1, 2, 2],
+    ...    [1, 3, 3, 5, 5],
+    ... ]).astype(np.float32))
+    >>> adata = scgenome.tl.cluster_cells_kmeans(adata, layer_name=None, max_k=3)
+    >>> adata.obs['cluster_id']
+    0    0
+    1    2
+    2    1
+    3    0
+    Name: cluster_id, dtype: category
+    Categories (3, int64): [0, 1, 2]
+
     """
 
     if layer_name is not None:
         X = adata.layers[layer_name]
     else:
         X = adata.X
```

### Comparing `scgenome-0.0.8/scgenome/tools/concat.py` & `scgenome-0.0.9/scgenome/tools/concat.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/tools/genes.py` & `scgenome-0.0.9/scgenome/tools/genes.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/tools/pca.py` & `scgenome-0.0.9/scgenome/tools/pca.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/tools/sorting.py` & `scgenome-0.0.9/scgenome/tools/sorting.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome/utils.py` & `scgenome-0.0.9/scgenome/utils.py`

 * *Files identical despite different names*

### Comparing `scgenome-0.0.8/scgenome.egg-info/SOURCES.txt` & `scgenome-0.0.9/scgenome.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 MANIFEST.in
 README.md
-pyproject.toml
 setup.cfg
 setup.py
 versioneer.py
 scgenome/__init__.py
 scgenome/_version.py
 scgenome/breakpointdata.py
 scgenome/cnclones.py
@@ -20,30 +19,29 @@
 scgenome/snvphylo.py
 scgenome/utils.py
 scgenome.egg-info/PKG-INFO
 scgenome.egg-info/SOURCES.txt
 scgenome.egg-info/dependency_links.txt
 scgenome.egg-info/requires.txt
 scgenome.egg-info/top_level.txt
-scgenome/data/GRCh37-lite.fa.fai
+scgenome/data/grch38.fa.fai
+scgenome/data/hg19.fa.fai
 scgenome/data/mm10.fa.fai
+scgenome/datasets/__init__.py
+scgenome/datasets/_datasets.py
+scgenome/datasets/data/OV2295_HMMCopy_reduced.h5ad
 scgenome/loaders/__init__.py
 scgenome/loaders/align.py
 scgenome/loaders/allele.py
 scgenome/loaders/annotation.py
 scgenome/loaders/breakpoint.py
 scgenome/loaders/hmmcopy.py
 scgenome/loaders/qc.py
 scgenome/loaders/snv.py
 scgenome/loaders/utils.py
-scgenome/loaders/dtypes/alignment_gc_metrics_defs.yaml
-scgenome/loaders/dtypes/hmmcopy_params_defs.yaml
-scgenome/loaders/dtypes/hmmcopy_reads_defs.yaml
-scgenome/loaders/dtypes/hmmcopy_segments_defs.yaml
-scgenome/loaders/dtypes/metrics_column_defs.yaml
 scgenome/plotting/__init__.py
 scgenome/plotting/cn.py
 scgenome/plotting/heatmap.py
 scgenome/plotting/phylo.py
 scgenome/plotting/qc.py
 scgenome/preprocessing/__init__.py
 scgenome/preprocessing/filtering.py
```

### Comparing `scgenome-0.0.8/setup.py` & `scgenome-0.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         'adjustText',
         'anndata',
         'bamread',
         'biopython',
         'bokeh',
         'brewer2mpl',
         'Click',
-        'csverve',
+        'csverve>=0.3.1',
         'hdbscan',
         'hmmlearn',
         'ipython',
         'jupyter',
         'lda',
         'matplotlib',
         'nose',
@@ -37,16 +37,21 @@
         'PyYAML',
         'scikit-learn',
         'scipy',
         'seaborn',
         'statsmodels',
         'umap-learn',
         'wgs_analysis',
+        'nose',
+        'biopython',
+        'pypeliner',
+        'joblib==1.1.0',
+        'sphinx==5.1.1'
     ],
     package_data={
         'scgenome': [
-            'data/mm10.fa.fai',
-            'data/GRCh37-lite.fa.fai',
+            'data/*',
             'dtypes/*.yaml',
+            'datasets/data/*'
         ],
     },
 )
```

### Comparing `scgenome-0.0.8/versioneer.py` & `scgenome-0.0.9/versioneer.py`

 * *Files identical despite different names*

