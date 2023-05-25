# Comparing `tmp/jupyterlab_pachyderm-2.6.0rc2.tar.gz` & `tmp/jupyterlab_pachyderm-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_pachyderm-2.6.0rc2.tar", last modified: Fri May  5 14:43:53 2023, max compression
+gzip compressed data, was "jupyterlab_pachyderm-2.6.1.tar", last modified: Thu May 25 15:46:43 2023, max compression
```

## Comparing `jupyterlab_pachyderm-2.6.0rc2.tar` & `jupyterlab_pachyderm-2.6.1.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.383269 jupyterlab_pachyderm-2.6.0rc2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11108 2023-05-05 14:43:53.383269 jupyterlab_pachyderm-2.6.0rc2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10130 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/babel.config.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/install.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      366 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jest.config.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.359269 jupyterlab_pachyderm-2.6.0rc2/jupyter-config/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.363269 jupyterlab_pachyderm-2.6.0rc2/jupyter-config/nb-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyter-config/nb-config/jupyterlab_pachyderm.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.363269 jupyterlab_pachyderm-2.6.0rc2/jupyter-config/server-config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       95 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyter-config/server-config/jupyterlab_pachyderm.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.367269 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/dev_server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      554 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/env.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/filemanager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12522 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/handlers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.367269 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4409 2023-05-05 14:43:51.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.359269 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/schemas/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.367269 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-05-05 14:43:40.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/examples.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-05-05 14:43:40.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/help.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-05-05 14:43:40.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/mount.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4267 2023-05-05 14:43:40.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-05-05 14:43:40.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/telemetry.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.371269 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2023-05-05 14:43:51.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2023-05-05 14:43:51.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    70514 2023-05-05 14:43:51.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2023-05-05 14:43:51.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)   401782 2023-05-05 14:43:51.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   102166 2023-05-05 14:43:51.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16896 2023-05-05 14:43:51.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)   160105 2023-05-05 14:43:51.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/829.58d0c33e721471840271.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8301 2023-05-05 14:43:51.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/remoteEntry.020bdee857c5f964fd3e.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-05-05 14:43:40.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/style.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8183 2023-05-05 14:43:51.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/third-party-licenses.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/log.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9051 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/mount_server_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      640 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/pachyderm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9524 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/pps_client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.371269 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.371269 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/tests/data/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19088 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/tests/test_handlers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16841 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/tests/test_integrations.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.367269 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11108 2023-05-05 14:43:53.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4690 2023-05-05 14:43:53.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-05 14:43:53.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-05 14:43:24.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-05-05 14:43:53.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-05-05 14:43:53.000000 jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4267 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/pyproject.toml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.371269 jupyterlab_pachyderm-2.6.0rc2/schema/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/schema/examples.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/schema/help.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/schema/mount.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/schema/telemetry.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      980 2023-05-05 14:43:53.383269 jupyterlab_pachyderm-2.6.0rc2/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2260 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.371269 jupyterlab_pachyderm-2.6.0rc2/src/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/global.d.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/handler.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.363269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/examples/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/examples/__test__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/examples/__test__/examples.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1789 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/examples/examples.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      413 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/examples/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/help/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/help/__tests__/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/help/__tests__/__snapshots__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1937 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/help/__tests__/help.test.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/help/help.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/help/help.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/help/index.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5675 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/__tests__/mount.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.363269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8530 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Config/Config.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Config/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12024 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Config/__tests__/Config.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Config/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Config/hooks/useConfig.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Datum/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4675 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Datum/Datum.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Datum/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7511 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Datum/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6182 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Datum/hooks/useDatum.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/FullPageError/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1012 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/FullPageError/FullPageError.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/FullPageError/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Pipeline/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5779 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Pipeline/Pipeline.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      999 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Pipeline/Splash.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.375269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Pipeline/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3800 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Pipeline/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4746 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/SortableList/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3730 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/SortableList/ListMount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5159 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/SortableList/ListUnmount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3415 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/SortableList/SortableList.tsx
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/SortableList/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14680 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2984 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/customFileBrowser.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1488 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8702 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/mount.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21546 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/mount.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2993 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/mountDrive.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3658 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/pollMounts.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2606 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/types.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/telemetry/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/src/plugins/telemetry/__tests__/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1988 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/telemetry/__tests__/telemetry.test.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/telemetry/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      814 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/plugins/telemetry/telemetry.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/setupTests.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/src/utils/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.363269 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Circle/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      757 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Circle/Circle.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Circle/circle.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/LoadingDots/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/LoadingDots/LoadingDots.tsx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      853 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/LoadingDots/loadingDots.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Svgs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26381 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Svgs/GenericError.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    74288 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Svgs/KubernetesElephant.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16523 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Svgs/PachydermLogo.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Svgs/StatusWarning.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Svgs/index.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/src/utils/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/hooks/usePreviousValue.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/hooks/useSort.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      675 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/icons.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/src/utils/testUtils.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/style/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/style/base.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.379269 jupyterlab_pachyderm-2.6.0rc2/style/components/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1524 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/style/components/button.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/style/components/input.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 14:43:53.383269 jupyterlab_pachyderm-2.6.0rc2/style/icons/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/style/icons/file.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/style/icons/info.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/style/icons/mount-logo.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/style/icons/repo.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/style/index.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/style/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-05-05 14:41:25.000000 jupyterlab_pachyderm-2.6.0rc2/tsconfig.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.143847 jupyterlab_pachyderm-2.6.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      744 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11105 2023-05-25 15:46:43.143847 jupyterlab_pachyderm-2.6.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10130 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/babel.config.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/install.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      366 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jest.config.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.119847 jupyterlab_pachyderm-2.6.1/jupyter-config/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.123847 jupyterlab_pachyderm-2.6.1/jupyter-config/nb-config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyter-config/nb-config/jupyterlab_pachyderm.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.123847 jupyterlab_pachyderm-2.6.1/jupyter-config/server-config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       95 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyter-config/server-config/jupyterlab_pachyderm.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.127847 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/dev_server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      554 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/env.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/filemanager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12522 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/handlers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.127847 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4404 2023-05-25 15:46:40.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.119847 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/schemas/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.131847 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-05-25 15:46:29.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/examples.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-05-25 15:46:29.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/help.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-05-25 15:46:29.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/mount.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4262 2023-05-25 15:46:29.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-05-25 15:46:29.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/telemetry.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.131847 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2023-05-25 15:46:40.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2023-05-25 15:46:40.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    70514 2023-05-25 15:46:40.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2023-05-25 15:46:40.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   401782 2023-05-25 15:46:40.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   102166 2023-05-25 15:46:40.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16896 2023-05-25 15:46:40.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   160194 2023-05-25 15:46:40.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/829.0234ec6e026820778750.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8296 2023-05-25 15:46:40.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/remoteEntry.d9811dd3652ac1fc0383.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      163 2023-05-25 15:46:29.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/style.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8183 2023-05-25 15:46:40.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/third-party-licenses.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      431 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/log.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9051 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/mount_server_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      640 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/pachyderm.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9524 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/pps_client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.131847 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      164 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.135847 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/tests/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/tests/data/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19088 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/tests/test_handlers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16841 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/tests/test_integrations.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.127847 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11105 2023-05-25 15:46:43.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4690 2023-05-25 15:46:43.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-25 15:46:43.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-25 15:46:14.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-05-25 15:46:43.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-05-25 15:46:43.000000 jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4262 2023-05-25 15:43:56.000000 jupyterlab_pachyderm-2.6.1/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/pyproject.toml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.135847 jupyterlab_pachyderm-2.6.1/schema/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/schema/examples.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/schema/help.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/schema/mount.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/schema/telemetry.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      980 2023-05-25 15:46:43.147847 jupyterlab_pachyderm-2.6.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2260 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.135847 jupyterlab_pachyderm-2.6.1/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/global.d.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/handler.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.123847 jupyterlab_pachyderm-2.6.1/src/plugins/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.135847 jupyterlab_pachyderm-2.6.1/src/plugins/examples/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.135847 jupyterlab_pachyderm-2.6.1/src/plugins/examples/__test__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/examples/__test__/examples.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1789 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/examples/examples.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      413 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/examples/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.135847 jupyterlab_pachyderm-2.6.1/src/plugins/help/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.135847 jupyterlab_pachyderm-2.6.1/src/plugins/help/__tests__/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.135847 jupyterlab_pachyderm-2.6.1/src/plugins/help/__tests__/__snapshots__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1937 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/help/__tests__/help.test.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/help/help.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/help/help.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/help/index.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.135847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.135847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6919 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/__tests__/mount.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.123847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8530 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Config/Config.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Config/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12024 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Config/__tests__/Config.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Config/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Config/hooks/useConfig.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Datum/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4675 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Datum/Datum.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Datum/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7511 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Datum/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6182 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Datum/hooks/useDatum.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/FullPageError/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1012 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/FullPageError/FullPageError.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/FullPageError/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Pipeline/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5779 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Pipeline/Pipeline.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      999 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Pipeline/Splash.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Pipeline/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3800 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Pipeline/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4746 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/SortableList/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3730 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/SortableList/ListMount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5159 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/SortableList/ListUnmount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3415 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/SortableList/SortableList.tsx
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/SortableList/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14680 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2984 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/customFileBrowser.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1488 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8702 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/mount.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21752 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/mount.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2993 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/mountDrive.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3658 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/pollMounts.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2606 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/mount/types.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/telemetry/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/plugins/telemetry/__tests__/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1988 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/telemetry/__tests__/telemetry.test.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/telemetry/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      814 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/plugins/telemetry/telemetry.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/setupTests.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/utils/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.123847 jupyterlab_pachyderm-2.6.1/src/utils/components/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.139847 jupyterlab_pachyderm-2.6.1/src/utils/components/Circle/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      757 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/components/Circle/Circle.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/components/Circle/circle.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.143847 jupyterlab_pachyderm-2.6.1/src/utils/components/LoadingDots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/components/LoadingDots/LoadingDots.tsx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      853 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/components/LoadingDots/loadingDots.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.143847 jupyterlab_pachyderm-2.6.1/src/utils/components/Svgs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26381 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/components/Svgs/GenericError.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    74288 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/components/Svgs/KubernetesElephant.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16523 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/components/Svgs/PachydermLogo.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/components/Svgs/StatusWarning.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/components/Svgs/index.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.143847 jupyterlab_pachyderm-2.6.1/src/utils/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/hooks/usePreviousValue.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/hooks/useSort.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      675 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/icons.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      377 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/src/utils/testUtils.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.143847 jupyterlab_pachyderm-2.6.1/style/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/style/base.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.143847 jupyterlab_pachyderm-2.6.1/style/components/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1524 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/style/components/button.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/style/components/input.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:46:43.143847 jupyterlab_pachyderm-2.6.1/style/icons/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/style/icons/file.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/style/icons/info.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/style/icons/mount-logo.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/style/icons/repo.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/style/index.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/style/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-05-25 15:43:55.000000 jupyterlab_pachyderm-2.6.1/tsconfig.json
```

### Comparing `jupyterlab_pachyderm-2.6.0rc2/LICENSE` & `jupyterlab_pachyderm-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/MANIFEST.in` & `jupyterlab_pachyderm-2.6.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/PKG-INFO` & `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jupyterlab_pachyderm
-Version: 2.6.0rc2
+Name: jupyterlab-pachyderm
+Version: 2.6.1
 Summary: A JupyterLab extension.
 Home-page: https://github.com/pachyderm/jupyterlab-pachyderm
 Author: 
 Author-email: 
 License: BSD-3-Clause
 Keywords: jupyter,jupyterlab,jupyterlab-extension
 Platform: Linux
