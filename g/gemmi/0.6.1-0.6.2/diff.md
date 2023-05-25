# Comparing `tmp/gemmi-0.6.1.tar.gz` & `tmp/gemmi-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemmi-0.6.1.tar", last modified: Tue Apr 18 20:39:49 2023, max compression
+gzip compressed data, was "gemmi-0.6.2.tar", last modified: Thu May 25 11:57:59 2023, max compression
```

## Comparing `gemmi-0.6.1.tar` & `gemmi-0.6.2.tar`

### file list

```diff
@@ -1,344 +1,346 @@
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.036314 gemmi-0.6.1/
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16726 2020-07-10 20:35:39.000000 gemmi-0.6.1/LICENSE.txt
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      389 2022-08-01 10:42:25.000000 gemmi-0.6.1/MANIFEST.in
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2111 2023-04-18 20:39:49.036314 gemmi-0.6.1/PKG-INFO
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1390 2023-04-15 23:14:09.000000 gemmi-0.6.1/README.md
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.000314 gemmi-0.6.1/examples/
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)        0 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/__init__.py
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      396 2020-08-19 11:40:21.000000 gemmi-0.6.1/examples/__main__.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1380 2020-08-19 11:40:21.000000 gemmi-0.6.1/examples/aafreq.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     2378 2023-03-05 13:04:05.000000 gemmi-0.6.1/examples/ccd_gi.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1266 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/ccd_subgraph.py
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      529 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/cif_i_sigi.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1338 2020-08-19 11:40:21.000000 gemmi-0.6.1/examples/col_order.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)      763 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/from_json.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)      503 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/hello.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1442 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/long_geom.py
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      605 2022-04-23 21:43:35.000000 gemmi-0.6.1/examples/map2mtz.py
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3590 2022-04-23 21:43:35.000000 gemmi-0.6.1/examples/maskcheck.py
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      824 2022-04-23 21:43:35.000000 gemmi-0.6.1/examples/maskdiff.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     6855 2020-08-19 11:40:21.000000 gemmi-0.6.1/examples/matthews.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1446 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/merge_mtz_mmcif.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     5382 2020-08-19 11:40:21.000000 gemmi-0.6.1/examples/monomers.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1101 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/mtrix_iso.py
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      575 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/mtz_i_sigi.py
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      571 2021-03-08 21:34:35.000000 gemmi-0.6.1/examples/multiproc.py
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      564 2022-04-23 21:43:35.000000 gemmi-0.6.1/examples/patterson_slice.py
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1315 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/rama_gather.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1145 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/rama_plot.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)      361 2020-08-19 11:40:21.000000 gemmi-0.6.1/examples/simple_search.py
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      568 2020-07-10 20:35:39.000000 gemmi-0.6.1/examples/sub_ccd.py
--rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     4960 2021-02-26 16:20:11.000000 gemmi-0.6.1/examples/weight.py
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.000314 gemmi-0.6.1/gemmi.egg-info/
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2111 2023-04-18 20:39:48.000000 gemmi-0.6.1/gemmi.egg-info/PKG-INFO
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    11864 2023-04-18 20:39:48.000000 gemmi-0.6.1/gemmi.egg-info/SOURCES.txt
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)        1 2023-04-18 20:39:48.000000 gemmi-0.6.1/gemmi.egg-info/dependency_links.txt
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)        1 2021-05-18 19:29:14.000000 gemmi-0.6.1/gemmi.egg-info/not-zip-safe
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)       21 2023-04-18 20:39:48.000000 gemmi-0.6.1/gemmi.egg-info/top_level.txt
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:48.996314 gemmi-0.6.1/include/
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.012314 gemmi-0.6.1/include/gemmi/
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      844 2020-12-01 20:02:25.000000 gemmi-0.6.1/include/gemmi/addends.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    11033 2022-10-12 14:10:08.000000 gemmi-0.6.1/include/gemmi/align.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4590 2023-04-03 18:48:39.000000 gemmi-0.6.1/include/gemmi/assembly.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7484 2023-02-01 21:08:48.000000 gemmi-0.6.1/include/gemmi/asudata.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    11431 2022-08-23 21:05:21.000000 gemmi-0.6.1/include/gemmi/asumask.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1023 2022-08-01 10:43:22.000000 gemmi-0.6.1/include/gemmi/atof.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3791 2021-05-20 19:43:31.000000 gemmi-0.6.1/include/gemmi/atox.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3983 2022-04-23 21:43:35.000000 gemmi-0.6.1/include/gemmi/bessel.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6974 2023-02-01 21:07:05.000000 gemmi-0.6.1/include/gemmi/binner.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4864 2022-06-13 10:43:35.000000 gemmi-0.6.1/include/gemmi/blob.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3045 2023-04-18 20:21:43.000000 gemmi-0.6.1/include/gemmi/bond_idx.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    10368 2022-08-23 21:23:50.000000 gemmi-0.6.1/include/gemmi/c4322.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5574 2023-03-21 08:04:35.000000 gemmi-0.6.1/include/gemmi/calculate.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    17280 2022-09-07 12:58:00.000000 gemmi-0.6.1/include/gemmi/ccp4.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    13372 2022-05-18 17:02:25.000000 gemmi-0.6.1/include/gemmi/cellred.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    23755 2023-04-14 09:25:55.000000 gemmi-0.6.1/include/gemmi/chemcomp.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4657 2023-03-29 11:09:35.000000 gemmi-0.6.1/include/gemmi/chemcomp_xyz.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    13992 2022-12-28 09:35:27.000000 gemmi-0.6.1/include/gemmi/cif.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    15241 2023-04-17 21:09:38.000000 gemmi-0.6.1/include/gemmi/cif2mtz.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    35703 2022-10-14 19:25:51.000000 gemmi-0.6.1/include/gemmi/cifdoc.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5036 2023-04-13 00:17:52.000000 gemmi-0.6.1/include/gemmi/contact.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      543 2023-04-15 22:21:44.000000 gemmi-0.6.1/include/gemmi/crd.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7049 2023-02-07 09:15:44.000000 gemmi-0.6.1/include/gemmi/dencalc.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6965 2021-10-27 09:15:46.000000 gemmi-0.6.1/include/gemmi/dirwalk.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      314 2023-03-17 20:22:37.000000 gemmi-0.6.1/include/gemmi/eig3.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    14634 2022-10-14 12:06:03.000000 gemmi-0.6.1/include/gemmi/elem.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4526 2022-10-11 18:19:45.000000 gemmi-0.6.1/include/gemmi/enumstr.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2123 2023-03-04 21:35:09.000000 gemmi-0.6.1/include/gemmi/fail.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5371 2022-04-23 21:43:35.000000 gemmi-0.6.1/include/gemmi/fileutil.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5139 2022-06-09 09:52:00.000000 gemmi-0.6.1/include/gemmi/floodfill.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4468 2023-01-31 21:22:45.000000 gemmi-0.6.1/include/gemmi/formfact.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    13191 2022-10-26 13:00:57.000000 gemmi-0.6.1/include/gemmi/fourier.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)   271931 2022-10-31 20:46:06.000000 gemmi-0.6.1/include/gemmi/fprime.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2222 2021-05-24 17:07:41.000000 gemmi-0.6.1/include/gemmi/fstream.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    26551 2023-02-01 21:08:11.000000 gemmi-0.6.1/include/gemmi/grid.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5182 2023-03-02 00:39:15.000000 gemmi-0.6.1/include/gemmi/gz.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4512 2021-12-22 18:43:49.000000 gemmi-0.6.1/include/gemmi/input.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1846 2022-09-12 17:26:20.000000 gemmi-0.6.1/include/gemmi/interop.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    10429 2022-08-23 21:24:04.000000 gemmi-0.6.1/include/gemmi/it92.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     9757 2022-04-23 21:43:35.000000 gemmi-0.6.1/include/gemmi/iterator.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4820 2021-12-07 17:42:29.000000 gemmi-0.6.1/include/gemmi/json.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     9023 2023-02-23 15:44:49.000000 gemmi-0.6.1/include/gemmi/levmar.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6788 2023-04-13 00:17:52.000000 gemmi-0.6.1/include/gemmi/linkhunt.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    14300 2023-03-17 19:40:39.000000 gemmi-0.6.1/include/gemmi/math.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16984 2023-02-01 21:10:16.000000 gemmi-0.6.1/include/gemmi/merge.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    13592 2023-03-16 21:39:04.000000 gemmi-0.6.1/include/gemmi/metadata.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      991 2023-03-04 21:10:00.000000 gemmi-0.6.1/include/gemmi/mmcif.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1243 2023-01-20 13:06:29.000000 gemmi-0.6.1/include/gemmi/mmcif_impl.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     9234 2023-03-17 14:07:43.000000 gemmi-0.6.1/include/gemmi/mmdb.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3894 2022-10-06 22:31:53.000000 gemmi-0.6.1/include/gemmi/mmread.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      818 2023-03-04 21:07:51.000000 gemmi-0.6.1/include/gemmi/mmread_gz.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    35817 2023-03-17 12:43:09.000000 gemmi-0.6.1/include/gemmi/model.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6285 2022-11-14 14:06:08.000000 gemmi-0.6.1/include/gemmi/modify.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    11283 2023-03-28 13:58:50.000000 gemmi-0.6.1/include/gemmi/monlib.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    38452 2023-04-18 17:28:58.000000 gemmi-0.6.1/include/gemmi/mtz.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4439 2023-04-15 22:22:09.000000 gemmi-0.6.1/include/gemmi/mtz2cif.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    13422 2023-04-13 09:39:56.000000 gemmi-0.6.1/include/gemmi/neighbor.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2787 2022-04-23 21:43:35.000000 gemmi-0.6.1/include/gemmi/neutron92.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1479 2022-08-01 10:43:31.000000 gemmi-0.6.1/include/gemmi/numb.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    26254 2023-04-16 18:00:05.000000 gemmi-0.6.1/include/gemmi/pdb.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1287 2020-08-26 14:14:17.000000 gemmi-0.6.1/include/gemmi/pirfasta.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     8257 2023-04-15 22:23:44.000000 gemmi-0.6.1/include/gemmi/polyheur.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    12909 2021-12-29 23:52:19.000000 gemmi-0.6.1/include/gemmi/qcp.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      954 2023-03-04 21:08:41.000000 gemmi-0.6.1/include/gemmi/read_cif.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1117 2022-09-08 19:52:57.000000 gemmi-0.6.1/include/gemmi/read_map.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5846 2023-01-31 21:22:45.000000 gemmi-0.6.1/include/gemmi/recgrid.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1992 2023-02-04 08:56:39.000000 gemmi-0.6.1/include/gemmi/reciproc.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     8857 2023-01-20 13:06:29.000000 gemmi-0.6.1/include/gemmi/refln.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    25493 2023-03-13 12:53:53.000000 gemmi-0.6.1/include/gemmi/remarks.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2849 2023-03-04 21:17:00.000000 gemmi-0.6.1/include/gemmi/resinfo.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1016 2023-03-27 14:36:57.000000 gemmi-0.6.1/include/gemmi/riding_h.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    11608 2022-11-23 12:18:21.000000 gemmi-0.6.1/include/gemmi/scaling.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16331 2023-04-05 08:00:20.000000 gemmi-0.6.1/include/gemmi/select.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    10437 2021-04-18 11:38:33.000000 gemmi-0.6.1/include/gemmi/seqalign.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5125 2023-03-01 16:42:39.000000 gemmi-0.6.1/include/gemmi/seqid.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5432 2023-01-31 21:22:45.000000 gemmi-0.6.1/include/gemmi/sfcalc.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4034 2021-12-06 18:48:11.000000 gemmi-0.6.1/include/gemmi/small.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6843 2021-12-06 18:46:12.000000 gemmi-0.6.1/include/gemmi/smcif.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    17639 2022-08-23 21:05:21.000000 gemmi-0.6.1/include/gemmi/solmask.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4668 2022-08-30 15:08:57.000000 gemmi-0.6.1/include/gemmi/span.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1521 2023-01-27 13:29:28.000000 gemmi-0.6.1/include/gemmi/sprintf.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2761 2023-02-01 21:07:17.000000 gemmi-0.6.1/include/gemmi/stats.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    92527 2023-02-03 17:41:30.000000 gemmi-0.6.1/include/gemmi/symmetry.hpp
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.012314 gemmi-0.6.1/include/gemmi/third_party/
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)   114265 2023-01-19 09:46:30.000000 gemmi-0.6.1/include/gemmi/third_party/fast_float.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)   107015 2021-08-26 08:18:28.000000 gemmi-0.6.1/include/gemmi/third_party/pocketfft_hdronly.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    95912 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/sajson.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    58248 2023-03-02 00:36:53.000000 gemmi-0.6.1/include/gemmi/third_party/stb_sprintf.h
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.012314 gemmi-0.6.1/include/gemmi/third_party/tao/
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1104 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/LICENSE
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      359 2022-05-19 09:34:03.000000 gemmi-0.6.1/include/gemmi/third_party/tao/NOTES
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.016314 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.016314 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4544 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/analyze_cycles.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      646 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/counted.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      954 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/generic.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      943 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/grammar_info.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1705 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/insert_guard.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1099 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/insert_rules.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      749 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/rule_info.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      990 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/rule_type.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      559 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analyze.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      451 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/apply_mode.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1339 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/argv_input.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3463 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/ascii.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5021 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/buffer_input.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      534 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/config.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      872 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/cstream_input.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1042 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/eol.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      440 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/eol_pair.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      961 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/file_input.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1513 2021-05-24 17:06:09.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/input_error.hpp
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.024314 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1439 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/action.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2869 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/action_input.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      548 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/alnum.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      538 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/alpha.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1664 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/any.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2750 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/apply.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2521 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/apply0.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1154 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/apply0_single.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1229 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/apply_single.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1626 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/at.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      862 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/bof.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      870 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/bol.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1573 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/bump_help.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1373 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/bump_impl.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1076 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/bytes.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1445 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/control.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1049 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/cr_crlf_eol.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      975 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/cr_eol.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1025 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/crlf_eol.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1389 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/cstream_reader.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1178 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/cstring_reader.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      843 2022-08-06 17:18:16.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/demangle.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1045 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/demangle_cxxabi.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      567 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/demangle_nop.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1376 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/demangle_sanitise.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1382 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/disable.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1003 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/discard.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      616 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/dusel_mode.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7228 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/duseltronik.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1377 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/enable.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1557 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/endian.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5410 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/endian_gcc.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2938 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/endian_win.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      884 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/eof.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      920 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/eol.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      974 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/eolf.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2518 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/file_mapper.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2011 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/file_opener.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3297 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/file_reader.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      751 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/has_apply.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      756 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/has_apply0.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      772 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/identifier.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3802 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/if_apply.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      580 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/if_must.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      634 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/if_must_else.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1862 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/if_then_else.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      723 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/input_pair.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3323 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/integer_sequence.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1159 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/istream_reader.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2766 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/istring.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1493 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/iterator.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1229 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/lf_crlf_eol.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      975 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/lf_eol.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      567 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/list.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      610 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/list_must.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      607 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/list_tail.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      697 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/list_tail_pad.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2409 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/marker.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2092 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/minus.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2484 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/must.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1652 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/not_at.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2429 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/one.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1648 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/opt.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      596 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/pad.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      609 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/pad_opt.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      837 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/peek_char.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2245 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/peek_utf16.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1800 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/peek_utf32.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2931 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/peek_utf8.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4180 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/pegtl_string.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1786 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/plus.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1598 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/raise.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1684 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/range.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2994 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/ranges.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2020 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rep.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      641 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rep_min.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2880 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rep_min_max.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1500 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rep_opt.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1172 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/require.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      568 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/result_on_found.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1910 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rule_conjunction.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1393 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rules.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2240 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/seq.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      903 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/skip_control.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2150 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/sor.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1494 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/star.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      594 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/star_must.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2769 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/state.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1736 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/string.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      955 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/trivial.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1972 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/try_catch_type.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2874 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/until.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      876 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/istream_input.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     9778 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/memory_input.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1913 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/mmap_input.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3897 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/normal.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      586 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/nothing.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1616 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/parse.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1106 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/parse_error.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1351 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/position.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2198 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/read_input.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      459 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/rewind_mode.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4942 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/rules.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1936 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/string_input.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      445 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/tracking_mode.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2832 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/utf16.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2832 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/utf32.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1553 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/utf8.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      602 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/version.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      793 2020-07-10 20:35:39.000000 gemmi-0.6.1/include/gemmi/third_party/tao/pegtl.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    19235 2022-04-23 21:43:35.000000 gemmi-0.6.1/include/gemmi/third_party/tinydir.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2797 2022-11-12 21:59:36.000000 gemmi-0.6.1/include/gemmi/to_chemcomp.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6242 2022-11-08 19:08:56.000000 gemmi-0.6.1/include/gemmi/to_cif.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     8862 2021-11-15 18:03:22.000000 gemmi-0.6.1/include/gemmi/to_json.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2391 2023-03-21 15:10:08.000000 gemmi-0.6.1/include/gemmi/to_mmcif.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      862 2023-03-04 21:20:57.000000 gemmi-0.6.1/include/gemmi/to_pdb.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    10769 2023-04-14 09:26:04.000000 gemmi-0.6.1/include/gemmi/topo.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    10282 2022-10-14 12:11:45.000000 gemmi-0.6.1/include/gemmi/twin.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    21692 2022-10-27 19:50:42.000000 gemmi-0.6.1/include/gemmi/unitcell.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2476 2021-04-17 18:25:34.000000 gemmi-0.6.1/include/gemmi/utf.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     8661 2023-02-09 23:24:19.000000 gemmi-0.6.1/include/gemmi/util.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      152 2023-04-18 20:19:22.000000 gemmi-0.6.1/include/gemmi/version.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    14985 2023-03-22 12:06:35.000000 gemmi-0.6.1/include/gemmi/xds_ascii.hpp
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.028314 gemmi-0.6.1/python/
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4085 2022-09-12 16:59:12.000000 gemmi-0.6.1/python/align.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      327 2022-02-04 16:03:43.000000 gemmi-0.6.1/python/arrvec.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2447 2022-12-21 13:51:11.000000 gemmi-0.6.1/python/ccp4.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     8464 2023-02-16 00:04:33.000000 gemmi-0.6.1/python/chemcomp.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    17105 2022-12-21 13:17:59.000000 gemmi-0.6.1/python/cif.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3052 2023-03-17 18:03:23.000000 gemmi-0.6.1/python/common.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      195 2022-01-13 20:51:13.000000 gemmi-0.6.1/python/custom.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5307 2022-10-09 18:06:55.000000 gemmi-0.6.1/python/elem.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6075 2023-03-17 18:03:23.000000 gemmi-0.6.1/python/gemmi.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    12480 2022-10-26 15:34:30.000000 gemmi-0.6.1/python/grid.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16824 2023-02-04 08:44:54.000000 gemmi-0.6.1/python/hkl.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16973 2023-03-17 13:35:13.000000 gemmi-0.6.1/python/meta.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      745 2023-02-18 19:56:19.000000 gemmi-0.6.1/python/meta.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      571 2021-01-14 17:40:02.000000 gemmi-0.6.1/python/miller_a.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    26685 2023-04-03 18:53:47.000000 gemmi-0.6.1/python/mol.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5526 2023-03-27 16:12:52.000000 gemmi-0.6.1/python/monlib.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    14926 2023-03-14 19:10:45.000000 gemmi-0.6.1/python/mtz.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7676 2023-01-19 17:21:52.000000 gemmi-0.6.1/python/read.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     9555 2022-12-21 20:39:07.000000 gemmi-0.6.1/python/recgrid.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2005 2022-04-23 21:43:35.000000 gemmi-0.6.1/python/scaling.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6733 2023-04-13 08:18:16.000000 gemmi-0.6.1/python/search.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3819 2023-01-31 21:22:45.000000 gemmi-0.6.1/python/sf.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    12208 2023-03-10 16:44:25.000000 gemmi-0.6.1/python/sym.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7386 2023-04-14 09:26:04.000000 gemmi-0.6.1/python/topo.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      835 2022-04-23 21:43:35.000000 gemmi-0.6.1/python/tostr.hpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    17460 2023-04-13 15:15:53.000000 gemmi-0.6.1/python/unitcell.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3795 2023-03-13 17:58:41.000000 gemmi-0.6.1/python/write.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      178 2023-04-18 20:39:49.036314 gemmi-0.6.1/setup.cfg
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7613 2023-04-16 18:07:18.000000 gemmi-0.6.1/setup.py
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.032314 gemmi-0.6.1/src/
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    15603 2023-04-13 00:17:52.000000 gemmi-0.6.1/src/assembly.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      927 2023-03-15 20:18:52.000000 gemmi-0.6.1/src/calculate.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    23793 2023-04-14 09:27:01.000000 gemmi-0.6.1/src/crd.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5709 2023-03-17 20:24:22.000000 gemmi-0.6.1/src/eig3.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    37325 2023-03-17 09:08:42.000000 gemmi-0.6.1/src/mmcif.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      697 2023-01-19 17:16:44.000000 gemmi-0.6.1/src/mmread_gz.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    20572 2023-04-13 00:17:52.000000 gemmi-0.6.1/src/monlib.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    11299 2023-03-14 20:24:04.000000 gemmi-0.6.1/src/mtz.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    37188 2023-04-15 22:22:44.000000 gemmi-0.6.1/src/mtz2cif.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     9007 2023-04-15 22:41:28.000000 gemmi-0.6.1/src/polyheur.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      899 2023-01-19 17:18:32.000000 gemmi-0.6.1/src/read_cif.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    24654 2023-04-15 12:45:01.000000 gemmi-0.6.1/src/resinfo.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    17837 2023-04-15 22:24:51.000000 gemmi-0.6.1/src/riding_h.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)       99 2023-01-03 20:55:04.000000 gemmi-0.6.1/src/sprintf.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    52888 2023-03-21 15:10:08.000000 gemmi-0.6.1/src/to_mmcif.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    26456 2023-04-15 22:14:14.000000 gemmi-0.6.1/src/to_pdb.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    39163 2023-04-14 09:26:04.000000 gemmi-0.6.1/src/topo.cpp
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2219 2023-03-01 16:42:39.000000 gemmi-0.6.1/src/xds_ascii.cpp
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:48.996314 gemmi-0.6.1/third_party/
-drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-04-18 20:39:49.036314 gemmi-0.6.1/third_party/zlib/
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5204 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/adler32.c
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    14053 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/crc32.c
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    30562 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/crc32.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6819 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/gzguts.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16599 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/gzlib.c
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    20428 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/gzread.c
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    12978 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/inffast.c
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      427 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/inffast.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6332 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/inffixed.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    54800 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/inflate.c
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6618 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/inflate.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    12999 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/inftrees.c
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2928 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/inftrees.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1031 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/license
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16298 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/zconf.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    96239 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/zlib.h
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7304 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/zutil.c
--rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7127 2020-07-10 20:35:39.000000 gemmi-0.6.1/third_party/zlib/zutil.h
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-05-25 11:57:59.143690 gemmi-0.6.2/
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16726 2020-07-10 20:35:39.000000 gemmi-0.6.2/LICENSE.txt
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      375 2023-05-01 08:51:11.000000 gemmi-0.6.2/MANIFEST.in
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2111 2023-05-25 11:57:59.143690 gemmi-0.6.2/PKG-INFO
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1390 2023-04-15 23:14:09.000000 gemmi-0.6.2/README.md
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-05-25 11:57:59.115690 gemmi-0.6.2/examples/
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)        0 2020-07-10 20:35:39.000000 gemmi-0.6.2/examples/__init__.py
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      396 2020-08-19 11:40:21.000000 gemmi-0.6.2/examples/__main__.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1214 2023-04-20 16:04:05.000000 gemmi-0.6.2/examples/aafreq.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     2378 2023-03-05 13:04:05.000000 gemmi-0.6.2/examples/ccd_gi.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1266 2020-07-10 20:35:39.000000 gemmi-0.6.2/examples/ccd_subgraph.py
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      529 2020-07-10 20:35:39.000000 gemmi-0.6.2/examples/cif_i_sigi.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1338 2020-08-19 11:40:21.000000 gemmi-0.6.2/examples/col_order.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)      763 2020-07-10 20:35:39.000000 gemmi-0.6.2/examples/from_json.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)      503 2020-07-10 20:35:39.000000 gemmi-0.6.2/examples/hello.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1442 2020-07-10 20:35:39.000000 gemmi-0.6.2/examples/long_geom.py
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      605 2023-05-09 17:15:58.000000 gemmi-0.6.2/examples/map2mtz.py
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3590 2022-04-23 21:43:35.000000 gemmi-0.6.2/examples/maskcheck.py
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      824 2022-04-23 21:43:35.000000 gemmi-0.6.2/examples/maskdiff.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     6855 2020-08-19 11:40:21.000000 gemmi-0.6.2/examples/matthews.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1446 2020-07-10 20:35:39.000000 gemmi-0.6.2/examples/merge_mtz_mmcif.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     5382 2020-08-19 11:40:21.000000 gemmi-0.6.2/examples/monomers.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1090 2023-04-19 20:00:50.000000 gemmi-0.6.2/examples/mtrix_iso.py
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      575 2020-07-10 20:35:39.000000 gemmi-0.6.2/examples/mtz_i_sigi.py
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      571 2021-03-08 21:34:35.000000 gemmi-0.6.2/examples/multiproc.py
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      564 2022-04-23 21:43:35.000000 gemmi-0.6.2/examples/patterson_slice.py
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1315 2020-07-10 20:35:39.000000 gemmi-0.6.2/examples/rama_gather.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     1145 2020-07-10 20:35:39.000000 gemmi-0.6.2/examples/rama_plot.py
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1453 2023-04-26 14:18:23.000000 gemmi-0.6.2/examples/refln-stats.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)      361 2020-08-19 11:40:21.000000 gemmi-0.6.2/examples/simple_search.py
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      568 2020-07-10 20:35:39.000000 gemmi-0.6.2/examples/sub_ccd.py
+-rwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)     4960 2021-02-26 16:20:11.000000 gemmi-0.6.2/examples/weight.py
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-05-25 11:57:59.115690 gemmi-0.6.2/gemmi.egg-info/
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2111 2023-05-25 11:57:59.000000 gemmi-0.6.2/gemmi.egg-info/PKG-INFO
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    11899 2023-05-25 11:57:59.000000 gemmi-0.6.2/gemmi.egg-info/SOURCES.txt
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)        1 2023-05-25 11:57:59.000000 gemmi-0.6.2/gemmi.egg-info/dependency_links.txt
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)        1 2023-05-25 11:57:59.000000 gemmi-0.6.2/gemmi.egg-info/not-zip-safe
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)       21 2023-05-25 11:57:59.000000 gemmi-0.6.2/gemmi.egg-info/top_level.txt
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-05-25 11:57:59.111689 gemmi-0.6.2/include/
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-05-25 11:57:59.123690 gemmi-0.6.2/include/gemmi/
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      844 2020-12-01 20:02:25.000000 gemmi-0.6.2/include/gemmi/addends.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    11033 2022-10-12 14:10:08.000000 gemmi-0.6.2/include/gemmi/align.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4590 2023-04-03 18:48:39.000000 gemmi-0.6.2/include/gemmi/assembly.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7484 2023-02-01 21:08:48.000000 gemmi-0.6.2/include/gemmi/asudata.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    11451 2023-04-29 08:48:43.000000 gemmi-0.6.2/include/gemmi/asumask.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1023 2022-08-01 10:43:22.000000 gemmi-0.6.2/include/gemmi/atof.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3810 2023-04-29 08:48:43.000000 gemmi-0.6.2/include/gemmi/atox.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3983 2022-04-23 21:43:35.000000 gemmi-0.6.2/include/gemmi/bessel.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6974 2023-02-01 21:07:05.000000 gemmi-0.6.2/include/gemmi/binner.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4864 2022-06-13 10:43:35.000000 gemmi-0.6.2/include/gemmi/blob.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3045 2023-04-18 20:21:43.000000 gemmi-0.6.2/include/gemmi/bond_idx.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    10368 2022-08-23 21:23:50.000000 gemmi-0.6.2/include/gemmi/c4322.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5574 2023-03-21 08:04:35.000000 gemmi-0.6.2/include/gemmi/calculate.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    17280 2022-09-07 12:58:00.000000 gemmi-0.6.2/include/gemmi/ccp4.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    13372 2022-05-18 17:02:25.000000 gemmi-0.6.2/include/gemmi/cellred.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    23755 2023-04-14 09:25:55.000000 gemmi-0.6.2/include/gemmi/chemcomp.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4657 2023-03-29 11:09:35.000000 gemmi-0.6.2/include/gemmi/chemcomp_xyz.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    14110 2023-05-22 10:02:59.000000 gemmi-0.6.2/include/gemmi/cif.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    21584 2023-05-08 17:49:49.000000 gemmi-0.6.2/include/gemmi/cif2mtz.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    35703 2022-10-14 19:25:51.000000 gemmi-0.6.2/include/gemmi/cifdoc.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5036 2023-04-13 00:17:52.000000 gemmi-0.6.2/include/gemmi/contact.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      543 2023-04-15 22:21:44.000000 gemmi-0.6.2/include/gemmi/crd.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7049 2023-02-07 09:15:44.000000 gemmi-0.6.2/include/gemmi/dencalc.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7422 2023-04-19 20:04:58.000000 gemmi-0.6.2/include/gemmi/dirwalk.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      314 2023-03-17 20:22:37.000000 gemmi-0.6.2/include/gemmi/eig3.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    14634 2022-10-14 12:06:03.000000 gemmi-0.6.2/include/gemmi/elem.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4526 2022-10-11 18:19:45.000000 gemmi-0.6.2/include/gemmi/enumstr.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2102 2023-04-27 11:46:03.000000 gemmi-0.6.2/include/gemmi/fail.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3810 2023-04-29 08:48:43.000000 gemmi-0.6.2/include/gemmi/fileutil.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5139 2022-06-09 09:52:00.000000 gemmi-0.6.2/include/gemmi/floodfill.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4468 2023-01-31 21:22:45.000000 gemmi-0.6.2/include/gemmi/formfact.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    13191 2022-10-26 13:00:57.000000 gemmi-0.6.2/include/gemmi/fourier.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)   271931 2022-10-31 20:46:06.000000 gemmi-0.6.2/include/gemmi/fprime.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2222 2021-05-24 17:07:41.000000 gemmi-0.6.2/include/gemmi/fstream.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    26551 2023-02-01 21:08:11.000000 gemmi-0.6.2/include/gemmi/grid.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5182 2023-03-02 00:39:15.000000 gemmi-0.6.2/include/gemmi/gz.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4512 2021-12-22 18:43:49.000000 gemmi-0.6.2/include/gemmi/input.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1846 2022-09-12 17:26:20.000000 gemmi-0.6.2/include/gemmi/interop.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    10429 2022-08-23 21:24:04.000000 gemmi-0.6.2/include/gemmi/it92.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     9757 2022-04-23 21:43:35.000000 gemmi-0.6.2/include/gemmi/iterator.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4820 2021-12-07 17:42:29.000000 gemmi-0.6.2/include/gemmi/json.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     9023 2023-02-23 15:44:49.000000 gemmi-0.6.2/include/gemmi/levmar.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6788 2023-04-13 00:17:52.000000 gemmi-0.6.2/include/gemmi/linkhunt.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    14300 2023-03-17 19:40:39.000000 gemmi-0.6.2/include/gemmi/math.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16861 2023-05-06 21:33:25.000000 gemmi-0.6.2/include/gemmi/merge.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    13775 2023-05-11 09:27:55.000000 gemmi-0.6.2/include/gemmi/metadata.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      991 2023-03-04 21:10:00.000000 gemmi-0.6.2/include/gemmi/mmcif.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1243 2023-01-20 13:06:29.000000 gemmi-0.6.2/include/gemmi/mmcif_impl.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     9234 2023-03-17 14:07:43.000000 gemmi-0.6.2/include/gemmi/mmdb.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3894 2022-10-06 22:31:53.000000 gemmi-0.6.2/include/gemmi/mmread.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      818 2023-03-04 21:07:51.000000 gemmi-0.6.2/include/gemmi/mmread_gz.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    36259 2023-05-15 18:09:04.000000 gemmi-0.6.2/include/gemmi/model.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6058 2023-05-20 12:39:17.000000 gemmi-0.6.2/include/gemmi/modify.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    11568 2023-05-10 16:37:42.000000 gemmi-0.6.2/include/gemmi/monlib.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    38452 2023-04-18 17:28:58.000000 gemmi-0.6.2/include/gemmi/mtz.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4439 2023-04-15 22:22:09.000000 gemmi-0.6.2/include/gemmi/mtz2cif.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    13422 2023-04-13 09:39:56.000000 gemmi-0.6.2/include/gemmi/neighbor.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2787 2022-04-23 21:43:35.000000 gemmi-0.6.2/include/gemmi/neutron92.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1479 2022-08-01 10:43:31.000000 gemmi-0.6.2/include/gemmi/numb.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    27207 2023-05-15 20:42:05.000000 gemmi-0.6.2/include/gemmi/pdb.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2083 2023-05-15 21:03:27.000000 gemmi-0.6.2/include/gemmi/pdb_id.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1287 2020-08-26 14:14:17.000000 gemmi-0.6.2/include/gemmi/pirfasta.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     8877 2023-05-15 19:35:56.000000 gemmi-0.6.2/include/gemmi/polyheur.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    12909 2021-12-29 23:52:19.000000 gemmi-0.6.2/include/gemmi/qcp.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      954 2023-03-04 21:08:41.000000 gemmi-0.6.2/include/gemmi/read_cif.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1117 2022-09-08 19:52:57.000000 gemmi-0.6.2/include/gemmi/read_map.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5846 2023-01-31 21:22:45.000000 gemmi-0.6.2/include/gemmi/recgrid.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1992 2023-02-04 08:56:39.000000 gemmi-0.6.2/include/gemmi/reciproc.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     8868 2023-04-20 20:07:53.000000 gemmi-0.6.2/include/gemmi/refln.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    25493 2023-03-13 12:53:53.000000 gemmi-0.6.2/include/gemmi/remarks.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2849 2023-03-04 21:17:00.000000 gemmi-0.6.2/include/gemmi/resinfo.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1016 2023-03-27 14:36:57.000000 gemmi-0.6.2/include/gemmi/riding_h.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    11608 2022-11-23 12:18:21.000000 gemmi-0.6.2/include/gemmi/scaling.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16331 2023-04-05 08:00:20.000000 gemmi-0.6.2/include/gemmi/select.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    10437 2021-04-18 11:38:33.000000 gemmi-0.6.2/include/gemmi/seqalign.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5125 2023-03-01 16:42:39.000000 gemmi-0.6.2/include/gemmi/seqid.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5432 2023-01-31 21:22:45.000000 gemmi-0.6.2/include/gemmi/sfcalc.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4034 2021-12-06 18:48:11.000000 gemmi-0.6.2/include/gemmi/small.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6843 2021-12-06 18:46:12.000000 gemmi-0.6.2/include/gemmi/smcif.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    17639 2022-08-23 21:05:21.000000 gemmi-0.6.2/include/gemmi/solmask.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4668 2022-08-30 15:08:57.000000 gemmi-0.6.2/include/gemmi/span.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2244 2023-04-29 10:04:00.000000 gemmi-0.6.2/include/gemmi/sprintf.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2761 2023-02-01 21:07:17.000000 gemmi-0.6.2/include/gemmi/stats.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    93297 2023-05-06 21:31:37.000000 gemmi-0.6.2/include/gemmi/symmetry.hpp
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-05-25 11:57:59.123690 gemmi-0.6.2/include/gemmi/third_party/
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)   114265 2023-01-19 09:46:30.000000 gemmi-0.6.2/include/gemmi/third_party/fast_float.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)   107015 2021-08-26 08:18:28.000000 gemmi-0.6.2/include/gemmi/third_party/pocketfft_hdronly.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    95912 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/sajson.h
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-05-25 11:57:59.127690 gemmi-0.6.2/include/gemmi/third_party/tao/
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1104 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/LICENSE
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      359 2022-05-19 09:34:03.000000 gemmi-0.6.2/include/gemmi/third_party/tao/NOTES
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-05-25 11:57:59.127690 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-05-25 11:57:59.127690 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/analysis/
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4544 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/analysis/analyze_cycles.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      646 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/analysis/counted.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      954 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/analysis/generic.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      943 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/analysis/grammar_info.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1705 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/analysis/insert_guard.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1099 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/analysis/insert_rules.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      749 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/analysis/rule_info.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      990 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/analysis/rule_type.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      559 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/analyze.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      451 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/apply_mode.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1339 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/argv_input.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3463 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/ascii.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5021 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/buffer_input.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      534 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/config.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      872 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/cstream_input.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1042 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/eol.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      440 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/eol_pair.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      961 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/file_input.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1513 2021-05-24 17:06:09.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/input_error.hpp
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-05-25 11:57:59.135690 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1439 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/action.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2869 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/action_input.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      548 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/alnum.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      538 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/alpha.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1664 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/any.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2750 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/apply.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2521 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/apply0.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1154 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/apply0_single.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1229 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/apply_single.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1626 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/at.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      862 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/bof.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      870 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/bol.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1573 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/bump_help.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1373 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/bump_impl.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1076 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/bytes.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1445 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/control.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1049 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/cr_crlf_eol.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      975 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/cr_eol.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1025 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/crlf_eol.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1389 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/cstream_reader.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1178 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/cstring_reader.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      843 2022-08-06 17:18:16.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/demangle.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1045 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/demangle_cxxabi.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      567 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/demangle_nop.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1376 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/demangle_sanitise.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1382 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/disable.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1003 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/discard.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      616 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/dusel_mode.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7228 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/duseltronik.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1377 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/enable.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1557 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/endian.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5410 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/endian_gcc.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2938 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/endian_win.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      884 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/eof.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      920 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/eol.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      974 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/eolf.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2518 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/file_mapper.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2011 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/file_opener.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3297 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/file_reader.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      751 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/has_apply.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      756 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/has_apply0.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      772 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/identifier.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3802 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/if_apply.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      580 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/if_must.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      634 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/if_must_else.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1862 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/if_then_else.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      723 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/input_pair.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3323 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/integer_sequence.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1159 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/istream_reader.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2766 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/istring.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1493 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/iterator.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1229 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/lf_crlf_eol.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      975 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/lf_eol.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      567 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/list.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      610 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/list_must.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      607 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/list_tail.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      697 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/list_tail_pad.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2409 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/marker.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2092 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/minus.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2484 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/must.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1652 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/not_at.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2429 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/one.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1648 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/opt.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      596 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/pad.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      609 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/pad_opt.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      837 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/peek_char.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2245 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/peek_utf16.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1800 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/peek_utf32.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2931 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/peek_utf8.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4180 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/pegtl_string.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1786 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/plus.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1598 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/raise.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1684 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/range.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2994 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/ranges.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2020 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/rep.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      641 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/rep_min.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2880 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/rep_min_max.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1500 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/rep_opt.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1172 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/require.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      568 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/result_on_found.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1910 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/rule_conjunction.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1393 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/rules.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2240 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/seq.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      903 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/skip_control.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2150 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/sor.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1494 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/star.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      594 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/star_must.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2769 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/state.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1736 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/string.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      955 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/trivial.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1972 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/try_catch_type.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2874 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/until.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      876 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/istream_input.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     9778 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/memory_input.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1913 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/mmap_input.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3897 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/normal.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      586 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/nothing.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1616 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/parse.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1106 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/parse_error.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1351 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/position.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2198 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/read_input.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      459 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/rewind_mode.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4942 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/rules.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1936 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/string_input.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      445 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/tracking_mode.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2832 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/utf16.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2832 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/utf32.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1553 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/utf8.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      602 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/version.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      793 2020-07-10 20:35:39.000000 gemmi-0.6.2/include/gemmi/third_party/tao/pegtl.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    19235 2022-04-23 21:43:35.000000 gemmi-0.6.2/include/gemmi/third_party/tinydir.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2797 2022-11-12 21:59:36.000000 gemmi-0.6.2/include/gemmi/to_chemcomp.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6242 2022-11-08 19:08:56.000000 gemmi-0.6.2/include/gemmi/to_cif.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     8862 2021-11-15 18:03:22.000000 gemmi-0.6.2/include/gemmi/to_json.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2421 2023-05-10 16:37:42.000000 gemmi-0.6.2/include/gemmi/to_mmcif.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      862 2023-03-04 21:20:57.000000 gemmi-0.6.2/include/gemmi/to_pdb.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    10769 2023-04-14 09:26:04.000000 gemmi-0.6.2/include/gemmi/topo.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    10282 2022-10-14 12:11:45.000000 gemmi-0.6.2/include/gemmi/twin.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    21692 2022-10-27 19:50:42.000000 gemmi-0.6.2/include/gemmi/unitcell.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2476 2021-04-17 18:25:34.000000 gemmi-0.6.2/include/gemmi/utf.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     8661 2023-02-09 23:24:19.000000 gemmi-0.6.2/include/gemmi/util.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      152 2023-05-25 11:04:11.000000 gemmi-0.6.2/include/gemmi/version.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    14985 2023-03-22 12:06:35.000000 gemmi-0.6.2/include/gemmi/xds_ascii.hpp
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-05-25 11:57:59.139690 gemmi-0.6.2/python/
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     4085 2022-09-12 16:59:12.000000 gemmi-0.6.2/python/align.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      327 2022-02-04 16:03:43.000000 gemmi-0.6.2/python/arrvec.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2447 2022-12-21 13:51:11.000000 gemmi-0.6.2/python/ccp4.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     8464 2023-02-16 00:04:33.000000 gemmi-0.6.2/python/chemcomp.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    17105 2022-12-21 13:17:59.000000 gemmi-0.6.2/python/cif.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3052 2023-03-17 18:03:23.000000 gemmi-0.6.2/python/common.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      195 2022-01-13 20:51:13.000000 gemmi-0.6.2/python/custom.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5307 2022-10-09 18:06:55.000000 gemmi-0.6.2/python/elem.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6254 2023-04-19 19:44:21.000000 gemmi-0.6.2/python/gemmi.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    12480 2022-10-26 15:34:30.000000 gemmi-0.6.2/python/grid.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16885 2023-04-19 15:30:51.000000 gemmi-0.6.2/python/hkl.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16973 2023-03-17 13:35:13.000000 gemmi-0.6.2/python/meta.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      745 2023-02-18 19:56:19.000000 gemmi-0.6.2/python/meta.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      571 2021-01-14 17:40:02.000000 gemmi-0.6.2/python/miller_a.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    26698 2023-05-20 12:30:09.000000 gemmi-0.6.2/python/mol.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5526 2023-03-27 16:12:52.000000 gemmi-0.6.2/python/monlib.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    14926 2023-03-14 19:10:45.000000 gemmi-0.6.2/python/mtz.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7676 2023-01-19 17:21:52.000000 gemmi-0.6.2/python/read.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     9555 2022-12-21 20:39:07.000000 gemmi-0.6.2/python/recgrid.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2005 2022-04-23 21:43:35.000000 gemmi-0.6.2/python/scaling.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6733 2023-04-13 08:18:16.000000 gemmi-0.6.2/python/search.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3819 2023-01-31 21:22:45.000000 gemmi-0.6.2/python/sf.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    12208 2023-03-10 16:44:25.000000 gemmi-0.6.2/python/sym.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7443 2023-05-17 19:25:39.000000 gemmi-0.6.2/python/topo.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      835 2022-04-23 21:43:35.000000 gemmi-0.6.2/python/tostr.hpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    17506 2023-05-01 08:51:11.000000 gemmi-0.6.2/python/unitcell.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     3795 2023-03-13 17:58:41.000000 gemmi-0.6.2/python/write.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      178 2023-05-25 11:57:59.143690 gemmi-0.6.2/setup.cfg
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7613 2023-04-16 18:07:18.000000 gemmi-0.6.2/setup.py
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-05-25 11:57:59.143690 gemmi-0.6.2/src/
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    15648 2023-05-03 18:51:43.000000 gemmi-0.6.2/src/assembly.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      927 2023-03-15 20:18:52.000000 gemmi-0.6.2/src/calculate.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    23784 2023-05-22 14:53:11.000000 gemmi-0.6.2/src/crd.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5709 2023-03-17 20:24:22.000000 gemmi-0.6.2/src/eig3.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    38280 2023-05-11 09:37:44.000000 gemmi-0.6.2/src/mmcif.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      697 2023-01-19 17:16:44.000000 gemmi-0.6.2/src/mmread_gz.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    20572 2023-04-13 00:17:52.000000 gemmi-0.6.2/src/monlib.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    11412 2023-05-06 20:48:55.000000 gemmi-0.6.2/src/mtz.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    37228 2023-05-17 19:25:39.000000 gemmi-0.6.2/src/mtz2cif.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    12734 2023-05-15 18:30:08.000000 gemmi-0.6.2/src/polyheur.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      899 2023-01-19 17:18:32.000000 gemmi-0.6.2/src/read_cif.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    24654 2023-04-15 12:45:01.000000 gemmi-0.6.2/src/resinfo.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    17837 2023-04-15 22:24:51.000000 gemmi-0.6.2/src/riding_h.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1864 2023-05-01 08:51:11.000000 gemmi-0.6.2/src/sprintf.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    54095 2023-05-15 13:42:05.000000 gemmi-0.6.2/src/to_mmcif.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    26716 2023-05-15 18:28:38.000000 gemmi-0.6.2/src/to_pdb.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    39755 2023-05-07 19:41:29.000000 gemmi-0.6.2/src/topo.cpp
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2219 2023-03-01 16:42:39.000000 gemmi-0.6.2/src/xds_ascii.cpp
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-05-25 11:57:59.143690 gemmi-0.6.2/third_party/
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    58248 2023-05-01 08:51:11.000000 gemmi-0.6.2/third_party/stb_sprintf.h
+drwxrwxr-x   0 wojdyr    (1000) wojdyr    (1000)        0 2023-05-25 11:57:59.143690 gemmi-0.6.2/third_party/zlib/
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     5204 2020-07-10 20:35:39.000000 gemmi-0.6.2/third_party/zlib/adler32.c
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    14053 2020-07-10 20:35:39.000000 gemmi-0.6.2/third_party/zlib/crc32.c
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    30562 2020-07-10 20:35:39.000000 gemmi-0.6.2/third_party/zlib/crc32.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6819 2020-07-10 20:35:39.000000 gemmi-0.6.2/third_party/zlib/gzguts.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16599 2020-07-10 20:35:39.000000 gemmi-0.6.2/third_party/zlib/gzlib.c
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    20428 2020-07-10 20:35:39.000000 gemmi-0.6.2/third_party/zlib/gzread.c
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    12978 2020-07-10 20:35:39.000000 gemmi-0.6.2/third_party/zlib/inffast.c
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)      427 2020-07-10 20:35:39.000000 gemmi-0.6.2/third_party/zlib/inffast.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6332 2020-07-10 20:35:39.000000 gemmi-0.6.2/third_party/zlib/inffixed.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    54800 2020-07-10 20:35:39.000000 gemmi-0.6.2/third_party/zlib/inflate.c
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     6618 2020-07-10 20:35:39.000000 gemmi-0.6.2/third_party/zlib/inflate.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    12999 2020-07-10 20:35:39.000000 gemmi-0.6.2/third_party/zlib/inftrees.c
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     2928 2020-07-10 20:35:39.000000 gemmi-0.6.2/third_party/zlib/inftrees.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     1031 2020-07-10 20:35:39.000000 gemmi-0.6.2/third_party/zlib/license
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    16298 2020-07-10 20:35:39.000000 gemmi-0.6.2/third_party/zlib/zconf.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)    96239 2020-07-10 20:35:39.000000 gemmi-0.6.2/third_party/zlib/zlib.h
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7304 2020-07-10 20:35:39.000000 gemmi-0.6.2/third_party/zlib/zutil.c
+-rw-rw-r--   0 wojdyr    (1000) wojdyr    (1000)     7127 2020-07-10 20:35:39.000000 gemmi-0.6.2/third_party/zlib/zutil.h
```

### Comparing `gemmi-0.6.1/LICENSE.txt` & `gemmi-0.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/PKG-INFO` & `gemmi-0.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemmi
-Version: 0.6.1
+Version: 0.6.2
 Summary: library for structural biology
 Home-page: https://project-gemmi.github.io/
 Author: Marcin Wojdyr
 Author-email: wojdyr@gmail.com
 License: MPL-2.0
 Keywords: structural bioinformatics,structural biology,crystallography,CIF,mmCIF,PDB,CCP4,MTZ
 Platform: UNKNOWN
