# Comparing `tmp/jupyterlab_pachyderm-2.6.1.tar.gz` & `tmp/jupyterlab_pachyderm-2.7.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_pachyderm-2.6.1.tar", last modified: Thu May 25 15:46:43 2023, max compression
+gzip compressed data, was "jupyterlab_pachyderm-2.7.0a1.tar", last modified: Thu May 25 18:30:50 2023, max compression
```

## Comparing `jupyterlab_pachyderm-2.6.1.tar` & `jupyterlab_pachyderm-2.7.0a1.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.143847 jupyterlab_pachyderm-2.6.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11105 2023-05-25 15:46:43.143847 jupyterlab_pachyderm-2.6.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10130 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/babel.config.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/install.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      366 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jest.config.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.119847 jupyterlab_pachyderm-2.6.1/jupyter-config/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.123847 jupyterlab_pachyderm-2.6.1/jupyter-config/nb-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyter-config/nb-config/jupyterlab_pachyderm.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.123847 jupyterlab_pachyderm-2.6.1/jupyter-config/server-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       95 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyter-config/server-config/jupyterlab_pachyderm.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.127847 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/dev_server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      554 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/env.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/filemanager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12522 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/handlers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.127847 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4404 2023-05-25 15:46:40.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.119847 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/schemas/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.131847 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-05-25 15:46:29.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/examples.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-05-25 15:46:29.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/help.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-05-25 15:46:29.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/mount.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4262 2023-05-25 15:46:29.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-05-25 15:46:29.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/telemetry.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.131847 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2023-05-25 15:46:40.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2023-05-25 15:46:40.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    70514 2023-05-25 15:46:40.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2023-05-25 15:46:40.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)   401782 2023-05-25 15:46:40.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   102166 2023-05-25 15:46:40.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16896 2023-05-25 15:46:40.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   160194 2023-05-25 15:46:40.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/829.0234ec6e026820778750.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8296 2023-05-25 15:46:40.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/remoteEntry.d9811dd3652ac1fc0383.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-05-25 15:46:29.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/style.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8183 2023-05-25 15:46:40.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/third-party-licenses.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/log.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9051 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/mount_server_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      640 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/pachyderm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9524 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/pps_client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.131847 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.135847 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/tests/data/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19088 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/tests/test_handlers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16841 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/tests/test_integrations.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.127847 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11105 2023-05-25 15:46:43.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4690 2023-05-25 15:46:43.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-25 15:46:43.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-25 15:46:14.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-05-25 15:46:43.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-05-25 15:46:43.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4262 2023-05-25 15:43:56.000000 jupyterlab_pachyderm-2.6.1/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/pyproject.toml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.135847 jupyterlab_pachyderm-2.6.1/schema/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/schema/examples.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/schema/help.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/schema/mount.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/schema/telemetry.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      980 2023-05-25 15:46:43.147847 jupyterlab_pachyderm-2.6.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2260 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.135847 jupyterlab_pachyderm-2.6.1/src/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/global.d.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/handler.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.123847 jupyterlab_pachyderm-2.6.1/src/plugins/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.135847 jupyterlab_pachyderm-2.6.1/src/plugins/examples/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.135847 jupyterlab_pachyderm-2.6.1/src/plugins/examples/__test__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/examples/__test__/examples.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1789 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/examples/examples.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      413 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/examples/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.135847 jupyterlab_pachyderm-2.6.1/src/plugins/help/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.135847 jupyterlab_pachyderm-2.6.1/src/plugins/help/__tests__/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.135847 jupyterlab_pachyderm-2.6.1/src/plugins/help/__tests__/__snapshots__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1937 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/help/__tests__/help.test.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/help/help.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/help/help.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/help/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.135847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.135847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6919 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/__tests__/mount.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.123847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8530 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Config/Config.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Config/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12024 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Config/__tests__/Config.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Config/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Config/hooks/useConfig.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Datum/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4675 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Datum/Datum.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Datum/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7511 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Datum/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6182 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Datum/hooks/useDatum.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/FullPageError/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1012 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/FullPageError/FullPageError.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/FullPageError/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Pipeline/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5779 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Pipeline/Pipeline.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      999 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Pipeline/Splash.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Pipeline/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3800 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Pipeline/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4746 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/SortableList/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3730 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/SortableList/ListMount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5159 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/SortableList/ListUnmount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3415 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/SortableList/SortableList.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/SortableList/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14680 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2984 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/customFileBrowser.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1488 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8702 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/mount.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21752 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/mount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2993 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/mountDrive.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3658 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/pollMounts.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2606 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/types.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/telemetry/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/telemetry/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1988 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/telemetry/__tests__/telemetry.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/telemetry/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      814 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/telemetry/telemetry.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/setupTests.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/utils/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.123847 jupyterlab_pachyderm-2.6.1/src/utils/components/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/utils/components/Circle/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      757 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/components/Circle/Circle.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/components/Circle/circle.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.143847 jupyterlab_pachyderm-2.6.1/src/utils/components/LoadingDots/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/components/LoadingDots/LoadingDots.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      853 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/components/LoadingDots/loadingDots.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.143847 jupyterlab_pachyderm-2.6.1/src/utils/components/Svgs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26381 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/components/Svgs/GenericError.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    74288 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/components/Svgs/KubernetesElephant.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16523 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/components/Svgs/PachydermLogo.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/components/Svgs/StatusWarning.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/components/Svgs/index.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.143847 jupyterlab_pachyderm-2.6.1/src/utils/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/hooks/usePreviousValue.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/hooks/useSort.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      675 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/icons.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/testUtils.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.143847 jupyterlab_pachyderm-2.6.1/style/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/style/base.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.143847 jupyterlab_pachyderm-2.6.1/style/components/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1524 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/style/components/button.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/style/components/input.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.143847 jupyterlab_pachyderm-2.6.1/style/icons/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/style/icons/file.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/style/icons/info.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/style/icons/mount-logo.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/style/icons/repo.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/style/index.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/style/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/tsconfig.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.160175 jupyterlab_pachyderm-2.7.0a1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11107 2023-05-25 18:30:50.160175 jupyterlab_pachyderm-2.7.0a1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10130 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/babel.config.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/install.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      366 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/jest.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.136175 jupyterlab_pachyderm-2.7.0a1/jupyter-config/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.144175 jupyterlab_pachyderm-2.7.0a1/jupyter-config/nb-config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/jupyter-config/nb-config/jupyterlab_pachyderm.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.144175 jupyterlab_pachyderm-2.7.0a1/jupyter-config/server-config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       95 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/jupyter-config/server-config/jupyterlab_pachyderm.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.144175 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/dev_server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      554 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/env.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/filemanager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13073 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/handlers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.148175 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4412 2023-05-25 18:30:48.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.136175 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/schemas/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.148175 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-05-25 18:30:38.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/examples.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-05-25 18:30:38.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/help.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-05-25 18:30:38.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/mount.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4270 2023-05-25 18:30:38.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-05-25 18:30:38.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/telemetry.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.148175 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2023-05-25 18:30:48.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2023-05-25 18:30:48.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    70514 2023-05-25 18:30:48.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2023-05-25 18:30:48.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   401782 2023-05-25 18:30:48.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   102166 2023-05-25 18:30:48.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16896 2023-05-25 18:30:48.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   161102 2023-05-25 18:30:48.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/static/829.75c9ab3fc9e1a8c63de6.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8304 2023-05-25 18:30:48.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/static/remoteEntry.472bd5c5853eeaa9de7a.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-05-25 18:30:38.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/static/style.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8183 2023-05-25 18:30:48.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/static/third-party-licenses.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/log.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9229 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/mount_server_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/pachyderm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9524 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/pps_client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.152176 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.152176 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/tests/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/tests/data/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19829 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/tests/test_handlers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16841 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/tests/test_integrations.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.148175 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11107 2023-05-25 18:30:50.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4690 2023-05-25 18:30:50.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-25 18:30:50.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-25 18:30:23.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-05-25 18:30:50.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-05-25 18:30:50.000000 jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4270 2023-05-25 18:28:21.000000 jupyterlab_pachyderm-2.7.0a1/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/pyproject.toml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.152176 jupyterlab_pachyderm-2.7.0a1/schema/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/schema/examples.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/schema/help.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/schema/mount.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/schema/telemetry.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      980 2023-05-25 18:30:50.160175 jupyterlab_pachyderm-2.7.0a1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2260 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.152176 jupyterlab_pachyderm-2.7.0a1/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/global.d.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/handler.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.140175 jupyterlab_pachyderm-2.7.0a1/src/plugins/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.152176 jupyterlab_pachyderm-2.7.0a1/src/plugins/examples/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.152176 jupyterlab_pachyderm-2.7.0a1/src/plugins/examples/__test__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/examples/__test__/examples.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1789 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/examples/examples.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      413 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/examples/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.152176 jupyterlab_pachyderm-2.7.0a1/src/plugins/help/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.152176 jupyterlab_pachyderm-2.7.0a1/src/plugins/help/__tests__/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.152176 jupyterlab_pachyderm-2.7.0a1/src/plugins/help/__tests__/__snapshots__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1937 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/help/__tests__/help.test.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/help/help.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/help/help.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/help/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.152176 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.152176 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6919 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/__tests__/mount.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.140175 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.152176 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8530 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Config/Config.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.152176 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Config/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12024 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Config/__tests__/Config.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.156175 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Config/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Config/hooks/useConfig.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.156175 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Datum/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4675 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Datum/Datum.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.156175 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Datum/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7511 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.156175 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Datum/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6182 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Datum/hooks/useDatum.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.156175 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/FullPageError/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1012 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/FullPageError/FullPageError.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.156175 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/FullPageError/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.156175 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Pipeline/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6365 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Pipeline/Pipeline.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      999 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Pipeline/Splash.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.156175 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Pipeline/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3528 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.156175 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Pipeline/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4308 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.156175 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/SortableList/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3730 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/SortableList/ListMount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5159 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/SortableList/ListUnmount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3498 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/SortableList/SortableList.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.156175 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/SortableList/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15391 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2984 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/customFileBrowser.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1488 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8702 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/mount.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22029 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/mount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2993 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/mountDrive.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4382 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/pollMounts.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2763 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/types.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.156175 jupyterlab_pachyderm-2.7.0a1/src/plugins/telemetry/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.156175 jupyterlab_pachyderm-2.7.0a1/src/plugins/telemetry/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1988 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/telemetry/__tests__/telemetry.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/telemetry/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      814 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/plugins/telemetry/telemetry.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/setupTests.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.156175 jupyterlab_pachyderm-2.7.0a1/src/utils/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.140175 jupyterlab_pachyderm-2.7.0a1/src/utils/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.156175 jupyterlab_pachyderm-2.7.0a1/src/utils/components/Circle/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      757 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/utils/components/Circle/Circle.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/utils/components/Circle/circle.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.156175 jupyterlab_pachyderm-2.7.0a1/src/utils/components/LoadingDots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/utils/components/LoadingDots/LoadingDots.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      853 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/utils/components/LoadingDots/loadingDots.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.156175 jupyterlab_pachyderm-2.7.0a1/src/utils/components/Svgs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26381 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/utils/components/Svgs/GenericError.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74288 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/utils/components/Svgs/KubernetesElephant.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16523 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/utils/components/Svgs/PachydermLogo.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/utils/components/Svgs/StatusWarning.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/utils/components/Svgs/index.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.160175 jupyterlab_pachyderm-2.7.0a1/src/utils/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/utils/hooks/usePreviousValue.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/utils/hooks/useSort.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      675 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/utils/icons.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/src/utils/testUtils.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.160175 jupyterlab_pachyderm-2.7.0a1/style/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/style/base.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.160175 jupyterlab_pachyderm-2.7.0a1/style/components/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1524 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/style/components/button.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/style/components/input.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 18:30:50.160175 jupyterlab_pachyderm-2.7.0a1/style/icons/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/style/icons/file.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/style/icons/info.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/style/icons/mount-logo.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/style/icons/repo.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/style/index.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/style/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-05-25 18:28:20.000000 jupyterlab_pachyderm-2.7.0a1/tsconfig.json
```

### Comparing `jupyterlab_pachyderm-2.6.1/LICENSE` & `jupyterlab_pachyderm-2.7.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/MANIFEST.in` & `jupyterlab_pachyderm-2.7.0a1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/PKG-INFO` & `jupyterlab_pachyderm-2.7.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_pachyderm
-Version: 2.6.1
+Version: 2.7.0a1
 Summary: A JupyterLab extension.
 Home-page: https://github.com/pachyderm/jupyterlab-pachyderm
 Author: 
 Author-email: 
 License: BSD-3-Clause
 Keywords: jupyter,jupyterlab,jupyterlab-extension
 Platform: Linux
```

### Comparing `jupyterlab_pachyderm-2.6.1/README.md` & `jupyterlab_pachyderm-2.7.0a1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/__init__.py` & `jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/_version.py` & `jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/_version.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/env.py` & `jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/env.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/handlers.py` & `jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,28 @@
         except Exception as e:
             get_logger().error("Error listing mounts.", exc_info=True)
             raise tornado.web.HTTPError(
                 status_code=getattr(e, "code", 500), reason=f"Error listing mounts: {e}."
             )
 
 