```

### Comparing `jupyterlab_pachyderm-2.6.0rc2/README.md` & `jupyterlab_pachyderm-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/__init__.py` & `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/_version.py` & `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/_version.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/env.py` & `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/env.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/handlers.py` & `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/package.json` & `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222223%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'2.6.1'"}*

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
-            "load": "static/remoteEntry.020bdee857c5f964fd3e.js",
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
-    "version": "2.6.0-rc.2"
+    "version": "2.6.1"
 }
```

### Comparing `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/schemas/jupyterlab-pachyderm/package.json.orig` & `jupyterlab_pachyderm-2.6.1/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'2.6.1'"}*

```diff
@@ -128,9 +128,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.6.0-rc.2"
+    "version": "2.6.1"
 }
```

### Comparing `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js` & `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js` & `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js` & `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js` & `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js` & `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/829.58d0c33e721471840271.js` & `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/829.0234ec6e026820778750.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -391,16 +391,16 @@
                     })))(e, t)
                 };
             var C = a(5687),
                 M = a(7986),
                 z = a(7280),
                 S = a(4038),
                 L = a(1123),
-                N = a(1840),
-                B = a(8832),
+                B = a(1840),
+                N = a(8832),
                 O = a(3114);
 
             function D(e = "", t = "GET", a = null, n = "pachyderm/v2") {
                 return r = this, l = void 0, i = function*() {
                     const r = _.ServerConnection.makeSettings(),
                         l = E.URLExt.join(r.baseUrl, n, e),
                         s = {
@@ -485,15 +485,15 @@
                 constructor(e) {
                     this._rawData = {}, this._mounted = [], this._unmounted = [], this._status = {
                         code: 999,
                         message: ""
                     }, this._config = {
                         pachd_address: "",
                         cluster_status: "INVALID"
-                    }, this._mountedSignal = new N.Signal(this), this._unmountedSignal = new N.Signal(this), this._statusSignal = new N.Signal(this), this._configSignal = new N.Signal(this), this._dataPoll = new O.n_({
+                    }, this._mountedSignal = new B.Signal(this), this._unmountedSignal = new B.Signal(this), this._statusSignal = new B.Signal(this), this._configSignal = new B.Signal(this), this._dataPoll = new O.n_({
                         auto: !0,
                         factory: () => A(this, void 0, void 0, (function*() {
                             return this.getData()
                         })),
                         frequency: {
                             interval: 2e3,
                             backoff: !0,
@@ -563,15 +563,15 @@
                     }))
                 }
             }
             var j = a(6057),
                 H = a(8918);
             class P {
                 constructor(e) {
-                    this._fileChanged = new N.Signal(this), this._serverSettings = _.ServerConnection.makeSettings(), this._isDisposed = !1, this._registry = e
+                    this._fileChanged = new B.Signal(this), this._serverSettings = _.ServerConnection.makeSettings(), this._isDisposed = !1, this._registry = e
                 }
                 get name() {
                     return "mount-browser"
                 }
                 get fileChanged() {
                     return this._fileChanged
                 }
@@ -656,15 +656,15 @@
                 restoreCheckpoint(e, t) {
                     return Promise.resolve()
                 }
                 deleteCheckpoint(e, t) {
                     return Promise.resolve()
                 }
                 dispose() {
-                    this.isDisposed || (this._isDisposed = !0, N.Signal.clearData(this))
+                    this.isDisposed || (this._isDisposed = !0, B.Signal.clearData(this))
                 }
             }
             var I = function(e, t, a, n) {
                 return new(a || (a = Promise))((function(r, l) {
                     function s(e) {
                         try {
                             c(n.next(e))
@@ -2578,16 +2578,16 @@
                     }, m().createElement(R, {
                         width: "230px",
                         height: "230px"
                     }))))
                 };
             var G = a(930),
                 T = a.n(G),
-                $ = a(4439),
-                V = function(e, t, a, n) {
+                V = a(4439),
+                $ = function(e, t, a, n) {
                     return new(a || (a = Promise))((function(r, l) {
                         function s(e) {
                             try {
                                 c(n.next(e))
                             } catch (e) {
                                 l(e)
                             }
@@ -2669,25 +2669,25 @@
                                 if (0 === Object.keys(e).length) return "";
                                 try {
                                     return JSON.parse(E), JSON.stringify(e, null, 2)
                                 } catch (t) {
                                     return T().stringify(e, null, 2)
                                 }
                             },
-                            z = () => V(void 0, void 0, void 0, (function*() {
+                            z = () => $(void 0, void 0, void 0, (function*() {
                                 c(!0);
                                 try {
                                     const e = yield D(`_show_datum?idx=${u}`, "PUT");
                                     n(""), f(e)
                                 } catch (e) {
                                     console.log(e)
                                 }
                                 c(!1)
                             })),
-                            S = () => V(void 0, void 0, void 0, (function*() {
+                            S = () => $(void 0, void 0, void 0, (function*() {
                                 c(!0);
                                 try {
                                     n(""), yield D("_unmount_all", "PUT"), n(""), yield r(), h(-1), f({
                                         id: "",
                                         idx: -1,
                                         num_datums: 0
                                     }), d(!1)
@@ -2700,15 +2700,15 @@
                             loading: i,
                             shouldShowCycler: m,
                             currDatum: p,
                             currIdx: u,
                             setCurrIdx: h,
                             inputSpec: E,
                             setInputSpec: g,
-                            callMountDatums: () => V(void 0, void 0, void 0, (function*() {
+                            callMountDatums: () => $(void 0, void 0, void 0, (function*() {
                                 c(!0), b("");
                                 try {
                                     const e = C(),
                                         t = yield D("_mount_datums", "PUT", {
                                             input: e
                                         });
                                     n(""), h(0), f(t), d(!0), g(M(e))
@@ -2718,15 +2718,15 @@
                                 c(!1)
                             })),
                             callUnmountAll: S,
                             errorMessage: y,
                             saveInputSpec: () => {
                                 try {
                                     const e = C();
-                                    (0, $.isEqual)(l, e) ? x({}): x(e || {})
+                                    (0, V.isEqual)(l, e) ? x({}): x(e || {})
                                 } catch (e) {
                                     if (!(e instanceof T().YAMLParseError)) throw e;
                                     x(E)
                                 }
                             },
                             initialInputSpec: v
                         }
@@ -3258,15 +3258,15 @@
                             case "unmounting":
                             case "mounting":
                                 a = "yellow";
                                 break;
                             case "error":
                                 a = "red"
                         }
-                        return n = t ? `${(0,$.capitalize)(e||"Unknown")}: ${t}` : (0, $.capitalize)(e || "Unknown"), m().createElement(m().Fragment, null, m().createElement(te, {
+                        return n = t ? `${(0,V.capitalize)(e||"Unknown")}: ${t}` : (0, V.capitalize)(e || "Unknown"), m().createElement(m().Fragment, null, m().createElement(te, {
                             color: a,
                             className: "pachyderm-mount-list-item-status-circle"
                         }), m().createElement("div", {
                             "data-testid": "ListItem__statusIcon",
                             className: "pachyderm-mount-list-item-status-icon",
                             title: n
                         }, m().createElement(y.react, {
@@ -4069,15 +4069,15 @@
                     c((n = n.apply(e, t || [])).next())
                 }))
             };
             const de = "mount-browser:",
                 ue = "pachyderm_pps";
             class he {
                 constructor(e, t, a, n, r, l) {
-                    this._showConfig = !1, this._showConfigSignal = new N.Signal(this), this._readyPromise = Promise.resolve(), this._showDatum = !1, this._showPipeline = !1, this._keepMounted = !1, this._showDatumSignal = new N.Signal(this), this._repoViewInputSpec = {}, this._saveInputSpecSignal = new N.Signal(this), this._showPipelineSignal = new N.Signal(this), this._ppsContextSignal = new N.Signal(this), this.isCurrentWidgetNotebook = e => (e = null != e ? e : this._widgetTracker.currentWidget) instanceof L.NotebookPanel, this.getActiveNotebook = () => {
+                    this._showConfig = !1, this._showConfigSignal = new B.Signal(this), this._readyPromise = Promise.resolve(), this._showDatum = !1, this._showPipeline = !1, this._keepMounted = !1, this._showDatumSignal = new B.Signal(this), this._repoViewInputSpec = {}, this._saveInputSpecSignal = new B.Signal(this), this._showPipelineSignal = new B.Signal(this), this._ppsContextSignal = new B.Signal(this), this.isCurrentWidgetNotebook = e => (e = null != e ? e : this._widgetTracker.currentWidget) instanceof L.NotebookPanel, this.getActiveNotebook = () => {
                         const e = this._widgetTracker.currentWidget;
                         return this.isCurrentWidgetNotebook(e) ? e : null
                     }, this.handleWidgetChanged = (e, t) => me(this, void 0, void 0, (function*() {
                         this.isCurrentWidgetNotebook(t.newValue) && (yield this.handleNotebookChanged(t.newValue)), this.setShowPipeline(this._showPipeline), yield Promise.resolve()
                     })), this.handleNotebookChanged = e => me(this, void 0, void 0, (function*() {
                         yield e.sessionContext.ready, e.context.fileChanged.connect(this.handleNotebookReload);
                         const t = {
@@ -4104,19 +4104,21 @@
                     })), this.open = e => {
                         this._app.commands.execute("filebrowser:open-path", {
                             path: de + e
                         })
                     }, this.refresh = (e, t) => me(this, void 0, void 0, (function*() {
                         yield this._mountBrowser.model.refresh()
                     })), this.verifyBrowserPath = (e, t) => {
-                        if (this._mountBrowser.model.path === this._mountBrowser.model.rootPath) return;
-                        const a = this._mountBrowser.model.path.split(de)[1].split("/")[0];
+                        this._mountBrowser.model.path !== this._mountBrowser.model.rootPath && (this.isValidBrowserPath(this._mountBrowser.model.path, t) || this.open(""))
+                    }, this.isValidBrowserPath = (e, t) => {
+                        const a = e.split(de)[1].split("/")[0];
+                        if ("out" === a) return !0;
                         for (let e = 0; e < t.length; e++)
-                            if (a === t[e].name) return;
-                        this.open("")
+                            if (a === t[e].name) return !0;
+                        return !1
                     }, this.setShowDatum = e => me(this, void 0, void 0, (function*() {
                         e ? (this._datum.setHidden(!1), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this.saveMountedReposList()) : (this._datum.setHidden(!0), this._mountedList.setHidden(!1), this._unmountedList.setHidden(!1), yield this.restoreMountedReposList()), this._mountBrowser.setHidden(!1), this._config.setHidden(!0), this._pipeline.setHidden(!0), this._fullPageError.setHidden(!0), this._showDatum = e, this._showDatumSignal.emit(e)
                     })), this.saveMountedReposList = () => {
                         const e = this._poller.mounted,
                             t = [];
                         for (let a = 0; a < e.length; a++) {
                             const n = {
@@ -4312,15 +4314,15 @@
                                     mnemonic: 0,
                                     execute: () => {
                                         (0, H.each)(l.selectedItems(), (e => {
                                             d.Clipboard.copyToSystem(e.path.replace(de, "/pfs/"))
                                         }))
                                     }
                                 });
-                                const a = new B.Menu({
+                                const a = new N.Menu({
                                     commands: e
                                 });
                                 a.addItem({
                                     command: "file-open"
                                 }), a.addItem({
                                     command: "copy-path"
                                 }), i.node.getElementsByClassName("jp-DirListing-content")[0].addEventListener("contextmenu", (e => {
@@ -4330,15 +4332,15 @@
                                     a.open(t, n)
                                 }))
                             }
                         } catch (e) {
                             console.log("Failed to edit default browser.")
                         }
                         return l
-                    })(e, a, n), this._poller.mountedSignal.connect(this.verifyBrowserPath), this._poller.mountedSignal.connect(this.refresh), this._poller.unmountedSignal.connect(this.refresh), this._widgetTracker.currentChanged.connect(this.handleWidgetChanged, this), this._panel = new B.SplitPanel, this._panel.orientation = "vertical", this._panel.spacing = 0, this._panel.title.icon = k, this._panel.title.caption = "Pachyderm Mount", this._panel.id = "pachyderm-mount", this._panel.addWidget(this._mountedList), this._panel.addWidget(this._unmountedList), this._panel.addWidget(this._datum), this._panel.addWidget(this._pipelineSplash), this._panel.addWidget(this._pipeline), this._panel.addWidget(this._mountBrowser), this._panel.setRelativeSizes([1, 1, 3, 3]), this._panel.addWidget(this._loader), this._panel.addWidget(this._config), this._panel.addWidget(this._fullPageError), this._config.setHidden(!0), this._fullPageError.setHidden(!0), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this._datum.setHidden(!0), this._pipelineSplash.setHidden(!0), this._pipeline.setHidden(!0), this._mountBrowser.setHidden(!0), window.addEventListener("resize", (() => {
+                    })(e, a, n), this._poller.mountedSignal.connect(this.verifyBrowserPath), this._poller.mountedSignal.connect(this.refresh), this._poller.unmountedSignal.connect(this.refresh), this._widgetTracker.currentChanged.connect(this.handleWidgetChanged, this), this._panel = new N.SplitPanel, this._panel.orientation = "vertical", this._panel.spacing = 0, this._panel.title.icon = k, this._panel.title.caption = "Pachyderm Mount", this._panel.id = "pachyderm-mount", this._panel.addWidget(this._mountedList), this._panel.addWidget(this._unmountedList), this._panel.addWidget(this._datum), this._panel.addWidget(this._pipelineSplash), this._panel.addWidget(this._pipeline), this._panel.addWidget(this._mountBrowser), this._panel.setRelativeSizes([1, 1, 3, 3]), this._panel.addWidget(this._loader), this._panel.addWidget(this._config), this._panel.addWidget(this._fullPageError), this._config.setHidden(!0), this._fullPageError.setHidden(!0), this._mountedList.setHidden(!0), this._unmountedList.setHidden(!0), this._datum.setHidden(!0), this._pipelineSplash.setHidden(!0), this._pipeline.setHidden(!0), this._mountBrowser.setHidden(!0), window.addEventListener("resize", (() => {
                         this._panel.update()
                     })), r.add(this._panel, "jupyterlab-pachyderm"), e.shell.add(this._panel, "left", {
                         rank: 100
                     })
                 }
                 get mountedRepos() {
                     return this._poller.poll.tick, this._poller.mounted
```

### Comparing `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/remoteEntry.020bdee857c5f964fd3e.js` & `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/remoteEntry.d9811dd3652ac1fc0383.js`

 * *Files 4% similar despite different names*

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
-        829: "58d0c33e721471840271"
+        829: "0234ec6e026820778750"
     } [e] + ".js?v=" + {
         67: "9d3e2934cfe0e102619e",
         371: "8ac933b7fbb0f688b6f4",
         486: "003d1d2cc9cc6927471e",
         676: "95f9b834e9f9b133c00b",
         747: "b62f963856036a13fba1",
-        829: "58d0c33e721471840271"
+        829: "0234ec6e026820778750"
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
-                return "default" === t && (u("jupyterlab-pachyderm", "2.6.0-rc.2", (() => Promise.all([j.e(371), j.e(829)]).then((() => () => j(7363))))), u("lodash", "4.17.21", (() => j.e(486).then((() => () => j(6486))))), u("rudder-sdk-js", "1.2.5", (() => j.e(67).then((() => () => j(3067))))), u("yaml", "0", (() => j.e(676).then((() => () => j(5676)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("jupyterlab-pachyderm", "2.6.1", (() => Promise.all([j.e(371), j.e(829)]).then((() => () => j(7363))))), u("lodash", "4.17.21", (() => j.e(486).then((() => () => j(6486))))), u("rudder-sdk-js", "1.2.5", (() => j.e(67).then((() => () => j(3067))))), u("yaml", "0", (() => j.e(676).then((() => () => j(5676)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/labextension/static/third-party-licenses.json` & `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/mount_server_client.py` & `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/mount_server_client.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/pachyderm.py` & `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/pachyderm.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/pps_client.py` & `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/pps_client.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb` & `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/tests/data/TestNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/tests/test_handlers.py` & `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm/tests/test_integrations.py` & `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/tests/test_integrations.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm.egg-info/PKG-INFO` & `jupyterlab_pachyderm-2.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jupyterlab-pachyderm
-Version: 2.6.0rc2
+Name: jupyterlab_pachyderm
+Version: 2.6.1
 Summary: A JupyterLab extension.
 Home-page: https://github.com/pachyderm/jupyterlab-pachyderm
 Author: 
 Author-email: 
 License: BSD-3-Clause
 Keywords: jupyter,jupyterlab,jupyterlab-extension
 Platform: Linux
```

### Comparing `jupyterlab_pachyderm-2.6.0rc2/jupyterlab_pachyderm.egg-info/SOURCES.txt` & `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js
 jupyterlab_pachyderm/labextension/static/371.8ac933b7fbb0f688b6f4.js.LICENSE.txt
 jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js
 jupyterlab_pachyderm/labextension/static/486.003d1d2cc9cc6927471e.js.LICENSE.txt
 jupyterlab_pachyderm/labextension/static/67.9d3e2934cfe0e102619e.js
 jupyterlab_pachyderm/labextension/static/676.95f9b834e9f9b133c00b.js
 jupyterlab_pachyderm/labextension/static/747.b62f963856036a13fba1.js
-jupyterlab_pachyderm/labextension/static/829.58d0c33e721471840271.js
-jupyterlab_pachyderm/labextension/static/remoteEntry.020bdee857c5f964fd3e.js
+jupyterlab_pachyderm/labextension/static/829.0234ec6e026820778750.js
+jupyterlab_pachyderm/labextension/static/remoteEntry.d9811dd3652ac1fc0383.js
 jupyterlab_pachyderm/labextension/static/style.js
 jupyterlab_pachyderm/labextension/static/third-party-licenses.json
 jupyterlab_pachyderm/tests/__init__.py
 jupyterlab_pachyderm/tests/test_handlers.py
 jupyterlab_pachyderm/tests/test_integrations.py
 jupyterlab_pachyderm/tests/data/TestNotebook.ipynb
 jupyterlab_pachyderm/tests/data/requirements.txt
```

### Comparing `jupyterlab_pachyderm-2.6.0rc2/package.json` & `jupyterlab_pachyderm-2.6.1/jupyterlab_pachyderm/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222223%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.d9811dd3652ac1fc0383.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'2.6.1'"}*

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
+            "load": "static/remoteEntry.d9811dd3652ac1fc0383.js",
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
-    "version": "2.6.0-rc.2"
+    "version": "2.6.1"
 }
```

### Comparing `jupyterlab_pachyderm-2.6.0rc2/pyproject.toml` & `jupyterlab_pachyderm-2.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/setup.cfg` & `jupyterlab_pachyderm-2.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/setup.py` & `jupyterlab_pachyderm-2.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/handler.ts` & `jupyterlab_pachyderm-2.6.1/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/examples/__test__/examples.test.tsx` & `jupyterlab_pachyderm-2.6.1/src/plugins/examples/__test__/examples.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/examples/examples.tsx` & `jupyterlab_pachyderm-2.6.1/src/plugins/examples/examples.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap` & `jupyterlab_pachyderm-2.6.1/src/plugins/help/__tests__/__snapshots__/help.test.ts.snap`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/help/__tests__/help.test.ts` & `jupyterlab_pachyderm-2.6.1/src/plugins/help/__tests__/help.test.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/help/help.tsx` & `jupyterlab_pachyderm-2.6.1/src/plugins/help/help.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/__tests__/mount.test.tsx` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/__tests__/mount.test.tsx`

 * *Files 19% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import {StateDB} from '@jupyterlab/statedb';
 import {CommandRegistry} from '@lumino/commands';
 import {Widget} from '@lumino/widgets';
 import {mockedRequestAPI} from 'utils/testUtils';
 import {MountPlugin} from '../mount';
 import * as requestAPI from '../../../handler';
 import {waitFor} from '@testing-library/react';
-import {MountSettings} from '../types';
+import {Mount, MountSettings} from '../types';
 
 jest.mock('../../../handler');
 
 const items = {
   unmounted: [
     {
       repo: 'images',
@@ -78,14 +78,58 @@
     restorer = new LayoutRestorer({
       connector: new StateDB(),
       first: Promise.resolve<void>(void 0),
       registry: new CommandRegistry(),
     });
   });
 
+  it('should accept /pfs/out as a valid FileBrowser path', async () => {
+    const plugin = new MountPlugin(
+      app,
+      settings,
+      docManager,
+      factory,
+      restorer,
+      widgetTracker,
+    );
+    const mounts: Mount[] = [
+      {
+        name: 'default_images',
+        project: 'default',
+        branch: 'master',
+        commit: null,
+        repo: 'images',
+        glob: '/*',
+        mode: 'ro',
+        state: 'mounted',
+        status: '',
+        mountpoint: '/pfs',
+        how_many_commits_behind: 0,
+        actual_mounted_commit: '1a2b3c',
+        latest_commit: '1a2b3c',
+      },
+    ];
+    expect(
+      plugin.isValidBrowserPath('mount-browser:default_images', mounts),
+    ).toBe(true);
+    expect(
+      plugin.isValidBrowserPath('mount-browser:default_images/testdir', mounts),
+    ).toBe(true);
+    expect(
+      plugin.isValidBrowserPath('mount-browser:default_edges', mounts),
+    ).toBe(false);
+    expect(
+      plugin.isValidBrowserPath('mount-browser:default_edges/testdir', mounts),
+    ).toBe(false);
+    expect(plugin.isValidBrowserPath('mount-browser:out', mounts)).toBe(true);
+    expect(plugin.isValidBrowserPath('mount-browser:out/testdir', mounts)).toBe(
+      true,
+    );
+  });
+
   it.skip('should poll for mounts', async () => {
     mockRequestAPI.requestAPI
       .mockImplementationOnce(mockedRequestAPI(items)) // call to api from setup function, part of auth flow.
       .mockImplementationOnce(mockedRequestAPI(items))
       .mockImplementationOnce(
         mockedRequestAPI({
           mounted: [
```

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Config/Config.tsx` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Config/Config.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Config/__tests__/Config.test.tsx` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Config/__tests__/Config.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Config/hooks/useConfig.tsx` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Config/hooks/useConfig.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Datum/Datum.tsx` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Datum/Datum.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Datum/__tests__/Datum.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Datum/hooks/useDatum.tsx` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Datum/hooks/useDatum.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/FullPageError/FullPageError.tsx` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/FullPageError/FullPageError.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/FullPageError/__tests__/FullPageError.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Pipeline/Pipeline.tsx` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Pipeline/Pipeline.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Pipeline/Splash.tsx` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Pipeline/Splash.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Pipeline/__tests__/Pipeline.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/Pipeline/hooks/usePipeline.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/SortableList/ListMount.tsx` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/SortableList/ListMount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/SortableList/ListUnmount.tsx` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/SortableList/ListUnmount.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/SortableList/SortableList.tsx` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/SortableList/SortableList.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/components/SortableList/__tests__/SortableList.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/customFileBrowser.ts` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/customFileBrowser.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/index.ts` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/mount.css` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/mount.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/mount.tsx` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/mount.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -415,23 +415,30 @@
 
   // Change back to root directory if in a mount that no longer exists
   verifyBrowserPath = (_: PollMounts, mounted: Mount[]): void => {
     if (this._mountBrowser.model.path === this._mountBrowser.model.rootPath) {
       return;
     }
 
-    const currentMountDir = this._mountBrowser.model.path
-      .split(MOUNT_BROWSER_NAME)[1]
-      .split('/')[0];
+    if (!this.isValidBrowserPath(this._mountBrowser.model.path, mounted)) {
+      this.open('');
+    }
+  };
+
+  isValidBrowserPath = (path: string, mounted: Mount[]): boolean => {
+    const currentMountDir = path.split(MOUNT_BROWSER_NAME)[1].split('/')[0];
+    if (currentMountDir === 'out') {
+      return true;
+    }
     for (let i = 0; i < mounted.length; i++) {
       if (currentMountDir === mounted[i].name) {
-        return;
+        return true;
       }
     }
-    this.open('');
+    return false;
   };
 
   setShowDatum = async (shouldShow: boolean): Promise<void> => {
     if (shouldShow) {
       this._datum.setHidden(false);
       this._mountedList.setHidden(true);
       this._unmountedList.setHidden(true);
```

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/mountDrive.ts` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/mountDrive.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/pollMounts.ts` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/pollMounts.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/mount/types.ts` & `jupyterlab_pachyderm-2.6.1/src/plugins/mount/types.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/telemetry/__tests__/telemetry.test.tsx` & `jupyterlab_pachyderm-2.6.1/src/plugins/telemetry/__tests__/telemetry.test.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/plugins/telemetry/telemetry.ts` & `jupyterlab_pachyderm-2.6.1/src/plugins/telemetry/telemetry.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Circle/Circle.tsx` & `jupyterlab_pachyderm-2.6.1/src/utils/components/Circle/Circle.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/utils/components/LoadingDots/loadingDots.css` & `jupyterlab_pachyderm-2.6.1/src/utils/components/LoadingDots/loadingDots.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Svgs/GenericError.js` & `jupyterlab_pachyderm-2.6.1/src/utils/components/Svgs/GenericError.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Svgs/KubernetesElephant.js` & `jupyterlab_pachyderm-2.6.1/src/utils/components/Svgs/KubernetesElephant.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Svgs/PachydermLogo.js` & `jupyterlab_pachyderm-2.6.1/src/utils/components/Svgs/PachydermLogo.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/utils/components/Svgs/StatusWarning.js` & `jupyterlab_pachyderm-2.6.1/src/utils/components/Svgs/StatusWarning.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/utils/hooks/useSort.ts` & `jupyterlab_pachyderm-2.6.1/src/utils/hooks/useSort.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/src/utils/icons.ts` & `jupyterlab_pachyderm-2.6.1/src/utils/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/style/base.css` & `jupyterlab_pachyderm-2.6.1/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/style/components/button.css` & `jupyterlab_pachyderm-2.6.1/style/components/button.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/style/icons/file.svg` & `jupyterlab_pachyderm-2.6.1/style/icons/file.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/style/icons/info.svg` & `jupyterlab_pachyderm-2.6.1/style/icons/info.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/style/icons/mount-logo.svg` & `jupyterlab_pachyderm-2.6.1/style/icons/mount-logo.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_pachyderm-2.6.0rc2/style/icons/repo.svg` & `jupyterlab_pachyderm-2.6.1/style/icons/repo.svg`

 * *Files identical despite different names*