```

### Comparing `gemmi-0.6.1/README.md` & `gemmi-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/examples/aafreq.py` & `gemmi-0.6.2/examples/aafreq.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,27 @@
 #!/usr/bin/env python
 # Check amino-acid frequency in the PDB database (or it's subset)
 # by reading meta-data from mmCIF files.
 
 from __future__ import print_function
 import sys
-import os
 from collections import Counter
-from gemmi import cif, CifWalk, expand_if_pdb_code
-
-def get_file_paths_from_args():
-    for arg in sys.argv[1:]:
-        if os.path.isdir(arg):
-            for path in CifWalk(arg):
-                yield path
-        else:
-            yield expand_if_pdb_code(arg)
+from gemmi import cif, CifWalk
 
 totals = Counter()
-for path in get_file_paths_from_args():
-    # read file (uncompressing on the fly) and get the only block
-    block = cif.read(path).sole_block()
-    # find table with the sequence
-    seq = block.find('_entity_poly_seq.', ['entity_id', 'mon_id'])
-    # convert table with chain types (protein/DNA/RNA) to dict
-    entity_types = dict(block.find('_entity_poly.', ['entity_id', 'type']))
-    # and count these monomers that correspond to a protein chain
-    aa_counter = Counter(row.str(1) for row in seq
-                         if 'polypeptide' in entity_types[row.str(0)])
-    totals += aa_counter
-    # print residue counts for each file
-    print(block.name, *('%s:%d' % c for c in aa_counter.most_common()))
+for arg in sys.argv[1:]:
+    for path in CifWalk(arg, try_pdbid='M'):
+        # read file (uncompressing on the fly) and get the only block
+        block = cif.read(path).sole_block()
+        # find table with the sequence
+        seq = block.find('_entity_poly_seq.', ['entity_id', 'mon_id'])
+        # convert table with chain types (protein/DNA/RNA) to dict
+        entity_types = dict(block.find('_entity_poly.', ['entity_id', 'type']))
+        # and count these monomers that correspond to a protein chain
+        aa_counter = Counter(row.str(1) for row in seq
+                             if 'polypeptide' in entity_types[row.str(0)])
+        totals += aa_counter
+        # print residue counts for each file
+        print(block.name, *('%s:%d' % c for c in aa_counter.most_common()))
 # finally, print the total counts as percentages
 f = 100.0 / sum(totals.values())
 print('TOTAL', *('%s:%.2f%%' % (m, c*f) for (m, c) in totals.most_common(20)))