+class ProjectsHandler(BaseHandler):
+    @tornado.web.authenticated
+    async def get(self):
+        try:
+            response = await self.mount_client.list_projects()
+            get_logger().debug(f"Projects: {response}")
+            self.finish(response)
+        except Exception as e:
+            get_logger().error("Error listing projects.", exc_info=True)
+            raise tornado.web.HTTPError(
+                status_code=getattr(e, "code", 500), reason=f"Error listing projects: {e}."
+            )
+
+
 class MountHandler(BaseHandler):
     @tornado.web.authenticated
     async def put(self):
         try:
             body = self.get_json_body()
             response = await self.mount_client.mount(body)
             get_logger().debug(f"Mount: {response}")
@@ -309,14 +323,15 @@
     web_app.settings["pfs_contents_manager"] = PFSContentsManager(PFS_MOUNT_DIR)
     web_app.settings["pachyderm_mount_client"] = MountServerClient(PFS_MOUNT_DIR)
     web_app.settings["pachyderm_pps_client"] = PPSClient()
 
     _handlers = [
         ("/repos", ReposHandler),
         ("/mounts", MountsHandler),
+        ("/projects", ProjectsHandler),
         ("/_mount", MountHandler),
         ("/_unmount", UnmountHandler),
         ("/_commit", CommitHandler),
         ("/_unmount_all", UnmountAllHandler),
         ("/_mount_datums", MountDatumsHandler),
         (r"/_show_datum", ShowDatumHandler),
         (r"/pfs%s" % path_regex, PFSHandler),
```

### Comparing `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/package.json` & `jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222223%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'2.7.0-alpha.1'"}*

```diff
@@ -66,19 +66,14 @@
             "before-build-npm": [
                 "python -m pip install jupyterlab~=3.1",
                 "npm"
             ]
         }
     },
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.d9811dd3652ac1fc0383.js",
-            "style": "./style"
-        },
         "disabledExtensions": [
             "jupyterlab-pachyderm:examples"
         ],
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_pachyderm"
@@ -133,9 +128,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.6.1"
+    "version": "2.7.0-alpha.1"
 }
```

### Comparing `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig` & `jupyterlab_pachyderm-2.7.0a1/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'2.7.0-alpha.1'"}*

```diff
@@ -128,9 +128,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.6.1"
+    "version": "2.7.0-alpha.1"
 }
```

### Comparing `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js` & `jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js` & `jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js` & `jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js` & `jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js` & `jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/829.0234ec6e026820778750.js` & `jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/static/829.75c9ab3fc9e1a8c63de6.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 "use strict";
 (self.webpackChunkjupyterlab_pachyderm = self.webpackChunkjupyterlab_pachyderm || []).push([
     [829], {
         7363: (e, t, a) => {
             a.r(t), a.d(t, {
-                default: () => fe
+                default: () => Ee
             });
             var n = a(3279),
                 r = a.n(n),
                 l = a(4234);
             const s = r()((e => {
                     const t = e.target.getAttribute("data-testid");
                     t && (0, l.track)("notebook:click", {
@@ -388,19 +388,19 @@
                                 rank: e.rank
                             }))
                         })))(a, e, t))))
                     })))(e, t)
                 };
             var C = a(5687),
                 M = a(7986),
-                z = a(7280),
-                S = a(4038),
+                S = a(7280),
+                z = a(4038),
                 L = a(1123),
