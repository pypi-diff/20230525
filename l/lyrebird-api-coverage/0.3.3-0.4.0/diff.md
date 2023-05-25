# Comparing `tmp/lyrebird-api-coverage-0.3.3.tar.gz` & `tmp/lyrebird-api-coverage-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lyrebird-api-coverage-0.3.3.tar", last modified: Fri Dec  2 12:24:15 2022, max compression
+gzip compressed data, was "dist/lyrebird-api-coverage-0.4.0.tar", last modified: Thu May 25 13:32:36 2023, max compression
```

## Comparing `lyrebird-api-coverage-0.3.3.tar` & `lyrebird-api-coverage-0.4.0.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:24:15.000000 lyrebird-api-coverage-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2022-12-02 12:24:15.000000 lyrebird-api-coverage-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:24:15.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:24:15.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/client/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/client/event_subscibe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/client/filter_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/client/format_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/client/jsonscheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/client/load_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/client/merge_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/client/report.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/client/url_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:24:15.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/default_conf/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/default_conf/base.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/default_conf/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      165 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/default_conf/filter_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:24:15.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:24:15.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/css/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/css/app.0233d703.css
--rw-r--r--   0 runner    (1001) docker     (123)   377184 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/css/chunk-vendors.129fc3b2.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:24:15.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    56484 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/fonts/codicon.a609dc0f.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    82216 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/fonts/ionicons.143146fa.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   197740 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/fonts/ionicons.99ac3308.woff
--rw-r--r--   0 runner    (1001) docker     (123)   197664 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/fonts/ionicons.d535a25a.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:24:15.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/img/
--rw-r--r--   0 runner    (1001) docker     (123)   555353 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/img/ionicons.a2c4a261.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:24:15.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/
--rw-r--r--   0 runner    (1001) docker     (123)    23802 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/app.3e82be3c.js
--rw-r--r--   0 runner    (1001) docker     (123)   704862 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-0b65ffb6.4d11c55b.js
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0a3577.e9944055.js
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0a43df.673ca57f.js
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0aa90c.bb4da71a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0aab07.b30b422d.js
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0abc00.ae916ae6.js
--rw-r--r--   0 runner    (1001) docker     (123)    18269 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0ae937.5dfe330b.js
--rw-r--r--   0 runner    (1001) docker     (123)    18627 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0aeb45.d6889297.js
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0af08c.d2b0fda9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0afa49.75ef7177.js
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0b2762.04d401e4.js
--rw-r--r--   0 runner    (1001) docker     (123)    17660 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0b6187.044b0232.js
--rw-r--r--   0 runner    (1001) docker     (123)      876 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0ba136.3f3f68c3.js
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0bb267.de956ef3.js
--rw-r--r--   0 runner    (1001) docker     (123)    11812 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0bcec1.bb1e0dcf.js
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0bdf38.4ed8de90.js
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0bff92.0d3c28c2.js
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0c0494.089a3f44.js
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0c0a09.c01173ca.js
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0c4313.2d2e16b9.js
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0c46d1.1547c887.js
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0c512b.227874be.js
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0cf16e.d7823e95.js
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0d056d.50e40d69.js
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0d0645.00f3a9b7.js
--rw-r--r--   0 runner    (1001) docker     (123)    16969 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0d2f22.deddf49a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0d61fd.c87f9452.js
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0d7e63.4e91911e.js
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0e1b57.2f0a463f.js
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0e1fbe.0fae86fb.js
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0e22d6.9822404b.js
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0e542a.00ed19f2.js
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0e57ec.9fc2995d.js
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0e6553.d113a072.js
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0e6c86.af95b5ef.js
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0ea098.47e7590e.js
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0f0a11.2c633a92.js
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d208ac5.2d741554.js
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d209408.fbdaeb7f.js
--rw-r--r--   0 runner    (1001) docker     (123)    14526 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d20f745.9eec45ed.js
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d20ff23.99d59ed8.js
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d2138c7.b8ff4f70.js
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d216f3b.7cfad27f.js
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d217e5b.b2ad3334.js
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d21b84a.59c92178.js
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d21dcd2.11000279.js
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d21f327.bb87e8ce.js
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d2214b3.ed0b709c.js
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d221799.af1ee392.js
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d221814.725c56d8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d221a34.c98683c5.js
--rw-r--r--   0 runner    (1001) docker     (123)    22952 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d22502a.40401bee.js
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d226775.1ecaef90.js
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d229411.f42e99d7.js
--rw-r--r--   0 runner    (1001) docker     (123)     8531 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d2295e9.cf55c1f6.js
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d22c171.b06a7e37.js
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d22c2b8.160bc0cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d22ca58.01faff7d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d2311f7.12260884.js
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d237ee7.6655aefa.js
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d238465.270fbbc6.js
--rw-r--r--   0 runner    (1001) docker     (123)   414560 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-30597b4a.ab012e90.js
--rw-r--r--   0 runner    (1001) docker     (123)     6091 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-7532b3ea.a9fe4911.js
--rw-r--r--   0 runner    (1001) docker     (123)   109437 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-e13e4362.9cc9d271.js
--rw-r--r--   0 runner    (1001) docker     (123)  3117005 2022-12-02 12:24:00.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-vendors.324e53e6.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:24:15.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/handlers/base_source_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/handlers/filter_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/handlers/import_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/handlers/result_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:24:15.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2022-12-02 12:24:14.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2022-12-02 12:24:15.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-02 12:24:14.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-02 12:24:14.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-02 12:24:14.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       58 2022-12-02 12:24:14.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-02 12:24:14.000000 lyrebird-api-coverage-0.3.3/lyrebird_api_coverage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-02 12:24:15.000000 lyrebird-api-coverage-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2022-12-02 12:22:45.000000 lyrebird-api-coverage-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/event_subscibe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/filter_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/format_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/jsonscheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/load_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/merge_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/url_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/default_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/default_conf/base.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/default_conf/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/default_conf/filter_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/css/app.964cc419.css
+-rw-r--r--   0 runner    (1001) docker     (123)   377184 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/css/chunk-vendors.129fc3b2.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    56484 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/fonts/codicon.a609dc0f.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    82216 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/fonts/ionicons.143146fa.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   197740 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/fonts/ionicons.99ac3308.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   197664 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/fonts/ionicons.d535a25a.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   555353 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/img/ionicons.a2c4a261.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    24092 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/app.6994bbbd.js
+-rw-r--r--   0 runner    (1001) docker     (123)   704862 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-0b65ffb6.4d11c55b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0a3577.e9944055.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0a43df.673ca57f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0aa90c.bb4da71a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0aab07.b30b422d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0abc00.ae916ae6.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18269 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0ae937.5dfe330b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18627 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0aeb45.d6889297.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0af08c.d2b0fda9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0afa49.75ef7177.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0b2762.04d401e4.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17660 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0b6187.044b0232.js
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0ba136.3f3f68c3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0bb267.de956ef3.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11812 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0bcec1.bb1e0dcf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0bdf38.4ed8de90.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0bff92.0d3c28c2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0c0494.089a3f44.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0c0a09.c01173ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0c4313.2d2e16b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0c46d1.1547c887.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0c512b.227874be.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0cf16e.d7823e95.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0d056d.50e40d69.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0d0645.00f3a9b7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16969 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0d2f22.deddf49a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0d61fd.c87f9452.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0d7e63.4e91911e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e1b57.2f0a463f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e1fbe.0fae86fb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e22d6.9822404b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e542a.00ed19f2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e57ec.9fc2995d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e6553.d113a072.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e6c86.af95b5ef.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0ea098.47e7590e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0f0a11.2c633a92.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d208ac5.2d741554.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d209408.fbdaeb7f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d20f745.9eec45ed.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d20ff23.99d59ed8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d2138c7.b8ff4f70.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d216f3b.7cfad27f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d217e5b.b2ad3334.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d21b84a.59c92178.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d21dcd2.11000279.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d21f327.bb87e8ce.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d2214b3.ed0b709c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d221799.af1ee392.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d221814.725c56d8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d221a34.c98683c5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22952 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d22502a.40401bee.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d226775.1ecaef90.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d229411.f42e99d7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d2295e9.cf55c1f6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d22c171.b06a7e37.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d22c2b8.160bc0cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d22ca58.01faff7d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d2311f7.12260884.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d237ee7.6655aefa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d238465.270fbbc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)   414560 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-30597b4a.ab012e90.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-7532b3ea.a9fe4911.js
+-rw-r--r--   0 runner    (1001) docker     (123)   109437 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-e13e4362.9cc9d271.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3117005 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-vendors.324e53e6.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/handlers/base_source_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/handlers/filter_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/handlers/import_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/handlers/result_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/setup.py
```

### Comparing `lyrebird-api-coverage-0.3.3/PKG-INFO` & `lyrebird-api-coverage-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyrebird-api-coverage
-Version: 0.3.3
+Version: 0.4.0
 Summary: UNKNOWN
 Home-page: https://github.com/meituan/lyrebird-api-coverage
 Author: HBQA
 License: UNKNOWN
 Description: # Lyrebird Plugin API-Coverage
         
         [![Build Status](https://travis-ci.org/meituan/lyrebird-api-coverage.svg?branch=master)](https://travis-ci.org/meituan/lyrebird-api-coverage)
```

### Comparing `lyrebird-api-coverage-0.3.3/README.md` & `lyrebird-api-coverage-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/api.py` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 def generate(data):
     rtext = json.dumps(data)
     yield rtext
 
 # 获取内存里保存的测试结果API
 # /getTest
 def get_test_data():
-    return Response(stream_with_context(generate({'test_data': app_context.merge_list})), content_type='application/json')
+    return context.make_ok_response(test_data=app_context.merge_list)
 
 # 获取内存里保存的测试覆盖率信息
 # /getCoverage
 def get_coverage():
-    return Response(stream_with_context(generate(app_context.coverage)), content_type='application/json')
+    return context.make_ok_response(coverage = app_context.coverage)
 
 # 保存测试数据在本地
 #  /saveResult
 def save_result():
     # 传入文件名
     filename = request.form.get('result_name')
     ResultHandler().save_result(filename)
```

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/client/config.py` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/config.py`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/client/context.py` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,11 +33,15 @@
         self.user_info = {}
         # 记录请求最后的时间，避免频繁emit io消息
         self.endtime = 0
         # 记录上次coverage变化的时间，避免频繁emit io消息
         self.covtime = 0
         # 时间间隔，每隔指定时间触发1次socket io消息，防止刷新频繁
         self.SOCKET_PUSH_INTERVAL = 1
+        # 是否使用接口请求实时base数据
+        self.is_api_base_data = False
+        # category信息
+        self.category = ''
 
 
 # 单例模式
 app_context = Context()
```

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/client/filter_url.py` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/filter_url.py`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/client/format_url.py` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/format_url.py`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/client/jsonscheme.py` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/jsonscheme.py`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/client/load_base.py` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/handlers/filter_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 import codecs
-import hashlib
 import json
-import lyrebird
-from lyrebird.log import get_logger
 import os
-
+import lyrebird
+from lyrebird.mock import context
 from lyrebird_api_coverage.client.context import app_context
+from lyrebird_api_coverage.client.jsonscheme import check_filter_schema
 
-PLUGINS_CONF_DIR = lyrebird.get_plugin_storage()
-DEFAULT_BASE = os.path.join(PLUGINS_CONF_DIR, 'base.json')
 CURRENT_DIR = os.path.dirname(__file__)
+PLUGIN_DIR = lyrebird.get_plugin_storage()
+FILTER_CONF = os.path.join(PLUGIN_DIR, 'filter_conf.json')
 
 
-def get_file_sha1(path):
-    with open(path, 'rb') as f:
-        sha1obj = hashlib.sha1()
-        sha1obj.update(f.read())
-        hash_sha1 = sha1obj.hexdigest()
-        return hash_sha1
-
-
-def auto_load_base():
-    lyrebird_conf = lyrebird.context.application.conf
-    # 读取指定base文件，写入到base.json
-    if lyrebird_conf.get('hunter.base'):
-        base_path = lyrebird_conf.get('hunter.base')
-        base = codecs.open(base_path, 'r', 'utf-8').read()
-        f = codecs.open(DEFAULT_BASE, 'w', 'utf-8')
-        f.write(base)
-        f.close()
-        app_context.base_sha1 = get_file_sha1(DEFAULT_BASE)
-        return json.loads(base)
-    # 通过本地默认base文件获取base
-    elif not os.path.exists(DEFAULT_BASE):
-        copy_file(DEFAULT_BASE)
-    with codecs.open(DEFAULT_BASE, 'r', 'utf-8') as f:
-        json_obj = json.load(f)
-        app_context.base_sha1 = get_file_sha1(DEFAULT_BASE)
-        return json_obj
-
-
-def copy_file(target_path):
-    os.path.abspath(os.path.join(CURRENT_DIR, '..', './default_conf/base.json'))
-    f_from = codecs.open(os.path.abspath(os.path.join(CURRENT_DIR, '..', './default_conf/base.json')), 'r', 'utf-8')
-    f_to = codecs.open(target_path, 'w', 'utf-8')
-    f_to.write(f_from.read())
-    f_to.close()
-    f_from.close()
+'''
+过滤处理器
+'''
+
+class FilterHandler:
+    def init_filter_conf(self):
+        if not os.path.exists(FILTER_CONF):
+            self.copy_conf_file(FILTER_CONF)
+
+    def copy_conf_file(self, target_path):
+        os.path.abspath(os.path.join(CURRENT_DIR, '..', './default_conf/filter_config.json'))
+        f_from = codecs.open(os.path.abspath(os.path.join(CURRENT_DIR, '..', './default_conf/filter_config.json')), 'r',
+                             'utf-8')
+        f_to = codecs.open(target_path, 'w', 'utf-8')
+        f_to.write(f_from.read())
+        f_to.close()
+        f_from.close()
+
+    def get_filer_conf(self):
+        self.init_filter_conf()
+        try:
+            json_obj = json.loads(codecs.open(FILTER_CONF, 'r', 'utf-8').read())
+            check_filter_schema(json_obj)
+            app_context.filter_dic = json_obj
+            msg = json_obj
+        except Exception as e:
+            msg = '过滤请求的配置文件格式有误:' + e.__getattribute__('message')
+        return msg
+
+    def save_filer_conf(self, conf_obj):
+        self.init_filter_conf()
+        try:
+            check_filter_schema(conf_obj)
+            f = codecs.open(FILTER_CONF, 'w', 'utf-8')
+            f.write(json.dumps(conf_obj))
+            f.close()
+            # 配置保存后当时生效
+            app_context.filter_dic = conf_obj
+            return context.make_ok_response()
+        except Exception as e:
+            msg = '过滤请求的配置文件格式有误:' + e.__getattribute__('message')
+            lyrebird.publish('api_coverage', 'error', name='set_filter')
+            return context.make_fail_response(msg)
```

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/client/merge_algorithm.py` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/merge_algorithm.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,65 +31,96 @@
         app_context.base_list = list(map(lambda x: x.get('url'), json_obj.get('api_list')))
 
     def init_basedata_handler(self, dic):
         # for k, v in dic.items():
         #     url_dic = {'url': k, 'desc': v.get('desc'), 'priority': v.get('priority'), 'count': 0, 'status': 0,
         #                'org': []}
         #     app_context.merge_list.append(url_dic)
-        dict2 = {'count': 0, 'status': 0, 'id': ''}
-        for item in dic.get('api_list'):
-            # 处理带参数的情况
-            if '?' in item['url']:
-                path = item['url'].split('?')[0].lower()
-                params = item['url'].split('?')[1].split('&')
-                param_dic = {}
-                for i in params:
-                    key = i.split('=')[0]
-                    val = i.split('=')[1]
-                    param_dic[key] = val
-
-                if app_context.path_param_dic.get(path):
-                    app_context.path_param_dic[path].append({'url': item['url'], 'params': param_dic,
-                                                             'url_base': format_url.format_api_source(
-                                                                 item.get('url')).lower()})
-                else:
-                    app_context.path_param_dic[path] = [{'url': item['url'], 'params': param_dic,
-                                                         'url_base': format_url.format_api_source(
-                                                             item.get('url')).lower()}]
-
-            # format base源 同时变成大小写归一化，变小写
-            item['url'] = format_url.format_api_source(item.get('url')).lower()
-            item.update(dict2)
-            app_context.merge_list.append(item)
+        if app_context.is_api_base_data:
+            # 如果接口获取base数据，同步merge_list内容
+            app_context.merge_list = dic.get('api_list')
+        else:
+            dict2 = {'count': 0, 'status': 0, 'id': ''}
+            for item in dic.get('api_list'):
+                # 处理带参数的情况
+                if '?' in item['url']:
+                    path = item['url'].split('?')[0].lower()
+                    params = item['url'].split('?')[1].split('&')
+                    param_dic = {}
+                    for i in params:
+                        key = i.split('=')[0]
+                        val = i.split('=')[1]
+                        param_dic[key] = val
+
+                    if app_context.path_param_dic.get(path):
+                        app_context.path_param_dic[path].append({'url': item['url'], 'params': param_dic,
+                                                                'url_base': format_url.format_api_source(
+                                                                    item.get('url')).lower()})
+                    else:
+                        app_context.path_param_dic[path] = [{'url': item['url'], 'params': param_dic,
+                                                            'url_base': format_url.format_api_source(
+                                                                item.get('url')).lower()}]
+                # format base源 同时变成大小写归一化，变小写
+                item['url'] = format_url.format_api_source(item.get('url')).lower()
+                item.update(dict2)
+                app_context.merge_list.append(item)
 
-    def merge_handler_new(self, user_url, path_id):
+    def merge_handler_new(self, user_url, path_id, category):
         """
         status=0 base中包含未覆盖，status=1 base中包含已覆盖，status=2 base中不包含且覆盖到的;
         path_id表示URL的handler_context的唯一标识，查看详情用
         """
 
         # 在list中筛选出想要的数据,筛选结果直接取0即可
         specific_filter_list = list(filter(lambda x: x.get('url') == user_url, app_context.merge_list))
 
         # 判断筛选出来的list是否为空,即是否在list中存在
         if specific_filter_list:
             specific_dic = specific_filter_list[0]
             # 移除掉对应的数据为插入index0的位置做前置处理
             app_context.merge_list.remove(specific_dic)
-            # 做业务处理
-            if specific_dic['status'] == 0:
-                specific_dic['status'] = 1
-                # 把首次覆盖到的API,放入user_list里面
-                app_context.user_list.append(user_url)
+            # 根据数据源,进行业务处理
+            if app_context.is_api_base_data:
+                category_dic = specific_dic.get('category')
+                for p in category_dic:
+                    if category == p['name'] and p['status'] == 0:
+                        p['status'] = 1
+                        p['count'] += 1
+                        p['id'] = path_id
+                if specific_dic['status'] == 0:
+                    specific_dic['status'] = 1
+                    # 把首次覆盖到的API,放入user_list里面
+                    app_context.user_list.append(user_url)
+            else:
+                # 非接口获取base数据
+                if specific_dic['status'] == 0:
+                    specific_dic['status'] = 1
+                    # 把首次覆盖到的API,放入user_list里面
+                    app_context.user_list.append(user_url)
             # count +1
             specific_dic['count'] += 1  # 插入原始url  # specific_dic['org'].append(org_url)
             specific_dic['id'] = path_id
         else:
-            # specific_dic = {'url': user_url, 'desc': '', 'priority': '', 'count': 1, 'status': 2, 'org': [org_url]}
-            specific_dic = {'url': user_url, 'desc': '', 'priority': None, 'count': 1, 'status': 2, 'id': path_id}
+            if app_context.is_api_base_data:
+                specific_dic = {
+                    'url': user_url,
+                    'desc': '',
+                    'priority': None,
+                    'status': 2,
+                    'count': 1,
+                    'category': []
+                }
+                specific_dic['category'].append({
+                    'id': None,
+                    'name': category,
+                    'status': 2,
+                    'count': 1
+                })
+            else:
+                specific_dic = {'url': user_url, 'desc': '', 'priority': None, 'count': 1, 'status': 2, 'id': path_id}
         # 插入到 index=0 的位置
         app_context.merge_list.insert(0, specific_dic)
 
     def coverage_handler(self):
         """
         总体覆盖率
         """
```

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/client/report.py` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/report.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 from lyrebird_api_coverage.client.context import app_context
-from lyrebird import report
+from lyrebird import publish
 
 """
 上报处理器，用户请求行为上报到ELK中
 ps:需要在lyrebird中设定reporter相关配置
 """
 
 class ReportHandler:
-    def check_url_info(self, url, device_ip):
+    def check_url_info(self, url, device_ip, category):
         specific_list = list(filter(lambda x: x.get('url') == url, app_context.merge_list))
         if specific_list and specific_list[0].get('status') == 1:
             desc = specific_list[0].get('desc')
             count_flag = 1
             priority = specific_list[0].get('priority')
         else:
             desc = 'N/A'
             count_flag = -1
             priority = -1
-        info_dict = {'url': url, 'desc': desc, 'priority': priority, 'count_flag': count_flag,
-                     'business': app_context.business, 'version_name': app_context.version_name,
-                     'version_code': app_context.version_code}
+        info_dict = {
+            'coverage':{
+                'url': url,
+                'desc': desc,
+                'priority': priority,
+                'count_flag': count_flag,
+                'version_name': app_context.version_name,
+                'version_code': app_context.version_code,
+                'category': category
+            }
+        }
         if app_context.info.get(device_ip):
             # 如果有Device信息，就上报device相关的信息
-            info_dict.update(app_context.info.get(device_ip))
+            info_dict['coverage'].update(app_context.info.get(device_ip))
         return info_dict
 
 
 report_handler = ReportHandler()
 
 
-def report_worker(url, device_ip):
-    update_data = report_handler.check_url_info(url, device_ip)
-    update_data.update({"action": "api-coverage", "user_info": app_context.user_info})
-    report(update_data)
+def report_worker(url, device_ip, category):
+    update_data = report_handler.check_url_info(url, device_ip, category)
+    publish('coverage', update_data)
```

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/client/url_compare.py` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/url_compare.py`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/css/chunk-vendors.129fc3b2.css` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/css/chunk-vendors.129fc3b2.css`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/fonts/codicon.a609dc0f.ttf` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/fonts/codicon.a609dc0f.ttf`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/fonts/ionicons.143146fa.woff2` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/fonts/ionicons.143146fa.woff2`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/fonts/ionicons.99ac3308.woff` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/fonts/ionicons.99ac3308.woff`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/fonts/ionicons.d535a25a.ttf` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/fonts/ionicons.d535a25a.ttf`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/img/ionicons.a2c4a261.svg` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/img/ionicons.a2c4a261.svg`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/index.html` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><meta charset=utf-8><meta http-equiv=X-UA-Compatible content="IE=edge"><meta name=viewport content="width=device-width,initial-scale=1"><title>Vue App</title><link href=dist/js/chunk-0b65ffb6.4d11c55b.js rel=prefetch><link href=dist/js/chunk-2d0a3577.e9944055.js rel=prefetch><link href=dist/js/chunk-2d0a43df.673ca57f.js rel=prefetch><link href=dist/js/chunk-2d0aa90c.bb4da71a.js rel=prefetch><link href=dist/js/chunk-2d0aab07.b30b422d.js rel=prefetch><link href=dist/js/chunk-2d0abc00.ae916ae6.js rel=prefetch><link href=dist/js/chunk-2d0ae937.5dfe330b.js rel=prefetch><link href=dist/js/chunk-2d0aeb45.d6889297.js rel=prefetch><link href=dist/js/chunk-2d0af08c.d2b0fda9.js rel=prefetch><link href=dist/js/chunk-2d0afa49.75ef7177.js rel=prefetch><link href=dist/js/chunk-2d0b2762.04d401e4.js rel=prefetch><link href=dist/js/chunk-2d0b6187.044b0232.js rel=prefetch><link href=dist/js/chunk-2d0ba136.3f3f68c3.js rel=prefetch><link href=dist/js/chunk-2d0bb267.de956ef3.js rel=prefetch><link href=dist/js/chunk-2d0bcec1.bb1e0dcf.js rel=prefetch><link href=dist/js/chunk-2d0bdf38.4ed8de90.js rel=prefetch><link href=dist/js/chunk-2d0bff92.0d3c28c2.js rel=prefetch><link href=dist/js/chunk-2d0c0494.089a3f44.js rel=prefetch><link href=dist/js/chunk-2d0c0a09.c01173ca.js rel=prefetch><link href=dist/js/chunk-2d0c4313.2d2e16b9.js rel=prefetch><link href=dist/js/chunk-2d0c46d1.1547c887.js rel=prefetch><link href=dist/js/chunk-2d0c512b.227874be.js rel=prefetch><link href=dist/js/chunk-2d0cf16e.d7823e95.js rel=prefetch><link href=dist/js/chunk-2d0d056d.50e40d69.js rel=prefetch><link href=dist/js/chunk-2d0d0645.00f3a9b7.js rel=prefetch><link href=dist/js/chunk-2d0d2f22.deddf49a.js rel=prefetch><link href=dist/js/chunk-2d0d61fd.c87f9452.js rel=prefetch><link href=dist/js/chunk-2d0d7e63.4e91911e.js rel=prefetch><link href=dist/js/chunk-2d0e1b57.2f0a463f.js rel=prefetch><link href=dist/js/chunk-2d0e1fbe.0fae86fb.js rel=prefetch><link href=dist/js/chunk-2d0e22d6.9822404b.js rel=prefetch><link href=dist/js/chunk-2d0e542a.00ed19f2.js rel=prefetch><link href=dist/js/chunk-2d0e57ec.9fc2995d.js rel=prefetch><link href=dist/js/chunk-2d0e6553.d113a072.js rel=prefetch><link href=dist/js/chunk-2d0e6c86.af95b5ef.js rel=prefetch><link href=dist/js/chunk-2d0ea098.47e7590e.js rel=prefetch><link href=dist/js/chunk-2d0f0a11.2c633a92.js rel=prefetch><link href=dist/js/chunk-2d208ac5.2d741554.js rel=prefetch><link href=dist/js/chunk-2d209408.fbdaeb7f.js rel=prefetch><link href=dist/js/chunk-2d20f745.9eec45ed.js rel=prefetch><link href=dist/js/chunk-2d20ff23.99d59ed8.js rel=prefetch><link href=dist/js/chunk-2d2138c7.b8ff4f70.js rel=prefetch><link href=dist/js/chunk-2d216f3b.7cfad27f.js rel=prefetch><link href=dist/js/chunk-2d217e5b.b2ad3334.js rel=prefetch><link href=dist/js/chunk-2d21b84a.59c92178.js rel=prefetch><link href=dist/js/chunk-2d21dcd2.11000279.js rel=prefetch><link href=dist/js/chunk-2d21f327.bb87e8ce.js rel=prefetch><link href=dist/js/chunk-2d2214b3.ed0b709c.js rel=prefetch><link href=dist/js/chunk-2d221799.af1ee392.js rel=prefetch><link href=dist/js/chunk-2d221814.725c56d8.js rel=prefetch><link href=dist/js/chunk-2d221a34.c98683c5.js rel=prefetch><link href=dist/js/chunk-2d22502a.40401bee.js rel=prefetch><link href=dist/js/chunk-2d226775.1ecaef90.js rel=prefetch><link href=dist/js/chunk-2d229411.f42e99d7.js rel=prefetch><link href=dist/js/chunk-2d2295e9.cf55c1f6.js rel=prefetch><link href=dist/js/chunk-2d22c171.b06a7e37.js rel=prefetch><link href=dist/js/chunk-2d22c2b8.160bc0cf.js rel=prefetch><link href=dist/js/chunk-2d22ca58.01faff7d.js rel=prefetch><link href=dist/js/chunk-2d2311f7.12260884.js rel=prefetch><link href=dist/js/chunk-2d237ee7.6655aefa.js rel=prefetch><link href=dist/js/chunk-2d238465.270fbbc6.js rel=prefetch><link href=dist/js/chunk-30597b4a.ab012e90.js rel=prefetch><link href=dist/js/chunk-7532b3ea.a9fe4911.js rel=prefetch><link href=dist/js/chunk-e13e4362.9cc9d271.js rel=prefetch><link href=dist/css/app.0233d703.css rel=preload as=style><link href=dist/css/chunk-vendors.129fc3b2.css rel=preload as=style><link href=dist/js/app.3e82be3c.js rel=preload as=script><link href=dist/js/chunk-vendors.324e53e6.js rel=preload as=script><link href=dist/css/chunk-vendors.129fc3b2.css rel=stylesheet><link href=dist/css/app.0233d703.css rel=stylesheet></head><body><div id=app></div><script src=dist/js/chunk-vendors.324e53e6.js></script><script src=dist/js/app.3e82be3c.js></script></body></html>
+<!DOCTYPE html><html><head><meta charset=utf-8><meta http-equiv=X-UA-Compatible content="IE=edge"><meta name=viewport content="width=device-width,initial-scale=1"><title>Vue App</title><link href=dist/js/chunk-0b65ffb6.4d11c55b.js rel=prefetch><link href=dist/js/chunk-2d0a3577.e9944055.js rel=prefetch><link href=dist/js/chunk-2d0a43df.673ca57f.js rel=prefetch><link href=dist/js/chunk-2d0aa90c.bb4da71a.js rel=prefetch><link href=dist/js/chunk-2d0aab07.b30b422d.js rel=prefetch><link href=dist/js/chunk-2d0abc00.ae916ae6.js rel=prefetch><link href=dist/js/chunk-2d0ae937.5dfe330b.js rel=prefetch><link href=dist/js/chunk-2d0aeb45.d6889297.js rel=prefetch><link href=dist/js/chunk-2d0af08c.d2b0fda9.js rel=prefetch><link href=dist/js/chunk-2d0afa49.75ef7177.js rel=prefetch><link href=dist/js/chunk-2d0b2762.04d401e4.js rel=prefetch><link href=dist/js/chunk-2d0b6187.044b0232.js rel=prefetch><link href=dist/js/chunk-2d0ba136.3f3f68c3.js rel=prefetch><link href=dist/js/chunk-2d0bb267.de956ef3.js rel=prefetch><link href=dist/js/chunk-2d0bcec1.bb1e0dcf.js rel=prefetch><link href=dist/js/chunk-2d0bdf38.4ed8de90.js rel=prefetch><link href=dist/js/chunk-2d0bff92.0d3c28c2.js rel=prefetch><link href=dist/js/chunk-2d0c0494.089a3f44.js rel=prefetch><link href=dist/js/chunk-2d0c0a09.c01173ca.js rel=prefetch><link href=dist/js/chunk-2d0c4313.2d2e16b9.js rel=prefetch><link href=dist/js/chunk-2d0c46d1.1547c887.js rel=prefetch><link href=dist/js/chunk-2d0c512b.227874be.js rel=prefetch><link href=dist/js/chunk-2d0cf16e.d7823e95.js rel=prefetch><link href=dist/js/chunk-2d0d056d.50e40d69.js rel=prefetch><link href=dist/js/chunk-2d0d0645.00f3a9b7.js rel=prefetch><link href=dist/js/chunk-2d0d2f22.deddf49a.js rel=prefetch><link href=dist/js/chunk-2d0d61fd.c87f9452.js rel=prefetch><link href=dist/js/chunk-2d0d7e63.4e91911e.js rel=prefetch><link href=dist/js/chunk-2d0e1b57.2f0a463f.js rel=prefetch><link href=dist/js/chunk-2d0e1fbe.0fae86fb.js rel=prefetch><link href=dist/js/chunk-2d0e22d6.9822404b.js rel=prefetch><link href=dist/js/chunk-2d0e542a.00ed19f2.js rel=prefetch><link href=dist/js/chunk-2d0e57ec.9fc2995d.js rel=prefetch><link href=dist/js/chunk-2d0e6553.d113a072.js rel=prefetch><link href=dist/js/chunk-2d0e6c86.af95b5ef.js rel=prefetch><link href=dist/js/chunk-2d0ea098.47e7590e.js rel=prefetch><link href=dist/js/chunk-2d0f0a11.2c633a92.js rel=prefetch><link href=dist/js/chunk-2d208ac5.2d741554.js rel=prefetch><link href=dist/js/chunk-2d209408.fbdaeb7f.js rel=prefetch><link href=dist/js/chunk-2d20f745.9eec45ed.js rel=prefetch><link href=dist/js/chunk-2d20ff23.99d59ed8.js rel=prefetch><link href=dist/js/chunk-2d2138c7.b8ff4f70.js rel=prefetch><link href=dist/js/chunk-2d216f3b.7cfad27f.js rel=prefetch><link href=dist/js/chunk-2d217e5b.b2ad3334.js rel=prefetch><link href=dist/js/chunk-2d21b84a.59c92178.js rel=prefetch><link href=dist/js/chunk-2d21dcd2.11000279.js rel=prefetch><link href=dist/js/chunk-2d21f327.bb87e8ce.js rel=prefetch><link href=dist/js/chunk-2d2214b3.ed0b709c.js rel=prefetch><link href=dist/js/chunk-2d221799.af1ee392.js rel=prefetch><link href=dist/js/chunk-2d221814.725c56d8.js rel=prefetch><link href=dist/js/chunk-2d221a34.c98683c5.js rel=prefetch><link href=dist/js/chunk-2d22502a.40401bee.js rel=prefetch><link href=dist/js/chunk-2d226775.1ecaef90.js rel=prefetch><link href=dist/js/chunk-2d229411.f42e99d7.js rel=prefetch><link href=dist/js/chunk-2d2295e9.cf55c1f6.js rel=prefetch><link href=dist/js/chunk-2d22c171.b06a7e37.js rel=prefetch><link href=dist/js/chunk-2d22c2b8.160bc0cf.js rel=prefetch><link href=dist/js/chunk-2d22ca58.01faff7d.js rel=prefetch><link href=dist/js/chunk-2d2311f7.12260884.js rel=prefetch><link href=dist/js/chunk-2d237ee7.6655aefa.js rel=prefetch><link href=dist/js/chunk-2d238465.270fbbc6.js rel=prefetch><link href=dist/js/chunk-30597b4a.ab012e90.js rel=prefetch><link href=dist/js/chunk-7532b3ea.a9fe4911.js rel=prefetch><link href=dist/js/chunk-e13e4362.9cc9d271.js rel=prefetch><link href=dist/css/app.964cc419.css rel=preload as=style><link href=dist/css/chunk-vendors.129fc3b2.css rel=preload as=style><link href=dist/js/app.6994bbbd.js rel=preload as=script><link href=dist/js/chunk-vendors.324e53e6.js rel=preload as=script><link href=dist/css/chunk-vendors.129fc3b2.css rel=stylesheet><link href=dist/css/app.964cc419.css rel=stylesheet></head><body><div id=app></div><script src=dist/js/chunk-vendors.324e53e6.js></script><script src=dist/js/app.6994bbbd.js></script></body></html>
```

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/app.3e82be3c.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/app.6994bbbd.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -738,23 +738,37 @@
                     staticClass: "box box-solid",
                     attrs: {
                         id: "tab"
                     }
                 }, [a("div", {
                     staticClass: "box-body",
                     staticStyle: {
-                        "max-height": "calc(100vh - 100px)",
-                        overflow: "auto"
+                        "max-height": "calc(100vh - 100px) overflow:auto"
                     }
                 }, [a("i-table", {
                     attrs: {
                         stripe: "",
                         columns: e.columns,
                         data: e.showedAPIData
-                    }
+                    },
+                    scopedSlots: e._u([{
+                        key: "category",
+                        fn: function(t) {
+                            var n = t.row;
+                            return [0 !== n.category.length ? a("span", e._l(n.category, (function(t, n) {
+                                return a("span", {
+                                    key: n
+                                }, [1 == t.status ? a("Tag", {
+                                    attrs: {
+                                        color: "green"
+                                    }
+                                }, [e._v(e._s(t.label))]) : e._e()], 1)
+                            })), 0) : e._e()]
+                        }
+                    }])
                 }), a("Modal", {
                     attrs: {
                         title: "Flow Detail",
                         width: "1300"
                     },
                     model: {
                         value: e.isApiDetailModalShow,
@@ -1090,26 +1104,23 @@
                 data: function() {
                     var e = this;
                     return {
                         msg: 1,
                         columns: [{
                             title: "Priority",
                             key: "priority",
-                            sortable: !0,
-                            width: 110
+                            sortable: !0
                         }, {
                             title: "API",
                             key: "url",
-                            sortable: !0,
-                            width: 380
+                            sortable: !0
                         }, {
                             title: "Description",
                             key: "desc",
-                            sortable: !0,
-                            width: 200
+                            sortable: !0
                         }, {
                             title: "Count",
                             key: "count",
                             sortable: !0
                         }, {
                             title: "Status",
                             key: "status",
@@ -1136,14 +1147,19 @@
                                 value: 2
                             }],
                             filterMultiple: !1,
                             filterMethod: function(e, t) {
                                 return 1 === e ? 1 === t.status : 2 === e ? 2 === t.status : 0 === e ? 0 === t.status : null === t.status
                             }
                         }, {
+                            title: "Category",
+                            key: "category",
+                            slot: "category",
+                            sortable: !0
+                        }, {
                             title: "Detail",
                             key: "id",
                             render: function(t, a) {
                                 return a.row.id ? t("i-button", {
                                     props: {
                                         size: "small"
                                     },
@@ -1164,15 +1180,15 @@
                         table_data: [],
                         api_id: "",
                         isApiDetailModalShow: !1
                     }
                 }
             },
             me = pe,
-            be = (a("93d0"), Object(N["a"])(me, H, W, !1, null, "f455e602", null)),
+            be = (a("cd62"), Object(N["a"])(me, H, W, !1, null, "20625c83", null)),
             ve = be.exports,
             ge = {
                 name: "app",
                 created: function() {
                     this.loadBasicDatas(), this.$io.on("apiCoverageBaseData", this.loadBasicDatas)
                 },
                 methods: {
@@ -1292,15 +1308,15 @@
                             title: "loadDetailData error!"
                         })
                     }))
                 },
                 loadCoverageData: function(e) {
                     var t = this;
                     $().then((function(t) {
-                        e.commit("setCoverageData", t.data)
+                        e.commit("setCoverageData", t.data.coverage)
                     })).catch((function() {
                         t.$Notice.open({
                             title: "loadCoverageData error!"
                         })
                     }))
                 },
                 setShowedAPIData: function(e, t) {
@@ -1316,28 +1332,28 @@
         n["default"].config.productionTip = !1, n["default"].use(i.a), n["default"].prototype.$io = s()(), new n["default"]({
             store: _e,
             render: function(e) {
                 return e(ke)
             }
         }).$mount("#app")
     },
+    "59d2": function(e, t, a) {},
     "8f19": function(e, t, a) {},
-    "93d0": function(e, t, a) {
+    "960a": function(e, t, a) {
         "use strict";
-        var n = a("bede"),
+        var n = a("d645"),
             o = a.n(n);
         o.a
     },
-    "960a": function(e, t, a) {
+    cd62: function(e, t, a) {
         "use strict";
-        var n = a("d645"),
+        var n = a("59d2"),
             o = a.n(n);
         o.a
     },
-    bede: function(e, t, a) {},
     d317: function(e, t, a) {
         "use strict";
         var n = a("12e2"),
             o = a.n(n);
         o.a
     },
     d645: function(e, t, a) {},
```

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-0b65ffb6.4d11c55b.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-0b65ffb6.4d11c55b.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0a3577.e9944055.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0a3577.e9944055.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0a43df.673ca57f.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0a43df.673ca57f.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0aa90c.bb4da71a.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0aa90c.bb4da71a.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0aab07.b30b422d.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0aab07.b30b422d.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0abc00.ae916ae6.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0abc00.ae916ae6.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0ae937.5dfe330b.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0ae937.5dfe330b.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0aeb45.d6889297.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0aeb45.d6889297.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0af08c.d2b0fda9.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0af08c.d2b0fda9.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0afa49.75ef7177.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0afa49.75ef7177.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0b2762.04d401e4.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0b2762.04d401e4.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0b6187.044b0232.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0b6187.044b0232.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0ba136.3f3f68c3.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0ba136.3f3f68c3.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0bb267.de956ef3.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0bb267.de956ef3.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0bcec1.bb1e0dcf.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0bcec1.bb1e0dcf.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0bdf38.4ed8de90.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0bdf38.4ed8de90.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0bff92.0d3c28c2.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0bff92.0d3c28c2.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0c0494.089a3f44.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0c0494.089a3f44.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0c0a09.c01173ca.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0c0a09.c01173ca.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0c4313.2d2e16b9.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0c4313.2d2e16b9.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0c46d1.1547c887.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0c46d1.1547c887.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0c512b.227874be.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0c512b.227874be.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0cf16e.d7823e95.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0cf16e.d7823e95.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0d056d.50e40d69.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0d056d.50e40d69.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0d0645.00f3a9b7.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0d0645.00f3a9b7.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0d2f22.deddf49a.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0d2f22.deddf49a.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0d61fd.c87f9452.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0d61fd.c87f9452.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0d7e63.4e91911e.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0d7e63.4e91911e.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0e1b57.2f0a463f.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e1b57.2f0a463f.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0e1fbe.0fae86fb.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e1fbe.0fae86fb.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0e22d6.9822404b.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e22d6.9822404b.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0e542a.00ed19f2.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e542a.00ed19f2.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0e57ec.9fc2995d.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e57ec.9fc2995d.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0e6553.d113a072.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e6553.d113a072.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0e6c86.af95b5ef.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e6c86.af95b5ef.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0ea098.47e7590e.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0ea098.47e7590e.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d0f0a11.2c633a92.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0f0a11.2c633a92.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d208ac5.2d741554.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d208ac5.2d741554.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d209408.fbdaeb7f.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d209408.fbdaeb7f.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d20f745.9eec45ed.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d20f745.9eec45ed.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d20ff23.99d59ed8.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d20ff23.99d59ed8.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d2138c7.b8ff4f70.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d2138c7.b8ff4f70.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d216f3b.7cfad27f.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d216f3b.7cfad27f.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d217e5b.b2ad3334.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d217e5b.b2ad3334.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d21b84a.59c92178.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d21b84a.59c92178.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d21dcd2.11000279.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d21dcd2.11000279.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d21f327.bb87e8ce.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d21f327.bb87e8ce.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d2214b3.ed0b709c.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d2214b3.ed0b709c.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d221799.af1ee392.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d221799.af1ee392.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d221814.725c56d8.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d221814.725c56d8.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d221a34.c98683c5.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d221a34.c98683c5.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d22502a.40401bee.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d22502a.40401bee.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d226775.1ecaef90.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d226775.1ecaef90.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d229411.f42e99d7.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d229411.f42e99d7.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d2295e9.cf55c1f6.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d2295e9.cf55c1f6.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d22c171.b06a7e37.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d22c171.b06a7e37.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d22c2b8.160bc0cf.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d22c2b8.160bc0cf.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d22ca58.01faff7d.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d22ca58.01faff7d.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d2311f7.12260884.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d2311f7.12260884.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d237ee7.6655aefa.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d237ee7.6655aefa.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-2d238465.270fbbc6.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d238465.270fbbc6.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-30597b4a.ab012e90.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-30597b4a.ab012e90.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-7532b3ea.a9fe4911.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-7532b3ea.a9fe4911.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-e13e4362.9cc9d271.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-e13e4362.9cc9d271.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/dist/js/chunk-vendors.324e53e6.js` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-vendors.324e53e6.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/handlers/base_source_handler.py` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/handlers/base_source_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,31 +42,32 @@
 
     '''
     检查base是否符合规则
     '''
     def check_base(self, obj):
         try:
             # 检查base schema
-            check_schema(obj)
+            if not app_context.is_api_base_data:
+                check_schema(obj)
             # 检查url是否有重复项存在
             redundant_items = check_url_redundant(obj)
             if redundant_items:
                 redundant_items_str = '\n'.join(redundant_items)
                 logger.error(
                     f'API-Coverage import API file error: Duplicated API\n'
                     f'{len(redundant_items)} duplicated API:\n'
                     f'{redundant_items_str}\n'
                 )
                 resp = context.make_fail_response('导入API有重复项' + str(redundant_items))
                 lyrebird.publish('api_coverage', 'error', name='import_base')
                 return resp
-            # 获取base内容，解析出base的business等字段
-            filename = obj.get('business') + obj.get('version_name') + '.' + str(obj.get('version_code'))
+            # 获取base内容，解析出base的business等字段 
+            filename = f'''{obj.get('business','')}{obj.get('version_name','')}{obj.get('version_code','')}'''
             app_context.filename = filename
-            app_context.business = obj.get('business')
-            app_context.version_name = obj.get('version_name')
-            app_context.version_code = obj.get('version_code')
+            app_context.business = obj.get('business', '')
+            app_context.version_name = obj.get('version_name', '--')
+            app_context.version_code = obj.get('version_code', '--')
             return
         except Exception as e:
             resp = context.make_fail_response(f'导入文件有误: {e}\n请重新import base')
 
         return resp
```

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/handlers/import_file_handler.py` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/handlers/import_file_handler.py`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/handlers/result_handler.py` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/handlers/result_handler.py`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage/manifest.py` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/manifest.py`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage.egg-info/PKG-INFO` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyrebird-api-coverage
-Version: 0.3.3
+Version: 0.4.0
 Summary: UNKNOWN
 Home-page: https://github.com/meituan/lyrebird-api-coverage
 Author: HBQA
 License: UNKNOWN
 Description: # Lyrebird Plugin API-Coverage
         
         [![Build Status](https://travis-ci.org/meituan/lyrebird-api-coverage.svg?branch=master)](https://travis-ci.org/meituan/lyrebird-api-coverage)
```

### Comparing `lyrebird-api-coverage-0.3.3/lyrebird_api_coverage.egg-info/SOURCES.txt` & `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,22 +24,22 @@
 lyrebird_api_coverage/client/merge_algorithm.py
 lyrebird_api_coverage/client/report.py
 lyrebird_api_coverage/client/url_compare.py
 lyrebird_api_coverage/default_conf/base.json
 lyrebird_api_coverage/default_conf/conf.json
 lyrebird_api_coverage/default_conf/filter_config.json
 lyrebird_api_coverage/dist/index.html
-lyrebird_api_coverage/dist/css/app.0233d703.css
+lyrebird_api_coverage/dist/css/app.964cc419.css
 lyrebird_api_coverage/dist/css/chunk-vendors.129fc3b2.css
 lyrebird_api_coverage/dist/fonts/codicon.a609dc0f.ttf
 lyrebird_api_coverage/dist/fonts/ionicons.143146fa.woff2
 lyrebird_api_coverage/dist/fonts/ionicons.99ac3308.woff
 lyrebird_api_coverage/dist/fonts/ionicons.d535a25a.ttf
 lyrebird_api_coverage/dist/img/ionicons.a2c4a261.svg
-lyrebird_api_coverage/dist/js/app.3e82be3c.js
+lyrebird_api_coverage/dist/js/app.6994bbbd.js
 lyrebird_api_coverage/dist/js/chunk-0b65ffb6.4d11c55b.js
 lyrebird_api_coverage/dist/js/chunk-2d0a3577.e9944055.js
 lyrebird_api_coverage/dist/js/chunk-2d0a43df.673ca57f.js
 lyrebird_api_coverage/dist/js/chunk-2d0aa90c.bb4da71a.js
 lyrebird_api_coverage/dist/js/chunk-2d0aab07.b30b422d.js
 lyrebird_api_coverage/dist/js/chunk-2d0abc00.ae916ae6.js
 lyrebird_api_coverage/dist/js/chunk-2d0ae937.5dfe330b.js
```

### Comparing `lyrebird-api-coverage-0.3.3/setup.py` & `lyrebird-api-coverage-0.4.0/setup.py`

 * *Files identical despite different names*