```

### Comparing `gemmi-0.6.1/examples/ccd_gi.py` & `gemmi-0.6.2/examples/ccd_gi.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/examples/ccd_subgraph.py` & `gemmi-0.6.2/examples/ccd_subgraph.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/examples/cif_i_sigi.py` & `gemmi-0.6.2/examples/cif_i_sigi.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/examples/col_order.py` & `gemmi-0.6.2/examples/col_order.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/examples/from_json.py` & `gemmi-0.6.2/examples/from_json.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/examples/long_geom.py` & `gemmi-0.6.2/examples/long_geom.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/examples/map2mtz.py` & `gemmi-0.6.2/examples/map2mtz.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/examples/maskcheck.py` & `gemmi-0.6.2/examples/maskcheck.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/examples/maskdiff.py` & `gemmi-0.6.2/examples/maskdiff.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/examples/matthews.py` & `gemmi-0.6.2/examples/matthews.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/examples/merge_mtz_mmcif.py` & `gemmi-0.6.2/examples/merge_mtz_mmcif.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/examples/monomers.py` & `gemmi-0.6.2/examples/monomers.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/examples/mtrix_iso.py` & `gemmi-0.6.2/examples/mtrix_iso.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,12 +22,12 @@
                      '' if eps < 0.01 else 'NOT', eps, det)
         print('%s %3s %c    %s' % (st.name, ncs.id, 'NY'[ncs.given], status))
 
 def main():
     if len(sys.argv) < 2:
         sys.exit('Specify files, directories or PDB codes.')
     for arg in sys.argv[1:]:
-        for path in gemmi.CoorFileWalk(gemmi.expand_if_pdb_code(arg)):
+        for path in gemmi.CoorFileWalk(arg, try_pdbid='M'):
             check_mtrix_rot(path)
 
 if __name__ == '__main__':
     main()
```

### Comparing `gemmi-0.6.1/examples/mtz_i_sigi.py` & `gemmi-0.6.2/examples/mtz_i_sigi.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/examples/multiproc.py` & `gemmi-0.6.2/examples/multiproc.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/examples/patterson_slice.py` & `gemmi-0.6.2/examples/patterson_slice.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/examples/rama_gather.py` & `gemmi-0.6.2/examples/rama_gather.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/examples/rama_plot.py` & `gemmi-0.6.2/examples/rama_plot.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/examples/sub_ccd.py` & `gemmi-0.6.2/examples/sub_ccd.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/examples/weight.py` & `gemmi-0.6.2/examples/weight.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/gemmi.egg-info/PKG-INFO` & `gemmi-0.6.2/gemmi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemmi
-Version: 0.6.1
+Version: 0.6.2
 Summary: library for structural biology
 Home-page: https://project-gemmi.github.io/
 Author: Marcin Wojdyr
 Author-email: wojdyr@gmail.com
 License: MPL-2.0
 Keywords: structural bioinformatics,structural biology,crystallography,CIF,mmCIF,PDB,CCP4,MTZ
 Platform: UNKNOWN
```

### Comparing `gemmi-0.6.1/gemmi.egg-info/SOURCES.txt` & `gemmi-0.6.2/gemmi.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 examples/monomers.py
 examples/mtrix_iso.py
 examples/mtz_i_sigi.py
 examples/multiproc.py
 examples/patterson_slice.py
 examples/rama_gather.py
 examples/rama_plot.py
+examples/refln-stats.py
 examples/simple_search.py
 examples/sub_ccd.py
 examples/weight.py
 gemmi.egg-info/PKG-INFO
 gemmi.egg-info/SOURCES.txt
 gemmi.egg-info/dependency_links.txt
 gemmi.egg-info/not-zip-safe
@@ -89,14 +90,15 @@
 include/gemmi/monlib.hpp
 include/gemmi/mtz.hpp
 include/gemmi/mtz2cif.hpp
 include/gemmi/neighbor.hpp
 include/gemmi/neutron92.hpp
 include/gemmi/numb.hpp
 include/gemmi/pdb.hpp
+include/gemmi/pdb_id.hpp
 include/gemmi/pirfasta.hpp
 include/gemmi/polyheur.hpp
 include/gemmi/qcp.hpp
 include/gemmi/read_cif.hpp
 include/gemmi/read_map.hpp
 include/gemmi/recgrid.hpp
 include/gemmi/reciproc.hpp
@@ -127,15 +129,14 @@
 include/gemmi/utf.hpp
 include/gemmi/util.hpp
 include/gemmi/version.hpp
 include/gemmi/xds_ascii.hpp
 include/gemmi/third_party/fast_float.h
 include/gemmi/third_party/pocketfft_hdronly.h
 include/gemmi/third_party/sajson.h
-include/gemmi/third_party/stb_sprintf.h
 include/gemmi/third_party/tinydir.h
 include/gemmi/third_party/tao/LICENSE
 include/gemmi/third_party/tao/NOTES
 include/gemmi/third_party/tao/pegtl.hpp
 include/gemmi/third_party/tao/pegtl/analyze.hpp
 include/gemmi/third_party/tao/pegtl/apply_mode.hpp
 include/gemmi/third_party/tao/pegtl/argv_input.hpp
@@ -305,14 +306,15 @@
 src/resinfo.cpp
 src/riding_h.cpp
 src/sprintf.cpp
 src/to_mmcif.cpp
 src/to_pdb.cpp
 src/topo.cpp
 src/xds_ascii.cpp
+third_party/stb_sprintf.h
 third_party/zlib/adler32.c
 third_party/zlib/crc32.c
 third_party/zlib/crc32.h
 third_party/zlib/gzguts.h
 third_party/zlib/gzlib.c
 third_party/zlib/gzread.c
 third_party/zlib/inffast.c
```

### Comparing `gemmi-0.6.1/include/gemmi/addends.hpp` & `gemmi-0.6.2/include/gemmi/addends.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/align.hpp` & `gemmi-0.6.2/include/gemmi/align.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/assembly.hpp` & `gemmi-0.6.2/include/gemmi/assembly.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/asudata.hpp` & `gemmi-0.6.2/include/gemmi/asudata.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/asumask.hpp` & `gemmi-0.6.2/include/gemmi/asumask.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 // Copyright 2022 Global Phasing Ltd.
 //
 // AsuBrick and MaskedGrid that is used primarily as direct-space asu mask.
 
 #ifndef GEMMI_ASUMASK_HPP_
 #define GEMMI_ASUMASK_HPP_
 