-                B = a(1840),
-                N = a(8832),
+                N = a(1840),
+                B = a(8832),
                 O = a(3114);
 
             function D(e = "", t = "GET", a = null, n = "pachyderm/v2") {
                 return r = this, l = void 0, i = function*() {
                     const r = _.ServerConnection.makeSettings(),
                         l = E.URLExt.join(r.baseUrl, n, e),
                         s = {
@@ -479,48 +479,56 @@
                         }))).then(s, i)
                     }
                     c((n = n.apply(e, t || [])).next())
                 }))
             };
             class F {
                 constructor(e) {
-                    this._rawData = {}, this._mounted = [], this._unmounted = [], this._status = {
+                    this._rawData = {}, this._mounted = [], this._unmounted = [], this._projects = [], this._status = {
                         code: 999,
                         message: ""
                     }, this._config = {
                         pachd_address: "",
                         cluster_status: "INVALID"
-                    }, this._mountedSignal = new B.Signal(this), this._unmountedSignal = new B.Signal(this), this._statusSignal = new B.Signal(this), this._configSignal = new B.Signal(this), this._dataPoll = new O.n_({
+                    }, this._mountedSignal = new N.Signal(this), this._unmountedSignal = new N.Signal(this), this._projectSignal = new N.Signal(this), this._statusSignal = new N.Signal(this), this._configSignal = new N.Signal(this), this._dataPoll = new O.n_({
                         auto: !0,
                         factory: () => A(this, void 0, void 0, (function*() {
                             return this.getData()
                         })),
                         frequency: {
                             interval: 2e3,
                             backoff: !0,
                             max: 5e3
                         }
                     }), this.refresh = () => A(this, void 0, void 0, (function*() {
                         yield this._dataPoll.refresh(), yield this._dataPoll.tick
                     })), this.updateData = e => {
                         JSON.stringify(e) !== JSON.stringify(this._rawData) && (this._rawData = e, this.mounted = Array.from(Object.values(e.mounted)), this.unmounted = Array.from(Object.values(e.unmounted)))
+                    }, this.updateProjects = e => {
+                        JSON.stringify(e) !== JSON.stringify(this.projects) && (this.projects = e)
                     }, this.name = e
                 }
                 get mounted() {
                     return this._mounted
                 }
                 set mounted(e) {
                     e !== this._mounted && (this._mounted = e, this._mountedSignal.emit(e))
                 }
                 get unmounted() {
                     return this._unmounted
                 }
                 set unmounted(e) {
                     e !== this._unmounted && (this._unmounted = e, this._unmountedSignal.emit(e))
                 }
+                get projects() {
+                    return this._projects
+                }
+                set projects(e) {
+                    e !== this._projects && (this._projects = e, this._projectSignal.emit(e))
+                }
                 get status() {
                     return this._status
                 }
                 set status(e) {
                     JSON.stringify(e) !== JSON.stringify(this._status) && (this._status = e, this._statusSignal.emit(e))
                 }
                 get config() {
@@ -531,14 +539,17 @@
                 }
                 get mountedSignal() {
                     return this._mountedSignal
                 }
                 get unmountedSignal() {
                     return this._unmountedSignal
                 }
+                get projectSignal() {
+                    return this._projectSignal
+                }
                 get statusSignal() {
                     return this._statusSignal
                 }
                 get configSignal() {
                     return this._configSignal
                 }
                 get poll() {
@@ -548,30 +559,32 @@
                     return A(this, void 0, void 0, (function*() {
                         try {
                             const e = yield D("config", "GET");
                             if (this.config = e, "INVALID" !== e.cluster_status) {
                                 const e = yield D("mounts", "GET");
                                 this.status = {
                                     code: 200
-                                }, this.updateData(e)
+                                }, this.updateData(e);
+                                const t = yield D("projects", "GET");
+                                this.updateProjects(t)
                             }
                         } catch (e) {
                             e instanceof _.ServerConnection.ResponseError && (this.status = {
                                 code: e.response.status,
                                 message: e.response.statusText
                             })
                         }
                     }))
                 }
             }
             var j = a(6057),
-                H = a(8918);
-            class P {
+                P = a(8918);
+            class H {
                 constructor(e) {
-                    this._fileChanged = new B.Signal(this), this._serverSettings = _.ServerConnection.makeSettings(), this._isDisposed = !1, this._registry = e
+                    this._fileChanged = new N.Signal(this), this._serverSettings = _.ServerConnection.makeSettings(), this._isDisposed = !1, this._registry = e
                 }
                 get name() {
                     return "mount-browser"
                 }
                 get fileChanged() {
                     return this._fileChanged
                 }
@@ -656,15 +669,15 @@
                 restoreCheckpoint(e, t) {
                     return Promise.resolve()
                 }
                 deleteCheckpoint(e, t) {
                     return Promise.resolve()
                 }
                 dispose() {
-                    this.isDisposed || (this._isDisposed = !0, B.Signal.clearData(this))
+                    this.isDisposed || (this._isDisposed = !0, N.Signal.clearData(this))
                 }
             }
             var I = function(e, t, a, n) {
                 return new(a || (a = Promise))((function(r, l) {
                     function s(e) {
                         try {
                             c(n.next(e))
@@ -2637,18 +2650,18 @@
                     } = ((e, t, a, n, r, l, s) => {
                         const [i, c] = (0, o.useState)(!1), [m, d] = (0, o.useState)(!1), [u, h] = (0, o.useState)(-1), [p, f] = (0, o.useState)({
                             id: "",
                             idx: -1,
                             num_datums: 0
                         }), [E, g] = (0, o.useState)(""), [v, k] = (0, o.useState)({}), [y, b] = (0, o.useState)(""), [w, x] = (0, o.useState)({});
                         (0, o.useEffect)((() => {
-                            e && -1 !== u && z()
+                            e && -1 !== u && S()
                         }), [u, e]), (0, o.useEffect)((() => {
                             if (e)
-                                if (t || S(), t && s) d(!0), h(s.curr_idx), f({
+                                if (t || z(), t && s) d(!0), h(s.curr_idx), f({
                                     id: "",
                                     idx: s.curr_idx,
                                     num_datums: s.num_datums
                                 }), g(M(s.input)), a(!1);
                                 else if ("string" == typeof w) g(w);
                             else {
                                 let e = {};
@@ -2669,25 +2682,25 @@
                                 if (0 === Object.keys(e).length) return "";
                                 try {
                                     return JSON.parse(E), JSON.stringify(e, null, 2)
                                 } catch (t) {
                                     return T().stringify(e, null, 2)
                                 }
                             },
-                            z = () => $(void 0, void 0, void 0, (function*() {
+                            S = () => $(void 0, void 0, void 0, (function*() {
                                 c(!0);
                                 try {
                                     const e = yield D(`_show_datum?idx=${u}`, "PUT");
                                     n(""), f(e)
                                 } catch (e) {
                                     console.log(e)
                                 }
                                 c(!1)
                             })),
-                            S = () => $(void 0, void 0, void 0, (function*() {
+                            z = () => $(void 0, void 0, void 0, (function*() {
                                 c(!0);
                                 try {
                                     n(""), yield D("_unmount_all", "PUT"), n(""), yield r(), h(-1), f({
                                         id: "",
                                         idx: -1,
                                         num_datums: 0
                                     }), d(!1)
@@ -2713,15 +2726,15 @@
                                         });
                                     n(""), h(0), f(t), d(!0), g(M(e))
                                 } catch (e) {
                                     console.log(e), e instanceof T().YAMLParseError ? b("Poorly formatted input spec- must be either YAML or JSON") : e instanceof _.ServerConnection.ResponseError ? b("Bad data in input spec") : b("Error mounting datums")
                                 }
                                 c(!1)
                             })),
-                            callUnmountAll: S,
+                            callUnmountAll: z,
                             errorMessage: y,
                             saveInputSpec: () => {
                                 try {
                                     const e = C();
                                     (0, V.isEqual)(l, e) ? x({}): x(e || {})
                                 } catch (e) {
                                     if (!(e instanceof T().YAMLParseError)) throw e;
@@ -2864,244 +2877,251 @@
                         e.done ? r(e.value) : (t = e.value, t instanceof a ? t : new a((function(e) {
                             e(t)
                         }))).then(s, i)
                     }
                     c((n = n.apply(e, t || [])).next())
                 }))
             };
-            const q = ({
-                ppsContext: e,
-                settings: t,
-                setShowPipeline: a,
-                saveNotebookMetadata: n,
-                saveNotebookToDisk: r
-            }) => {
-                var l, s, i;
-                const {
-                    loading: c,
-                    pipeline: d,
-                    setPipeline: u,
-                    imageName: h,
-                    setImageName: p,
-                    inputSpec: f,
-                    setInputSpec: E,
-                    requirements: v,
-                    setRequirements: k,
-                    callCreatePipeline: y,
-                    currentNotebook: b,
-                    errorMessage: w,
-                    responseMessage: x
-                } = ((e, t, a, n) => {
-                    const [r, l] = (0, o.useState)(!1), [s, i] = (0, o.useState)({
-                        name: ""
-                    }), [c, m] = (0, o.useState)(""), [d, u] = (0, o.useState)(""), [h, p] = (0, o.useState)(""), [f, E] = (0, o.useState)(""), [g, v] = (0, o.useState)(""), [k, y] = (0, o.useState)("None");
-                    let b;
-                    if ((0, o.useEffect)((() => {
-                            var a, n, r, l, s, c, o, d, h;
-                            m(null !== (n = null === (a = null == e ? void 0 : e.metadata) || void 0 === a ? void 0 : a.config.image) && void 0 !== n ? n : t.defaultPipelineImage), i(null !== (l = null === (r = null == e ? void 0 : e.metadata) || void 0 === r ? void 0 : r.config.pipeline) && void 0 !== l ? l : {
-                                name: ""
-                            }), p(null !== (c = null === (s = null == e ? void 0 : e.metadata) || void 0 === s ? void 0 : s.config.requirements) && void 0 !== c ? c : ""), v(""), (null === (o = null == e ? void 0 : e.metadata) || void 0 === o ? void 0 : o.config.input_spec) ? u(e.metadata.config.input_spec) : u(""), y(null !== (h = null === (d = null == e ? void 0 : e.notebookModel) || void 0 === d ? void 0 : d.name) && void 0 !== h ? h : "None")
-                        }), [e]), (0, o.useEffect)((() => {
-                            const e = w();
-                            a(e)
-                        }), [s, c, h, d]), null == e ? void 0 : e.notebookModel) {
-                        const t = e.notebookModel;
-                        b = () => J(void 0, void 0, void 0, (function*() {
-                            l(!0), E(""), v("");
-                            const e = w();
-                            a(e);
-                            const r = yield n();
-                            try {
-                                const e = yield D(`pps/_create/${encodeURI(t.path)}`, "PUT", {
-                                    last_modified_time: null != r ? r : t.last_modified
-                                });
-                                null !== e.message && v(e.message)
-                            } catch (e) {
-                                if (!(e instanceof _.ServerConnection.ResponseError)) throw e;
-                                E("Error creating pipeline: " + e.response.statusText)
-                            }
-                            l(!1)
-                        }))
-                    } else b = () => J(void 0, void 0, void 0, (function*() {
-                        E("Error: No notebook in focus")
-                    }));
-                    const w = () => ({
-                        version: "v1.0.0",
-                        config: {
-                            pipeline: s,
-                            image: c,
-                            requirements: h,
-                            input_spec: d
-                        }
-                    });
-                    return {
-                        loading: r,
-                        pipeline: s,
-                        setPipeline: e => {
-                            if ("" === e) return void i({
-                                name: ""
-                            });
-                            const t = e.split(/\/(.*)/s, 2);
-                            1 === t.length ? i({
-                                name: e
-                            }) : i({
-                                name: t[1],
-                                project: {
-                                    name: t[0]
-                                }
-                            })
-                        },
-                        imageName: c,
-                        setImageName: m,
-                        inputSpec: d,
-                        setInputSpec: u,
-                        requirements: h,
-                        setRequirements: p,
-                        callCreatePipeline: b,
-                        currentNotebook: k,
-                        errorMessage: f,
-                        responseMessage: g
-                    }
-                })(e, t, n, r);
-                return m().createElement("div", {
-                    className: "pachyderm-mount-pipeline-base"
-                }, m().createElement("div", {
-                    className: "pachyderm-mount-pipeline-back"
-                }, m().createElement("button", {
-                    "data-testid": "Pipeline__back",
-                    className: "pachyderm-button-link",
-                    onClick: () => {
-                        return e = void 0, t = void 0, r = function*() {
-                            a(!1)
-                        }, new((n = void 0) || (n = Promise))((function(a, l) {
-                            function s(e) {
+            const q = "default",
+                Y = ({
+                    ppsContext: e,
+                    settings: t,
+                    setShowPipeline: a,
+                    saveNotebookMetadata: n,
+                    saveNotebookToDisk: r
+                }) => {
+                    const {
+                        loading: l,
+                        pipelineName: s,
+                        setPipelineName: i,
+                        pipelineProject: c,
+                        setPipelineProject: d,
+                        imageName: u,
+                        setImageName: h,
+                        inputSpec: p,
+                        setInputSpec: f,
+                        requirements: E,
+                        setRequirements: v,
+                        callCreatePipeline: k,
+                        currentNotebook: y,
+                        errorMessage: b,
+                        responseMessage: w
+                    } = ((e, t, a, n) => {
+                        const [r, l] = (0, o.useState)(!1), [s, i] = (0, o.useState)(""), [c, m] = (0, o.useState)(""), [d, u] = (0, o.useState)(""), [h, p] = (0, o.useState)(""), [f, E] = (0, o.useState)(""), [g, v] = (0, o.useState)(""), [k, y] = (0, o.useState)(""), [b, w] = (0, o.useState)("None");
+                        let x;
+                        if ((0, o.useEffect)((() => {
+                                var a, n, r, l, s, c, o, d, h, f, _, g;
+                                u(null !== (n = null === (a = null == e ? void 0 : e.metadata) || void 0 === a ? void 0 : a.config.image) && void 0 !== n ? n : t.defaultPipelineImage), i(null !== (l = null === (r = null == e ? void 0 : e.metadata) || void 0 === r ? void 0 : r.config.pipeline.name) && void 0 !== l ? l : ""), m(null !== (o = null === (c = null === (s = null == e ? void 0 : e.metadata) || void 0 === s ? void 0 : s.config.pipeline.project) || void 0 === c ? void 0 : c.name) && void 0 !== o ? o : ""), E(null !== (h = null === (d = null == e ? void 0 : e.metadata) || void 0 === d ? void 0 : d.config.requirements) && void 0 !== h ? h : ""), y(""), (null === (f = null == e ? void 0 : e.metadata) || void 0 === f ? void 0 : f.config.input_spec) ? p(e.metadata.config.input_spec) : p(""), w(null !== (g = null === (_ = null == e ? void 0 : e.notebookModel) || void 0 === _ ? void 0 : _.name) && void 0 !== g ? g : "None")
+                            }), [e]), (0, o.useEffect)((() => {
+                                const e = C();
+                                a(e)
+                            }), [s, c, d, f, h]), null == e ? void 0 : e.notebookModel) {
+                            const t = e.notebookModel;
+                            x = () => J(void 0, void 0, void 0, (function*() {
+                                l(!0), v(""), y("");
+                                const e = C();
+                                a(e);
+                                const r = yield n();
                                 try {
-                                    c(r.next(e))
+                                    const e = yield D(`pps/_create/${encodeURI(t.path)}`, "PUT", {
+                                        last_modified_time: null != r ? r : t.last_modified
+                                    });
+                                    null !== e.message && y(e.message)
                                 } catch (e) {
-                                    l(e)
+                                    if (!(e instanceof _.ServerConnection.ResponseError)) throw e;
+                                    v("Error creating pipeline: " + e.response.statusText)
                                 }
+                                l(!1)
+                            }))
+                        } else x = () => J(void 0, void 0, void 0, (function*() {
+                            v("Error: No notebook in focus")
+                        }));
+                        const C = () => ({
+                            version: "v1.0.0",
+                            config: {
+                                pipeline: {
+                                    name: s,
+                                    project: {
+                                        name: c
+                                    }
+                                },
+                                image: d,
+                                requirements: f,
+                                input_spec: h
                             }
+                        });
+                        return {
+                            loading: r,
+                            pipelineName: s,
+                            setPipelineName: i,
+                            pipelineProject: c,
+                            setPipelineProject: m,
+                            imageName: d,
+                            setImageName: u,
+                            inputSpec: h,
+                            setInputSpec: p,
+                            requirements: f,
+                            setRequirements: E,
+                            callCreatePipeline: x,
+                            currentNotebook: b,
+                            errorMessage: g,
+                            responseMessage: k
+                        }
+                    })(e, t, n, r);
+                    return m().createElement("div", {
+                        className: "pachyderm-mount-pipeline-base"
+                    }, m().createElement("div", {
+                        className: "pachyderm-mount-pipeline-back"
+                    }, m().createElement("button", {
+                        "data-testid": "Pipeline__back",
+                        className: "pachyderm-button-link",
+                        onClick: () => {
+                            return e = void 0, t = void 0, r = function*() {
+                                a(!1)
+                            }, new((n = void 0) || (n = Promise))((function(a, l) {
+                                function s(e) {
+                                    try {
+                                        c(r.next(e))
+                                    } catch (e) {
+                                        l(e)
+                                    }
+                                }
 
-                            function i(e) {
-                                try {
-                                    c(r.throw(e))
-                                } catch (e) {
-                                    l(e)
+                                function i(e) {
+                                    try {
+                                        c(r.throw(e))
+                                    } catch (e) {
+                                        l(e)
+                                    }
                                 }
-                            }
 
-                            function c(e) {
-                                var t;
-                                e.done ? a(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
-                                    e(t)
-                                }))).then(s, i)
-                            }
-                            c((r = r.apply(e, t || [])).next())
-                        }));
-                        var e, t, n, r
-                    }
-                }, "Back", " ", m().createElement(g.closeIcon.react, {
-                    tag: "span",
-                    className: "pachyderm-mount-icon-padding"
-                }))), m().createElement("span", {
-                    className: "pachyderm-mount-pipeline-subheading"
-                }, "Publish as Pipeline"), m().createElement("div", {
-                    className: "pachyderm-pipeline-current-notebook-wrapper"
-                }, m().createElement("label", {
-                    className: "pachyderm-pipeline-current-notebook-label",
-                    htmlFor: "currentNotebook"
-                }, "Current Notebook:", "  "), m().createElement("span", {
-                    className: "pachyderm-pipeline-current-notebook-value",
-                    "data-testid": "Pipeline__currentNotebookValue"
-                }, b)), m().createElement("div", {
-                    className: "pachyderm-pipeline-input-wrapper"
-                }, m().createElement("label", {
-                    className: "pachyderm-pipeline-input-label",
-                    htmlFor: "pipelineName"
-                }, "*Pipeline Name:", "  "), m().createElement("input", {
-                    className: "pachyderm-pipeline-input",
-                    "data-testid": "Pipeline__inputPipelineName",
-                    name: "pipelineName",
-                    value: (null === (l = d.project) || void 0 === l ? void 0 : l.name) ? `${d.project.name}/${d.name}` : d.name,
-                    onChange: e => {
-                        u(e.target.value)
-                    },
-                    disabled: c
-                })), m().createElement("div", {
-                    className: "pachyderm-pipeline-input-wrapper"
-                }, m().createElement("label", {
-                    className: "pachyderm-pipeline-input-label",
-                    htmlFor: "imageName"
-                }, "*Container Image Name:", "  "), m().createElement("input", {
-                    className: "pachyderm-pipeline-input",
-                    "data-testid": "Pipeline__inputImageName",
-                    name: "imageName",
-                    value: h,
-                    onChange: e => {
-                        p(e.target.value)
-                    },
-                    disabled: c
-                })), m().createElement("div", {
-                    className: "pachyderm-pipeline-input-wrapper"
-                }, m().createElement("label", {
-                    className: "pachyderm-pipeline-input-label",
-                    htmlFor: "requirements"
-                }, "Requirements File:", "  "), m().createElement("input", {
-                    className: "pachyderm-pipeline-input",
-                    "data-testid": "Pipeline__inputRequirements",
-                    name: "requirements",
-                    value: v,
-                    onChange: e => {
-                        k(e.target.value)
-                    },
-                    disabled: c,
-                    placeholder: "./requirements.txt"
-                })), m().createElement("div", {
-                    className: "pachyderm-pipeline-textarea-wrapper"
-                }, m().createElement("label", {
-                    className: "pachyderm-pipeline-textarea-label",
-                    htmlFor: "inputSpec"
-                }, "Pipeline Input Spec:"), m().createElement("textarea", {
-                    className: "pachyderm-pipeline-textarea pachyderm-input",
-                    "data-testid": "Pipeline__inputSpecInput",
-                    name: "inputSpec",
-                    value: f,
-                    onChange: e => {
-                        E(e.target.value)
-                    },
-                    disabled: c,
-                    placeholder: "# example:\npfs:\n  repo: images\n  branch: dev\n  glob: /*\n"
-                })), m().createElement("div", {
-                    className: "pachyderm-pipeline-spec-preview pachyderm-pipeline-textarea-wrapper"
-                }, m().createElement("label", {
-                    className: "pachyderm-pipeline-preview-label"
-                }, "Pipeline Spec Preview: ", "  "), m().createElement("textarea", {
-                    className: "pachyderm-pipeline-spec-preview-textarea",
-                    style: {
-                        backgroundColor: "#80808080"
-                    },
-                    "data-testid": "Pipeline__specPreview",
-                    name: "specPreview",
-                    value: `pipeline:\n  name: ${d.name}\n  project: ${null!==(i=null===(s=d.project)||void 0===s?void 0:s.name)&&void 0!==i?i:"default"}\ntransform:\n  image: ${h}\ninput:\n${f.split("\n").map(((e,t,a)=>"  "+e)).join("\n")}\n`,
-                    readOnly: !0
-                })), m().createElement("div", {
-                    className: "pachyderm-pipeline-buttons"
-                }, m().createElement("button", {
-                    "data-testid": "Pipeline__create_pipeline",
-                    className: "pachyderm-button",
-                    onClick: y
-                }, "Run")), m().createElement("span", {
-                    className: "pachyderm-pipeline-error",
-                    "data-testid": "Pipeline__errorMessage"
-                }, w), m().createElement("span", {
-                    className: "pachyderm-pipeline-response",
-                    "data-testid": "Pipeline__responseMessage"
-                }, x))
-            };
-            const Y = ({
+                                function c(e) {
+                                    var t;
+                                    e.done ? a(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
+                                        e(t)
+                                    }))).then(s, i)
+                                }
+                                c((r = r.apply(e, t || [])).next())
+                            }));
+                            var e, t, n, r
+                        }
+                    }, "Back", " ", m().createElement(g.closeIcon.react, {
+                        tag: "span",
+                        className: "pachyderm-mount-icon-padding"
+                    }))), m().createElement("span", {
+                        className: "pachyderm-mount-pipeline-subheading"
+                    }, "Publish as Pipeline"), m().createElement("div", {
+                        className: "pachyderm-pipeline-current-notebook-wrapper"
+                    }, m().createElement("label", {
+                        className: "pachyderm-pipeline-current-notebook-label",
+                        htmlFor: "currentNotebook"
+                    }, "Current Notebook:", "  "), m().createElement("span", {
+                        className: "pachyderm-pipeline-current-notebook-value",
+                        "data-testid": "Pipeline__currentNotebookValue"
+                    }, y)), m().createElement("div", {
+                        className: "pachyderm-pipeline-input-wrapper"
+                    }, m().createElement("label", {
+                        className: "pachyderm-pipeline-input-label",
+                        htmlFor: "pipelineName"
+                    }, "*Pipeline Name:", "  "), m().createElement("input", {
+                        className: "pachyderm-pipeline-input",
+                        "data-testid": "Pipeline__inputPipelineName",
+                        name: "pipelineName",
+                        value: s,
+                        onChange: e => {
+                            i(e.target.value)
+                        },
+                        disabled: l
+                    })), m().createElement("div", {
+                        className: "pachyderm-pipeline-input-wrapper"
+                    }, m().createElement("label", {
+                        className: "pachyderm-pipeline-input-label",
+                        htmlFor: "pipelineProjectName"
+                    }, "Pipeline Project Name:", "  "), m().createElement("input", {
+                        className: "pachyderm-pipeline-input",
+                        "data-testid": "Pipeline__inputPipelineProjectName",
+                        name: "pipelineName",
+                        value: c,
+                        onChange: e => {
+                            d(e.target.value)
+                        },
+                        disabled: l,
+                        placeholder: q
+                    })), m().createElement("div", {
+                        className: "pachyderm-pipeline-input-wrapper"
+                    }, m().createElement("label", {
+                        className: "pachyderm-pipeline-input-label",
+                        htmlFor: "imageName"
+                    }, "*Container Image Name:", "  "), m().createElement("input", {
+                        className: "pachyderm-pipeline-input",
+                        "data-testid": "Pipeline__inputImageName",
+                        name: "imageName",
+                        value: u,
+                        onChange: e => {
+                            h(e.target.value)
+                        },
+                        disabled: l
+                    })), m().createElement("div", {
+                        className: "pachyderm-pipeline-input-wrapper"
+                    }, m().createElement("label", {
+                        className: "pachyderm-pipeline-input-label",
+                        htmlFor: "requirements"
+                    }, "Requirements File:", "  "), m().createElement("input", {
+                        className: "pachyderm-pipeline-input",
+                        "data-testid": "Pipeline__inputRequirements",
+                        name: "requirements",
+                        value: E,
+                        onChange: e => {
+                            v(e.target.value)
+                        },
+                        disabled: l,
+                        placeholder: "./requirements.txt"
+                    })), m().createElement("div", {
+                        className: "pachyderm-pipeline-textarea-wrapper"
+                    }, m().createElement("label", {
+                        className: "pachyderm-pipeline-textarea-label",
+                        htmlFor: "inputSpec"
+                    }, "Pipeline Input Spec:"), m().createElement("textarea", {
+                        className: "pachyderm-pipeline-textarea pachyderm-input",
+                        "data-testid": "Pipeline__inputSpecInput",
+                        name: "inputSpec",
+                        value: p,
+                        onChange: e => {
+                            f(e.target.value)
+                        },
+                        disabled: l,
+                        placeholder: "# example:\npfs:\n  repo: images\n  branch: dev\n  glob: /*\n"
+                    })), m().createElement("div", {
+                        className: "pachyderm-pipeline-spec-preview pachyderm-pipeline-textarea-wrapper"
+                    }, m().createElement("label", {
+                        className: "pachyderm-pipeline-preview-label"
+                    }, "Pipeline Spec Preview: ", "  "), m().createElement("textarea", {
+                        className: "pachyderm-pipeline-spec-preview-textarea",
+                        style: {
+                            backgroundColor: "#80808080"
+                        },
+                        "data-testid": "Pipeline__specPreview",
+                        name: "specPreview",
+                        value: `pipeline:\n  name: ${s}\n  project: ${c||q}\ntransform:\n  image: ${u}\ninput:\n${p.split("\n").map(((e,t,a)=>"  "+e)).join("\n")}\n`,
+                        readOnly: !0
+                    })), m().createElement("div", {
+                        className: "pachyderm-pipeline-buttons"
+                    }, m().createElement("button", {
+                        "data-testid": "Pipeline__create_pipeline",
+                        className: "pachyderm-button",
+                        onClick: k
+                    }, "Run")), m().createElement("span", {
+                        className: "pachyderm-pipeline-error",
+                        "data-testid": "Pipeline__errorMessage"
+                    }, b), m().createElement("span", {
+                        className: "pachyderm-pipeline-response",
+                        "data-testid": "Pipeline__responseMessage"
+                    }, w))
+                };
+            const X = ({
                     setShowPipeline: e
                 }) => m().createElement("div", {
                     className: "pachyderm-mount-pipeline-base"
                 }, m().createElement("div", {
                     className: "pachyderm-mount-pipeline-back"
                 }, m().createElement("button", {
                     "data-testid": "Pipeline__back",
@@ -3140,51 +3160,51 @@
                     tag: "span",
                     className: "pachyderm-mount-icon-padding"
                 }))), m().createElement("span", {
                     className: "pachyderm-mount-pipeline-subheading"
                 }, "Publish as Pipeline"), m().createElement("div", {
                     className: "pachyderm-mount-pipeline-splash"
                 }, m().createElement("span", null, "Open a notebook to create a pipeline"))),
-                X = (e, t) => e > t ? 1 : e < t ? -1 : 0,
-                K = (e, t) => e - t;
-            var Q = a(4184),
-                ee = a.n(Q);
-            const te = e => {
+                K = (e, t) => e > t ? 1 : e < t ? -1 : 0,
+                Q = (e, t) => e - t;
+            var ee = a(4184),
+                te = a.n(ee);
+            const ae = e => {
                 var {
                     children: t,
                     className: a,
                     color: n = "gray"
                 } = e, r = function(e, t) {
                     var a = {};
                     for (var n in e) Object.prototype.hasOwnProperty.call(e, n) && t.indexOf(n) < 0 && (a[n] = e[n]);
                     if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
                         var r = 0;
                         for (n = Object.getOwnPropertySymbols(e); r < n.length; r++) t.indexOf(n[r]) < 0 && Object.prototype.propertyIsEnumerable.call(e, n[r]) && (a[n[r]] = e[n[r]])
                     }
                     return a
                 }(e, ["children", "className", "color"]);
-                const l = ee()("jp-circle-base", a, {
+                const l = te()("jp-circle-base", a, {
                     "jp-circle-green": "green" === n,
                     "jp-circle-red": "red" === n,
                     "jp-circle-yellow": "yellow" === n,
                     "jp-circle-gray": "gray" === n
                 });
                 return m().createElement("div", Object.assign({
                     className: l
                 }, r), t)
             };
-            const ae = ["unmounting", "mounting", "error"],
-                ne = ({
+            const ne = ["unmounting", "mounting", "error"],
+                re = ({
                     item: e,
                     open: t,
                     updateData: a
                 }) => {
                     const [n, r] = (0, o.useState)(!1), l = e.branch, s = "Unmount", i = e.how_many_commits_behind;
                     return (0, o.useEffect)((() => {
-                        r(ae.includes(e.state))
+                        r(ne.includes(e.state))
                     }), [e]), m().createElement("li", {
                         className: "pachyderm-mount-sortableList-item",
                         "data-testid": "ListItem__repo"
                     }, m().createElement("span", {
                         className: "pachyderm-mount-list-item-name-branch-wrapper " + (n ? "pachyderm-mount-sortableList-disabled" : ""),
                         onClick: () => {
                             t(e.name)
@@ -3258,27 +3278,27 @@
                             case "unmounting":
                             case "mounting":
                                 a = "yellow";
                                 break;
                             case "error":
                                 a = "red"
                         }
-                        return n = t ? `${(0,V.capitalize)(e||"Unknown")}: ${t}` : (0, V.capitalize)(e || "Unknown"), m().createElement(m().Fragment, null, m().createElement(te, {
+                        return n = t ? `${(0,V.capitalize)(e||"Unknown")}: ${t}` : (0, V.capitalize)(e || "Unknown"), m().createElement(m().Fragment, null, m().createElement(ae, {
                             color: a,
                             className: "pachyderm-mount-list-item-status-circle"
                         }), m().createElement("div", {
                             "data-testid": "ListItem__statusIcon",
                             className: "pachyderm-mount-list-item-status-icon",
                             title: n
                         }, m().createElement(y.react, {
                             tag: "span"
                         })))
                     })(e.state, e.status))))
                 };
-            const re = ({
+            const le = ({
                     item: e,
                     updateData: t,
                     mountedItems: a
                 }) => {
                     var n;
                     const [r, l] = (0, o.useState)(""), [s, i] = (0, o.useState)(!1), [c, d] = (0, o.useState)(!1), [u, h] = (0, o.useState)(!1), p = (null === (n = null == e ? void 0 : e.branches) || void 0 === n ? void 0 : n.length) > 0, f = "Mount";
                     return (0, o.useEffect)((() => {
@@ -3388,33 +3408,34 @@
                     }, m().createElement("span", {
                         className: "pachyderm-mount-list-item-name",
                         title: `${e.project}_${e.repo}`
                     }, `${e.project}_${e.repo}`), m().createElement("span", {
                         className: "pachyderm-mount-list-item-branch"
                     }, "No read access")))
                 },
-                le = {
+                se = {
                     name: "Name",
-                    func: X,
+                    func: K,
                     accessor: e => "name" in e ? e.name : `${e.project}_${e.repo}`
                 },
-                se = ({
+                ie = ({
                     open: e,
                     items: t,
                     updateData: a,
                     mountedItems: n,
-                    type: r
+                    type: r,
+                    projects: l
                 }) => {
-                    const l = "All projects",
-                        s = [...new Set(t.map((e => e.project)))],
-                        [i, c] = (0, o.useState)(l),
+                    const s = "All projects",
+                        i = l.map((e => e.project.name)),
+                        [c, d] = (0, o.useState)(s),
                         {
-                            sortedData: d,
-                            setComparator: u,
-                            reversed: h
+                            sortedData: u,
+                            setComparator: h,
+                            reversed: p
                         } = (({
                             data: e,
                             initialSort: t = {
                                 func: () => 1,
                                 name: "",
                                 accessor: e => e
                             },
@@ -3424,65 +3445,65 @@
                                 s((t => (e.name === t.name || e.reverse ? r(-1 * n) : r(1), e)))
                             }), [n]);
                             return {
                                 sortedData: (0, o.useMemo)((() => [...e].sort(((e, t) => n * l.func(l.accessor(e), l.accessor(t))))), [l, e, n]),
                                 reversed: -1 === n,
                                 setComparator: i,
                                 comparatorName: l.name,
-                                numberComparator: K,
-                                stringComparator: X
+                                numberComparator: Q,
+                                stringComparator: K
                             }
                         })({
                             data: t,
-                            initialSort: le,
+                            initialSort: se,
                             initialDirection: 1
                         }),
-                        p = (0, o.useCallback)((() => {
-                            u(le)
-                        }), [u]);
+                        f = (0, o.useCallback)((() => {
+                            h(se)
+                        }), [h]);
                     return m().createElement("div", {
                         className: "pachyderm-mount-sortableList"
                     }, "unmounted" === r && m().createElement("div", {
                         className: "pachyderm-mount-sortableList-projectFilter"
                     }, m().createElement("div", {
                         className: "pachyderm-mount-projectFilter-headerItem"
                     }, m().createElement("span", null, "Project: "), m().createElement("select", {
                         name: "project",
-                        value: i,
+                        value: c,
                         className: "pachyderm-mount-project-list-select",
                         onChange: e => {
-                            c(e.target.value)
+                            d(e.target.value)
                         },
                         "data-testid": "ProjectList__select"
                     }, m().createElement("option", {
-                        key: l,
-                        value: l
-                    }, l), s.map((e => m().createElement("option", {
+                        key: s,
+                        value: s
+                    }, s), i.map((e => m().createElement("option", {
                         key: e,
                         value: e
                     }, e)))))), m().createElement("div", {
                         className: "pachyderm-mount-sortableList-header"
                     }, m().createElement("div", {
                         className: "pachyderm-mount-sortableList-headerItem",
-                        onClick: p
-                    }, m().createElement("span", null, "Name"), m().createElement("span", null, h ? m().createElement(g.caretDownIcon.react, null) : m().createElement(g.caretUpIcon.react, null)))), m().createElement("ul", {
+                        onClick: f
+                    }, m().createElement("span", null, "Name"), m().createElement("span", null, p ? m().createElement(g.caretDownIcon.react, null) : m().createElement(g.caretUpIcon.react, null)))), m().createElement("ul", {
                         className: "pachyderm-mount-sortableList-content"
-                    }, d && d.map((t => "name" in t ? m().createElement(ne, {
+                    }, u && u.map((t => "name" in t ? m().createElement(re, {
                         item: t,
                         key: t.name,
                         open: e,
                         updateData: a
-                    }) : (i === t.project || i === l) && m().createElement(re, {
+                    }) : (c === t.project || c === s) && m().createElement(le, {
                         item: t,
                         key: `${t.project}_${t.repo}`,
                         updateData: a,
                         mountedItems: n
                     })))))
                 },
-                ie = e => o.createElement("svg", Object.assign({
+                ce = e => o.createElement("svg", Object.assign({
                     xmlns: "http://www.w3.org/2000/svg",
                     width: 400,
                     height: 180,
                     viewBox: "320 -20 180 270",
                     xmlnsXlink: "http://www.w3.org/1999/xlink"
                 }, e), o.createElement("defs", null, o.createElement("path", {
                     id: "genericError_svg__b",
@@ -3997,56 +4018,56 @@
                     d: "M142.52 208.32 154 228.48h-22.96z"
                 }), o.createElement("path", {
                     d: "M607.04 74.706c1.237 0 2.24-1.12 2.24-2.501 0-.921-.747-2.7-2.24-5.34-1.493 2.64-2.24 4.419-2.24 5.34 0 1.381 1.003 2.5 2.24 2.5zm-5.6-11.2c1.237 0 2.24-1.12 2.24-2.501 0-.921-.747-2.7-2.24-5.34-1.493 2.64-2.24 4.419-2.24 5.34 0 1.381 1.003 2.5 2.24 2.5z",
                     stroke: "#26101A",
                     strokeWidth: 1.4,
                     fill: "#C3E5D7"
                 }))),
-                ce = e => o.createElement("svg", Object.assign({
+                oe = e => o.createElement("svg", Object.assign({
                     width: 20,
                     height: 20,
                     xmlns: "http://www.w3.org/2000/svg",
                     viewBox: "0 0 16 16"
                 }, e), o.createElement("g", {
                     fill: "none",
                     fillRule: "evenodd"
                 }, o.createElement("path", {
                     d: "M0 0h16v16H0z"
                 }), o.createElement("path", {
                     d: "M8 0a8 8 0 1 1 0 16A8 8 0 0 1 8 0Zm0 11.65a1.2 1.2 0 1 0 0 2.4 1.2 1.2 0 0 0 0-2.4Zm0-9.7a1.2 1.2 0 0 0-1.2 1.2v5.6a1.2 1.2 0 1 0 2.4 0v-5.6A1.2 1.2 0 0 0 8 1.95Z",
                     fill: "#BF444F"
                 }))),
-                oe = ({
+                me = ({
                     status: e
                 }) => m().createElement("div", {
                     className: "pachyderm-mount-base",
                     style: {
                         display: "flex",
                         flexDirection: "column",
                         alignItems: "center",
                         justifyContent: "center"
                     }
-                }, m().createElement("div", null, m().createElement(ie, {
+                }, m().createElement("div", null, m().createElement(ce, {
                     width: "280px",
                     height: "130px"
                 })), m().createElement("div", {
                     style: {
                         display: "flex",
                         flexDirection: "row",
                         alignItems: "center",
                         paddingBottom: "1rem"
                     }
-                }, m().createElement(ce, null), m().createElement("span", {
+                }, m().createElement(oe, null), m().createElement("span", {
                     style: {
                         paddingLeft: ".5rem"
                     }
                 }, "Looks like there was an error")), m().createElement("div", {
                     "data-testid": "FullPageError__message"
                 }, e.message));
-            var me = function(e, t, a, n) {
+            var de = function(e, t, a, n) {
                 return new(a || (a = Promise))((function(r, l) {
                     function s(e) {
                         try {
                             c(n.next(e))
                         } catch (e) {
                             l(e)
                         }
@@ -4065,61 +4086,61 @@
                         e.done ? r(e.value) : (t = e.value, t instanceof a ? t : new a((function(e) {
                             e(t)
                         }))).then(s, i)
                     }
                     c((n = n.apply(e, t || [])).next())
                 }))
             };
-            const de = "mount-browser:",
-                ue = "pachyderm_pps";
-            class he {
+            const ue = "mount-browser:",
+                he = "pachyderm_pps";
+            class pe {
                 constructor(e, t, a, n, r, l) {
-                    this._showConfig = !1, this._showConfigSignal = new B.Signal(this), this._readyPromise = Promise.resolve(), this._showDatum = !1, this._showPipeline = !1, this._keepMounted = !1, this._showDatumSignal = new B.Signal(this), this._repoViewInputSpec = {}, this._saveInputSpecSignal = new B.Signal(this), this._showPipelineSignal = new B.Signal(this), this._ppsContextSignal = new B.Signal(this), this.isCurrentWidgetNotebook = e => (e = null != e ? e : this._widgetTracker.currentWidget) instanceof L.NotebookPanel, this.getActiveNotebook = () => {
+                    this._showConfig = !1, this._showConfigSignal = new N.Signal(this), this._readyPromise = Promise.resolve(), this._showDatum = !1, this._showPipeline = !1, this._keepMounted = !1, this._showDatumSignal = new N.Signal(this), this._repoViewInputSpec = {}, this._saveInputSpecSignal = new N.Signal(this), this._showPipelineSignal = new N.Signal(this), this._ppsContextSignal = new N.Signal(this), this.isCurrentWidgetNotebook = e => (e = null != e ? e : this._widgetTracker.currentWidget) instanceof L.NotebookPanel, this.getActiveNotebook = () => {
                         const e = this._widgetTracker.currentWidget;
                         return this.isCurrentWidgetNotebook(e) ? e : null
-                    }, this.handleWidgetChanged = (e, t) => me(this, void 0, void 0, (function*() {
+                    }, this.handleWidgetChanged = (e, t) => de(this, void 0, void 0, (function*() {
                         this.isCurrentWidgetNotebook(t.newValue) && (yield this.handleNotebookChanged(t.newValue)), this.setShowPipeline(this._showPipeline), yield Promise.resolve()
-                    })), this.handleNotebookChanged = e => me(this, void 0, void 0, (function*() {
+                    })), this.handleNotebookChanged = e => de(this, void 0, void 0, (function*() {
                         yield e.sessionContext.ready, e.context.fileChanged.connect(this.handleNotebookReload);
                         const t = {
                             metadata: this.getNotebookMetadata(e),
                             notebookModel: e.context.contentsModel
                         };
                         this._ppsContextSignal.emit(t), yield Promise.resolve()
-                    })), this.handleNotebookReload = (e, t) => me(this, void 0, void 0, (function*() {
+                    })), this.handleNotebookReload = (e, t) => de(this, void 0, void 0, (function*() {
                         const e = {
                             metadata: this.getNotebookMetadata(),
                             notebookModel: t
                         };
                         this._ppsContextSignal.emit(e), yield Promise.resolve()
                     })), this.getNotebookMetadata = e => {
                         var t;
-                        return null === (t = null == (e = null != e ? e : this.getActiveNotebook()) ? void 0 : e.model) || void 0 === t ? void 0 : t.metadata.get(ue)
+                        return null === (t = null == (e = null != e ? e : this.getActiveNotebook()) ? void 0 : e.model) || void 0 === t ? void 0 : t.metadata.get(he)
                     }, this.saveNotebookMetadata = e => {
                         var t;
                         const a = this.getActiveNotebook();
-                        null !== a ? (null === (t = null == a ? void 0 : a.model) || void 0 === t || t.metadata.set(ue, e), console.log("notebook metadata saved")) : console.log("No active notebook")
-                    }, this.saveNotebookToDisk = () => me(this, void 0, void 0, (function*() {
+                        null !== a ? (null === (t = null == a ? void 0 : a.model) || void 0 === t || t.metadata.set(he, e), console.log("notebook metadata saved")) : console.log("No active notebook")
+                    }, this.saveNotebookToDisk = () => de(this, void 0, void 0, (function*() {
                         const e = this.getActiveNotebook();
                         return null !== e ? (yield e.context.ready, yield e.context.save(), yield e.context.ready, e.context.contentsModel.last_modified) : null
                     })), this.open = e => {
                         this._app.commands.execute("filebrowser:open-path", {
-                            path: de + e
+                            path: ue + e
                         })
-                    }, this.refresh = (e, t) => me(this, void 0, void 0, (function*() {
+                    }, this.refresh = (e, t) => de(this, void 0, void 0, (function*() {
                         yield this._mountBrowser.model.refresh()
                     })), this.verifyBrowserPath = (e, t) => {
                         this._mountBrowser.model.path !== this._mountBrowser.model.rootPath && (this.isValidBrowserPath(this._mountBrowser.model.path, t) || this.open(""))
                     }, this.isValidBrowserPath = (e, t) => {
-                        const a = e.split(de)[1].split("/")[0];
+                        const a = e.split(ue)[1].split("/")[0];
                         if ("out" === a) return !0;
                         for (let e = 0; e < t.length; e++)
                             if (a === t[e].name) return !0;
                         return !1
-                    }, this.setShowDatum = e => me(this, void 0, void 0, (function*() {
+                    }, this.setShowDatum = e => de(this, void 0, void 0, (function*() {
                         e ? (this._datum.setHidden(!1), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this.saveMountedReposList()) : (this._datum.setHidden(!0), this._mountedList.setHidden(!1), this._unmountedList.setHidden(!1), yield this.restoreMountedReposList()), this._mountBrowser.setHidden(!1), this._config.setHidden(!0), this._pipeline.setHidden(!0), this._fullPageError.setHidden(!0), this._showDatum = e, this._showDatumSignal.emit(e)
                     })), this.saveMountedReposList = () => {
                         const e = this._poller.mounted,
                             t = [];
                         for (let a = 0; a < e.length; a++) {
                             const n = {
                                 pfs: Object.assign(Object.assign(Object.assign(Object.assign(Object.assign({
@@ -4137,15 +4158,15 @@
                                 })
                             };
                             t.push(n)
                         }
                         0 === e.length ? this._repoViewInputSpec = {} : 1 === e.length ? this._repoViewInputSpec = t[0] : this._repoViewInputSpec = {
                             cross: t
                         }, this._saveInputSpecSignal.emit(this._repoViewInputSpec)
-                    }, this.restoreMountedReposList = () => me(this, void 0, void 0, (function*() {
+                    }, this.restoreMountedReposList = () => de(this, void 0, void 0, (function*() {
                         const e = [];
                         if (Object.prototype.hasOwnProperty.call(this._repoViewInputSpec, "cross") && Array.isArray(this._repoViewInputSpec.cross))
                             for (let t = 0; t < this._repoViewInputSpec.cross.length; t++) {
                                 const a = this._repoViewInputSpec.cross[t].pfs;
                                 e.push({
                                     name: a.name ? a.name : a.repo,
                                     repo: a.repo,
@@ -4175,15 +4196,15 @@
                         this._keepMounted = e
                     }, this.setShowConfig = e => {
                         e ? (this._config.setHidden(!1), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this._mountBrowser.setHidden(!0)) : (this._config.setHidden(!0), this._mountedList.setHidden(!1), this._unmountedList.setHidden(!1), this._mountBrowser.setHidden(!1)), this._datum.setHidden(!0), this._pipeline.setHidden(!0), this._fullPageError.setHidden(!0), this._showConfig = e, this._showConfigSignal.emit(e)
                     }, this.setShowFullPageError = e => {
                         e ? (this._fullPageError.setHidden(!1), this._config.setHidden(!0), this._datum.setHidden(!0), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this._mountBrowser.setHidden(!0), this._pipeline.setHidden(!0)) : (this._fullPageError.setHidden(!0), this._config.setHidden(!1), this._datum.setHidden(!1), this._mountedList.setHidden(!1), this._unmountedList.setHidden(!1), this._mountBrowser.setHidden(!1), this._pipeline.setHidden(!1))
                     }, this.updateConfig = e => {
                         this._poller.config = e
-                    }, this.setup = () => me(this, void 0, void 0, (function*() {
+                    }, this.setup = () => de(this, void 0, void 0, (function*() {
                         if (yield this._poller.refresh(), 500 === this._poller.status.code) this.setShowFullPageError(!0);
                         else if (this.setShowConfig("INVALID" === this._poller.config.cluster_status || 200 !== this._poller.status.code), 200 === this._poller.status.code) try {
                             const e = yield D("datums", "GET");
                             e.num_datums > 0 && (this._keepMounted = !0, this._currentDatumInfo = e, yield this.setShowDatum(!0))
                         } catch (e) {
                             console.log(e)
                         }
@@ -4227,102 +4248,106 @@
                         className: "pachyderm-button-alpha-notice"
                     }, "Alpha")), m().createElement("button", {
                         className: "pachyderm-button-link",
                         onClick: () => this.setShowConfig(!0)
                     }, m().createElement(g.settingsIcon.react, {
                         tag: "span",
                         className: "pachyderm-mount-icon-padding"
-                    }))), m().createElement(se, {
+                    }))), m().createElement(ie, {
                         open: this.open,
                         items: t || this._poller.mounted,
                         updateData: this._poller.updateData,
                         mountedItems: [],
-                        type: "mounted"
+                        type: "mounted",
+                        projects: []
                     }))))), this._mountedList.addClass("pachyderm-mount-react-wrapper"), this._unmountedList = d.ReactWidget.create(m().createElement(d.UseSignal, {
                         signal: this._poller.unmountedSignal
-                    }, ((e, t) => m().createElement("div", {
+                    }, ((e, t) => m().createElement(d.UseSignal, {
+                        signal: this._poller.projectSignal
+                    }, ((e, a) => m().createElement("div", {
                         className: "pachyderm-mount-base"
                     }, m().createElement("div", {
                         className: "pachyderm-mount-base-title"
-                    }, "Unmounted Repositories"), m().createElement(se, {
+                    }, "Unmounted Repositories"), m().createElement(ie, {
                         open: this.open,
                         items: t || this._poller.unmounted,
                         updateData: this._poller.updateData,
                         mountedItems: this._poller.mounted,
-                        type: "unmounted"
-                    }))))), this._unmountedList.addClass("pachyderm-mount-react-wrapper"), this._datum = d.ReactWidget.create(m().createElement(d.UseSignal, {
+                        type: "unmounted",
+                        projects: a || this._poller.projects
+                    }))))))), this._unmountedList.addClass("pachyderm-mount-react-wrapper"), this._datum = d.ReactWidget.create(m().createElement(d.UseSignal, {
                         signal: this._showDatumSignal
                     }, ((e, t) => m().createElement(d.UseSignal, {
                         signal: this._saveInputSpecSignal
                     }, ((e, a) => m().createElement(Z, {
                         showDatum: t || this._showDatum,
                         setShowDatum: this.setShowDatum,
                         keepMounted: this._keepMounted,
                         setKeepMounted: this.setKeepMounted,
                         open: this.open,
                         pollRefresh: this._poller.refresh,
                         currentDatumInfo: this._currentDatumInfo,
                         repoViewInputSpec: a || this._repoViewInputSpec
                     })))))), this._datum.addClass("pachyderm-mount-datum-wrapper"), this._pipeline = d.ReactWidget.create(m().createElement(d.UseSignal, {
                         signal: this._ppsContextSignal
-                    }, ((e, a) => m().createElement(q, {
+                    }, ((e, a) => m().createElement(Y, {
                         ppsContext: a,
                         settings: t,
                         setShowPipeline: this.setShowPipeline,
                         saveNotebookMetadata: this.saveNotebookMetadata,
                         saveNotebookToDisk: this.saveNotebookToDisk
-                    })))), this._pipelineSplash = d.ReactWidget.create(m().createElement(Y, {
+                    })))), this._pipelineSplash = d.ReactWidget.create(m().createElement(X, {
                         setShowPipeline: this.setShowPipeline
                     })), this._pipeline.addClass("pachyderm-mount-pipeline-wrapper"), this._pipelineSplash.addClass("pachyderm-mount-pipeline-wrapper"), this._loader = d.ReactWidget.create(m().createElement(W, null)), this._loader.addClass("pachyderm-mount-react-wrapper"), this._fullPageError = d.ReactWidget.create(m().createElement(d.UseSignal, {
                         signal: this._poller.statusSignal
-                    }, ((e, t) => m().createElement(oe, {
+                    }, ((e, t) => m().createElement(me, {
                         status: t || this._poller.status
                     })))), this._fullPageError.addClass("pachyderm-mount-react-wrapper"), this._mountBrowser = ((e, t, a) => {
                         var n;
-                        const r = new P(e.docRegistry);
+                        const r = new H(e.docRegistry);
                         t.services.contents.addDrive(r);
                         const l = a.createFileBrowser("jupyterlab-pachyderm-browser", {
                             driveName: r.name,
                             state: null,
                             refreshInterval: 1e4
                         });
                         try {
                             const e = l.toolbar.node.childNodes[0],
                                 a = l.toolbar.node.childNodes[1];
                             l.toolbar.node.removeChild(e), l.toolbar.node.removeChild(a);
                             const r = l.layout.widgets || [],
-                                s = r.find((e => e instanceof z.BreadCrumbs));
+                                s = r.find((e => e instanceof S.BreadCrumbs));
                             if (s) {
                                 null === (n = s.node.querySelector('svg[data-icon="ui-components:folder"]')) || void 0 === n || n.replaceWith("/ pfs");
                                 const e = s.node.querySelector('span[title="~/extension-wd"]');
                                 e && (e.className = "jp-BreadCrumbs-item")
                             }
-                            const i = r.find((e => e instanceof z.DirListing));
+                            const i = r.find((e => e instanceof S.DirListing));
                             if (i) {
                                 const e = new j.CommandRegistry;
                                 e.addCommand("file-open", {
                                     label: "Open",
                                     icon: "fa fa-folder",
                                     mnemonic: 0,
                                     execute: () => {
-                                        (0, H.each)(l.selectedItems(), (e => {
+                                        (0, P.each)(l.selectedItems(), (e => {
                                             t.openOrReveal(e.path)
                                         }))
                                     }
                                 }), e.addCommand("copy-path", {
                                     label: "Copy Path",
                                     icon: "fa fa-file",
                                     mnemonic: 0,
                                     execute: () => {
-                                        (0, H.each)(l.selectedItems(), (e => {
-                                            d.Clipboard.copyToSystem(e.path.replace(de, "/pfs/"))
+                                        (0, P.each)(l.selectedItems(), (e => {
+                                            d.Clipboard.copyToSystem(e.path.replace(ue, "/pfs/"))
                                         }))
                                     }
                                 });
-                                const a = new N.Menu({
+                                const a = new B.Menu({
                                     commands: e
                                 });
                                 a.addItem({
                                     command: "file-open"
                                 }), a.addItem({
                                     command: "copy-path"
                                 }), i.node.getElementsByClassName("jp-DirListing-content")[0].addEventListener("contextmenu", (e => {
@@ -4332,15 +4357,15 @@
                                     a.open(t, n)
                                 }))
                             }
                         } catch (e) {
                             console.log("Failed to edit default browser.")
                         }
                         return l
-                    })(e, a, n), this._poller.mountedSignal.connect(this.verifyBrowserPath), this._poller.mountedSignal.connect(this.refresh), this._poller.unmountedSignal.connect(this.refresh), this._widgetTracker.currentChanged.connect(this.handleWidgetChanged, this), this._panel = new N.SplitPanel, this._panel.orientation = "vertical", this._panel.spacing = 0, this._panel.title.icon = k, this._panel.title.caption = "Pachyderm Mount", this._panel.id = "pachyderm-mount", this._panel.addWidget(this._mountedList), this._panel.addWidget(this._unmountedList), this._panel.addWidget(this._datum), this._panel.addWidget(this._pipelineSplash), this._panel.addWidget(this._pipeline), this._panel.addWidget(this._mountBrowser), this._panel.setRelativeSizes([1, 1, 3, 3]), this._panel.addWidget(this._loader), this._panel.addWidget(this._config), this._panel.addWidget(this._fullPageError), this._config.setHidden(!0), this._fullPageError.setHidden(!0), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this._datum.setHidden(!0), this._pipelineSplash.setHidden(!0), this._pipeline.setHidden(!0), this._mountBrowser.setHidden(!0), window.addEventListener("resize", (() => {
+                    })(e, a, n), this._poller.mountedSignal.connect(this.verifyBrowserPath), this._poller.mountedSignal.connect(this.refresh), this._poller.unmountedSignal.connect(this.refresh), this._widgetTracker.currentChanged.connect(this.handleWidgetChanged, this), this._panel = new B.SplitPanel, this._panel.orientation = "vertical", this._panel.spacing = 0, this._panel.title.icon = k, this._panel.title.caption = "Pachyderm Mount", this._panel.id = "pachyderm-mount", this._panel.addWidget(this._mountedList), this._panel.addWidget(this._unmountedList), this._panel.addWidget(this._datum), this._panel.addWidget(this._pipelineSplash), this._panel.addWidget(this._pipeline), this._panel.addWidget(this._mountBrowser), this._panel.setRelativeSizes([1, 1, 3, 3]), this._panel.addWidget(this._loader), this._panel.addWidget(this._config), this._panel.addWidget(this._fullPageError), this._config.setHidden(!0), this._fullPageError.setHidden(!0), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this._datum.setHidden(!0), this._pipelineSplash.setHidden(!0), this._pipeline.setHidden(!0), this._mountBrowser.setHidden(!0), window.addEventListener("resize", (() => {
                         this._panel.update()
                     })), r.add(this._panel, "jupyterlab-pachyderm"), e.shell.add(this._panel, "left", {
                         rank: 100
                     })
                 }
                 get mountedRepos() {
                     return this._poller.poll.tick, this._poller.mounted
@@ -4351,27 +4376,27 @@
                 get layout() {
                     return this._panel
                 }
                 get ready() {
                     return this._readyPromise
                 }
             }
-            const pe = "jupyterlab-pachyderm:mount",
-                fe = [{
-                    id: pe,
+            const fe = "jupyterlab-pachyderm:mount",
+                Ee = [{
+                    id: fe,
                     autoStart: !0,
-                    requires: [M.IDocumentManager, z.IFileBrowserFactory, C.ILayoutRestorer, C.ILabShell, S.ISettingRegistry],
+                    requires: [M.IDocumentManager, S.IFileBrowserFactory, C.ILayoutRestorer, C.ILabShell, z.ISettingRegistry],
                     activate: (e, t, a, n, r, l) => {
                         const s = {
                                 defaultPipelineImage: ""
                             },
                             i = e => {
                                 s.defaultPipelineImage = e.get("defaultPipelineImage").composite
                             };
-                        return Promise.all([l.load(pe), e.restored]).then((([e]) => {
+                        return Promise.all([l.load(fe), e.restored]).then((([e]) => {
                             i(e), e.changed.connect(i)
-                        })), new he(e, s, t, a, n, r)
+                        })), new pe(e, s, t, a, n, r)
                     }
                 }, i, p, x]
         }
     }
 ]);
```

### Comparing `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/remoteEntry.d9811dd3652ac1fc0383.js` & `jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/static/remoteEntry.472bd5c5853eeaa9de7a.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -49,22 +49,22 @@
         })
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         67: "9d3e2934cfe0e102619e",
         371: "8ac933b7fbb0f688b6f4",
         486: "003d1d2cc9cc6927471e",
         676: "95f9b834e9f9b133c00b",
         747: "b62f963856036a13fba1",
-        829: "0234ec6e026820778750"
+        829: "75c9ab3fc9e1a8c63de6"
     } [e] + ".js?v=" + {
         67: "9d3e2934cfe0e102619e",
         371: "8ac933b7fbb0f688b6f4",
         486: "003d1d2cc9cc6927471e",
         676: "95f9b834e9f9b133c00b",
         747: "b62f963856036a13fba1",
-        829: "0234ec6e026820778750"
+        829: "75c9ab3fc9e1a8c63de6"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -116,15 +116,15 @@
                         (!u || !u.loaded && (!a != !u.eager ? a : l > u.from)) && (n[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     i = [];
-                return "default" === t && (u("jupyterlab-pachyderm", "2.6.1", (() => Promise.all([j.e(371), j.e(829)]).then((() => () => j(7363))))), u("lodash", "4.17.21", (() => j.e(486).then((() => () => j(6486))))), u("rudder-sdk-js", "1.2.5", (() => j.e(67).then((() => () => j(3067))))), u("yaml", "0", (() => j.e(676).then((() => () => j(5676)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("jupyterlab-pachyderm", "2.7.0-alpha.1", (() => Promise.all([j.e(371), j.e(829)]).then((() => () => j(7363))))), u("lodash", "4.17.21", (() => j.e(486).then((() => () => j(6486))))), u("rudder-sdk-js", "1.2.5", (() => j.e(67).then((() => () => j(3067))))), u("yaml", "0", (() => j.e(676).then((() => () => j(5676)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/third-party-licenses.json` & `jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/mount_server_client.py` & `jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/mount_server_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,19 @@
         response = await self.client.fetch(f"{self.address}/repos")
         return response.body
 
     async def list_mounts(self):
         await self._ensure_mount_server()
         response = await self.client.fetch(f"{self.address}/mounts")
         return response.body
+
+    async def list_projects(self):
+        await self._ensure_mount_server()
+        response = await self.client.fetch(f"{self.address}/projects")
+        return response.body
         
     async def mount(self, body):
         await self._ensure_mount_server()
         response = await self.client.fetch(
             f"{self.address}/_mount",
             method="PUT",
             body=json.dumps(body),
```

### Comparing `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/pachyderm.py` & `jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/pachyderm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 class MountInterface:
     async def list_repos(self):
         pass
 
     async def list_mounts(self):
         pass
 
+    async def list_projects(self):
+        pass
+
     async def mount(self, body):
         pass
 
     async def unmount(self, body):
         pass
 
     async def commit(self, body):
```

### Comparing `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/pps_client.py` & `jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/pps_client.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb` & `jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/tests/test_handlers.py` & `jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/tests/test_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -548,14 +548,36 @@
     response = await jp_fetch(f"/{NAMESPACE}/{VERSION}/pps/_create/{notebook_path}")
     assert response.code == 200
     body = json.loads(response.body)
     for expected_key in ("pipeline", "description", "transform", "input"):
         assert expected_key in body
 
 
+@pytest.mark.skipif(sys.version_info < (3, 7), reason="requires python3.7 or higher")
+@patch(
+    "jupyterlab_pachyderm.handlers.ProjectsHandler.mount_client",
+    spec=MountInterface,
+)
+async def test_get_projects(mock_client, jp_fetch):
+    test_projects = [
+        {
+            "project": {"name": "default"},
+            "auth_info":{"permissions": [1, 2, 3], "roles": ["clusterAdmin", "projectOwner"]}
+        },
+        {
+            "project": {"name": "p1"},
+            "auth_info":{"permissions": [4, 5, 6], "roles": ["test"]}
+        }
+    ]
+
+    mock_client.list_projects.return_value = json.dumps(test_projects)
+    resp = await jp_fetch(f"/{NAMESPACE}/{VERSION}/projects")
+    assert json.loads(resp.body) == test_projects
+
+
 async def test_write_token_to_config_no_context():
     timestamp = time.time_ns()
     test_config_path = f"/tmp/pach_test_config_{timestamp}.json"
 
     # test non-existent context
     # we expect the entire context to be copied
     test_mount_server_config_str = """{
```

### Comparing `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/tests/test_integrations.py` & `jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/tests/test_integrations.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm.egg-info/PKG-INFO` & `jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-pachyderm
-Version: 2.6.1
+Version: 2.7.0a1
 Summary: A JupyterLab extension.
 Home-page: https://github.com/pachyderm/jupyterlab-pachyderm
 Author: 
 Author-email: 
 License: BSD-3-Clause
 Keywords: jupyter,jupyterlab,jupyterlab-extension
 Platform: Linux
```

### Comparing `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm.egg-info/SOURCES.txt` & `jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
 jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
 jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
 jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
 jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
 jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
 jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js
-jupyterlab_pachyderm/labextension/static/829.0234ec6e026820778750.js
-jupyterlab_pachyderm/labextension/static/remoteEntry.d9811dd3652ac1fc0383.js
+jupyterlab_pachyderm/labextension/static/829.75c9ab3fc9e1a8c63de6.js
+jupyterlab_pachyderm/labextension/static/remoteEntry.472bd5c5853eeaa9de7a.js
 jupyterlab_pachyderm/labextension/static/style.js
 jupyterlab_pachyderm/labextension/static/third-party-licenses.json
 jupyterlab_pachyderm/tests/__init__.py
 jupyterlab_pachyderm/tests/test_handlers.py
 jupyterlab_pachyderm/tests/test_integrations.py
 jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
 jupyterlab_pachyderm/tests/data/requirements.txt
```

### Comparing `jupyterlab_pachyderm-2.6.1/package.json` & `jupyterlab_pachyderm-2.7.0a1/jupyterlab_pachyderm/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222223%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.472bd5c5853eeaa9de7a.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'2.7.0-alpha.1'"}*

```diff
@@ -66,14 +66,19 @@
             "before-build-npm": [
                 "python -m pip install jupyterlab~=3.1",
                 "npm"
             ]
         }
     },
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.472bd5c5853eeaa9de7a.js",
+            "style": "./style"
+        },
         "disabledExtensions": [
             "jupyterlab-pachyderm:examples"
         ],
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyterlab_pachyderm"
@@ -128,9 +133,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.6.1"
+    "version": "2.7.0-alpha.1"
 }
```

### Comparing `jupyterlab_pachyderm-2.6.1/pyproject.toml` & `jupyterlab_pachyderm-2.7.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/setup.cfg` & `jupyterlab_pachyderm-2.7.0a1/setup.cfg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/setup.py` & `jupyterlab_pachyderm-2.7.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/handler.ts` & `jupyterlab_pachyderm-2.7.0a1/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/examples/__test__/examples.test.tsx` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/examples/__test__/examples.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/examples/examples.tsx` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/examples/examples.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/help/__tests__/help.test.ts` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/help/__tests__/help.test.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/help/help.tsx` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/help/help.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/mount/__tests__/mount.test.tsx` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/__tests__/mount.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Config/Config.tsx` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Config/Config.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Config/__tests__/Config.test.tsx` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Config/__tests__/Config.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Config/hooks/useConfig.tsx` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Config/hooks/useConfig.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Datum/Datum.tsx` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Datum/Datum.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Datum/hooks/useDatum.tsx` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Datum/hooks/useDatum.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/FullPageError/FullPageError.tsx` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/FullPageError/FullPageError.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Pipeline/Pipeline.tsx` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Pipeline/Pipeline.tsx`

 * *Files 4% similar despite different names*

```diff
@@ -14,26 +14,29 @@
 const placeholderInputSpec = `# example:
 pfs:
   repo: images
   branch: dev
   glob: /*
 `;
 const placeholderRequirements = './requirements.txt';
+const placeholderProject = 'default';
 
 const Pipeline: React.FC<PipelineProps> = ({
   ppsContext,
   settings,
   setShowPipeline,
   saveNotebookMetadata,
   saveNotebookToDisk,
 }) => {
   const {
     loading,
-    pipeline,
-    setPipeline,
+    pipelineName,
+    setPipelineName,
+    pipelineProject,
+    setPipelineProject,
     imageName,
     setImageName,
     inputSpec,
     setInputSpec,
     requirements,
     setRequirements,
     callCreatePipeline,
@@ -90,26 +93,41 @@
         >
           *Pipeline Name:{'  '}
         </label>
         <input
           className="pachyderm-pipeline-input"
           data-testid="Pipeline__inputPipelineName"
           name="pipelineName"
-          value={
-            pipeline.project?.name
-              ? `${pipeline.project.name}/${pipeline.name}`
-              : pipeline.name
-          }
+          value={pipelineName}
           onChange={(e: any) => {
-            setPipeline(e.target.value);
+            setPipelineName(e.target.value);
           }}
           disabled={loading}
         ></input>
       </div>
       <div className="pachyderm-pipeline-input-wrapper">
+        <label
+          className="pachyderm-pipeline-input-label"
+          htmlFor="pipelineProjectName"
+        >
+          Pipeline Project Name:{'  '}
+        </label>
+        <input
+          className="pachyderm-pipeline-input"
+          data-testid="Pipeline__inputPipelineProjectName"
+          name="pipelineName"
+          value={pipelineProject}
+          onChange={(e: any) => {
+            setPipelineProject(e.target.value);
+          }}
+          disabled={loading}
+          placeholder={placeholderProject}
+        ></input>
+      </div>
+      <div className="pachyderm-pipeline-input-wrapper">
         <label className="pachyderm-pipeline-input-label" htmlFor="imageName">
           *Container Image Name:{'  '}
         </label>
         <input
           className="pachyderm-pipeline-input"
           data-testid="Pipeline__inputImageName"
           name="imageName"
@@ -165,16 +183,16 @@
         </label>
         <textarea
           className="pachyderm-pipeline-spec-preview-textarea"
           style={{backgroundColor: '#80808080'}}
           data-testid="Pipeline__specPreview"
           name="specPreview"
           value={`pipeline:
-  name: ${pipeline.name}
-  project: ${pipeline.project?.name ?? 'default'}
+  name: ${pipelineName}
+  project: ${pipelineProject || placeholderProject}
 transform:
   image: ${imageName}
 input:
 ${inputSpec
   .split('\n')
   .map((line, _, __) => '  ' + line)
   .join('\n')}
```

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Pipeline/Splash.tsx` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Pipeline/Splash.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import {render} from '@testing-library/react';
 import userEvent from '@testing-library/user-event';
 import {Contents} from '@jupyterlab/services';
 
 import * as requestAPI from '../../../../../handler';
 import {mockedRequestAPI} from 'utils/testUtils';
 import Pipeline from '../Pipeline';
-import {splitAtFirstSlash} from '../hooks/usePipeline';
 
 jest.mock('../../../../../handler');
 import {MountSettings} from '../../../types';
 
 describe('PPS screen', () => {
   let setShowPipeline = jest.fn();
   const saveNotebookMetaData = jest.fn();
@@ -43,15 +42,20 @@
         'Pipeline__currentNotebookValue',
       );
       expect(valueCurrentNotebook).toHaveTextContent(testNotebookName);
 
       const inputPipelineName = await findByTestId(
         'Pipeline__inputPipelineName',
       );
-      userEvent.type(inputPipelineName, 'test_project/ThisPipelineIsNamedFred');
+      userEvent.type(inputPipelineName, 'ThisPipelineIsNamedFred');
+
+      const inputPipelineProject = await findByTestId(
+        'Pipeline__inputPipelineProjectName',
+      );
+      userEvent.type(inputPipelineProject, 'test_project');
 
       const inputImageName = await findByTestId('Pipeline__inputImageName');
       expect(inputImageName).toHaveValue(settings.defaultPipelineImage);
       userEvent.clear(inputImageName);
       userEvent.type(inputImageName, 'ThisImageIsNamedLucy');
 
       const inputRequirements = await findByTestId(
@@ -103,21 +107,7 @@
       const valueCurrentNotebook = await findByTestId(
         'Pipeline__currentNotebookValue',
       );
       expect(valueCurrentNotebook).toHaveTextContent('None');
     });
   });
 });
-
-describe('unit tests for helper functions', () => {
-  it('splitAtFirstSlash', () => {
-    expect(splitAtFirstSlash('name')).toStrictEqual(['name']);
-    expect(splitAtFirstSlash('first/second')).toStrictEqual([
-      'first',
-      'second',
-    ]);
-    expect(splitAtFirstSlash('first/second/third')).toStrictEqual([
-      'first',
-      'second/third',
-    ]);
-  });
-});
```

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/SortableList/ListMount.tsx` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/SortableList/ListMount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/SortableList/ListUnmount.tsx` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/SortableList/ListUnmount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/SortableList/SortableList.tsx` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/SortableList/SortableList.tsx`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 import React, {useCallback, useState} from 'react';
-import {Repo, Mount, ListMountsResponse} from '../../types';
+import {
+  Repo,
+  Mount,
+  ListMountsResponse,
+  Project,
+  ProjectInfo,
+} from '../../types';
 import {caretUpIcon, caretDownIcon} from '@jupyterlab/ui-components';
 import {useSort, stringComparator} from '../../../../utils/hooks/useSort';
 import ListMount from './ListMount';
 import ListUnmount from './ListUnmount';
 
 type SortableListProps = {
   items: Array<Mount | Repo>;
   open: (path: string) => void;
   updateData: (data: ListMountsResponse) => void;
   mountedItems: Mount[];
   type: string;
+  projects: ProjectInfo[];
 };
 
 const nameComparator = {
   name: 'Name',
   func: stringComparator,
   accessor: (item: Mount | Repo) =>
     'name' in item ? item.name : `${item.project}_${item.repo}`,
@@ -22,19 +29,20 @@
 
 const SortableList: React.FC<SortableListProps> = ({
   open,
   items,
   updateData,
   mountedItems,
   type,
+  projects,
 }) => {
   const allProjectsLabel = 'All projects';
-  const projectsList = [
-    ...new Set(items.map((item: Mount | Repo): string => item.project)),
-  ];
+  const projectsList: string[] = projects.map(
+    (project: ProjectInfo): string => project.project.name,
+  );
   const [selectedProject, setSelectedProject] =
     useState<string>(allProjectsLabel);
 
   const onChange = (e: React.ChangeEvent<HTMLSelectElement>) => {
     setSelectedProject(e.target.value);
   };
```

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import React from 'react';
 import {render, fireEvent, waitFor} from '@testing-library/react';
 
 import SortableList from '../SortableList';
-import {Repo, Mount} from 'plugins/mount/types';
+import {Repo, Mount, ProjectInfo} from 'plugins/mount/types';
 import * as requestAPI from '../../../../../handler';
 import {mockedRequestAPI} from 'utils/testUtils';
 jest.mock('../../../../../handler');
 
 describe('sortable list components', () => {
   let open = jest.fn();
   let updateData = jest.fn();
@@ -31,14 +31,15 @@
     const {getByTestId} = render(
       <SortableList
         open={open}
         items={items}
         updateData={updateData}
         mountedItems={[]}
         type={'unmounted'}
+        projects={[]}
       />,
     );
     const listItem = getByTestId('ListItem__noBranches');
     expect(listItem).toHaveTextContent('images');
     expect(listItem).toHaveTextContent('No branches');
     expect(listItem).toHaveAttribute('title', "Repo doesn't have a branch");
   });
@@ -56,14 +57,15 @@
     const {getByTestId} = render(
       <SortableList
         open={open}
         items={items}
         updateData={updateData}
         mountedItems={[]}
         type={'unmounted'}
+        projects={[]}
       />,
     );
     const listItem = getByTestId('ListItem__unauthorized');
     expect(listItem).toHaveTextContent('images');
     expect(listItem).toHaveTextContent('No read access');
     expect(listItem).toHaveAttribute(
       'title',
@@ -90,14 +92,15 @@
     const {getByText, getAllByTestId} = render(
       <SortableList
         open={open}
         items={items}
         updateData={updateData}
         mountedItems={[]}
         type={'unmounted'}
+        projects={[]}
       />,
     );
     let listItems = getAllByTestId('ListItem__noBranches');
     expect(listItems).toHaveLength(2);
     expect(listItems[0]).toHaveTextContent('data');
     expect(listItems[1]).toHaveTextContent('images');
 
@@ -122,14 +125,15 @@
     const {getByTestId} = render(
       <SortableList
         open={open}
         items={items}
         updateData={updateData}
         mountedItems={[]}
         type={'unmounted'}
+        projects={[]}
       />,
     );
     const listItem = getByTestId('ListItem__repo');
     const mountButton = getByTestId('ListItem__mount');
 
     expect(listItem).toHaveTextContent('images');
     expect(mountButton).not.toBeDisabled();
@@ -174,14 +178,15 @@
     const {getByTestId} = render(
       <SortableList
         open={open}
         items={items}
         updateData={updateData}
         mountedItems={[]}
         type={'mounted'}
+        projects={[]}
       />,
     );
     const listItem = getByTestId('ListItem__repo');
     const unmountButton = getByTestId('ListItem__unmount');
 
     expect(listItem).toHaveTextContent('images');
     expect(unmountButton).not.toBeDisabled();
@@ -223,14 +228,15 @@
     const {getByText} = render(
       <SortableList
         open={open}
         items={items}
         updateData={updateData}
         mountedItems={[]}
         type={'mounted'}
+        projects={[]}
       />,
     );
     getByText('images').click();
     expect(open).toHaveBeenCalledWith('images');
   });
 
   it('should allow user to select a branch to mount', async () => {
@@ -246,14 +252,15 @@
     const {getByText, getByTestId} = render(
       <SortableList
         open={open}
         items={items}
         updateData={updateData}
         mountedItems={[]}
         type={'unmounted'}
+        projects={[]}
       />,
     );
     const select = getByTestId('ListItem__select') as HTMLSelectElement;
 
     expect(select.value).toBe('master');
     fireEvent.change(select, {target: {value: 'develop'}});
 
@@ -293,14 +300,15 @@
     const {getByTestId} = render(
       <SortableList
         open={open}
         items={items}
         updateData={updateData}
         mountedItems={[]}
         type={'mounted'}
+        projects={[]}
       />,
     );
 
     const statusIcon = getByTestId('ListItem__statusIcon');
     expect(statusIcon.title).toBe('Error: error mounting branch');
     const commitBehindnessText = getByTestId('ListItem__commitBehindness');
     expect(commitBehindnessText.textContent).toContain('up to date');
@@ -357,14 +365,15 @@
     const {getAllByTestId} = render(
       <SortableList
         open={open}
         items={items}
         updateData={updateData}
         mountedItems={[]}
         type={'mounted'}
+        projects={[]}
       />,
     );
     const unmountButtons = getAllByTestId('ListItem__unmount');
     expect(unmountButtons[0]).toBeDisabled();
     expect(unmountButtons[1]).toBeDisabled();
     expect(unmountButtons[2]).toBeDisabled();
   });
@@ -391,14 +400,15 @@
     const {getByTestId} = render(
       <SortableList
         open={open}
         items={items}
         updateData={updateData}
         mountedItems={[]}
         type={'mounted'}
+        projects={[]}
       />,
     );
 
     const commitBehindnessText = getByTestId('ListItem__commitBehindness');
     expect(commitBehindnessText.textContent).toContain('up to date');
   });
 
@@ -424,14 +434,15 @@
     const {getByTestId} = render(
       <SortableList
         open={open}
         items={items}
         updateData={updateData}
         mountedItems={[]}
         type={'mounted'}
+        projects={[]}
       />,
     );
 
     const commitBehindnessText = getByTestId('ListItem__commitBehindness');
     expect(commitBehindnessText.textContent).toContain('1 commit behind');
   });
 
@@ -457,14 +468,15 @@
     const {getByTestId} = render(
       <SortableList
         open={open}
         items={items}
         updateData={updateData}
         mountedItems={[]}
         type={'mounted'}
+        projects={[]}
       />,
     );
 
     const commitBehindnessText = getByTestId('ListItem__commitBehindness');
     expect(commitBehindnessText.textContent).toContain('2 commits behind');
   });
 
@@ -499,14 +511,15 @@
     const {getByTestId} = render(
       <SortableList
         open={open}
         items={items}
         updateData={updateData}
         mountedItems={mountedItems}
         type={'unmounted'}
+        projects={[]}
       />,
     );
 
     fireEvent.change(getByTestId('ListItem__select'), {
       target: {value: 'mounted_branch'},
     });
     expect(getByTestId('ListItem__mount')).toBeDisabled();
@@ -533,21 +546,43 @@
         repo: 'edges',
         project: 'default',
         authorization: 'off',
         branches: ['master'],
       },
     ];
 
+    const projects: ProjectInfo[] = [
+      {
+        project: {
+          name: 'p1',
+        },
+        auth: {
+          permissions: [0, 1, 2],
+          roles: ['foo', 'bar'],
+        },
+      },
+      {
+        project: {
+          name: 'default',
+        },
+        auth: {
+          permissions: [3, 4, 5],
+          roles: ['foo', 'bar', 'baz'],
+        },
+      },
+    ];
+
     const {getAllByTestId, getByTestId} = render(
       <SortableList
         open={open}
         items={items}
         updateData={updateData}
         mountedItems={[]}
         type={'unmounted'}
+        projects={projects}
       />,
     );
 
     let listItems = getAllByTestId('ListItem__repo');
     expect(listItems).toHaveLength(3);
 
     fireEvent.change(getByTestId('ProjectList__select'), {
```

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/mount/customFileBrowser.ts` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/customFileBrowser.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/mount/index.ts` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/mount/mount.css` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/mount.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/mount/mount.tsx` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/mount.tsx`

 * *Files 0% similar despite different names*

```diff
@@ -171,36 +171,42 @@
             </div>
             <SortableList
               open={this.open}
               items={mounted ? mounted : this._poller.mounted}
               updateData={this._poller.updateData}
               mountedItems={[]}
               type={'mounted'}
+              projects={[]}
             />
           </div>
         )}
       </UseSignal>,
     );
     this._mountedList.addClass('pachyderm-mount-react-wrapper');
 
     this._unmountedList = ReactWidget.create(
       <UseSignal signal={this._poller.unmountedSignal}>
         {(_, unmounted) => (
-          <div className="pachyderm-mount-base">
-            <div className="pachyderm-mount-base-title">
-              Unmounted Repositories
-            </div>
-            <SortableList
-              open={this.open}
-              items={unmounted ? unmounted : this._poller.unmounted}
-              updateData={this._poller.updateData}
-              mountedItems={this._poller.mounted}
-              type={'unmounted'}
-            />
-          </div>
+          <UseSignal signal={this._poller.projectSignal}>
+            {(_, projects) => (
+              <div className="pachyderm-mount-base">
+                <div className="pachyderm-mount-base-title">
+                  Unmounted Repositories
+                </div>
+                <SortableList
+                  open={this.open}
+                  items={unmounted ? unmounted : this._poller.unmounted}
+                  updateData={this._poller.updateData}
+                  mountedItems={this._poller.mounted}
+                  type={'unmounted'}
+                  projects={projects ? projects : this._poller.projects}
+                />
+              </div>
+            )}
+          </UseSignal>
         )}
       </UseSignal>,
     );
     this._unmountedList.addClass('pachyderm-mount-react-wrapper');
 
     this._datum = ReactWidget.create(
       <UseSignal signal={this._showDatumSignal}>
```

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/mount/mountDrive.ts` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/mountDrive.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/mount/pollMounts.ts` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/pollMounts.ts`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 import {ISignal, Signal} from '@lumino/signaling';
 import {Poll} from '@lumino/polling';
 import {requestAPI} from '../../handler';
-import {AuthConfig, Mount, ListMountsResponse, mountState, Repo} from './types';
+import {
+  AuthConfig,
+  Mount,
+  ListMountsResponse,
+  mountState,
+  Repo,
+  ProjectInfo,
+} from './types';
 import {ServerConnection} from '@jupyterlab/services';
 
 export const MOUNTED_STATES: mountState[] = [
   'unmounting',
   'mounted',
   'mounting',
   'error',
@@ -27,22 +34,24 @@
   }
   readonly name: string;
 
   private _rawData: ListMountsResponse = <ListMountsResponse>{};
 
   private _mounted: Mount[] = [];
   private _unmounted: Repo[] = [];
+  private _projects: ProjectInfo[] = [];
   private _status: ServerStatus = {code: 999, message: ''};
   private _config: AuthConfig = {
     pachd_address: '',
     cluster_status: 'INVALID',
   };
 
   private _mountedSignal = new Signal<this, Mount[]>(this);
   private _unmountedSignal = new Signal<this, Repo[]>(this);
+  private _projectSignal = new Signal<this, ProjectInfo[]>(this);
   private _statusSignal = new Signal<this, ServerStatus>(this);
   private _configSignal = new Signal<this, AuthConfig>(this);
 
   private _dataPoll = new Poll({
     auto: true,
     factory: async () => this.getData(),
     frequency: {
@@ -72,14 +81,26 @@
     if (data === this._unmounted) {
       return;
     }
     this._unmounted = data;
     this._unmountedSignal.emit(data);
   }
 
+  get projects(): ProjectInfo[] {
+    return this._projects;
+  }
+
+  set projects(data: ProjectInfo[]) {
+    if (data === this._projects) {
+      return;
+    }
+    this._projects = data;
+    this._projectSignal.emit(data);
+  }
+
   get status(): ServerStatus {
     return this._status;
   }
 
   set status(status: ServerStatus) {
     if (JSON.stringify(status) === JSON.stringify(this._status)) {
       return;
@@ -103,14 +124,17 @@
 
   get mountedSignal(): ISignal<this, Mount[]> {
     return this._mountedSignal;
   }
   get unmountedSignal(): ISignal<this, Repo[]> {
     return this._unmountedSignal;
   }
+  get projectSignal(): ISignal<this, ProjectInfo[]> {
+    return this._projectSignal;
+  }
 
   get statusSignal(): ISignal<this, ServerStatus> {
     return this._statusSignal;
   }
 
   get configSignal(): ISignal<this, AuthConfig> {
     return this._configSignal;
@@ -129,22 +153,30 @@
     if (JSON.stringify(data) !== JSON.stringify(this._rawData)) {
       this._rawData = data;
       this.mounted = Array.from(Object.values(data.mounted));
       this.unmounted = Array.from(Object.values(data.unmounted));
     }
   };
 
+  updateProjects = (data: ProjectInfo[]): void => {
+    if (JSON.stringify(data) !== JSON.stringify(this.projects)) {
+      this.projects = data;
+    }
+  };
+
   async getData(): Promise<void> {
     try {
       const config = await requestAPI<AuthConfig>('config', 'GET');
       this.config = config;
       if (config.cluster_status !== 'INVALID') {
         const data = await requestAPI<ListMountsResponse>('mounts', 'GET');
         this.status = {code: 200};
         this.updateData(data);
+        const project = await requestAPI<ProjectInfo[]>('projects', 'GET');
+        this.updateProjects(project);
       }
     } catch (error) {
       if (error instanceof ServerConnection.ResponseError) {
         this.status = {
           code: error.response.status,
           message: error.response.statusText,
         };
```

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/mount/types.ts` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/mount/types.ts`

 * *Files 7% similar despite different names*

```diff
@@ -74,31 +74,41 @@
 };
 
 export type ListMountsResponse = {
   mounted: {[key: string]: Mount};
   unmounted: {[key: string]: Repo};
 };
 
+export type Project = {
+  name: string;
+};
+
+export type ProjectAuthInfo = {
+  permissions: number[];
+  roles: string[];
+};
+
+export type ProjectInfo = {
+  project: Project;
+  auth: ProjectAuthInfo;
+};
+
 export type AuthConfig = {
   cluster_status: clusterStatus;
   pachd_address?: string;
   server_cas?: string;
 };
 
 export interface IMountPlugin {
   mountedRepos: Mount[];
   unmountedRepos: Repo[];
   layout: SplitPanel;
   ready: Promise<void>;
 }
 
-export type Project = {
-  name: string;
-};
-
 export type Pipeline = {
   name: string;
   project: Project | null;
 };
 
 export type PipelineSpec = {
   pipeline: Pipeline;
```

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/telemetry/__tests__/telemetry.test.tsx` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/telemetry/__tests__/telemetry.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/plugins/telemetry/telemetry.ts` & `jupyterlab_pachyderm-2.7.0a1/src/plugins/telemetry/telemetry.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/utils/components/Circle/Circle.tsx` & `jupyterlab_pachyderm-2.7.0a1/src/utils/components/Circle/Circle.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/utils/components/LoadingDots/loadingDots.css` & `jupyterlab_pachyderm-2.7.0a1/src/utils/components/LoadingDots/loadingDots.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/utils/components/Svgs/GenericError.js` & `jupyterlab_pachyderm-2.7.0a1/src/utils/components/Svgs/GenericError.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/utils/components/Svgs/KubernetesElephant.js` & `jupyterlab_pachyderm-2.7.0a1/src/utils/components/Svgs/KubernetesElephant.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/utils/components/Svgs/PachydermLogo.js` & `jupyterlab_pachyderm-2.7.0a1/src/utils/components/Svgs/PachydermLogo.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/utils/components/Svgs/StatusWarning.js` & `jupyterlab_pachyderm-2.7.0a1/src/utils/components/Svgs/StatusWarning.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/utils/hooks/useSort.ts` & `jupyterlab_pachyderm-2.7.0a1/src/utils/hooks/useSort.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/src/utils/icons.ts` & `jupyterlab_pachyderm-2.7.0a1/src/utils/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/style/base.css` & `jupyterlab_pachyderm-2.7.0a1/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/style/components/button.css` & `jupyterlab_pachyderm-2.7.0a1/style/components/button.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/style/icons/file.svg` & `jupyterlab_pachyderm-2.7.0a1/style/icons/file.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/style/icons/info.svg` & `jupyterlab_pachyderm-2.7.0a1/style/icons/info.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/style/icons/mount-logo.svg` & `jupyterlab_pachyderm-2.7.0a1/style/icons/mount-logo.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.1/style/icons/repo.svg` & `jupyterlab_pachyderm-2.7.0a1/style/icons/repo.svg`

 * *Files identical despite different names*