+#include <cstdint>
+
 #include "grid.hpp"
 
 namespace gemmi {
 
 struct AsuBrick {
   // The brick is 0<=x<=size[0]/24, 0<=y<=size[1]/24, 0<=z<=size[2]/24
   static constexpr int denom = 24;
```

### Comparing `gemmi-0.6.1/include/gemmi/atof.hpp` & `gemmi-0.6.2/include/gemmi/atof.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/atox.hpp` & `gemmi-0.6.2/include/gemmi/atox.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 // numbers from files). They don't set errno, don't signal overflow and
 // underflow. Due to the limited scope these functions tend to be faster
 // than the standard-library ones.
 
 #ifndef GEMMI_ATOX_HPP_
 #define GEMMI_ATOX_HPP_
 
+#include <cstdint>
 #include <stdexcept>  // for invalid_argument
 #include <string>
 
 namespace gemmi {
 
 // equivalent of std::isspace for C locale (no handling of EOF)
 inline bool is_space(char c) {
```

### Comparing `gemmi-0.6.1/include/gemmi/bessel.hpp` & `gemmi-0.6.2/include/gemmi/bessel.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/binner.hpp` & `gemmi-0.6.2/include/gemmi/binner.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/blob.hpp` & `gemmi-0.6.2/include/gemmi/blob.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/bond_idx.hpp` & `gemmi-0.6.2/include/gemmi/bond_idx.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/c4322.hpp` & `gemmi-0.6.2/include/gemmi/c4322.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/calculate.hpp` & `gemmi-0.6.2/include/gemmi/calculate.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/ccp4.hpp` & `gemmi-0.6.2/include/gemmi/ccp4.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/cellred.hpp` & `gemmi-0.6.2/include/gemmi/cellred.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/chemcomp.hpp` & `gemmi-0.6.2/include/gemmi/chemcomp.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/chemcomp_xyz.hpp` & `gemmi-0.6.2/include/gemmi/chemcomp_xyz.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/cif.hpp` & `gemmi-0.6.2/include/gemmi/cif.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -191,16 +191,18 @@
 //  }
 //};
 
 template<> struct Action<rules::datablockname> {
   template<typename Input> static void apply(const Input& in, Document& out) {
     out.blocks.emplace_back(in.string());
     Block& block = out.blocks.back();
-    if (block.name.empty()) // RELION's case
-      block.name += '#';
+    // Empty block name (just data_ ) is not STAR/CIF conformant,
+    // but it's written by RELION and buccaneer; we must support it.
+    if (block.name.empty())
+      block.name += ' ';
     out.items_ = &block.items;
   }
 };
 template<> struct Action<rules::str_global> {
   template<typename Input> static void apply(const Input&, Document& out) {
     out.blocks.emplace_back();
     out.items_ = &out.blocks.back().items;
```

### Comparing `gemmi-0.6.1/include/gemmi/cif2mtz.hpp` & `gemmi-0.6.2/include/gemmi/cif2mtz.hpp`

 * *Files 26% similar despite different names*

```diff
@@ -16,46 +16,168 @@
 #include "numb.hpp"     // for as_number
 #include "refln.hpp"    // for ReflnBlock
 #include "version.hpp"  // for GEMMI_VERSION
 
 namespace gemmi {
 
 template<typename DataProxy>
-DataType check_data_type_under_symmetry(const DataProxy& proxy) {
+std::pair<DataType, size_t> check_data_type_under_symmetry(const DataProxy& proxy) {
   const SpaceGroup* sg = proxy.spacegroup();
   if (!sg)
-    return DataType::Unknown;
+    return {DataType::Unknown, 0};
   std::unordered_map<Op::Miller, int, MillerHash> seen;
   ReciprocalAsu asu(sg);
   GroupOps gops = sg->operations();
   bool centric = gops.is_centrosymmetric();
   DataType data_type = DataType::Mean;
   for (size_t i = 0; i < proxy.size(); i += proxy.stride()) {
-    auto hkl_isym = asu.to_asu(proxy.get_hkl(i), gops);
-    int sign = hkl_isym.second % 2 + 1;  // 2=positive, 1=negative
-    auto r = seen.emplace(hkl_isym.first, sign);
-    if (!r.second) {
-      if ((r.first->second & sign) != 0 || centric)
-        return DataType::Unmerged;
-      r.first->second |= sign;
-      data_type = DataType::Anomalous;
+    auto hkl_sign = asu.to_asu_sign(proxy.get_hkl(i), gops);
+    int sign = hkl_sign.second ? 2 : 1;  // 2=positive, 1=negative
+    auto r = seen.emplace(hkl_sign.first, sign);
+    if (data_type != DataType::Unmerged && !r.second) {
+      if ((r.first->second & sign) != 0 || centric) {
+        data_type = DataType::Unmerged;
+      } else {
+        r.first->second |= sign;
+        data_type = DataType::Anomalous;
+      }
+    }
+  }
+  return {data_type, seen.size()};
+}
+
+// "Old-style" anomalous or unmerged data is expected to have only these tags.
+inline bool possible_old_style(const ReflnBlock& rb, DataType data_type) {
+  if (rb.refln_loop == nullptr)
+    return false;
+  for (const std::string& tag : rb.refln_loop->tags) {
+    if (tag.size() < 7 + 6)
+      return false;
+    int tag_id = ialpha4_id(tag.c_str() + 7);
+    if (tag_id != ialpha4_id("inde") &&  // index_[hkl]
+        tag_id != ialpha4_id("wave") &&  // wavelength_id
+        tag_id != ialpha4_id("crys") &&  // crystal_id
+        tag_id != ialpha4_id("scal") &&  // scale_group_code
+        tag_id != ialpha4_id("stat") &&  // status
+        tag_id != ialpha4_id("inte") &&  // intensity_meas, intensity_sigma
+        (data_type == DataType::Unmerged ||
+         (tag_id != ialpha4_id("F_me") &&  // F_meas_au, F_meas_sigma_au
+          tag != "_refln.pdbx_r_free_flag")))
+      return false;
+  }
+  return true;
+}
+
+
+/// Before _refln.pdbx_F_plus/minus was introduced, anomalous data was
+/// stored as two F_meas_au reflections, say (1,1,3) and (-1,-1,-3).
+/// This function transcribes it to how the anomalous data is stored
+/// in PDBx/mmCIF nowadays:
+///  _refln.F_meas_au -> pdbx_F_plus / pdbx_F_minus,
+///  _refln.F_meas_sigma_au -> pdbx_F_plus_sigma / pdbx_F_minus_sigma.
+///  _refln.intensity_{meas,sigma} -> _refln.pdbx_F_plus{,_sigma} / ...
+inline cif::Loop transcript_old_anomalous_to_standard(const cif::Loop& loop,
+                                                      const SpaceGroup* sg) {
+  std::vector<int> positions;
+  positions.reserve(13);  // usually less, but it doesn't matter
+  for (const char* tag : {"_refln.index_h", "_refln.index_k", "_refln.index_l"}) {
+    int pos = loop.find_tag_lc(tag);
+    if (pos == -1)
+      fail("while reading old anomalous: _refln.index_{h,k,l} not found");
+    positions.push_back(pos);
+  }
+  for (const char* tag : {"_refln.status", "_refln.pdbx_r_free_flag"}) {
+    int pos = loop.find_tag_lc(tag);
+    if (pos != -1)
+      positions.push_back(pos);
+  }
+
+  cif::Loop ret;
+  ret.tags.reserve(positions.size());
+  for (int p : positions)
+    ret.tags.push_back(loop.tags[p]);
+  const char* old_labels[2][2] = {
+    {"_refln.F_meas_au", "_refln.F_meas_sigma_au"},
+    {"_refln.intensity_meas", "_refln.intensity_sigma"}
+  };
+  const char* new_labels[2][4] = {
+    {"_refln.pdbx_F_plus", "_refln.pdbx_F_plus_sigma",
+     "_refln.pdbx_F_minus", "_refln.pdbx_F_minus_sigma"},
+    {"_refln.pdbx_I_plus", "_refln.pdbx_I_plus_sigma",
+     "_refln.pdbx_I_minus", "_refln.pdbx_I_minus_sigma"}
+  };
+  size_t common_tags = positions.size();
+  for (int n = 0; n < 2; ++n) {
+    int idx = loop.find_tag(old_labels[n][0]);
+    if (idx >= 0 && idx+1 < (int)loop.width() && loop.tags[idx+1] == old_labels[n][1]) {
+      positions.insert(positions.end(), {idx, idx+1, idx, idx+1});
+      ret.tags.insert(ret.tags.end(), new_labels[n], new_labels[n] + 4);
     }
   }
-  return data_type;
+  if (common_tags == positions.size())
+    fail("while reading old anomalous: _refln has neither F_meas_au nor intensity_meas");
+
+  ret.values.reserve(loop.length() * ret.width());  // upper bound
+  std::unordered_map<Miller, std::string*, MillerHash> seen;
+  if (!sg)
+    sg = &get_spacegroup_p1();
+  ReciprocalAsu asu(sg);
+  GroupOps gops = sg->operations();
+  for (size_t i = 0; i < loop.values.size(); i += loop.width()) {
+    const std::string* row = &loop.values[i];
+    Miller hkl;
+    for (size_t j = 0; j < 3; ++j)
+      hkl[j] = cif::as_int(row[positions[j]]);
+    auto hkl_sign = asu.to_asu_sign(hkl, gops);
+    // pointers don't change, .reserve() above prevents re-allocations
+    std::string* new_row = ret.values.data() + ret.values.size();
+    auto r = seen.emplace(hkl_sign.first, new_row);
+    bool sign = hkl_sign.second;
+    if (r.second) {  // adding a new row
+      for (int p : positions)
+        ret.values.push_back(row[p]);
+      // Don't move hkl to asu here, only change the sign if F- is before F+.
+      if (!sign)  // negative sign
+        for (int j = 0; j < 3; ++j)
+          new_row[j] = std::to_string(-hkl[j]);
+      size_t first_absent = common_tags + (sign ? 2 : 0);
+      for (size_t j = first_absent; j < ret.width(); j += 4) {
+        new_row[j] = ".";
+        new_row[j+1] = ".";
+      }
+    } else {  // modifying existing row
+      std::string* modified_row = r.first->second;
+      if (sign)  // positive sign - this hkl might be better
+        for (int j = 0; j < 3; ++j)
+          modified_row[j] = row[positions[j]];
+      // if a status or free flag value differs, set it to null
+      for (size_t j = 3; j < common_tags; ++j)
+        if (modified_row[j] != row[positions[j]])
+          modified_row[j] = ".";
+      for (size_t j = common_tags + (sign ? 0 : 2); j < ret.width(); j += 4) {
+        modified_row[j] = row[positions[j]];
+        modified_row[j+1] = row[positions[j+1]];
+      }
+    }
+  }
+
+  return ret;
 }
 
 
 struct CifToMtz {
   // Alternative mmCIF tags for the same MTZ label should be consecutive
   static const char** default_spec(bool for_merged) {
     static const char* merged[] = {
       "pdbx_r_free_flag FreeR_flag I 0",
       "status FreeR_flag I 0 o=1,f=0",
       "intensity_meas IMEAN J 1",
+      "F_squared_meas IMEAN J 1",
       "intensity_sigma SIGIMEAN Q 1",
+      "F_squared_sigma SIGIMEAN Q 1",
       "pdbx_I_plus I(+) K 1",
       "pdbx_I_plus_sigma SIGI(+) M 1",
       "pdbx_I_minus I(-) K 1",
       "pdbx_I_minus_sigma SIGI(-) M 1",
       "F_meas FP F 1",
       "F_meas_au FP F 1",
       "F_meas_sigma SIGFP Q 1",
@@ -401,20 +523,44 @@
           if (std::isnan(mtz.data[k]))
             out << "Value #" << i + indices[j] << " in the loop is not a number: "
                 << v << '\n';
         }
         ++k;
       }
     }
-    if (mtz.is_merged()) {
-      gemmi::DataType type = check_data_type_under_symmetry(gemmi::MtzDataProxy{mtz});
-      if (type == gemmi::DataType::Anomalous)
-        out << "WARNING: CIF block " << rb.block.name << " has old-style anomalous data.\n";
-      else if (type == gemmi::DataType::Unmerged)
-        out << "WARNING: CIF block " << rb.block.name << " has old-style unmerged data.\n";
+    return mtz;
+  }
+
+  Mtz auto_convert_block_to_mtz(ReflnBlock& rb, std::ostream& out, char mode) const {
+    if (mode == 'f' && possible_old_style(rb, DataType::Anomalous))
+      *rb.refln_loop = transcript_old_anomalous_to_standard(*rb.refln_loop, rb.spacegroup);
+    Mtz mtz = convert_block_to_mtz(rb, out);
+    if (mtz.is_merged() && mode == 'a') {
+      auto type_unique = check_data_type_under_symmetry(MtzDataProxy{mtz});
+      if (type_unique.first == DataType::Anomalous) {
+        if (possible_old_style(rb, DataType::Anomalous)) {
+          out << "NOTE: data in " << rb.block.name
+              << " is read as \"old-style\" anomalous (" << rb.refln_loop->length()
+              << " -> " << type_unique.second << " rows).\n";
+          *rb.refln_loop = transcript_old_anomalous_to_standard(*rb.refln_loop,
+                                                                rb.spacegroup);
+          // this is rare, so it's OK to run the conversion twice
+          mtz = convert_block_to_mtz(rb, out);
+        } else {
+          out << "WARNING: in " << rb.block.name << ", out of "
+              << rb.refln_loop->length() << " HKLs, only " << type_unique.second
+              << " are unique under symmetry; the rest are equivalent to Friedel mates\n";
+        }
+      } else if (type_unique.first == DataType::Unmerged) {
+        out << "WARNING: in " << rb.block.name << ", out of "
+            << rb.refln_loop->length() << " HKLs, only " << type_unique.second
+            << " are unique under symmetry\n";
+        if (possible_old_style(rb, gemmi::DataType::Unmerged))
+          out << "Possibly unmerged data - you may use option --refln-to=unmerged\n";
+      }
     }
     return mtz;
   }
 
 private:
   static float status_to_freeflag(const std::string& str) {
     char c = str[0];
```

### Comparing `gemmi-0.6.1/include/gemmi/cifdoc.hpp` & `gemmi-0.6.2/include/gemmi/cifdoc.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/contact.hpp` & `gemmi-0.6.2/include/gemmi/contact.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/crd.hpp` & `gemmi-0.6.2/include/gemmi/crd.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/dencalc.hpp` & `gemmi-0.6.2/include/gemmi/dencalc.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/dirwalk.hpp` & `gemmi-0.6.2/include/gemmi/dirwalk.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 #if defined(_MSC_VER) && !defined(NOMINMAX)
 # define NOMINMAX
 #endif
 #include "third_party/tinydir.h"
 
 #include "util.hpp"  // for giends_with
 #include "fail.hpp"  // for sys_fail
+#include "pdb_id.hpp" // for is_pdb_code, expand_pdb_code_to_path
 #if defined(_WIN32) && defined(_UNICODE)
  #include "utf.hpp"
 #endif
 
 namespace gemmi {
 
 inline std::string as_utf8(const _tinydir_char_t* path) {
@@ -119,31 +120,41 @@
 struct IsMatchingFile {
   bool check(const std::string& filename) const {
     return glob_match(pattern, filename);
   }
   std::string pattern;
 };
 
+inline int utf8_tinydir_file_open(tinydir_file* file, const char* path) {
+#if defined(_WIN32) && defined(_UNICODE)
+  return tinydir_file_open(file, UTF8_to_wchar(path).c_str());
+#else
+  return tinydir_file_open(file, path);
+#endif
+}
+
 } // namespace impl
 
 
 template<bool FileOnly=true, typename Filter=impl::IsAnyFile>
 class DirWalk {
 public:
-  explicit DirWalk(const char* path) {
-#if defined(_WIN32) && defined(_UNICODE)
-    std::wstring str = UTF8_to_wchar(path);
-    const _tinydir_char_t* xpath = str.c_str();
-#else
-    const char* xpath = path;
-#endif
-    if (tinydir_file_open(&top_, xpath) == -1)
-      sys_fail("Cannot open " + std::string(path));
+  explicit DirWalk(const char* path, char try_pdbid='\0') {
+    if (impl::utf8_tinydir_file_open(&top_, path) != -1)
+      return;
+    if (try_pdbid != '\0' && is_pdb_code(path)) {
+      std::string epath = expand_pdb_code_to_path(path, try_pdbid, true);
+      if (impl::utf8_tinydir_file_open(&top_, epath.c_str()) != -1)
+        return;
+      sys_fail("Cannot open " + epath);
+    }
+    sys_fail("Cannot open " + std::string(path));
   }
-  explicit DirWalk(const std::string& path) : DirWalk(path.c_str()) {}
+  explicit DirWalk(const std::string& path, char try_pdbid='\0')
+    : DirWalk(path.c_str(), try_pdbid) {}
   ~DirWalk() {
     for (auto& d : dirs_)
       tinydir_close(&d.second);
   }
   void push_dir(size_t cur_pos, const _tinydir_char_t* path) {
     dirs_.emplace_back();
     dirs_.back().first = cur_pos;
```

### Comparing `gemmi-0.6.1/include/gemmi/elem.hpp` & `gemmi-0.6.2/include/gemmi/elem.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/enumstr.hpp` & `gemmi-0.6.2/include/gemmi/enumstr.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/fail.hpp` & `gemmi-0.6.2/include/gemmi/fail.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,15 @@
 #  else
 #   define GEMMI_DLL __declspec(dllimport)
 #  endif  // GEMMI_BUILD
 # else
 #  define GEMMI_DLL
 # endif  // GEMMI_SHARED
 #else
-# define GEMMI_DLL
-//# define GEMMI_DLL __attribute__((visibility("default")))
+# define GEMMI_DLL __attribute__((visibility("default")))
 #endif
 
 namespace gemmi {
 
 [[noreturn]]
 inline void fail(const std::string& msg) { throw std::runtime_error(msg); }
```

### Comparing `gemmi-0.6.1/include/gemmi/floodfill.hpp` & `gemmi-0.6.2/include/gemmi/floodfill.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/formfact.hpp` & `gemmi-0.6.2/include/gemmi/formfact.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/fourier.hpp` & `gemmi-0.6.2/include/gemmi/fourier.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/fprime.hpp` & `gemmi-0.6.2/include/gemmi/fprime.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/fstream.hpp` & `gemmi-0.6.2/include/gemmi/fstream.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/grid.hpp` & `gemmi-0.6.2/include/gemmi/grid.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/gz.hpp` & `gemmi-0.6.2/include/gemmi/gz.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/input.hpp` & `gemmi-0.6.2/include/gemmi/input.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/interop.hpp` & `gemmi-0.6.2/include/gemmi/interop.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/it92.hpp` & `gemmi-0.6.2/include/gemmi/it92.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/iterator.hpp` & `gemmi-0.6.2/include/gemmi/iterator.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/json.hpp` & `gemmi-0.6.2/include/gemmi/json.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/levmar.hpp` & `gemmi-0.6.2/include/gemmi/levmar.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/linkhunt.hpp` & `gemmi-0.6.2/include/gemmi/linkhunt.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/math.hpp` & `gemmi-0.6.2/include/gemmi/math.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/merge.hpp` & `gemmi-0.6.2/include/gemmi/merge.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -247,22 +247,18 @@
             refl.isign = 1;  // since it's in asu - I+ or centric
           // when reading asu hkl from MTZ file - count centrics always as I+
           else if (refl.isign == -1 && gops.is_reflection_centric(refl.hkl))
             refl.isign = 1;
         }
         continue;
       }
-      auto hkl_isym = asu.to_asu(refl.hkl, gops);
-      refl.hkl = hkl_isym.first;
-      if (!merged) {
-        if (gops.is_reflection_centric(refl.hkl))
-          refl.isign = 1;
-        else
-          refl.isign = (hkl_isym.second % 2 == 0 ? -1 : 1);
-      }
+      bool sign;
+      std::tie(refl.hkl, sign) = asu.to_asu_sign(refl.hkl, gops);
+      if (!merged)
+        refl.isign = sign ? 1 : -1;
     }
   }
 
   void read_unmerged_intensities_from_mtz(const Mtz& mtz) {
     if (mtz.batches.empty())
       fail("expected unmerged file");
     const Mtz::Column* isym_col = mtz.column_with_label("M/ISYM");
```

### Comparing `gemmi-0.6.1/include/gemmi/metadata.hpp` & `gemmi-0.6.2/include/gemmi/metadata.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -271,14 +271,22 @@
   std::string model_str;
   // mmCIF has (unused by the PDB) tag _struct_mon_prot_cis.label_alt_id
   // that enables defining CIS link per conformation.
   char only_altloc = '\0';
   double reported_angle = NAN;
 };
 
+struct ModRes {
+  std::string chain_name;
+  ResidueId res_id;
+  std::string parent_comp_id;
+  std::string mod_id;  // non-standard extension used in Refmac
+  std::string details;
+};
+
 // Secondary structure. PDBx/mmCIF stores helices and sheets separately.
 
 // mmCIF spec defines 32 possible values for _struct_conf.conf_type_id -
 // "the type of the conformation of the backbone of the polymer (whether
 // protein or nucleic acid)". But as of 2019 only HELX_P is used (not counting
 // TURN_P that occurs in only 6 entries). The actual helix type is given
 // by numeric value of _struct_conf.pdbx_PDB_helix_class, which corresponds
```

### Comparing `gemmi-0.6.1/include/gemmi/mmcif.hpp` & `gemmi-0.6.2/include/gemmi/mmcif.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/mmcif_impl.hpp` & `gemmi-0.6.2/include/gemmi/mmcif_impl.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/mmdb.hpp` & `gemmi-0.6.2/include/gemmi/mmdb.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/mmread.hpp` & `gemmi-0.6.2/include/gemmi/mmread.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/mmread_gz.hpp` & `gemmi-0.6.2/include/gemmi/mmread_gz.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/model.hpp` & `gemmi-0.6.2/include/gemmi/model.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,23 @@
 
 /// File format of a macromolecular model. When passed to read_structure():
 /// Unknown = guess format from the extension,
 /// Detect = guess format from the content.
 enum class CoorFormat { Unknown, Detect, Pdb, Mmcif, Mmjson, ChemComp };
 
 /// corresponds to _atom_site.calc_flag in mmCIF
-enum class CalcFlag : signed char { NotSet=0, Determined, Calculated, Dummy };
+enum class CalcFlag : signed char {
+  // NoHydrogen is the same as NotSet; it's used internally to mark atoms
+  // which should not have riding hydrogens.
+  // NB: add_cif_atoms() relies on this order.
+  NotSet=0, NoHydrogen, Determined, Calculated, Dummy
+};
+
+/// helper type used for Structure::shortened_ccd_codes
+struct OldToNew { std::string old, new_; };
 
 /// options affecting how pdb file is read
 struct PdbReadOptions {
   int max_line_length = 0;
   bool split_chain_on_ter = false;
   bool skip_remarks = false;
 };
@@ -850,31 +858,34 @@
   UnitCell cell;
   std::string spacegroup_hm;  // usually pdb symbol, cf. SpaceGroup::pdb_name()
   std::vector<Model> models;
   std::vector<NcsOp> ncs;
   std::vector<Entity> entities;
   std::vector<Connection> connections;
   std::vector<CisPep> cispeps;
+  std::vector<ModRes> mod_residues;
   std::vector<Helix> helices;
   std::vector<Sheet> sheets;
   std::vector<Assembly> assemblies;
   Metadata meta;
 
   CoorFormat input_format = CoorFormat::Unknown;
   bool has_d_fraction = false;  // uses Refmac's ccp4_deuterium_fraction
 
-  // Store ORIGXn / _database_PDB_matrix.origx*
+  /// Store ORIGXn / _database_PDB_matrix.origx*
   bool has_origx = false;
   Transform origx;
 
-  // Minimal metadata with keys being mmcif tags: _entry.id, _cell.Z_PDB, ...
+  /// Minimal metadata with keys being mmcif tags: _entry.id, _cell.Z_PDB, ...
   std::map<std::string, std::string> info;
-  // original REMARK records stored if the file was read from the PDB format
+  /// Mapping of long (4+) CCD codes (residue names) to PDB-compatible ones
+  std::vector<OldToNew> shortened_ccd_codes;
+  /// original REMARK records stored if the file was read from the PDB format
   std::vector<std::string> raw_remarks;
-  // simplistic resolution value from/for REMARK 2
+  /// simplistic resolution value from/for REMARK 2
   double resolution = 0;
 
   const SpaceGroup* find_spacegroup() const {
     return find_spacegroup_by_name(spacegroup_hm, cell.alpha, cell.gamma);
   }
 
   const std::string& get_info(const std::string& tag) const {
```

### Comparing `gemmi-0.6.1/include/gemmi/modify.hpp` & `gemmi-0.6.2/include/gemmi/modify.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -100,54 +100,43 @@
     cra.atom->serial = ++serial;
 }
 inline void assign_serial_numbers(Structure& st) {
   for (Model& model : st.models)
     assign_serial_numbers(model);
 }
 
-/// Hydrogens modelled as H/D mixture (altlocs H and D with the same position
-/// and ADP, but with refined fraction of D), it can be stored in a file either
-/// as two atoms (H and D) or, using CCP4/Refmac extension, as H atoms with
-/// the ccp4_deuterium_fraction parameter.
-/// This function switches fraction -> altlocs
-inline void expand_hd_mixture(Structure& st) {
-  if (!st.has_d_fraction)
-    return;
-  for (Model& model : st.models)
-    for (Chain& chain : model.chains)
-      for (Residue& res : chain.residues)
-        for (size_t i = res.atoms.size(); i-- != 0; ) {
-          Atom& atom = res.atoms[i];
-          float d_fraction = atom.fraction;
-          if (atom.element == El::H && d_fraction > 0) {
-            if (d_fraction >= 1) {
-              atom.element = El::D;
-              if (atom.name[0] == 'H')
-                atom.name[0] = 'D';
-            } else {
-              int alt_offset = atom.altloc;
-              if (alt_offset) {
-                alt_offset -= 'A';
-                // we don't expect 4+ altlocs - ignore such cases
-                if (alt_offset < 0 || alt_offset >= 3)
-                  continue;
-              }
-              atom.altloc = 'A' + alt_offset;
-              float d_occ = atom.occ * d_fraction;
-              atom.occ *= (1 - d_fraction);
-              auto deut = res.atoms.insert(res.atoms.begin() + i + 1, atom);
-              deut->altloc = 'D' + alt_offset;
-              deut->element = El::D;
-              deut->occ = d_occ;
-              if (deut->name[0] == 'H')
-                deut->name[0] = 'D';
-            }
-          }
+inline void replace_d_fraction_with_altlocs(Residue& res) {
+  for (size_t i = res.atoms.size(); i-- != 0; ) {
+    Atom& atom = res.atoms[i];
+    float d_fraction = atom.fraction;
+    if (atom.element == El::H && d_fraction > 0) {
+      if (d_fraction >= 1) {
+        atom.element = El::D;
+        if (atom.name[0] == 'H')
+          atom.name[0] = 'D';
+      } else {
+        int alt_offset = atom.altloc;
+        if (alt_offset) {
+          alt_offset -= 'A';
+          // we don't expect 4+ altlocs - ignore such cases
+          if (alt_offset < 0 || alt_offset >= 3)
+            continue;
         }
-  st.has_d_fraction = false;
+        atom.altloc = 'A' + alt_offset;
+        float d_occ = atom.occ * d_fraction;
+        atom.occ *= (1 - d_fraction);
+        auto deut = res.atoms.insert(res.atoms.begin() + i + 1, atom);
+        deut->altloc = 'D' + alt_offset;
+        deut->element = El::D;
+        deut->occ = d_occ;
+        if (deut->name[0] == 'H')
+          deut->name[0] = 'D';
+      }
+    }
+  }
 }
 
 inline bool replace_deuterium_with_fraction(Residue& res) {
   bool found = false;
   for (auto d = res.atoms.end(); d-- != res.atoms.begin(); )
     if (d->element == El::D) {
       found = true;
@@ -173,20 +162,29 @@
         // Atom name is left unchanged. prepare_topology() first calls this
         // function and then conditionally changes the name (Dxx -> Hxx).
       }
     }
   return found;
 }
 
-/// Switch H/D altlocs at the same position to H w/ ccp4_deuterium_fraction.
-inline void collapse_hd_mixture(Structure& st) {
-  if (st.has_d_fraction)
+/// Hydrogens modelled as H/D mixture (altlocs H and D with the same position
+/// and ADP, but with refined fraction of D), it can be stored in mmCIF either
+/// as two atoms (H and D) or, using CCP4/Refmac extension, as H atoms with
+/// the ccp4_deuterium_fraction parameter.
+/// This function switches fraction <-> altlocs
+inline void store_deuterium_as_fraction(Structure& st, bool store_fraction) {
+  if (st.has_d_fraction == store_fraction)
     return;
+  st.has_d_fraction = false;
   for (Model& model : st.models)
     for (Chain& chain : model.chains)
       for (Residue& res : chain.residues)
-        if (replace_deuterium_with_fraction(res))
-          st.has_d_fraction = true;
+        if (store_fraction) {
+          if (replace_deuterium_with_fraction(res))
+            st.has_d_fraction = true;
+        } else {
+          replace_d_fraction_with_altlocs(res);
+        }
 }
 
 } // namespace gemmi
 #endif
```

### Comparing `gemmi-0.6.1/include/gemmi/monlib.hpp` & `gemmi-0.6.2/include/gemmi/monlib.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,17 @@
   match_link(const Residue& res1, const std::string& atom1, char alt1,
              const Residue& res2, const std::string& atom2, char alt2,
              double min_bond_sq=0) const {
     const ChemLink* best_link = nullptr;
     bool inverted = false;
     const ChemComp::Aliasing* aliasing1 = nullptr;
     const ChemComp::Aliasing* aliasing2 = nullptr;
-    int best_score = -1;
+    const ChemComp::Aliasing* aliasing1_final = nullptr;
+    const ChemComp::Aliasing* aliasing2_final = nullptr;
+    int best_score = -1000;
     for (auto& ml : links) {
       const ChemLink& link = ml.second;
       if (link.rt.bonds.empty() || starts_with(link.name, "auto-"))
         continue;
       // for now we don't have link definitions with >1 bonds
       const Restraints::Bond& bond = link.rt.bonds[0];
       if (sq(bond.value) < min_bond_sq)
@@ -164,30 +166,34 @@
           link_side_matches_residue(link.side2, res2.name, &aliasing2) &&
           atom_match_with_alias(bond.id1.atom, atom1, aliasing1) &&
           atom_match_with_alias(bond.id2.atom, atom2, aliasing2)) {
         int score = link.calculate_score(res1, &res2, alt1, alt2, aliasing1, aliasing2);
         if (score > best_score) {
           best_link = &link;
           best_score = score;
+          aliasing1_final = aliasing1;
+          aliasing2_final = aliasing2;
           inverted = false;
         }
       }
       if (link_side_matches_residue(link.side1, res2.name, &aliasing2) &&
           link_side_matches_residue(link.side2, res1.name, &aliasing1) &&
           atom_match_with_alias(bond.id1.atom, atom2, aliasing2) &&
           atom_match_with_alias(bond.id2.atom, atom1, aliasing1)) {
         int score = link.calculate_score(res2, &res1, alt2, alt1, aliasing2, aliasing1);
         if (score > best_score) {
           best_link = &link;
           best_score = score;
+          aliasing1_final = aliasing1;
+          aliasing2_final = aliasing2;
           inverted = true;
         }
       }
     }
-    return std::make_tuple(best_link, inverted, aliasing1, aliasing2);
+    return std::make_tuple(best_link, inverted, aliasing1_final, aliasing2_final);
   }
 
   void add_monomer_if_present(const cif::Block& block) {
     if (block.has_tag("_chem_comp_atom.atom_id")) {
       ChemComp cc = make_chemcomp_from_block(block);
       if (cc.group == ChemComp::Group::Null) {
         auto it = cc_groups.find(cc.name);
```

### Comparing `gemmi-0.6.1/include/gemmi/mtz.hpp` & `gemmi-0.6.2/include/gemmi/mtz.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/mtz2cif.hpp` & `gemmi-0.6.2/include/gemmi/mtz2cif.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/neighbor.hpp` & `gemmi-0.6.2/include/gemmi/neighbor.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/neutron92.hpp` & `gemmi-0.6.2/include/gemmi/neutron92.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/numb.hpp` & `gemmi-0.6.2/include/gemmi/numb.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/pdb.hpp` & `gemmi-0.6.2/include/gemmi/pdb.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -407,14 +407,35 @@
       ent.entity_type = EntityType::Polymer;
       for (int i = 19; i < 68; i += 4) {
         std::string res_name = read_string(line+i, 3);
         if (!res_name.empty())
           ent.full_sequence.emplace_back(res_name);
       }
 
+    } else if (is_record_type(line, "MODRES")) {
+      ModRes modres;
+      modres.chain_name = read_string(line + 15, 2);
+      modres.res_id = read_res_id(line + 18, line + 12);
+      modres.parent_comp_id = read_string(line + 24, 3);
+      if (len >= 30)
+        // this field is named comment in PDB spec, but details in mmCIF
+        modres.details = read_string(line + 29, 41);
+      // Refmac's extension: 73-80 mod_id
+      // Check for spaces to make sure it's not an overflowed comment
+      if (len >= 73 && line[70] == ' ' && line[71] == ' ')
+        modres.mod_id = read_string(line + 72, 6);
+      st.mod_residues.push_back(modres);
+
+    } else if (is_record_type(line, "HETNAM")) {
+      if (len > 71 && line[70] == ' ') {
+        std::string full_code = read_string(line + 71, 8);
+        if (!full_code.empty())
+          st.shortened_ccd_codes.push_back({full_code, read_string(line + 11, 3)});
+      }
+
     } else if (is_record_type(line, "DBREF")) { // DBREF or DBREF1 or DBREF2
       std::string chain_name = read_string(line+11, 2);
       Entity& ent = impl::find_or_add(st.entities, chain_name);
       if (line[5] == ' ' || line[5] == '1')
         ent.dbrefs.emplace_back();
       else if (ent.dbrefs.empty()) // DBREF2 without DBREF1?
         continue;
@@ -615,14 +636,16 @@
 
   for (std::string& name : st.meta.authors)
     change_author_name_format_to_mmcif(name);
 
   if (!options.skip_remarks)
     read_metadata_from_remarks(st);
 
+  restore_full_ccd_codes(st);
+
   return st;
 }
 
 }  // namespace pdb_impl
 
 inline Structure read_pdb_file(const std::string& path,
                                PdbReadOptions options=PdbReadOptions()) {
```

### Comparing `gemmi-0.6.1/include/gemmi/pirfasta.hpp` & `gemmi-0.6.2/include/gemmi/pirfasta.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/polyheur.hpp` & `gemmi-0.6.2/include/gemmi/polyheur.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -144,14 +144,17 @@
 /// for residues with entity_type==Unknown, unless overwrite=true).
 /// Determining where the polymer ends and ligands start is sometimes
 /// arbitrary -- there can be a non-standard residue at the end that can
 /// be regarded as as either the last residue or a linked ligand.
 GEMMI_DLL void add_entity_types(Chain& chain, bool overwrite);
 GEMMI_DLL void add_entity_types(Structure& st, bool overwrite);
 
+/// Assigns Residue::entity_id based on Residue::subchain and Entity::subchains.
+GEMMI_DLL void add_entity_ids(Structure& st, bool overwrite);
+
 /// The subchain field in the residue is where we store_atom_site.label_asym_id
 /// from mmCIF files. As of 2018 wwPDB software splits author's chains
 /// (auth_asym_id) into label_asym_id units:
 /// * linear polymer,
 /// * non-polymers (each residue has different separate label_asym_id),
 /// * and waters.
 /// Refmac/makecif is doing similar thing but using different naming and
@@ -215,9 +218,22 @@
 }
 
 inline void trim_to_alanine(Chain& chain) {
   for (Residue& res : chain.residues)
     trim_to_alanine(res);
 }
 
+// Functions for switching between long (>3 chars) residue names (CCD codes)
+// and shortened ones that are compatible with the PDB format.
+GEMMI_DLL
+void change_ccd_code(Structure& st, const std::string& old, const std::string& new_);
+
+GEMMI_DLL void shorten_ccd_codes(Structure& st);
+
+inline void restore_full_ccd_codes(Structure& st) {
+  for (const OldToNew& item : st.shortened_ccd_codes)
+    change_ccd_code(st, item.new_, item.old);
+  st.shortened_ccd_codes.clear();
+}
+
 } // namespace gemmi
 #endif
```

### Comparing `gemmi-0.6.1/include/gemmi/qcp.hpp` & `gemmi-0.6.2/include/gemmi/qcp.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/read_cif.hpp` & `gemmi-0.6.2/include/gemmi/read_cif.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/read_map.hpp` & `gemmi-0.6.2/include/gemmi/read_map.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/recgrid.hpp` & `gemmi-0.6.2/include/gemmi/recgrid.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/reciproc.hpp` & `gemmi-0.6.2/include/gemmi/reciproc.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/refln.hpp` & `gemmi-0.6.2/include/gemmi/refln.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   int wavelength_count;
   cif::Loop* refln_loop = nullptr;
   cif::Loop* diffrn_refln_loop = nullptr;
   cif::Loop* default_loop = nullptr;
 
   ReflnBlock() = default;
   ReflnBlock(ReflnBlock&& rblock_) = default;
-  ReflnBlock(cif::Block&& block_) : block(block_) {
+  ReflnBlock(cif::Block&& block_) : block(std::move(block_)) {
     entry_id = cif::as_string(block.find_value("_entry.id"));
     impl::set_cell_from_mmcif(block, cell);
     if (const std::string* hm = impl::find_spacegroup_hm_value(block))
       spacegroup = find_spacegroup_by_name(cif::as_string(*hm),
                                            cell.alpha, cell.gamma);
     cell.set_cell_images_from_spacegroup(spacegroup);
     const char* wave_tag = "_diffrn_radiation_wavelength.wavelength";
```

### Comparing `gemmi-0.6.1/include/gemmi/remarks.hpp` & `gemmi-0.6.2/include/gemmi/remarks.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/resinfo.hpp` & `gemmi-0.6.2/include/gemmi/resinfo.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/riding_h.hpp` & `gemmi-0.6.2/include/gemmi/riding_h.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/scaling.hpp` & `gemmi-0.6.2/include/gemmi/scaling.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/select.hpp` & `gemmi-0.6.2/include/gemmi/select.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/seqalign.hpp` & `gemmi-0.6.2/include/gemmi/seqalign.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/seqid.hpp` & `gemmi-0.6.2/include/gemmi/seqid.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/sfcalc.hpp` & `gemmi-0.6.2/include/gemmi/sfcalc.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/small.hpp` & `gemmi-0.6.2/include/gemmi/small.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/smcif.hpp` & `gemmi-0.6.2/include/gemmi/smcif.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/solmask.hpp` & `gemmi-0.6.2/include/gemmi/solmask.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/span.hpp` & `gemmi-0.6.2/include/gemmi/span.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/stats.hpp` & `gemmi-0.6.2/include/gemmi/stats.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/symmetry.hpp` & `gemmi-0.6.2/include/gemmi/symmetry.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -2073,30 +2073,46 @@
       case 15: return "(k>=0 and h>0) or (h==0 and k==0 and l>=0)";
       case 18: return "k>=0 and l>=0 and ((h>k and h>l) or (h==k and h>=l))";
       case 19: return "h>=k and k>=l and l>=0";
     }
     unreachable();
   }
 
-  // Returns hkl in asu and MTZ ISYM - 2*n-1 for reflections in the positive
-  // asu (I+ of a Friedel pair), 2*n for reflections in the negative asu (I-).
+  /// Returns hkl in asu and MTZ ISYM - 2*n-1 for reflections in the positive
+  /// asu (I+ of a Friedel pair), 2*n for reflections in the negative asu (I-).
   std::pair<Op::Miller,int> to_asu(const Op::Miller& hkl, const GroupOps& gops) const {
     int isym = 0;
     for (const Op& op : gops.sym_ops) {
       ++isym;
       Op::Miller new_hkl = op.apply_to_hkl_without_division(hkl);
       if (is_in(new_hkl))
         return {Op::divide_hkl_by_DEN(new_hkl), isym};
       ++isym;
       Op::Miller negated_new_hkl{{-new_hkl[0], -new_hkl[1], -new_hkl[2]}};
       if (is_in(negated_new_hkl))
         return {Op::divide_hkl_by_DEN(negated_new_hkl), isym};
     }
     fail("Oops, maybe inconsistent GroupOps?");
   }
+  /// Similar to to_asu(), but the second returned value is sign: true for + or centric
+  std::pair<Op::Miller,bool> to_asu_sign(const Op::Miller& hkl, const GroupOps& gops) const {
+    std::pair<Op::Miller,bool> neg = {{0,0,0}, true};
+    for (const Op& op : gops.sym_ops) {
+      Op::Miller new_hkl = op.apply_to_hkl_without_division(hkl);
+      if (is_in(new_hkl))
+        return {Op::divide_hkl_by_DEN(new_hkl), true};
+      Op::Miller negated_new_hkl{{-new_hkl[0], -new_hkl[1], -new_hkl[2]}};
+      if (is_in(negated_new_hkl))
+        // don't return it yet, because for centric reflection we prefer (+)
+        neg = {Op::divide_hkl_by_DEN(negated_new_hkl), false};
+    }
+    if (neg.second)
+      fail("Oops, maybe inconsistent GroupOps?");
+    return neg;
+  }
 };
 
 } // namespace gemmi
 
 namespace std {
 template<> struct hash<gemmi::Op> {
   size_t operator()(const gemmi::Op& op) const {
```

### Comparing `gemmi-0.6.1/include/gemmi/third_party/fast_float.h` & `gemmi-0.6.2/include/gemmi/third_party/fast_float.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/pocketfft_hdronly.h` & `gemmi-0.6.2/include/gemmi/third_party/pocketfft_hdronly.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/sajson.h` & `gemmi-0.6.2/include/gemmi/third_party/sajson.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/stb_sprintf.h` & `gemmi-0.6.2/third_party/stb_sprintf.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/LICENSE` & `gemmi-0.6.2/include/gemmi/third_party/tao/LICENSE`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/analyze_cycles.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/analysis/analyze_cycles.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/counted.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/analysis/counted.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/generic.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/analysis/generic.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/grammar_info.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/analysis/grammar_info.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/insert_guard.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/analysis/insert_guard.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/insert_rules.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/analysis/insert_rules.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/rule_info.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/analysis/rule_info.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analysis/rule_type.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/analysis/rule_type.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/analyze.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/analyze.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/argv_input.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/argv_input.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/ascii.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/ascii.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/buffer_input.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/buffer_input.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/config.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/config.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/cstream_input.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/cstream_input.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/eol.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/eol.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/file_input.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/file_input.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/input_error.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/input_error.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/action.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/action.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/action_input.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/action_input.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/alnum.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/alnum.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/alpha.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/alpha.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/any.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/any.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/apply.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/apply.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/apply0.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/apply0.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/apply0_single.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/apply0_single.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/apply_single.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/apply_single.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/at.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/at.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/bof.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/bof.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/bol.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/bol.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/bump_help.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/bump_help.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/bump_impl.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/bump_impl.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/bytes.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/bytes.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/control.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/control.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/cr_crlf_eol.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/cr_crlf_eol.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/cr_eol.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/cr_eol.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/crlf_eol.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/crlf_eol.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/cstream_reader.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/cstream_reader.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/cstring_reader.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/cstring_reader.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/demangle.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/demangle.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/demangle_cxxabi.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/demangle_cxxabi.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/demangle_nop.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/demangle_nop.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/demangle_sanitise.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/demangle_sanitise.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/disable.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/disable.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/discard.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/discard.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/dusel_mode.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/dusel_mode.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/duseltronik.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/duseltronik.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/enable.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/enable.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/endian.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/endian.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/endian_gcc.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/endian_gcc.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/endian_win.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/endian_win.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/eof.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/eof.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/eol.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/eol.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/eolf.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/eolf.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/file_mapper.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/file_mapper.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/file_opener.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/file_opener.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/file_reader.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/file_reader.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/has_apply.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/has_apply.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/has_apply0.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/has_apply0.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/identifier.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/identifier.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/if_apply.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/if_apply.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/if_must.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/if_must.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/if_must_else.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/if_must_else.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/if_then_else.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/if_then_else.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/input_pair.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/input_pair.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/integer_sequence.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/integer_sequence.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/istream_reader.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/istream_reader.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/istring.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/istring.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/iterator.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/iterator.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/lf_crlf_eol.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/lf_crlf_eol.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/lf_eol.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/lf_eol.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/list.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/list.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/list_must.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/list_must.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/list_tail.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/list_tail.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/list_tail_pad.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/list_tail_pad.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/marker.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/marker.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/minus.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/minus.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/must.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/must.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/not_at.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/not_at.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/one.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/one.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/opt.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/opt.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/pad.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/pad.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/pad_opt.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/pad_opt.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/peek_char.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/peek_char.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/peek_utf16.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/peek_utf16.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/peek_utf32.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/peek_utf32.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/peek_utf8.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/peek_utf8.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/pegtl_string.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/pegtl_string.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/plus.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/plus.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/raise.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/raise.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/range.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/range.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/ranges.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/ranges.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rep.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/rep.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rep_min.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/rep_min.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rep_min_max.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/rep_min_max.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rep_opt.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/rep_opt.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/require.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/require.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/result_on_found.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/result_on_found.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rule_conjunction.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/rule_conjunction.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/rules.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/rules.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/seq.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/seq.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/skip_control.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/skip_control.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/sor.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/sor.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/star.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/star.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/star_must.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/star_must.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/state.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/state.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/string.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/string.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/trivial.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/trivial.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/try_catch_type.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/try_catch_type.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/internal/until.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/internal/until.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/istream_input.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/istream_input.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/memory_input.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/memory_input.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/mmap_input.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/mmap_input.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/normal.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/normal.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/nothing.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/nothing.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/parse.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/parse.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/parse_error.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/parse_error.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/position.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/position.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/read_input.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/read_input.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/rules.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/rules.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/string_input.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/string_input.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/utf16.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/utf16.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/utf32.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/utf32.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/utf8.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/utf8.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl/version.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl/version.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tao/pegtl.hpp` & `gemmi-0.6.2/include/gemmi/third_party/tao/pegtl.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/third_party/tinydir.h` & `gemmi-0.6.2/include/gemmi/third_party/tinydir.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/to_chemcomp.hpp` & `gemmi-0.6.2/include/gemmi/to_chemcomp.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/to_cif.hpp` & `gemmi-0.6.2/include/gemmi/to_cif.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/to_json.hpp` & `gemmi-0.6.2/include/gemmi/to_json.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/to_mmcif.hpp` & `gemmi-0.6.2/include/gemmi/to_mmcif.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
   bool origx:1;
   bool struct_conf:1;
   bool struct_sheet:1;
   bool struct_biol:1;
   bool assembly:1;
   bool conn:1;
   bool cis:1;
+  bool modres:1;
   bool scale:1;
   bool atom_type:1;
   bool entity_poly_seq:1;
   bool tls:1;
   bool software:1;
   bool group_pdb:1;  // include _atom_site.group_PDB
   bool auth_all:1;   // include _atom_site.auth_atom_id and auth_comp_id
@@ -47,15 +48,15 @@
   explicit MmcifOutputGroups(bool all)
     : atoms(all), block_name(all), entry(all), database_status(all),
       author(all), cell(all), symmetry(all), entity(all),
       entity_poly(false),  // see the comment under "if (groups.entity_poly)"
       struct_ref(all), chem_comp(all), exptl(all), diffrn(all),
       reflns(all), refine(all), title_keywords(all), ncs(all),
       struct_asym(all), origx(all), struct_conf(all), struct_sheet(all),
-      struct_biol(all), assembly(all), conn(all), cis(all),
+      struct_biol(all), assembly(all), conn(all), cis(all), modres(all),
       scale(all), atom_type(all), entity_poly_seq(all), tls(all),
       software(all), group_pdb(all), auth_all(false) {}
 };
 
 GEMMI_DLL void update_mmcif_block(const Structure& st, cif::Block& block,
                                   MmcifOutputGroups groups=MmcifOutputGroups(true));
 GEMMI_DLL cif::Document make_mmcif_document(const Structure& st,
```

### Comparing `gemmi-0.6.1/include/gemmi/to_pdb.hpp` & `gemmi-0.6.2/include/gemmi/to_pdb.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/topo.hpp` & `gemmi-0.6.2/include/gemmi/topo.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/twin.hpp` & `gemmi-0.6.2/include/gemmi/twin.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/unitcell.hpp` & `gemmi-0.6.2/include/gemmi/unitcell.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/utf.hpp` & `gemmi-0.6.2/include/gemmi/utf.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/util.hpp` & `gemmi-0.6.2/include/gemmi/util.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/include/gemmi/xds_ascii.hpp` & `gemmi-0.6.2/include/gemmi/xds_ascii.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/python/align.cpp` & `gemmi-0.6.2/python/align.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/python/ccp4.cpp` & `gemmi-0.6.2/python/ccp4.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/python/chemcomp.cpp` & `gemmi-0.6.2/python/chemcomp.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/python/cif.cpp` & `gemmi-0.6.2/python/cif.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/python/common.h` & `gemmi-0.6.2/python/common.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/python/elem.cpp` & `gemmi-0.6.2/python/elem.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/python/gemmi.cpp` & `gemmi-0.6.2/python/gemmi.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 // Copyright 2017 Global Phasing Ltd.
 
 #include "gemmi/version.hpp"   // for GEMMI_VERSION
 #include "gemmi/math.hpp"      // for hc
 #include "gemmi/dirwalk.hpp"   // for CifWalk, CoorFileWalk
-#include "gemmi/fileutil.hpp"  // for expand_if_pdb_code
+#include "gemmi/pdb_id.hpp"    // for expand_if_pdb_code
 #include "gemmi/bessel.hpp"    // for bessel_i1_over_i0
 #include "gemmi/stats.hpp"     // for Correlation
 #include "gemmi/third_party/tao/pegtl/parse_error.hpp" // for parse_error
 
 #include "common.h"
 #include <pybind11/stl.h>
 #include <pybind11/numpy.h>    // for vectorize
@@ -26,25 +26,26 @@
     throw py::value_error("bin numbers must be smaller than million");
   return max_bin;
 }
 } // anonymous namespace
 
 void add_misc(py::module& m) {
   py::class_<gemmi::CifWalk>(m, "CifWalk")
-    .def(py::init<const char*>())
+    .def(py::init<const char*, char>(), py::arg("path"), py::arg("try_pdbid")='\0')
     .def("__iter__", [](gemmi::CifWalk& self) {
         return py::make_iterator(self);
     }, py::keep_alive<0, 1>());
   py::class_<gemmi::CoorFileWalk>(m, "CoorFileWalk")
-    .def(py::init<const char*>())
+    .def(py::init<const char*, char>(), py::arg("path"), py::arg("try_pdbid")='\0')
     .def("__iter__", [](gemmi::CoorFileWalk& self) {
         return py::make_iterator(self);
     }, py::keep_alive<0, 1>());
   m.def("is_pdb_code", &gemmi::is_pdb_code);
-  m.def("expand_pdb_code_to_path", &gemmi::expand_pdb_code_to_path);
+  m.def("expand_pdb_code_to_path", &gemmi::expand_pdb_code_to_path,
+        py::arg("code"), py::arg("filetype"), py::arg("throw_if_unset")=false);
   m.def("expand_if_pdb_code", &gemmi::expand_if_pdb_code,
         py::arg("code"), py::arg("filetype")='M');
   m.attr("hc") = py::float_(gemmi::hc());
   m.def("bessel_i1_over_i0", py::vectorize(gemmi::bessel_i1_over_i0));
   m.def("log_bessel_i0", py::vectorize(gemmi::log_bessel_i0));
   m.def("log_cosh", py::vectorize([](double x) {
         // ln(cosh(x)) = ln(e^x + e^-x) - ln(2) = ln(e^x * (1 + e^-2x)) - ln(2)
```

### Comparing `gemmi-0.6.1/python/grid.cpp` & `gemmi-0.6.2/python/grid.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/python/hkl.cpp` & `gemmi-0.6.2/python/hkl.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
   pyReflnBlock
     .def_readonly("block", &ReflnBlock::block)
     .def_readonly("entry_id", &ReflnBlock::entry_id)
     .def_readonly("cell", &ReflnBlock::cell)
     .def_readonly("spacegroup", &ReflnBlock::spacegroup)
     .def_readonly("wavelength", &ReflnBlock::wavelength)
+    .def_readonly("default_loop", &ReflnBlock::default_loop)
     .def("column_labels", &ReflnBlock::column_labels)
     .def("make_int_array",
          [](ReflnBlock& self, const std::string& tag, int null) {
            return py_array_from_vector(self.make_vector(tag, null));
     }, py::arg("tag"), py::arg("null"))
     .def("make_float_array",
          [](ReflnBlock& self, const std::string& tag, double null) {
```

### Comparing `gemmi-0.6.1/python/meta.cpp` & `gemmi-0.6.2/python/meta.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/python/meta.h` & `gemmi-0.6.2/python/meta.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/python/miller_a.h` & `gemmi-0.6.2/python/miller_a.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/python/mol.cpp` & `gemmi-0.6.2/python/mol.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -163,16 +163,15 @@
     .def("deduplicate_entities", &deduplicate_entities)
     .def("setup_entities", &setup_entities)
     .def("remove_alternative_conformations",
          remove_alternative_conformations<Structure>)
     .def("remove_hydrogens", remove_hydrogens<Structure>)
     .def("remove_waters", remove_waters<Structure>)
     .def("remove_ligands_and_waters", remove_ligands_and_waters<Structure>)
-    .def("expand_hd_mixture", &expand_hd_mixture)
-    .def("collapse_hd_mixture", &collapse_hd_mixture)
+    .def("store_deuterium_as_fraction", &store_deuterium_as_fraction)
     .def("assign_serial_numbers", (void (*)(Structure&)) &assign_serial_numbers)
     .def("shorten_chain_names", &shorten_chain_names)
     .def("expand_ncs", &expand_ncs, py::arg("how"))
     .def("transform_to_assembly",
          [](Structure& st, const std::string& assembly_name, HowToNameCopiedChain how) {
         return transform_to_assembly(st, assembly_name, how, nullptr);
     }, py::arg("assembly_name"), py::arg("how"))
@@ -461,14 +460,15 @@
     .def("__repr__", [](const Residue& self) {
         return tostr("<gemmi.Residue ", self.str(), " with ",
                      self.atoms.size(), " atoms>");
     });
 
   py::enum_<CalcFlag>(m, "CalcFlag")
     .value("NotSet", CalcFlag::NotSet)
+    .value("NoHydrogen", CalcFlag::NoHydrogen)
     .value("Determined", CalcFlag::Determined)
     .value("Calculated", CalcFlag::Calculated)
     .value("Dummy", CalcFlag::Dummy);
 
   pyAtom
     .def(py::init<>())
     .def_readwrite("name", &Atom::name)
```

### Comparing `gemmi-0.6.1/python/monlib.cpp` & `gemmi-0.6.2/python/monlib.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/python/mtz.cpp` & `gemmi-0.6.2/python/mtz.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/python/read.cpp` & `gemmi-0.6.2/python/read.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/python/recgrid.cpp` & `gemmi-0.6.2/python/recgrid.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/python/scaling.cpp` & `gemmi-0.6.2/python/scaling.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/python/search.cpp` & `gemmi-0.6.2/python/search.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/python/sf.cpp` & `gemmi-0.6.2/python/sf.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/python/sym.cpp` & `gemmi-0.6.2/python/sym.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/python/topo.cpp` & `gemmi-0.6.2/python/topo.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     ;
   py::class_<Topo::Link>(topo, "Link")
     .def_readonly("link_id", &Topo::Link::link_id)
     .def_readonly("res1", &Topo::Link::res1)
     .def_readonly("res2", &Topo::Link::res2)
     .def_readonly("alt1", &Topo::Link::alt1)
     .def_readonly("alt2", &Topo::Link::alt2)
+    .def_readonly("link_rules", &Topo::Link::link_rules)
     ;
   py::enum_<Topo::RKind>(m, "RKind")
     .value("Bond", Topo::RKind::Bond)
     .value("Angle", Topo::RKind::Angle)
     .value("Torsion", Topo::RKind::Torsion)
     .value("Chirality", Topo::RKind::Chirality)
     .value("Plane", Topo::RKind::Plane)
```

### Comparing `gemmi-0.6.1/python/tostr.hpp` & `gemmi-0.6.2/python/tostr.hpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/python/unitcell.cpp` & `gemmi-0.6.2/python/unitcell.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -232,14 +232,15 @@
 
   py::class_<FTransform, Transform>(m, "FTransform")
     .def("apply", &FTransform::apply);
 
 
   py::class_<NearestImage>(m, "NearestImage")
     .def("dist", &NearestImage::dist)
+    .def("same_asu", &NearestImage::same_asu)
     .def("symmetry_code", &NearestImage::symmetry_code, py::arg("underscore")=true)
     .def_readonly("sym_idx", &NearestImage::sym_idx)
     .def_property_readonly("pbc_shift", [](const NearestImage& self) {
         return py::make_tuple(self.pbc_shift[0], self.pbc_shift[1], self.pbc_shift[2]);
     })
     .def("__repr__", [](const NearestImage& self) {
         using namespace std;  // VS2015/17 doesn't like std::snprintf
```

### Comparing `gemmi-0.6.1/python/write.cpp` & `gemmi-0.6.2/python/write.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/setup.py` & `gemmi-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/src/assembly.cpp` & `gemmi-0.6.2/src/assembly.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -323,16 +323,18 @@
               AtomAddress& aa = j == 0 ? c.partner1 : c.partner2;
               if (how == HowToNameCopiedChain::Dup) {
                 aa.res_id.segment = op.id;
               } else {
                 auto it = chain_mapping.find(aa.chain_name);
                 if (it != chain_mapping.end())
                   aa.chain_name = it->second;
-                else
+                else {
                   st.connections.pop_back();
+                  break;
+                }
               }
             }
           }
         }
       }
   }
   // adjust connections after changing segment of original chains to "0"
```

### Comparing `gemmi-0.6.1/src/calculate.cpp` & `gemmi-0.6.2/src/calculate.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/src/crd.cpp` & `gemmi-0.6.2/src/crd.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #include "gemmi/version.hpp"   // for GEMMI_VERSION
 
 namespace gemmi {
 
 void setup_for_crd(Structure& st) {
   // setup_entities(st) but with forced subchain reassignment
   add_entity_types(st, /*overwrite=*/false);
+  add_entity_ids(st, /*overwrite=*/false);
   assign_subchains(st, /*force=*/true);
   for (Model& model : st.models)
     for (Chain& chain : model.chains)
       for (Residue& res : chain.residues) {
         size_t n = chain.name.size();
         assert(res.subchain[n] == 'x');
         res.subchain[n] = '_';
@@ -37,14 +38,15 @@
           return true;
   return false;
 }
 
 static std::string refmac_calc_flag(const Atom& a) {
   switch (a.calc_flag) {
     case CalcFlag::NotSet: return ".";
+    case CalcFlag::NoHydrogen: return ".";
     // Refmac seems to be using only flags R and M
     case CalcFlag::Calculated: return a.is_hydrogen() ? "R" : "M";
     // I think these are not used
     case CalcFlag::Determined: return "d";
     case CalcFlag::Dummy: return "dum";
   }
   unreachable();
@@ -99,16 +101,20 @@
     st.connections.push_back(conn);
   });
 }
 
 cif::Block prepare_crd(const Structure& st, const Topo& topo,
                        HydrogenChange h_change, const std::string& info_comment) {
   auto e_id = st.info.find("_entry.id");
-  std::string id = cif::quote(e_id != st.info.end() ? e_id->second : st.name);
+  std::string id = (e_id != st.info.end() ? e_id->second : st.name);
   cif::Block block("structure_" + id);
+  if (id.empty() || id == " " || id == "#")
+    id = "?";
+  else
+    id = cif::quote(id);
   auto& items = block.items;
 
   if (!info_comment.empty())
     items.emplace_back(cif::CommentArg{info_comment});
   items.emplace_back("_entry.id", id);
   items.emplace_back("_database_2.code_PDB", id);
   auto keywords = st.info.find("_struct_keywords.pdbx_keywords");
@@ -305,22 +311,15 @@
       }
     }
   return block;
 }
 
 template<int Prec>
 std::string to_str_dot(double d) {
-  static_assert(Prec >= 0 && Prec < 7, "unsupported precision");
-  if (!std::isnan(d)) {
-    char buf[16];
-    int len = gstb_sprintf(buf, "%.*f", Prec, d);
-    if (len > 0)
-      return std::string(buf, len);
-  }
-  return ".";
+  return std::isnan(d) ? "." : to_str_prec<Prec>(d);
 }
 
 static void add_restraint_row(cif::Loop& restr_loop,
                               const char* record, int counter,
                               const std::string& label, const std::string& period,
                               std::initializer_list<const Atom*> atoms,
                               double value, double dev,
```

### Comparing `gemmi-0.6.1/src/eig3.cpp` & `gemmi-0.6.2/src/eig3.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/src/mmcif.cpp` & `gemmi-0.6.2/src/mmcif.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -268,14 +268,37 @@
       cispep.only_altloc = cif::as_char(row[kAltId], '\0');
     if (row.has(kOmegaAngle))
       cispep.reported_angle = cif::as_number(row[kOmegaAngle]);
     st.cispeps.push_back(cispep);
   }
 }
 
+// MODRES equivalent
+void read_struct_mod_residue(cif::Block& block, Structure& st) {
+  // Here auth_asym_id etc are mandatory and label_asym_id etc optional.
+  for (auto row : block.find("_pdbx_struct_mod_residue.",
+                             {"auth_asym_id",  // 0
+                              "auth_seq_id", "?PDB_ins_code",  // 1-2
+                              "?auth_comp_id", "?label_comp_id",  // 3-4
+                              "?parent_comp_id", "?details",  // 5-6
+                              "?ccp4_mod_id"})) {  // 7
+    ModRes modres;
+    modres.chain_name = row.str(0);
+    modres.res_id.seqid = make_seqid(row.str(1), row.ptr_at(2));
+    modres.res_id.name = row.one_of(3, 4);
+    if (row.has(5))
+      modres.parent_comp_id = row.str(5);
+    if (row.has(6))
+      modres.details = row.str(6);
+    if (row.has(7))
+      modres.mod_id = row.str(7);
+    st.mod_residues.push_back(modres);
+  }
+}
+
 // Operation expression is an item type used for *.oper_expression.
 // Here, to keep it simple, we ignore products such as "(2)(3)".
 // We parse "3", "1,3,5", "one,two", "(3)", "(a)", "(1-60)", "(2,3-8,XY)", etc
 std::vector<std::string> parse_operation_expr(const std::string& expr) {
   std::vector<std::string> result;
   std::size_t start = 0;
   std::size_t close_br = std::string::npos;
@@ -873,14 +896,15 @@
   st.setup_cell_images();
 
 
   st.helices = read_helices(block);
   st.sheets = read_sheets(block);
   read_connectivity(block, st);
   read_prot_cis(block, st);
+  read_struct_mod_residue(block, st);
   st.assemblies = read_assemblies(block);
   read_sifts_unp(block, st);
 
   return st;
 }
 
 } // namespace gemmi
```

### Comparing `gemmi-0.6.1/src/mmread_gz.cpp` & `gemmi-0.6.2/src/mmread_gz.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/src/monlib.cpp` & `gemmi-0.6.2/src/monlib.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/src/mtz.cpp` & `gemmi-0.6.2/src/mtz.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,17 @@
           data[n + *(i+0)] = float(a * cosx - b * sinx);
           data[n + *(i+1)] = float(a * sinx + b * cosx);
           data[n + *(i+2)] = float(c * cos2x - d * sin2x);
           data[n + *(i+3)] = float(c * sin2x + d * cos2x);
         }
       }
     }
-    if (isym % 2 == 0 && !centric) {
+    if (isym % 2 == 0 && !centric &&
+        // usually, centric reflections have empty F(-), so avoid swapping it
+        !gops.is_reflection_centric(hkl)) {
       for (std::pair<int,int> cols : plus_minus_columns)
         std::swap(data[n + cols.first], data[n + cols.second]);
       for (int col : dano_columns)
         data[n + col] = -data[n + col];
     }
   }
 }
@@ -127,15 +129,15 @@
     ds.cell = ds.cell.changed_basis_backward(transposed_op, false);
   for (Mtz::Batch& batch : batches)
     batch.set_cell(batch.get_cell().changed_basis_backward(transposed_op, false));
 }
 
 
 #define WRITE(...) do { \
-    int len = gstb_snprintf(buf, 81, __VA_ARGS__); \
+    int len = snprintf_z(buf, 81, __VA_ARGS__); \
     if (len < 80) \
       std::memset(buf + len, ' ', 80 - len); \
     if (write(buf, 80, 1) != 1) \
       sys_fail("Writing MTZ file failed"); \
   } while(0)
 
 template<typename Write>
@@ -192,15 +194,15 @@
   WRITE("RESO %-20.12f %-20.12f", reso[0], reso[1]);
   if (std::isnan(valm))
     WRITE("VALM NAN");
   else
     WRITE("VALM %f", valm);
   auto format17 = [](float f) {
     char buffer[18];
-    int len = gstb_snprintf(buffer, 18, "%.9f", f);
+    int len = snprintf_z(buffer, 18, "%.9f", f);
     return std::string(buffer, len > 0 ? std::min(len, 17) : 0);
   };
   for (const Column& col : columns) {
     auto minmax = calculate_min_max_disregarding_nans(col.begin(), col.end());
     const char* label = !col.label.empty() ? col.label.c_str() : "_";
     WRITE("COLUMN %-30s %c %17s %17s %4d",
           label, col.type,
@@ -218,15 +220,15 @@
     WRITE("DCELL %9d %10.4f%10.4f%10.4f%10.4f%10.4f%10.4f",
           ds.id, uc.a, uc.b, uc.c, uc.alpha, uc.beta, uc.gamma);
     WRITE("DWAVEL %8d %10.5f", ds.id, ds.wavelength);
     for (size_t i = 0; i < batches.size(); i += 12) {
       std::memcpy(buf, "BATCH ", 6);
       int pos = 6;
       for (size_t j = i; j < std::min(batches.size(), i + 12); ++j, pos += 6)
-        gstb_snprintf(buf + pos, 7, "%6zu", j + 1);
+        snprintf_z(buf + pos, 7, "%6zu", j + 1);
       std::memset(buf + pos, ' ', 80 - pos);
       if (write(buf, 80, 1) != 1)
         fail("Writing MTZ file failed");
     }
   }
   WRITE("END");
   if (!history.empty()) {
```

### Comparing `gemmi-0.6.1/src/mtz2cif.cpp` & `gemmi-0.6.2/src/mtz2cif.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #include <climits>       // for INT_MIN
 #include <algorithm>     // for all_of
 #include <set>
 #include <unordered_map>
 
 #include <gemmi/asudata.hpp>   // for calculate_hkl_value_correlation
 #include <gemmi/eig3.hpp>      // for eigen_decomposition
-#include <gemmi/sprintf.hpp>   // for gstb_snprintf, to_str
+#include <gemmi/sprintf.hpp>   // for snprintf_z, to_str
 #include <gemmi/atox.hpp>      // for read_word
 #include <gemmi/version.hpp>   // for GEMMI_VERSION
 
 namespace gemmi {
 
 namespace {
 
@@ -58,15 +58,15 @@
   if (c != 'F' && c != 'G' && c != 'E')
     fail("expected floating-point format, got: " + fmt);
   if (min_width > 32)
     fail("the width exceeds 32: " + fmt);
   return min_width;
 }
 
-#define WRITE(...) os.write(buf, gstb_snprintf(buf, 255, __VA_ARGS__))
+#define WRITE(...) os.write(buf, snprintf_z(buf, 255, __VA_ARGS__))
 
 void write_cell_and_symmetry(const std::string& entry_id,
                              const UnitCell& cell, double* rmsds, const SpaceGroup* sg,
                              char* buf, std::ostream& os) {
   os << "_cell.entry_id " << entry_id << '\n';
   WRITE("_cell.length_a    %8.4f\n", cell.a);
   if (rmsds && rmsds[0] != 0.)
@@ -375,15 +375,15 @@
     if (t.is_status)
       return &t;
   return nullptr;
 }
 
 void write_main_loop(const MtzToCif& m2c, const SweepInfo& sweep_info,
                      const Mtz& mtz, const std::vector<Trans>& recipe,
-                     char* buf, std::ostream& os) {
+                     char (&buf)[256], std::ostream& os) {
   // prepare indices
   std::vector<int> value_indices;  // used for --skip_empty
   std::vector<int> sigma_indices;  // used for status 'x' and --skip-negative-sigi
   for (const Trans& tr : recipe) {
     if (tr.col_idx < 0)
       continue;
     const Mtz::Column& col = mtz.columns[tr.col_idx];
@@ -429,15 +429,15 @@
         if (val == 0.f)
           count++;
       free_flag_value = count < mtz.nreflections / 2 ? 0 : 1;
     }
   }
 
   auto write_int = [](char* p, int num) {
-    //return gstb_snprintf(p, 32, "%d", num);
+    //return snprintf_z(p, 32, "%d", num);
     std::string s = std::to_string(num);
     std::memcpy(p, s.data(), s.size());
     return s.size();
   };
 
   char* ptr = buf;
   for (int i = 0, idx = 0; i != mtz.nreflections; ++i) {
@@ -471,15 +471,16 @@
     }
     bool first = true;
     for (const Trans& tr : recipe) {
       if (first)
         first = false;
       else
         *ptr++ = ' ';
-      if (ptr - buf > 220) {
+      static_assert(sizeof(buf) == 256, "sizeof buf");
+      if (ptr - buf > 256 - 36) {
         os.write(buf, ptr - buf);
         ptr = buf;
       }
       if (tr.col_idx < 0) {
         switch (tr.col_idx) {
           case Var::Dot: *ptr++ = '.'; break;
           case Var::Qmark: *ptr++ = '?'; break;
@@ -502,15 +503,15 @@
             *ptr++ = ' ';
           *ptr++ = '?';
         } else {
 #if defined(__GNUC__)
 # pragma GCC diagnostic push
 # pragma GCC diagnostic ignored "-Wformat-nonliteral"
 #endif
-          ptr += gstb_snprintf(ptr, 32, tr.format.c_str(), v);
+          ptr += snprintf_z(ptr, 32, tr.format.c_str(), v);
 #if defined(__GNUC__)
 # pragma GCC diagnostic pop
 #endif
         }
       }
     }
     *ptr++ = '\n';
@@ -808,22 +809,22 @@
     os << "\n_diffrn_refln.pdbx_scan_angle";
   os << "\n_diffrn_refln.pdbx_image_id\n";
   int idx = 0;
   for (const XdsAscii::Refl& refl : xds.data) {
     if (refl.sigma < 0 && skip_negative_sigi)  // misfit
       continue;
     char* ptr = buf;
-    ptr += gstb_snprintf(ptr, 128, "%d %d %d %d %d %g %.5g ",
-                         refl.iset, ++idx, refl.hkl[0], refl.hkl[1], refl.hkl[2],
-                         refl.iobs, refl.sigma);
+    ptr += snprintf_z(ptr, 128, "%d %d %d %d %d %g %.5g ",
+                      refl.iset, ++idx, refl.hkl[0], refl.hkl[1], refl.hkl[2],
+                      refl.iobs, refl.sigma);
     if (xds.oscillation_range != 0.) {
       double angle = xds.rot_angle(refl);
-      ptr += gstb_snprintf(ptr, 16, "%.5g ", angle);
+      ptr += snprintf_z(ptr, 16, "%.5g ", angle);
     }
-    ptr += gstb_snprintf(ptr, 16, "%d\n", refl.frame());
+    ptr += snprintf_z(ptr, 16, "%d\n", refl.frame());
     os.write(buf, ptr - buf);
   }
 }
 
 #undef WRITE
 
 void remove_appendix_from_column_names(Mtz& mtz, std::ostream& out) {
```

### Comparing `gemmi-0.6.1/src/read_cif.cpp` & `gemmi-0.6.2/src/read_cif.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/src/resinfo.cpp` & `gemmi-0.6.2/src/resinfo.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/src/riding_h.cpp` & `gemmi-0.6.2/src/riding_h.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/src/to_mmcif.cpp` & `gemmi-0.6.2/src/to_mmcif.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,16 @@
   bool has_tls_group_id = false;
   size_t atom_site_count = 0;
   for (const Model& model : st.models)
     for (const Chain& chain : model.chains)
       for (const Residue& res : chain.residues)
         for (const Atom& atom : res.atoms) {
           ++atom_site_count;
-          if (atom.calc_flag != CalcFlag::NotSet)
+          if (atom.calc_flag != CalcFlag::NotSet &&
+              atom.calc_flag != CalcFlag::NoHydrogen)
             has_calc_flag = true;
           if (atom.tls_group_id >= 0)
             has_tls_group_id = true;
         }
   if (has_calc_flag)
     atom_loop.tags.emplace_back("_atom_site.calc_flag");
   if (has_tls_group_id)
@@ -142,15 +143,15 @@
             vv.emplace_back(vv[atom_name_idx]);  // auth_atom_id = label_atom_id
             vv.emplace_back(vv[atom_name_idx + 2]);  // auth_comp_id = label_comp_id
           }
           vv.emplace_back(auth_seq_id);
           vv.emplace_back(qchain(chain.name));
           vv.emplace_back(string_or_qmark(model.name));
           if (has_calc_flag)
-            vv.emplace_back(&".\0d\0c\0dum"[2 * (int) atom.calc_flag]);
+            vv.emplace_back(&".\0.\0d\0c\0dum"[2 * (int) atom.calc_flag]);
           if (has_tls_group_id)
             vv.emplace_back(int_or_qmark(atom.tls_group_id));
           if (st.has_d_fraction)
             vv.emplace_back(to_str(atom.fraction));
           if (atom.aniso.nonzero())
             aniso.emplace_back(serial, &atom);
         }
@@ -854,29 +855,28 @@
         if (!sub_id.empty()) {
           const Entity* ent = find_entity_of_subchain(sub_id, st.entities);
           asym_loop.add_row({sub_id, (ent ? qchain(ent->name) : "?")});
         }
       }
   }
 
-  if (groups.origx) { // _database_PDB_matrix (ORIGX)
-    if (st.has_origx && !st.origx.is_identity()) {
-      cif::ItemSpan span(block.items, "_database_PDB_matrix.");
-      span.set_pair("_database_PDB_matrix.entry_id", id);
-      std::string tag_mat = "_database_PDB_matrix.origx[0][0]";
-      std::string tag_vec = "_database_PDB_matrix.origx_vector[0]";
-      for (int i = 0; i < 3; ++i) {
-        tag_mat[27] += 1;  // origx[0] -> origx[1] -> origx[2]
-        tag_vec[34] += 1;
-        for (int j = 0; j < 3; ++j) {
-          tag_mat[30] = '1' + j;
-          span.set_pair(tag_mat, to_str(st.origx.mat[i][j]));
-        }
-        span.set_pair(tag_vec, to_str(st.origx.vec.at(i)));
+  bool nontrivial_origx = st.has_origx && !st.origx.is_identity();
+  if (groups.origx && nontrivial_origx) { // _database_PDB_matrix (ORIGX)
+    cif::ItemSpan span(block.items, "_database_PDB_matrix.");
+    span.set_pair("_database_PDB_matrix.entry_id", id);
+    std::string tag_mat = "_database_PDB_matrix.origx[0][0]";
+    std::string tag_vec = "_database_PDB_matrix.origx_vector[0]";
+    for (int i = 0; i < 3; ++i) {
+      tag_mat[27] += 1;  // origx[0] -> origx[1] -> origx[2]
+      tag_vec[34] += 1;
+      for (int j = 0; j < 3; ++j) {
+        tag_mat[30] = '1' + j;
+        span.set_pair(tag_mat, to_str(st.origx.mat[i][j]));
       }
+      span.set_pair(tag_vec, to_str(st.origx.vec.at(i)));
     }
   }
 
   if (groups.struct_conf && !st.helices.empty()) {
     cif::Loop& struct_conf_loop = block.init_mmcif_loop("_struct_conf.",
         {"conf_type_id", "id",
          "beg_auth_asym_id", "beg_label_asym_id", "beg_label_comp_id",
@@ -1014,16 +1014,43 @@
 
   if (groups.conn)
     write_struct_conn(st, block);
 
   if (groups.cis)  // _struct_mon_prot_cis
     write_cispeps(st, block);
 
+  // _pdbx_struct_mod_residue (MODRES)
+  if (groups.modres && !st.mod_residues.empty()) {
+    bool use_ccp4_mod_id = false;
+    for (const ModRes& modres : st.mod_residues)
+      if (!modres.mod_id.empty())
+        use_ccp4_mod_id = true;
+    cif::Loop& loop = block.init_mmcif_loop("_pdbx_struct_mod_residue.",
+        {"id", "auth_asym_id", "auth_seq_id", "PDB_ins_code", "auth_comp_id",
+         "label_comp_id", "parent_comp_id", "details"});
+    if (use_ccp4_mod_id)
+      loop.tags.push_back("_pdbx_struct_mod_residue.ccp4_mod_id");
+    int counter = 0;
+    for (const ModRes& modres : st.mod_residues) {
+      auto& v = loop.values;
+      v.push_back(std::to_string(++counter));
+      v.push_back(qchain(modres.chain_name));
+      v.push_back(modres.res_id.seqid.num.str());
+      v.push_back(pdbx_icode(modres.res_id));
+      v.push_back(string_or_dot(modres.res_id.name));
+      v.push_back(string_or_qmark(modres.res_id.name));
+      v.push_back(string_or_qmark(modres.parent_comp_id));
+      v.push_back(string_or_qmark(modres.details));
+      if (use_ccp4_mod_id)
+        v.push_back(string_or_qmark(modres.mod_id));
+    }
+  }
+
   // _atom_sites (SCALE)
-  if (groups.scale && (st.has_origx || st.cell.explicit_matrices)) {
+  if (groups.scale && (nontrivial_origx || st.cell.explicit_matrices)) {
     cif::ItemSpan span(block.items, "_atom_sites.");
     span.set_pair("_atom_sites.entry_id", id);
     std::string prefix = "_atom_sites.fract_transf_";
     for (int i = 0; i < 3; ++i) {
       std::string idx = "[" + std::to_string(i + 1) + "]";
       const auto& frac = st.cell.frac;
       std::string matrix_idx = prefix + "matrix";
```

### Comparing `gemmi-0.6.1/src/to_pdb.cpp` & `gemmi-0.6.2/src/to_pdb.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 #include <gemmi/sprintf.hpp>
 #include <gemmi/resinfo.hpp>
 #include <gemmi/util.hpp>
 
 namespace gemmi {
 
 #define WRITE(...) do { \
-    gstb_snprintf(buf, 82, __VA_ARGS__); \
+    snprintf_z(buf, 82, __VA_ARGS__); \
     buf[80] = '\n'; \
     os.write(buf, 81); \
   } while(0)
 
 #define WRITEU(...) do { \
-    gstb_snprintf(buf, 82, __VA_ARGS__); \
+    snprintf_z(buf, 82, __VA_ARGS__); \
     buf[80] = '\n'; \
     for (int i_ = 0; i_ != 80; i_++) \
       if (buf[i_] >= 'a' && buf[i_] <= 'z') buf[i_] -= 0x20; \
     os.write(buf, 81); \
   } while(0)
 
 #define WRITELN(...) do { \
-    int length__ = gstb_snprintf(buf, 82, __VA_ARGS__); \
+    int length__ = snprintf_z(buf, 82, __VA_ARGS__); \
     if (length__ < 80) \
       std::memset(buf + length__, ' ', 80 - length__); \
     buf[80] = '\n'; \
     os.write(buf, 81); \
   } while(0)
 
 namespace {
@@ -65,35 +65,31 @@
 }
 
 // based on http://cci.lbl.gov/hybrid_36/
 inline std::array<char,8> encode_serial_in_hybrid36(int serial) {
   std::array<char,8> str;
   assert(serial >= 0);
   if (serial < 100000)
-    gstb_sprintf(str.data(), "%5d", serial);
+    to_chars_z(str.data(), str.data() + 8, serial);
   else
-    base36_encode(str.data(), 5, serial - 100000 + 10 * 36 * 36 * 36 * 36);
+    base36_encode(str.data(), 5, serial + (10 * 36 * 36 * 36 * 36 - 100000));
   return str;
 }
 
-// based on http://cci.lbl.gov/hybrid_36/
-inline void encode_seq_num_in_hybrid36(char* str, SeqId::OptionalNum seq_num) {
-  if (*seq_num > -1000 && *seq_num < 10000)
-    gstb_sprintf(str, "%4d", *seq_num);
-  else if (seq_num.has_value())
-    base36_encode(str, 4, *seq_num - 10000 + 10 * 36 * 36 * 36);
-  else
-    std::memcpy(str, "    ", 4);
-}
-
 inline std::array<char,8> write_seq_id(const SeqId& seqid) {
   std::array<char,8> str;
-  encode_seq_num_in_hybrid36(str.data(), *seqid.num);
-  str[4] = seqid.icode;
-  str[5] = '\0';
+  char* ptr = str.data();
+  if (*seqid.num > -1000 && *seqid.num < 10000) {
+    ptr = to_chars_z(ptr, ptr + 5, *seqid.num);
+  } else if (seqid.num.has_value()) {
+    base36_encode(ptr, 4, *seqid.num + (10 * 36 * 36 * 36 - 10000));
+    ptr += 4;
+  }
+  *ptr++ = seqid.icode;
+  *ptr = '\0';
   return str;
 }
 
 inline const char* find_last_break(const char *str, int max_len) {
   int last_break = 0;
   for (int i = 0; i < max_len; i++) {
     if (str[i] == '\0')
@@ -257,15 +253,15 @@
       // 47-54  8f  z
       // 55-60  6f  occupancy (6.2)
       // 61-66  6f  temperature factor (6.2)
       // 67-76  6   -
       // 73-76      segment identifier, left-justified (non-standard)
       // 77-78  2s  element symbol, right-justified
       // 79-80  2s  charge
-      WRITE("%-6s%5s %-4.4s%c%3s"
+      WRITE("%-6s%5s %-4.4s%c%3.3s"
             "%2s%5s   %8.3f%8.3f%8.3f"
             "%6.2f%6.2f      %-4.4s%2s%c%c",
             as_het ? "HETATM" : "ATOM",
             encode_serial_in_hybrid36(++serial).data(),
             a.padded_name().c_str(),
             a.altloc ? std::toupper(a.altloc) : ' ',
             res.name.c_str(),
@@ -289,33 +285,33 @@
             // Sometimes PDB files have explicit 0s (5M05); we ignore them.
             a.charge ? a.charge > 0 ? '0'+a.charge : '0'-a.charge : ' ',
             a.charge ? a.charge > 0 ? '+' : '-' : ' ');
       if (a.aniso.nonzero()) {
         // re-using part of the buffer
         std::memcpy(buf, "ANISOU", 6);
         const double eps = 1e-6;
-        gstb_snprintf(buf+28, 43, "%7.0f%7.0f%7.0f%7.0f%7.0f%7.0f",
-                      a.aniso.u11*1e4 + eps, a.aniso.u22*1e4 + eps,
-                      a.aniso.u33*1e4 + eps, a.aniso.u12*1e4 + eps,
-                      a.aniso.u13*1e4 + eps, a.aniso.u23*1e4 + eps);
+        snprintf_z(buf+28, 43, "%7.0f%7.0f%7.0f%7.0f%7.0f%7.0f",
+                   a.aniso.u11*1e4 + eps, a.aniso.u22*1e4 + eps,
+                   a.aniso.u33*1e4 + eps, a.aniso.u12*1e4 + eps,
+                   a.aniso.u13*1e4 + eps, a.aniso.u23*1e4 + eps);
         buf[28+42] = ' ';
         buf[80] = '\n';
         os.write(buf, 81);
       }
     }
     if (opt.ter_records && buf[0] != '\0' &&
         (opt.ter_ignores_type ? &res == &chain.residues.back()
                               : (res.entity_type == EntityType::Polymer &&
                                 (&res == &chain.residues.back() ||
                                  (&res + 1)->entity_type != EntityType::Polymer)))) {
       if (opt.numbered_ter) {
         // re-using part of the buffer in the middle, e.g.:
         // TER    4153      LYS B 286
-        gstb_snprintf(buf, 82, "TER   %5s",
-                      encode_serial_in_hybrid36(++serial).data());
+        snprintf_z(buf, 82, "TER   %5s",
+                   encode_serial_in_hybrid36(++serial).data());
         std::memset(buf+11, ' ', 6);
         std::memset(buf+28, ' ', 52);
         buf[80] = '\n';
         os.write(buf, 81);
       } else {
         WRITE("%-80s", "TER");
       }
@@ -344,14 +340,15 @@
       WRITE("%-80s", "ENDMDL");
   }
 }
 
 inline void write_header(const Structure& st, std::ostream& os,
                          PdbWriteOptions opt) {
   const std::string& entry_id = st.get_info("_entry.id");
+  const char* entry_id_4 = entry_id.size() <= 4 ? entry_id.c_str() : "";
   char buf[88];
   { // header line
     const char* months = "JANFEBMARAPRMAYJUNJULAUGSEPOCTNOVDEC???";
     const std::string& date =
       st.get_info("_pdbx_database_status.recvd_initial_deposition_date");
     std::string pdb_date;
     if (date.size() == 10) {
@@ -404,90 +401,101 @@
       }
       entity_list.push_back(entity);
     }
     // DBREF / DBREF1 / DBREF2
     for (size_t i = 0; i != entity_list.size(); ++i)
       if (const Entity* entity = entity_list[i]) {
         const Chain& ch = st.models[0].chains[i];
-        const char* dbref_entry_id = entry_id.size() <= 4 ? entry_id.c_str() : "";
         for (const Entity::DbRef& dbref : entity->dbrefs) {
           bool short_record = *dbref.db_end.num < 100000 &&
                               dbref.accession_code.size() < 9 &&
                               dbref.id_code.size() < 13;
           SeqId begin = dbref.seq_begin;
           SeqId end = dbref.seq_end;
           if (!begin.num || !end.num)
             if (ConstResidueGroup polymer = ch.get_polymer()) {
               begin = polymer.label_seq_id_to_auth(dbref.label_seq_begin);
               end = polymer.label_seq_id_to_auth(dbref.label_seq_end);
             }
-          gstb_snprintf(buf, 82, "DBREF  %4s%2s %5s %5s %-6s  ",
-                        dbref_entry_id, ch.name.c_str(),
-                        write_seq_id(begin).data(),
-                        write_seq_id(end).data(),
-                        dbref.db_name.c_str());
+          snprintf_z(buf, 82, "DBREF  %4s%2s %5s %5s %-6s  ",
+                     entry_id_4, ch.name.c_str(),
+                     write_seq_id(begin).data(),
+                     write_seq_id(end).data(),
+                     dbref.db_name.c_str());
           if (dbref.db_name == "PDB" && dbref.id_code == entry_id) {
             // PDB uses self-reference for fragments that don't have real
             // reference. No idea why. In such case the same begin/end is used.
           } else {
             begin = dbref.db_begin;
             end = dbref.db_end;
           }
           if (short_record) {
-            gstb_snprintf(buf+33, 82-33, "%-8s %-12s %5d%c %5d%c            \n",
-                          dbref.accession_code.c_str(), dbref.id_code.c_str(),
-                          *begin.num, begin.icode, *end.num, end.icode);
+            snprintf_z(buf+33, 82-33, "%-8s %-12s %5d%c %5d%c            \n",
+                       dbref.accession_code.c_str(), dbref.id_code.c_str(),
+                       *begin.num, begin.icode, *end.num, end.icode);
           } else {
             buf[5] = '1';  // -> DBREF1
-            gstb_snprintf(buf+33, 82-33, "              %-33s\n",
-                          dbref.id_code.c_str());
+            snprintf_z(buf+33, 82-33, "              %-33s\n",
+                       dbref.id_code.c_str());
           }
           buf[80] = '\n';
           os.write(buf, 81);
           if (!short_record)
             WRITE("DBREF2 %4s%2s     %-22s     %10d  %10d             ",
-                  dbref_entry_id, ch.name.c_str(),
+                  entry_id_4, ch.name.c_str(),
                   dbref.accession_code.c_str(), *begin.num, *end.num);
         }
       }
     // SEQRES
     for (size_t i = 0; i != entity_list.size(); ++i)
       if (const Entity* entity = entity_list[i]) {
         const Chain& ch = st.models[0].chains[i];
         int row = 0;
         int col = 0;
         for (const std::string& monomers : entity->full_sequence) {
           if (col == 0)
-            gstb_snprintf(buf, 82, "SEQRES%4d%2s%5zu %62s\n",
-                          ++row, ch.name.c_str(),
-                          entity->full_sequence.size(), "");
-          size_t end = monomers.find(',');
-          if (end == std::string::npos)
-            end = monomers.length();
+            snprintf_z(buf, 82, "SEQRES%4d%2s%5zu %62s\n",
+                       ++row, ch.name.c_str(),
+                       entity->full_sequence.size(), "");
+          size_t end = std::min(monomers.find(','), std::min(monomers.length(), (size_t)3));
           std::memcpy(buf + 18 + 4*col + 4-end, monomers.c_str(), end);
           if (++col == 13) {
             os.write(buf, 81);
             col = 0;
           }
         }
         if (col != 0) {
           buf[80] = '\n';
           os.write(buf, 81);
         }
       }
   }
 
+  for (const ModRes& modres : st.mod_residues) {
+    WRITE("MODRES %4s %3.3s%2s %5s %3s  %-41.41s  %-8.8s\n",
+          entry_id_4,
+          modres.res_id.name.c_str(),
+          modres.chain_name.c_str(),
+          write_seq_id(modres.res_id.seqid).data(),
+          modres.parent_comp_id.c_str(),
+          modres.details.c_str(),
+          modres.mod_id.c_str());
+  }
+
+  for (const OldToNew& mapping : st.shortened_ccd_codes)
+    WRITE("HETNAM     %3s %55s %-9s\n", mapping.new_.c_str(), "", mapping.old.c_str());
+
   if (!st.helices.empty()) {
     int counter = 0;
     for (const Helix& helix : st.helices) {
       if (++counter == 10000)
         counter = 0;
       // According to the PDB spec serial number can be from 1 to 999.
       // Here, we allow for up to 9999 helices by using columns 7 and 11.
-      gstb_snprintf(buf, 82, "HELIX %4d%4d %3s%2s %5s %3s%2s %5s%2d %35d    \n",
+      snprintf_z(buf, 82, "HELIX %4d%4d %3.3s%2s %5s %3.3s%2s %5s%2d %35d    \n",
             counter, counter,
             helix.start.res_id.name.c_str(), helix.start.chain_name.c_str(),
             write_seq_id(helix.start.res_id.seqid).data(),
             helix.end.res_id.name.c_str(), helix.end.chain_name.c_str(),
             write_seq_id(helix.end.res_id.seqid).data(),
             (int) helix.pdb_helix_class, helix.length);
       if (helix.length < 0) // make 72-76 blank if the length is not given
@@ -500,16 +508,16 @@
   if (!st.sheets.empty()) {
     for (const Sheet& sheet : st.sheets) {
       int strand_counter = 0;
       for (const Sheet::Strand& strand : sheet.strands) {
         const AtomAddress& a2 = strand.hbond_atom2;
         const AtomAddress& a1 = strand.hbond_atom1;
         // H-bond atom names are expected to be O and N
-        WRITE("SHEET%5d %3.3s%2zu %3s%2s%5s %3s%2s%5s%2d  %-3s%3s%2s%5s "
-              " %-3s%3s%2s%5s          ",
+        WRITE("SHEET%5d %3.3s%2zu %3.3s%2s%5s %3.3s%2s%5s%2d  %-3s%3.3s%2s%5s "
+              " %-3s%3.3s%2s%5s          ",
               ++strand_counter, sheet.name.c_str(), sheet.strands.size(),
               strand.start.res_id.name.c_str(), strand.start.chain_name.c_str(),
               write_seq_id(strand.start.res_id.seqid).data(),
               strand.end.res_id.name.c_str(), strand.end.chain_name.c_str(),
               write_seq_id(strand.end.res_id.seqid).data(), strand.sense,
               a2.atom_name.c_str(), a2.res_id.name.c_str(),
               a2.chain_name.c_str(),
@@ -531,15 +539,15 @@
           const_CRA cra2 = st.models[0].find_cra(con.partner2, true);
           if (!cra1.atom || !cra2.atom)
             continue;
           NearestImage im = st.cell.find_nearest_image(cra1.atom->pos,
                                                        cra2.atom->pos, con.asu);
           if (++counter == 10000)
             counter = 0;
-          WRITE("SSBOND%4d %3s%2s %5s %5s%2s %5s %28s %6s %5.2f  ",
+          WRITE("SSBOND%4d %3.3s%2s %5s   %3.3s%2s %5s %28s %6s %5.2f  ",
              counter,
              cra1.residue->name.c_str(), cra1.chain->name.c_str(),
              write_seq_id(cra1.residue->seqid).data(),
              cra2.residue->name.c_str(), cra2.chain->name.c_str(),
              write_seq_id(cra2.residue->seqid).data(),
              "1555", im.symmetry_code(false).c_str(), im.dist());
         }
@@ -565,16 +573,16 @@
             im_same_asu = im.same_asu();
           }
           // Pdb spec: "sym1 and sym2 are right justified and are given as
           // blank when the identity operator (and no cell translation) is
           // to be applied to the atom." But all files from wwPDB have
           // 1555 not blank, so here we also write 1555,
           // except for LINKR (Refmac variant of LINK).
-          gstb_snprintf(buf, 82, "LINK        %-4s%c%3s%2s%5s   "
-                "            %-4s%c%3s%2s%5s  %6s %6s %5s  \n",
+          snprintf_z(buf, 82, "LINK        %-4s%c%3.3s%2s%5s   "
+                "            %-4s%c%3.3s%2s%5s  %6s %6s %5s  \n",
                 cra1.atom ? cra1.atom->padded_name().c_str() : "",
                 cra1.atom && cra1.atom->altloc ? std::toupper(cra1.atom->altloc) : ' ',
                 cra1.residue->name.c_str(),
                 con.partner1.chain_name.c_str(),
                 write_seq_id(cra1.residue->seqid).data(),
                 cra2.atom ? cra2.atom->padded_name().c_str() : "",
                 cra2.atom && cra2.atom->altloc ? std::toupper(cra2.atom->altloc) : ' ',
@@ -583,26 +591,26 @@
                 write_seq_id(cra2.residue->seqid).data(),
                 "1555", im_pdb_symbol.c_str(), im_dist_str.c_str());
           if (opt.use_linkr && !con.link_id.empty()) {
             buf[4] = 'R';  // LINK -> LINKR
             if (im_same_asu)
               std::memset(buf+58, ' ', 14); // erase symmetry
             // overwrite distance with link_id
-            gstb_snprintf(buf+72, 82-72, "%-8s\n", con.link_id.c_str());
+            snprintf_z(buf+72, 82-72, "%-8s\n", con.link_id.c_str());
           }
           buf[80] = '\n';
           os.write(buf, 81);
         }
     }
 
     // CISPEP
     if (opt.cispep_records) {
       int counter = 0;
       for (const CisPep& cispep : st.cispeps) {
-        WRITE("CISPEP%4d %3s%2s %5s   %3s%2s %5s %9s %12.2f %20s",
+        WRITE("CISPEP%4d %3.3s%2s %5s   %3.3s%2s %5s %9s %12.2f %20s",
               ++counter,
               cispep.partner_c.res_id.name.c_str(),
               cispep.partner_c.chain_name.c_str(),
               write_seq_id(cispep.partner_c.res_id.seqid).data(),
               cispep.partner_n.res_id.name.c_str(),
               cispep.partner_n.chain_name.c_str(),
               write_seq_id(cispep.partner_n.res_id.seqid).data(),
@@ -653,16 +661,15 @@
   check_if_structure_can_be_written_as_pdb(st);
   write_header(st, os, opt);
   write_atoms(st, os, opt);
   char buf[88];
   WRITE("%-80s", "END");
 }
 
-void write_minimal_pdb(const Structure& st, std::ostream& os,
-                       PdbWriteOptions opt) {
+void write_minimal_pdb(const Structure& st, std::ostream& os, PdbWriteOptions opt) {
   check_if_structure_can_be_written_as_pdb(st);
   write_cryst1(st, os);
   write_ncs(st, os);
   write_atoms(st, os, opt);
 }
 
 #undef WRITE
```

### Comparing `gemmi-0.6.1/src/topo.cpp` & `gemmi-0.6.2/src/topo.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,32 @@
   for (int n = 0; monlib.get_link(cl.id) != nullptr; ++n)
     cl.id.replace(orig_len, cl.id.size(), std::to_string(n));
 
   auto it = monlib.links.emplace(cl.id, cl);
   return it.first->first;
 }
 
+static const ChemLink* setup_link_if_matches(Topo::Link& link, const MonLib& monlib,
+                                             const std::string& atom1,
+                                             const std::string& atom2) {
+  bool invert;
+  const ChemLink* match = nullptr;
+  std::tie(match, invert, link.aliasing1, link.aliasing2) =
+    monlib.match_link(*link.res1, atom1, link.alt1, *link.res2, atom2, link.alt2);
+  if (match) {
+    link.link_id = match->id;
+    if (invert) {
+      std::swap(link.res1, link.res2);
+      std::swap(link.alt1, link.alt2);
+      std::swap(link.aliasing1, link.aliasing2);
+    }
+  }
+  return match;
+}
+
 static void add_polymer_links(PolymerType polymer_type,
                               const Topo::ResInfo& ri1,
                               Topo::ResInfo& ri2,
                               MonLib* monlib) {
   Topo::Link link;
   link.res1 = ri1.res;
   link.res2 = ri2.res;
@@ -220,18 +238,19 @@
               if (n_terminus_group == ChemComp::Group::PPeptide)
                 link.link_id = link.is_cis ? "PCIS" : "PTRANS";
               else if (n_terminus_group == ChemComp::Group::MPeptide)
                 link.link_id = link.is_cis ? "NMCIS" : "NMTRANS";
               else
                 link.link_id = link.is_cis ? "CIS" : "TRANS";
             } else if (monlib) {
-              link.link_id = add_auto_chemlink(*monlib,
-                                               ri1.res->name, c,
-                                               ri2.res->name, n,
-                                               1.34, 0.04);
+              if (!setup_link_if_matches(link, *monlib, c, n))
+                link.link_id = add_auto_chemlink(*monlib,
+                                                 ri1.res->name, c,
+                                                 ri2.res->name, n,
+                                                 1.34, 0.04);
             }
             ri2.prev.push_back(link);
           }
       }
 
   } else if (is_polynucleotide(polymer_type)) {
     std::string o3p = "O3'";
@@ -262,21 +281,23 @@
       if (a1.name == o3p && a1.element == El::O) {
         for (const Atom& a2 : ri2.res->atoms)
           if (a2.name == p && a2.element == El::P &&
               (a2.altloc == a1.altloc || a2.altloc == '\0' || a1.altloc == '\0') &&
               in_nucleotide_bond_distance(&a1, &a2)) {
             link.alt1 = a1.altloc;
             link.alt2 = a2.altloc;
-            if (groups_ok)
+            if (groups_ok) {
               link.link_id = "p";
-            else if (monlib)
-              link.link_id = add_auto_chemlink(*monlib,
-                                               ri1.res->name, o3p,
-                                               ri2.res->name, p,
-                                               1.606, 0.02);
+            } else if (monlib) {
+              if (!setup_link_if_matches(link, *monlib, o3p, p))
+                link.link_id = add_auto_chemlink(*monlib,
+                                                 ri1.res->name, o3p,
+                                                 ri2.res->name, p,
+                                                 1.606, 0.02);
+            }
             ri2.prev.push_back(link);
           }
     }
   }
 
   if (ri2.prev.empty()) {
     link.link_id = "gap";
@@ -615,27 +636,19 @@
                                conn.partner1.atom_name, extra.aliasing1) ||
         !atom_match_with_alias(match->rt.bonds[0].id2.atom,
                                conn.partner2.atom_name, extra.aliasing2)) {
       err("link from the monomer library does not match: " + conn.link_id);
       return;
     }
   } else {
-    bool invert;
     // we don't have link_id - use the best matching link (if any)
-    std::tie(match, invert, extra.aliasing1, extra.aliasing2) =
-      monlib.match_link(*extra.res1, conn.partner1.atom_name, extra.alt1,
-                        *extra.res2, conn.partner2.atom_name, extra.alt2);
-    if (match) {
+    match = setup_link_if_matches(extra, monlib,
+                                  conn.partner1.atom_name, conn.partner2.atom_name);
+    if (match)
       conn.link_id = match->id;
-      if (invert) {
-        std::swap(extra.res1, extra.res2);
-        std::swap(extra.alt1, extra.alt2);
-        std::swap(extra.aliasing1, extra.aliasing2);
-      }
-    }
   }
 
   // If a polymer link is also given in LINK/struct_conn,
   // use only one of them. If LINK has explicit name (ccp4_link_id),
   // or if it matches residue-specific link from monomer library, use it;
   // otherwise, LINK is repetition of TRANS/CIS, so ignore LINK.
   if (Link* polymer_link = find_polymer_link(conn.partner1, conn.partner2)) {
@@ -762,38 +775,40 @@
   float occ;
 };
 using NeighMap = std::unordered_multimap<int, Neigh>;
 
 // Assumes no hydrogens in the residue.
 // Position and serial number are not assigned for new atoms.
 void add_hydrogens_without_positions(Topo::ResInfo& ri, const NeighMap& neighbors) {
-  Residue& res = *ri.res;
+  std::vector<Atom>& atoms = ri.res->atoms;
   // Add H atom for each conformation (altloc) of the parent atom and its
   // first neighbors.
-  for (size_t i = 0, size = res.atoms.size(); i != size; ++i) {
-    char parent_alt = res.atoms[i].altloc;
-    float parent_occ = res.atoms[i].occ;
+  for (size_t i = 0, size = atoms.size(); i != size; ++i) {
+    if (atoms[i].calc_flag == CalcFlag::NoHydrogen)
+      continue;
+    char parent_alt = atoms[i].altloc;
+    float parent_occ = atoms[i].occ;
     std::map<char, float> altlocs; // altloc + occupancy
     if (parent_alt == '\0') {
       float max_occ = 1.001f;
-      auto range = neighbors.equal_range(res.atoms[i].serial);
+      auto range = neighbors.equal_range(atoms[i].serial);
       for (auto it = range.first; it != range.second; ++it) {
         const Neigh& neigh = it->second;
         if (neigh.alt && altlocs.count(neigh.alt) == 0 && neigh.occ < max_occ) {
           altlocs.emplace(neigh.alt, neigh.occ * parent_occ);
           max_occ -= neigh.occ;
         }
       }
     }
     if (altlocs.empty())
       altlocs.emplace(parent_alt, parent_occ);
     const ChemComp& cc = ri.get_final_chemcomp(parent_alt);
     for (const Restraints::Bond& bond : cc.rt.bonds) {
-      // res.atoms may get re-allocated, so we can't set parent earlier
-      const Atom& parent = res.atoms[i];
+      // atoms may get re-allocated, so we can't set parent earlier
+      const Atom& parent = atoms[i];
       assert(!parent.is_hydrogen());
       const Restraints::AtomId* atom_id = bond.other(parent.name);
       if (!atom_id)
         continue;
       auto it = cc.find_atom(atom_id->atom);
       if (it == cc.atoms.end())
         fail("inconsistent _chem_comp " + cc.name);
@@ -803,15 +818,15 @@
         atom.element = it->el;
         // calc_flag will be changed to Calculated when the position is set
         atom.calc_flag = CalcFlag::Dummy;
         atom.b_iso = parent.b_iso;
         for (auto alt_occ : altlocs) {
           atom.altloc = alt_occ.first;
           atom.occ = alt_occ.second;
-          res.atoms.push_back(atom);
+          atoms.push_back(atom);
         }
       }
     }
   }
 }
 
 NeighMap prepare_neighbor_data(Topo& topo, const MonLib& monlib) {
```

### Comparing `gemmi-0.6.1/src/xds_ascii.cpp` & `gemmi-0.6.2/src/xds_ascii.cpp`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/third_party/zlib/adler32.c` & `gemmi-0.6.2/third_party/zlib/adler32.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/third_party/zlib/crc32.c` & `gemmi-0.6.2/third_party/zlib/crc32.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/third_party/zlib/crc32.h` & `gemmi-0.6.2/third_party/zlib/crc32.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/third_party/zlib/gzguts.h` & `gemmi-0.6.2/third_party/zlib/gzguts.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/third_party/zlib/gzlib.c` & `gemmi-0.6.2/third_party/zlib/gzlib.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/third_party/zlib/gzread.c` & `gemmi-0.6.2/third_party/zlib/gzread.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/third_party/zlib/inffast.c` & `gemmi-0.6.2/third_party/zlib/inffast.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/third_party/zlib/inffixed.h` & `gemmi-0.6.2/third_party/zlib/inffixed.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/third_party/zlib/inflate.c` & `gemmi-0.6.2/third_party/zlib/inflate.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/third_party/zlib/inflate.h` & `gemmi-0.6.2/third_party/zlib/inflate.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/third_party/zlib/inftrees.c` & `gemmi-0.6.2/third_party/zlib/inftrees.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/third_party/zlib/inftrees.h` & `gemmi-0.6.2/third_party/zlib/inftrees.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/third_party/zlib/license` & `gemmi-0.6.2/third_party/zlib/license`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/third_party/zlib/zconf.h` & `gemmi-0.6.2/third_party/zlib/zconf.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/third_party/zlib/zlib.h` & `gemmi-0.6.2/third_party/zlib/zlib.h`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/third_party/zlib/zutil.c` & `gemmi-0.6.2/third_party/zlib/zutil.c`

 * *Files identical despite different names*

### Comparing `gemmi-0.6.1/third_party/zlib/zutil.h` & `gemmi-0.6.2/third_party/zlib/zutil.h`

 * *Files identical despite different names*

