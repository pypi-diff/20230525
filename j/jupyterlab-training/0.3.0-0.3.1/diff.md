# Comparing `tmp/jupyterlab_training-0.3.0.tar.gz` & `tmp/jupyterlab_training-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_training-0.3.0.tar", last modified: Thu May 25 14:19:36 2023, max compression
+gzip compressed data, was "jupyterlab_training-0.3.1.tar", last modified: Thu May 25 15:00:52 2023, max compression
```

## Comparing `jupyterlab_training-0.3.0.tar` & `jupyterlab_training-0.3.1.tar`

### file list

```diff
@@ -1,574 +1,565 @@
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.710862 jupyterlab_training-0.3.0/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1516 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/LICENSE
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      435 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/MANIFEST.in
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3133 2023-05-25 14:19:36.710862 jupyterlab_training-0.3.0/PKG-INFO
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2375 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/README.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      199 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/install.json
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.918853 jupyterlab_training-0.3.0/jupyter-config/
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.930853 jupyterlab_training-0.3.0/jupyter-config/server-config/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       94 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/jupyter-config/server-config/jupyterlab-training.json
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.930853 jupyterlab_training-0.3.0/jupyterlab_training/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4311 2022-04-26 13:53:46.000000 jupyterlab_training-0.3.0/jupyterlab_training/__init__.py
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      473 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/jupyterlab_training/_version.py
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2277 2023-04-14 08:02:10.000000 jupyterlab_training-0.3.0/jupyterlab_training/db.py
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8227 2023-05-25 09:07:08.000000 jupyterlab_training-0.3.0/jupyterlab_training/handlers.py
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.930853 jupyterlab_training-0.3.0/jupyterlab_training/labextension/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    22621 2023-05-25 14:19:28.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/build_log.json
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3710 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/package.json
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.938853 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4436 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/9c539cf459fdeaebf6835c214cb5cac1d43cd5d497cf4b96647401981d180043.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   690266 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/lib_index_js.2449aa1867353f272d86.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   853257 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/lib_index_js.2449aa1867353f272d86.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3657 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/node_modules_file-saver_dist_FileSaver_min_js.7a6e01f58ee54adc0a2d.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10385 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/node_modules_file-saver_dist_FileSaver_min_js.7a6e01f58ee54adc0a2d.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    37044 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/remoteEntry.a514b68d4bfa7874093f.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    36004 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/remoteEntry.a514b68d4bfa7874093f.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      162 2023-05-25 14:19:28.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/style.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4262 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/style_index_js.90cbacf63e7b78baf3a0.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1431 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/style_index_js.90cbacf63e7b78baf3a0.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12068 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b34d146cd46239887005.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    13805 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b34d146cd46239887005.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    18778 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/vendors-node_modules_i18next-browser-languagedetector_dist_esm_i18nextBrowserLanguageDetector_js.461ad3153f790b00e805.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    17560 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/vendors-node_modules_i18next-browser-languagedetector_dist_esm_i18nextBrowserLanguageDetector_js.461ad3153f790b00e805.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    98957 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/vendors-node_modules_i18next_dist_esm_i18next_js.a7d4998d1b735c7aa976.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   102279 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/vendors-node_modules_i18next_dist_esm_i18next_js.a7d4998d1b735c7aa976.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   462780 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/vendors-node_modules_js-yaml_index_js.d7ae774bce0e28557217.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   538921 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/vendors-node_modules_js-yaml_index_js.d7ae774bce0e28557217.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   103711 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/vendors-node_modules_jszip_dist_jszip_min_js.b3f8875733e3ec888679.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   122137 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/vendors-node_modules_jszip_dist_jszip_min_js.b3f8875733e3ec888679.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   253464 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/vendors-node_modules_luxon_build_cjs-browser_luxon_js.fe773dc86647f20d9d58.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   414483 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/vendors-node_modules_luxon_build_cjs-browser_luxon_js.fe773dc86647f20d9d58.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   842358 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/vendors-node_modules_react-bootstrap_esm_index_js.6fbf310996ef2effea89.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   574567 2023-05-25 14:19:31.000000 jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/vendors-node_modules_react-bootstrap_esm_index_js.6fbf310996ef2effea89.js.map
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.930853 jupyterlab_training-0.3.0/jupyterlab_training.egg-info/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3133 2023-05-25 14:19:35.000000 jupyterlab_training-0.3.0/jupyterlab_training.egg-info/PKG-INFO
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    22792 2023-05-25 14:19:35.000000 jupyterlab_training-0.3.0/jupyterlab_training.egg-info/SOURCES.txt
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)        1 2023-05-25 14:19:35.000000 jupyterlab_training-0.3.0/jupyterlab_training.egg-info/dependency_links.txt
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)        1 2022-11-23 09:48:09.000000 jupyterlab_training-0.3.0/jupyterlab_training.egg-info/not-zip-safe
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      164 2023-05-25 14:19:35.000000 jupyterlab_training-0.3.0/jupyterlab_training.egg-info/requires.txt
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       20 2023-05-25 14:19:35.000000 jupyterlab_training-0.3.0/jupyterlab_training.egg-info/top_level.txt
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3804 2023-04-14 08:47:17.000000 jupyterlab_training-0.3.0/package.json
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      610 2022-04-26 12:17:31.000000 jupyterlab_training-0.3.0/pyproject.toml
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       38 2023-05-25 14:19:36.710862 jupyterlab_training-0.3.0/setup.cfg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2671 2022-04-26 13:51:23.000000 jupyterlab_training-0.3.0/setup.py
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.938853 jupyterlab_training-0.3.0/src/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1481 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/src/flake8.tsx
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.942854 jupyterlab_training-0.3.0/src/i18n/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    17168 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/src/i18n/index.ts
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3457 2023-04-14 10:37:08.000000 jupyterlab_training-0.3.0/src/index.ts
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7641 2023-05-25 13:39:32.000000 jupyterlab_training-0.3.0/src/menu.tsx
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1870 2023-04-04 13:29:43.000000 jupyterlab_training-0.3.0/src/model.tsx
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    19967 2023-04-05 08:23:46.000000 jupyterlab_training-0.3.0/src/panel.tsx
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4415 2022-04-26 12:49:05.000000 jupyterlab_training-0.3.0/src/progressButton.tsx
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4664 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/src/statsWidget.tsx
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8902 2023-05-09 07:57:45.000000 jupyterlab_training-0.3.0/src/tour.tsx
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1009 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/src/utils.tsx
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.942854 jupyterlab_training-0.3.0/style/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)        0 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/base.css
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.958854 jupyterlab_training-0.3.0/style/bootstrap/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      313 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/.babelrc.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      208 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/.editorconfig
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       56 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/.eslintignore
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7131 2023-04-04 13:29:43.000000 jupyterlab_training-0.3.0/style/bootstrap/.eslintrc.json
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      359 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/.gitattributes
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.958854 jupyterlab_training-0.3.0/style/bootstrap/.github/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    14268 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/.github/CONTRIBUTING.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1178 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      517 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/.gitignore
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       45 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/.stylelintignore
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6685 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/.stylelintrc
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      782 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/.travis.yml
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       17 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/CNAME
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3217 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/CODE_OF_CONDUCT.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      199 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/Gemfile
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1905 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/Gemfile.lock
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1131 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/LICENSE
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9138 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/README.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2505 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_config.yml
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.962854 jupyterlab_training-0.3.0/style/bootstrap/_data/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      418 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_data/breakpoints.yml
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9113 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_data/browser-bugs.yml
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3244 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_data/browser-features.yml
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      401 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_data/colors.yml
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2870 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_data/examples.yml
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      261 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_data/grays.yml
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1657 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_data/nav.yml
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      257 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_data/theme-colors.yml
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      519 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_data/translations.yml
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.966854 jupyterlab_training-0.3.0/style/bootstrap/_includes/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      137 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_includes/ads.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      445 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_includes/callout-danger-async-methods.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      451 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_includes/callout-info-mediaqueries-breakpoints.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      454 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_includes/callout-warning-color-assistive-technologies.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3520 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_includes/docs-navbar.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2269 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_includes/docs-sidebar.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      748 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_includes/favicons.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1148 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_includes/footer.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1540 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_includes/header.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.966854 jupyterlab_training-0.3.0/style/bootstrap/_includes/icons/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      890 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_includes/icons/bootstrap.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      482 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_includes/icons/download.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1116 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_includes/icons/github.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      441 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_includes/icons/import.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      442 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_includes/icons/lightning.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      410 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_includes/icons/menu.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1362 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_includes/icons/slack.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      861 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_includes/icons/twitter.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1376 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_includes/scripts.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1290 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_includes/social.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.970854 jupyterlab_training-0.3.0/style/bootstrap/_layouts/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      556 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_layouts/default.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1040 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_layouts/docs.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      538 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_layouts/examples.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      412 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_layouts/home.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1134 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_layouts/redirect.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      288 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_layouts/simple.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.970854 jupyterlab_training-0.3.0/style/bootstrap/_plugins/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1326 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_plugins/bugify.rb
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      827 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_plugins/callout.rb
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3402 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_plugins/example.rb
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      525 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/_plugins/markdown-block.rb
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.922853 jupyterlab_training-0.3.0/style/bootstrap/assets/
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.974854 jupyterlab_training-0.3.0/style/bootstrap/assets/brand/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1306 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/brand/bootstrap-outline.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1140 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/brand/bootstrap-punchout.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    23959 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/brand/bootstrap-social-logo.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   231733 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/brand/bootstrap-social.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1127 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/brand/bootstrap-solid.svg
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.974854 jupyterlab_training-0.3.0/style/bootstrap/assets/css/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    21574 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/css/docs.min.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    40321 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/css/docs.min.css.map
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.974854 jupyterlab_training-0.3.0/style/bootstrap/assets/img/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    52160 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/img/bootstrap-stack.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    80588 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/img/bootstrap-themes.png
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.978854 jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1935 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/android-chrome-192x192.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4269 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/android-chrome-512x512.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1738 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/apple-touch-icon.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      292 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/browserconfig.xml
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      310 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/favicon-16x16.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      491 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/favicon-32x32.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      550 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/manifest.json
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1479 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/mstile-144x144.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1428 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/mstile-150x150.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1746 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/mstile-310x150.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3085 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/mstile-310x310.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1104 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/mstile-70x70.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1025 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/safari-pinned-tab.svg
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.978854 jupyterlab_training-0.3.0/style/bootstrap/assets/js/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      490 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/js/.eslintrc.json
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    52015 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/js/docs.min.js
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.982854 jupyterlab_training-0.3.0/style/bootstrap/assets/js/src/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4518 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/js/src/application.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2005 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/js/src/ie-emulation-modes-warning.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      545 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/js/src/pwa.js
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.982854 jupyterlab_training-0.3.0/style/bootstrap/assets/js/vendor/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5389 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/js/vendor/anchor.min.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10917 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/js/vendor/clipboard.min.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    32283 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/js/vendor/holder.min.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    69597 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/js/vendor/jquery-slim.min.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    19188 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/js/vendor/popper.min.js
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.126855 jupyterlab_training-0.3.0/style/bootstrap/assets/scss/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      593 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_ads.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3422 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_algolia.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      172 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_anchor.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1827 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_brand.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      195 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_browser-bugs.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      487 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_buttons.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      695 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_callouts.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      574 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_clipboard-js.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      419 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_colors.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6341 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_component-examples.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1995 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_content.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      363 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_examples.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      459 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_footer.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      887 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_masthead.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1685 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_nav.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2724 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_sidebar.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      213 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_skiplink.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1669 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_syntax.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      382 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_variables.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1520 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/assets/scss/docs.scss
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.130856 jupyterlab_training-0.3.0/style/bootstrap/build/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      385 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/build/.eslintrc.json
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1260 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/build/.htmllintrc
--rwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)     2758 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/build/change-version.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2304 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/build/gcp-key.json.enc
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1505 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/build/generate-sri.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2070 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/build/lint-vars.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      238 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/build/postcss.config.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1379 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/build/rollup.config.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1221 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/build/sauce_browsers.json
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3116 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/build/saucelabs-unit-test.js
--rwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)     2778 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/build/ship.sh
--rwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)      701 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/build/upload-preview.sh
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2605 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/build/vnu-jar.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      156 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/build/workbox.config.json
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1282 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/build/workbox.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      744 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/composer.json
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.922853 jupyterlab_training-0.3.0/style/bootstrap/dist/
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.138856 jupyterlab_training-0.3.0/style/bootstrap/dist/css/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    43852 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap-grid.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    95910 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap-grid.css.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    34243 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap-grid.min.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    76209 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap-grid.min.css.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4798 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap-reboot.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    57721 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap-reboot.css.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3936 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap-reboot.min.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    25881 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   178152 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   411645 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap.css.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   144877 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap.min.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   551641 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap.min.css.map
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.150856 jupyterlab_training-0.3.0/style/bootstrap/dist/js/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   195855 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/dist/js/bootstrap.bundle.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   326634 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/dist/js/bootstrap.bundle.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    67742 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/dist/js/bootstrap.bundle.min.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   273872 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/dist/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   115048 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/dist/js/bootstrap.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   195373 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/dist/js/bootstrap.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    48944 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/dist/js/bootstrap.min.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   161998 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/dist/js/bootstrap.min.js.map
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.922853 jupyterlab_training-0.3.0/style/bootstrap/docs/
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.154856 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.154856 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/about/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2940 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/about/brand.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1717 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/about/license.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2495 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/about/overview.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      630 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/about/translations.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2474 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/browser-bugs.md
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.266857 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4439 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/alerts.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3450 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/badge.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1503 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/breadcrumb.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9208 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/button-group.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7445 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/buttons.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    26080 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/card.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12440 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/carousel.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12091 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/collapse.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    33022 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/dropdowns.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    51564 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/forms.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12974 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/input-group.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1199 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/jumbotron.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    18093 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/list-group.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    29516 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/modal.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    23281 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/navbar.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    35152 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/navs.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6170 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/pagination.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    15225 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/popovers.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6318 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/progress.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    18827 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/scrollspy.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    15834 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/tooltips.md
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.266857 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/content/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1436 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/content/code.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1329 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/content/figures.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3349 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/content/images.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12826 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/content/reboot.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    16669 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/content/tables.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10926 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/content/typography.md
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.270857 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      185 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/.eslintrc.json
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      339 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/.stylelintrc
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.270857 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/album/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      655 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/album/album.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12744 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/album/index.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.270857 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/blog/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2133 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/blog/blog.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12774 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/blog/index.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.270857 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/carousel/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1658 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/carousel/carousel.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10159 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/carousel/index.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.270857 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/checkout/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      287 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/checkout/form-validation.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11933 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/checkout/index.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.270857 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/cover/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1503 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/cover/cover.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2340 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/cover/index.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.270857 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/dashboard/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1539 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/dashboard/dashboard.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10152 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/dashboard/index.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.274857 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/floating-labels/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1716 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/floating-labels/floating-labels.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1824 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/floating-labels/index.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.274857 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/grid/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      372 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/grid/grid.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5271 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/grid/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1001 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/index.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.274857 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/jumbotron/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4989 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/jumbotron/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      107 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/jumbotron/jumbotron.css
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.274857 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/navbar-bottom/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2852 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/navbar-bottom/index.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.274857 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/navbar-fixed/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2777 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/navbar-fixed/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       87 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/navbar-fixed/navbar-top-fixed.css
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.274857 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/navbar-static/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2783 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/navbar-static/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       67 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/navbar-static/navbar-top.css
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.278857 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/navbars/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    16619 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/navbars/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       69 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/navbars/navbar.css
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.278857 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/offcanvas/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7697 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/offcanvas/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1756 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/offcanvas/offcanvas.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      148 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/offcanvas/offcanvas.js
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.278857 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/pricing/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6160 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/pricing/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      377 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/pricing/pricing.css
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.278857 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/product/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9286 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/product/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1383 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/product/product.css
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.334858 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    26370 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/album.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    36944 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/blog.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    31465 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/carousel.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    28180 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/checkout.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    17953 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/cover.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    26556 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/dashboard.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11053 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/floating-labels.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    33860 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/grid.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    38408 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/jumbotron.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11316 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/navbar-bottom.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    13616 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/navbar-fixed.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    14893 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/navbar-static.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    27187 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/navbars.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    23975 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/offcanvas.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    29128 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/pricing.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    27953 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/product.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5680 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/sign-in.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11334 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/starter-template.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    15836 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/sticky-footer-navbar.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9665 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/sticky-footer.png
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.338858 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/sign-in/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1462 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/sign-in/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      902 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/sign-in/signin.css
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.338858 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/starter-template/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3196 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/starter-template/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       98 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/starter-template/starter-template.css
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.338858 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/sticky-footer/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1122 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/sticky-footer/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      613 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/sticky-footer/sticky-footer.css
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.342858 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/sticky-footer-navbar/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3104 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/sticky-footer-navbar/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      693 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/sticky-footer-navbar/sticky-footer-navbar.css
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.342858 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/tooltip-viewport/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2417 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/tooltip-viewport/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      385 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/tooltip-viewport/tooltip-viewport.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      583 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/tooltip-viewport/tooltip-viewport.js
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.346858 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/extend/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6986 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/extend/approach.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      987 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/extend/icons.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       59 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/extend/index.md
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.490859 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/getting-started/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4099 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/getting-started/accessibility.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      617 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/getting-started/best-practices.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9246 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/getting-started/browsers-devices.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3527 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/getting-started/build-tools.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5408 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/getting-started/contents.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4716 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/getting-started/download.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7193 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/getting-started/introduction.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6596 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/getting-started/javascript.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    17078 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/getting-started/theming.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3364 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/getting-started/webpack.md
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.494860 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/layout/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    24684 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/layout/grid.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7742 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/layout/media-object.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6737 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/layout/overview.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2039 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/layout/utilities-for-layout.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    27814 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/migration.md
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.502860 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2381 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/borders.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      985 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/clearfix.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      378 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/close-icon.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2758 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/colors.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3915 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/display.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1655 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/embed.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    20834 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/flex.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1607 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/float.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      758 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/image-replacement.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1525 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/position.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      811 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/screenreaders.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1722 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/sizing.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3078 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/spacing.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2825 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/text.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1285 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/vertical-align.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      751 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/visibility.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5430 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/favicon.ico
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4384 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/index.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:35.926853 jupyterlab_training-0.3.0/style/bootstrap/js/
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.518860 jupyterlab_training-0.3.0/style/bootstrap/js/dist/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4948 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/alert.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8180 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/alert.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5221 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/button.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8975 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/button.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    15569 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/carousel.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    28130 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/carousel.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11524 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/collapse.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    21118 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/collapse.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    15011 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/dropdown.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    26869 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/dropdown.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      921 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/index.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2222 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/index.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    18307 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/modal.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    33324 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/modal.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6301 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/popover.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9090 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/popover.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10254 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/scrollspy.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    18393 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/scrollspy.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7472 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/tab.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    13674 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/tab.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    19826 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/tooltip.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    37424 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/tooltip.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4359 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/util.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8425 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/dist/util.js.map
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.522860 jupyterlab_training-0.3.0/style/bootstrap/js/src/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4148 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/src/alert.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4672 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/src/button.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    14305 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/src/carousel.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10530 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/src/collapse.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    14017 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/src/dropdown.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1373 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/src/index.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    16753 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/src/modal.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4710 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/src/popover.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9218 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/src/scrollspy.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6922 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/src/tab.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    18575 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/src/tooltip.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4185 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/src/util.js
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.522860 jupyterlab_training-0.3.0/style/bootstrap/js/tests/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2769 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/README.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4330 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1602 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/karma.conf.js
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.526860 jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      632 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/.eslintrc.json
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2760 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/alert.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7344 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/button.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    36530 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/carousel.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    34057 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/collapse.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    33910 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/dropdown.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    26038 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/modal.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    16308 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/popover.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    27058 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/scrollspy.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    16396 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/tab.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    29666 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/tooltip.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2473 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/util.js
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.526860 jupyterlab_training-0.3.0/style/bootstrap/js/tests/vendor/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    92629 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/vendor/jquery-1.9.1.min.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7875 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/vendor/qunit.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   145326 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/vendor/qunit.js
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.570860 jupyterlab_training-0.3.0/style/bootstrap/js/tests/visual/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2185 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/visual/alert.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3011 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/visual/button.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2301 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/visual/carousel.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4128 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/visual/collapse.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8864 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/visual/dropdown.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    13438 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/visual/modal.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1960 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/visual/popover.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    19115 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/visual/scrollspy.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    32329 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/visual/tab.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3147 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/js/tests/visual/tooltip.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.574860 jupyterlab_training-0.3.0/style/bootstrap/nuget/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      935 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/nuget/MyGet.ps1
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1385 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/nuget/bootstrap.nuspec
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1409 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/nuget/bootstrap.sass.nuspec
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   433474 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/package-lock.json
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      530 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/package.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9152 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/package.json
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      123 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/robots.txt
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      249 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/sache.json
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.698862 jupyterlab_training-0.3.0/style/bootstrap/scss/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1150 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_alert.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      982 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_badge.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1249 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_breadcrumb.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3647 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_button-group.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2714 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_buttons.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5693 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_card.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4221 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_carousel.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      860 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_close.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1065 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_code.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7797 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_custom-forms.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3092 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_dropdown.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8766 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_forms.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2657 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_functions.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1016 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_grid.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1146 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_images.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4864 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_input-group.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      378 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_jumbotron.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2887 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_list-group.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       83 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_media.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1018 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_mixins.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4623 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_modal.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2022 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_nav.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6781 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_navbar.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1834 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_pagination.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4536 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_popover.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2768 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_print.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      841 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_progress.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11591 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_reboot.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      572 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_root.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3426 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_tables.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2503 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_tooltip.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      452 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_transitions.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2115 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_type.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      407 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_utilities.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    35747 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/_variables.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      648 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/bootstrap-grid.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      410 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/bootstrap-reboot.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      881 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/bootstrap.scss
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.706862 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      242 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_alert.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      474 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_background-variant.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      230 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_badge.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      722 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_border-radius.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       87 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_box-shadow.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4468 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_breakpoints.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3182 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_buttons.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1459 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_caret.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       93 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_clearfix.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      193 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_float.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3199 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_forms.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2024 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_gradients.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1899 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_grid-framework.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1606 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_grid.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      783 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_hover.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1172 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_image.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      429 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_list-group.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      168 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_lists.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      220 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_nav-divider.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      385 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_navbar-align.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      453 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_pagination.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      547 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_reset-text.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      202 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_resize.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      778 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_screen-reader.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       98 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_size.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      647 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_table-row.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      259 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_text-emphasis.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      231 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_text-hide.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      168 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_text-truncate.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      192 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_transition.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      134 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_visibility.scss
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.710862 jupyterlab_training-0.3.0/style/bootstrap/scss/utilities/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      420 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/utilities/_align.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      397 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/utilities/_background.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1551 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/utilities/_borders.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       37 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/utilities/_clearfix.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1409 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/utilities/_display.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      727 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/utilities/_embed.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2458 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/utilities/_flex.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      320 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/utilities/_float.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      614 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/utilities/_position.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      115 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/utilities/_screenreaders.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      298 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/utilities/_sizing.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1406 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/utilities/_spacing.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1338 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/utilities/_text.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      121 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/scss/utilities/_visibility.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      114 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/bootstrap/sw.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    39502 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/homePage.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3761 2022-11-16 10:58:25.000000 jupyterlab_training-0.3.0/style/index.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       21 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/index.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1051 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/logilab-icon.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1150 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/logilab.ico
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7498 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/logilab.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4436 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.0/style/stop_app.png
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 14:19:36.710862 jupyterlab_training-0.3.0/tests/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1138 2022-01-12 11:00:40.000000 jupyterlab_training-0.3.0/tests/test_handlers.py
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      569 2023-04-04 13:32:50.000000 jupyterlab_training-0.3.0/tsconfig.json
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.737838 jupyterlab_training-0.3.1/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1516 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/LICENSE
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      435 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/MANIFEST.in
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3133 2023-05-25 15:00:52.737838 jupyterlab_training-0.3.1/PKG-INFO
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2375 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/README.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      199 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/install.json
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.865829 jupyterlab_training-0.3.1/jupyter-config/
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.869829 jupyterlab_training-0.3.1/jupyter-config/server-config/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       94 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/jupyter-config/server-config/jupyterlab-training.json
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.873829 jupyterlab_training-0.3.1/jupyterlab_training/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4311 2022-04-26 13:53:46.000000 jupyterlab_training-0.3.1/jupyterlab_training/__init__.py
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      473 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/jupyterlab_training/_version.py
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2277 2023-04-14 08:02:10.000000 jupyterlab_training-0.3.1/jupyterlab_training/db.py
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8227 2023-05-25 09:07:08.000000 jupyterlab_training-0.3.1/jupyterlab_training/handlers.py
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.873829 jupyterlab_training-0.3.1/jupyterlab_training/labextension/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3710 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/package.json
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.873829 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   115723 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/147.61d247f0dd79cb5e6c03.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      121 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/147.61d247f0dd79cb5e6c03.js.LICENSE.txt
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2686 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/162.54797b341de4f60c5f53.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    44687 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/169.dde25e4dfa365788e2d3.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   242635 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/3.97e5ce5c6c551fd93ee6.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   197062 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/320.e87de993e15ebd1d087e.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      225 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/320.e87de993e15ebd1d087e.js.LICENSE.txt
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    72799 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/490.76b7872fc9815805fce9.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7272 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/71.b08e1d3adafbcb17349c.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    98509 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/733.c4acd437d42492321d94.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      383 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/733.c4acd437d42492321d94.js.LICENSE.txt
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3378 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/747.d4b5f772f188f310ccf4.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4436 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/9c539cf459fdeaebf6835c214cb5cac1d43cd5d497cf4b96647401981d180043.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9396 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/remoteEntry.1860e2c61e01ab7c6b1c.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      162 2023-05-25 15:00:41.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/style.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    69137 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.873829 jupyterlab_training-0.3.1/jupyterlab_training.egg-info/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3133 2023-05-25 15:00:51.000000 jupyterlab_training-0.3.1/jupyterlab_training.egg-info/PKG-INFO
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    21243 2023-05-25 15:00:51.000000 jupyterlab_training-0.3.1/jupyterlab_training.egg-info/SOURCES.txt
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)        1 2023-05-25 15:00:51.000000 jupyterlab_training-0.3.1/jupyterlab_training.egg-info/dependency_links.txt
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)        1 2023-05-25 15:00:51.000000 jupyterlab_training-0.3.1/jupyterlab_training.egg-info/not-zip-safe
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      158 2023-05-25 15:00:51.000000 jupyterlab_training-0.3.1/jupyterlab_training.egg-info/requires.txt
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       20 2023-05-25 15:00:51.000000 jupyterlab_training-0.3.1/jupyterlab_training.egg-info/top_level.txt
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3804 2023-05-25 14:59:50.000000 jupyterlab_training-0.3.1/package.json
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      610 2022-04-26 12:17:31.000000 jupyterlab_training-0.3.1/pyproject.toml
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       38 2023-05-25 15:00:52.737838 jupyterlab_training-0.3.1/setup.cfg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2671 2022-04-26 13:51:23.000000 jupyterlab_training-0.3.1/setup.py
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.873829 jupyterlab_training-0.3.1/src/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1481 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/src/flake8.tsx
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.877829 jupyterlab_training-0.3.1/src/i18n/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    17168 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/src/i18n/index.ts
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3457 2023-04-14 10:37:08.000000 jupyterlab_training-0.3.1/src/index.ts
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7641 2023-05-25 13:39:32.000000 jupyterlab_training-0.3.1/src/menu.tsx
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1870 2023-04-04 13:29:43.000000 jupyterlab_training-0.3.1/src/model.tsx
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    19967 2023-04-05 08:23:46.000000 jupyterlab_training-0.3.1/src/panel.tsx
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4415 2022-04-26 12:49:05.000000 jupyterlab_training-0.3.1/src/progressButton.tsx
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4664 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/src/statsWidget.tsx
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8902 2023-05-09 07:57:45.000000 jupyterlab_training-0.3.1/src/tour.tsx
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1009 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/src/utils.tsx
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.877829 jupyterlab_training-0.3.1/style/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)        0 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/base.css
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.881829 jupyterlab_training-0.3.1/style/bootstrap/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      313 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/.babelrc.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      208 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/.editorconfig
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       56 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/.eslintignore
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7131 2023-04-04 13:29:43.000000 jupyterlab_training-0.3.1/style/bootstrap/.eslintrc.json
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      359 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/.gitattributes
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.881829 jupyterlab_training-0.3.1/style/bootstrap/.github/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    14268 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/.github/CONTRIBUTING.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1178 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      517 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/.gitignore
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       45 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/.stylelintignore
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6685 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/.stylelintrc
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      782 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/.travis.yml
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       17 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/CNAME
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3217 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/CODE_OF_CONDUCT.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      199 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/Gemfile
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1905 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/Gemfile.lock
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1131 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/LICENSE
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9138 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/README.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2505 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_config.yml
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.881829 jupyterlab_training-0.3.1/style/bootstrap/_data/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      418 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_data/breakpoints.yml
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9113 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_data/browser-bugs.yml
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3244 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_data/browser-features.yml
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      401 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_data/colors.yml
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2870 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_data/examples.yml
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      261 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_data/grays.yml
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1657 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_data/nav.yml
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      257 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_data/theme-colors.yml
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      519 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_data/translations.yml
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.881829 jupyterlab_training-0.3.1/style/bootstrap/_includes/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      137 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/ads.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      445 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/callout-danger-async-methods.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      451 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/callout-info-mediaqueries-breakpoints.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      454 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/callout-warning-color-assistive-technologies.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3520 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/docs-navbar.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2269 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/docs-sidebar.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      748 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/favicons.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1148 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/footer.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1540 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/header.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.881829 jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      890 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/bootstrap.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      482 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/download.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1116 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/github.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      441 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/import.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      442 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/lightning.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      410 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/menu.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1362 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/slack.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      861 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/twitter.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1376 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/scripts.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1290 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/social.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.881829 jupyterlab_training-0.3.1/style/bootstrap/_layouts/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      556 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_layouts/default.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1040 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_layouts/docs.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      538 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_layouts/examples.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      412 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_layouts/home.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1134 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_layouts/redirect.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      288 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_layouts/simple.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.885829 jupyterlab_training-0.3.1/style/bootstrap/_plugins/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1326 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_plugins/bugify.rb
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      827 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_plugins/callout.rb
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3402 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_plugins/example.rb
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      525 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_plugins/markdown-block.rb
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.865829 jupyterlab_training-0.3.1/style/bootstrap/assets/
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.885829 jupyterlab_training-0.3.1/style/bootstrap/assets/brand/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1306 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/brand/bootstrap-outline.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1140 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/brand/bootstrap-punchout.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    23959 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/brand/bootstrap-social-logo.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   231733 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/brand/bootstrap-social.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1127 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/brand/bootstrap-solid.svg
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.885829 jupyterlab_training-0.3.1/style/bootstrap/assets/css/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    21574 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/css/docs.min.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    40321 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/css/docs.min.css.map
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.885829 jupyterlab_training-0.3.1/style/bootstrap/assets/img/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    52160 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/bootstrap-stack.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    80588 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/bootstrap-themes.png
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.885829 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1935 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/android-chrome-192x192.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4269 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/android-chrome-512x512.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1738 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/apple-touch-icon.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      292 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/browserconfig.xml
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      310 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/favicon-16x16.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      491 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/favicon-32x32.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      550 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/manifest.json
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1479 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/mstile-144x144.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1428 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/mstile-150x150.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1746 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/mstile-310x150.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3085 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/mstile-310x310.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1104 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/mstile-70x70.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1025 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/safari-pinned-tab.svg
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.885829 jupyterlab_training-0.3.1/style/bootstrap/assets/js/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      490 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/js/.eslintrc.json
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    52015 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/js/docs.min.js
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.885829 jupyterlab_training-0.3.1/style/bootstrap/assets/js/src/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4518 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/js/src/application.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2005 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/js/src/ie-emulation-modes-warning.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      545 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/js/src/pwa.js
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.885829 jupyterlab_training-0.3.1/style/bootstrap/assets/js/vendor/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5389 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/js/vendor/anchor.min.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10917 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/js/vendor/clipboard.min.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    32283 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/js/vendor/holder.min.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    69597 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/js/vendor/jquery-slim.min.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    19188 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/js/vendor/popper.min.js
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.069831 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      593 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_ads.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3422 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_algolia.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      172 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_anchor.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1827 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_brand.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      195 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_browser-bugs.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      487 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_buttons.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      695 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_callouts.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      574 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_clipboard-js.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      419 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_colors.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6341 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_component-examples.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1995 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_content.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      363 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_examples.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      459 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_footer.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      887 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_masthead.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1685 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_nav.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2724 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_sidebar.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      213 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_skiplink.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1669 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_syntax.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      382 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_variables.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1520 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/docs.scss
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.073831 jupyterlab_training-0.3.1/style/bootstrap/build/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      385 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/.eslintrc.json
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1260 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/.htmllintrc
+-rwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)     2758 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/change-version.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2304 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/gcp-key.json.enc
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1505 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/generate-sri.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2070 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/lint-vars.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      238 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/postcss.config.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1379 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/rollup.config.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1221 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/sauce_browsers.json
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3116 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/saucelabs-unit-test.js
+-rwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)     2778 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/ship.sh
+-rwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)      701 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/upload-preview.sh
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2605 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/vnu-jar.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      156 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/workbox.config.json
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1282 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/workbox.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      744 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/composer.json
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.865829 jupyterlab_training-0.3.1/style/bootstrap/dist/
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.077831 jupyterlab_training-0.3.1/style/bootstrap/dist/css/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    43852 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-grid.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    95910 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-grid.css.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    34243 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-grid.min.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    76209 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4798 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-reboot.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    57721 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-reboot.css.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3936 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-reboot.min.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    25881 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   178152 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   411645 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap.css.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   144877 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap.min.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   551641 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap.min.css.map
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.077831 jupyterlab_training-0.3.1/style/bootstrap/dist/js/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   195855 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.bundle.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   326634 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.bundle.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    67742 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.bundle.min.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   273872 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   115048 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   195373 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    48944 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.min.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   161998 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.min.js.map
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.865829 jupyterlab_training-0.3.1/style/bootstrap/docs/
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.077831 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.081831 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/about/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2940 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/about/brand.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1717 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/about/license.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2495 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/about/overview.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      630 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/about/translations.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2474 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/browser-bugs.md
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.081831 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4439 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/alerts.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3450 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/badge.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1503 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/breadcrumb.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9208 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/button-group.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7445 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/buttons.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    26080 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/card.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12440 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/carousel.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12091 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/collapse.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    33022 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/dropdowns.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    51564 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/forms.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12974 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/input-group.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1199 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/jumbotron.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    18093 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/list-group.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    29516 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/modal.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    23281 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/navbar.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    35152 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/navs.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6170 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/pagination.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    15225 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/popovers.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6318 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/progress.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    18827 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/scrollspy.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    15834 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/tooltips.md
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.081831 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1436 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/code.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1329 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/figures.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3349 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/images.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12826 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/reboot.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    16669 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/tables.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10926 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/typography.md
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.121832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      185 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/.eslintrc.json
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      339 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/.stylelintrc
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.125832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/album/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      655 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/album/album.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12744 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/album/index.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.125832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/blog/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2133 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/blog/blog.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12774 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/blog/index.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.125832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/carousel/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1658 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/carousel/carousel.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10159 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/carousel/index.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.125832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/checkout/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      287 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/checkout/form-validation.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11933 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/checkout/index.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.125832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/cover/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1503 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/cover/cover.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2340 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/cover/index.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.129832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/dashboard/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1539 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/dashboard/dashboard.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10152 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/dashboard/index.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.129832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/floating-labels/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1716 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/floating-labels/floating-labels.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1824 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/floating-labels/index.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.129832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/grid/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      372 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/grid/grid.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5271 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/grid/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1001 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/index.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.129832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/jumbotron/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4989 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/jumbotron/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      107 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/jumbotron/jumbotron.css
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.129832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbar-bottom/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2852 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbar-bottom/index.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.129832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbar-fixed/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2777 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbar-fixed/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       87 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbar-fixed/navbar-top-fixed.css
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.133832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbar-static/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2783 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbar-static/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       67 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbar-static/navbar-top.css
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.133832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbars/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    16619 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbars/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       69 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbars/navbar.css
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.133832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/offcanvas/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7697 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/offcanvas/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1756 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/offcanvas/offcanvas.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      148 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/offcanvas/offcanvas.js
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.325834 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/pricing/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6160 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/pricing/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      377 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/pricing/pricing.css
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.325834 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/product/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9286 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/product/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1383 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/product/product.css
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.337834 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    26370 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/album.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    36944 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/blog.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    31465 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/carousel.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    28180 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/checkout.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    17953 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/cover.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    26556 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/dashboard.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11053 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/floating-labels.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    33860 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/grid.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    38408 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/jumbotron.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11316 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/navbar-bottom.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    13616 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/navbar-fixed.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    14893 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/navbar-static.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    27187 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/navbars.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    23975 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/offcanvas.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    29128 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/pricing.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    27953 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/product.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5680 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/sign-in.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11334 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/starter-template.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    15836 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/sticky-footer-navbar.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9665 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/sticky-footer.png
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.337834 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sign-in/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1462 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sign-in/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      902 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sign-in/signin.css
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.337834 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/starter-template/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3196 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/starter-template/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       98 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/starter-template/starter-template.css
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.337834 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sticky-footer/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1122 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sticky-footer/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      613 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sticky-footer/sticky-footer.css
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.337834 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sticky-footer-navbar/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3104 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sticky-footer-navbar/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      693 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sticky-footer-navbar/sticky-footer-navbar.css
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.341834 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/tooltip-viewport/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2417 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/tooltip-viewport/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      385 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/tooltip-viewport/tooltip-viewport.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      583 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/tooltip-viewport/tooltip-viewport.js
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.341834 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/extend/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6986 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/extend/approach.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      987 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/extend/icons.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       59 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/extend/index.md
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.345834 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4099 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/accessibility.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      617 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/best-practices.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9246 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/browsers-devices.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3527 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/build-tools.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5408 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/contents.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4716 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/download.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7193 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/introduction.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6596 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/javascript.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    17078 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/theming.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3364 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/webpack.md
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.345834 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/layout/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    24684 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/layout/grid.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7742 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/layout/media-object.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6737 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/layout/overview.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2039 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/layout/utilities-for-layout.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    27814 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/migration.md
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.433835 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2381 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/borders.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      985 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/clearfix.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      378 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/close-icon.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2758 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/colors.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3915 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/display.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1655 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/embed.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    20834 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/flex.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1607 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/float.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      758 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/image-replacement.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1525 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/position.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      811 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/screenreaders.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1722 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/sizing.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3078 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/spacing.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2825 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/text.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1285 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/vertical-align.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      751 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/visibility.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5430 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/favicon.ico
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4384 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/index.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.869829 jupyterlab_training-0.3.1/style/bootstrap/js/
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.441835 jupyterlab_training-0.3.1/style/bootstrap/js/dist/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4948 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/alert.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8180 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/alert.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5221 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/button.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8975 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/button.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    15569 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/carousel.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    28130 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/carousel.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11524 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/collapse.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    21118 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/collapse.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    15011 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/dropdown.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    26869 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/dropdown.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      921 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/index.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2222 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/index.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    18307 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/modal.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    33324 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/modal.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6301 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/popover.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9090 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/popover.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10254 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/scrollspy.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    18393 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/scrollspy.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7472 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/tab.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    13674 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/tab.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    19826 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/tooltip.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    37424 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/tooltip.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4359 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/util.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8425 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/util.js.map
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.633837 jupyterlab_training-0.3.1/style/bootstrap/js/src/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4148 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/alert.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4672 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/button.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    14305 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/carousel.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10530 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/collapse.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    14017 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/dropdown.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1373 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/index.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    16753 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/modal.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4710 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/popover.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9218 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/scrollspy.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6922 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/tab.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    18575 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/tooltip.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4185 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/util.js
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.633837 jupyterlab_training-0.3.1/style/bootstrap/js/tests/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2769 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/README.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4330 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1602 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/karma.conf.js
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.641837 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      632 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/.eslintrc.json
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2760 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/alert.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7344 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/button.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    36530 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/carousel.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    34057 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/collapse.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    33910 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/dropdown.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    26038 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/modal.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    16308 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/popover.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    27058 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/scrollspy.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    16396 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/tab.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    29666 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/tooltip.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2473 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/util.js
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.641837 jupyterlab_training-0.3.1/style/bootstrap/js/tests/vendor/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    92629 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/vendor/jquery-1.9.1.min.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7875 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/vendor/qunit.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   145326 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/vendor/qunit.js
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.641837 jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2185 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/alert.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3011 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/button.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2301 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/carousel.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4128 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/collapse.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8864 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/dropdown.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    13438 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/modal.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1960 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/popover.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    19115 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/scrollspy.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    32329 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/tab.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3147 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/tooltip.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.641837 jupyterlab_training-0.3.1/style/bootstrap/nuget/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      935 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/nuget/MyGet.ps1
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1385 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/nuget/bootstrap.nuspec
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1409 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/nuget/bootstrap.sass.nuspec
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   433474 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/package-lock.json
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      530 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/package.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9152 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/package.json
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      123 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/robots.txt
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      249 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/sache.json
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.645837 jupyterlab_training-0.3.1/style/bootstrap/scss/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1150 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_alert.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      982 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_badge.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1249 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_breadcrumb.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3647 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_button-group.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2714 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_buttons.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5693 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_card.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4221 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_carousel.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      860 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_close.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1065 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_code.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7797 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_custom-forms.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3092 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_dropdown.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8766 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_forms.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2657 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_functions.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1016 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_grid.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1146 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_images.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4864 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_input-group.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      378 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_jumbotron.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2887 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_list-group.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       83 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_media.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1018 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_mixins.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4623 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_modal.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2022 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_nav.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6781 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_navbar.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1834 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_pagination.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4536 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_popover.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2768 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_print.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      841 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_progress.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11591 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_reboot.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      572 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_root.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3426 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_tables.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2503 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_tooltip.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      452 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_transitions.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2115 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_type.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      407 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_utilities.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    35747 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_variables.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      648 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/bootstrap-grid.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      410 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/bootstrap-reboot.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      881 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/bootstrap.scss
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.733838 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      242 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_alert.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      474 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_background-variant.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      230 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_badge.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      722 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_border-radius.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       87 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_box-shadow.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4468 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_breakpoints.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3182 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_buttons.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1459 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_caret.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       93 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_clearfix.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      193 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_float.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3199 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_forms.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2024 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_gradients.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1899 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_grid-framework.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1606 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_grid.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      783 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_hover.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1172 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_image.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      429 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_list-group.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      168 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_lists.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      220 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_nav-divider.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      385 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_navbar-align.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      453 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_pagination.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      547 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_reset-text.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      202 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_resize.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      778 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_screen-reader.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       98 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_size.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      647 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_table-row.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      259 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_text-emphasis.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      231 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_text-hide.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      168 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_text-truncate.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      192 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_transition.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      134 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_visibility.scss
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.737838 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      420 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_align.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      397 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_background.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1551 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_borders.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       37 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_clearfix.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1409 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_display.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      727 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_embed.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2458 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_flex.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      320 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_float.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      614 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_position.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      115 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_screenreaders.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      298 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_sizing.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1406 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_spacing.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1338 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_text.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      121 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_visibility.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      114 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/sw.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    39502 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/homePage.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3761 2022-11-16 10:58:25.000000 jupyterlab_training-0.3.1/style/index.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       21 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/index.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1051 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/logilab-icon.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1150 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/logilab.ico
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7498 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/logilab.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4436 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/stop_app.png
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.737838 jupyterlab_training-0.3.1/tests/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1138 2022-01-12 11:00:40.000000 jupyterlab_training-0.3.1/tests/test_handlers.py
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      569 2023-04-04 13:32:50.000000 jupyterlab_training-0.3.1/tsconfig.json
```

### Comparing `jupyterlab_training-0.3.0/LICENSE` & `jupyterlab_training-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/PKG-INFO` & `jupyterlab_training-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_training
-Version: 0.3.0
+Version: 0.3.1
 Summary: jupyterlab training courses and exercices platform
 Home-page: https://gitlab.com/logilab/jupyterlab-training
 Author: Logilab
 Author-email: ogiorgis@logilab.fr
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `jupyterlab_training-0.3.0/README.md` & `jupyterlab_training-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/jupyterlab_training/__init__.py` & `jupyterlab_training-0.3.1/jupyterlab_training/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/jupyterlab_training/db.py` & `jupyterlab_training-0.3.1/jupyterlab_training/db.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/jupyterlab_training/handlers.py` & `jupyterlab_training-0.3.1/jupyterlab_training/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/jupyterlab_training/labextension/package.json` & `jupyterlab_training-0.3.1/jupyterlab_training/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9743055555555555%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.1860e2c61e01ab7c6b1c.js'}}",*

 * * "'version'": "'0.3.1'"}*

```diff
@@ -52,15 +52,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://gitlab.com/logilab/jupyterlab-training",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.a514b68d4bfa7874093f.js",
+            "load": "static/remoteEntry.1860e2c61e01ab7c6b1c.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_training/labextension"
     },
     "keywords": [
         "jupyter",
@@ -101,9 +101,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.0"
+    "version": "0.3.1"
 }
```

### Comparing `jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/9c539cf459fdeaebf6835c214cb5cac1d43cd5d497cf4b96647401981d180043.png` & `jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/9c539cf459fdeaebf6835c214cb5cac1d43cd5d497cf4b96647401981d180043.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/jupyterlab_training/labextension/static/vendors-node_modules_jszip_dist_jszip_min_js.b3f8875733e3ec888679.js` & `jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/733.c4acd437d42492321d94.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,3530 +1,3329 @@
-(self["webpackChunkjupyterlab_training"] = self["webpackChunkjupyterlab_training"] || []).push([
-    ["vendors-node_modules_jszip_dist_jszip_min_js"], {
-
-        /***/
-        "./node_modules/jszip/dist/jszip.min.js":
-            /*!**********************************************!*\
-              !*** ./node_modules/jszip/dist/jszip.min.js ***!
-              \**********************************************/
-            /***/
-            ((module, __unused_webpack_exports, __webpack_require__) => {
-
-                /* provided dependency */
-                var process = __webpack_require__( /*! process/browser */ "./node_modules/process/browser.js");
-                /*!
-
-                JSZip v3.10.1 - A JavaScript class for generating and reading zip files
-                <http://stuartk.com/jszip>
-
-                (c) 2009-2016 Stuart Knightley <stuart [at] stuartk.com>
-                Dual licenced under the MIT license or GPLv3. See https://raw.github.com/Stuk/jszip/main/LICENSE.markdown.
-
-                JSZip uses the library pako released under the MIT license :
-                https://github.com/nodeca/pako/blob/main/LICENSE
-                */
-
-                ! function(e) {
-                    if (true) module.exports = e();
-                    else {}
-                }(function() {
-                    return function s(a, o, h) {
-                        function u(r, e) {
-                            if (!o[r]) {
-                                if (!a[r]) {
-                                    var t = undefined;
-                                    if (!e && t) return require(r, !0);
-                                    if (l) return l(r, !0);
-                                    var n = new Error("Cannot find module '" + r + "'");
-                                    throw n.code = "MODULE_NOT_FOUND", n
-                                }
-                                var i = o[r] = {
-                                    exports: {}
-                                };
-                                a[r][0].call(i.exports, function(e) {
-                                    var t = a[r][1][e];
-                                    return u(t || e)
-                                }, i, i.exports, s, a, o, h)
-                            }
-                            return o[r].exports
-                        }
-                        for (var l = undefined, e = 0; e < h.length; e++) u(h[e]);
-                        return u
-                    }({
-                        1: [function(e, t, r) {
-                            "use strict";
-                            var d = e("./utils"),
-                                c = e("./support"),
-                                p = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/=";
-                            r.encode = function(e) {
-                                for (var t, r, n, i, s, a, o, h = [], u = 0, l = e.length, f = l, c = "string" !== d.getTypeOf(e); u < e.length;) f = l - u, n = c ? (t = e[u++], r = u < l ? e[u++] : 0, u < l ? e[u++] : 0) : (t = e.charCodeAt(u++), r = u < l ? e.charCodeAt(u++) : 0, u < l ? e.charCodeAt(u++) : 0), i = t >> 2, s = (3 & t) << 4 | r >> 4, a = 1 < f ? (15 & r) << 2 | n >> 6 : 64, o = 2 < f ? 63 & n : 64, h.push(p.charAt(i) + p.charAt(s) + p.charAt(a) + p.charAt(o));
-                                return h.join("")
-                            }, r.decode = function(e) {
-                                var t, r, n, i, s, a, o = 0,
-                                    h = 0,
-                                    u = "data:";
-                                if (e.substr(0, u.length) === u) throw new Error("Invalid base64 input, it looks like a data url.");
-                                var l, f = 3 * (e = e.replace(/[^A-Za-z0-9+/=]/g, "")).length / 4;
-                                if (e.charAt(e.length - 1) === p.charAt(64) && f--, e.charAt(e.length - 2) === p.charAt(64) && f--, f % 1 != 0) throw new Error("Invalid base64 input, bad content length.");
-                                for (l = c.uint8array ? new Uint8Array(0 | f) : new Array(0 | f); o < e.length;) t = p.indexOf(e.charAt(o++)) << 2 | (i = p.indexOf(e.charAt(o++))) >> 4, r = (15 & i) << 4 | (s = p.indexOf(e.charAt(o++))) >> 2, n = (3 & s) << 6 | (a = p.indexOf(e.charAt(o++))), l[h++] = t, 64 !== s && (l[h++] = r), 64 !== a && (l[h++] = n);
-                                return l
-                            }
-                        }, {
-                            "./support": 30,
-                            "./utils": 32
-                        }],
-                        2: [function(e, t, r) {
-                            "use strict";
-                            var n = e("./external"),
-                                i = e("./stream/DataWorker"),
-                                s = e("./stream/Crc32Probe"),
-                                a = e("./stream/DataLengthProbe");
-
-                            function o(e, t, r, n, i) {
-                                this.compressedSize = e, this.uncompressedSize = t, this.crc32 = r, this.compression = n, this.compressedContent = i
-                            }
-                            o.prototype = {
-                                getContentWorker: function() {
-                                    var e = new i(n.Promise.resolve(this.compressedContent)).pipe(this.compression.uncompressWorker()).pipe(new a("data_length")),
-                                        t = this;
-                                    return e.on("end", function() {
-                                        if (this.streamInfo.data_length !== t.uncompressedSize) throw new Error("Bug : uncompressed data size mismatch")
-                                    }), e
-                                },
-                                getCompressedWorker: function() {
-                                    return new i(n.Promise.resolve(this.compressedContent)).withStreamInfo("compressedSize", this.compressedSize).withStreamInfo("uncompressedSize", this.uncompressedSize).withStreamInfo("crc32", this.crc32).withStreamInfo("compression", this.compression)
-                                }
-                            }, o.createWorkerFrom = function(e, t, r) {
-                                return e.pipe(new s).pipe(new a("uncompressedSize")).pipe(t.compressWorker(r)).pipe(new a("compressedSize")).withStreamInfo("compression", t)
-                            }, t.exports = o
-                        }, {
-                            "./external": 6,
-                            "./stream/Crc32Probe": 25,
-                            "./stream/DataLengthProbe": 26,
-                            "./stream/DataWorker": 27
-                        }],
-                        3: [function(e, t, r) {
-                            "use strict";
-                            var n = e("./stream/GenericWorker");
-                            r.STORE = {
-                                magic: "\0\0",
-                                compressWorker: function() {
-                                    return new n("STORE compression")
-                                },
-                                uncompressWorker: function() {
-                                    return new n("STORE decompression")
-                                }
-                            }, r.DEFLATE = e("./flate")
-                        }, {
-                            "./flate": 7,
-                            "./stream/GenericWorker": 28
-                        }],
-                        4: [function(e, t, r) {
-                            "use strict";
-                            var n = e("./utils");
-                            var o = function() {
-                                for (var e, t = [], r = 0; r < 256; r++) {
-                                    e = r;
-                                    for (var n = 0; n < 8; n++) e = 1 & e ? 3988292384 ^ e >>> 1 : e >>> 1;
-                                    t[r] = e
-                                }
-                                return t
-                            }();
-                            t.exports = function(e, t) {
-                                return void 0 !== e && e.length ? "string" !== n.getTypeOf(e) ? function(e, t, r, n) {
-                                    var i = o,
-                                        s = n + r;
-                                    e ^= -1;
-                                    for (var a = n; a < s; a++) e = e >>> 8 ^ i[255 & (e ^ t[a])];
-                                    return -1 ^ e
-                                }(0 | t, e, e.length, 0) : function(e, t, r, n) {
-                                    var i = o,
-                                        s = n + r;
-                                    e ^= -1;
-                                    for (var a = n; a < s; a++) e = e >>> 8 ^ i[255 & (e ^ t.charCodeAt(a))];
-                                    return -1 ^ e
-                                }(0 | t, e, e.length, 0) : 0
-                            }
-                        }, {
-                            "./utils": 32
-                        }],
-                        5: [function(e, t, r) {
-                            "use strict";
-                            r.base64 = !1, r.binary = !1, r.dir = !1, r.createFolders = !0, r.date = null, r.compression = null, r.compressionOptions = null, r.comment = null, r.unixPermissions = null, r.dosPermissions = null
-                        }, {}],
-                        6: [function(e, t, r) {
-                            "use strict";
-                            var n = null;
-                            n = "undefined" != typeof Promise ? Promise : e("lie"), t.exports = {
-                                Promise: n
-                            }
-                        }, {
-                            lie: 37
-                        }],
-                        7: [function(e, t, r) {
-                            "use strict";
-                            var n = "undefined" != typeof Uint8Array && "undefined" != typeof Uint16Array && "undefined" != typeof Uint32Array,
-                                i = e("pako"),
-                                s = e("./utils"),
-                                a = e("./stream/GenericWorker"),
-                                o = n ? "uint8array" : "array";
-
-                            function h(e, t) {
-                                a.call(this, "FlateWorker/" + e), this._pako = null, this._pakoAction = e, this._pakoOptions = t, this.meta = {}
-                            }
-                            r.magic = "\b\0", s.inherits(h, a), h.prototype.processChunk = function(e) {
-                                this.meta = e.meta, null === this._pako && this._createPako(), this._pako.push(s.transformTo(o, e.data), !1)
-                            }, h.prototype.flush = function() {
-                                a.prototype.flush.call(this), null === this._pako && this._createPako(), this._pako.push([], !0)
-                            }, h.prototype.cleanUp = function() {
-                                a.prototype.cleanUp.call(this), this._pako = null
-                            }, h.prototype._createPako = function() {
-                                this._pako = new i[this._pakoAction]({
-                                    raw: !0,
-                                    level: this._pakoOptions.level || -1
-                                });
-                                var t = this;
-                                this._pako.onData = function(e) {
-                                    t.push({
-                                        data: e,
-                                        meta: t.meta
-                                    })
-                                }
-                            }, r.compressWorker = function(e) {
-                                return new h("Deflate", e)
-                            }, r.uncompressWorker = function() {
-                                return new h("Inflate", {})
-                            }
-                        }, {
-                            "./stream/GenericWorker": 28,
-                            "./utils": 32,
-                            pako: 38
-                        }],
-                        8: [function(e, t, r) {
-                            "use strict";
-
-                            function A(e, t) {
-                                var r, n = "";
-                                for (r = 0; r < t; r++) n += String.fromCharCode(255 & e), e >>>= 8;
-                                return n
-                            }
-
-                            function n(e, t, r, n, i, s) {
-                                var a, o, h = e.file,
-                                    u = e.compression,
-                                    l = s !== O.utf8encode,
-                                    f = I.transformTo("string", s(h.name)),
-                                    c = I.transformTo("string", O.utf8encode(h.name)),
-                                    d = h.comment,
-                                    p = I.transformTo("string", s(d)),
-                                    m = I.transformTo("string", O.utf8encode(d)),
-                                    _ = c.length !== h.name.length,
-                                    g = m.length !== d.length,
-                                    b = "",
-                                    v = "",
-                                    y = "",
-                                    w = h.dir,
-                                    k = h.date,
-                                    x = {
-                                        crc32: 0,
-                                        compressedSize: 0,
-                                        uncompressedSize: 0
-                                    };
-                                t && !r || (x.crc32 = e.crc32, x.compressedSize = e.compressedSize, x.uncompressedSize = e.uncompressedSize);
-                                var S = 0;
-                                t && (S |= 8), l || !_ && !g || (S |= 2048);
-                                var z = 0,
-                                    C = 0;
-                                w && (z |= 16), "UNIX" === i ? (C = 798, z |= function(e, t) {
-                                    var r = e;
-                                    return e || (r = t ? 16893 : 33204), (65535 & r) << 16
-                                }(h.unixPermissions, w)) : (C = 20, z |= function(e) {
-                                    return 63 & (e || 0)
-                                }(h.dosPermissions)), a = k.getUTCHours(), a <<= 6, a |= k.getUTCMinutes(), a <<= 5, a |= k.getUTCSeconds() / 2, o = k.getUTCFullYear() - 1980, o <<= 4, o |= k.getUTCMonth() + 1, o <<= 5, o |= k.getUTCDate(), _ && (v = A(1, 1) + A(B(f), 4) + c, b += "up" + A(v.length, 2) + v), g && (y = A(1, 1) + A(B(p), 4) + m, b += "uc" + A(y.length, 2) + y);
-                                var E = "";
-                                return E += "\n\0", E += A(S, 2), E += u.magic, E += A(a, 2), E += A(o, 2), E += A(x.crc32, 4), E += A(x.compressedSize, 4), E += A(x.uncompressedSize, 4), E += A(f.length, 2), E += A(b.length, 2), {
-                                    fileRecord: R.LOCAL_FILE_HEADER + E + f + b,
-                                    dirRecord: R.CENTRAL_FILE_HEADER + A(C, 2) + E + A(p.length, 2) + "\0\0\0\0" + A(z, 4) + A(n, 4) + f + b + p
-                                }
-                            }
-                            var I = e("../utils"),
-                                i = e("../stream/GenericWorker"),
-                                O = e("../utf8"),
-                                B = e("../crc32"),
-                                R = e("../signature");
-
-                            function s(e, t, r, n) {
-                                i.call(this, "ZipFileWorker"), this.bytesWritten = 0, this.zipComment = t, this.zipPlatform = r, this.encodeFileName = n, this.streamFiles = e, this.accumulate = !1, this.contentBuffer = [], this.dirRecords = [], this.currentSourceOffset = 0, this.entriesCount = 0, this.currentFile = null, this._sources = []
-                            }
-                            I.inherits(s, i), s.prototype.push = function(e) {
-                                var t = e.meta.percent || 0,
-                                    r = this.entriesCount,
-                                    n = this._sources.length;
-                                this.accumulate ? this.contentBuffer.push(e) : (this.bytesWritten += e.data.length, i.prototype.push.call(this, {
-                                    data: e.data,
-                                    meta: {
-                                        currentFile: this.currentFile,
-                                        percent: r ? (t + 100 * (r - n - 1)) / r : 100
-                                    }
-                                }))
-                            }, s.prototype.openedSource = function(e) {
-                                this.currentSourceOffset = this.bytesWritten, this.currentFile = e.file.name;
-                                var t = this.streamFiles && !e.file.dir;
-                                if (t) {
-                                    var r = n(e, t, !1, this.currentSourceOffset, this.zipPlatform, this.encodeFileName);
-                                    this.push({
-                                        data: r.fileRecord,
-                                        meta: {
-                                            percent: 0
-                                        }
-                                    })
-                                } else this.accumulate = !0
-                            }, s.prototype.closedSource = function(e) {
-                                this.accumulate = !1;
-                                var t = this.streamFiles && !e.file.dir,
-                                    r = n(e, t, !0, this.currentSourceOffset, this.zipPlatform, this.encodeFileName);
-                                if (this.dirRecords.push(r.dirRecord), t) this.push({
-                                    data: function(e) {
-                                        return R.DATA_DESCRIPTOR + A(e.crc32, 4) + A(e.compressedSize, 4) + A(e.uncompressedSize, 4)
-                                    }(e),
-                                    meta: {
-                                        percent: 100
-                                    }
-                                });
-                                else
-                                    for (this.push({
-                                            data: r.fileRecord,
-                                            meta: {
-                                                percent: 0
-                                            }
-                                        }); this.contentBuffer.length;) this.push(this.contentBuffer.shift());
-                                this.currentFile = null
-                            }, s.prototype.flush = function() {
-                                for (var e = this.bytesWritten, t = 0; t < this.dirRecords.length; t++) this.push({
-                                    data: this.dirRecords[t],
-                                    meta: {
-                                        percent: 100
-                                    }
-                                });
-                                var r = this.bytesWritten - e,
-                                    n = function(e, t, r, n, i) {
-                                        var s = I.transformTo("string", i(n));
-                                        return R.CENTRAL_DIRECTORY_END + "\0\0\0\0" + A(e, 2) + A(e, 2) + A(t, 4) + A(r, 4) + A(s.length, 2) + s
-                                    }(this.dirRecords.length, r, e, this.zipComment, this.encodeFileName);
-                                this.push({
-                                    data: n,
-                                    meta: {
-                                        percent: 100
-                                    }
-                                })
-                            }, s.prototype.prepareNextSource = function() {
-                                this.previous = this._sources.shift(), this.openedSource(this.previous.streamInfo), this.isPaused ? this.previous.pause() : this.previous.resume()
-                            }, s.prototype.registerPrevious = function(e) {
-                                this._sources.push(e);
-                                var t = this;
-                                return e.on("data", function(e) {
-                                    t.processChunk(e)
-                                }), e.on("end", function() {
-                                    t.closedSource(t.previous.streamInfo), t._sources.length ? t.prepareNextSource() : t.end()
-                                }), e.on("error", function(e) {
-                                    t.error(e)
-                                }), this
-                            }, s.prototype.resume = function() {
-                                return !!i.prototype.resume.call(this) && (!this.previous && this._sources.length ? (this.prepareNextSource(), !0) : this.previous || this._sources.length || this.generatedError ? void 0 : (this.end(), !0))
-                            }, s.prototype.error = function(e) {
-                                var t = this._sources;
-                                if (!i.prototype.error.call(this, e)) return !1;
-                                for (var r = 0; r < t.length; r++) try {
-                                    t[r].error(e)
-                                } catch (e) {}
-                                return !0
-                            }, s.prototype.lock = function() {
-                                i.prototype.lock.call(this);
-                                for (var e = this._sources, t = 0; t < e.length; t++) e[t].lock()
-                            }, t.exports = s
-                        }, {
-                            "../crc32": 4,
-                            "../signature": 23,
-                            "../stream/GenericWorker": 28,
-                            "../utf8": 31,
-                            "../utils": 32
-                        }],
-                        9: [function(e, t, r) {
-                            "use strict";
-                            var u = e("../compressions"),
-                                n = e("./ZipFileWorker");
-                            r.generateWorker = function(e, a, t) {
-                                var o = new n(a.streamFiles, t, a.platform, a.encodeFileName),
-                                    h = 0;
-                                try {
-                                    e.forEach(function(e, t) {
-                                        h++;
-                                        var r = function(e, t) {
-                                                var r = e || t,
-                                                    n = u[r];
-                                                if (!n) throw new Error(r + " is not a valid compression method !");
-                                                return n
-                                            }(t.options.compression, a.compression),
-                                            n = t.options.compressionOptions || a.compressionOptions || {},
-                                            i = t.dir,
-                                            s = t.date;
-                                        t._compressWorker(r, n).withStreamInfo("file", {
-                                            name: e,
-                                            dir: i,
-                                            date: s,
-                                            comment: t.comment || "",
-                                            unixPermissions: t.unixPermissions,
-                                            dosPermissions: t.dosPermissions
-                                        }).pipe(o)
-                                    }), o.entriesCount = h
-                                } catch (e) {
-                                    o.error(e)
-                                }
-                                return o
-                            }
-                        }, {
-                            "../compressions": 3,
-                            "./ZipFileWorker": 8
-                        }],
-                        10: [function(e, t, r) {
-                            "use strict";
-
-                            function n() {
-                                if (!(this instanceof n)) return new n;
-                                if (arguments.length) throw new Error("The constructor with parameters has been removed in JSZip 3.0, please check the upgrade guide.");
-                                this.files = Object.create(null), this.comment = null, this.root = "", this.clone = function() {
-                                    var e = new n;
-                                    for (var t in this) "function" != typeof this[t] && (e[t] = this[t]);
-                                    return e
-                                }
-                            }(n.prototype = e("./object")).loadAsync = e("./load"), n.support = e("./support"), n.defaults = e("./defaults"), n.version = "3.10.1", n.loadAsync = function(e, t) {
-                                return (new n).loadAsync(e, t)
-                            }, n.external = e("./external"), t.exports = n
-                        }, {
-                            "./defaults": 5,
-                            "./external": 6,
-                            "./load": 11,
-                            "./object": 15,
-                            "./support": 30
-                        }],
-                        11: [function(e, t, r) {
-                            "use strict";
-                            var u = e("./utils"),
-                                i = e("./external"),
-                                n = e("./utf8"),
-                                s = e("./zipEntries"),
-                                a = e("./stream/Crc32Probe"),
-                                l = e("./nodejsUtils");
-
-                            function f(n) {
-                                return new i.Promise(function(e, t) {
-                                    var r = n.decompressed.getContentWorker().pipe(new a);
-                                    r.on("error", function(e) {
-                                        t(e)
-                                    }).on("end", function() {
-                                        r.streamInfo.crc32 !== n.decompressed.crc32 ? t(new Error("Corrupted zip : CRC32 mismatch")) : e()
-                                    }).resume()
-                                })
-                            }
-                            t.exports = function(e, o) {
-                                var h = this;
-                                return o = u.extend(o || {}, {
-                                    base64: !1,
-                                    checkCRC32: !1,
-                                    optimizedBinaryString: !1,
-                                    createFolders: !1,
-                                    decodeFileName: n.utf8decode
-                                }), l.isNode && l.isStream(e) ? i.Promise.reject(new Error("JSZip can't accept a stream when loading a zip file.")) : u.prepareContent("the loaded zip file", e, !0, o.optimizedBinaryString, o.base64).then(function(e) {
-                                    var t = new s(o);
-                                    return t.load(e), t
-                                }).then(function(e) {
-                                    var t = [i.Promise.resolve(e)],
-                                        r = e.files;
-                                    if (o.checkCRC32)
-                                        for (var n = 0; n < r.length; n++) t.push(f(r[n]));
-                                    return i.Promise.all(t)
-                                }).then(function(e) {
-                                    for (var t = e.shift(), r = t.files, n = 0; n < r.length; n++) {
-                                        var i = r[n],
-                                            s = i.fileNameStr,
-                                            a = u.resolve(i.fileNameStr);
-                                        h.file(a, i.decompressed, {
-                                            binary: !0,
-                                            optimizedBinaryString: !0,
-                                            date: i.date,
-                                            dir: i.dir,
-                                            comment: i.fileCommentStr.length ? i.fileCommentStr : null,
-                                            unixPermissions: i.unixPermissions,
-                                            dosPermissions: i.dosPermissions,
-                                            createFolders: o.createFolders
-                                        }), i.dir || (h.file(a).unsafeOriginalName = s)
-                                    }
-                                    return t.zipComment.length && (h.comment = t.zipComment), h
-                                })
-                            }
-                        }, {
-                            "./external": 6,
-                            "./nodejsUtils": 14,
-                            "./stream/Crc32Probe": 25,
-                            "./utf8": 31,
-                            "./utils": 32,
-                            "./zipEntries": 33
-                        }],
-                        12: [function(e, t, r) {
-                            "use strict";
-                            var n = e("../utils"),
-                                i = e("../stream/GenericWorker");
+/*! For license information please see 733.c4acd437d42492321d94.js.LICENSE.txt */
+(self.webpackChunkjupyterlab_training = self.webpackChunkjupyterlab_training || []).push([
+    [733], {
+        5733: (t, e, r) => {
+            var n = r(4155);
+            t.exports = function t(e, r, n) {
+                function i(a, o) {
+                    if (!r[a]) {
+                        if (!e[a]) {
+                            if (s) return s(a, !0);
+                            var h = new Error("Cannot find module '" + a + "'");
+                            throw h.code = "MODULE_NOT_FOUND", h
+                        }
+                        var u = r[a] = {
+                            exports: {}
+                        };
+                        e[a][0].call(u.exports, (function(t) {
+                            return i(e[a][1][t] || t)
+                        }), u, u.exports, t, e, r, n)
+                    }
+                    return r[a].exports
+                }
+                for (var s = void 0, a = 0; a < n.length; a++) i(n[a]);
+                return i
+            }({
+                1: [function(t, e, r) {
+                    "use strict";
+                    var n = t("./utils"),
+                        i = t("./support"),
+                        s = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/=";
+                    r.encode = function(t) {
+                        for (var e, r, i, a, o, h, u, l = [], f = 0, c = t.length, d = c, p = "string" !== n.getTypeOf(t); f < t.length;) d = c - f, i = p ? (e = t[f++], r = f < c ? t[f++] : 0, f < c ? t[f++] : 0) : (e = t.charCodeAt(f++), r = f < c ? t.charCodeAt(f++) : 0, f < c ? t.charCodeAt(f++) : 0), a = e >> 2, o = (3 & e) << 4 | r >> 4, h = 1 < d ? (15 & r) << 2 | i >> 6 : 64, u = 2 < d ? 63 & i : 64, l.push(s.charAt(a) + s.charAt(o) + s.charAt(h) + s.charAt(u));
+                        return l.join("")
+                    }, r.decode = function(t) {
+                        var e, r, n, a, o, h, u = 0,
+                            l = 0,
+                            f = "data:";
+                        if (t.substr(0, f.length) === f) throw new Error("Invalid base64 input, it looks like a data url.");
+                        var c, d = 3 * (t = t.replace(/[^A-Za-z0-9+/=]/g, "")).length / 4;
+                        if (t.charAt(t.length - 1) === s.charAt(64) && d--, t.charAt(t.length - 2) === s.charAt(64) && d--, d % 1 != 0) throw new Error("Invalid base64 input, bad content length.");
+                        for (c = i.uint8array ? new Uint8Array(0 | d) : new Array(0 | d); u < t.length;) e = s.indexOf(t.charAt(u++)) << 2 | (a = s.indexOf(t.charAt(u++))) >> 4, r = (15 & a) << 4 | (o = s.indexOf(t.charAt(u++))) >> 2, n = (3 & o) << 6 | (h = s.indexOf(t.charAt(u++))), c[l++] = e, 64 !== o && (c[l++] = r), 64 !== h && (c[l++] = n);
+                        return c
+                    }
+                }, {
+                    "./support": 30,
+                    "./utils": 32
+                }],
+                2: [function(t, e, r) {
+                    "use strict";
+                    var n = t("./external"),
+                        i = t("./stream/DataWorker"),
+                        s = t("./stream/Crc32Probe"),
+                        a = t("./stream/DataLengthProbe");
 
-                            function s(e, t) {
-                                i.call(this, "Nodejs stream input adapter for " + e), this._upstreamEnded = !1, this._bindStream(t)
-                            }
-                            n.inherits(s, i), s.prototype._bindStream = function(e) {
-                                var t = this;
-                                (this._stream = e).pause(), e.on("data", function(e) {
-                                    t.push({
-                                        data: e,
-                                        meta: {
-                                            percent: 0
-                                        }
-                                    })
-                                }).on("error", function(e) {
-                                    t.isPaused ? this.generatedError = e : t.error(e)
-                                }).on("end", function() {
-                                    t.isPaused ? t._upstreamEnded = !0 : t.end()
-                                })
-                            }, s.prototype.pause = function() {
-                                return !!i.prototype.pause.call(this) && (this._stream.pause(), !0)
-                            }, s.prototype.resume = function() {
-                                return !!i.prototype.resume.call(this) && (this._upstreamEnded ? this.end() : this._stream.resume(), !0)
-                            }, t.exports = s
-                        }, {
-                            "../stream/GenericWorker": 28,
-                            "../utils": 32
-                        }],
-                        13: [function(e, t, r) {
-                            "use strict";
-                            var i = e("readable-stream").Readable;
+                    function o(t, e, r, n, i) {
+                        this.compressedSize = t, this.uncompressedSize = e, this.crc32 = r, this.compression = n, this.compressedContent = i
+                    }
+                    o.prototype = {
+                        getContentWorker: function() {
+                            var t = new i(n.Promise.resolve(this.compressedContent)).pipe(this.compression.uncompressWorker()).pipe(new a("data_length")),
+                                e = this;
+                            return t.on("end", (function() {
+                                if (this.streamInfo.data_length !== e.uncompressedSize) throw new Error("Bug : uncompressed data size mismatch")
+                            })), t
+                        },
+                        getCompressedWorker: function() {
+                            return new i(n.Promise.resolve(this.compressedContent)).withStreamInfo("compressedSize", this.compressedSize).withStreamInfo("uncompressedSize", this.uncompressedSize).withStreamInfo("crc32", this.crc32).withStreamInfo("compression", this.compression)
+                        }
+                    }, o.createWorkerFrom = function(t, e, r) {
+                        return t.pipe(new s).pipe(new a("uncompressedSize")).pipe(e.compressWorker(r)).pipe(new a("compressedSize")).withStreamInfo("compression", e)
+                    }, e.exports = o
+                }, {
+                    "./external": 6,
+                    "./stream/Crc32Probe": 25,
+                    "./stream/DataLengthProbe": 26,
+                    "./stream/DataWorker": 27
+                }],
+                3: [function(t, e, r) {
+                    "use strict";
+                    var n = t("./stream/GenericWorker");
+                    r.STORE = {
+                        magic: "\0\0",
+                        compressWorker: function() {
+                            return new n("STORE compression")
+                        },
+                        uncompressWorker: function() {
+                            return new n("STORE decompression")
+                        }
+                    }, r.DEFLATE = t("./flate")
+                }, {
+                    "./flate": 7,
+                    "./stream/GenericWorker": 28
+                }],
+                4: [function(t, e, r) {
+                    "use strict";
+                    var n = t("./utils"),
+                        i = function() {
+                            for (var t, e = [], r = 0; r < 256; r++) {
+                                t = r;
+                                for (var n = 0; n < 8; n++) t = 1 & t ? 3988292384 ^ t >>> 1 : t >>> 1;
+                                e[r] = t
+                            }
+                            return e
+                        }();
+                    e.exports = function(t, e) {
+                        return void 0 !== t && t.length ? "string" !== n.getTypeOf(t) ? function(t, e, r, n) {
+                            var s = i,
+                                a = 0 + r;
+                            t ^= -1;
+                            for (var o = 0; o < a; o++) t = t >>> 8 ^ s[255 & (t ^ e[o])];
+                            return -1 ^ t
+                        }(0 | e, t, t.length) : function(t, e, r, n) {
+                            var s = i,
+                                a = 0 + r;
+                            t ^= -1;
+                            for (var o = 0; o < a; o++) t = t >>> 8 ^ s[255 & (t ^ e.charCodeAt(o))];
+                            return -1 ^ t
+                        }(0 | e, t, t.length) : 0
+                    }
+                }, {
+                    "./utils": 32
+                }],
+                5: [function(t, e, r) {
+                    "use strict";
+                    r.base64 = !1, r.binary = !1, r.dir = !1, r.createFolders = !0, r.date = null, r.compression = null, r.compressionOptions = null, r.comment = null, r.unixPermissions = null, r.dosPermissions = null
+                }, {}],
+                6: [function(t, e, r) {
+                    "use strict";
+                    var n;
+                    n = "undefined" != typeof Promise ? Promise : t("lie"), e.exports = {
+                        Promise: n
+                    }
+                }, {
+                    lie: 37
+                }],
+                7: [function(t, e, r) {
+                    "use strict";
+                    var n = "undefined" != typeof Uint8Array && "undefined" != typeof Uint16Array && "undefined" != typeof Uint32Array,
+                        i = t("pako"),
+                        s = t("./utils"),
+                        a = t("./stream/GenericWorker"),
+                        o = n ? "uint8array" : "array";
 
-                            function n(e, t, r) {
-                                i.call(this, t), this._helper = e;
-                                var n = this;
-                                e.on("data", function(e, t) {
-                                    n.push(e) || n._helper.pause(), r && r(t)
-                                }).on("error", function(e) {
-                                    n.emit("error", e)
-                                }).on("end", function() {
-                                    n.push(null)
-                                })
-                            }
-                            e("../utils").inherits(n, i), n.prototype._read = function() {
-                                this._helper.resume()
-                            }, t.exports = n
-                        }, {
-                            "../utils": 32,
-                            "readable-stream": 16
-                        }],
-                        14: [function(e, t, r) {
-                            "use strict";
-                            t.exports = {
-                                isNode: "undefined" != typeof Buffer,
-                                newBufferFrom: function(e, t) {
-                                    if (Buffer.from && Buffer.from !== Uint8Array.from) return Buffer.from(e, t);
-                                    if ("number" == typeof e) throw new Error('The "data" argument must not be a number');
-                                    return new Buffer(e, t)
-                                },
-                                allocBuffer: function(e) {
-                                    if (Buffer.alloc) return Buffer.alloc(e);
-                                    var t = new Buffer(e);
-                                    return t.fill(0), t
-                                },
-                                isBuffer: function(e) {
-                                    return Buffer.isBuffer(e)
-                                },
-                                isStream: function(e) {
-                                    return e && "function" == typeof e.on && "function" == typeof e.pause && "function" == typeof e.resume
-                                }
-                            }
-                        }, {}],
-                        15: [function(e, t, r) {
-                            "use strict";
+                    function h(t, e) {
+                        a.call(this, "FlateWorker/" + t), this._pako = null, this._pakoAction = t, this._pakoOptions = e, this.meta = {}
+                    }
+                    r.magic = "\b\0", s.inherits(h, a), h.prototype.processChunk = function(t) {
+                        this.meta = t.meta, null === this._pako && this._createPako(), this._pako.push(s.transformTo(o, t.data), !1)
+                    }, h.prototype.flush = function() {
+                        a.prototype.flush.call(this), null === this._pako && this._createPako(), this._pako.push([], !0)
+                    }, h.prototype.cleanUp = function() {
+                        a.prototype.cleanUp.call(this), this._pako = null
+                    }, h.prototype._createPako = function() {
+                        this._pako = new i[this._pakoAction]({
+                            raw: !0,
+                            level: this._pakoOptions.level || -1
+                        });
+                        var t = this;
+                        this._pako.onData = function(e) {
+                            t.push({
+                                data: e,
+                                meta: t.meta
+                            })
+                        }
+                    }, r.compressWorker = function(t) {
+                        return new h("Deflate", t)
+                    }, r.uncompressWorker = function() {
+                        return new h("Inflate", {})
+                    }
+                }, {
+                    "./stream/GenericWorker": 28,
+                    "./utils": 32,
+                    pako: 38
+                }],
+                8: [function(t, e, r) {
+                    "use strict";
+
+                    function n(t, e) {
+                        var r, n = "";
+                        for (r = 0; r < e; r++) n += String.fromCharCode(255 & t), t >>>= 8;
+                        return n
+                    }
 
-                            function s(e, t, r) {
-                                var n, i = u.getTypeOf(t),
-                                    s = u.extend(r || {}, f);
-                                s.date = s.date || new Date, null !== s.compression && (s.compression = s.compression.toUpperCase()), "string" == typeof s.unixPermissions && (s.unixPermissions = parseInt(s.unixPermissions, 8)), s.unixPermissions && 16384 & s.unixPermissions && (s.dir = !0), s.dosPermissions && 16 & s.dosPermissions && (s.dir = !0), s.dir && (e = g(e)), s.createFolders && (n = _(e)) && b.call(this, n, !0);
-                                var a = "string" === i && !1 === s.binary && !1 === s.base64;
-                                r && void 0 !== r.binary || (s.binary = !a), (t instanceof c && 0 === t.uncompressedSize || s.dir || !t || 0 === t.length) && (s.base64 = !1, s.binary = !0, t = "", s.compression = "STORE", i = "string");
-                                var o = null;
-                                o = t instanceof c || t instanceof l ? t : p.isNode && p.isStream(t) ? new m(e, t) : u.prepareContent(e, t, s.binary, s.optimizedBinaryString, s.base64);
-                                var h = new d(e, o, s);
-                                this.files[e] = h
-                            }
-                            var i = e("./utf8"),
-                                u = e("./utils"),
-                                l = e("./stream/GenericWorker"),
-                                a = e("./stream/StreamHelper"),
-                                f = e("./defaults"),
-                                c = e("./compressedObject"),
-                                d = e("./zipObject"),
-                                o = e("./generate"),
-                                p = e("./nodejsUtils"),
-                                m = e("./nodejs/NodejsStreamInputAdapter"),
-                                _ = function(e) {
-                                    "/" === e.slice(-1) && (e = e.substring(0, e.length - 1));
-                                    var t = e.lastIndexOf("/");
-                                    return 0 < t ? e.substring(0, t) : ""
-                                },
-                                g = function(e) {
-                                    return "/" !== e.slice(-1) && (e += "/"), e
-                                },
-                                b = function(e, t) {
-                                    return t = void 0 !== t ? t : f.createFolders, e = g(e), this.files[e] || s.call(this, e, null, {
-                                        dir: !0,
-                                        createFolders: t
-                                    }), this.files[e]
-                                };
-
-                            function h(e) {
-                                return "[object RegExp]" === Object.prototype.toString.call(e)
-                            }
-                            var n = {
-                                load: function() {
-                                    throw new Error("This method has been removed in JSZip 3.0, please check the upgrade guide.")
-                                },
-                                forEach: function(e) {
-                                    var t, r, n;
-                                    for (t in this.files) n = this.files[t], (r = t.slice(this.root.length, t.length)) && t.slice(0, this.root.length) === this.root && e(r, n)
-                                },
-                                filter: function(r) {
-                                    var n = [];
-                                    return this.forEach(function(e, t) {
-                                        r(e, t) && n.push(t)
-                                    }), n
-                                },
-                                file: function(e, t, r) {
-                                    if (1 !== arguments.length) return e = this.root + e, s.call(this, e, t, r), this;
-                                    if (h(e)) {
-                                        var n = e;
-                                        return this.filter(function(e, t) {
-                                            return !t.dir && n.test(e)
-                                        })
-                                    }
-                                    var i = this.files[this.root + e];
-                                    return i && !i.dir ? i : null
-                                },
-                                folder: function(r) {
-                                    if (!r) return this;
-                                    if (h(r)) return this.filter(function(e, t) {
-                                        return t.dir && r.test(e)
-                                    });
-                                    var e = this.root + r,
-                                        t = b.call(this, e),
-                                        n = this.clone();
-                                    return n.root = t.name, n
-                                },
-                                remove: function(r) {
-                                    r = this.root + r;
-                                    var e = this.files[r];
-                                    if (e || ("/" !== r.slice(-1) && (r += "/"), e = this.files[r]), e && !e.dir) delete this.files[r];
-                                    else
-                                        for (var t = this.filter(function(e, t) {
-                                                return t.name.slice(0, r.length) === r
-                                            }), n = 0; n < t.length; n++) delete this.files[t[n].name];
-                                    return this
-                                },
-                                generate: function() {
-                                    throw new Error("This method has been removed in JSZip 3.0, please check the upgrade guide.")
-                                },
-                                generateInternalStream: function(e) {
-                                    var t, r = {};
-                                    try {
-                                        if ((r = u.extend(e || {}, {
-                                                streamFiles: !1,
-                                                compression: "STORE",
-                                                compressionOptions: null,
-                                                type: "",
-                                                platform: "DOS",
-                                                comment: null,
-                                                mimeType: "application/zip",
-                                                encodeFileName: i.utf8encode
-                                            })).type = r.type.toLowerCase(), r.compression = r.compression.toUpperCase(), "binarystring" === r.type && (r.type = "string"), !r.type) throw new Error("No output type specified.");
-                                        u.checkSupport(r.type), "darwin" !== r.platform && "freebsd" !== r.platform && "linux" !== r.platform && "sunos" !== r.platform || (r.platform = "UNIX"), "win32" === r.platform && (r.platform = "DOS");
-                                        var n = r.comment || this.comment || "";
-                                        t = o.generateWorker(this, r, n)
-                                    } catch (e) {
-                                        (t = new l("error")).error(e)
-                                    }
-                                    return new a(t, r.type || "string", r.mimeType)
-                                },
-                                generateAsync: function(e, t) {
-                                    return this.generateInternalStream(e).accumulate(t)
-                                },
-                                generateNodeStream: function(e, t) {
-                                    return (e = e || {}).type || (e.type = "nodebuffer"), this.generateInternalStream(e).toNodejsStream(t)
-                                }
+                    function i(t, e, r, i, a, l) {
+                        var f, c, d = t.file,
+                            p = t.compression,
+                            m = l !== o.utf8encode,
+                            _ = s.transformTo("string", l(d.name)),
+                            g = s.transformTo("string", o.utf8encode(d.name)),
+                            b = d.comment,
+                            v = s.transformTo("string", l(b)),
+                            y = s.transformTo("string", o.utf8encode(b)),
+                            w = g.length !== d.name.length,
+                            k = y.length !== b.length,
+                            x = "",
+                            S = "",
+                            z = "",
+                            C = d.dir,
+                            E = d.date,
+                            A = {
+                                crc32: 0,
+                                compressedSize: 0,
+                                uncompressedSize: 0
                             };
-                            t.exports = n
-                        }, {
-                            "./compressedObject": 2,
-                            "./defaults": 5,
-                            "./generate": 9,
-                            "./nodejs/NodejsStreamInputAdapter": 12,
-                            "./nodejsUtils": 14,
-                            "./stream/GenericWorker": 28,
-                            "./stream/StreamHelper": 29,
-                            "./utf8": 31,
-                            "./utils": 32,
-                            "./zipObject": 35
-                        }],
-                        16: [function(e, t, r) {
-                            "use strict";
-                            t.exports = e("stream")
-                        }, {
-                            stream: void 0
-                        }],
-                        17: [function(e, t, r) {
-                            "use strict";
-                            var n = e("./DataReader");
-
-                            function i(e) {
-                                n.call(this, e);
-                                for (var t = 0; t < this.data.length; t++) e[t] = 255 & e[t]
-                            }
-                            e("../utils").inherits(i, n), i.prototype.byteAt = function(e) {
-                                return this.data[this.zero + e]
-                            }, i.prototype.lastIndexOfSignature = function(e) {
-                                for (var t = e.charCodeAt(0), r = e.charCodeAt(1), n = e.charCodeAt(2), i = e.charCodeAt(3), s = this.length - 4; 0 <= s; --s)
-                                    if (this.data[s] === t && this.data[s + 1] === r && this.data[s + 2] === n && this.data[s + 3] === i) return s - this.zero;
-                                return -1
-                            }, i.prototype.readAndCheckSignature = function(e) {
-                                var t = e.charCodeAt(0),
-                                    r = e.charCodeAt(1),
-                                    n = e.charCodeAt(2),
-                                    i = e.charCodeAt(3),
-                                    s = this.readData(4);
-                                return t === s[0] && r === s[1] && n === s[2] && i === s[3]
-                            }, i.prototype.readData = function(e) {
-                                if (this.checkOffset(e), 0 === e) return [];
-                                var t = this.data.slice(this.zero + this.index, this.zero + this.index + e);
-                                return this.index += e, t
-                            }, t.exports = i
-                        }, {
-                            "../utils": 32,
-                            "./DataReader": 18
-                        }],
-                        18: [function(e, t, r) {
-                            "use strict";
-                            var n = e("../utils");
+                        e && !r || (A.crc32 = t.crc32, A.compressedSize = t.compressedSize, A.uncompressedSize = t.uncompressedSize);
+                        var I = 0;
+                        e && (I |= 8), m || !w && !k || (I |= 2048);
+                        var O = 0,
+                            B = 0;
+                        C && (O |= 16), "UNIX" === a ? (B = 798, O |= function(t, e) {
+                            var r = t;
+                            return t || (r = e ? 16893 : 33204), (65535 & r) << 16
+                        }(d.unixPermissions, C)) : (B = 20, O |= function(t) {
+                            return 63 & (t || 0)
+                        }(d.dosPermissions)), f = E.getUTCHours(), f <<= 6, f |= E.getUTCMinutes(), f <<= 5, f |= E.getUTCSeconds() / 2, c = E.getUTCFullYear() - 1980, c <<= 4, c |= E.getUTCMonth() + 1, c <<= 5, c |= E.getUTCDate(), w && (S = n(1, 1) + n(h(_), 4) + g, x += "up" + n(S.length, 2) + S), k && (z = n(1, 1) + n(h(v), 4) + y, x += "uc" + n(z.length, 2) + z);
+                        var T = "";
+                        return T += "\n\0", T += n(I, 2), T += p.magic, T += n(f, 2), T += n(c, 2), T += n(A.crc32, 4), T += n(A.compressedSize, 4), T += n(A.uncompressedSize, 4), T += n(_.length, 2), T += n(x.length, 2), {
+                            fileRecord: u.LOCAL_FILE_HEADER + T + _ + x,
+                            dirRecord: u.CENTRAL_FILE_HEADER + n(B, 2) + T + n(v.length, 2) + "\0\0\0\0" + n(O, 4) + n(i, 4) + _ + x + v
+                        }
+                    }
+                    var s = t("../utils"),
+                        a = t("../stream/GenericWorker"),
+                        o = t("../utf8"),
+                        h = t("../crc32"),
+                        u = t("../signature");
 
-                            function i(e) {
-                                this.data = e, this.length = e.length, this.index = 0, this.zero = 0
+                    function l(t, e, r, n) {
+                        a.call(this, "ZipFileWorker"), this.bytesWritten = 0, this.zipComment = e, this.zipPlatform = r, this.encodeFileName = n, this.streamFiles = t, this.accumulate = !1, this.contentBuffer = [], this.dirRecords = [], this.currentSourceOffset = 0, this.entriesCount = 0, this.currentFile = null, this._sources = []
+                    }
+                    s.inherits(l, a), l.prototype.push = function(t) {
+                        var e = t.meta.percent || 0,
+                            r = this.entriesCount,
+                            n = this._sources.length;
+                        this.accumulate ? this.contentBuffer.push(t) : (this.bytesWritten += t.data.length, a.prototype.push.call(this, {
+                            data: t.data,
+                            meta: {
+                                currentFile: this.currentFile,
+                                percent: r ? (e + 100 * (r - n - 1)) / r : 100
+                            }
+                        }))
+                    }, l.prototype.openedSource = function(t) {
+                        this.currentSourceOffset = this.bytesWritten, this.currentFile = t.file.name;
+                        var e = this.streamFiles && !t.file.dir;
+                        if (e) {
+                            var r = i(t, e, !1, this.currentSourceOffset, this.zipPlatform, this.encodeFileName);
+                            this.push({
+                                data: r.fileRecord,
+                                meta: {
+                                    percent: 0
+                                }
+                            })
+                        } else this.accumulate = !0
+                    }, l.prototype.closedSource = function(t) {
+                        this.accumulate = !1;
+                        var e = this.streamFiles && !t.file.dir,
+                            r = i(t, e, !0, this.currentSourceOffset, this.zipPlatform, this.encodeFileName);
+                        if (this.dirRecords.push(r.dirRecord), e) this.push({
+                            data: function(t) {
+                                return u.DATA_DESCRIPTOR + n(t.crc32, 4) + n(t.compressedSize, 4) + n(t.uncompressedSize, 4)
+                            }(t),
+                            meta: {
+                                percent: 100
+                            }
+                        });
+                        else
+                            for (this.push({
+                                    data: r.fileRecord,
+                                    meta: {
+                                        percent: 0
+                                    }
+                                }); this.contentBuffer.length;) this.push(this.contentBuffer.shift());
+                        this.currentFile = null
+                    }, l.prototype.flush = function() {
+                        for (var t = this.bytesWritten, e = 0; e < this.dirRecords.length; e++) this.push({
+                            data: this.dirRecords[e],
+                            meta: {
+                                percent: 100
+                            }
+                        });
+                        var r = this.bytesWritten - t,
+                            i = function(t, e, r, i, a) {
+                                var o = s.transformTo("string", a(i));
+                                return u.CENTRAL_DIRECTORY_END + "\0\0\0\0" + n(t, 2) + n(t, 2) + n(e, 4) + n(r, 4) + n(o.length, 2) + o
+                            }(this.dirRecords.length, r, t, this.zipComment, this.encodeFileName);
+                        this.push({
+                            data: i,
+                            meta: {
+                                percent: 100
+                            }
+                        })
+                    }, l.prototype.prepareNextSource = function() {
+                        this.previous = this._sources.shift(), this.openedSource(this.previous.streamInfo), this.isPaused ? this.previous.pause() : this.previous.resume()
+                    }, l.prototype.registerPrevious = function(t) {
+                        this._sources.push(t);
+                        var e = this;
+                        return t.on("data", (function(t) {
+                            e.processChunk(t)
+                        })), t.on("end", (function() {
+                            e.closedSource(e.previous.streamInfo), e._sources.length ? e.prepareNextSource() : e.end()
+                        })), t.on("error", (function(t) {
+                            e.error(t)
+                        })), this
+                    }, l.prototype.resume = function() {
+                        return !!a.prototype.resume.call(this) && (!this.previous && this._sources.length ? (this.prepareNextSource(), !0) : this.previous || this._sources.length || this.generatedError ? void 0 : (this.end(), !0))
+                    }, l.prototype.error = function(t) {
+                        var e = this._sources;
+                        if (!a.prototype.error.call(this, t)) return !1;
+                        for (var r = 0; r < e.length; r++) try {
+                            e[r].error(t)
+                        } catch (t) {}
+                        return !0
+                    }, l.prototype.lock = function() {
+                        a.prototype.lock.call(this);
+                        for (var t = this._sources, e = 0; e < t.length; e++) t[e].lock()
+                    }, e.exports = l
+                }, {
+                    "../crc32": 4,
+                    "../signature": 23,
+                    "../stream/GenericWorker": 28,
+                    "../utf8": 31,
+                    "../utils": 32
+                }],
+                9: [function(t, e, r) {
+                    "use strict";
+                    var n = t("../compressions"),
+                        i = t("./ZipFileWorker");
+                    r.generateWorker = function(t, e, r) {
+                        var s = new i(e.streamFiles, r, e.platform, e.encodeFileName),
+                            a = 0;
+                        try {
+                            t.forEach((function(t, r) {
+                                a++;
+                                var i = function(t, e) {
+                                        var r = t || e,
+                                            i = n[r];
+                                        if (!i) throw new Error(r + " is not a valid compression method !");
+                                        return i
+                                    }(r.options.compression, e.compression),
+                                    o = r.options.compressionOptions || e.compressionOptions || {},
+                                    h = r.dir,
+                                    u = r.date;
+                                r._compressWorker(i, o).withStreamInfo("file", {
+                                    name: t,
+                                    dir: h,
+                                    date: u,
+                                    comment: r.comment || "",
+                                    unixPermissions: r.unixPermissions,
+                                    dosPermissions: r.dosPermissions
+                                }).pipe(s)
+                            })), s.entriesCount = a
+                        } catch (t) {
+                            s.error(t)
+                        }
+                        return s
+                    }
+                }, {
+                    "../compressions": 3,
+                    "./ZipFileWorker": 8
+                }],
+                10: [function(t, e, r) {
+                    "use strict";
+
+                    function n() {
+                        if (!(this instanceof n)) return new n;
+                        if (arguments.length) throw new Error("The constructor with parameters has been removed in JSZip 3.0, please check the upgrade guide.");
+                        this.files = Object.create(null), this.comment = null, this.root = "", this.clone = function() {
+                            var t = new n;
+                            for (var e in this) "function" != typeof this[e] && (t[e] = this[e]);
+                            return t
+                        }
+                    }(n.prototype = t("./object")).loadAsync = t("./load"), n.support = t("./support"), n.defaults = t("./defaults"), n.version = "3.10.1", n.loadAsync = function(t, e) {
+                        return (new n).loadAsync(t, e)
+                    }, n.external = t("./external"), e.exports = n
+                }, {
+                    "./defaults": 5,
+                    "./external": 6,
+                    "./load": 11,
+                    "./object": 15,
+                    "./support": 30
+                }],
+                11: [function(t, e, r) {
+                    "use strict";
+                    var n = t("./utils"),
+                        i = t("./external"),
+                        s = t("./utf8"),
+                        a = t("./zipEntries"),
+                        o = t("./stream/Crc32Probe"),
+                        h = t("./nodejsUtils");
+
+                    function u(t) {
+                        return new i.Promise((function(e, r) {
+                            var n = t.decompressed.getContentWorker().pipe(new o);
+                            n.on("error", (function(t) {
+                                r(t)
+                            })).on("end", (function() {
+                                n.streamInfo.crc32 !== t.decompressed.crc32 ? r(new Error("Corrupted zip : CRC32 mismatch")) : e()
+                            })).resume()
+                        }))
+                    }
+                    e.exports = function(t, e) {
+                        var r = this;
+                        return e = n.extend(e || {}, {
+                            base64: !1,
+                            checkCRC32: !1,
+                            optimizedBinaryString: !1,
+                            createFolders: !1,
+                            decodeFileName: s.utf8decode
+                        }), h.isNode && h.isStream(t) ? i.Promise.reject(new Error("JSZip can't accept a stream when loading a zip file.")) : n.prepareContent("the loaded zip file", t, !0, e.optimizedBinaryString, e.base64).then((function(t) {
+                            var r = new a(e);
+                            return r.load(t), r
+                        })).then((function(t) {
+                            var r = [i.Promise.resolve(t)],
+                                n = t.files;
+                            if (e.checkCRC32)
+                                for (var s = 0; s < n.length; s++) r.push(u(n[s]));
+                            return i.Promise.all(r)
+                        })).then((function(t) {
+                            for (var i = t.shift(), s = i.files, a = 0; a < s.length; a++) {
+                                var o = s[a],
+                                    h = o.fileNameStr,
+                                    u = n.resolve(o.fileNameStr);
+                                r.file(u, o.decompressed, {
+                                    binary: !0,
+                                    optimizedBinaryString: !0,
+                                    date: o.date,
+                                    dir: o.dir,
+                                    comment: o.fileCommentStr.length ? o.fileCommentStr : null,
+                                    unixPermissions: o.unixPermissions,
+                                    dosPermissions: o.dosPermissions,
+                                    createFolders: e.createFolders
+                                }), o.dir || (r.file(u).unsafeOriginalName = h)
                             }
-                            i.prototype = {
-                                checkOffset: function(e) {
-                                    this.checkIndex(this.index + e)
-                                },
-                                checkIndex: function(e) {
-                                    if (this.length < this.zero + e || e < 0) throw new Error("End of data reached (data length = " + this.length + ", asked index = " + e + "). Corrupted zip ?")
-                                },
-                                setIndex: function(e) {
-                                    this.checkIndex(e), this.index = e
-                                },
-                                skip: function(e) {
-                                    this.setIndex(this.index + e)
-                                },
-                                byteAt: function() {},
-                                readInt: function(e) {
-                                    var t, r = 0;
-                                    for (this.checkOffset(e), t = this.index + e - 1; t >= this.index; t--) r = (r << 8) + this.byteAt(t);
-                                    return this.index += e, r
-                                },
-                                readString: function(e) {
-                                    return n.transformTo("string", this.readData(e))
-                                },
-                                readData: function() {},
-                                lastIndexOfSignature: function() {},
-                                readAndCheckSignature: function() {},
-                                readDate: function() {
-                                    var e = this.readInt(4);
-                                    return new Date(Date.UTC(1980 + (e >> 25 & 127), (e >> 21 & 15) - 1, e >> 16 & 31, e >> 11 & 31, e >> 5 & 63, (31 & e) << 1))
-                                }
-                            }, t.exports = i
-                        }, {
-                            "../utils": 32
-                        }],
-                        19: [function(e, t, r) {
-                            "use strict";
-                            var n = e("./Uint8ArrayReader");
+                            return i.zipComment.length && (r.comment = i.zipComment), r
+                        }))
+                    }
+                }, {
+                    "./external": 6,
+                    "./nodejsUtils": 14,
+                    "./stream/Crc32Probe": 25,
+                    "./utf8": 31,
+                    "./utils": 32,
+                    "./zipEntries": 33
+                }],
+                12: [function(t, e, r) {
+                    "use strict";
+                    var n = t("../utils"),
+                        i = t("../stream/GenericWorker");
 
-                            function i(e) {
-                                n.call(this, e)
-                            }
-                            e("../utils").inherits(i, n), i.prototype.readData = function(e) {
-                                this.checkOffset(e);
-                                var t = this.data.slice(this.zero + this.index, this.zero + this.index + e);
-                                return this.index += e, t
-                            }, t.exports = i
-                        }, {
-                            "../utils": 32,
-                            "./Uint8ArrayReader": 21
-                        }],
-                        20: [function(e, t, r) {
-                            "use strict";
-                            var n = e("./DataReader");
+                    function s(t, e) {
+                        i.call(this, "Nodejs stream input adapter for " + t), this._upstreamEnded = !1, this._bindStream(e)
+                    }
+                    n.inherits(s, i), s.prototype._bindStream = function(t) {
+                        var e = this;
+                        (this._stream = t).pause(), t.on("data", (function(t) {
+                            e.push({
+                                data: t,
+                                meta: {
+                                    percent: 0
+                                }
+                            })
+                        })).on("error", (function(t) {
+                            e.isPaused ? this.generatedError = t : e.error(t)
+                        })).on("end", (function() {
+                            e.isPaused ? e._upstreamEnded = !0 : e.end()
+                        }))
+                    }, s.prototype.pause = function() {
+                        return !!i.prototype.pause.call(this) && (this._stream.pause(), !0)
+                    }, s.prototype.resume = function() {
+                        return !!i.prototype.resume.call(this) && (this._upstreamEnded ? this.end() : this._stream.resume(), !0)
+                    }, e.exports = s
+                }, {
+                    "../stream/GenericWorker": 28,
+                    "../utils": 32
+                }],
+                13: [function(t, e, r) {
+                    "use strict";
+                    var n = t("readable-stream").Readable;
+
+                    function i(t, e, r) {
+                        n.call(this, e), this._helper = t;
+                        var i = this;
+                        t.on("data", (function(t, e) {
+                            i.push(t) || i._helper.pause(), r && r(e)
+                        })).on("error", (function(t) {
+                            i.emit("error", t)
+                        })).on("end", (function() {
+                            i.push(null)
+                        }))
+                    }
+                    t("../utils").inherits(i, n), i.prototype._read = function() {
+                        this._helper.resume()
+                    }, e.exports = i
+                }, {
+                    "../utils": 32,
+                    "readable-stream": 16
+                }],
+                14: [function(t, e, r) {
+                    "use strict";
+                    e.exports = {
+                        isNode: "undefined" != typeof Buffer,
+                        newBufferFrom: function(t, e) {
+                            if (Buffer.from && Buffer.from !== Uint8Array.from) return Buffer.from(t, e);
+                            if ("number" == typeof t) throw new Error('The "data" argument must not be a number');
+                            return new Buffer(t, e)
+                        },
+                        allocBuffer: function(t) {
+                            if (Buffer.alloc) return Buffer.alloc(t);
+                            var e = new Buffer(t);
+                            return e.fill(0), e
+                        },
+                        isBuffer: function(t) {
+                            return Buffer.isBuffer(t)
+                        },
+                        isStream: function(t) {
+                            return t && "function" == typeof t.on && "function" == typeof t.pause && "function" == typeof t.resume
+                        }
+                    }
+                }, {}],
+                15: [function(t, e, r) {
+                    "use strict";
+
+                    function n(t, e, r) {
+                        var n, i = s.getTypeOf(e),
+                            o = s.extend(r || {}, h);
+                        o.date = o.date || new Date, null !== o.compression && (o.compression = o.compression.toUpperCase()), "string" == typeof o.unixPermissions && (o.unixPermissions = parseInt(o.unixPermissions, 8)), o.unixPermissions && 16384 & o.unixPermissions && (o.dir = !0), o.dosPermissions && 16 & o.dosPermissions && (o.dir = !0), o.dir && (t = m(t)), o.createFolders && (n = p(t)) && _.call(this, n, !0);
+                        var f = "string" === i && !1 === o.binary && !1 === o.base64;
+                        r && void 0 !== r.binary || (o.binary = !f), (e instanceof u && 0 === e.uncompressedSize || o.dir || !e || 0 === e.length) && (o.base64 = !1, o.binary = !0, e = "", o.compression = "STORE", i = "string");
+                        var g;
+                        g = e instanceof u || e instanceof a ? e : c.isNode && c.isStream(e) ? new d(t, e) : s.prepareContent(t, e, o.binary, o.optimizedBinaryString, o.base64);
+                        var b = new l(t, g, o);
+                        this.files[t] = b
+                    }
+                    var i = t("./utf8"),
+                        s = t("./utils"),
+                        a = t("./stream/GenericWorker"),
+                        o = t("./stream/StreamHelper"),
+                        h = t("./defaults"),
+                        u = t("./compressedObject"),
+                        l = t("./zipObject"),
+                        f = t("./generate"),
+                        c = t("./nodejsUtils"),
+                        d = t("./nodejs/NodejsStreamInputAdapter"),
+                        p = function(t) {
+                            "/" === t.slice(-1) && (t = t.substring(0, t.length - 1));
+                            var e = t.lastIndexOf("/");
+                            return 0 < e ? t.substring(0, e) : ""
+                        },
+                        m = function(t) {
+                            return "/" !== t.slice(-1) && (t += "/"), t
+                        },
+                        _ = function(t, e) {
+                            return e = void 0 !== e ? e : h.createFolders, t = m(t), this.files[t] || n.call(this, t, null, {
+                                dir: !0,
+                                createFolders: e
+                            }), this.files[t]
+                        };
 
-                            function i(e) {
-                                n.call(this, e)
+                    function g(t) {
+                        return "[object RegExp]" === Object.prototype.toString.call(t)
+                    }
+                    var b = {
+                        load: function() {
+                            throw new Error("This method has been removed in JSZip 3.0, please check the upgrade guide.")
+                        },
+                        forEach: function(t) {
+                            var e, r, n;
+                            for (e in this.files) n = this.files[e], (r = e.slice(this.root.length, e.length)) && e.slice(0, this.root.length) === this.root && t(r, n)
+                        },
+                        filter: function(t) {
+                            var e = [];
+                            return this.forEach((function(r, n) {
+                                t(r, n) && e.push(n)
+                            })), e
+                        },
+                        file: function(t, e, r) {
+                            if (1 !== arguments.length) return t = this.root + t, n.call(this, t, e, r), this;
+                            if (g(t)) {
+                                var i = t;
+                                return this.filter((function(t, e) {
+                                    return !e.dir && i.test(t)
+                                }))
                             }
-                            e("../utils").inherits(i, n), i.prototype.byteAt = function(e) {
-                                return this.data.charCodeAt(this.zero + e)
-                            }, i.prototype.lastIndexOfSignature = function(e) {
-                                return this.data.lastIndexOf(e) - this.zero
-                            }, i.prototype.readAndCheckSignature = function(e) {
-                                return e === this.readData(4)
-                            }, i.prototype.readData = function(e) {
-                                this.checkOffset(e);
-                                var t = this.data.slice(this.zero + this.index, this.zero + this.index + e);
-                                return this.index += e, t
-                            }, t.exports = i
-                        }, {
-                            "../utils": 32,
-                            "./DataReader": 18
-                        }],
-                        21: [function(e, t, r) {
-                            "use strict";
-                            var n = e("./ArrayReader");
+                            var s = this.files[this.root + t];
+                            return s && !s.dir ? s : null
+                        },
+                        folder: function(t) {
+                            if (!t) return this;
+                            if (g(t)) return this.filter((function(e, r) {
+                                return r.dir && t.test(e)
+                            }));
+                            var e = this.root + t,
+                                r = _.call(this, e),
+                                n = this.clone();
+                            return n.root = r.name, n
+                        },
+                        remove: function(t) {
+                            t = this.root + t;
+                            var e = this.files[t];
+                            if (e || ("/" !== t.slice(-1) && (t += "/"), e = this.files[t]), e && !e.dir) delete this.files[t];
+                            else
+                                for (var r = this.filter((function(e, r) {
+                                        return r.name.slice(0, t.length) === t
+                                    })), n = 0; n < r.length; n++) delete this.files[r[n].name];
+                            return this
+                        },
+                        generate: function() {
+                            throw new Error("This method has been removed in JSZip 3.0, please check the upgrade guide.")
+                        },
+                        generateInternalStream: function(t) {
+                            var e, r = {};
+                            try {
+                                if ((r = s.extend(t || {}, {
+                                        streamFiles: !1,
+                                        compression: "STORE",
+                                        compressionOptions: null,
+                                        type: "",
+                                        platform: "DOS",
+                                        comment: null,
+                                        mimeType: "application/zip",
+                                        encodeFileName: i.utf8encode
+                                    })).type = r.type.toLowerCase(), r.compression = r.compression.toUpperCase(), "binarystring" === r.type && (r.type = "string"), !r.type) throw new Error("No output type specified.");
+                                s.checkSupport(r.type), "darwin" !== r.platform && "freebsd" !== r.platform && "linux" !== r.platform && "sunos" !== r.platform || (r.platform = "UNIX"), "win32" === r.platform && (r.platform = "DOS");
+                                var n = r.comment || this.comment || "";
+                                e = f.generateWorker(this, r, n)
+                            } catch (t) {
+                                (e = new a("error")).error(t)
+                            }
+                            return new o(e, r.type || "string", r.mimeType)
+                        },
+                        generateAsync: function(t, e) {
+                            return this.generateInternalStream(t).accumulate(e)
+                        },
+                        generateNodeStream: function(t, e) {
+                            return (t = t || {}).type || (t.type = "nodebuffer"), this.generateInternalStream(t).toNodejsStream(e)
+                        }
+                    };
+                    e.exports = b
+                }, {
+                    "./compressedObject": 2,
+                    "./defaults": 5,
+                    "./generate": 9,
+                    "./nodejs/NodejsStreamInputAdapter": 12,
+                    "./nodejsUtils": 14,
+                    "./stream/GenericWorker": 28,
+                    "./stream/StreamHelper": 29,
+                    "./utf8": 31,
+                    "./utils": 32,
+                    "./zipObject": 35
+                }],
+                16: [function(t, e, r) {
+                    "use strict";
+                    e.exports = t("stream")
+                }, {
+                    stream: void 0
+                }],
+                17: [function(t, e, r) {
+                    "use strict";
+                    var n = t("./DataReader");
+
+                    function i(t) {
+                        n.call(this, t);
+                        for (var e = 0; e < this.data.length; e++) t[e] = 255 & t[e]
+                    }
+                    t("../utils").inherits(i, n), i.prototype.byteAt = function(t) {
+                        return this.data[this.zero + t]
+                    }, i.prototype.lastIndexOfSignature = function(t) {
+                        for (var e = t.charCodeAt(0), r = t.charCodeAt(1), n = t.charCodeAt(2), i = t.charCodeAt(3), s = this.length - 4; 0 <= s; --s)
+                            if (this.data[s] === e && this.data[s + 1] === r && this.data[s + 2] === n && this.data[s + 3] === i) return s - this.zero;
+                        return -1
+                    }, i.prototype.readAndCheckSignature = function(t) {
+                        var e = t.charCodeAt(0),
+                            r = t.charCodeAt(1),
+                            n = t.charCodeAt(2),
+                            i = t.charCodeAt(3),
+                            s = this.readData(4);
+                        return e === s[0] && r === s[1] && n === s[2] && i === s[3]
+                    }, i.prototype.readData = function(t) {
+                        if (this.checkOffset(t), 0 === t) return [];
+                        var e = this.data.slice(this.zero + this.index, this.zero + this.index + t);
+                        return this.index += t, e
+                    }, e.exports = i
+                }, {
+                    "../utils": 32,
+                    "./DataReader": 18
+                }],
+                18: [function(t, e, r) {
+                    "use strict";
+                    var n = t("../utils");
 
-                            function i(e) {
-                                n.call(this, e)
-                            }
-                            e("../utils").inherits(i, n), i.prototype.readData = function(e) {
-                                if (this.checkOffset(e), 0 === e) return new Uint8Array(0);
-                                var t = this.data.subarray(this.zero + this.index, this.zero + this.index + e);
-                                return this.index += e, t
-                            }, t.exports = i
-                        }, {
-                            "../utils": 32,
-                            "./ArrayReader": 17
-                        }],
-                        22: [function(e, t, r) {
-                            "use strict";
-                            var n = e("../utils"),
-                                i = e("../support"),
-                                s = e("./ArrayReader"),
-                                a = e("./StringReader"),
-                                o = e("./NodeBufferReader"),
-                                h = e("./Uint8ArrayReader");
-                            t.exports = function(e) {
-                                var t = n.getTypeOf(e);
-                                return n.checkSupport(t), "string" !== t || i.uint8array ? "nodebuffer" === t ? new o(e) : i.uint8array ? new h(n.transformTo("uint8array", e)) : new s(n.transformTo("array", e)) : new a(e)
-                            }
-                        }, {
-                            "../support": 30,
-                            "../utils": 32,
-                            "./ArrayReader": 17,
-                            "./NodeBufferReader": 19,
-                            "./StringReader": 20,
-                            "./Uint8ArrayReader": 21
-                        }],
-                        23: [function(e, t, r) {
-                            "use strict";
-                            r.LOCAL_FILE_HEADER = "PK", r.CENTRAL_FILE_HEADER = "PK", r.CENTRAL_DIRECTORY_END = "PK", r.ZIP64_CENTRAL_DIRECTORY_LOCATOR = "PK", r.ZIP64_CENTRAL_DIRECTORY_END = "PK", r.DATA_DESCRIPTOR = "PK\b"
-                        }, {}],
-                        24: [function(e, t, r) {
-                            "use strict";
-                            var n = e("./GenericWorker"),
-                                i = e("../utils");
+                    function i(t) {
+                        this.data = t, this.length = t.length, this.index = 0, this.zero = 0
+                    }
+                    i.prototype = {
+                        checkOffset: function(t) {
+                            this.checkIndex(this.index + t)
+                        },
+                        checkIndex: function(t) {
+                            if (this.length < this.zero + t || t < 0) throw new Error("End of data reached (data length = " + this.length + ", asked index = " + t + "). Corrupted zip ?")
+                        },
+                        setIndex: function(t) {
+                            this.checkIndex(t), this.index = t
+                        },
+                        skip: function(t) {
+                            this.setIndex(this.index + t)
+                        },
+                        byteAt: function() {},
+                        readInt: function(t) {
+                            var e, r = 0;
+                            for (this.checkOffset(t), e = this.index + t - 1; e >= this.index; e--) r = (r << 8) + this.byteAt(e);
+                            return this.index += t, r
+                        },
+                        readString: function(t) {
+                            return n.transformTo("string", this.readData(t))
+                        },
+                        readData: function() {},
+                        lastIndexOfSignature: function() {},
+                        readAndCheckSignature: function() {},
+                        readDate: function() {
+                            var t = this.readInt(4);
+                            return new Date(Date.UTC(1980 + (t >> 25 & 127), (t >> 21 & 15) - 1, t >> 16 & 31, t >> 11 & 31, t >> 5 & 63, (31 & t) << 1))
+                        }
+                    }, e.exports = i
+                }, {
+                    "../utils": 32
+                }],
+                19: [function(t, e, r) {
+                    "use strict";
+                    var n = t("./Uint8ArrayReader");
 
-                            function s(e) {
-                                n.call(this, "ConvertWorker to " + e), this.destType = e
-                            }
-                            i.inherits(s, n), s.prototype.processChunk = function(e) {
-                                this.push({
-                                    data: i.transformTo(this.destType, e.data),
-                                    meta: e.meta
-                                })
-                            }, t.exports = s
-                        }, {
-                            "../utils": 32,
-                            "./GenericWorker": 28
-                        }],
-                        25: [function(e, t, r) {
-                            "use strict";
-                            var n = e("./GenericWorker"),
-                                i = e("../crc32");
+                    function i(t) {
+                        n.call(this, t)
+                    }
+                    t("../utils").inherits(i, n), i.prototype.readData = function(t) {
+                        this.checkOffset(t);
+                        var e = this.data.slice(this.zero + this.index, this.zero + this.index + t);
+                        return this.index += t, e
+                    }, e.exports = i
+                }, {
+                    "../utils": 32,
+                    "./Uint8ArrayReader": 21
+                }],
+                20: [function(t, e, r) {
+                    "use strict";
+                    var n = t("./DataReader");
 
-                            function s() {
-                                n.call(this, "Crc32Probe"), this.withStreamInfo("crc32", 0)
-                            }
-                            e("../utils").inherits(s, n), s.prototype.processChunk = function(e) {
-                                this.streamInfo.crc32 = i(e.data, this.streamInfo.crc32 || 0), this.push(e)
-                            }, t.exports = s
-                        }, {
-                            "../crc32": 4,
-                            "../utils": 32,
-                            "./GenericWorker": 28
-                        }],
-                        26: [function(e, t, r) {
-                            "use strict";
-                            var n = e("../utils"),
-                                i = e("./GenericWorker");
+                    function i(t) {
+                        n.call(this, t)
+                    }
+                    t("../utils").inherits(i, n), i.prototype.byteAt = function(t) {
+                        return this.data.charCodeAt(this.zero + t)
+                    }, i.prototype.lastIndexOfSignature = function(t) {
+                        return this.data.lastIndexOf(t) - this.zero
+                    }, i.prototype.readAndCheckSignature = function(t) {
+                        return t === this.readData(4)
+                    }, i.prototype.readData = function(t) {
+                        this.checkOffset(t);
+                        var e = this.data.slice(this.zero + this.index, this.zero + this.index + t);
+                        return this.index += t, e
+                    }, e.exports = i
+                }, {
+                    "../utils": 32,
+                    "./DataReader": 18
+                }],
+                21: [function(t, e, r) {
+                    "use strict";
+                    var n = t("./ArrayReader");
 
-                            function s(e) {
-                                i.call(this, "DataLengthProbe for " + e), this.propName = e, this.withStreamInfo(e, 0)
-                            }
-                            n.inherits(s, i), s.prototype.processChunk = function(e) {
-                                if (e) {
-                                    var t = this.streamInfo[this.propName] || 0;
-                                    this.streamInfo[this.propName] = t + e.data.length
-                                }
-                                i.prototype.processChunk.call(this, e)
-                            }, t.exports = s
-                        }, {
-                            "../utils": 32,
-                            "./GenericWorker": 28
-                        }],
-                        27: [function(e, t, r) {
-                            "use strict";
-                            var n = e("../utils"),
-                                i = e("./GenericWorker");
+                    function i(t) {
+                        n.call(this, t)
+                    }
+                    t("../utils").inherits(i, n), i.prototype.readData = function(t) {
+                        if (this.checkOffset(t), 0 === t) return new Uint8Array(0);
+                        var e = this.data.subarray(this.zero + this.index, this.zero + this.index + t);
+                        return this.index += t, e
+                    }, e.exports = i
+                }, {
+                    "../utils": 32,
+                    "./ArrayReader": 17
+                }],
+                22: [function(t, e, r) {
+                    "use strict";
+                    var n = t("../utils"),
+                        i = t("../support"),
+                        s = t("./ArrayReader"),
+                        a = t("./StringReader"),
+                        o = t("./NodeBufferReader"),
+                        h = t("./Uint8ArrayReader");
+                    e.exports = function(t) {
+                        var e = n.getTypeOf(t);
+                        return n.checkSupport(e), "string" !== e || i.uint8array ? "nodebuffer" === e ? new o(t) : i.uint8array ? new h(n.transformTo("uint8array", t)) : new s(n.transformTo("array", t)) : new a(t)
+                    }
+                }, {
+                    "../support": 30,
+                    "../utils": 32,
+                    "./ArrayReader": 17,
+                    "./NodeBufferReader": 19,
+                    "./StringReader": 20,
+                    "./Uint8ArrayReader": 21
+                }],
+                23: [function(t, e, r) {
+                    "use strict";
+                    r.LOCAL_FILE_HEADER = "PK", r.CENTRAL_FILE_HEADER = "PK", r.CENTRAL_DIRECTORY_END = "PK", r.ZIP64_CENTRAL_DIRECTORY_LOCATOR = "PK", r.ZIP64_CENTRAL_DIRECTORY_END = "PK", r.DATA_DESCRIPTOR = "PK\b"
+                }, {}],
+                24: [function(t, e, r) {
+                    "use strict";
+                    var n = t("./GenericWorker"),
+                        i = t("../utils");
 
-                            function s(e) {
-                                i.call(this, "DataWorker");
-                                var t = this;
-                                this.dataIsReady = !1, this.index = 0, this.max = 0, this.data = null, this.type = "", this._tickScheduled = !1, e.then(function(e) {
-                                    t.dataIsReady = !0, t.data = e, t.max = e && e.length || 0, t.type = n.getTypeOf(e), t.isPaused || t._tickAndRepeat()
-                                }, function(e) {
-                                    t.error(e)
-                                })
-                            }
-                            n.inherits(s, i), s.prototype.cleanUp = function() {
-                                i.prototype.cleanUp.call(this), this.data = null
-                            }, s.prototype.resume = function() {
-                                return !!i.prototype.resume.call(this) && (!this._tickScheduled && this.dataIsReady && (this._tickScheduled = !0, n.delay(this._tickAndRepeat, [], this)), !0)
-                            }, s.prototype._tickAndRepeat = function() {
-                                this._tickScheduled = !1, this.isPaused || this.isFinished || (this._tick(), this.isFinished || (n.delay(this._tickAndRepeat, [], this), this._tickScheduled = !0))
-                            }, s.prototype._tick = function() {
-                                if (this.isPaused || this.isFinished) return !1;
-                                var e = null,
-                                    t = Math.min(this.max, this.index + 16384);
-                                if (this.index >= this.max) return this.end();
-                                switch (this.type) {
-                                    case "string":
-                                        e = this.data.substring(this.index, t);
-                                        break;
-                                    case "uint8array":
-                                        e = this.data.subarray(this.index, t);
-                                        break;
-                                    case "array":
-                                    case "nodebuffer":
-                                        e = this.data.slice(this.index, t)
-                                }
-                                return this.index = t, this.push({
-                                    data: e,
-                                    meta: {
-                                        percent: this.max ? this.index / this.max * 100 : 0
-                                    }
-                                })
-                            }, t.exports = s
-                        }, {
-                            "../utils": 32,
-                            "./GenericWorker": 28
-                        }],
-                        28: [function(e, t, r) {
-                            "use strict";
+                    function s(t) {
+                        n.call(this, "ConvertWorker to " + t), this.destType = t
+                    }
+                    i.inherits(s, n), s.prototype.processChunk = function(t) {
+                        this.push({
+                            data: i.transformTo(this.destType, t.data),
+                            meta: t.meta
+                        })
+                    }, e.exports = s
+                }, {
+                    "../utils": 32,
+                    "./GenericWorker": 28
+                }],
+                25: [function(t, e, r) {
+                    "use strict";
+                    var n = t("./GenericWorker"),
+                        i = t("../crc32");
 
-                            function n(e) {
-                                this.name = e || "default", this.streamInfo = {}, this.generatedError = null, this.extraStreamInfo = {}, this.isPaused = !0, this.isFinished = !1, this.isLocked = !1, this._listeners = {
-                                    data: [],
-                                    end: [],
-                                    error: []
-                                }, this.previous = null
-                            }
-                            n.prototype = {
-                                push: function(e) {
-                                    this.emit("data", e)
-                                },
-                                end: function() {
-                                    if (this.isFinished) return !1;
-                                    this.flush();
-                                    try {
-                                        this.emit("end"), this.cleanUp(), this.isFinished = !0
-                                    } catch (e) {
-                                        this.emit("error", e)
-                                    }
-                                    return !0
-                                },
-                                error: function(e) {
-                                    return !this.isFinished && (this.isPaused ? this.generatedError = e : (this.isFinished = !0, this.emit("error", e), this.previous && this.previous.error(e), this.cleanUp()), !0)
-                                },
-                                on: function(e, t) {
-                                    return this._listeners[e].push(t), this
-                                },
-                                cleanUp: function() {
-                                    this.streamInfo = this.generatedError = this.extraStreamInfo = null, this._listeners = []
-                                },
-                                emit: function(e, t) {
-                                    if (this._listeners[e])
-                                        for (var r = 0; r < this._listeners[e].length; r++) this._listeners[e][r].call(this, t)
-                                },
-                                pipe: function(e) {
-                                    return e.registerPrevious(this)
-                                },
-                                registerPrevious: function(e) {
-                                    if (this.isLocked) throw new Error("The stream '" + this + "' has already been used.");
-                                    this.streamInfo = e.streamInfo, this.mergeStreamInfo(), this.previous = e;
-                                    var t = this;
-                                    return e.on("data", function(e) {
-                                        t.processChunk(e)
-                                    }), e.on("end", function() {
-                                        t.end()
-                                    }), e.on("error", function(e) {
-                                        t.error(e)
-                                    }), this
-                                },
-                                pause: function() {
-                                    return !this.isPaused && !this.isFinished && (this.isPaused = !0, this.previous && this.previous.pause(), !0)
-                                },
-                                resume: function() {
-                                    if (!this.isPaused || this.isFinished) return !1;
-                                    var e = this.isPaused = !1;
-                                    return this.generatedError && (this.error(this.generatedError), e = !0), this.previous && this.previous.resume(), !e
-                                },
-                                flush: function() {},
-                                processChunk: function(e) {
-                                    this.push(e)
-                                },
-                                withStreamInfo: function(e, t) {
-                                    return this.extraStreamInfo[e] = t, this.mergeStreamInfo(), this
-                                },
-                                mergeStreamInfo: function() {
-                                    for (var e in this.extraStreamInfo) Object.prototype.hasOwnProperty.call(this.extraStreamInfo, e) && (this.streamInfo[e] = this.extraStreamInfo[e])
-                                },
-                                lock: function() {
-                                    if (this.isLocked) throw new Error("The stream '" + this + "' has already been used.");
-                                    this.isLocked = !0, this.previous && this.previous.lock()
-                                },
-                                toString: function() {
-                                    var e = "Worker " + this.name;
-                                    return this.previous ? this.previous + " -> " + e : e
-                                }
-                            }, t.exports = n
-                        }, {}],
-                        29: [function(e, t, r) {
-                            "use strict";
-                            var h = e("../utils"),
-                                i = e("./ConvertWorker"),
-                                s = e("./GenericWorker"),
-                                u = e("../base64"),
-                                n = e("../support"),
-                                a = e("../external"),
-                                o = null;
-                            if (n.nodestream) try {
-                                o = e("../nodejs/NodejsStreamOutputAdapter")
-                            } catch (e) {}
-
-                            function l(e, o) {
-                                return new a.Promise(function(t, r) {
-                                    var n = [],
-                                        i = e._internalType,
-                                        s = e._outputType,
-                                        a = e._mimeType;
-                                    e.on("data", function(e, t) {
-                                        n.push(e), o && o(t)
-                                    }).on("error", function(e) {
-                                        n = [], r(e)
-                                    }).on("end", function() {
+                    function s() {
+                        n.call(this, "Crc32Probe"), this.withStreamInfo("crc32", 0)
+                    }
+                    t("../utils").inherits(s, n), s.prototype.processChunk = function(t) {
+                        this.streamInfo.crc32 = i(t.data, this.streamInfo.crc32 || 0), this.push(t)
+                    }, e.exports = s
+                }, {
+                    "../crc32": 4,
+                    "../utils": 32,
+                    "./GenericWorker": 28
+                }],
+                26: [function(t, e, r) {
+                    "use strict";
+                    var n = t("../utils"),
+                        i = t("./GenericWorker");
+
+                    function s(t) {
+                        i.call(this, "DataLengthProbe for " + t), this.propName = t, this.withStreamInfo(t, 0)
+                    }
+                    n.inherits(s, i), s.prototype.processChunk = function(t) {
+                        if (t) {
+                            var e = this.streamInfo[this.propName] || 0;
+                            this.streamInfo[this.propName] = e + t.data.length
+                        }
+                        i.prototype.processChunk.call(this, t)
+                    }, e.exports = s
+                }, {
+                    "../utils": 32,
+                    "./GenericWorker": 28
+                }],
+                27: [function(t, e, r) {
+                    "use strict";
+                    var n = t("../utils"),
+                        i = t("./GenericWorker");
+
+                    function s(t) {
+                        i.call(this, "DataWorker");
+                        var e = this;
+                        this.dataIsReady = !1, this.index = 0, this.max = 0, this.data = null, this.type = "", this._tickScheduled = !1, t.then((function(t) {
+                            e.dataIsReady = !0, e.data = t, e.max = t && t.length || 0, e.type = n.getTypeOf(t), e.isPaused || e._tickAndRepeat()
+                        }), (function(t) {
+                            e.error(t)
+                        }))
+                    }
+                    n.inherits(s, i), s.prototype.cleanUp = function() {
+                        i.prototype.cleanUp.call(this), this.data = null
+                    }, s.prototype.resume = function() {
+                        return !!i.prototype.resume.call(this) && (!this._tickScheduled && this.dataIsReady && (this._tickScheduled = !0, n.delay(this._tickAndRepeat, [], this)), !0)
+                    }, s.prototype._tickAndRepeat = function() {
+                        this._tickScheduled = !1, this.isPaused || this.isFinished || (this._tick(), this.isFinished || (n.delay(this._tickAndRepeat, [], this), this._tickScheduled = !0))
+                    }, s.prototype._tick = function() {
+                        if (this.isPaused || this.isFinished) return !1;
+                        var t = null,
+                            e = Math.min(this.max, this.index + 16384);
+                        if (this.index >= this.max) return this.end();
+                        switch (this.type) {
+                            case "string":
+                                t = this.data.substring(this.index, e);
+                                break;
+                            case "uint8array":
+                                t = this.data.subarray(this.index, e);
+                                break;
+                            case "array":
+                            case "nodebuffer":
+                                t = this.data.slice(this.index, e)
+                        }
+                        return this.index = e, this.push({
+                            data: t,
+                            meta: {
+                                percent: this.max ? this.index / this.max * 100 : 0
+                            }
+                        })
+                    }, e.exports = s
+                }, {
+                    "../utils": 32,
+                    "./GenericWorker": 28
+                }],
+                28: [function(t, e, r) {
+                    "use strict";
+
+                    function n(t) {
+                        this.name = t || "default", this.streamInfo = {}, this.generatedError = null, this.extraStreamInfo = {}, this.isPaused = !0, this.isFinished = !1, this.isLocked = !1, this._listeners = {
+                            data: [],
+                            end: [],
+                            error: []
+                        }, this.previous = null
+                    }
+                    n.prototype = {
+                        push: function(t) {
+                            this.emit("data", t)
+                        },
+                        end: function() {
+                            if (this.isFinished) return !1;
+                            this.flush();
+                            try {
+                                this.emit("end"), this.cleanUp(), this.isFinished = !0
+                            } catch (t) {
+                                this.emit("error", t)
+                            }
+                            return !0
+                        },
+                        error: function(t) {
+                            return !this.isFinished && (this.isPaused ? this.generatedError = t : (this.isFinished = !0, this.emit("error", t), this.previous && this.previous.error(t), this.cleanUp()), !0)
+                        },
+                        on: function(t, e) {
+                            return this._listeners[t].push(e), this
+                        },
+                        cleanUp: function() {
+                            this.streamInfo = this.generatedError = this.extraStreamInfo = null, this._listeners = []
+                        },
+                        emit: function(t, e) {
+                            if (this._listeners[t])
+                                for (var r = 0; r < this._listeners[t].length; r++) this._listeners[t][r].call(this, e)
+                        },
+                        pipe: function(t) {
+                            return t.registerPrevious(this)
+                        },
+                        registerPrevious: function(t) {
+                            if (this.isLocked) throw new Error("The stream '" + this + "' has already been used.");
+                            this.streamInfo = t.streamInfo, this.mergeStreamInfo(), this.previous = t;
+                            var e = this;
+                            return t.on("data", (function(t) {
+                                e.processChunk(t)
+                            })), t.on("end", (function() {
+                                e.end()
+                            })), t.on("error", (function(t) {
+                                e.error(t)
+                            })), this
+                        },
+                        pause: function() {
+                            return !this.isPaused && !this.isFinished && (this.isPaused = !0, this.previous && this.previous.pause(), !0)
+                        },
+                        resume: function() {
+                            if (!this.isPaused || this.isFinished) return !1;
+                            var t = this.isPaused = !1;
+                            return this.generatedError && (this.error(this.generatedError), t = !0), this.previous && this.previous.resume(), !t
+                        },
+                        flush: function() {},
+                        processChunk: function(t) {
+                            this.push(t)
+                        },
+                        withStreamInfo: function(t, e) {
+                            return this.extraStreamInfo[t] = e, this.mergeStreamInfo(), this
+                        },
+                        mergeStreamInfo: function() {
+                            for (var t in this.extraStreamInfo) Object.prototype.hasOwnProperty.call(this.extraStreamInfo, t) && (this.streamInfo[t] = this.extraStreamInfo[t])
+                        },
+                        lock: function() {
+                            if (this.isLocked) throw new Error("The stream '" + this + "' has already been used.");
+                            this.isLocked = !0, this.previous && this.previous.lock()
+                        },
+                        toString: function() {
+                            var t = "Worker " + this.name;
+                            return this.previous ? this.previous + " -> " + t : t
+                        }
+                    }, e.exports = n
+                }, {}],
+                29: [function(t, e, r) {
+                    "use strict";
+                    var n = t("../utils"),
+                        i = t("./ConvertWorker"),
+                        s = t("./GenericWorker"),
+                        a = t("../base64"),
+                        o = t("../support"),
+                        h = t("../external"),
+                        u = null;
+                    if (o.nodestream) try {
+                        u = t("../nodejs/NodejsStreamOutputAdapter")
+                    } catch (t) {}
+
+                    function l(t, e, r) {
+                        var a = e;
+                        switch (e) {
+                            case "blob":
+                            case "arraybuffer":
+                                a = "uint8array";
+                                break;
+                            case "base64":
+                                a = "string"
+                        }
+                        try {
+                            this._internalType = a, this._outputType = e, this._mimeType = r, n.checkSupport(a), this._worker = t.pipe(new i(a)), t.lock()
+                        } catch (t) {
+                            this._worker = new s("error"), this._worker.error(t)
+                        }
+                    }
+                    l.prototype = {
+                        accumulate: function(t) {
+                            return function(t, e) {
+                                return new h.Promise((function(r, i) {
+                                    var s = [],
+                                        o = t._internalType,
+                                        h = t._outputType,
+                                        u = t._mimeType;
+                                    t.on("data", (function(t, r) {
+                                        s.push(t), e && e(r)
+                                    })).on("error", (function(t) {
+                                        s = [], i(t)
+                                    })).on("end", (function() {
                                         try {
-                                            var e = function(e, t, r) {
-                                                switch (e) {
+                                            var t = function(t, e, r) {
+                                                switch (t) {
                                                     case "blob":
-                                                        return h.newBlob(h.transformTo("arraybuffer", t), r);
+                                                        return n.newBlob(n.transformTo("arraybuffer", e), r);
                                                     case "base64":
-                                                        return u.encode(t);
+                                                        return a.encode(e);
                                                     default:
-                                                        return h.transformTo(e, t)
+                                                        return n.transformTo(t, e)
                                                 }
-                                            }(s, function(e, t) {
+                                            }(h, function(t, e) {
                                                 var r, n = 0,
                                                     i = null,
                                                     s = 0;
-                                                for (r = 0; r < t.length; r++) s += t[r].length;
-                                                switch (e) {
+                                                for (r = 0; r < e.length; r++) s += e[r].length;
+                                                switch (t) {
                                                     case "string":
-                                                        return t.join("");
+                                                        return e.join("");
                                                     case "array":
-                                                        return Array.prototype.concat.apply([], t);
+                                                        return Array.prototype.concat.apply([], e);
                                                     case "uint8array":
-                                                        for (i = new Uint8Array(s), r = 0; r < t.length; r++) i.set(t[r], n), n += t[r].length;
+                                                        for (i = new Uint8Array(s), r = 0; r < e.length; r++) i.set(e[r], n), n += e[r].length;
                                                         return i;
                                                     case "nodebuffer":
-                                                        return Buffer.concat(t);
+                                                        return Buffer.concat(e);
                                                     default:
-                                                        throw new Error("concat : unsupported type '" + e + "'")
+                                                        throw new Error("concat : unsupported type '" + t + "'")
                                                 }
-                                            }(i, n), a);
-                                            t(e)
-                                        } catch (e) {
-                                            r(e)
+                                            }(o, s), u);
+                                            r(t)
+                                        } catch (t) {
+                                            i(t)
                                         }
-                                        n = []
-                                    }).resume()
-                                })
+                                        s = []
+                                    })).resume()
+                                }))
+                            }(this, t)
+                        },
+                        on: function(t, e) {
+                            var r = this;
+                            return "data" === t ? this._worker.on(t, (function(t) {
+                                e.call(r, t.data, t.meta)
+                            })) : this._worker.on(t, (function() {
+                                n.delay(e, arguments, r)
+                            })), this
+                        },
+                        resume: function() {
+                            return n.delay(this._worker.resume, [], this._worker), this
+                        },
+                        pause: function() {
+                            return this._worker.pause(), this
+                        },
+                        toNodejsStream: function(t) {
+                            if (n.checkSupport("nodestream"), "nodebuffer" !== this._outputType) throw new Error(this._outputType + " is not supported by this method");
+                            return new u(this, {
+                                objectMode: "nodebuffer" !== this._outputType
+                            }, t)
+                        }
+                    }, e.exports = l
+                }, {
+                    "../base64": 1,
+                    "../external": 6,
+                    "../nodejs/NodejsStreamOutputAdapter": 13,
+                    "../support": 30,
+                    "../utils": 32,
+                    "./ConvertWorker": 24,
+                    "./GenericWorker": 28
+                }],
+                30: [function(t, e, r) {
+                    "use strict";
+                    if (r.base64 = !0, r.array = !0, r.string = !0, r.arraybuffer = "undefined" != typeof ArrayBuffer && "undefined" != typeof Uint8Array, r.nodebuffer = "undefined" != typeof Buffer, r.uint8array = "undefined" != typeof Uint8Array, "undefined" == typeof ArrayBuffer) r.blob = !1;
+                    else {
+                        var n = new ArrayBuffer(0);
+                        try {
+                            r.blob = 0 === new Blob([n], {
+                                type: "application/zip"
+                            }).size
+                        } catch (t) {
+                            try {
+                                var i = new(self.BlobBuilder || self.WebKitBlobBuilder || self.MozBlobBuilder || self.MSBlobBuilder);
+                                i.append(n), r.blob = 0 === i.getBlob("application/zip").size
+                            } catch (t) {
+                                r.blob = !1
+                            }
+                        }
+                    }
+                    try {
+                        r.nodestream = !!t("readable-stream").Readable
+                    } catch (t) {
+                        r.nodestream = !1
+                    }
+                }, {
+                    "readable-stream": 16
+                }],
+                31: [function(t, e, r) {
+                    "use strict";
+                    for (var n = t("./utils"), i = t("./support"), s = t("./nodejsUtils"), a = t("./stream/GenericWorker"), o = new Array(256), h = 0; h < 256; h++) o[h] = 252 <= h ? 6 : 248 <= h ? 5 : 240 <= h ? 4 : 224 <= h ? 3 : 192 <= h ? 2 : 1;
+
+                    function u() {
+                        a.call(this, "utf-8 decode"), this.leftOver = null
+                    }
+
+                    function l() {
+                        a.call(this, "utf-8 encode")
+                    }
+                    o[254] = o[254] = 1, r.utf8encode = function(t) {
+                        return i.nodebuffer ? s.newBufferFrom(t, "utf-8") : function(t) {
+                            var e, r, n, s, a, o = t.length,
+                                h = 0;
+                            for (s = 0; s < o; s++) 55296 == (64512 & (r = t.charCodeAt(s))) && s + 1 < o && 56320 == (64512 & (n = t.charCodeAt(s + 1))) && (r = 65536 + (r - 55296 << 10) + (n - 56320), s++), h += r < 128 ? 1 : r < 2048 ? 2 : r < 65536 ? 3 : 4;
+                            for (e = i.uint8array ? new Uint8Array(h) : new Array(h), s = a = 0; a < h; s++) 55296 == (64512 & (r = t.charCodeAt(s))) && s + 1 < o && 56320 == (64512 & (n = t.charCodeAt(s + 1))) && (r = 65536 + (r - 55296 << 10) + (n - 56320), s++), r < 128 ? e[a++] = r : (r < 2048 ? e[a++] = 192 | r >>> 6 : (r < 65536 ? e[a++] = 224 | r >>> 12 : (e[a++] = 240 | r >>> 18, e[a++] = 128 | r >>> 12 & 63), e[a++] = 128 | r >>> 6 & 63), e[a++] = 128 | 63 & r);
+                            return e
+                        }(t)
+                    }, r.utf8decode = function(t) {
+                        return i.nodebuffer ? n.transformTo("nodebuffer", t).toString("utf-8") : function(t) {
+                            var e, r, i, s, a = t.length,
+                                h = new Array(2 * a);
+                            for (e = r = 0; e < a;)
+                                if ((i = t[e++]) < 128) h[r++] = i;
+                                else if (4 < (s = o[i])) h[r++] = 65533, e += s - 1;
+                            else {
+                                for (i &= 2 === s ? 31 : 3 === s ? 15 : 7; 1 < s && e < a;) i = i << 6 | 63 & t[e++], s--;
+                                1 < s ? h[r++] = 65533 : i < 65536 ? h[r++] = i : (i -= 65536, h[r++] = 55296 | i >> 10 & 1023, h[r++] = 56320 | 1023 & i)
                             }
+                            return h.length !== r && (h.subarray ? h = h.subarray(0, r) : h.length = r), n.applyFromCharCode(h)
+                        }(t = n.transformTo(i.uint8array ? "uint8array" : "array", t))
+                    }, n.inherits(u, a), u.prototype.processChunk = function(t) {
+                        var e = n.transformTo(i.uint8array ? "uint8array" : "array", t.data);
+                        if (this.leftOver && this.leftOver.length) {
+                            if (i.uint8array) {
+                                var s = e;
+                                (e = new Uint8Array(s.length + this.leftOver.length)).set(this.leftOver, 0), e.set(s, this.leftOver.length)
+                            } else e = this.leftOver.concat(e);
+                            this.leftOver = null
+                        }
+                        var a = function(t, e) {
+                                var r;
+                                for ((e = e || t.length) > t.length && (e = t.length), r = e - 1; 0 <= r && 128 == (192 & t[r]);) r--;
+                                return r < 0 || 0 === r ? e : r + o[t[r]] > e ? r : e
+                            }(e),
+                            h = e;
+                        a !== e.length && (i.uint8array ? (h = e.subarray(0, a), this.leftOver = e.subarray(a, e.length)) : (h = e.slice(0, a), this.leftOver = e.slice(a, e.length))), this.push({
+                            data: r.utf8decode(h),
+                            meta: t.meta
+                        })
+                    }, u.prototype.flush = function() {
+                        this.leftOver && this.leftOver.length && (this.push({
+                            data: r.utf8decode(this.leftOver),
+                            meta: {}
+                        }), this.leftOver = null)
+                    }, r.Utf8DecodeWorker = u, n.inherits(l, a), l.prototype.processChunk = function(t) {
+                        this.push({
+                            data: r.utf8encode(t.data),
+                            meta: t.meta
+                        })
+                    }, r.Utf8EncodeWorker = l
+                }, {
+                    "./nodejsUtils": 14,
+                    "./stream/GenericWorker": 28,
+                    "./support": 30,
+                    "./utils": 32
+                }],
+                32: [function(t, e, r) {
+                    "use strict";
+                    var n = t("./support"),
+                        i = t("./base64"),
+                        s = t("./nodejsUtils"),
+                        a = t("./external");
 
-                            function f(e, t, r) {
-                                var n = t;
-                                switch (t) {
-                                    case "blob":
-                                    case "arraybuffer":
-                                        n = "uint8array";
-                                        break;
-                                    case "base64":
-                                        n = "string"
+                    function o(t) {
+                        return t
+                    }
+
+                    function h(t, e) {
+                        for (var r = 0; r < t.length; ++r) e[r] = 255 & t.charCodeAt(r);
+                        return e
+                    }
+                    t("setimmediate"), r.newBlob = function(t, e) {
+                        r.checkSupport("blob");
+                        try {
+                            return new Blob([t], {
+                                type: e
+                            })
+                        } catch (r) {
+                            try {
+                                var n = new(self.BlobBuilder || self.WebKitBlobBuilder || self.MozBlobBuilder || self.MSBlobBuilder);
+                                return n.append(t), n.getBlob(e)
+                            } catch (t) {
+                                throw new Error("Bug : can't construct the Blob.")
+                            }
+                        }
+                    };
+                    var u = {
+                        stringifyByChunk: function(t, e, r) {
+                            var n = [],
+                                i = 0,
+                                s = t.length;
+                            if (s <= r) return String.fromCharCode.apply(null, t);
+                            for (; i < s;) "array" === e || "nodebuffer" === e ? n.push(String.fromCharCode.apply(null, t.slice(i, Math.min(i + r, s)))) : n.push(String.fromCharCode.apply(null, t.subarray(i, Math.min(i + r, s)))), i += r;
+                            return n.join("")
+                        },
+                        stringifyByChar: function(t) {
+                            for (var e = "", r = 0; r < t.length; r++) e += String.fromCharCode(t[r]);
+                            return e
+                        },
+                        applyCanBeUsed: {
+                            uint8array: function() {
+                                try {
+                                    return n.uint8array && 1 === String.fromCharCode.apply(null, new Uint8Array(1)).length
+                                } catch (t) {
+                                    return !1
                                 }
+                            }(),
+                            nodebuffer: function() {
                                 try {
-                                    this._internalType = n, this._outputType = t, this._mimeType = r, h.checkSupport(n), this._worker = e.pipe(new i(n)), e.lock()
-                                } catch (e) {
-                                    this._worker = new s("error"), this._worker.error(e)
+                                    return n.nodebuffer && 1 === String.fromCharCode.apply(null, s.allocBuffer(1)).length
+                                } catch (t) {
+                                    return !1
                                 }
+                            }()
+                        }
+                    };
+
+                    function l(t) {
+                        var e = 65536,
+                            n = r.getTypeOf(t),
+                            i = !0;
+                        if ("uint8array" === n ? i = u.applyCanBeUsed.uint8array : "nodebuffer" === n && (i = u.applyCanBeUsed.nodebuffer), i)
+                            for (; 1 < e;) try {
+                                return u.stringifyByChunk(t, n, e)
+                            } catch (t) {
+                                e = Math.floor(e / 2)
                             }
-                            f.prototype = {
-                                accumulate: function(e) {
-                                    return l(this, e)
-                                },
-                                on: function(e, t) {
-                                    var r = this;
-                                    return "data" === e ? this._worker.on(e, function(e) {
-                                        t.call(r, e.data, e.meta)
-                                    }) : this._worker.on(e, function() {
-                                        h.delay(t, arguments, r)
-                                    }), this
-                                },
-                                resume: function() {
-                                    return h.delay(this._worker.resume, [], this._worker), this
-                                },
-                                pause: function() {
-                                    return this._worker.pause(), this
-                                },
-                                toNodejsStream: function(e) {
-                                    if (h.checkSupport("nodestream"), "nodebuffer" !== this._outputType) throw new Error(this._outputType + " is not supported by this method");
-                                    return new o(this, {
-                                        objectMode: "nodebuffer" !== this._outputType
-                                    }, e)
-                                }
-                            }, t.exports = f
-                        }, {
-                            "../base64": 1,
-                            "../external": 6,
-                            "../nodejs/NodejsStreamOutputAdapter": 13,
-                            "../support": 30,
-                            "../utils": 32,
-                            "./ConvertWorker": 24,
-                            "./GenericWorker": 28
-                        }],
-                        30: [function(e, t, r) {
-                            "use strict";
-                            if (r.base64 = !0, r.array = !0, r.string = !0, r.arraybuffer = "undefined" != typeof ArrayBuffer && "undefined" != typeof Uint8Array, r.nodebuffer = "undefined" != typeof Buffer, r.uint8array = "undefined" != typeof Uint8Array, "undefined" == typeof ArrayBuffer) r.blob = !1;
+                        return u.stringifyByChar(t)
+                    }
+
+                    function f(t, e) {
+                        for (var r = 0; r < t.length; r++) e[r] = t[r];
+                        return e
+                    }
+                    r.applyFromCharCode = l;
+                    var c = {};
+                    c.string = {
+                        string: o,
+                        array: function(t) {
+                            return h(t, new Array(t.length))
+                        },
+                        arraybuffer: function(t) {
+                            return c.string.uint8array(t).buffer
+                        },
+                        uint8array: function(t) {
+                            return h(t, new Uint8Array(t.length))
+                        },
+                        nodebuffer: function(t) {
+                            return h(t, s.allocBuffer(t.length))
+                        }
+                    }, c.array = {
+                        string: l,
+                        array: o,
+                        arraybuffer: function(t) {
+                            return new Uint8Array(t).buffer
+                        },
+                        uint8array: function(t) {
+                            return new Uint8Array(t)
+                        },
+                        nodebuffer: function(t) {
+                            return s.newBufferFrom(t)
+                        }
+                    }, c.arraybuffer = {
+                        string: function(t) {
+                            return l(new Uint8Array(t))
+                        },
+                        array: function(t) {
+                            return f(new Uint8Array(t), new Array(t.byteLength))
+                        },
+                        arraybuffer: o,
+                        uint8array: function(t) {
+                            return new Uint8Array(t)
+                        },
+                        nodebuffer: function(t) {
+                            return s.newBufferFrom(new Uint8Array(t))
+                        }
+                    }, c.uint8array = {
+                        string: l,
+                        array: function(t) {
+                            return f(t, new Array(t.length))
+                        },
+                        arraybuffer: function(t) {
+                            return t.buffer
+                        },
+                        uint8array: o,
+                        nodebuffer: function(t) {
+                            return s.newBufferFrom(t)
+                        }
+                    }, c.nodebuffer = {
+                        string: l,
+                        array: function(t) {
+                            return f(t, new Array(t.length))
+                        },
+                        arraybuffer: function(t) {
+                            return c.nodebuffer.uint8array(t).buffer
+                        },
+                        uint8array: function(t) {
+                            return f(t, new Uint8Array(t.length))
+                        },
+                        nodebuffer: o
+                    }, r.transformTo = function(t, e) {
+                        if (e = e || "", !t) return e;
+                        r.checkSupport(t);
+                        var n = r.getTypeOf(e);
+                        return c[n][t](e)
+                    }, r.resolve = function(t) {
+                        for (var e = t.split("/"), r = [], n = 0; n < e.length; n++) {
+                            var i = e[n];
+                            "." === i || "" === i && 0 !== n && n !== e.length - 1 || (".." === i ? r.pop() : r.push(i))
+                        }
+                        return r.join("/")
+                    }, r.getTypeOf = function(t) {
+                        return "string" == typeof t ? "string" : "[object Array]" === Object.prototype.toString.call(t) ? "array" : n.nodebuffer && s.isBuffer(t) ? "nodebuffer" : n.uint8array && t instanceof Uint8Array ? "uint8array" : n.arraybuffer && t instanceof ArrayBuffer ? "arraybuffer" : void 0
+                    }, r.checkSupport = function(t) {
+                        if (!n[t.toLowerCase()]) throw new Error(t + " is not supported by this platform")
+                    }, r.MAX_VALUE_16BITS = 65535, r.MAX_VALUE_32BITS = -1, r.pretty = function(t) {
+                        var e, r, n = "";
+                        for (r = 0; r < (t || "").length; r++) n += "\\x" + ((e = t.charCodeAt(r)) < 16 ? "0" : "") + e.toString(16).toUpperCase();
+                        return n
+                    }, r.delay = function(t, e, r) {
+                        setImmediate((function() {
+                            t.apply(r || null, e || [])
+                        }))
+                    }, r.inherits = function(t, e) {
+                        function r() {}
+                        r.prototype = e.prototype, t.prototype = new r
+                    }, r.extend = function() {
+                        var t, e, r = {};
+                        for (t = 0; t < arguments.length; t++)
+                            for (e in arguments[t]) Object.prototype.hasOwnProperty.call(arguments[t], e) && void 0 === r[e] && (r[e] = arguments[t][e]);
+                        return r
+                    }, r.prepareContent = function(t, e, s, o, u) {
+                        return a.Promise.resolve(e).then((function(t) {
+                            return n.blob && (t instanceof Blob || -1 !== ["[object File]", "[object Blob]"].indexOf(Object.prototype.toString.call(t))) && "undefined" != typeof FileReader ? new a.Promise((function(e, r) {
+                                var n = new FileReader;
+                                n.onload = function(t) {
+                                    e(t.target.result)
+                                }, n.onerror = function(t) {
+                                    r(t.target.error)
+                                }, n.readAsArrayBuffer(t)
+                            })) : t
+                        })).then((function(e) {
+                            var l = r.getTypeOf(e);
+                            return l ? ("arraybuffer" === l ? e = r.transformTo("uint8array", e) : "string" === l && (u ? e = i.decode(e) : s && !0 !== o && (e = function(t) {
+                                return h(t, n.uint8array ? new Uint8Array(t.length) : new Array(t.length))
+                            }(e))), e) : a.Promise.reject(new Error("Can't read the data of '" + t + "'. Is it in a supported JavaScript type (String, Blob, ArrayBuffer, etc) ?"))
+                        }))
+                    }
+                }, {
+                    "./base64": 1,
+                    "./external": 6,
+                    "./nodejsUtils": 14,
+                    "./support": 30,
+                    setimmediate: 54
+                }],
+                33: [function(t, e, r) {
+                    "use strict";
+                    var n = t("./reader/readerFor"),
+                        i = t("./utils"),
+                        s = t("./signature"),
+                        a = t("./zipEntry"),
+                        o = t("./support");
+
+                    function h(t) {
+                        this.files = [], this.loadOptions = t
+                    }
+                    h.prototype = {
+                        checkSignature: function(t) {
+                            if (!this.reader.readAndCheckSignature(t)) {
+                                this.reader.index -= 4;
+                                var e = this.reader.readString(4);
+                                throw new Error("Corrupted zip or bug: unexpected signature (" + i.pretty(e) + ", expected " + i.pretty(t) + ")")
+                            }
+                        },
+                        isSignature: function(t, e) {
+                            var r = this.reader.index;
+                            this.reader.setIndex(t);
+                            var n = this.reader.readString(4) === e;
+                            return this.reader.setIndex(r), n
+                        },
+                        readBlockEndOfCentral: function() {
+                            this.diskNumber = this.reader.readInt(2), this.diskWithCentralDirStart = this.reader.readInt(2), this.centralDirRecordsOnThisDisk = this.reader.readInt(2), this.centralDirRecords = this.reader.readInt(2), this.centralDirSize = this.reader.readInt(4), this.centralDirOffset = this.reader.readInt(4), this.zipCommentLength = this.reader.readInt(2);
+                            var t = this.reader.readData(this.zipCommentLength),
+                                e = o.uint8array ? "uint8array" : "array",
+                                r = i.transformTo(e, t);
+                            this.zipComment = this.loadOptions.decodeFileName(r)
+                        },
+                        readBlockZip64EndOfCentral: function() {
+                            this.zip64EndOfCentralSize = this.reader.readInt(8), this.reader.skip(4), this.diskNumber = this.reader.readInt(4), this.diskWithCentralDirStart = this.reader.readInt(4), this.centralDirRecordsOnThisDisk = this.reader.readInt(8), this.centralDirRecords = this.reader.readInt(8), this.centralDirSize = this.reader.readInt(8), this.centralDirOffset = this.reader.readInt(8), this.zip64ExtensibleData = {};
+                            for (var t, e, r, n = this.zip64EndOfCentralSize - 44; 0 < n;) t = this.reader.readInt(2), e = this.reader.readInt(4), r = this.reader.readData(e), this.zip64ExtensibleData[t] = {
+                                id: t,
+                                length: e,
+                                value: r
+                            }
+                        },
+                        readBlockZip64EndOfCentralLocator: function() {
+                            if (this.diskWithZip64CentralDirStart = this.reader.readInt(4), this.relativeOffsetEndOfZip64CentralDir = this.reader.readInt(8), this.disksCount = this.reader.readInt(4), 1 < this.disksCount) throw new Error("Multi-volumes zip are not supported")
+                        },
+                        readLocalFiles: function() {
+                            var t, e;
+                            for (t = 0; t < this.files.length; t++) e = this.files[t], this.reader.setIndex(e.localHeaderOffset), this.checkSignature(s.LOCAL_FILE_HEADER), e.readLocalPart(this.reader), e.handleUTF8(), e.processAttributes()
+                        },
+                        readCentralDir: function() {
+                            var t;
+                            for (this.reader.setIndex(this.centralDirOffset); this.reader.readAndCheckSignature(s.CENTRAL_FILE_HEADER);)(t = new a({
+                                zip64: this.zip64
+                            }, this.loadOptions)).readCentralPart(this.reader), this.files.push(t);
+                            if (this.centralDirRecords !== this.files.length && 0 !== this.centralDirRecords && 0 === this.files.length) throw new Error("Corrupted zip or bug: expected " + this.centralDirRecords + " records in central dir, got " + this.files.length)
+                        },
+                        readEndOfCentral: function() {
+                            var t = this.reader.lastIndexOfSignature(s.CENTRAL_DIRECTORY_END);
+                            if (t < 0) throw this.isSignature(0, s.LOCAL_FILE_HEADER) ? new Error("Corrupted zip: can't find end of central directory") : new Error("Can't find end of central directory : is this a zip file ? If it is, see https://stuk.github.io/jszip/documentation/howto/read_zip.html");
+                            this.reader.setIndex(t);
+                            var e = t;
+                            if (this.checkSignature(s.CENTRAL_DIRECTORY_END), this.readBlockEndOfCentral(), this.diskNumber === i.MAX_VALUE_16BITS || this.diskWithCentralDirStart === i.MAX_VALUE_16BITS || this.centralDirRecordsOnThisDisk === i.MAX_VALUE_16BITS || this.centralDirRecords === i.MAX_VALUE_16BITS || this.centralDirSize === i.MAX_VALUE_32BITS || this.centralDirOffset === i.MAX_VALUE_32BITS) {
+                                if (this.zip64 = !0, (t = this.reader.lastIndexOfSignature(s.ZIP64_CENTRAL_DIRECTORY_LOCATOR)) < 0) throw new Error("Corrupted zip: can't find the ZIP64 end of central directory locator");
+                                if (this.reader.setIndex(t), this.checkSignature(s.ZIP64_CENTRAL_DIRECTORY_LOCATOR), this.readBlockZip64EndOfCentralLocator(), !this.isSignature(this.relativeOffsetEndOfZip64CentralDir, s.ZIP64_CENTRAL_DIRECTORY_END) && (this.relativeOffsetEndOfZip64CentralDir = this.reader.lastIndexOfSignature(s.ZIP64_CENTRAL_DIRECTORY_END), this.relativeOffsetEndOfZip64CentralDir < 0)) throw new Error("Corrupted zip: can't find the ZIP64 end of central directory");
+                                this.reader.setIndex(this.relativeOffsetEndOfZip64CentralDir), this.checkSignature(s.ZIP64_CENTRAL_DIRECTORY_END), this.readBlockZip64EndOfCentral()
+                            }
+                            var r = this.centralDirOffset + this.centralDirSize;
+                            this.zip64 && (r += 20, r += 12 + this.zip64EndOfCentralSize);
+                            var n = e - r;
+                            if (0 < n) this.isSignature(e, s.CENTRAL_FILE_HEADER) || (this.reader.zero = n);
+                            else if (n < 0) throw new Error("Corrupted zip: missing " + Math.abs(n) + " bytes.")
+                        },
+                        prepareReader: function(t) {
+                            this.reader = n(t)
+                        },
+                        load: function(t) {
+                            this.prepareReader(t), this.readEndOfCentral(), this.readCentralDir(), this.readLocalFiles()
+                        }
+                    }, e.exports = h
+                }, {
+                    "./reader/readerFor": 22,
+                    "./signature": 23,
+                    "./support": 30,
+                    "./utils": 32,
+                    "./zipEntry": 34
+                }],
+                34: [function(t, e, r) {
+                    "use strict";
+                    var n = t("./reader/readerFor"),
+                        i = t("./utils"),
+                        s = t("./compressedObject"),
+                        a = t("./crc32"),
+                        o = t("./utf8"),
+                        h = t("./compressions"),
+                        u = t("./support");
+
+                    function l(t, e) {
+                        this.options = t, this.loadOptions = e
+                    }
+                    l.prototype = {
+                        isEncrypted: function() {
+                            return 1 == (1 & this.bitFlag)
+                        },
+                        useUTF8: function() {
+                            return 2048 == (2048 & this.bitFlag)
+                        },
+                        readLocalPart: function(t) {
+                            var e, r;
+                            if (t.skip(22), this.fileNameLength = t.readInt(2), r = t.readInt(2), this.fileName = t.readData(this.fileNameLength), t.skip(r), -1 === this.compressedSize || -1 === this.uncompressedSize) throw new Error("Bug or corrupted zip : didn't get enough information from the central directory (compressedSize === -1 || uncompressedSize === -1)");
+                            if (null === (e = function(t) {
+                                    for (var e in h)
+                                        if (Object.prototype.hasOwnProperty.call(h, e) && h[e].magic === t) return h[e];
+                                    return null
+                                }(this.compressionMethod))) throw new Error("Corrupted zip : compression " + i.pretty(this.compressionMethod) + " unknown (inner file : " + i.transformTo("string", this.fileName) + ")");
+                            this.decompressed = new s(this.compressedSize, this.uncompressedSize, this.crc32, e, t.readData(this.compressedSize))
+                        },
+                        readCentralPart: function(t) {
+                            this.versionMadeBy = t.readInt(2), t.skip(2), this.bitFlag = t.readInt(2), this.compressionMethod = t.readString(2), this.date = t.readDate(), this.crc32 = t.readInt(4), this.compressedSize = t.readInt(4), this.uncompressedSize = t.readInt(4);
+                            var e = t.readInt(2);
+                            if (this.extraFieldsLength = t.readInt(2), this.fileCommentLength = t.readInt(2), this.diskNumberStart = t.readInt(2), this.internalFileAttributes = t.readInt(2), this.externalFileAttributes = t.readInt(4), this.localHeaderOffset = t.readInt(4), this.isEncrypted()) throw new Error("Encrypted zip are not supported");
+                            t.skip(e), this.readExtraFields(t), this.parseZIP64ExtraField(t), this.fileComment = t.readData(this.fileCommentLength)
+                        },
+                        processAttributes: function() {
+                            this.unixPermissions = null, this.dosPermissions = null;
+                            var t = this.versionMadeBy >> 8;
+                            this.dir = !!(16 & this.externalFileAttributes), 0 == t && (this.dosPermissions = 63 & this.externalFileAttributes), 3 == t && (this.unixPermissions = this.externalFileAttributes >> 16 & 65535), this.dir || "/" !== this.fileNameStr.slice(-1) || (this.dir = !0)
+                        },
+                        parseZIP64ExtraField: function() {
+                            if (this.extraFields[1]) {
+                                var t = n(this.extraFields[1].value);
+                                this.uncompressedSize === i.MAX_VALUE_32BITS && (this.uncompressedSize = t.readInt(8)), this.compressedSize === i.MAX_VALUE_32BITS && (this.compressedSize = t.readInt(8)), this.localHeaderOffset === i.MAX_VALUE_32BITS && (this.localHeaderOffset = t.readInt(8)), this.diskNumberStart === i.MAX_VALUE_32BITS && (this.diskNumberStart = t.readInt(4))
+                            }
+                        },
+                        readExtraFields: function(t) {
+                            var e, r, n, i = t.index + this.extraFieldsLength;
+                            for (this.extraFields || (this.extraFields = {}); t.index + 4 < i;) e = t.readInt(2), r = t.readInt(2), n = t.readData(r), this.extraFields[e] = {
+                                id: e,
+                                length: r,
+                                value: n
+                            };
+                            t.setIndex(i)
+                        },
+                        handleUTF8: function() {
+                            var t = u.uint8array ? "uint8array" : "array";
+                            if (this.useUTF8()) this.fileNameStr = o.utf8decode(this.fileName), this.fileCommentStr = o.utf8decode(this.fileComment);
                             else {
-                                var n = new ArrayBuffer(0);
-                                try {
-                                    r.blob = 0 === new Blob([n], {
-                                        type: "application/zip"
-                                    }).size
-                                } catch (e) {
-                                    try {
-                                        var i = new(self.BlobBuilder || self.WebKitBlobBuilder || self.MozBlobBuilder || self.MSBlobBuilder);
-                                        i.append(n), r.blob = 0 === i.getBlob("application/zip").size
-                                    } catch (e) {
-                                        r.blob = !1
-                                    }
+                                var e = this.findExtraFieldUnicodePath();
+                                if (null !== e) this.fileNameStr = e;
+                                else {
+                                    var r = i.transformTo(t, this.fileName);
+                                    this.fileNameStr = this.loadOptions.decodeFileName(r)
                                 }
+                                var n = this.findExtraFieldUnicodeComment();
+                                if (null !== n) this.fileCommentStr = n;
+                                else {
+                                    var s = i.transformTo(t, this.fileComment);
+                                    this.fileCommentStr = this.loadOptions.decodeFileName(s)
+                                }
+                            }
+                        },
+                        findExtraFieldUnicodePath: function() {
+                            var t = this.extraFields[28789];
+                            if (t) {
+                                var e = n(t.value);
+                                return 1 !== e.readInt(1) || a(this.fileName) !== e.readInt(4) ? null : o.utf8decode(e.readData(t.length - 5))
+                            }
+                            return null
+                        },
+                        findExtraFieldUnicodeComment: function() {
+                            var t = this.extraFields[25461];
+                            if (t) {
+                                var e = n(t.value);
+                                return 1 !== e.readInt(1) || a(this.fileComment) !== e.readInt(4) ? null : o.utf8decode(e.readData(t.length - 5))
                             }
+                            return null
+                        }
+                    }, e.exports = l
+                }, {
+                    "./compressedObject": 2,
+                    "./compressions": 3,
+                    "./crc32": 4,
+                    "./reader/readerFor": 22,
+                    "./support": 30,
+                    "./utf8": 31,
+                    "./utils": 32
+                }],
+                35: [function(t, e, r) {
+                    "use strict";
+
+                    function n(t, e, r) {
+                        this.name = t, this.dir = r.dir, this.date = r.date, this.comment = r.comment, this.unixPermissions = r.unixPermissions, this.dosPermissions = r.dosPermissions, this._data = e, this._dataBinary = r.binary, this.options = {
+                            compression: r.compression,
+                            compressionOptions: r.compressionOptions
+                        }
+                    }
+                    var i = t("./stream/StreamHelper"),
+                        s = t("./stream/DataWorker"),
+                        a = t("./utf8"),
+                        o = t("./compressedObject"),
+                        h = t("./stream/GenericWorker");
+                    n.prototype = {
+                        internalStream: function(t) {
+                            var e = null,
+                                r = "string";
                             try {
-                                r.nodestream = !!e("readable-stream").Readable
-                            } catch (e) {
-                                r.nodestream = !1
+                                if (!t) throw new Error("No output type specified.");
+                                var n = "string" === (r = t.toLowerCase()) || "text" === r;
+                                "binarystring" !== r && "text" !== r || (r = "string"), e = this._decompressWorker();
+                                var s = !this._dataBinary;
+                                s && !n && (e = e.pipe(new a.Utf8EncodeWorker)), !s && n && (e = e.pipe(new a.Utf8DecodeWorker))
+                            } catch (t) {
+                                (e = new h("error")).error(t)
+                            }
+                            return new i(e, r, "")
+                        },
+                        async: function(t, e) {
+                            return this.internalStream(t).accumulate(e)
+                        },
+                        nodeStream: function(t, e) {
+                            return this.internalStream(t || "nodebuffer").toNodejsStream(e)
+                        },
+                        _compressWorker: function(t, e) {
+                            if (this._data instanceof o && this._data.compression.magic === t.magic) return this._data.getCompressedWorker();
+                            var r = this._decompressWorker();
+                            return this._dataBinary || (r = r.pipe(new a.Utf8EncodeWorker)), o.createWorkerFrom(r, t, e)
+                        },
+                        _decompressWorker: function() {
+                            return this._data instanceof o ? this._data.getContentWorker() : this._data instanceof h ? this._data : new s(this._data)
+                        }
+                    };
+                    for (var u = ["asText", "asBinary", "asNodeBuffer", "asUint8Array", "asArrayBuffer"], l = function() {
+                            throw new Error("This method has been removed in JSZip 3.0, please check the upgrade guide.")
+                        }, f = 0; f < u.length; f++) n.prototype[u[f]] = l;
+                    e.exports = n
+                }, {
+                    "./compressedObject": 2,
+                    "./stream/DataWorker": 27,
+                    "./stream/GenericWorker": 28,
+                    "./stream/StreamHelper": 29,
+                    "./utf8": 31
+                }],
+                36: [function(t, e, n) {
+                    (function(t) {
+                        "use strict";
+                        var r, n, i = t.MutationObserver || t.WebKitMutationObserver;
+                        if (i) {
+                            var s = 0,
+                                a = new i(l),
+                                o = t.document.createTextNode("");
+                            a.observe(o, {
+                                characterData: !0
+                            }), r = function() {
+                                o.data = s = ++s % 2
+                            }
+                        } else if (t.setImmediate || void 0 === t.MessageChannel) r = "document" in t && "onreadystatechange" in t.document.createElement("script") ? function() {
+                            var e = t.document.createElement("script");
+                            e.onreadystatechange = function() {
+                                l(), e.onreadystatechange = null, e.parentNode.removeChild(e), e = null
+                            }, t.document.documentElement.appendChild(e)
+                        } : function() {
+                            setTimeout(l, 0)
+                        };
+                        else {
+                            var h = new t.MessageChannel;
+                            h.port1.onmessage = l, r = function() {
+                                h.port2.postMessage(0)
                             }
-                        }, {
-                            "readable-stream": 16
-                        }],
-                        31: [function(e, t, s) {
-                            "use strict";
-                            for (var o = e("./utils"), h = e("./support"), r = e("./nodejsUtils"), n = e("./stream/GenericWorker"), u = new Array(256), i = 0; i < 256; i++) u[i] = 252 <= i ? 6 : 248 <= i ? 5 : 240 <= i ? 4 : 224 <= i ? 3 : 192 <= i ? 2 : 1;
-                            u[254] = u[254] = 1;
+                        }
+                        var u = [];
 
-                            function a() {
-                                n.call(this, "utf-8 decode"), this.leftOver = null
+                        function l() {
+                            var t, e;
+                            n = !0;
+                            for (var r = u.length; r;) {
+                                for (e = u, u = [], t = -1; ++t < r;) e[t]();
+                                r = u.length
                             }
+                            n = !1
+                        }
+                        e.exports = function(t) {
+                            1 !== u.push(t) || n || r()
+                        }
+                    }).call(this, void 0 !== r.g ? r.g : "undefined" != typeof self ? self : "undefined" != typeof window ? window : {})
+                }, {}],
+                37: [function(t, e, r) {
+                    "use strict";
+                    var n = t("immediate");
+
+                    function i() {}
+                    var s = {},
+                        a = ["REJECTED"],
+                        o = ["FULFILLED"],
+                        h = ["PENDING"];
+
+                    function u(t) {
+                        if ("function" != typeof t) throw new TypeError("resolver must be a function");
+                        this.state = h, this.queue = [], this.outcome = void 0, t !== i && d(this, t)
+                    }
 
-                            function l() {
-                                n.call(this, "utf-8 encode")
-                            }
-                            s.utf8encode = function(e) {
-                                return h.nodebuffer ? r.newBufferFrom(e, "utf-8") : function(e) {
-                                    var t, r, n, i, s, a = e.length,
-                                        o = 0;
-                                    for (i = 0; i < a; i++) 55296 == (64512 & (r = e.charCodeAt(i))) && i + 1 < a && 56320 == (64512 & (n = e.charCodeAt(i + 1))) && (r = 65536 + (r - 55296 << 10) + (n - 56320), i++), o += r < 128 ? 1 : r < 2048 ? 2 : r < 65536 ? 3 : 4;
-                                    for (t = h.uint8array ? new Uint8Array(o) : new Array(o), i = s = 0; s < o; i++) 55296 == (64512 & (r = e.charCodeAt(i))) && i + 1 < a && 56320 == (64512 & (n = e.charCodeAt(i + 1))) && (r = 65536 + (r - 55296 << 10) + (n - 56320), i++), r < 128 ? t[s++] = r : (r < 2048 ? t[s++] = 192 | r >>> 6 : (r < 65536 ? t[s++] = 224 | r >>> 12 : (t[s++] = 240 | r >>> 18, t[s++] = 128 | r >>> 12 & 63), t[s++] = 128 | r >>> 6 & 63), t[s++] = 128 | 63 & r);
-                                    return t
-                                }(e)
-                            }, s.utf8decode = function(e) {
-                                return h.nodebuffer ? o.transformTo("nodebuffer", e).toString("utf-8") : function(e) {
-                                    var t, r, n, i, s = e.length,
-                                        a = new Array(2 * s);
-                                    for (t = r = 0; t < s;)
-                                        if ((n = e[t++]) < 128) a[r++] = n;
-                                        else if (4 < (i = u[n])) a[r++] = 65533, t += i - 1;
-                                    else {
-                                        for (n &= 2 === i ? 31 : 3 === i ? 15 : 7; 1 < i && t < s;) n = n << 6 | 63 & e[t++], i--;
-                                        1 < i ? a[r++] = 65533 : n < 65536 ? a[r++] = n : (n -= 65536, a[r++] = 55296 | n >> 10 & 1023, a[r++] = 56320 | 1023 & n)
-                                    }
-                                    return a.length !== r && (a.subarray ? a = a.subarray(0, r) : a.length = r), o.applyFromCharCode(a)
-                                }(e = o.transformTo(h.uint8array ? "uint8array" : "array", e))
-                            }, o.inherits(a, n), a.prototype.processChunk = function(e) {
-                                var t = o.transformTo(h.uint8array ? "uint8array" : "array", e.data);
-                                if (this.leftOver && this.leftOver.length) {
-                                    if (h.uint8array) {
-                                        var r = t;
-                                        (t = new Uint8Array(r.length + this.leftOver.length)).set(this.leftOver, 0), t.set(r, this.leftOver.length)
-                                    } else t = this.leftOver.concat(t);
-                                    this.leftOver = null
-                                }
-                                var n = function(e, t) {
-                                        var r;
-                                        for ((t = t || e.length) > e.length && (t = e.length), r = t - 1; 0 <= r && 128 == (192 & e[r]);) r--;
-                                        return r < 0 ? t : 0 === r ? t : r + u[e[r]] > t ? r : t
-                                    }(t),
-                                    i = t;
-                                n !== t.length && (h.uint8array ? (i = t.subarray(0, n), this.leftOver = t.subarray(n, t.length)) : (i = t.slice(0, n), this.leftOver = t.slice(n, t.length))), this.push({
-                                    data: s.utf8decode(i),
-                                    meta: e.meta
-                                })
-                            }, a.prototype.flush = function() {
-                                this.leftOver && this.leftOver.length && (this.push({
-                                    data: s.utf8decode(this.leftOver),
-                                    meta: {}
-                                }), this.leftOver = null)
-                            }, s.Utf8DecodeWorker = a, o.inherits(l, n), l.prototype.processChunk = function(e) {
-                                this.push({
-                                    data: s.utf8encode(e.data),
-                                    meta: e.meta
-                                })
-                            }, s.Utf8EncodeWorker = l
-                        }, {
-                            "./nodejsUtils": 14,
-                            "./stream/GenericWorker": 28,
-                            "./support": 30,
-                            "./utils": 32
-                        }],
-                        32: [function(e, t, a) {
-                            "use strict";
-                            var o = e("./support"),
-                                h = e("./base64"),
-                                r = e("./nodejsUtils"),
-                                u = e("./external");
+                    function l(t, e, r) {
+                        this.promise = t, "function" == typeof e && (this.onFulfilled = e, this.callFulfilled = this.otherCallFulfilled), "function" == typeof r && (this.onRejected = r, this.callRejected = this.otherCallRejected)
+                    }
 
-                            function n(e) {
-                                return e
+                    function f(t, e, r) {
+                        n((function() {
+                            var n;
+                            try {
+                                n = e(r)
+                            } catch (n) {
+                                return s.reject(t, n)
                             }
+                            n === t ? s.reject(t, new TypeError("Cannot resolve promise with itself")) : s.resolve(t, n)
+                        }))
+                    }
 
-                            function l(e, t) {
-                                for (var r = 0; r < e.length; ++r) t[r] = 255 & e.charCodeAt(r);
-                                return t
-                            }
-                            e("setimmediate"), a.newBlob = function(t, r) {
-                                a.checkSupport("blob");
-                                try {
-                                    return new Blob([t], {
-                                        type: r
-                                    })
-                                } catch (e) {
-                                    try {
-                                        var n = new(self.BlobBuilder || self.WebKitBlobBuilder || self.MozBlobBuilder || self.MSBlobBuilder);
-                                        return n.append(t), n.getBlob(r)
-                                    } catch (e) {
-                                        throw new Error("Bug : can't construct the Blob.")
-                                    }
-                                }
-                            };
-                            var i = {
-                                stringifyByChunk: function(e, t, r) {
-                                    var n = [],
-                                        i = 0,
-                                        s = e.length;
-                                    if (s <= r) return String.fromCharCode.apply(null, e);
-                                    for (; i < s;) "array" === t || "nodebuffer" === t ? n.push(String.fromCharCode.apply(null, e.slice(i, Math.min(i + r, s)))) : n.push(String.fromCharCode.apply(null, e.subarray(i, Math.min(i + r, s)))), i += r;
-                                    return n.join("")
-                                },
-                                stringifyByChar: function(e) {
-                                    for (var t = "", r = 0; r < e.length; r++) t += String.fromCharCode(e[r]);
-                                    return t
-                                },
-                                applyCanBeUsed: {
-                                    uint8array: function() {
-                                        try {
-                                            return o.uint8array && 1 === String.fromCharCode.apply(null, new Uint8Array(1)).length
-                                        } catch (e) {
-                                            return !1
-                                        }
-                                    }(),
-                                    nodebuffer: function() {
-                                        try {
-                                            return o.nodebuffer && 1 === String.fromCharCode.apply(null, r.allocBuffer(1)).length
-                                        } catch (e) {
-                                            return !1
-                                        }
-                                    }()
-                                }
-                            };
+                    function c(t) {
+                        var e = t && t.then;
+                        if (t && ("object" == typeof t || "function" == typeof t) && "function" == typeof e) return function() {
+                            e.apply(t, arguments)
+                        }
+                    }
 
-                            function s(e) {
-                                var t = 65536,
-                                    r = a.getTypeOf(e),
-                                    n = !0;
-                                if ("uint8array" === r ? n = i.applyCanBeUsed.uint8array : "nodebuffer" === r && (n = i.applyCanBeUsed.nodebuffer), n)
-                                    for (; 1 < t;) try {
-                                        return i.stringifyByChunk(e, r, t)
-                                    } catch (e) {
-                                        t = Math.floor(t / 2)
-                                    }
-                                return i.stringifyByChar(e)
-                            }
-
-                            function f(e, t) {
-                                for (var r = 0; r < e.length; r++) t[r] = e[r];
-                                return t
-                            }
-                            a.applyFromCharCode = s;
-                            var c = {};
-                            c.string = {
-                                string: n,
-                                array: function(e) {
-                                    return l(e, new Array(e.length))
-                                },
-                                arraybuffer: function(e) {
-                                    return c.string.uint8array(e).buffer
-                                },
-                                uint8array: function(e) {
-                                    return l(e, new Uint8Array(e.length))
-                                },
-                                nodebuffer: function(e) {
-                                    return l(e, r.allocBuffer(e.length))
-                                }
-                            }, c.array = {
-                                string: s,
-                                array: n,
-                                arraybuffer: function(e) {
-                                    return new Uint8Array(e).buffer
-                                },
-                                uint8array: function(e) {
-                                    return new Uint8Array(e)
-                                },
-                                nodebuffer: function(e) {
-                                    return r.newBufferFrom(e)
-                                }
-                            }, c.arraybuffer = {
-                                string: function(e) {
-                                    return s(new Uint8Array(e))
-                                },
-                                array: function(e) {
-                                    return f(new Uint8Array(e), new Array(e.byteLength))
-                                },
-                                arraybuffer: n,
-                                uint8array: function(e) {
-                                    return new Uint8Array(e)
-                                },
-                                nodebuffer: function(e) {
-                                    return r.newBufferFrom(new Uint8Array(e))
-                                }
-                            }, c.uint8array = {
-                                string: s,
-                                array: function(e) {
-                                    return f(e, new Array(e.length))
-                                },
-                                arraybuffer: function(e) {
-                                    return e.buffer
-                                },
-                                uint8array: n,
-                                nodebuffer: function(e) {
-                                    return r.newBufferFrom(e)
-                                }
-                            }, c.nodebuffer = {
-                                string: s,
-                                array: function(e) {
-                                    return f(e, new Array(e.length))
-                                },
-                                arraybuffer: function(e) {
-                                    return c.nodebuffer.uint8array(e).buffer
-                                },
-                                uint8array: function(e) {
-                                    return f(e, new Uint8Array(e.length))
-                                },
-                                nodebuffer: n
-                            }, a.transformTo = function(e, t) {
-                                if (t = t || "", !e) return t;
-                                a.checkSupport(e);
-                                var r = a.getTypeOf(t);
-                                return c[r][e](t)
-                            }, a.resolve = function(e) {
-                                for (var t = e.split("/"), r = [], n = 0; n < t.length; n++) {
-                                    var i = t[n];
-                                    "." === i || "" === i && 0 !== n && n !== t.length - 1 || (".." === i ? r.pop() : r.push(i))
-                                }
-                                return r.join("/")
-                            }, a.getTypeOf = function(e) {
-                                return "string" == typeof e ? "string" : "[object Array]" === Object.prototype.toString.call(e) ? "array" : o.nodebuffer && r.isBuffer(e) ? "nodebuffer" : o.uint8array && e instanceof Uint8Array ? "uint8array" : o.arraybuffer && e instanceof ArrayBuffer ? "arraybuffer" : void 0
-                            }, a.checkSupport = function(e) {
-                                if (!o[e.toLowerCase()]) throw new Error(e + " is not supported by this platform")
-                            }, a.MAX_VALUE_16BITS = 65535, a.MAX_VALUE_32BITS = -1, a.pretty = function(e) {
-                                var t, r, n = "";
-                                for (r = 0; r < (e || "").length; r++) n += "\\x" + ((t = e.charCodeAt(r)) < 16 ? "0" : "") + t.toString(16).toUpperCase();
-                                return n
-                            }, a.delay = function(e, t, r) {
-                                setImmediate(function() {
-                                    e.apply(r || null, t || [])
-                                })
-                            }, a.inherits = function(e, t) {
-                                function r() {}
-                                r.prototype = t.prototype, e.prototype = new r
-                            }, a.extend = function() {
-                                var e, t, r = {};
-                                for (e = 0; e < arguments.length; e++)
-                                    for (t in arguments[e]) Object.prototype.hasOwnProperty.call(arguments[e], t) && void 0 === r[t] && (r[t] = arguments[e][t]);
-                                return r
-                            }, a.prepareContent = function(r, e, n, i, s) {
-                                return u.Promise.resolve(e).then(function(n) {
-                                    return o.blob && (n instanceof Blob || -1 !== ["[object File]", "[object Blob]"].indexOf(Object.prototype.toString.call(n))) && "undefined" != typeof FileReader ? new u.Promise(function(t, r) {
-                                        var e = new FileReader;
-                                        e.onload = function(e) {
-                                            t(e.target.result)
-                                        }, e.onerror = function(e) {
-                                            r(e.target.error)
-                                        }, e.readAsArrayBuffer(n)
-                                    }) : n
-                                }).then(function(e) {
-                                    var t = a.getTypeOf(e);
-                                    return t ? ("arraybuffer" === t ? e = a.transformTo("uint8array", e) : "string" === t && (s ? e = h.decode(e) : n && !0 !== i && (e = function(e) {
-                                        return l(e, o.uint8array ? new Uint8Array(e.length) : new Array(e.length))
-                                    }(e))), e) : u.Promise.reject(new Error("Can't read the data of '" + r + "'. Is it in a supported JavaScript type (String, Blob, ArrayBuffer, etc) ?"))
-                                })
-                            }
-                        }, {
-                            "./base64": 1,
-                            "./external": 6,
-                            "./nodejsUtils": 14,
-                            "./support": 30,
-                            setimmediate: 54
-                        }],
-                        33: [function(e, t, r) {
-                            "use strict";
-                            var n = e("./reader/readerFor"),
-                                i = e("./utils"),
-                                s = e("./signature"),
-                                a = e("./zipEntry"),
-                                o = e("./support");
-
-                            function h(e) {
-                                this.files = [], this.loadOptions = e
-                            }
-                            h.prototype = {
-                                checkSignature: function(e) {
-                                    if (!this.reader.readAndCheckSignature(e)) {
-                                        this.reader.index -= 4;
-                                        var t = this.reader.readString(4);
-                                        throw new Error("Corrupted zip or bug: unexpected signature (" + i.pretty(t) + ", expected " + i.pretty(e) + ")")
-                                    }
-                                },
-                                isSignature: function(e, t) {
-                                    var r = this.reader.index;
-                                    this.reader.setIndex(e);
-                                    var n = this.reader.readString(4) === t;
-                                    return this.reader.setIndex(r), n
-                                },
-                                readBlockEndOfCentral: function() {
-                                    this.diskNumber = this.reader.readInt(2), this.diskWithCentralDirStart = this.reader.readInt(2), this.centralDirRecordsOnThisDisk = this.reader.readInt(2), this.centralDirRecords = this.reader.readInt(2), this.centralDirSize = this.reader.readInt(4), this.centralDirOffset = this.reader.readInt(4), this.zipCommentLength = this.reader.readInt(2);
-                                    var e = this.reader.readData(this.zipCommentLength),
-                                        t = o.uint8array ? "uint8array" : "array",
-                                        r = i.transformTo(t, e);
-                                    this.zipComment = this.loadOptions.decodeFileName(r)
-                                },
-                                readBlockZip64EndOfCentral: function() {
-                                    this.zip64EndOfCentralSize = this.reader.readInt(8), this.reader.skip(4), this.diskNumber = this.reader.readInt(4), this.diskWithCentralDirStart = this.reader.readInt(4), this.centralDirRecordsOnThisDisk = this.reader.readInt(8), this.centralDirRecords = this.reader.readInt(8), this.centralDirSize = this.reader.readInt(8), this.centralDirOffset = this.reader.readInt(8), this.zip64ExtensibleData = {};
-                                    for (var e, t, r, n = this.zip64EndOfCentralSize - 44; 0 < n;) e = this.reader.readInt(2), t = this.reader.readInt(4), r = this.reader.readData(t), this.zip64ExtensibleData[e] = {
-                                        id: e,
-                                        length: t,
-                                        value: r
-                                    }
-                                },
-                                readBlockZip64EndOfCentralLocator: function() {
-                                    if (this.diskWithZip64CentralDirStart = this.reader.readInt(4), this.relativeOffsetEndOfZip64CentralDir = this.reader.readInt(8), this.disksCount = this.reader.readInt(4), 1 < this.disksCount) throw new Error("Multi-volumes zip are not supported")
-                                },
-                                readLocalFiles: function() {
-                                    var e, t;
-                                    for (e = 0; e < this.files.length; e++) t = this.files[e], this.reader.setIndex(t.localHeaderOffset), this.checkSignature(s.LOCAL_FILE_HEADER), t.readLocalPart(this.reader), t.handleUTF8(), t.processAttributes()
-                                },
-                                readCentralDir: function() {
-                                    var e;
-                                    for (this.reader.setIndex(this.centralDirOffset); this.reader.readAndCheckSignature(s.CENTRAL_FILE_HEADER);)(e = new a({
-                                        zip64: this.zip64
-                                    }, this.loadOptions)).readCentralPart(this.reader), this.files.push(e);
-                                    if (this.centralDirRecords !== this.files.length && 0 !== this.centralDirRecords && 0 === this.files.length) throw new Error("Corrupted zip or bug: expected " + this.centralDirRecords + " records in central dir, got " + this.files.length)
-                                },
-                                readEndOfCentral: function() {
-                                    var e = this.reader.lastIndexOfSignature(s.CENTRAL_DIRECTORY_END);
-                                    if (e < 0) throw !this.isSignature(0, s.LOCAL_FILE_HEADER) ? new Error("Can't find end of central directory : is this a zip file ? If it is, see https://stuk.github.io/jszip/documentation/howto/read_zip.html") : new Error("Corrupted zip: can't find end of central directory");
-                                    this.reader.setIndex(e);
-                                    var t = e;
-                                    if (this.checkSignature(s.CENTRAL_DIRECTORY_END), this.readBlockEndOfCentral(), this.diskNumber === i.MAX_VALUE_16BITS || this.diskWithCentralDirStart === i.MAX_VALUE_16BITS || this.centralDirRecordsOnThisDisk === i.MAX_VALUE_16BITS || this.centralDirRecords === i.MAX_VALUE_16BITS || this.centralDirSize === i.MAX_VALUE_32BITS || this.centralDirOffset === i.MAX_VALUE_32BITS) {
-                                        if (this.zip64 = !0, (e = this.reader.lastIndexOfSignature(s.ZIP64_CENTRAL_DIRECTORY_LOCATOR)) < 0) throw new Error("Corrupted zip: can't find the ZIP64 end of central directory locator");
-                                        if (this.reader.setIndex(e), this.checkSignature(s.ZIP64_CENTRAL_DIRECTORY_LOCATOR), this.readBlockZip64EndOfCentralLocator(), !this.isSignature(this.relativeOffsetEndOfZip64CentralDir, s.ZIP64_CENTRAL_DIRECTORY_END) && (this.relativeOffsetEndOfZip64CentralDir = this.reader.lastIndexOfSignature(s.ZIP64_CENTRAL_DIRECTORY_END), this.relativeOffsetEndOfZip64CentralDir < 0)) throw new Error("Corrupted zip: can't find the ZIP64 end of central directory");
-                                        this.reader.setIndex(this.relativeOffsetEndOfZip64CentralDir), this.checkSignature(s.ZIP64_CENTRAL_DIRECTORY_END), this.readBlockZip64EndOfCentral()
-                                    }
-                                    var r = this.centralDirOffset + this.centralDirSize;
-                                    this.zip64 && (r += 20, r += 12 + this.zip64EndOfCentralSize);
-                                    var n = t - r;
-                                    if (0 < n) this.isSignature(t, s.CENTRAL_FILE_HEADER) || (this.reader.zero = n);
-                                    else if (n < 0) throw new Error("Corrupted zip: missing " + Math.abs(n) + " bytes.")
-                                },
-                                prepareReader: function(e) {
-                                    this.reader = n(e)
-                                },
-                                load: function(e) {
-                                    this.prepareReader(e), this.readEndOfCentral(), this.readCentralDir(), this.readLocalFiles()
-                                }
-                            }, t.exports = h
-                        }, {
-                            "./reader/readerFor": 22,
-                            "./signature": 23,
-                            "./support": 30,
-                            "./utils": 32,
-                            "./zipEntry": 34
-                        }],
-                        34: [function(e, t, r) {
-                            "use strict";
-                            var n = e("./reader/readerFor"),
-                                s = e("./utils"),
-                                i = e("./compressedObject"),
-                                a = e("./crc32"),
-                                o = e("./utf8"),
-                                h = e("./compressions"),
-                                u = e("./support");
-
-                            function l(e, t) {
-                                this.options = e, this.loadOptions = t
-                            }
-                            l.prototype = {
-                                isEncrypted: function() {
-                                    return 1 == (1 & this.bitFlag)
-                                },
-                                useUTF8: function() {
-                                    return 2048 == (2048 & this.bitFlag)
-                                },
-                                readLocalPart: function(e) {
-                                    var t, r;
-                                    if (e.skip(22), this.fileNameLength = e.readInt(2), r = e.readInt(2), this.fileName = e.readData(this.fileNameLength), e.skip(r), -1 === this.compressedSize || -1 === this.uncompressedSize) throw new Error("Bug or corrupted zip : didn't get enough information from the central directory (compressedSize === -1 || uncompressedSize === -1)");
-                                    if (null === (t = function(e) {
-                                            for (var t in h)
-                                                if (Object.prototype.hasOwnProperty.call(h, t) && h[t].magic === e) return h[t];
-                                            return null
-                                        }(this.compressionMethod))) throw new Error("Corrupted zip : compression " + s.pretty(this.compressionMethod) + " unknown (inner file : " + s.transformTo("string", this.fileName) + ")");
-                                    this.decompressed = new i(this.compressedSize, this.uncompressedSize, this.crc32, t, e.readData(this.compressedSize))
-                                },
-                                readCentralPart: function(e) {
-                                    this.versionMadeBy = e.readInt(2), e.skip(2), this.bitFlag = e.readInt(2), this.compressionMethod = e.readString(2), this.date = e.readDate(), this.crc32 = e.readInt(4), this.compressedSize = e.readInt(4), this.uncompressedSize = e.readInt(4);
-                                    var t = e.readInt(2);
-                                    if (this.extraFieldsLength = e.readInt(2), this.fileCommentLength = e.readInt(2), this.diskNumberStart = e.readInt(2), this.internalFileAttributes = e.readInt(2), this.externalFileAttributes = e.readInt(4), this.localHeaderOffset = e.readInt(4), this.isEncrypted()) throw new Error("Encrypted zip are not supported");
-                                    e.skip(t), this.readExtraFields(e), this.parseZIP64ExtraField(e), this.fileComment = e.readData(this.fileCommentLength)
-                                },
-                                processAttributes: function() {
-                                    this.unixPermissions = null, this.dosPermissions = null;
-                                    var e = this.versionMadeBy >> 8;
-                                    this.dir = !!(16 & this.externalFileAttributes), 0 == e && (this.dosPermissions = 63 & this.externalFileAttributes), 3 == e && (this.unixPermissions = this.externalFileAttributes >> 16 & 65535), this.dir || "/" !== this.fileNameStr.slice(-1) || (this.dir = !0)
-                                },
-                                parseZIP64ExtraField: function() {
-                                    if (this.extraFields[1]) {
-                                        var e = n(this.extraFields[1].value);
-                                        this.uncompressedSize === s.MAX_VALUE_32BITS && (this.uncompressedSize = e.readInt(8)), this.compressedSize === s.MAX_VALUE_32BITS && (this.compressedSize = e.readInt(8)), this.localHeaderOffset === s.MAX_VALUE_32BITS && (this.localHeaderOffset = e.readInt(8)), this.diskNumberStart === s.MAX_VALUE_32BITS && (this.diskNumberStart = e.readInt(4))
-                                    }
-                                },
-                                readExtraFields: function(e) {
-                                    var t, r, n, i = e.index + this.extraFieldsLength;
-                                    for (this.extraFields || (this.extraFields = {}); e.index + 4 < i;) t = e.readInt(2), r = e.readInt(2), n = e.readData(r), this.extraFields[t] = {
-                                        id: t,
-                                        length: r,
-                                        value: n
-                                    };
-                                    e.setIndex(i)
-                                },
-                                handleUTF8: function() {
-                                    var e = u.uint8array ? "uint8array" : "array";
-                                    if (this.useUTF8()) this.fileNameStr = o.utf8decode(this.fileName), this.fileCommentStr = o.utf8decode(this.fileComment);
-                                    else {
-                                        var t = this.findExtraFieldUnicodePath();
-                                        if (null !== t) this.fileNameStr = t;
-                                        else {
-                                            var r = s.transformTo(e, this.fileName);
-                                            this.fileNameStr = this.loadOptions.decodeFileName(r)
-                                        }
-                                        var n = this.findExtraFieldUnicodeComment();
-                                        if (null !== n) this.fileCommentStr = n;
-                                        else {
-                                            var i = s.transformTo(e, this.fileComment);
-                                            this.fileCommentStr = this.loadOptions.decodeFileName(i)
-                                        }
-                                    }
-                                },
-                                findExtraFieldUnicodePath: function() {
-                                    var e = this.extraFields[28789];
-                                    if (e) {
-                                        var t = n(e.value);
-                                        return 1 !== t.readInt(1) ? null : a(this.fileName) !== t.readInt(4) ? null : o.utf8decode(t.readData(e.length - 5))
-                                    }
-                                    return null
-                                },
-                                findExtraFieldUnicodeComment: function() {
-                                    var e = this.extraFields[25461];
-                                    if (e) {
-                                        var t = n(e.value);
-                                        return 1 !== t.readInt(1) ? null : a(this.fileComment) !== t.readInt(4) ? null : o.utf8decode(t.readData(e.length - 5))
-                                    }
-                                    return null
-                                }
-                            }, t.exports = l
-                        }, {
-                            "./compressedObject": 2,
-                            "./compressions": 3,
-                            "./crc32": 4,
-                            "./reader/readerFor": 22,
-                            "./support": 30,
-                            "./utf8": 31,
-                            "./utils": 32
-                        }],
-                        35: [function(e, t, r) {
-                            "use strict";
+                    function d(t, e) {
+                        var r = !1;
 
-                            function n(e, t, r) {
-                                this.name = e, this.dir = r.dir, this.date = r.date, this.comment = r.comment, this.unixPermissions = r.unixPermissions, this.dosPermissions = r.dosPermissions, this._data = t, this._dataBinary = r.binary, this.options = {
-                                    compression: r.compression,
-                                    compressionOptions: r.compressionOptions
-                                }
-                            }
-                            var s = e("./stream/StreamHelper"),
-                                i = e("./stream/DataWorker"),
-                                a = e("./utf8"),
-                                o = e("./compressedObject"),
-                                h = e("./stream/GenericWorker");
-                            n.prototype = {
-                                internalStream: function(e) {
-                                    var t = null,
-                                        r = "string";
-                                    try {
-                                        if (!e) throw new Error("No output type specified.");
-                                        var n = "string" === (r = e.toLowerCase()) || "text" === r;
-                                        "binarystring" !== r && "text" !== r || (r = "string"), t = this._decompressWorker();
-                                        var i = !this._dataBinary;
-                                        i && !n && (t = t.pipe(new a.Utf8EncodeWorker)), !i && n && (t = t.pipe(new a.Utf8DecodeWorker))
-                                    } catch (e) {
-                                        (t = new h("error")).error(e)
-                                    }
-                                    return new s(t, r, "")
-                                },
-                                async: function(e, t) {
-                                    return this.internalStream(e).accumulate(t)
-                                },
-                                nodeStream: function(e, t) {
-                                    return this.internalStream(e || "nodebuffer").toNodejsStream(t)
-                                },
-                                _compressWorker: function(e, t) {
-                                    if (this._data instanceof o && this._data.compression.magic === e.magic) return this._data.getCompressedWorker();
-                                    var r = this._decompressWorker();
-                                    return this._dataBinary || (r = r.pipe(new a.Utf8EncodeWorker)), o.createWorkerFrom(r, e, t)
-                                },
-                                _decompressWorker: function() {
-                                    return this._data instanceof o ? this._data.getContentWorker() : this._data instanceof h ? this._data : new i(this._data)
-                                }
-                            };
-                            for (var u = ["asText", "asBinary", "asNodeBuffer", "asUint8Array", "asArrayBuffer"], l = function() {
-                                    throw new Error("This method has been removed in JSZip 3.0, please check the upgrade guide.")
-                                }, f = 0; f < u.length; f++) n.prototype[u[f]] = l;
-                            t.exports = n
-                        }, {
-                            "./compressedObject": 2,
-                            "./stream/DataWorker": 27,
-                            "./stream/GenericWorker": 28,
-                            "./stream/StreamHelper": 29,
-                            "./utf8": 31
-                        }],
-                        36: [function(e, l, t) {
-                            (function(t) {
-                                "use strict";
-                                var r, n, e = t.MutationObserver || t.WebKitMutationObserver;
-                                if (e) {
-                                    var i = 0,
-                                        s = new e(u),
-                                        a = t.document.createTextNode("");
-                                    s.observe(a, {
-                                        characterData: !0
-                                    }), r = function() {
-                                        a.data = i = ++i % 2
-                                    }
-                                } else if (t.setImmediate || void 0 === t.MessageChannel) r = "document" in t && "onreadystatechange" in t.document.createElement("script") ? function() {
-                                    var e = t.document.createElement("script");
-                                    e.onreadystatechange = function() {
-                                        u(), e.onreadystatechange = null, e.parentNode.removeChild(e), e = null
-                                    }, t.document.documentElement.appendChild(e)
-                                } : function() {
-                                    setTimeout(u, 0)
-                                };
-                                else {
-                                    var o = new t.MessageChannel;
-                                    o.port1.onmessage = u, r = function() {
-                                        o.port2.postMessage(0)
-                                    }
-                                }
-                                var h = [];
+                        function n(e) {
+                            r || (r = !0, s.reject(t, e))
+                        }
 
-                                function u() {
-                                    var e, t;
-                                    n = !0;
-                                    for (var r = h.length; r;) {
-                                        for (t = h, h = [], e = -1; ++e < r;) t[e]();
-                                        r = h.length
-                                    }
-                                    n = !1
-                                }
-                                l.exports = function(e) {
-                                    1 !== h.push(e) || n || r()
-                                }
-                            }).call(this, "undefined" != typeof __webpack_require__.g ? __webpack_require__.g : "undefined" != typeof self ? self : "undefined" != typeof window ? window : {})
-                        }, {}],
-                        37: [function(e, t, r) {
-                            "use strict";
-                            var i = e("immediate");
+                        function i(e) {
+                            r || (r = !0, s.resolve(t, e))
+                        }
+                        var a = p((function() {
+                            e(i, n)
+                        }));
+                        "error" === a.status && n(a.value)
+                    }
 
-                            function u() {}
-                            var l = {},
-                                s = ["REJECTED"],
-                                a = ["FULFILLED"],
-                                n = ["PENDING"];
+                    function p(t, e) {
+                        var r = {};
+                        try {
+                            r.value = t(e), r.status = "success"
+                        } catch (t) {
+                            r.status = "error", r.value = t
+                        }
+                        return r
+                    }(e.exports = u).prototype.finally = function(t) {
+                        if ("function" != typeof t) return this;
+                        var e = this.constructor;
+                        return this.then((function(r) {
+                            return e.resolve(t()).then((function() {
+                                return r
+                            }))
+                        }), (function(r) {
+                            return e.resolve(t()).then((function() {
+                                throw r
+                            }))
+                        }))
+                    }, u.prototype.catch = function(t) {
+                        return this.then(null, t)
+                    }, u.prototype.then = function(t, e) {
+                        if ("function" != typeof t && this.state === o || "function" != typeof e && this.state === a) return this;
+                        var r = new this.constructor(i);
+                        return this.state !== h ? f(r, this.state === o ? t : e, this.outcome) : this.queue.push(new l(r, t, e)), r
+                    }, l.prototype.callFulfilled = function(t) {
+                        s.resolve(this.promise, t)
+                    }, l.prototype.otherCallFulfilled = function(t) {
+                        f(this.promise, this.onFulfilled, t)
+                    }, l.prototype.callRejected = function(t) {
+                        s.reject(this.promise, t)
+                    }, l.prototype.otherCallRejected = function(t) {
+                        f(this.promise, this.onRejected, t)
+                    }, s.resolve = function(t, e) {
+                        var r = p(c, e);
+                        if ("error" === r.status) return s.reject(t, r.value);
+                        var n = r.value;
+                        if (n) d(t, n);
+                        else {
+                            t.state = o, t.outcome = e;
+                            for (var i = -1, a = t.queue.length; ++i < a;) t.queue[i].callFulfilled(e)
+                        }
+                        return t
+                    }, s.reject = function(t, e) {
+                        t.state = a, t.outcome = e;
+                        for (var r = -1, n = t.queue.length; ++r < n;) t.queue[r].callRejected(e);
+                        return t
+                    }, u.resolve = function(t) {
+                        return t instanceof this ? t : s.resolve(new this(i), t)
+                    }, u.reject = function(t) {
+                        var e = new this(i);
+                        return s.reject(e, t)
+                    }, u.all = function(t) {
+                        var e = this;
+                        if ("[object Array]" !== Object.prototype.toString.call(t)) return this.reject(new TypeError("must be an array"));
+                        var r = t.length,
+                            n = !1;
+                        if (!r) return this.resolve([]);
+                        for (var a = new Array(r), o = 0, h = -1, u = new this(i); ++h < r;) l(t[h], h);
+                        return u;
+
+                        function l(t, i) {
+                            e.resolve(t).then((function(t) {
+                                a[i] = t, ++o !== r || n || (n = !0, s.resolve(u, a))
+                            }), (function(t) {
+                                n || (n = !0, s.reject(u, t))
+                            }))
+                        }
+                    }, u.race = function(t) {
+                        if ("[object Array]" !== Object.prototype.toString.call(t)) return this.reject(new TypeError("must be an array"));
+                        var e = t.length,
+                            r = !1;
+                        if (!e) return this.resolve([]);
+                        for (var n, a = -1, o = new this(i); ++a < e;) n = t[a], this.resolve(n).then((function(t) {
+                            r || (r = !0, s.resolve(o, t))
+                        }), (function(t) {
+                            r || (r = !0, s.reject(o, t))
+                        }));
+                        return o
+                    }
+                }, {
+                    immediate: 36
+                }],
+                38: [function(t, e, r) {
+                    "use strict";
+                    var n = {};
+                    (0, t("./lib/utils/common").assign)(n, t("./lib/deflate"), t("./lib/inflate"), t("./lib/zlib/constants")), e.exports = n
+                }, {
+                    "./lib/deflate": 39,
+                    "./lib/inflate": 40,
+                    "./lib/utils/common": 41,
+                    "./lib/zlib/constants": 44
+                }],
+                39: [function(t, e, r) {
+                    "use strict";
+                    var n = t("./zlib/deflate"),
+                        i = t("./utils/common"),
+                        s = t("./utils/strings"),
+                        a = t("./zlib/messages"),
+                        o = t("./zlib/zstream"),
+                        h = Object.prototype.toString;
+
+                    function u(t) {
+                        if (!(this instanceof u)) return new u(t);
+                        this.options = i.assign({
+                            level: -1,
+                            method: 8,
+                            chunkSize: 16384,
+                            windowBits: 15,
+                            memLevel: 8,
+                            strategy: 0,
+                            to: ""
+                        }, t || {});
+                        var e = this.options;
+                        e.raw && 0 < e.windowBits ? e.windowBits = -e.windowBits : e.gzip && 0 < e.windowBits && e.windowBits < 16 && (e.windowBits += 16), this.err = 0, this.msg = "", this.ended = !1, this.chunks = [], this.strm = new o, this.strm.avail_out = 0;
+                        var r = n.deflateInit2(this.strm, e.level, e.method, e.windowBits, e.memLevel, e.strategy);
+                        if (0 !== r) throw new Error(a[r]);
+                        if (e.header && n.deflateSetHeader(this.strm, e.header), e.dictionary) {
+                            var l;
+                            if (l = "string" == typeof e.dictionary ? s.string2buf(e.dictionary) : "[object ArrayBuffer]" === h.call(e.dictionary) ? new Uint8Array(e.dictionary) : e.dictionary, 0 !== (r = n.deflateSetDictionary(this.strm, l))) throw new Error(a[r]);
+                            this._dict_set = !0
+                        }
+                    }
 
-                            function o(e) {
-                                if ("function" != typeof e) throw new TypeError("resolver must be a function");
-                                this.state = n, this.queue = [], this.outcome = void 0, e !== u && d(this, e)
-                            }
+                    function l(t, e) {
+                        var r = new u(e);
+                        if (r.push(t, !0), r.err) throw r.msg || a[r.err];
+                        return r.result
+                    }
+                    u.prototype.push = function(t, e) {
+                        var r, a, o = this.strm,
+                            u = this.options.chunkSize;
+                        if (this.ended) return !1;
+                        a = e === ~~e ? e : !0 === e ? 4 : 0, "string" == typeof t ? o.input = s.string2buf(t) : "[object ArrayBuffer]" === h.call(t) ? o.input = new Uint8Array(t) : o.input = t, o.next_in = 0, o.avail_in = o.input.length;
+                        do {
+                            if (0 === o.avail_out && (o.output = new i.Buf8(u), o.next_out = 0, o.avail_out = u), 1 !== (r = n.deflate(o, a)) && 0 !== r) return this.onEnd(r), !(this.ended = !0);
+                            0 !== o.avail_out && (0 !== o.avail_in || 4 !== a && 2 !== a) || ("string" === this.options.to ? this.onData(s.buf2binstring(i.shrinkBuf(o.output, o.next_out))) : this.onData(i.shrinkBuf(o.output, o.next_out)))
+                        } while ((0 < o.avail_in || 0 === o.avail_out) && 1 !== r);
+                        return 4 === a ? (r = n.deflateEnd(this.strm), this.onEnd(r), this.ended = !0, 0 === r) : 2 !== a || (this.onEnd(0), !(o.avail_out = 0))
+                    }, u.prototype.onData = function(t) {
+                        this.chunks.push(t)
+                    }, u.prototype.onEnd = function(t) {
+                        0 === t && ("string" === this.options.to ? this.result = this.chunks.join("") : this.result = i.flattenChunks(this.chunks)), this.chunks = [], this.err = t, this.msg = this.strm.msg
+                    }, r.Deflate = u, r.deflate = l, r.deflateRaw = function(t, e) {
+                        return (e = e || {}).raw = !0, l(t, e)
+                    }, r.gzip = function(t, e) {
+                        return (e = e || {}).gzip = !0, l(t, e)
+                    }
+                }, {
+                    "./utils/common": 41,
+                    "./utils/strings": 42,
+                    "./zlib/deflate": 46,
+                    "./zlib/messages": 51,
+                    "./zlib/zstream": 53
+                }],
+                40: [function(t, e, r) {
+                    "use strict";
+                    var n = t("./zlib/inflate"),
+                        i = t("./utils/common"),
+                        s = t("./utils/strings"),
+                        a = t("./zlib/constants"),
+                        o = t("./zlib/messages"),
+                        h = t("./zlib/zstream"),
+                        u = t("./zlib/gzheader"),
+                        l = Object.prototype.toString;
+
+                    function f(t) {
+                        if (!(this instanceof f)) return new f(t);
+                        this.options = i.assign({
+                            chunkSize: 16384,
+                            windowBits: 0,
+                            to: ""
+                        }, t || {});
+                        var e = this.options;
+                        e.raw && 0 <= e.windowBits && e.windowBits < 16 && (e.windowBits = -e.windowBits, 0 === e.windowBits && (e.windowBits = -15)), !(0 <= e.windowBits && e.windowBits < 16) || t && t.windowBits || (e.windowBits += 32), 15 < e.windowBits && e.windowBits < 48 && 0 == (15 & e.windowBits) && (e.windowBits |= 15), this.err = 0, this.msg = "", this.ended = !1, this.chunks = [], this.strm = new h, this.strm.avail_out = 0;
+                        var r = n.inflateInit2(this.strm, e.windowBits);
+                        if (r !== a.Z_OK) throw new Error(o[r]);
+                        this.header = new u, n.inflateGetHeader(this.strm, this.header)
+                    }
 
-                            function h(e, t, r) {
-                                this.promise = e, "function" == typeof t && (this.onFulfilled = t, this.callFulfilled = this.otherCallFulfilled), "function" == typeof r && (this.onRejected = r, this.callRejected = this.otherCallRejected)
+                    function c(t, e) {
+                        var r = new f(e);
+                        if (r.push(t, !0), r.err) throw r.msg || o[r.err];
+                        return r.result
+                    }
+                    f.prototype.push = function(t, e) {
+                        var r, o, h, u, f, c, d = this.strm,
+                            p = this.options.chunkSize,
+                            m = this.options.dictionary,
+                            _ = !1;
+                        if (this.ended) return !1;
+                        o = e === ~~e ? e : !0 === e ? a.Z_FINISH : a.Z_NO_FLUSH, "string" == typeof t ? d.input = s.binstring2buf(t) : "[object ArrayBuffer]" === l.call(t) ? d.input = new Uint8Array(t) : d.input = t, d.next_in = 0, d.avail_in = d.input.length;
+                        do {
+                            if (0 === d.avail_out && (d.output = new i.Buf8(p), d.next_out = 0, d.avail_out = p), (r = n.inflate(d, a.Z_NO_FLUSH)) === a.Z_NEED_DICT && m && (c = "string" == typeof m ? s.string2buf(m) : "[object ArrayBuffer]" === l.call(m) ? new Uint8Array(m) : m, r = n.inflateSetDictionary(this.strm, c)), r === a.Z_BUF_ERROR && !0 === _ && (r = a.Z_OK, _ = !1), r !== a.Z_STREAM_END && r !== a.Z_OK) return this.onEnd(r), !(this.ended = !0);
+                            d.next_out && (0 !== d.avail_out && r !== a.Z_STREAM_END && (0 !== d.avail_in || o !== a.Z_FINISH && o !== a.Z_SYNC_FLUSH) || ("string" === this.options.to ? (h = s.utf8border(d.output, d.next_out), u = d.next_out - h, f = s.buf2string(d.output, h), d.next_out = u, d.avail_out = p - u, u && i.arraySet(d.output, d.output, h, u, 0), this.onData(f)) : this.onData(i.shrinkBuf(d.output, d.next_out)))), 0 === d.avail_in && 0 === d.avail_out && (_ = !0)
+                        } while ((0 < d.avail_in || 0 === d.avail_out) && r !== a.Z_STREAM_END);
+                        return r === a.Z_STREAM_END && (o = a.Z_FINISH), o === a.Z_FINISH ? (r = n.inflateEnd(this.strm), this.onEnd(r), this.ended = !0, r === a.Z_OK) : o !== a.Z_SYNC_FLUSH || (this.onEnd(a.Z_OK), !(d.avail_out = 0))
+                    }, f.prototype.onData = function(t) {
+                        this.chunks.push(t)
+                    }, f.prototype.onEnd = function(t) {
+                        t === a.Z_OK && ("string" === this.options.to ? this.result = this.chunks.join("") : this.result = i.flattenChunks(this.chunks)), this.chunks = [], this.err = t, this.msg = this.strm.msg
+                    }, r.Inflate = f, r.inflate = c, r.inflateRaw = function(t, e) {
+                        return (e = e || {}).raw = !0, c(t, e)
+                    }, r.ungzip = c
+                }, {
+                    "./utils/common": 41,
+                    "./utils/strings": 42,
+                    "./zlib/constants": 44,
+                    "./zlib/gzheader": 47,
+                    "./zlib/inflate": 49,
+                    "./zlib/messages": 51,
+                    "./zlib/zstream": 53
+                }],
+                41: [function(t, e, r) {
+                    "use strict";
+                    var n = "undefined" != typeof Uint8Array && "undefined" != typeof Uint16Array && "undefined" != typeof Int32Array;
+                    r.assign = function(t) {
+                        for (var e = Array.prototype.slice.call(arguments, 1); e.length;) {
+                            var r = e.shift();
+                            if (r) {
+                                if ("object" != typeof r) throw new TypeError(r + "must be non-object");
+                                for (var n in r) r.hasOwnProperty(n) && (t[n] = r[n])
                             }
+                        }
+                        return t
+                    }, r.shrinkBuf = function(t, e) {
+                        return t.length === e ? t : t.subarray ? t.subarray(0, e) : (t.length = e, t)
+                    };
+                    var i = {
+                            arraySet: function(t, e, r, n, i) {
+                                if (e.subarray && t.subarray) t.set(e.subarray(r, r + n), i);
+                                else
+                                    for (var s = 0; s < n; s++) t[i + s] = e[r + s]
+                            },
+                            flattenChunks: function(t) {
+                                var e, r, n, i, s, a;
+                                for (e = n = 0, r = t.length; e < r; e++) n += t[e].length;
+                                for (a = new Uint8Array(n), e = i = 0, r = t.length; e < r; e++) s = t[e], a.set(s, i), i += s.length;
+                                return a
+                            }
+                        },
+                        s = {
+                            arraySet: function(t, e, r, n, i) {
+                                for (var s = 0; s < n; s++) t[i + s] = e[r + s]
+                            },
+                            flattenChunks: function(t) {
+                                return [].concat.apply([], t)
+                            }
+                        };
+                    r.setTyped = function(t) {
+                        t ? (r.Buf8 = Uint8Array, r.Buf16 = Uint16Array, r.Buf32 = Int32Array, r.assign(r, i)) : (r.Buf8 = Array, r.Buf16 = Array, r.Buf32 = Array, r.assign(r, s))
+                    }, r.setTyped(n)
+                }, {}],
+                42: [function(t, e, r) {
+                    "use strict";
+                    var n = t("./common"),
+                        i = !0,
+                        s = !0;
+                    try {
+                        String.fromCharCode.apply(null, [0])
+                    } catch (t) {
+                        i = !1
+                    }
+                    try {
+                        String.fromCharCode.apply(null, new Uint8Array(1))
+                    } catch (t) {
+                        s = !1
+                    }
+                    for (var a = new n.Buf8(256), o = 0; o < 256; o++) a[o] = 252 <= o ? 6 : 248 <= o ? 5 : 240 <= o ? 4 : 224 <= o ? 3 : 192 <= o ? 2 : 1;
 
-                            function f(t, r, n) {
-                                i(function() {
-                                    var e;
-                                    try {
-                                        e = r(n)
-                                    } catch (e) {
-                                        return l.reject(t, e)
-                                    }
-                                    e === t ? l.reject(t, new TypeError("Cannot resolve promise with itself")) : l.resolve(t, e)
-                                })
-                            }
+                    function h(t, e) {
+                        if (e < 65537 && (t.subarray && s || !t.subarray && i)) return String.fromCharCode.apply(null, n.shrinkBuf(t, e));
+                        for (var r = "", a = 0; a < e; a++) r += String.fromCharCode(t[a]);
+                        return r
+                    }
+                    a[254] = a[254] = 1, r.string2buf = function(t) {
+                        var e, r, i, s, a, o = t.length,
+                            h = 0;
+                        for (s = 0; s < o; s++) 55296 == (64512 & (r = t.charCodeAt(s))) && s + 1 < o && 56320 == (64512 & (i = t.charCodeAt(s + 1))) && (r = 65536 + (r - 55296 << 10) + (i - 56320), s++), h += r < 128 ? 1 : r < 2048 ? 2 : r < 65536 ? 3 : 4;
+                        for (e = new n.Buf8(h), s = a = 0; a < h; s++) 55296 == (64512 & (r = t.charCodeAt(s))) && s + 1 < o && 56320 == (64512 & (i = t.charCodeAt(s + 1))) && (r = 65536 + (r - 55296 << 10) + (i - 56320), s++), r < 128 ? e[a++] = r : (r < 2048 ? e[a++] = 192 | r >>> 6 : (r < 65536 ? e[a++] = 224 | r >>> 12 : (e[a++] = 240 | r >>> 18, e[a++] = 128 | r >>> 12 & 63), e[a++] = 128 | r >>> 6 & 63), e[a++] = 128 | 63 & r);
+                        return e
+                    }, r.buf2binstring = function(t) {
+                        return h(t, t.length)
+                    }, r.binstring2buf = function(t) {
+                        for (var e = new n.Buf8(t.length), r = 0, i = e.length; r < i; r++) e[r] = t.charCodeAt(r);
+                        return e
+                    }, r.buf2string = function(t, e) {
+                        var r, n, i, s, o = e || t.length,
+                            u = new Array(2 * o);
+                        for (r = n = 0; r < o;)
+                            if ((i = t[r++]) < 128) u[n++] = i;
+                            else if (4 < (s = a[i])) u[n++] = 65533, r += s - 1;
+                        else {
+                            for (i &= 2 === s ? 31 : 3 === s ? 15 : 7; 1 < s && r < o;) i = i << 6 | 63 & t[r++], s--;
+                            1 < s ? u[n++] = 65533 : i < 65536 ? u[n++] = i : (i -= 65536, u[n++] = 55296 | i >> 10 & 1023, u[n++] = 56320 | 1023 & i)
+                        }
+                        return h(u, n)
+                    }, r.utf8border = function(t, e) {
+                        var r;
+                        for ((e = e || t.length) > t.length && (e = t.length), r = e - 1; 0 <= r && 128 == (192 & t[r]);) r--;
+                        return r < 0 || 0 === r ? e : r + a[t[r]] > e ? r : e
+                    }
+                }, {
+                    "./common": 41
+                }],
+                43: [function(t, e, r) {
+                    "use strict";
+                    e.exports = function(t, e, r, n) {
+                        for (var i = 65535 & t | 0, s = t >>> 16 & 65535 | 0, a = 0; 0 !== r;) {
+                            for (r -= a = 2e3 < r ? 2e3 : r; s = s + (i = i + e[n++] | 0) | 0, --a;);
+                            i %= 65521, s %= 65521
+                        }
+                        return i | s << 16 | 0
+                    }
+                }, {}],
+                44: [function(t, e, r) {
+                    "use strict";
+                    e.exports = {
+                        Z_NO_FLUSH: 0,
+                        Z_PARTIAL_FLUSH: 1,
+                        Z_SYNC_FLUSH: 2,
+                        Z_FULL_FLUSH: 3,
+                        Z_FINISH: 4,
+                        Z_BLOCK: 5,
+                        Z_TREES: 6,
+                        Z_OK: 0,
+                        Z_STREAM_END: 1,
+                        Z_NEED_DICT: 2,
+                        Z_ERRNO: -1,
+                        Z_STREAM_ERROR: -2,
+                        Z_DATA_ERROR: -3,
+                        Z_BUF_ERROR: -5,
+                        Z_NO_COMPRESSION: 0,
+                        Z_BEST_SPEED: 1,
+                        Z_BEST_COMPRESSION: 9,
+                        Z_DEFAULT_COMPRESSION: -1,
+                        Z_FILTERED: 1,
+                        Z_HUFFMAN_ONLY: 2,
+                        Z_RLE: 3,
+                        Z_FIXED: 4,
+                        Z_DEFAULT_STRATEGY: 0,
+                        Z_BINARY: 0,
+                        Z_TEXT: 1,
+                        Z_UNKNOWN: 2,
+                        Z_DEFLATED: 8
+                    }
+                }, {}],
+                45: [function(t, e, r) {
+                    "use strict";
+                    var n = function() {
+                        for (var t, e = [], r = 0; r < 256; r++) {
+                            t = r;
+                            for (var n = 0; n < 8; n++) t = 1 & t ? 3988292384 ^ t >>> 1 : t >>> 1;
+                            e[r] = t
+                        }
+                        return e
+                    }();
+                    e.exports = function(t, e, r, i) {
+                        var s = n,
+                            a = i + r;
+                        t ^= -1;
+                        for (var o = i; o < a; o++) t = t >>> 8 ^ s[255 & (t ^ e[o])];
+                        return -1 ^ t
+                    }
+                }, {}],
+                46: [function(t, e, r) {
+                    "use strict";
+                    var n, i = t("../utils/common"),
+                        s = t("./trees"),
+                        a = t("./adler32"),
+                        o = t("./crc32"),
+                        h = t("./messages"),
+                        u = -2,
+                        l = 258,
+                        f = 262,
+                        c = 113;
 
-                            function c(e) {
-                                var t = e && e.then;
-                                if (e && ("object" == typeof e || "function" == typeof e) && "function" == typeof t) return function() {
-                                    t.apply(e, arguments)
-                                }
-                            }
+                    function d(t, e) {
+                        return t.msg = h[e], e
+                    }
 
-                            function d(t, e) {
-                                var r = !1;
+                    function p(t) {
+                        return (t << 1) - (4 < t ? 9 : 0)
+                    }
 
-                                function n(e) {
-                                    r || (r = !0, l.reject(t, e))
-                                }
+                    function m(t) {
+                        for (var e = t.length; 0 <= --e;) t[e] = 0
+                    }
 
-                                function i(e) {
-                                    r || (r = !0, l.resolve(t, e))
-                                }
-                                var s = p(function() {
-                                    e(i, n)
-                                });
-                                "error" === s.status && n(s.value)
-                            }
+                    function _(t) {
+                        var e = t.state,
+                            r = e.pending;
+                        r > t.avail_out && (r = t.avail_out), 0 !== r && (i.arraySet(t.output, e.pending_buf, e.pending_out, r, t.next_out), t.next_out += r, e.pending_out += r, t.total_out += r, t.avail_out -= r, e.pending -= r, 0 === e.pending && (e.pending_out = 0))
+                    }
 
-                            function p(e, t) {
-                                var r = {};
-                                try {
-                                    r.value = e(t), r.status = "success"
-                                } catch (e) {
-                                    r.status = "error", r.value = e
-                                }
-                                return r
-                            }(t.exports = o).prototype.finally = function(t) {
-                                if ("function" != typeof t) return this;
-                                var r = this.constructor;
-                                return this.then(function(e) {
-                                    return r.resolve(t()).then(function() {
-                                        return e
-                                    })
-                                }, function(e) {
-                                    return r.resolve(t()).then(function() {
-                                        throw e
-                                    })
-                                })
-                            }, o.prototype.catch = function(e) {
-                                return this.then(null, e)
-                            }, o.prototype.then = function(e, t) {
-                                if ("function" != typeof e && this.state === a || "function" != typeof t && this.state === s) return this;
-                                var r = new this.constructor(u);
-                                this.state !== n ? f(r, this.state === a ? e : t, this.outcome) : this.queue.push(new h(r, e, t));
-                                return r
-                            }, h.prototype.callFulfilled = function(e) {
-                                l.resolve(this.promise, e)
-                            }, h.prototype.otherCallFulfilled = function(e) {
-                                f(this.promise, this.onFulfilled, e)
-                            }, h.prototype.callRejected = function(e) {
-                                l.reject(this.promise, e)
-                            }, h.prototype.otherCallRejected = function(e) {
-                                f(this.promise, this.onRejected, e)
-                            }, l.resolve = function(e, t) {
-                                var r = p(c, t);
-                                if ("error" === r.status) return l.reject(e, r.value);
-                                var n = r.value;
-                                if (n) d(e, n);
-                                else {
-                                    e.state = a, e.outcome = t;
-                                    for (var i = -1, s = e.queue.length; ++i < s;) e.queue[i].callFulfilled(t)
-                                }
-                                return e
-                            }, l.reject = function(e, t) {
-                                e.state = s, e.outcome = t;
-                                for (var r = -1, n = e.queue.length; ++r < n;) e.queue[r].callRejected(t);
-                                return e
-                            }, o.resolve = function(e) {
-                                if (e instanceof this) return e;
-                                return l.resolve(new this(u), e)
-                            }, o.reject = function(e) {
-                                var t = new this(u);
-                                return l.reject(t, e)
-                            }, o.all = function(e) {
-                                var r = this;
-                                if ("[object Array]" !== Object.prototype.toString.call(e)) return this.reject(new TypeError("must be an array"));
-                                var n = e.length,
-                                    i = !1;
-                                if (!n) return this.resolve([]);
-                                var s = new Array(n),
-                                    a = 0,
-                                    t = -1,
-                                    o = new this(u);
-                                for (; ++t < n;) h(e[t], t);
-                                return o;
-
-                                function h(e, t) {
-                                    r.resolve(e).then(function(e) {
-                                        s[t] = e, ++a !== n || i || (i = !0, l.resolve(o, s))
-                                    }, function(e) {
-                                        i || (i = !0, l.reject(o, e))
-                                    })
-                                }
-                            }, o.race = function(e) {
-                                var t = this;
-                                if ("[object Array]" !== Object.prototype.toString.call(e)) return this.reject(new TypeError("must be an array"));
-                                var r = e.length,
-                                    n = !1;
-                                if (!r) return this.resolve([]);
-                                var i = -1,
-                                    s = new this(u);
-                                for (; ++i < r;) a = e[i], t.resolve(a).then(function(e) {
-                                    n || (n = !0, l.resolve(s, e))
-                                }, function(e) {
-                                    n || (n = !0, l.reject(s, e))
-                                });
-                                var a;
-                                return s
-                            }
-                        }, {
-                            immediate: 36
-                        }],
-                        38: [function(e, t, r) {
-                            "use strict";
-                            var n = {};
-                            (0, e("./lib/utils/common").assign)(n, e("./lib/deflate"), e("./lib/inflate"), e("./lib/zlib/constants")), t.exports = n
-                        }, {
-                            "./lib/deflate": 39,
-                            "./lib/inflate": 40,
-                            "./lib/utils/common": 41,
-                            "./lib/zlib/constants": 44
-                        }],
-                        39: [function(e, t, r) {
-                            "use strict";
-                            var a = e("./zlib/deflate"),
-                                o = e("./utils/common"),
-                                h = e("./utils/strings"),
-                                i = e("./zlib/messages"),
-                                s = e("./zlib/zstream"),
-                                u = Object.prototype.toString,
-                                l = 0,
-                                f = -1,
-                                c = 0,
-                                d = 8;
+                    function g(t, e) {
+                        s._tr_flush_block(t, 0 <= t.block_start ? t.block_start : -1, t.strstart - t.block_start, e), t.block_start = t.strstart, _(t.strm)
+                    }
 
-                            function p(e) {
-                                if (!(this instanceof p)) return new p(e);
-                                this.options = o.assign({
-                                    level: f,
-                                    method: d,
-                                    chunkSize: 16384,
-                                    windowBits: 15,
-                                    memLevel: 8,
-                                    strategy: c,
-                                    to: ""
-                                }, e || {});
-                                var t = this.options;
-                                t.raw && 0 < t.windowBits ? t.windowBits = -t.windowBits : t.gzip && 0 < t.windowBits && t.windowBits < 16 && (t.windowBits += 16), this.err = 0, this.msg = "", this.ended = !1, this.chunks = [], this.strm = new s, this.strm.avail_out = 0;
-                                var r = a.deflateInit2(this.strm, t.level, t.method, t.windowBits, t.memLevel, t.strategy);
-                                if (r !== l) throw new Error(i[r]);
-                                if (t.header && a.deflateSetHeader(this.strm, t.header), t.dictionary) {
-                                    var n;
-                                    if (n = "string" == typeof t.dictionary ? h.string2buf(t.dictionary) : "[object ArrayBuffer]" === u.call(t.dictionary) ? new Uint8Array(t.dictionary) : t.dictionary, (r = a.deflateSetDictionary(this.strm, n)) !== l) throw new Error(i[r]);
-                                    this._dict_set = !0
+                    function b(t, e) {
+                        t.pending_buf[t.pending++] = e
+                    }
+
+                    function v(t, e) {
+                        t.pending_buf[t.pending++] = e >>> 8 & 255, t.pending_buf[t.pending++] = 255 & e
+                    }
+
+                    function y(t, e) {
+                        var r, n, i = t.max_chain_length,
+                            s = t.strstart,
+                            a = t.prev_length,
+                            o = t.nice_match,
+                            h = t.strstart > t.w_size - f ? t.strstart - (t.w_size - f) : 0,
+                            u = t.window,
+                            c = t.w_mask,
+                            d = t.prev,
+                            p = t.strstart + l,
+                            m = u[s + a - 1],
+                            _ = u[s + a];
+                        t.prev_length >= t.good_match && (i >>= 2), o > t.lookahead && (o = t.lookahead);
+                        do {
+                            if (u[(r = e) + a] === _ && u[r + a - 1] === m && u[r] === u[s] && u[++r] === u[s + 1]) {
+                                s += 2, r++;
+                                do {} while (u[++s] === u[++r] && u[++s] === u[++r] && u[++s] === u[++r] && u[++s] === u[++r] && u[++s] === u[++r] && u[++s] === u[++r] && u[++s] === u[++r] && u[++s] === u[++r] && s < p);
+                                if (n = l - (p - s), s = p - l, a < n) {
+                                    if (t.match_start = e, o <= (a = n)) break;
+                                    m = u[s + a - 1], _ = u[s + a]
                                 }
                             }
+                        } while ((e = d[e & c]) > h && 0 != --i);
+                        return a <= t.lookahead ? a : t.lookahead
+                    }
+
+                    function w(t) {
+                        var e, r, n, s, h, u, l, c, d, p, m = t.w_size;
+                        do {
+                            if (s = t.window_size - t.lookahead - t.strstart, t.strstart >= m + (m - f)) {
+                                for (i.arraySet(t.window, t.window, m, m, 0), t.match_start -= m, t.strstart -= m, t.block_start -= m, e = r = t.hash_size; n = t.head[--e], t.head[e] = m <= n ? n - m : 0, --r;);
+                                for (e = r = m; n = t.prev[--e], t.prev[e] = m <= n ? n - m : 0, --r;);
+                                s += m
+                            }
+                            if (0 === t.strm.avail_in) break;
+                            if (u = t.strm, l = t.window, c = t.strstart + t.lookahead, p = void 0, (d = s) < (p = u.avail_in) && (p = d), r = 0 === p ? 0 : (u.avail_in -= p, i.arraySet(l, u.input, u.next_in, p, c), 1 === u.state.wrap ? u.adler = a(u.adler, l, p, c) : 2 === u.state.wrap && (u.adler = o(u.adler, l, p, c)), u.next_in += p, u.total_in += p, p), t.lookahead += r, t.lookahead + t.insert >= 3)
+                                for (h = t.strstart - t.insert, t.ins_h = t.window[h], t.ins_h = (t.ins_h << t.hash_shift ^ t.window[h + 1]) & t.hash_mask; t.insert && (t.ins_h = (t.ins_h << t.hash_shift ^ t.window[h + 3 - 1]) & t.hash_mask, t.prev[h & t.w_mask] = t.head[t.ins_h], t.head[t.ins_h] = h, h++, t.insert--, !(t.lookahead + t.insert < 3)););
+                        } while (t.lookahead < f && 0 !== t.strm.avail_in)
+                    }
+
+                    function k(t, e) {
+                        for (var r, n;;) {
+                            if (t.lookahead < f) {
+                                if (w(t), t.lookahead < f && 0 === e) return 1;
+                                if (0 === t.lookahead) break
+                            }
+                            if (r = 0, t.lookahead >= 3 && (t.ins_h = (t.ins_h << t.hash_shift ^ t.window[t.strstart + 3 - 1]) & t.hash_mask, r = t.prev[t.strstart & t.w_mask] = t.head[t.ins_h], t.head[t.ins_h] = t.strstart), 0 !== r && t.strstart - r <= t.w_size - f && (t.match_length = y(t, r)), t.match_length >= 3)
+                                if (n = s._tr_tally(t, t.strstart - t.match_start, t.match_length - 3), t.lookahead -= t.match_length, t.match_length <= t.max_lazy_match && t.lookahead >= 3) {
+                                    for (t.match_length--; t.strstart++, t.ins_h = (t.ins_h << t.hash_shift ^ t.window[t.strstart + 3 - 1]) & t.hash_mask, r = t.prev[t.strstart & t.w_mask] = t.head[t.ins_h], t.head[t.ins_h] = t.strstart, 0 != --t.match_length;);
+                                    t.strstart++
+                                } else t.strstart += t.match_length, t.match_length = 0, t.ins_h = t.window[t.strstart], t.ins_h = (t.ins_h << t.hash_shift ^ t.window[t.strstart + 1]) & t.hash_mask;
+                            else n = s._tr_tally(t, 0, t.window[t.strstart]), t.lookahead--, t.strstart++;
+                            if (n && (g(t, !1), 0 === t.strm.avail_out)) return 1
+                        }
+                        return t.insert = t.strstart < 2 ? t.strstart : 2, 4 === e ? (g(t, !0), 0 === t.strm.avail_out ? 3 : 4) : t.last_lit && (g(t, !1), 0 === t.strm.avail_out) ? 1 : 2
+                    }
+
+                    function x(t, e) {
+                        for (var r, n, i;;) {
+                            if (t.lookahead < f) {
+                                if (w(t), t.lookahead < f && 0 === e) return 1;
+                                if (0 === t.lookahead) break
+                            }
+                            if (r = 0, t.lookahead >= 3 && (t.ins_h = (t.ins_h << t.hash_shift ^ t.window[t.strstart + 3 - 1]) & t.hash_mask, r = t.prev[t.strstart & t.w_mask] = t.head[t.ins_h], t.head[t.ins_h] = t.strstart), t.prev_length = t.match_length, t.prev_match = t.match_start, t.match_length = 2, 0 !== r && t.prev_length < t.max_lazy_match && t.strstart - r <= t.w_size - f && (t.match_length = y(t, r), t.match_length <= 5 && (1 === t.strategy || 3 === t.match_length && 4096 < t.strstart - t.match_start) && (t.match_length = 2)), t.prev_length >= 3 && t.match_length <= t.prev_length) {
+                                for (i = t.strstart + t.lookahead - 3, n = s._tr_tally(t, t.strstart - 1 - t.prev_match, t.prev_length - 3), t.lookahead -= t.prev_length - 1, t.prev_length -= 2; ++t.strstart <= i && (t.ins_h = (t.ins_h << t.hash_shift ^ t.window[t.strstart + 3 - 1]) & t.hash_mask, r = t.prev[t.strstart & t.w_mask] = t.head[t.ins_h], t.head[t.ins_h] = t.strstart), 0 != --t.prev_length;);
+                                if (t.match_available = 0, t.match_length = 2, t.strstart++, n && (g(t, !1), 0 === t.strm.avail_out)) return 1
+                            } else if (t.match_available) {
+                                if ((n = s._tr_tally(t, 0, t.window[t.strstart - 1])) && g(t, !1), t.strstart++, t.lookahead--, 0 === t.strm.avail_out) return 1
+                            } else t.match_available = 1, t.strstart++, t.lookahead--
+                        }
+                        return t.match_available && (n = s._tr_tally(t, 0, t.window[t.strstart - 1]), t.match_available = 0), t.insert = t.strstart < 2 ? t.strstart : 2, 4 === e ? (g(t, !0), 0 === t.strm.avail_out ? 3 : 4) : t.last_lit && (g(t, !1), 0 === t.strm.avail_out) ? 1 : 2
+                    }
 
-                            function n(e, t) {
-                                var r = new p(t);
-                                if (r.push(e, !0), r.err) throw r.msg || i[r.err];
-                                return r.result
-                            }
-                            p.prototype.push = function(e, t) {
-                                var r, n, i = this.strm,
-                                    s = this.options.chunkSize;
-                                if (this.ended) return !1;
-                                n = t === ~~t ? t : !0 === t ? 4 : 0, "string" == typeof e ? i.input = h.string2buf(e) : "[object ArrayBuffer]" === u.call(e) ? i.input = new Uint8Array(e) : i.input = e, i.next_in = 0, i.avail_in = i.input.length;
+                    function S(t, e, r, n, i) {
+                        this.good_length = t, this.max_lazy = e, this.nice_length = r, this.max_chain = n, this.func = i
+                    }
+
+                    function z() {
+                        this.strm = null, this.status = 0, this.pending_buf = null, this.pending_buf_size = 0, this.pending_out = 0, this.pending = 0, this.wrap = 0, this.gzhead = null, this.gzindex = 0, this.method = 8, this.last_flush = -1, this.w_size = 0, this.w_bits = 0, this.w_mask = 0, this.window = null, this.window_size = 0, this.prev = null, this.head = null, this.ins_h = 0, this.hash_size = 0, this.hash_bits = 0, this.hash_mask = 0, this.hash_shift = 0, this.block_start = 0, this.match_length = 0, this.prev_match = 0, this.match_available = 0, this.strstart = 0, this.match_start = 0, this.lookahead = 0, this.prev_length = 0, this.max_chain_length = 0, this.max_lazy_match = 0, this.level = 0, this.strategy = 0, this.good_match = 0, this.nice_match = 0, this.dyn_ltree = new i.Buf16(1146), this.dyn_dtree = new i.Buf16(122), this.bl_tree = new i.Buf16(78), m(this.dyn_ltree), m(this.dyn_dtree), m(this.bl_tree), this.l_desc = null, this.d_desc = null, this.bl_desc = null, this.bl_count = new i.Buf16(16), this.heap = new i.Buf16(573), m(this.heap), this.heap_len = 0, this.heap_max = 0, this.depth = new i.Buf16(573), m(this.depth), this.l_buf = 0, this.lit_bufsize = 0, this.last_lit = 0, this.d_buf = 0, this.opt_len = 0, this.static_len = 0, this.matches = 0, this.insert = 0, this.bi_buf = 0, this.bi_valid = 0
+                    }
+
+                    function C(t) {
+                        var e;
+                        return t && t.state ? (t.total_in = t.total_out = 0, t.data_type = 2, (e = t.state).pending = 0, e.pending_out = 0, e.wrap < 0 && (e.wrap = -e.wrap), e.status = e.wrap ? 42 : c, t.adler = 2 === e.wrap ? 0 : 1, e.last_flush = 0, s._tr_init(e), 0) : d(t, u)
+                    }
+
+                    function E(t) {
+                        var e = C(t);
+                        return 0 === e && function(t) {
+                            t.window_size = 2 * t.w_size, m(t.head), t.max_lazy_match = n[t.level].max_lazy, t.good_match = n[t.level].good_length, t.nice_match = n[t.level].nice_length, t.max_chain_length = n[t.level].max_chain, t.strstart = 0, t.block_start = 0, t.lookahead = 0, t.insert = 0, t.match_length = t.prev_length = 2, t.match_available = 0, t.ins_h = 0
+                        }(t.state), e
+                    }
+
+                    function A(t, e, r, n, s, a) {
+                        if (!t) return u;
+                        var o = 1;
+                        if (-1 === e && (e = 6), n < 0 ? (o = 0, n = -n) : 15 < n && (o = 2, n -= 16), s < 1 || 9 < s || 8 !== r || n < 8 || 15 < n || e < 0 || 9 < e || a < 0 || 4 < a) return d(t, u);
+                        8 === n && (n = 9);
+                        var h = new z;
+                        return (t.state = h).strm = t, h.wrap = o, h.gzhead = null, h.w_bits = n, h.w_size = 1 << h.w_bits, h.w_mask = h.w_size - 1, h.hash_bits = s + 7, h.hash_size = 1 << h.hash_bits, h.hash_mask = h.hash_size - 1, h.hash_shift = ~~((h.hash_bits + 3 - 1) / 3), h.window = new i.Buf8(2 * h.w_size), h.head = new i.Buf16(h.hash_size), h.prev = new i.Buf16(h.w_size), h.lit_bufsize = 1 << s + 6, h.pending_buf_size = 4 * h.lit_bufsize, h.pending_buf = new i.Buf8(h.pending_buf_size), h.d_buf = 1 * h.lit_bufsize, h.l_buf = 3 * h.lit_bufsize, h.level = e, h.strategy = a, h.method = r, E(t)
+                    }
+                    n = [new S(0, 0, 0, 0, (function(t, e) {
+                        var r = 65535;
+                        for (r > t.pending_buf_size - 5 && (r = t.pending_buf_size - 5);;) {
+                            if (t.lookahead <= 1) {
+                                if (w(t), 0 === t.lookahead && 0 === e) return 1;
+                                if (0 === t.lookahead) break
+                            }
+                            t.strstart += t.lookahead, t.lookahead = 0;
+                            var n = t.block_start + r;
+                            if ((0 === t.strstart || t.strstart >= n) && (t.lookahead = t.strstart - n, t.strstart = n, g(t, !1), 0 === t.strm.avail_out)) return 1;
+                            if (t.strstart - t.block_start >= t.w_size - f && (g(t, !1), 0 === t.strm.avail_out)) return 1
+                        }
+                        return t.insert = 0, 4 === e ? (g(t, !0), 0 === t.strm.avail_out ? 3 : 4) : (t.strstart > t.block_start && (g(t, !1), t.strm.avail_out), 1)
+                    })), new S(4, 4, 8, 4, k), new S(4, 5, 16, 8, k), new S(4, 6, 32, 32, k), new S(4, 4, 16, 16, x), new S(8, 16, 32, 32, x), new S(8, 16, 128, 128, x), new S(8, 32, 128, 256, x), new S(32, 128, 258, 1024, x), new S(32, 258, 258, 4096, x)], r.deflateInit = function(t, e) {
+                        return A(t, e, 8, 15, 8, 0)
+                    }, r.deflateInit2 = A, r.deflateReset = E, r.deflateResetKeep = C, r.deflateSetHeader = function(t, e) {
+                        return t && t.state ? 2 !== t.state.wrap ? u : (t.state.gzhead = e, 0) : u
+                    }, r.deflate = function(t, e) {
+                        var r, i, a, h;
+                        if (!t || !t.state || 5 < e || e < 0) return t ? d(t, u) : u;
+                        if (i = t.state, !t.output || !t.input && 0 !== t.avail_in || 666 === i.status && 4 !== e) return d(t, 0 === t.avail_out ? -5 : u);
+                        if (i.strm = t, r = i.last_flush, i.last_flush = e, 42 === i.status)
+                            if (2 === i.wrap) t.adler = 0, b(i, 31), b(i, 139), b(i, 8), i.gzhead ? (b(i, (i.gzhead.text ? 1 : 0) + (i.gzhead.hcrc ? 2 : 0) + (i.gzhead.extra ? 4 : 0) + (i.gzhead.name ? 8 : 0) + (i.gzhead.comment ? 16 : 0)), b(i, 255 & i.gzhead.time), b(i, i.gzhead.time >> 8 & 255), b(i, i.gzhead.time >> 16 & 255), b(i, i.gzhead.time >> 24 & 255), b(i, 9 === i.level ? 2 : 2 <= i.strategy || i.level < 2 ? 4 : 0), b(i, 255 & i.gzhead.os), i.gzhead.extra && i.gzhead.extra.length && (b(i, 255 & i.gzhead.extra.length), b(i, i.gzhead.extra.length >> 8 & 255)), i.gzhead.hcrc && (t.adler = o(t.adler, i.pending_buf, i.pending, 0)), i.gzindex = 0, i.status = 69) : (b(i, 0), b(i, 0), b(i, 0), b(i, 0), b(i, 0), b(i, 9 === i.level ? 2 : 2 <= i.strategy || i.level < 2 ? 4 : 0), b(i, 3), i.status = c);
+                            else {
+                                var f = 8 + (i.w_bits - 8 << 4) << 8;
+                                f |= (2 <= i.strategy || i.level < 2 ? 0 : i.level < 6 ? 1 : 6 === i.level ? 2 : 3) << 6, 0 !== i.strstart && (f |= 32), f += 31 - f % 31, i.status = c, v(i, f), 0 !== i.strstart && (v(i, t.adler >>> 16), v(i, 65535 & t.adler)), t.adler = 1
+                            } if (69 === i.status)
+                            if (i.gzhead.extra) {
+                                for (a = i.pending; i.gzindex < (65535 & i.gzhead.extra.length) && (i.pending !== i.pending_buf_size || (i.gzhead.hcrc && i.pending > a && (t.adler = o(t.adler, i.pending_buf, i.pending - a, a)), _(t), a = i.pending, i.pending !== i.pending_buf_size));) b(i, 255 & i.gzhead.extra[i.gzindex]), i.gzindex++;
+                                i.gzhead.hcrc && i.pending > a && (t.adler = o(t.adler, i.pending_buf, i.pending - a, a)), i.gzindex === i.gzhead.extra.length && (i.gzindex = 0, i.status = 73)
+                            } else i.status = 73;
+                        if (73 === i.status)
+                            if (i.gzhead.name) {
+                                a = i.pending;
                                 do {
-                                    if (0 === i.avail_out && (i.output = new o.Buf8(s), i.next_out = 0, i.avail_out = s), 1 !== (r = a.deflate(i, n)) && r !== l) return this.onEnd(r), !(this.ended = !0);
-                                    0 !== i.avail_out && (0 !== i.avail_in || 4 !== n && 2 !== n) || ("string" === this.options.to ? this.onData(h.buf2binstring(o.shrinkBuf(i.output, i.next_out))) : this.onData(o.shrinkBuf(i.output, i.next_out)))
-                                } while ((0 < i.avail_in || 0 === i.avail_out) && 1 !== r);
-                                return 4 === n ? (r = a.deflateEnd(this.strm), this.onEnd(r), this.ended = !0, r === l) : 2 !== n || (this.onEnd(l), !(i.avail_out = 0))
-                            }, p.prototype.onData = function(e) {
-                                this.chunks.push(e)
-                            }, p.prototype.onEnd = function(e) {
-                                e === l && ("string" === this.options.to ? this.result = this.chunks.join("") : this.result = o.flattenChunks(this.chunks)), this.chunks = [], this.err = e, this.msg = this.strm.msg
-                            }, r.Deflate = p, r.deflate = n, r.deflateRaw = function(e, t) {
-                                return (t = t || {}).raw = !0, n(e, t)
-                            }, r.gzip = function(e, t) {
-                                return (t = t || {}).gzip = !0, n(e, t)
-                            }
-                        }, {
-                            "./utils/common": 41,
-                            "./utils/strings": 42,
-                            "./zlib/deflate": 46,
-                            "./zlib/messages": 51,
-                            "./zlib/zstream": 53
-                        }],
-                        40: [function(e, t, r) {
-                            "use strict";
-                            var c = e("./zlib/inflate"),
-                                d = e("./utils/common"),
-                                p = e("./utils/strings"),
-                                m = e("./zlib/constants"),
-                                n = e("./zlib/messages"),
-                                i = e("./zlib/zstream"),
-                                s = e("./zlib/gzheader"),
-                                _ = Object.prototype.toString;
-
-                            function a(e) {
-                                if (!(this instanceof a)) return new a(e);
-                                this.options = d.assign({
-                                    chunkSize: 16384,
-                                    windowBits: 0,
-                                    to: ""
-                                }, e || {});
-                                var t = this.options;
-                                t.raw && 0 <= t.windowBits && t.windowBits < 16 && (t.windowBits = -t.windowBits, 0 === t.windowBits && (t.windowBits = -15)), !(0 <= t.windowBits && t.windowBits < 16) || e && e.windowBits || (t.windowBits += 32), 15 < t.windowBits && t.windowBits < 48 && 0 == (15 & t.windowBits) && (t.windowBits |= 15), this.err = 0, this.msg = "", this.ended = !1, this.chunks = [], this.strm = new i, this.strm.avail_out = 0;
-                                var r = c.inflateInit2(this.strm, t.windowBits);
-                                if (r !== m.Z_OK) throw new Error(n[r]);
-                                this.header = new s, c.inflateGetHeader(this.strm, this.header)
-                            }
-
-                            function o(e, t) {
-                                var r = new a(t);
-                                if (r.push(e, !0), r.err) throw r.msg || n[r.err];
-                                return r.result
-                            }
-                            a.prototype.push = function(e, t) {
-                                var r, n, i, s, a, o, h = this.strm,
-                                    u = this.options.chunkSize,
-                                    l = this.options.dictionary,
-                                    f = !1;
-                                if (this.ended) return !1;
-                                n = t === ~~t ? t : !0 === t ? m.Z_FINISH : m.Z_NO_FLUSH, "string" == typeof e ? h.input = p.binstring2buf(e) : "[object ArrayBuffer]" === _.call(e) ? h.input = new Uint8Array(e) : h.input = e, h.next_in = 0, h.avail_in = h.input.length;
+                                    if (i.pending === i.pending_buf_size && (i.gzhead.hcrc && i.pending > a && (t.adler = o(t.adler, i.pending_buf, i.pending - a, a)), _(t), a = i.pending, i.pending === i.pending_buf_size)) {
+                                        h = 1;
+                                        break
+                                    }
+                                    h = i.gzindex < i.gzhead.name.length ? 255 & i.gzhead.name.charCodeAt(i.gzindex++) : 0, b(i, h)
+                                } while (0 !== h);
+                                i.gzhead.hcrc && i.pending > a && (t.adler = o(t.adler, i.pending_buf, i.pending - a, a)), 0 === h && (i.gzindex = 0, i.status = 91)
+                            } else i.status = 91;
+                        if (91 === i.status)
+                            if (i.gzhead.comment) {
+                                a = i.pending;
                                 do {
-                                    if (0 === h.avail_out && (h.output = new d.Buf8(u), h.next_out = 0, h.avail_out = u), (r = c.inflate(h, m.Z_NO_FLUSH)) === m.Z_NEED_DICT && l && (o = "string" == typeof l ? p.string2buf(l) : "[object ArrayBuffer]" === _.call(l) ? new Uint8Array(l) : l, r = c.inflateSetDictionary(this.strm, o)), r === m.Z_BUF_ERROR && !0 === f && (r = m.Z_OK, f = !1), r !== m.Z_STREAM_END && r !== m.Z_OK) return this.onEnd(r), !(this.ended = !0);
-                                    h.next_out && (0 !== h.avail_out && r !== m.Z_STREAM_END && (0 !== h.avail_in || n !== m.Z_FINISH && n !== m.Z_SYNC_FLUSH) || ("string" === this.options.to ? (i = p.utf8border(h.output, h.next_out), s = h.next_out - i, a = p.buf2string(h.output, i), h.next_out = s, h.avail_out = u - s, s && d.arraySet(h.output, h.output, i, s, 0), this.onData(a)) : this.onData(d.shrinkBuf(h.output, h.next_out)))), 0 === h.avail_in && 0 === h.avail_out && (f = !0)
-                                } while ((0 < h.avail_in || 0 === h.avail_out) && r !== m.Z_STREAM_END);
-                                return r === m.Z_STREAM_END && (n = m.Z_FINISH), n === m.Z_FINISH ? (r = c.inflateEnd(this.strm), this.onEnd(r), this.ended = !0, r === m.Z_OK) : n !== m.Z_SYNC_FLUSH || (this.onEnd(m.Z_OK), !(h.avail_out = 0))
-                            }, a.prototype.onData = function(e) {
-                                this.chunks.push(e)
-                            }, a.prototype.onEnd = function(e) {
-                                e === m.Z_OK && ("string" === this.options.to ? this.result = this.chunks.join("") : this.result = d.flattenChunks(this.chunks)), this.chunks = [], this.err = e, this.msg = this.strm.msg
-                            }, r.Inflate = a, r.inflate = o, r.inflateRaw = function(e, t) {
-                                return (t = t || {}).raw = !0, o(e, t)
-                            }, r.ungzip = o
-                        }, {
-                            "./utils/common": 41,
-                            "./utils/strings": 42,
-                            "./zlib/constants": 44,
-                            "./zlib/gzheader": 47,
-                            "./zlib/inflate": 49,
-                            "./zlib/messages": 51,
-                            "./zlib/zstream": 53
-                        }],
-                        41: [function(e, t, r) {
-                            "use strict";
-                            var n = "undefined" != typeof Uint8Array && "undefined" != typeof Uint16Array && "undefined" != typeof Int32Array;
-                            r.assign = function(e) {
-                                for (var t = Array.prototype.slice.call(arguments, 1); t.length;) {
-                                    var r = t.shift();
-                                    if (r) {
-                                        if ("object" != typeof r) throw new TypeError(r + "must be non-object");
-                                        for (var n in r) r.hasOwnProperty(n) && (e[n] = r[n])
+                                    if (i.pending === i.pending_buf_size && (i.gzhead.hcrc && i.pending > a && (t.adler = o(t.adler, i.pending_buf, i.pending - a, a)), _(t), a = i.pending, i.pending === i.pending_buf_size)) {
+                                        h = 1;
+                                        break
                                     }
+                                    h = i.gzindex < i.gzhead.comment.length ? 255 & i.gzhead.comment.charCodeAt(i.gzindex++) : 0, b(i, h)
+                                } while (0 !== h);
+                                i.gzhead.hcrc && i.pending > a && (t.adler = o(t.adler, i.pending_buf, i.pending - a, a)), 0 === h && (i.status = 103)
+                            } else i.status = 103;
+                        if (103 === i.status && (i.gzhead.hcrc ? (i.pending + 2 > i.pending_buf_size && _(t), i.pending + 2 <= i.pending_buf_size && (b(i, 255 & t.adler), b(i, t.adler >> 8 & 255), t.adler = 0, i.status = c)) : i.status = c), 0 !== i.pending) {
+                            if (_(t), 0 === t.avail_out) return i.last_flush = -1, 0
+                        } else if (0 === t.avail_in && p(e) <= p(r) && 4 !== e) return d(t, -5);
+                        if (666 === i.status && 0 !== t.avail_in) return d(t, -5);
+                        if (0 !== t.avail_in || 0 !== i.lookahead || 0 !== e && 666 !== i.status) {
+                            var y = 2 === i.strategy ? function(t, e) {
+                                for (var r;;) {
+                                    if (0 === t.lookahead && (w(t), 0 === t.lookahead)) {
+                                        if (0 === e) return 1;
+                                        break
+                                    }
+                                    if (t.match_length = 0, r = s._tr_tally(t, 0, t.window[t.strstart]), t.lookahead--, t.strstart++, r && (g(t, !1), 0 === t.strm.avail_out)) return 1
                                 }
-                                return e
-                            }, r.shrinkBuf = function(e, t) {
-                                return e.length === t ? e : e.subarray ? e.subarray(0, t) : (e.length = t, e)
-                            };
-                            var i = {
-                                    arraySet: function(e, t, r, n, i) {
-                                        if (t.subarray && e.subarray) e.set(t.subarray(r, r + n), i);
-                                        else
-                                            for (var s = 0; s < n; s++) e[i + s] = t[r + s]
-                                    },
-                                    flattenChunks: function(e) {
-                                        var t, r, n, i, s, a;
-                                        for (t = n = 0, r = e.length; t < r; t++) n += e[t].length;
-                                        for (a = new Uint8Array(n), t = i = 0, r = e.length; t < r; t++) s = e[t], a.set(s, i), i += s.length;
-                                        return a
-                                    }
-                                },
-                                s = {
-                                    arraySet: function(e, t, r, n, i) {
-                                        for (var s = 0; s < n; s++) e[i + s] = t[r + s]
-                                    },
-                                    flattenChunks: function(e) {
-                                        return [].concat.apply([], e)
-                                    }
-                                };
-                            r.setTyped = function(e) {
-                                e ? (r.Buf8 = Uint8Array, r.Buf16 = Uint16Array, r.Buf32 = Int32Array, r.assign(r, i)) : (r.Buf8 = Array, r.Buf16 = Array, r.Buf32 = Array, r.assign(r, s))
-                            }, r.setTyped(n)
-                        }, {}],
-                        42: [function(e, t, r) {
-                            "use strict";
-                            var h = e("./common"),
-                                i = !0,
-                                s = !0;
-                            try {
-                                String.fromCharCode.apply(null, [0])
-                            } catch (e) {
-                                i = !1
-                            }
-                            try {
-                                String.fromCharCode.apply(null, new Uint8Array(1))
-                            } catch (e) {
-                                s = !1
-                            }
-                            for (var u = new h.Buf8(256), n = 0; n < 256; n++) u[n] = 252 <= n ? 6 : 248 <= n ? 5 : 240 <= n ? 4 : 224 <= n ? 3 : 192 <= n ? 2 : 1;
-
-                            function l(e, t) {
-                                if (t < 65537 && (e.subarray && s || !e.subarray && i)) return String.fromCharCode.apply(null, h.shrinkBuf(e, t));
-                                for (var r = "", n = 0; n < t; n++) r += String.fromCharCode(e[n]);
-                                return r
-                            }
-                            u[254] = u[254] = 1, r.string2buf = function(e) {
-                                var t, r, n, i, s, a = e.length,
-                                    o = 0;
-                                for (i = 0; i < a; i++) 55296 == (64512 & (r = e.charCodeAt(i))) && i + 1 < a && 56320 == (64512 & (n = e.charCodeAt(i + 1))) && (r = 65536 + (r - 55296 << 10) + (n - 56320), i++), o += r < 128 ? 1 : r < 2048 ? 2 : r < 65536 ? 3 : 4;
-                                for (t = new h.Buf8(o), i = s = 0; s < o; i++) 55296 == (64512 & (r = e.charCodeAt(i))) && i + 1 < a && 56320 == (64512 & (n = e.charCodeAt(i + 1))) && (r = 65536 + (r - 55296 << 10) + (n - 56320), i++), r < 128 ? t[s++] = r : (r < 2048 ? t[s++] = 192 | r >>> 6 : (r < 65536 ? t[s++] = 224 | r >>> 12 : (t[s++] = 240 | r >>> 18, t[s++] = 128 | r >>> 12 & 63), t[s++] = 128 | r >>> 6 & 63), t[s++] = 128 | 63 & r);
-                                return t
-                            }, r.buf2binstring = function(e) {
-                                return l(e, e.length)
-                            }, r.binstring2buf = function(e) {
-                                for (var t = new h.Buf8(e.length), r = 0, n = t.length; r < n; r++) t[r] = e.charCodeAt(r);
-                                return t
-                            }, r.buf2string = function(e, t) {
-                                var r, n, i, s, a = t || e.length,
-                                    o = new Array(2 * a);
-                                for (r = n = 0; r < a;)
-                                    if ((i = e[r++]) < 128) o[n++] = i;
-                                    else if (4 < (s = u[i])) o[n++] = 65533, r += s - 1;
+                                return t.insert = 0, 4 === e ? (g(t, !0), 0 === t.strm.avail_out ? 3 : 4) : t.last_lit && (g(t, !1), 0 === t.strm.avail_out) ? 1 : 2
+                            }(i, e) : 3 === i.strategy ? function(t, e) {
+                                for (var r, n, i, a, o = t.window;;) {
+                                    if (t.lookahead <= l) {
+                                        if (w(t), t.lookahead <= l && 0 === e) return 1;
+                                        if (0 === t.lookahead) break
+                                    }
+                                    if (t.match_length = 0, t.lookahead >= 3 && 0 < t.strstart && (n = o[i = t.strstart - 1]) === o[++i] && n === o[++i] && n === o[++i]) {
+                                        a = t.strstart + l;
+                                        do {} while (n === o[++i] && n === o[++i] && n === o[++i] && n === o[++i] && n === o[++i] && n === o[++i] && n === o[++i] && n === o[++i] && i < a);
+                                        t.match_length = l - (a - i), t.match_length > t.lookahead && (t.match_length = t.lookahead)
+                                    }
+                                    if (t.match_length >= 3 ? (r = s._tr_tally(t, 1, t.match_length - 3), t.lookahead -= t.match_length, t.strstart += t.match_length, t.match_length = 0) : (r = s._tr_tally(t, 0, t.window[t.strstart]), t.lookahead--, t.strstart++), r && (g(t, !1), 0 === t.strm.avail_out)) return 1
+                                }
+                                return t.insert = 0, 4 === e ? (g(t, !0), 0 === t.strm.avail_out ? 3 : 4) : t.last_lit && (g(t, !1), 0 === t.strm.avail_out) ? 1 : 2
+                            }(i, e) : n[i.level].func(i, e);
+                            if (3 !== y && 4 !== y || (i.status = 666), 1 === y || 3 === y) return 0 === t.avail_out && (i.last_flush = -1), 0;
+                            if (2 === y && (1 === e ? s._tr_align(i) : 5 !== e && (s._tr_stored_block(i, 0, 0, !1), 3 === e && (m(i.head), 0 === i.lookahead && (i.strstart = 0, i.block_start = 0, i.insert = 0))), _(t), 0 === t.avail_out)) return i.last_flush = -1, 0
+                        }
+                        return 4 !== e ? 0 : i.wrap <= 0 ? 1 : (2 === i.wrap ? (b(i, 255 & t.adler), b(i, t.adler >> 8 & 255), b(i, t.adler >> 16 & 255), b(i, t.adler >> 24 & 255), b(i, 255 & t.total_in), b(i, t.total_in >> 8 & 255), b(i, t.total_in >> 16 & 255), b(i, t.total_in >> 24 & 255)) : (v(i, t.adler >>> 16), v(i, 65535 & t.adler)), _(t), 0 < i.wrap && (i.wrap = -i.wrap), 0 !== i.pending ? 0 : 1)
+                    }, r.deflateEnd = function(t) {
+                        var e;
+                        return t && t.state ? 42 !== (e = t.state.status) && 69 !== e && 73 !== e && 91 !== e && 103 !== e && e !== c && 666 !== e ? d(t, u) : (t.state = null, e === c ? d(t, -3) : 0) : u
+                    }, r.deflateSetDictionary = function(t, e) {
+                        var r, n, s, o, h, l, f, c, d = e.length;
+                        if (!t || !t.state) return u;
+                        if (2 === (o = (r = t.state).wrap) || 1 === o && 42 !== r.status || r.lookahead) return u;
+                        for (1 === o && (t.adler = a(t.adler, e, d, 0)), r.wrap = 0, d >= r.w_size && (0 === o && (m(r.head), r.strstart = 0, r.block_start = 0, r.insert = 0), c = new i.Buf8(r.w_size), i.arraySet(c, e, d - r.w_size, r.w_size, 0), e = c, d = r.w_size), h = t.avail_in, l = t.next_in, f = t.input, t.avail_in = d, t.next_in = 0, t.input = e, w(r); r.lookahead >= 3;) {
+                            for (n = r.strstart, s = r.lookahead - 2; r.ins_h = (r.ins_h << r.hash_shift ^ r.window[n + 3 - 1]) & r.hash_mask, r.prev[n & r.w_mask] = r.head[r.ins_h], r.head[r.ins_h] = n, n++, --s;);
+                            r.strstart = n, r.lookahead = 2, w(r)
+                        }
+                        return r.strstart += r.lookahead, r.block_start = r.strstart, r.insert = r.lookahead, r.lookahead = 0, r.match_length = r.prev_length = 2, r.match_available = 0, t.next_in = l, t.input = f, t.avail_in = h, r.wrap = o, 0
+                    }, r.deflateInfo = "pako deflate (from Nodeca project)"
+                }, {
+                    "../utils/common": 41,
+                    "./adler32": 43,
+                    "./crc32": 45,
+                    "./messages": 51,
+                    "./trees": 52
+                }],
+                47: [function(t, e, r) {
+                    "use strict";
+                    e.exports = function() {
+                        this.text = 0, this.time = 0, this.xflags = 0, this.os = 0, this.extra = null, this.extra_len = 0, this.name = "", this.comment = "", this.hcrc = 0, this.done = !1
+                    }
+                }, {}],
+                48: [function(t, e, r) {
+                    "use strict";
+                    e.exports = function(t, e) {
+                        var r, n, i, s, a, o, h, u, l, f, c, d, p, m, _, g, b, v, y, w, k, x, S, z, C;
+                        r = t.state, n = t.next_in, z = t.input, i = n + (t.avail_in - 5), s = t.next_out, C = t.output, a = s - (e - t.avail_out), o = s + (t.avail_out - 257), h = r.dmax, u = r.wsize, l = r.whave, f = r.wnext, c = r.window, d = r.hold, p = r.bits, m = r.lencode, _ = r.distcode, g = (1 << r.lenbits) - 1, b = (1 << r.distbits) - 1;
+                        t: do {
+                            p < 15 && (d += z[n++] << p, p += 8, d += z[n++] << p, p += 8), v = m[d & g];
+                            e: for (;;) {
+                                if (d >>>= y = v >>> 24, p -= y, 0 == (y = v >>> 16 & 255)) C[s++] = 65535 & v;
                                 else {
-                                    for (i &= 2 === s ? 31 : 3 === s ? 15 : 7; 1 < s && r < a;) i = i << 6 | 63 & e[r++], s--;
-                                    1 < s ? o[n++] = 65533 : i < 65536 ? o[n++] = i : (i -= 65536, o[n++] = 55296 | i >> 10 & 1023, o[n++] = 56320 | 1023 & i)
-                                }
-                                return l(o, n)
-                            }, r.utf8border = function(e, t) {
-                                var r;
-                                for ((t = t || e.length) > e.length && (t = e.length), r = t - 1; 0 <= r && 128 == (192 & e[r]);) r--;
-                                return r < 0 ? t : 0 === r ? t : r + u[e[r]] > t ? r : t
-                            }
-                        }, {
-                            "./common": 41
-                        }],
-                        43: [function(e, t, r) {
-                            "use strict";
-                            t.exports = function(e, t, r, n) {
-                                for (var i = 65535 & e | 0, s = e >>> 16 & 65535 | 0, a = 0; 0 !== r;) {
-                                    for (r -= a = 2e3 < r ? 2e3 : r; s = s + (i = i + t[n++] | 0) | 0, --a;);
-                                    i %= 65521, s %= 65521
-                                }
-                                return i | s << 16 | 0
-                            }
-                        }, {}],
-                        44: [function(e, t, r) {
-                            "use strict";
-                            t.exports = {
-                                Z_NO_FLUSH: 0,
-                                Z_PARTIAL_FLUSH: 1,
-                                Z_SYNC_FLUSH: 2,
-                                Z_FULL_FLUSH: 3,
-                                Z_FINISH: 4,
-                                Z_BLOCK: 5,
-                                Z_TREES: 6,
-                                Z_OK: 0,
-                                Z_STREAM_END: 1,
-                                Z_NEED_DICT: 2,
-                                Z_ERRNO: -1,
-                                Z_STREAM_ERROR: -2,
-                                Z_DATA_ERROR: -3,
-                                Z_BUF_ERROR: -5,
-                                Z_NO_COMPRESSION: 0,
-                                Z_BEST_SPEED: 1,
-                                Z_BEST_COMPRESSION: 9,
-                                Z_DEFAULT_COMPRESSION: -1,
-                                Z_FILTERED: 1,
-                                Z_HUFFMAN_ONLY: 2,
-                                Z_RLE: 3,
-                                Z_FIXED: 4,
-                                Z_DEFAULT_STRATEGY: 0,
-                                Z_BINARY: 0,
-                                Z_TEXT: 1,
-                                Z_UNKNOWN: 2,
-                                Z_DEFLATED: 8
-                            }
-                        }, {}],
-                        45: [function(e, t, r) {
-                            "use strict";
-                            var o = function() {
-                                for (var e, t = [], r = 0; r < 256; r++) {
-                                    e = r;
-                                    for (var n = 0; n < 8; n++) e = 1 & e ? 3988292384 ^ e >>> 1 : e >>> 1;
-                                    t[r] = e
-                                }
-                                return t
-                            }();
-                            t.exports = function(e, t, r, n) {
-                                var i = o,
-                                    s = n + r;
-                                e ^= -1;
-                                for (var a = n; a < s; a++) e = e >>> 8 ^ i[255 & (e ^ t[a])];
-                                return -1 ^ e
-                            }
-                        }, {}],
-                        46: [function(e, t, r) {
-                            "use strict";
-                            var h, c = e("../utils/common"),
-                                u = e("./trees"),
-                                d = e("./adler32"),
-                                p = e("./crc32"),
-                                n = e("./messages"),
-                                l = 0,
-                                f = 4,
-                                m = 0,
-                                _ = -2,
-                                g = -1,
-                                b = 4,
-                                i = 2,
-                                v = 8,
-                                y = 9,
-                                s = 286,
-                                a = 30,
-                                o = 19,
-                                w = 2 * s + 1,
-                                k = 15,
-                                x = 3,
-                                S = 258,
-                                z = S + x + 1,
-                                C = 42,
-                                E = 113,
-                                A = 1,
-                                I = 2,
-                                O = 3,
-                                B = 4;
-
-                            function R(e, t) {
-                                return e.msg = n[t], t
-                            }
-
-                            function T(e) {
-                                return (e << 1) - (4 < e ? 9 : 0)
-                            }
-
-                            function D(e) {
-                                for (var t = e.length; 0 <= --t;) e[t] = 0
-                            }
-
-                            function F(e) {
-                                var t = e.state,
-                                    r = t.pending;
-                                r > e.avail_out && (r = e.avail_out), 0 !== r && (c.arraySet(e.output, t.pending_buf, t.pending_out, r, e.next_out), e.next_out += r, t.pending_out += r, e.total_out += r, e.avail_out -= r, t.pending -= r, 0 === t.pending && (t.pending_out = 0))
-                            }
-
-                            function N(e, t) {
-                                u._tr_flush_block(e, 0 <= e.block_start ? e.block_start : -1, e.strstart - e.block_start, t), e.block_start = e.strstart, F(e.strm)
-                            }
-
-                            function U(e, t) {
-                                e.pending_buf[e.pending++] = t
-                            }
-
-                            function P(e, t) {
-                                e.pending_buf[e.pending++] = t >>> 8 & 255, e.pending_buf[e.pending++] = 255 & t
-                            }
-
-                            function L(e, t) {
-                                var r, n, i = e.max_chain_length,
-                                    s = e.strstart,
-                                    a = e.prev_length,
-                                    o = e.nice_match,
-                                    h = e.strstart > e.w_size - z ? e.strstart - (e.w_size - z) : 0,
-                                    u = e.window,
-                                    l = e.w_mask,
-                                    f = e.prev,
-                                    c = e.strstart + S,
-                                    d = u[s + a - 1],
-                                    p = u[s + a];
-                                e.prev_length >= e.good_match && (i >>= 2), o > e.lookahead && (o = e.lookahead);
-                                do {
-                                    if (u[(r = t) + a] === p && u[r + a - 1] === d && u[r] === u[s] && u[++r] === u[s + 1]) {
-                                        s += 2, r++;
-                                        do {} while (u[++s] === u[++r] && u[++s] === u[++r] && u[++s] === u[++r] && u[++s] === u[++r] && u[++s] === u[++r] && u[++s] === u[++r] && u[++s] === u[++r] && u[++s] === u[++r] && s < c);
-                                        if (n = S - (c - s), s = c - S, a < n) {
-                                            if (e.match_start = t, o <= (a = n)) break;
-                                            d = u[s + a - 1], p = u[s + a]
-                                        }
-                                    }
-                                } while ((t = f[t & l]) > h && 0 != --i);
-                                return a <= e.lookahead ? a : e.lookahead
-                            }
-
-                            function j(e) {
-                                var t, r, n, i, s, a, o, h, u, l, f = e.w_size;
-                                do {
-                                    if (i = e.window_size - e.lookahead - e.strstart, e.strstart >= f + (f - z)) {
-                                        for (c.arraySet(e.window, e.window, f, f, 0), e.match_start -= f, e.strstart -= f, e.block_start -= f, t = r = e.hash_size; n = e.head[--t], e.head[t] = f <= n ? n - f : 0, --r;);
-                                        for (t = r = f; n = e.prev[--t], e.prev[t] = f <= n ? n - f : 0, --r;);
-                                        i += f
-                                    }
-                                    if (0 === e.strm.avail_in) break;
-                                    if (a = e.strm, o = e.window, h = e.strstart + e.lookahead, u = i, l = void 0, l = a.avail_in, u < l && (l = u), r = 0 === l ? 0 : (a.avail_in -= l, c.arraySet(o, a.input, a.next_in, l, h), 1 === a.state.wrap ? a.adler = d(a.adler, o, l, h) : 2 === a.state.wrap && (a.adler = p(a.adler, o, l, h)), a.next_in += l, a.total_in += l, l), e.lookahead += r, e.lookahead + e.insert >= x)
-                                        for (s = e.strstart - e.insert, e.ins_h = e.window[s], e.ins_h = (e.ins_h << e.hash_shift ^ e.window[s + 1]) & e.hash_mask; e.insert && (e.ins_h = (e.ins_h << e.hash_shift ^ e.window[s + x - 1]) & e.hash_mask, e.prev[s & e.w_mask] = e.head[e.ins_h], e.head[e.ins_h] = s, s++, e.insert--, !(e.lookahead + e.insert < x)););
-                                } while (e.lookahead < z && 0 !== e.strm.avail_in)
-                            }
-
-                            function Z(e, t) {
-                                for (var r, n;;) {
-                                    if (e.lookahead < z) {
-                                        if (j(e), e.lookahead < z && t === l) return A;
-                                        if (0 === e.lookahead) break
-                                    }
-                                    if (r = 0, e.lookahead >= x && (e.ins_h = (e.ins_h << e.hash_shift ^ e.window[e.strstart + x - 1]) & e.hash_mask, r = e.prev[e.strstart & e.w_mask] = e.head[e.ins_h], e.head[e.ins_h] = e.strstart), 0 !== r && e.strstart - r <= e.w_size - z && (e.match_length = L(e, r)), e.match_length >= x)
-                                        if (n = u._tr_tally(e, e.strstart - e.match_start, e.match_length - x), e.lookahead -= e.match_length, e.match_length <= e.max_lazy_match && e.lookahead >= x) {
-                                            for (e.match_length--; e.strstart++, e.ins_h = (e.ins_h << e.hash_shift ^ e.window[e.strstart + x - 1]) & e.hash_mask, r = e.prev[e.strstart & e.w_mask] = e.head[e.ins_h], e.head[e.ins_h] = e.strstart, 0 != --e.match_length;);
-                                            e.strstart++
-                                        } else e.strstart += e.match_length, e.match_length = 0, e.ins_h = e.window[e.strstart], e.ins_h = (e.ins_h << e.hash_shift ^ e.window[e.strstart + 1]) & e.hash_mask;
-                                    else n = u._tr_tally(e, 0, e.window[e.strstart]), e.lookahead--, e.strstart++;
-                                    if (n && (N(e, !1), 0 === e.strm.avail_out)) return A
-                                }
-                                return e.insert = e.strstart < x - 1 ? e.strstart : x - 1, t === f ? (N(e, !0), 0 === e.strm.avail_out ? O : B) : e.last_lit && (N(e, !1), 0 === e.strm.avail_out) ? A : I
-                            }
-
-                            function W(e, t) {
-                                for (var r, n, i;;) {
-                                    if (e.lookahead < z) {
-                                        if (j(e), e.lookahead < z && t === l) return A;
-                                        if (0 === e.lookahead) break
-                                    }
-                                    if (r = 0, e.lookahead >= x && (e.ins_h = (e.ins_h << e.hash_shift ^ e.window[e.strstart + x - 1]) & e.hash_mask, r = e.prev[e.strstart & e.w_mask] = e.head[e.ins_h], e.head[e.ins_h] = e.strstart), e.prev_length = e.match_length, e.prev_match = e.match_start, e.match_length = x - 1, 0 !== r && e.prev_length < e.max_lazy_match && e.strstart - r <= e.w_size - z && (e.match_length = L(e, r), e.match_length <= 5 && (1 === e.strategy || e.match_length === x && 4096 < e.strstart - e.match_start) && (e.match_length = x - 1)), e.prev_length >= x && e.match_length <= e.prev_length) {
-                                        for (i = e.strstart + e.lookahead - x, n = u._tr_tally(e, e.strstart - 1 - e.prev_match, e.prev_length - x), e.lookahead -= e.prev_length - 1, e.prev_length -= 2; ++e.strstart <= i && (e.ins_h = (e.ins_h << e.hash_shift ^ e.window[e.strstart + x - 1]) & e.hash_mask, r = e.prev[e.strstart & e.w_mask] = e.head[e.ins_h], e.head[e.ins_h] = e.strstart), 0 != --e.prev_length;);
-                                        if (e.match_available = 0, e.match_length = x - 1, e.strstart++, n && (N(e, !1), 0 === e.strm.avail_out)) return A
-                                    } else if (e.match_available) {
-                                        if ((n = u._tr_tally(e, 0, e.window[e.strstart - 1])) && N(e, !1), e.strstart++, e.lookahead--, 0 === e.strm.avail_out) return A
-                                    } else e.match_available = 1, e.strstart++, e.lookahead--
-                                }
-                                return e.match_available && (n = u._tr_tally(e, 0, e.window[e.strstart - 1]), e.match_available = 0), e.insert = e.strstart < x - 1 ? e.strstart : x - 1, t === f ? (N(e, !0), 0 === e.strm.avail_out ? O : B) : e.last_lit && (N(e, !1), 0 === e.strm.avail_out) ? A : I
-                            }
-
-                            function M(e, t, r, n, i) {
-                                this.good_length = e, this.max_lazy = t, this.nice_length = r, this.max_chain = n, this.func = i
-                            }
-
-                            function H() {
-                                this.strm = null, this.status = 0, this.pending_buf = null, this.pending_buf_size = 0, this.pending_out = 0, this.pending = 0, this.wrap = 0, this.gzhead = null, this.gzindex = 0, this.method = v, this.last_flush = -1, this.w_size = 0, this.w_bits = 0, this.w_mask = 0, this.window = null, this.window_size = 0, this.prev = null, this.head = null, this.ins_h = 0, this.hash_size = 0, this.hash_bits = 0, this.hash_mask = 0, this.hash_shift = 0, this.block_start = 0, this.match_length = 0, this.prev_match = 0, this.match_available = 0, this.strstart = 0, this.match_start = 0, this.lookahead = 0, this.prev_length = 0, this.max_chain_length = 0, this.max_lazy_match = 0, this.level = 0, this.strategy = 0, this.good_match = 0, this.nice_match = 0, this.dyn_ltree = new c.Buf16(2 * w), this.dyn_dtree = new c.Buf16(2 * (2 * a + 1)), this.bl_tree = new c.Buf16(2 * (2 * o + 1)), D(this.dyn_ltree), D(this.dyn_dtree), D(this.bl_tree), this.l_desc = null, this.d_desc = null, this.bl_desc = null, this.bl_count = new c.Buf16(k + 1), this.heap = new c.Buf16(2 * s + 1), D(this.heap), this.heap_len = 0, this.heap_max = 0, this.depth = new c.Buf16(2 * s + 1), D(this.depth), this.l_buf = 0, this.lit_bufsize = 0, this.last_lit = 0, this.d_buf = 0, this.opt_len = 0, this.static_len = 0, this.matches = 0, this.insert = 0, this.bi_buf = 0, this.bi_valid = 0
-                            }
-
-                            function G(e) {
-                                var t;
-                                return e && e.state ? (e.total_in = e.total_out = 0, e.data_type = i, (t = e.state).pending = 0, t.pending_out = 0, t.wrap < 0 && (t.wrap = -t.wrap), t.status = t.wrap ? C : E, e.adler = 2 === t.wrap ? 0 : 1, t.last_flush = l, u._tr_init(t), m) : R(e, _)
-                            }
-
-                            function K(e) {
-                                var t = G(e);
-                                return t === m && function(e) {
-                                    e.window_size = 2 * e.w_size, D(e.head), e.max_lazy_match = h[e.level].max_lazy, e.good_match = h[e.level].good_length, e.nice_match = h[e.level].nice_length, e.max_chain_length = h[e.level].max_chain, e.strstart = 0, e.block_start = 0, e.lookahead = 0, e.insert = 0, e.match_length = e.prev_length = x - 1, e.match_available = 0, e.ins_h = 0
-                                }(e.state), t
-                            }
-
-                            function Y(e, t, r, n, i, s) {
-                                if (!e) return _;
-                                var a = 1;
-                                if (t === g && (t = 6), n < 0 ? (a = 0, n = -n) : 15 < n && (a = 2, n -= 16), i < 1 || y < i || r !== v || n < 8 || 15 < n || t < 0 || 9 < t || s < 0 || b < s) return R(e, _);
-                                8 === n && (n = 9);
-                                var o = new H;
-                                return (e.state = o).strm = e, o.wrap = a, o.gzhead = null, o.w_bits = n, o.w_size = 1 << o.w_bits, o.w_mask = o.w_size - 1, o.hash_bits = i + 7, o.hash_size = 1 << o.hash_bits, o.hash_mask = o.hash_size - 1, o.hash_shift = ~~((o.hash_bits + x - 1) / x), o.window = new c.Buf8(2 * o.w_size), o.head = new c.Buf16(o.hash_size), o.prev = new c.Buf16(o.w_size), o.lit_bufsize = 1 << i + 6, o.pending_buf_size = 4 * o.lit_bufsize, o.pending_buf = new c.Buf8(o.pending_buf_size), o.d_buf = 1 * o.lit_bufsize, o.l_buf = 3 * o.lit_bufsize, o.level = t, o.strategy = s, o.method = r, K(e)
-                            }
-                            h = [new M(0, 0, 0, 0, function(e, t) {
-                                var r = 65535;
-                                for (r > e.pending_buf_size - 5 && (r = e.pending_buf_size - 5);;) {
-                                    if (e.lookahead <= 1) {
-                                        if (j(e), 0 === e.lookahead && t === l) return A;
-                                        if (0 === e.lookahead) break
-                                    }
-                                    e.strstart += e.lookahead, e.lookahead = 0;
-                                    var n = e.block_start + r;
-                                    if ((0 === e.strstart || e.strstart >= n) && (e.lookahead = e.strstart - n, e.strstart = n, N(e, !1), 0 === e.strm.avail_out)) return A;
-                                    if (e.strstart - e.block_start >= e.w_size - z && (N(e, !1), 0 === e.strm.avail_out)) return A
-                                }
-                                return e.insert = 0, t === f ? (N(e, !0), 0 === e.strm.avail_out ? O : B) : (e.strstart > e.block_start && (N(e, !1), e.strm.avail_out), A)
-                            }), new M(4, 4, 8, 4, Z), new M(4, 5, 16, 8, Z), new M(4, 6, 32, 32, Z), new M(4, 4, 16, 16, W), new M(8, 16, 32, 32, W), new M(8, 16, 128, 128, W), new M(8, 32, 128, 256, W), new M(32, 128, 258, 1024, W), new M(32, 258, 258, 4096, W)], r.deflateInit = function(e, t) {
-                                return Y(e, t, v, 15, 8, 0)
-                            }, r.deflateInit2 = Y, r.deflateReset = K, r.deflateResetKeep = G, r.deflateSetHeader = function(e, t) {
-                                return e && e.state ? 2 !== e.state.wrap ? _ : (e.state.gzhead = t, m) : _
-                            }, r.deflate = function(e, t) {
-                                var r, n, i, s;
-                                if (!e || !e.state || 5 < t || t < 0) return e ? R(e, _) : _;
-                                if (n = e.state, !e.output || !e.input && 0 !== e.avail_in || 666 === n.status && t !== f) return R(e, 0 === e.avail_out ? -5 : _);
-                                if (n.strm = e, r = n.last_flush, n.last_flush = t, n.status === C)
-                                    if (2 === n.wrap) e.adler = 0, U(n, 31), U(n, 139), U(n, 8), n.gzhead ? (U(n, (n.gzhead.text ? 1 : 0) + (n.gzhead.hcrc ? 2 : 0) + (n.gzhead.extra ? 4 : 0) + (n.gzhead.name ? 8 : 0) + (n.gzhead.comment ? 16 : 0)), U(n, 255 & n.gzhead.time), U(n, n.gzhead.time >> 8 & 255), U(n, n.gzhead.time >> 16 & 255), U(n, n.gzhead.time >> 24 & 255), U(n, 9 === n.level ? 2 : 2 <= n.strategy || n.level < 2 ? 4 : 0), U(n, 255 & n.gzhead.os), n.gzhead.extra && n.gzhead.extra.length && (U(n, 255 & n.gzhead.extra.length), U(n, n.gzhead.extra.length >> 8 & 255)), n.gzhead.hcrc && (e.adler = p(e.adler, n.pending_buf, n.pending, 0)), n.gzindex = 0, n.status = 69) : (U(n, 0), U(n, 0), U(n, 0), U(n, 0), U(n, 0), U(n, 9 === n.level ? 2 : 2 <= n.strategy || n.level < 2 ? 4 : 0), U(n, 3), n.status = E);
-                                    else {
-                                        var a = v + (n.w_bits - 8 << 4) << 8;
-                                        a |= (2 <= n.strategy || n.level < 2 ? 0 : n.level < 6 ? 1 : 6 === n.level ? 2 : 3) << 6, 0 !== n.strstart && (a |= 32), a += 31 - a % 31, n.status = E, P(n, a), 0 !== n.strstart && (P(n, e.adler >>> 16), P(n, 65535 & e.adler)), e.adler = 1
-                                    } if (69 === n.status)
-                                    if (n.gzhead.extra) {
-                                        for (i = n.pending; n.gzindex < (65535 & n.gzhead.extra.length) && (n.pending !== n.pending_buf_size || (n.gzhead.hcrc && n.pending > i && (e.adler = p(e.adler, n.pending_buf, n.pending - i, i)), F(e), i = n.pending, n.pending !== n.pending_buf_size));) U(n, 255 & n.gzhead.extra[n.gzindex]), n.gzindex++;
-                                        n.gzhead.hcrc && n.pending > i && (e.adler = p(e.adler, n.pending_buf, n.pending - i, i)), n.gzindex === n.gzhead.extra.length && (n.gzindex = 0, n.status = 73)
-                                    } else n.status = 73;
-                                if (73 === n.status)
-                                    if (n.gzhead.name) {
-                                        i = n.pending;
-                                        do {
-                                            if (n.pending === n.pending_buf_size && (n.gzhead.hcrc && n.pending > i && (e.adler = p(e.adler, n.pending_buf, n.pending - i, i)), F(e), i = n.pending, n.pending === n.pending_buf_size)) {
-                                                s = 1;
-                                                break
-                                            }
-                                            s = n.gzindex < n.gzhead.name.length ? 255 & n.gzhead.name.charCodeAt(n.gzindex++) : 0, U(n, s)
-                                        } while (0 !== s);
-                                        n.gzhead.hcrc && n.pending > i && (e.adler = p(e.adler, n.pending_buf, n.pending - i, i)), 0 === s && (n.gzindex = 0, n.status = 91)
-                                    } else n.status = 91;
-                                if (91 === n.status)
-                                    if (n.gzhead.comment) {
-                                        i = n.pending;
-                                        do {
-                                            if (n.pending === n.pending_buf_size && (n.gzhead.hcrc && n.pending > i && (e.adler = p(e.adler, n.pending_buf, n.pending - i, i)), F(e), i = n.pending, n.pending === n.pending_buf_size)) {
-                                                s = 1;
-                                                break
-                                            }
-                                            s = n.gzindex < n.gzhead.comment.length ? 255 & n.gzhead.comment.charCodeAt(n.gzindex++) : 0, U(n, s)
-                                        } while (0 !== s);
-                                        n.gzhead.hcrc && n.pending > i && (e.adler = p(e.adler, n.pending_buf, n.pending - i, i)), 0 === s && (n.status = 103)
-                                    } else n.status = 103;
-                                if (103 === n.status && (n.gzhead.hcrc ? (n.pending + 2 > n.pending_buf_size && F(e), n.pending + 2 <= n.pending_buf_size && (U(n, 255 & e.adler), U(n, e.adler >> 8 & 255), e.adler = 0, n.status = E)) : n.status = E), 0 !== n.pending) {
-                                    if (F(e), 0 === e.avail_out) return n.last_flush = -1, m
-                                } else if (0 === e.avail_in && T(t) <= T(r) && t !== f) return R(e, -5);
-                                if (666 === n.status && 0 !== e.avail_in) return R(e, -5);
-                                if (0 !== e.avail_in || 0 !== n.lookahead || t !== l && 666 !== n.status) {
-                                    var o = 2 === n.strategy ? function(e, t) {
-                                        for (var r;;) {
-                                            if (0 === e.lookahead && (j(e), 0 === e.lookahead)) {
-                                                if (t === l) return A;
-                                                break
-                                            }
-                                            if (e.match_length = 0, r = u._tr_tally(e, 0, e.window[e.strstart]), e.lookahead--, e.strstart++, r && (N(e, !1), 0 === e.strm.avail_out)) return A
-                                        }
-                                        return e.insert = 0, t === f ? (N(e, !0), 0 === e.strm.avail_out ? O : B) : e.last_lit && (N(e, !1), 0 === e.strm.avail_out) ? A : I
-                                    }(n, t) : 3 === n.strategy ? function(e, t) {
-                                        for (var r, n, i, s, a = e.window;;) {
-                                            if (e.lookahead <= S) {
-                                                if (j(e), e.lookahead <= S && t === l) return A;
-                                                if (0 === e.lookahead) break
-                                            }
-                                            if (e.match_length = 0, e.lookahead >= x && 0 < e.strstart && (n = a[i = e.strstart - 1]) === a[++i] && n === a[++i] && n === a[++i]) {
-                                                s = e.strstart + S;
-                                                do {} while (n === a[++i] && n === a[++i] && n === a[++i] && n === a[++i] && n === a[++i] && n === a[++i] && n === a[++i] && n === a[++i] && i < s);
-                                                e.match_length = S - (s - i), e.match_length > e.lookahead && (e.match_length = e.lookahead)
-                                            }
-                                            if (e.match_length >= x ? (r = u._tr_tally(e, 1, e.match_length - x), e.lookahead -= e.match_length, e.strstart += e.match_length, e.match_length = 0) : (r = u._tr_tally(e, 0, e.window[e.strstart]), e.lookahead--, e.strstart++), r && (N(e, !1), 0 === e.strm.avail_out)) return A
-                                        }
-                                        return e.insert = 0, t === f ? (N(e, !0), 0 === e.strm.avail_out ? O : B) : e.last_lit && (N(e, !1), 0 === e.strm.avail_out) ? A : I
-                                    }(n, t) : h[n.level].func(n, t);
-                                    if (o !== O && o !== B || (n.status = 666), o === A || o === O) return 0 === e.avail_out && (n.last_flush = -1), m;
-                                    if (o === I && (1 === t ? u._tr_align(n) : 5 !== t && (u._tr_stored_block(n, 0, 0, !1), 3 === t && (D(n.head), 0 === n.lookahead && (n.strstart = 0, n.block_start = 0, n.insert = 0))), F(e), 0 === e.avail_out)) return n.last_flush = -1, m
-                                }
-                                return t !== f ? m : n.wrap <= 0 ? 1 : (2 === n.wrap ? (U(n, 255 & e.adler), U(n, e.adler >> 8 & 255), U(n, e.adler >> 16 & 255), U(n, e.adler >> 24 & 255), U(n, 255 & e.total_in), U(n, e.total_in >> 8 & 255), U(n, e.total_in >> 16 & 255), U(n, e.total_in >> 24 & 255)) : (P(n, e.adler >>> 16), P(n, 65535 & e.adler)), F(e), 0 < n.wrap && (n.wrap = -n.wrap), 0 !== n.pending ? m : 1)
-                            }, r.deflateEnd = function(e) {
-                                var t;
-                                return e && e.state ? (t = e.state.status) !== C && 69 !== t && 73 !== t && 91 !== t && 103 !== t && t !== E && 666 !== t ? R(e, _) : (e.state = null, t === E ? R(e, -3) : m) : _
-                            }, r.deflateSetDictionary = function(e, t) {
-                                var r, n, i, s, a, o, h, u, l = t.length;
-                                if (!e || !e.state) return _;
-                                if (2 === (s = (r = e.state).wrap) || 1 === s && r.status !== C || r.lookahead) return _;
-                                for (1 === s && (e.adler = d(e.adler, t, l, 0)), r.wrap = 0, l >= r.w_size && (0 === s && (D(r.head), r.strstart = 0, r.block_start = 0, r.insert = 0), u = new c.Buf8(r.w_size), c.arraySet(u, t, l - r.w_size, r.w_size, 0), t = u, l = r.w_size), a = e.avail_in, o = e.next_in, h = e.input, e.avail_in = l, e.next_in = 0, e.input = t, j(r); r.lookahead >= x;) {
-                                    for (n = r.strstart, i = r.lookahead - (x - 1); r.ins_h = (r.ins_h << r.hash_shift ^ r.window[n + x - 1]) & r.hash_mask, r.prev[n & r.w_mask] = r.head[r.ins_h], r.head[r.ins_h] = n, n++, --i;);
-                                    r.strstart = n, r.lookahead = x - 1, j(r)
-                                }
-                                return r.strstart += r.lookahead, r.block_start = r.strstart, r.insert = r.lookahead, r.lookahead = 0, r.match_length = r.prev_length = x - 1, r.match_available = 0, e.next_in = o, e.input = h, e.avail_in = a, r.wrap = s, m
-                            }, r.deflateInfo = "pako deflate (from Nodeca project)"
-                        }, {
-                            "../utils/common": 41,
-                            "./adler32": 43,
-                            "./crc32": 45,
-                            "./messages": 51,
-                            "./trees": 52
-                        }],
-                        47: [function(e, t, r) {
-                            "use strict";
-                            t.exports = function() {
-                                this.text = 0, this.time = 0, this.xflags = 0, this.os = 0, this.extra = null, this.extra_len = 0, this.name = "", this.comment = "", this.hcrc = 0, this.done = !1
-                            }
-                        }, {}],
-                        48: [function(e, t, r) {
-                            "use strict";
-                            t.exports = function(e, t) {
-                                var r, n, i, s, a, o, h, u, l, f, c, d, p, m, _, g, b, v, y, w, k, x, S, z, C;
-                                r = e.state, n = e.next_in, z = e.input, i = n + (e.avail_in - 5), s = e.next_out, C = e.output, a = s - (t - e.avail_out), o = s + (e.avail_out - 257), h = r.dmax, u = r.wsize, l = r.whave, f = r.wnext, c = r.window, d = r.hold, p = r.bits, m = r.lencode, _ = r.distcode, g = (1 << r.lenbits) - 1, b = (1 << r.distbits) - 1;
-                                e: do {
-                                    p < 15 && (d += z[n++] << p, p += 8, d += z[n++] << p, p += 8), v = m[d & g];
-                                    t: for (;;) {
-                                        if (d >>>= y = v >>> 24, p -= y, 0 === (y = v >>> 16 & 255)) C[s++] = 65535 & v;
-                                        else {
-                                            if (!(16 & y)) {
-                                                if (0 == (64 & y)) {
-                                                    v = m[(65535 & v) + (d & (1 << y) - 1)];
-                                                    continue t
-                                                }
-                                                if (32 & y) {
-                                                    r.mode = 12;
-                                                    break e
-                                                }
-                                                e.msg = "invalid literal/length code", r.mode = 30;
-                                                break e
-                                            }
-                                            w = 65535 & v, (y &= 15) && (p < y && (d += z[n++] << p, p += 8), w += d & (1 << y) - 1, d >>>= y, p -= y), p < 15 && (d += z[n++] << p, p += 8, d += z[n++] << p, p += 8), v = _[d & b];
-                                            r: for (;;) {
-                                                if (d >>>= y = v >>> 24, p -= y, !(16 & (y = v >>> 16 & 255))) {
-                                                    if (0 == (64 & y)) {
-                                                        v = _[(65535 & v) + (d & (1 << y) - 1)];
-                                                        continue r
-                                                    }
-                                                    e.msg = "invalid distance code", r.mode = 30;
-                                                    break e
-                                                }
-                                                if (k = 65535 & v, p < (y &= 15) && (d += z[n++] << p, (p += 8) < y && (d += z[n++] << p, p += 8)), h < (k += d & (1 << y) - 1)) {
-                                                    e.msg = "invalid distance too far back", r.mode = 30;
-                                                    break e
+                                    if (!(16 & y)) {
+                                        if (0 == (64 & y)) {
+                                            v = m[(65535 & v) + (d & (1 << y) - 1)];
+                                            continue e
+                                        }
+                                        if (32 & y) {
+                                            r.mode = 12;
+                                            break t
+                                        }
+                                        t.msg = "invalid literal/length code", r.mode = 30;
+                                        break t
+                                    }
+                                    w = 65535 & v, (y &= 15) && (p < y && (d += z[n++] << p, p += 8), w += d & (1 << y) - 1, d >>>= y, p -= y), p < 15 && (d += z[n++] << p, p += 8, d += z[n++] << p, p += 8), v = _[d & b];
+                                    r: for (;;) {
+                                        if (d >>>= y = v >>> 24, p -= y, !(16 & (y = v >>> 16 & 255))) {
+                                            if (0 == (64 & y)) {
+                                                v = _[(65535 & v) + (d & (1 << y) - 1)];
+                                                continue r
+                                            }
+                                            t.msg = "invalid distance code", r.mode = 30;
+                                            break t
+                                        }
+                                        if (k = 65535 & v, p < (y &= 15) && (d += z[n++] << p, (p += 8) < y && (d += z[n++] << p, p += 8)), h < (k += d & (1 << y) - 1)) {
+                                            t.msg = "invalid distance too far back", r.mode = 30;
+                                            break t
+                                        }
+                                        if (d >>>= y, p -= y, (y = s - a) < k) {
+                                            if (l < (y = k - y) && r.sane) {
+                                                t.msg = "invalid distance too far back", r.mode = 30;
+                                                break t
+                                            }
+                                            if (S = c, (x = 0) === f) {
+                                                if (x += u - y, y < w) {
+                                                    for (w -= y; C[s++] = c[x++], --y;);
+                                                    x = s - k, S = C
                                                 }
-                                                if (d >>>= y, p -= y, (y = s - a) < k) {
-                                                    if (l < (y = k - y) && r.sane) {
-                                                        e.msg = "invalid distance too far back", r.mode = 30;
-                                                        break e
-                                                    }
-                                                    if (S = c, (x = 0) === f) {
-                                                        if (x += u - y, y < w) {
-                                                            for (w -= y; C[s++] = c[x++], --y;);
-                                                            x = s - k, S = C
-                                                        }
-                                                    } else if (f < y) {
-                                                        if (x += u + f - y, (y -= f) < w) {
-                                                            for (w -= y; C[s++] = c[x++], --y;);
-                                                            if (x = 0, f < w) {
-                                                                for (w -= y = f; C[s++] = c[x++], --y;);
-                                                                x = s - k, S = C
-                                                            }
-                                                        }
-                                                    } else if (x += f - y, y < w) {
-                                                        for (w -= y; C[s++] = c[x++], --y;);
+                                            } else if (f < y) {
+                                                if (x += u + f - y, (y -= f) < w) {
+                                                    for (w -= y; C[s++] = c[x++], --y;);
+                                                    if (x = 0, f < w) {
+                                                        for (w -= y = f; C[s++] = c[x++], --y;);
                                                         x = s - k, S = C
                                                     }
-                                                    for (; 2 < w;) C[s++] = S[x++], C[s++] = S[x++], C[s++] = S[x++], w -= 3;
-                                                    w && (C[s++] = S[x++], 1 < w && (C[s++] = S[x++]))
-                                                } else {
-                                                    for (x = s - k; C[s++] = C[x++], C[s++] = C[x++], C[s++] = C[x++], 2 < (w -= 3););
-                                                    w && (C[s++] = C[x++], 1 < w && (C[s++] = C[x++]))
                                                 }
-                                                break
-                                            }
+                                            } else if (x += f - y, y < w) {
+                                                for (w -= y; C[s++] = c[x++], --y;);
+                                                x = s - k, S = C
+                                            }
+                                            for (; 2 < w;) C[s++] = S[x++], C[s++] = S[x++], C[s++] = S[x++], w -= 3;
+                                            w && (C[s++] = S[x++], 1 < w && (C[s++] = S[x++]))
+                                        } else {
+                                            for (x = s - k; C[s++] = C[x++], C[s++] = C[x++], C[s++] = C[x++], 2 < (w -= 3););
+                                            w && (C[s++] = C[x++], 1 < w && (C[s++] = C[x++]))
                                         }
                                         break
                                     }
-                                } while (n < i && s < o);
-                                n -= w = p >> 3, d &= (1 << (p -= w << 3)) - 1, e.next_in = n, e.next_out = s, e.avail_in = n < i ? i - n + 5 : 5 - (n - i), e.avail_out = s < o ? o - s + 257 : 257 - (s - o), r.hold = d, r.bits = p
+                                }
+                                break
                             }
-                        }, {}],
-                        49: [function(e, t, r) {
-                            "use strict";
-                            var I = e("../utils/common"),
-                                O = e("./adler32"),
-                                B = e("./crc32"),
-                                R = e("./inffast"),
-                                T = e("./inftrees"),
-                                D = 1,
-                                F = 2,
-                                N = 0,
-                                U = -2,
-                                P = 1,
-                                n = 852,
-                                i = 592;
-
-                            function L(e) {
-                                return (e >>> 24 & 255) + (e >>> 8 & 65280) + ((65280 & e) << 8) + ((255 & e) << 24)
-                            }
-
-                            function s() {
-                                this.mode = 0, this.last = !1, this.wrap = 0, this.havedict = !1, this.flags = 0, this.dmax = 0, this.check = 0, this.total = 0, this.head = null, this.wbits = 0, this.wsize = 0, this.whave = 0, this.wnext = 0, this.window = null, this.hold = 0, this.bits = 0, this.length = 0, this.offset = 0, this.extra = 0, this.lencode = null, this.distcode = null, this.lenbits = 0, this.distbits = 0, this.ncode = 0, this.nlen = 0, this.ndist = 0, this.have = 0, this.next = null, this.lens = new I.Buf16(320), this.work = new I.Buf16(288), this.lendyn = null, this.distdyn = null, this.sane = 0, this.back = 0, this.was = 0
-                            }
-
-                            function a(e) {
-                                var t;
-                                return e && e.state ? (t = e.state, e.total_in = e.total_out = t.total = 0, e.msg = "", t.wrap && (e.adler = 1 & t.wrap), t.mode = P, t.last = 0, t.havedict = 0, t.dmax = 32768, t.head = null, t.hold = 0, t.bits = 0, t.lencode = t.lendyn = new I.Buf32(n), t.distcode = t.distdyn = new I.Buf32(i), t.sane = 1, t.back = -1, N) : U
-                            }
-
-                            function o(e) {
-                                var t;
-                                return e && e.state ? ((t = e.state).wsize = 0, t.whave = 0, t.wnext = 0, a(e)) : U
-                            }
-
-                            function h(e, t) {
-                                var r, n;
-                                return e && e.state ? (n = e.state, t < 0 ? (r = 0, t = -t) : (r = 1 + (t >> 4), t < 48 && (t &= 15)), t && (t < 8 || 15 < t) ? U : (null !== n.window && n.wbits !== t && (n.window = null), n.wrap = r, n.wbits = t, o(e))) : U
-                            }
-
-                            function u(e, t) {
-                                var r, n;
-                                return e ? (n = new s, (e.state = n).window = null, (r = h(e, t)) !== N && (e.state = null), r) : U
-                            }
-                            var l, f, c = !0;
-
-                            function j(e) {
-                                if (c) {
-                                    var t;
-                                    for (l = new I.Buf32(512), f = new I.Buf32(32), t = 0; t < 144;) e.lens[t++] = 8;
-                                    for (; t < 256;) e.lens[t++] = 9;
-                                    for (; t < 280;) e.lens[t++] = 7;
-                                    for (; t < 288;) e.lens[t++] = 8;
-                                    for (T(D, e.lens, 0, 288, l, 0, e.work, {
-                                            bits: 9
-                                        }), t = 0; t < 32;) e.lens[t++] = 5;
-                                    T(F, e.lens, 0, 32, f, 0, e.work, {
-                                        bits: 5
-                                    }), c = !1
-                                }
-                                e.lencode = l, e.lenbits = 9, e.distcode = f, e.distbits = 5
-                            }
-
-                            function Z(e, t, r, n) {
-                                var i, s = e.state;
-                                return null === s.window && (s.wsize = 1 << s.wbits, s.wnext = 0, s.whave = 0, s.window = new I.Buf8(s.wsize)), n >= s.wsize ? (I.arraySet(s.window, t, r - s.wsize, s.wsize, 0), s.wnext = 0, s.whave = s.wsize) : (n < (i = s.wsize - s.wnext) && (i = n), I.arraySet(s.window, t, r - n, i, s.wnext), (n -= i) ? (I.arraySet(s.window, t, r - n, n, 0), s.wnext = n, s.whave = s.wsize) : (s.wnext += i, s.wnext === s.wsize && (s.wnext = 0), s.whave < s.wsize && (s.whave += i))), 0
-                            }
-                            r.inflateReset = o, r.inflateReset2 = h, r.inflateResetKeep = a, r.inflateInit = function(e) {
-                                return u(e, 15)
-                            }, r.inflateInit2 = u, r.inflate = function(e, t) {
-                                var r, n, i, s, a, o, h, u, l, f, c, d, p, m, _, g, b, v, y, w, k, x, S, z, C = 0,
-                                    E = new I.Buf8(4),
-                                    A = [16, 17, 18, 0, 8, 7, 9, 6, 10, 5, 11, 4, 12, 3, 13, 2, 14, 1, 15];
-                                if (!e || !e.state || !e.output || !e.input && 0 !== e.avail_in) return U;
-                                12 === (r = e.state).mode && (r.mode = 13), a = e.next_out, i = e.output, h = e.avail_out, s = e.next_in, n = e.input, o = e.avail_in, u = r.hold, l = r.bits, f = o, c = h, x = N;
-                                e: for (;;) switch (r.mode) {
-                                    case P:
-                                        if (0 === r.wrap) {
-                                            r.mode = 13;
-                                            break
-                                        }
-                                        for (; l < 16;) {
-                                            if (0 === o) break e;
-                                            o--, u += n[s++] << l, l += 8
-                                        }
-                                        if (2 & r.wrap && 35615 === u) {
-                                            E[r.check = 0] = 255 & u, E[1] = u >>> 8 & 255, r.check = B(r.check, E, 2, 0), l = u = 0, r.mode = 2;
-                                            break
-                                        }
-                                        if (r.flags = 0, r.head && (r.head.done = !1), !(1 & r.wrap) || (((255 & u) << 8) + (u >> 8)) % 31) {
-                                            e.msg = "incorrect header check", r.mode = 30;
-                                            break
-                                        }
-                                        if (8 != (15 & u)) {
-                                            e.msg = "unknown compression method", r.mode = 30;
-                                            break
-                                        }
-                                        if (l -= 4, k = 8 + (15 & (u >>>= 4)), 0 === r.wbits) r.wbits = k;
-                                        else if (k > r.wbits) {
-                                            e.msg = "invalid window size", r.mode = 30;
-                                            break
-                                        }
-                                        r.dmax = 1 << k, e.adler = r.check = 1, r.mode = 512 & u ? 10 : 12, l = u = 0;
+                        } while (n < i && s < o);
+                        n -= w = p >> 3, d &= (1 << (p -= w << 3)) - 1, t.next_in = n, t.next_out = s, t.avail_in = n < i ? i - n + 5 : 5 - (n - i), t.avail_out = s < o ? o - s + 257 : 257 - (s - o), r.hold = d, r.bits = p
+                    }
+                }, {}],
+                49: [function(t, e, r) {
+                    "use strict";
+                    var n = t("../utils/common"),
+                        i = t("./adler32"),
+                        s = t("./crc32"),
+                        a = t("./inffast"),
+                        o = t("./inftrees"),
+                        h = -2;
+
+                    function u(t) {
+                        return (t >>> 24 & 255) + (t >>> 8 & 65280) + ((65280 & t) << 8) + ((255 & t) << 24)
+                    }
+
+                    function l() {
+                        this.mode = 0, this.last = !1, this.wrap = 0, this.havedict = !1, this.flags = 0, this.dmax = 0, this.check = 0, this.total = 0, this.head = null, this.wbits = 0, this.wsize = 0, this.whave = 0, this.wnext = 0, this.window = null, this.hold = 0, this.bits = 0, this.length = 0, this.offset = 0, this.extra = 0, this.lencode = null, this.distcode = null, this.lenbits = 0, this.distbits = 0, this.ncode = 0, this.nlen = 0, this.ndist = 0, this.have = 0, this.next = null, this.lens = new n.Buf16(320), this.work = new n.Buf16(288), this.lendyn = null, this.distdyn = null, this.sane = 0, this.back = 0, this.was = 0
+                    }
+
+                    function f(t) {
+                        var e;
+                        return t && t.state ? (e = t.state, t.total_in = t.total_out = e.total = 0, t.msg = "", e.wrap && (t.adler = 1 & e.wrap), e.mode = 1, e.last = 0, e.havedict = 0, e.dmax = 32768, e.head = null, e.hold = 0, e.bits = 0, e.lencode = e.lendyn = new n.Buf32(852), e.distcode = e.distdyn = new n.Buf32(592), e.sane = 1, e.back = -1, 0) : h
+                    }
+
+                    function c(t) {
+                        var e;
+                        return t && t.state ? ((e = t.state).wsize = 0, e.whave = 0, e.wnext = 0, f(t)) : h
+                    }
+
+                    function d(t, e) {
+                        var r, n;
+                        return t && t.state ? (n = t.state, e < 0 ? (r = 0, e = -e) : (r = 1 + (e >> 4), e < 48 && (e &= 15)), e && (e < 8 || 15 < e) ? h : (null !== n.window && n.wbits !== e && (n.window = null), n.wrap = r, n.wbits = e, c(t))) : h
+                    }
+
+                    function p(t, e) {
+                        var r, n;
+                        return t ? (n = new l, (t.state = n).window = null, 0 !== (r = d(t, e)) && (t.state = null), r) : h
+                    }
+                    var m, _, g = !0;
+
+                    function b(t) {
+                        if (g) {
+                            var e;
+                            for (m = new n.Buf32(512), _ = new n.Buf32(32), e = 0; e < 144;) t.lens[e++] = 8;
+                            for (; e < 256;) t.lens[e++] = 9;
+                            for (; e < 280;) t.lens[e++] = 7;
+                            for (; e < 288;) t.lens[e++] = 8;
+                            for (o(1, t.lens, 0, 288, m, 0, t.work, {
+                                    bits: 9
+                                }), e = 0; e < 32;) t.lens[e++] = 5;
+                            o(2, t.lens, 0, 32, _, 0, t.work, {
+                                bits: 5
+                            }), g = !1
+                        }
+                        t.lencode = m, t.lenbits = 9, t.distcode = _, t.distbits = 5
+                    }
+
+                    function v(t, e, r, i) {
+                        var s, a = t.state;
+                        return null === a.window && (a.wsize = 1 << a.wbits, a.wnext = 0, a.whave = 0, a.window = new n.Buf8(a.wsize)), i >= a.wsize ? (n.arraySet(a.window, e, r - a.wsize, a.wsize, 0), a.wnext = 0, a.whave = a.wsize) : (i < (s = a.wsize - a.wnext) && (s = i), n.arraySet(a.window, e, r - i, s, a.wnext), (i -= s) ? (n.arraySet(a.window, e, r - i, i, 0), a.wnext = i, a.whave = a.wsize) : (a.wnext += s, a.wnext === a.wsize && (a.wnext = 0), a.whave < a.wsize && (a.whave += s))), 0
+                    }
+                    r.inflateReset = c, r.inflateReset2 = d, r.inflateResetKeep = f, r.inflateInit = function(t) {
+                        return p(t, 15)
+                    }, r.inflateInit2 = p, r.inflate = function(t, e) {
+                        var r, l, f, c, d, p, m, _, g, y, w, k, x, S, z, C, E, A, I, O, B, T, R, D, F = 0,
+                            N = new n.Buf8(4),
+                            U = [16, 17, 18, 0, 8, 7, 9, 6, 10, 5, 11, 4, 12, 3, 13, 2, 14, 1, 15];
+                        if (!t || !t.state || !t.output || !t.input && 0 !== t.avail_in) return h;
+                        12 === (r = t.state).mode && (r.mode = 13), d = t.next_out, f = t.output, m = t.avail_out, c = t.next_in, l = t.input, p = t.avail_in, _ = r.hold, g = r.bits, y = p, w = m, T = 0;
+                        t: for (;;) switch (r.mode) {
+                            case 1:
+                                if (0 === r.wrap) {
+                                    r.mode = 13;
+                                    break
+                                }
+                                for (; g < 16;) {
+                                    if (0 === p) break t;
+                                    p--, _ += l[c++] << g, g += 8
+                                }
+                                if (2 & r.wrap && 35615 === _) {
+                                    N[r.check = 0] = 255 & _, N[1] = _ >>> 8 & 255, r.check = s(r.check, N, 2, 0), g = _ = 0, r.mode = 2;
+                                    break
+                                }
+                                if (r.flags = 0, r.head && (r.head.done = !1), !(1 & r.wrap) || (((255 & _) << 8) + (_ >> 8)) % 31) {
+                                    t.msg = "incorrect header check", r.mode = 30;
+                                    break
+                                }
+                                if (8 != (15 & _)) {
+                                    t.msg = "unknown compression method", r.mode = 30;
+                                    break
+                                }
+                                if (g -= 4, B = 8 + (15 & (_ >>>= 4)), 0 === r.wbits) r.wbits = B;
+                                else if (B > r.wbits) {
+                                    t.msg = "invalid window size", r.mode = 30;
+                                    break
+                                }
+                                r.dmax = 1 << B, t.adler = r.check = 1, r.mode = 512 & _ ? 10 : 12, g = _ = 0;
+                                break;
+                            case 2:
+                                for (; g < 16;) {
+                                    if (0 === p) break t;
+                                    p--, _ += l[c++] << g, g += 8
+                                }
+                                if (r.flags = _, 8 != (255 & r.flags)) {
+                                    t.msg = "unknown compression method", r.mode = 30;
+                                    break
+                                }
+                                if (57344 & r.flags) {
+                                    t.msg = "unknown header flags set", r.mode = 30;
+                                    break
+                                }
+                                r.head && (r.head.text = _ >> 8 & 1), 512 & r.flags && (N[0] = 255 & _, N[1] = _ >>> 8 & 255, r.check = s(r.check, N, 2, 0)), g = _ = 0, r.mode = 3;
+                            case 3:
+                                for (; g < 32;) {
+                                    if (0 === p) break t;
+                                    p--, _ += l[c++] << g, g += 8
+                                }
+                                r.head && (r.head.time = _), 512 & r.flags && (N[0] = 255 & _, N[1] = _ >>> 8 & 255, N[2] = _ >>> 16 & 255, N[3] = _ >>> 24 & 255, r.check = s(r.check, N, 4, 0)), g = _ = 0, r.mode = 4;
+                            case 4:
+                                for (; g < 16;) {
+                                    if (0 === p) break t;
+                                    p--, _ += l[c++] << g, g += 8
+                                }
+                                r.head && (r.head.xflags = 255 & _, r.head.os = _ >> 8), 512 & r.flags && (N[0] = 255 & _, N[1] = _ >>> 8 & 255, r.check = s(r.check, N, 2, 0)), g = _ = 0, r.mode = 5;
+                            case 5:
+                                if (1024 & r.flags) {
+                                    for (; g < 16;) {
+                                        if (0 === p) break t;
+                                        p--, _ += l[c++] << g, g += 8
+                                    }
+                                    r.length = _, r.head && (r.head.extra_len = _), 512 & r.flags && (N[0] = 255 & _, N[1] = _ >>> 8 & 255, r.check = s(r.check, N, 2, 0)), g = _ = 0
+                                } else r.head && (r.head.extra = null);
+                                r.mode = 6;
+                            case 6:
+                                if (1024 & r.flags && (p < (k = r.length) && (k = p), k && (r.head && (B = r.head.extra_len - r.length, r.head.extra || (r.head.extra = new Array(r.head.extra_len)), n.arraySet(r.head.extra, l, c, k, B)), 512 & r.flags && (r.check = s(r.check, l, k, c)), p -= k, c += k, r.length -= k), r.length)) break t;
+                                r.length = 0, r.mode = 7;
+                            case 7:
+                                if (2048 & r.flags) {
+                                    if (0 === p) break t;
+                                    for (k = 0; B = l[c + k++], r.head && B && r.length < 65536 && (r.head.name += String.fromCharCode(B)), B && k < p;);
+                                    if (512 & r.flags && (r.check = s(r.check, l, k, c)), p -= k, c += k, B) break t
+                                } else r.head && (r.head.name = null);
+                                r.length = 0, r.mode = 8;
+                            case 8:
+                                if (4096 & r.flags) {
+                                    if (0 === p) break t;
+                                    for (k = 0; B = l[c + k++], r.head && B && r.length < 65536 && (r.head.comment += String.fromCharCode(B)), B && k < p;);
+                                    if (512 & r.flags && (r.check = s(r.check, l, k, c)), p -= k, c += k, B) break t
+                                } else r.head && (r.head.comment = null);
+                                r.mode = 9;
+                            case 9:
+                                if (512 & r.flags) {
+                                    for (; g < 16;) {
+                                        if (0 === p) break t;
+                                        p--, _ += l[c++] << g, g += 8
+                                    }
+                                    if (_ !== (65535 & r.check)) {
+                                        t.msg = "header crc mismatch", r.mode = 30;
+                                        break
+                                    }
+                                    g = _ = 0
+                                }
+                                r.head && (r.head.hcrc = r.flags >> 9 & 1, r.head.done = !0), t.adler = r.check = 0, r.mode = 12;
+                                break;
+                            case 10:
+                                for (; g < 32;) {
+                                    if (0 === p) break t;
+                                    p--, _ += l[c++] << g, g += 8
+                                }
+                                t.adler = r.check = u(_), g = _ = 0, r.mode = 11;
+                            case 11:
+                                if (0 === r.havedict) return t.next_out = d, t.avail_out = m, t.next_in = c, t.avail_in = p, r.hold = _, r.bits = g, 2;
+                                t.adler = r.check = 1, r.mode = 12;
+                            case 12:
+                                if (5 === e || 6 === e) break t;
+                            case 13:
+                                if (r.last) {
+                                    _ >>>= 7 & g, g -= 7 & g, r.mode = 27;
+                                    break
+                                }
+                                for (; g < 3;) {
+                                    if (0 === p) break t;
+                                    p--, _ += l[c++] << g, g += 8
+                                }
+                                switch (r.last = 1 & _, g -= 1, 3 & (_ >>>= 1)) {
+                                    case 0:
+                                        r.mode = 14;
                                         break;
+                                    case 1:
+                                        if (b(r), r.mode = 20, 6 !== e) break;
+                                        _ >>>= 2, g -= 2;
+                                        break t;
                                     case 2:
-                                        for (; l < 16;) {
-                                            if (0 === o) break e;
-                                            o--, u += n[s++] << l, l += 8
-                                        }
-                                        if (r.flags = u, 8 != (255 & r.flags)) {
-                                            e.msg = "unknown compression method", r.mode = 30;
-                                            break
-                                        }
-                                        if (57344 & r.flags) {
-                                            e.msg = "unknown header flags set", r.mode = 30;
-                                            break
-                                        }
-                                        r.head && (r.head.text = u >> 8 & 1), 512 & r.flags && (E[0] = 255 & u, E[1] = u >>> 8 & 255, r.check = B(r.check, E, 2, 0)), l = u = 0, r.mode = 3;
-                                    case 3:
-                                        for (; l < 32;) {
-                                            if (0 === o) break e;
-                                            o--, u += n[s++] << l, l += 8
-                                        }
-                                        r.head && (r.head.time = u), 512 & r.flags && (E[0] = 255 & u, E[1] = u >>> 8 & 255, E[2] = u >>> 16 & 255, E[3] = u >>> 24 & 255, r.check = B(r.check, E, 4, 0)), l = u = 0, r.mode = 4;
-                                    case 4:
-                                        for (; l < 16;) {
-                                            if (0 === o) break e;
-                                            o--, u += n[s++] << l, l += 8
-                                        }
-                                        r.head && (r.head.xflags = 255 & u, r.head.os = u >> 8), 512 & r.flags && (E[0] = 255 & u, E[1] = u >>> 8 & 255, r.check = B(r.check, E, 2, 0)), l = u = 0, r.mode = 5;
-                                    case 5:
-                                        if (1024 & r.flags) {
-                                            for (; l < 16;) {
-                                                if (0 === o) break e;
-                                                o--, u += n[s++] << l, l += 8
-                                            }
-                                            r.length = u, r.head && (r.head.extra_len = u), 512 & r.flags && (E[0] = 255 & u, E[1] = u >>> 8 & 255, r.check = B(r.check, E, 2, 0)), l = u = 0
-                                        } else r.head && (r.head.extra = null);
-                                        r.mode = 6;
-                                    case 6:
-                                        if (1024 & r.flags && (o < (d = r.length) && (d = o), d && (r.head && (k = r.head.extra_len - r.length, r.head.extra || (r.head.extra = new Array(r.head.extra_len)), I.arraySet(r.head.extra, n, s, d, k)), 512 & r.flags && (r.check = B(r.check, n, d, s)), o -= d, s += d, r.length -= d), r.length)) break e;
-                                        r.length = 0, r.mode = 7;
-                                    case 7:
-                                        if (2048 & r.flags) {
-                                            if (0 === o) break e;
-                                            for (d = 0; k = n[s + d++], r.head && k && r.length < 65536 && (r.head.name += String.fromCharCode(k)), k && d < o;);
-                                            if (512 & r.flags && (r.check = B(r.check, n, d, s)), o -= d, s += d, k) break e
-                                        } else r.head && (r.head.name = null);
-                                        r.length = 0, r.mode = 8;
-                                    case 8:
-                                        if (4096 & r.flags) {
-                                            if (0 === o) break e;
-                                            for (d = 0; k = n[s + d++], r.head && k && r.length < 65536 && (r.head.comment += String.fromCharCode(k)), k && d < o;);
-                                            if (512 & r.flags && (r.check = B(r.check, n, d, s)), o -= d, s += d, k) break e
-                                        } else r.head && (r.head.comment = null);
-                                        r.mode = 9;
-                                    case 9:
-                                        if (512 & r.flags) {
-                                            for (; l < 16;) {
-                                                if (0 === o) break e;
-                                                o--, u += n[s++] << l, l += 8
-                                            }
-                                            if (u !== (65535 & r.check)) {
-                                                e.msg = "header crc mismatch", r.mode = 30;
-                                                break
-                                            }
-                                            l = u = 0
-                                        }
-                                        r.head && (r.head.hcrc = r.flags >> 9 & 1, r.head.done = !0), e.adler = r.check = 0, r.mode = 12;
-                                        break;
-                                    case 10:
-                                        for (; l < 32;) {
-                                            if (0 === o) break e;
-                                            o--, u += n[s++] << l, l += 8
-                                        }
-                                        e.adler = r.check = L(u), l = u = 0, r.mode = 11;
-                                    case 11:
-                                        if (0 === r.havedict) return e.next_out = a, e.avail_out = h, e.next_in = s, e.avail_in = o, r.hold = u, r.bits = l, 2;
-                                        e.adler = r.check = 1, r.mode = 12;
-                                    case 12:
-                                        if (5 === t || 6 === t) break e;
-                                    case 13:
-                                        if (r.last) {
-                                            u >>>= 7 & l, l -= 7 & l, r.mode = 27;
-                                            break
-                                        }
-                                        for (; l < 3;) {
-                                            if (0 === o) break e;
-                                            o--, u += n[s++] << l, l += 8
-                                        }
-                                        switch (r.last = 1 & u, l -= 1, 3 & (u >>>= 1)) {
-                                            case 0:
-                                                r.mode = 14;
-                                                break;
-                                            case 1:
-                                                if (j(r), r.mode = 20, 6 !== t) break;
-                                                u >>>= 2, l -= 2;
-                                                break e;
-                                            case 2:
-                                                r.mode = 17;
-                                                break;
-                                            case 3:
-                                                e.msg = "invalid block type", r.mode = 30
-                                        }
-                                        u >>>= 2, l -= 2;
-                                        break;
-                                    case 14:
-                                        for (u >>>= 7 & l, l -= 7 & l; l < 32;) {
-                                            if (0 === o) break e;
-                                            o--, u += n[s++] << l, l += 8
-                                        }
-                                        if ((65535 & u) != (u >>> 16 ^ 65535)) {
-                                            e.msg = "invalid stored block lengths", r.mode = 30;
-                                            break
-                                        }
-                                        if (r.length = 65535 & u, l = u = 0, r.mode = 15, 6 === t) break e;
-                                    case 15:
-                                        r.mode = 16;
-                                    case 16:
-                                        if (d = r.length) {
-                                            if (o < d && (d = o), h < d && (d = h), 0 === d) break e;
-                                            I.arraySet(i, n, s, d, a), o -= d, s += d, h -= d, a += d, r.length -= d;
-                                            break
-                                        }
-                                        r.mode = 12;
-                                        break;
-                                    case 17:
-                                        for (; l < 14;) {
-                                            if (0 === o) break e;
-                                            o--, u += n[s++] << l, l += 8
-                                        }
-                                        if (r.nlen = 257 + (31 & u), u >>>= 5, l -= 5, r.ndist = 1 + (31 & u), u >>>= 5, l -= 5, r.ncode = 4 + (15 & u), u >>>= 4, l -= 4, 286 < r.nlen || 30 < r.ndist) {
-                                            e.msg = "too many length or distance symbols", r.mode = 30;
-                                            break
-                                        }
-                                        r.have = 0, r.mode = 18;
-                                    case 18:
-                                        for (; r.have < r.ncode;) {
-                                            for (; l < 3;) {
-                                                if (0 === o) break e;
-                                                o--, u += n[s++] << l, l += 8
-                                            }
-                                            r.lens[A[r.have++]] = 7 & u, u >>>= 3, l -= 3
-                                        }
-                                        for (; r.have < 19;) r.lens[A[r.have++]] = 0;
-                                        if (r.lencode = r.lendyn, r.lenbits = 7, S = {
-                                                bits: r.lenbits
-                                            }, x = T(0, r.lens, 0, 19, r.lencode, 0, r.work, S), r.lenbits = S.bits, x) {
-                                            e.msg = "invalid code lengths set", r.mode = 30;
-                                            break
-                                        }
-                                        r.have = 0, r.mode = 19;
-                                    case 19:
-                                        for (; r.have < r.nlen + r.ndist;) {
-                                            for (; g = (C = r.lencode[u & (1 << r.lenbits) - 1]) >>> 16 & 255, b = 65535 & C, !((_ = C >>> 24) <= l);) {
-                                                if (0 === o) break e;
-                                                o--, u += n[s++] << l, l += 8
-                                            }
-                                            if (b < 16) u >>>= _, l -= _, r.lens[r.have++] = b;
-                                            else {
-                                                if (16 === b) {
-                                                    for (z = _ + 2; l < z;) {
-                                                        if (0 === o) break e;
-                                                        o--, u += n[s++] << l, l += 8
-                                                    }
-                                                    if (u >>>= _, l -= _, 0 === r.have) {
-                                                        e.msg = "invalid bit length repeat", r.mode = 30;
-                                                        break
-                                                    }
-                                                    k = r.lens[r.have - 1], d = 3 + (3 & u), u >>>= 2, l -= 2
-                                                } else if (17 === b) {
-                                                    for (z = _ + 3; l < z;) {
-                                                        if (0 === o) break e;
-                                                        o--, u += n[s++] << l, l += 8
-                                                    }
-                                                    l -= _, k = 0, d = 3 + (7 & (u >>>= _)), u >>>= 3, l -= 3
-                                                } else {
-                                                    for (z = _ + 7; l < z;) {
-                                                        if (0 === o) break e;
-                                                        o--, u += n[s++] << l, l += 8
-                                                    }
-                                                    l -= _, k = 0, d = 11 + (127 & (u >>>= _)), u >>>= 7, l -= 7
-                                                }
-                                                if (r.have + d > r.nlen + r.ndist) {
-                                                    e.msg = "invalid bit length repeat", r.mode = 30;
-                                                    break
-                                                }
-                                                for (; d--;) r.lens[r.have++] = k
-                                            }
-                                        }
-                                        if (30 === r.mode) break;
-                                        if (0 === r.lens[256]) {
-                                            e.msg = "invalid code -- missing end-of-block", r.mode = 30;
-                                            break
-                                        }
-                                        if (r.lenbits = 9, S = {
-                                                bits: r.lenbits
-                                            }, x = T(D, r.lens, 0, r.nlen, r.lencode, 0, r.work, S), r.lenbits = S.bits, x) {
-                                            e.msg = "invalid literal/lengths set", r.mode = 30;
-                                            break
-                                        }
-                                        if (r.distbits = 6, r.distcode = r.distdyn, S = {
-                                                bits: r.distbits
-                                            }, x = T(F, r.lens, r.nlen, r.ndist, r.distcode, 0, r.work, S), r.distbits = S.bits, x) {
-                                            e.msg = "invalid distances set", r.mode = 30;
-                                            break
-                                        }
-                                        if (r.mode = 20, 6 === t) break e;
-                                    case 20:
-                                        r.mode = 21;
-                                    case 21:
-                                        if (6 <= o && 258 <= h) {
-                                            e.next_out = a, e.avail_out = h, e.next_in = s, e.avail_in = o, r.hold = u, r.bits = l, R(e, c), a = e.next_out, i = e.output, h = e.avail_out, s = e.next_in, n = e.input, o = e.avail_in, u = r.hold, l = r.bits, 12 === r.mode && (r.back = -1);
-                                            break
-                                        }
-                                        for (r.back = 0; g = (C = r.lencode[u & (1 << r.lenbits) - 1]) >>> 16 & 255, b = 65535 & C, !((_ = C >>> 24) <= l);) {
-                                            if (0 === o) break e;
-                                            o--, u += n[s++] << l, l += 8
-                                        }
-                                        if (g && 0 == (240 & g)) {
-                                            for (v = _, y = g, w = b; g = (C = r.lencode[w + ((u & (1 << v + y) - 1) >> v)]) >>> 16 & 255, b = 65535 & C, !(v + (_ = C >>> 24) <= l);) {
-                                                if (0 === o) break e;
-                                                o--, u += n[s++] << l, l += 8
-                                            }
-                                            u >>>= v, l -= v, r.back += v
-                                        }
-                                        if (u >>>= _, l -= _, r.back += _, r.length = b, 0 === g) {
-                                            r.mode = 26;
-                                            break
-                                        }
-                                        if (32 & g) {
-                                            r.back = -1, r.mode = 12;
-                                            break
-                                        }
-                                        if (64 & g) {
-                                            e.msg = "invalid literal/length code", r.mode = 30;
-                                            break
-                                        }
-                                        r.extra = 15 & g, r.mode = 22;
-                                    case 22:
-                                        if (r.extra) {
-                                            for (z = r.extra; l < z;) {
-                                                if (0 === o) break e;
-                                                o--, u += n[s++] << l, l += 8
-                                            }
-                                            r.length += u & (1 << r.extra) - 1, u >>>= r.extra, l -= r.extra, r.back += r.extra
-                                        }
-                                        r.was = r.length, r.mode = 23;
-                                    case 23:
-                                        for (; g = (C = r.distcode[u & (1 << r.distbits) - 1]) >>> 16 & 255, b = 65535 & C, !((_ = C >>> 24) <= l);) {
-                                            if (0 === o) break e;
-                                            o--, u += n[s++] << l, l += 8
-                                        }
-                                        if (0 == (240 & g)) {
-                                            for (v = _, y = g, w = b; g = (C = r.distcode[w + ((u & (1 << v + y) - 1) >> v)]) >>> 16 & 255, b = 65535 & C, !(v + (_ = C >>> 24) <= l);) {
-                                                if (0 === o) break e;
-                                                o--, u += n[s++] << l, l += 8
-                                            }
-                                            u >>>= v, l -= v, r.back += v
-                                        }
-                                        if (u >>>= _, l -= _, r.back += _, 64 & g) {
-                                            e.msg = "invalid distance code", r.mode = 30;
-                                            break
-                                        }
-                                        r.offset = b, r.extra = 15 & g, r.mode = 24;
-                                    case 24:
-                                        if (r.extra) {
-                                            for (z = r.extra; l < z;) {
-                                                if (0 === o) break e;
-                                                o--, u += n[s++] << l, l += 8
-                                            }
-                                            r.offset += u & (1 << r.extra) - 1, u >>>= r.extra, l -= r.extra, r.back += r.extra
-                                        }
-                                        if (r.offset > r.dmax) {
-                                            e.msg = "invalid distance too far back", r.mode = 30;
-                                            break
-                                        }
-                                        r.mode = 25;
-                                    case 25:
-                                        if (0 === h) break e;
-                                        if (d = c - h, r.offset > d) {
-                                            if ((d = r.offset - d) > r.whave && r.sane) {
-                                                e.msg = "invalid distance too far back", r.mode = 30;
-                                                break
-                                            }
-                                            p = d > r.wnext ? (d -= r.wnext, r.wsize - d) : r.wnext - d, d > r.length && (d = r.length), m = r.window
-                                        } else m = i, p = a - r.offset, d = r.length;
-                                        for (h < d && (d = h), h -= d, r.length -= d; i[a++] = m[p++], --d;);
-                                        0 === r.length && (r.mode = 21);
-                                        break;
-                                    case 26:
-                                        if (0 === h) break e;
-                                        i[a++] = r.length, h--, r.mode = 21;
+                                        r.mode = 17;
                                         break;
-                                    case 27:
-                                        if (r.wrap) {
-                                            for (; l < 32;) {
-                                                if (0 === o) break e;
-                                                o--, u |= n[s++] << l, l += 8
-                                            }
-                                            if (c -= h, e.total_out += c, r.total += c, c && (e.adler = r.check = r.flags ? B(r.check, i, c, a - c) : O(r.check, i, c, a - c)), c = h, (r.flags ? u : L(u)) !== r.check) {
-                                                e.msg = "incorrect data check", r.mode = 30;
-                                                break
-                                            }
-                                            l = u = 0
-                                        }
-                                        r.mode = 28;
-                                    case 28:
-                                        if (r.wrap && r.flags) {
-                                            for (; l < 32;) {
-                                                if (0 === o) break e;
-                                                o--, u += n[s++] << l, l += 8
+                                    case 3:
+                                        t.msg = "invalid block type", r.mode = 30
+                                }
+                                _ >>>= 2, g -= 2;
+                                break;
+                            case 14:
+                                for (_ >>>= 7 & g, g -= 7 & g; g < 32;) {
+                                    if (0 === p) break t;
+                                    p--, _ += l[c++] << g, g += 8
+                                }
+                                if ((65535 & _) != (_ >>> 16 ^ 65535)) {
+                                    t.msg = "invalid stored block lengths", r.mode = 30;
+                                    break
+                                }
+                                if (r.length = 65535 & _, g = _ = 0, r.mode = 15, 6 === e) break t;
+                            case 15:
+                                r.mode = 16;
+                            case 16:
+                                if (k = r.length) {
+                                    if (p < k && (k = p), m < k && (k = m), 0 === k) break t;
+                                    n.arraySet(f, l, c, k, d), p -= k, c += k, m -= k, d += k, r.length -= k;
+                                    break
+                                }
+                                r.mode = 12;
+                                break;
+                            case 17:
+                                for (; g < 14;) {
+                                    if (0 === p) break t;
+                                    p--, _ += l[c++] << g, g += 8
+                                }
+                                if (r.nlen = 257 + (31 & _), _ >>>= 5, g -= 5, r.ndist = 1 + (31 & _), _ >>>= 5, g -= 5, r.ncode = 4 + (15 & _), _ >>>= 4, g -= 4, 286 < r.nlen || 30 < r.ndist) {
+                                    t.msg = "too many length or distance symbols", r.mode = 30;
+                                    break
+                                }
+                                r.have = 0, r.mode = 18;
+                            case 18:
+                                for (; r.have < r.ncode;) {
+                                    for (; g < 3;) {
+                                        if (0 === p) break t;
+                                        p--, _ += l[c++] << g, g += 8
+                                    }
+                                    r.lens[U[r.have++]] = 7 & _, _ >>>= 3, g -= 3
+                                }
+                                for (; r.have < 19;) r.lens[U[r.have++]] = 0;
+                                if (r.lencode = r.lendyn, r.lenbits = 7, R = {
+                                        bits: r.lenbits
+                                    }, T = o(0, r.lens, 0, 19, r.lencode, 0, r.work, R), r.lenbits = R.bits, T) {
+                                    t.msg = "invalid code lengths set", r.mode = 30;
+                                    break
+                                }
+                                r.have = 0, r.mode = 19;
+                            case 19:
+                                for (; r.have < r.nlen + r.ndist;) {
+                                    for (; C = (F = r.lencode[_ & (1 << r.lenbits) - 1]) >>> 16 & 255, E = 65535 & F, !((z = F >>> 24) <= g);) {
+                                        if (0 === p) break t;
+                                        p--, _ += l[c++] << g, g += 8
+                                    }
+                                    if (E < 16) _ >>>= z, g -= z, r.lens[r.have++] = E;
+                                    else {
+                                        if (16 === E) {
+                                            for (D = z + 2; g < D;) {
+                                                if (0 === p) break t;
+                                                p--, _ += l[c++] << g, g += 8
                                             }
-                                            if (u !== (4294967295 & r.total)) {
-                                                e.msg = "incorrect length check", r.mode = 30;
+                                            if (_ >>>= z, g -= z, 0 === r.have) {
+                                                t.msg = "invalid bit length repeat", r.mode = 30;
                                                 break
                                             }
-                                            l = u = 0
-                                        }
-                                        r.mode = 29;
-                                    case 29:
-                                        x = 1;
-                                        break e;
-                                    case 30:
-                                        x = -3;
-                                        break e;
-                                    case 31:
-                                        return -4;
-                                    case 32:
-                                    default:
-                                        return U
-                                }
-                                return e.next_out = a, e.avail_out = h, e.next_in = s, e.avail_in = o, r.hold = u, r.bits = l, (r.wsize || c !== e.avail_out && r.mode < 30 && (r.mode < 27 || 4 !== t)) && Z(e, e.output, e.next_out, c - e.avail_out) ? (r.mode = 31, -4) : (f -= e.avail_in, c -= e.avail_out, e.total_in += f, e.total_out += c, r.total += c, r.wrap && c && (e.adler = r.check = r.flags ? B(r.check, i, c, e.next_out - c) : O(r.check, i, c, e.next_out - c)), e.data_type = r.bits + (r.last ? 64 : 0) + (12 === r.mode ? 128 : 0) + (20 === r.mode || 15 === r.mode ? 256 : 0), (0 == f && 0 === c || 4 === t) && x === N && (x = -5), x)
-                            }, r.inflateEnd = function(e) {
-                                if (!e || !e.state) return U;
-                                var t = e.state;
-                                return t.window && (t.window = null), e.state = null, N
-                            }, r.inflateGetHeader = function(e, t) {
-                                var r;
-                                return e && e.state ? 0 == (2 & (r = e.state).wrap) ? U : ((r.head = t).done = !1, N) : U
-                            }, r.inflateSetDictionary = function(e, t) {
-                                var r, n = t.length;
-                                return e && e.state ? 0 !== (r = e.state).wrap && 11 !== r.mode ? U : 11 === r.mode && O(1, t, n, 0) !== r.check ? -3 : Z(e, t, n, n) ? (r.mode = 31, -4) : (r.havedict = 1, N) : U
-                            }, r.inflateInfo = "pako inflate (from Nodeca project)"
-                        }, {
-                            "../utils/common": 41,
-                            "./adler32": 43,
-                            "./crc32": 45,
-                            "./inffast": 48,
-                            "./inftrees": 50
-                        }],
-                        50: [function(e, t, r) {
-                            "use strict";
-                            var D = e("../utils/common"),
-                                F = [3, 4, 5, 6, 7, 8, 9, 10, 11, 13, 15, 17, 19, 23, 27, 31, 35, 43, 51, 59, 67, 83, 99, 115, 131, 163, 195, 227, 258, 0, 0],
-                                N = [16, 16, 16, 16, 16, 16, 16, 16, 17, 17, 17, 17, 18, 18, 18, 18, 19, 19, 19, 19, 20, 20, 20, 20, 21, 21, 21, 21, 16, 72, 78],
-                                U = [1, 2, 3, 4, 5, 7, 9, 13, 17, 25, 33, 49, 65, 97, 129, 193, 257, 385, 513, 769, 1025, 1537, 2049, 3073, 4097, 6145, 8193, 12289, 16385, 24577, 0, 0],
-                                P = [16, 16, 16, 16, 17, 17, 18, 18, 19, 19, 20, 20, 21, 21, 22, 22, 23, 23, 24, 24, 25, 25, 26, 26, 27, 27, 28, 28, 29, 29, 64, 64];
-                            t.exports = function(e, t, r, n, i, s, a, o) {
-                                var h, u, l, f, c, d, p, m, _, g = o.bits,
-                                    b = 0,
-                                    v = 0,
-                                    y = 0,
-                                    w = 0,
-                                    k = 0,
-                                    x = 0,
-                                    S = 0,
-                                    z = 0,
-                                    C = 0,
-                                    E = 0,
-                                    A = null,
-                                    I = 0,
-                                    O = new D.Buf16(16),
-                                    B = new D.Buf16(16),
-                                    R = null,
-                                    T = 0;
-                                for (b = 0; b <= 15; b++) O[b] = 0;
-                                for (v = 0; v < n; v++) O[t[r + v]]++;
-                                for (k = g, w = 15; 1 <= w && 0 === O[w]; w--);
-                                if (w < k && (k = w), 0 === w) return i[s++] = 20971520, i[s++] = 20971520, o.bits = 1, 0;
-                                for (y = 1; y < w && 0 === O[y]; y++);
-                                for (k < y && (k = y), b = z = 1; b <= 15; b++)
-                                    if (z <<= 1, (z -= O[b]) < 0) return -1;
-                                if (0 < z && (0 === e || 1 !== w)) return -1;
-                                for (B[1] = 0, b = 1; b < 15; b++) B[b + 1] = B[b] + O[b];
-                                for (v = 0; v < n; v++) 0 !== t[r + v] && (a[B[t[r + v]]++] = v);
-                                if (d = 0 === e ? (A = R = a, 19) : 1 === e ? (A = F, I -= 257, R = N, T -= 257, 256) : (A = U, R = P, -1), b = y, c = s, S = v = E = 0, l = -1, f = (C = 1 << (x = k)) - 1, 1 === e && 852 < C || 2 === e && 592 < C) return 1;
-                                for (;;) {
-                                    for (p = b - S, _ = a[v] < d ? (m = 0, a[v]) : a[v] > d ? (m = R[T + a[v]], A[I + a[v]]) : (m = 96, 0), h = 1 << b - S, y = u = 1 << x; i[c + (E >> S) + (u -= h)] = p << 24 | m << 16 | _ | 0, 0 !== u;);
-                                    for (h = 1 << b - 1; E & h;) h >>= 1;
-                                    if (0 !== h ? (E &= h - 1, E += h) : E = 0, v++, 0 == --O[b]) {
-                                        if (b === w) break;
-                                        b = t[r + a[v]]
-                                    }
-                                    if (k < b && (E & f) !== l) {
-                                        for (0 === S && (S = k), c += y, z = 1 << (x = b - S); x + S < w && !((z -= O[x + S]) <= 0);) x++, z <<= 1;
-                                        if (C += 1 << x, 1 === e && 852 < C || 2 === e && 592 < C) return 1;
-                                        i[l = E & f] = k << 24 | x << 16 | c - s | 0
-                                    }
-                                }
-                                return 0 !== E && (i[c + E] = b - S << 24 | 64 << 16 | 0), o.bits = k, 0
-                            }
-                        }, {
-                            "../utils/common": 41
-                        }],
-                        51: [function(e, t, r) {
-                            "use strict";
-                            t.exports = {
-                                2: "need dictionary",
-                                1: "stream end",
-                                0: "",
-                                "-1": "file error",
-                                "-2": "stream error",
-                                "-3": "data error",
-                                "-4": "insufficient memory",
-                                "-5": "buffer error",
-                                "-6": "incompatible version"
-                            }
-                        }, {}],
-                        52: [function(e, t, r) {
-                            "use strict";
-                            var i = e("../utils/common"),
-                                o = 0,
-                                h = 1;
-
-                            function n(e) {
-                                for (var t = e.length; 0 <= --t;) e[t] = 0
-                            }
-                            var s = 0,
-                                a = 29,
-                                u = 256,
-                                l = u + 1 + a,
-                                f = 30,
-                                c = 19,
-                                _ = 2 * l + 1,
-                                g = 15,
-                                d = 16,
-                                p = 7,
-                                m = 256,
-                                b = 16,
-                                v = 17,
-                                y = 18,
-                                w = [0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 2, 2, 2, 2, 3, 3, 3, 3, 4, 4, 4, 4, 5, 5, 5, 5, 0],
-                                k = [0, 0, 0, 0, 1, 1, 2, 2, 3, 3, 4, 4, 5, 5, 6, 6, 7, 7, 8, 8, 9, 9, 10, 10, 11, 11, 12, 12, 13, 13],
-                                x = [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 2, 3, 7],
-                                S = [16, 17, 18, 0, 8, 7, 9, 6, 10, 5, 11, 4, 12, 3, 13, 2, 14, 1, 15],
-                                z = new Array(2 * (l + 2));
-                            n(z);
-                            var C = new Array(2 * f);
-                            n(C);
-                            var E = new Array(512);
-                            n(E);
-                            var A = new Array(256);
-                            n(A);
-                            var I = new Array(a);
-                            n(I);
-                            var O, B, R, T = new Array(f);
-
-                            function D(e, t, r, n, i) {
-                                this.static_tree = e, this.extra_bits = t, this.extra_base = r, this.elems = n, this.max_length = i, this.has_stree = e && e.length
-                            }
-
-                            function F(e, t) {
-                                this.dyn_tree = e, this.max_code = 0, this.stat_desc = t
-                            }
-
-                            function N(e) {
-                                return e < 256 ? E[e] : E[256 + (e >>> 7)]
-                            }
-
-                            function U(e, t) {
-                                e.pending_buf[e.pending++] = 255 & t, e.pending_buf[e.pending++] = t >>> 8 & 255
-                            }
-
-                            function P(e, t, r) {
-                                e.bi_valid > d - r ? (e.bi_buf |= t << e.bi_valid & 65535, U(e, e.bi_buf), e.bi_buf = t >> d - e.bi_valid, e.bi_valid += r - d) : (e.bi_buf |= t << e.bi_valid & 65535, e.bi_valid += r)
-                            }
-
-                            function L(e, t, r) {
-                                P(e, r[2 * t], r[2 * t + 1])
-                            }
-
-                            function j(e, t) {
-                                for (var r = 0; r |= 1 & e, e >>>= 1, r <<= 1, 0 < --t;);
-                                return r >>> 1
-                            }
-
-                            function Z(e, t, r) {
-                                var n, i, s = new Array(g + 1),
-                                    a = 0;
-                                for (n = 1; n <= g; n++) s[n] = a = a + r[n - 1] << 1;
-                                for (i = 0; i <= t; i++) {
-                                    var o = e[2 * i + 1];
-                                    0 !== o && (e[2 * i] = j(s[o]++, o))
-                                }
-                            }
-
-                            function W(e) {
-                                var t;
-                                for (t = 0; t < l; t++) e.dyn_ltree[2 * t] = 0;
-                                for (t = 0; t < f; t++) e.dyn_dtree[2 * t] = 0;
-                                for (t = 0; t < c; t++) e.bl_tree[2 * t] = 0;
-                                e.dyn_ltree[2 * m] = 1, e.opt_len = e.static_len = 0, e.last_lit = e.matches = 0
-                            }
-
-                            function M(e) {
-                                8 < e.bi_valid ? U(e, e.bi_buf) : 0 < e.bi_valid && (e.pending_buf[e.pending++] = e.bi_buf), e.bi_buf = 0, e.bi_valid = 0
-                            }
-
-                            function H(e, t, r, n) {
-                                var i = 2 * t,
-                                    s = 2 * r;
-                                return e[i] < e[s] || e[i] === e[s] && n[t] <= n[r]
-                            }
-
-                            function G(e, t, r) {
-                                for (var n = e.heap[r], i = r << 1; i <= e.heap_len && (i < e.heap_len && H(t, e.heap[i + 1], e.heap[i], e.depth) && i++, !H(t, n, e.heap[i], e.depth));) e.heap[r] = e.heap[i], r = i, i <<= 1;
-                                e.heap[r] = n
-                            }
-
-                            function K(e, t, r) {
-                                var n, i, s, a, o = 0;
-                                if (0 !== e.last_lit)
-                                    for (; n = e.pending_buf[e.d_buf + 2 * o] << 8 | e.pending_buf[e.d_buf + 2 * o + 1], i = e.pending_buf[e.l_buf + o], o++, 0 === n ? L(e, i, t) : (L(e, (s = A[i]) + u + 1, t), 0 !== (a = w[s]) && P(e, i -= I[s], a), L(e, s = N(--n), r), 0 !== (a = k[s]) && P(e, n -= T[s], a)), o < e.last_lit;);
-                                L(e, m, t)
-                            }
-
-                            function Y(e, t) {
-                                var r, n, i, s = t.dyn_tree,
-                                    a = t.stat_desc.static_tree,
-                                    o = t.stat_desc.has_stree,
-                                    h = t.stat_desc.elems,
-                                    u = -1;
-                                for (e.heap_len = 0, e.heap_max = _, r = 0; r < h; r++) 0 !== s[2 * r] ? (e.heap[++e.heap_len] = u = r, e.depth[r] = 0) : s[2 * r + 1] = 0;
-                                for (; e.heap_len < 2;) s[2 * (i = e.heap[++e.heap_len] = u < 2 ? ++u : 0)] = 1, e.depth[i] = 0, e.opt_len--, o && (e.static_len -= a[2 * i + 1]);
-                                for (t.max_code = u, r = e.heap_len >> 1; 1 <= r; r--) G(e, s, r);
-                                for (i = h; r = e.heap[1], e.heap[1] = e.heap[e.heap_len--], G(e, s, 1), n = e.heap[1], e.heap[--e.heap_max] = r, e.heap[--e.heap_max] = n, s[2 * i] = s[2 * r] + s[2 * n], e.depth[i] = (e.depth[r] >= e.depth[n] ? e.depth[r] : e.depth[n]) + 1, s[2 * r + 1] = s[2 * n + 1] = i, e.heap[1] = i++, G(e, s, 1), 2 <= e.heap_len;);
-                                e.heap[--e.heap_max] = e.heap[1],
-                                    function(e, t) {
-                                        var r, n, i, s, a, o, h = t.dyn_tree,
-                                            u = t.max_code,
-                                            l = t.stat_desc.static_tree,
-                                            f = t.stat_desc.has_stree,
-                                            c = t.stat_desc.extra_bits,
-                                            d = t.stat_desc.extra_base,
-                                            p = t.stat_desc.max_length,
-                                            m = 0;
-                                        for (s = 0; s <= g; s++) e.bl_count[s] = 0;
-                                        for (h[2 * e.heap[e.heap_max] + 1] = 0, r = e.heap_max + 1; r < _; r++) p < (s = h[2 * h[2 * (n = e.heap[r]) + 1] + 1] + 1) && (s = p, m++), h[2 * n + 1] = s, u < n || (e.bl_count[s]++, a = 0, d <= n && (a = c[n - d]), o = h[2 * n], e.opt_len += o * (s + a), f && (e.static_len += o * (l[2 * n + 1] + a)));
-                                        if (0 !== m) {
-                                            do {
-                                                for (s = p - 1; 0 === e.bl_count[s];) s--;
-                                                e.bl_count[s]--, e.bl_count[s + 1] += 2, e.bl_count[p]--, m -= 2
-                                            } while (0 < m);
-                                            for (s = p; 0 !== s; s--)
-                                                for (n = e.bl_count[s]; 0 !== n;) u < (i = e.heap[--r]) || (h[2 * i + 1] !== s && (e.opt_len += (s - h[2 * i + 1]) * h[2 * i], h[2 * i + 1] = s), n--)
-                                        }
-                                    }(e, t), Z(s, u, e.bl_count)
-                            }
-
-                            function X(e, t, r) {
-                                var n, i, s = -1,
-                                    a = t[1],
-                                    o = 0,
-                                    h = 7,
-                                    u = 4;
-                                for (0 === a && (h = 138, u = 3), t[2 * (r + 1) + 1] = 65535, n = 0; n <= r; n++) i = a, a = t[2 * (n + 1) + 1], ++o < h && i === a || (o < u ? e.bl_tree[2 * i] += o : 0 !== i ? (i !== s && e.bl_tree[2 * i]++, e.bl_tree[2 * b]++) : o <= 10 ? e.bl_tree[2 * v]++ : e.bl_tree[2 * y]++, s = i, u = (o = 0) === a ? (h = 138, 3) : i === a ? (h = 6, 3) : (h = 7, 4))
-                            }
-
-                            function V(e, t, r) {
-                                var n, i, s = -1,
-                                    a = t[1],
-                                    o = 0,
-                                    h = 7,
-                                    u = 4;
-                                for (0 === a && (h = 138, u = 3), n = 0; n <= r; n++)
-                                    if (i = a, a = t[2 * (n + 1) + 1], !(++o < h && i === a)) {
-                                        if (o < u)
-                                            for (; L(e, i, e.bl_tree), 0 != --o;);
-                                        else 0 !== i ? (i !== s && (L(e, i, e.bl_tree), o--), L(e, b, e.bl_tree), P(e, o - 3, 2)) : o <= 10 ? (L(e, v, e.bl_tree), P(e, o - 3, 3)) : (L(e, y, e.bl_tree), P(e, o - 11, 7));
-                                        s = i, u = (o = 0) === a ? (h = 138, 3) : i === a ? (h = 6, 3) : (h = 7, 4)
-                                    }
-                            }
-                            n(T);
-                            var q = !1;
-
-                            function J(e, t, r, n) {
-                                P(e, (s << 1) + (n ? 1 : 0), 3),
-                                    function(e, t, r, n) {
-                                        M(e), n && (U(e, r), U(e, ~r)), i.arraySet(e.pending_buf, e.window, t, r, e.pending), e.pending += r
-                                    }(e, t, r, !0)
-                            }
-                            r._tr_init = function(e) {
-                                q || (function() {
-                                    var e, t, r, n, i, s = new Array(g + 1);
-                                    for (n = r = 0; n < a - 1; n++)
-                                        for (I[n] = r, e = 0; e < 1 << w[n]; e++) A[r++] = n;
-                                    for (A[r - 1] = n, n = i = 0; n < 16; n++)
-                                        for (T[n] = i, e = 0; e < 1 << k[n]; e++) E[i++] = n;
-                                    for (i >>= 7; n < f; n++)
-                                        for (T[n] = i << 7, e = 0; e < 1 << k[n] - 7; e++) E[256 + i++] = n;
-                                    for (t = 0; t <= g; t++) s[t] = 0;
-                                    for (e = 0; e <= 143;) z[2 * e + 1] = 8, e++, s[8]++;
-                                    for (; e <= 255;) z[2 * e + 1] = 9, e++, s[9]++;
-                                    for (; e <= 279;) z[2 * e + 1] = 7, e++, s[7]++;
-                                    for (; e <= 287;) z[2 * e + 1] = 8, e++, s[8]++;
-                                    for (Z(z, l + 1, s), e = 0; e < f; e++) C[2 * e + 1] = 5, C[2 * e] = j(e, 5);
-                                    O = new D(z, w, u + 1, l, g), B = new D(C, k, 0, f, g), R = new D(new Array(0), x, 0, c, p)
-                                }(), q = !0), e.l_desc = new F(e.dyn_ltree, O), e.d_desc = new F(e.dyn_dtree, B), e.bl_desc = new F(e.bl_tree, R), e.bi_buf = 0, e.bi_valid = 0, W(e)
-                            }, r._tr_stored_block = J, r._tr_flush_block = function(e, t, r, n) {
-                                var i, s, a = 0;
-                                0 < e.level ? (2 === e.strm.data_type && (e.strm.data_type = function(e) {
-                                    var t, r = 4093624447;
-                                    for (t = 0; t <= 31; t++, r >>>= 1)
-                                        if (1 & r && 0 !== e.dyn_ltree[2 * t]) return o;
-                                    if (0 !== e.dyn_ltree[18] || 0 !== e.dyn_ltree[20] || 0 !== e.dyn_ltree[26]) return h;
-                                    for (t = 32; t < u; t++)
-                                        if (0 !== e.dyn_ltree[2 * t]) return h;
-                                    return o
-                                }(e)), Y(e, e.l_desc), Y(e, e.d_desc), a = function(e) {
-                                    var t;
-                                    for (X(e, e.dyn_ltree, e.l_desc.max_code), X(e, e.dyn_dtree, e.d_desc.max_code), Y(e, e.bl_desc), t = c - 1; 3 <= t && 0 === e.bl_tree[2 * S[t] + 1]; t--);
-                                    return e.opt_len += 3 * (t + 1) + 5 + 5 + 4, t
-                                }(e), i = e.opt_len + 3 + 7 >>> 3, (s = e.static_len + 3 + 7 >>> 3) <= i && (i = s)) : i = s = r + 5, r + 4 <= i && -1 !== t ? J(e, t, r, n) : 4 === e.strategy || s === i ? (P(e, 2 + (n ? 1 : 0), 3), K(e, z, C)) : (P(e, 4 + (n ? 1 : 0), 3), function(e, t, r, n) {
-                                    var i;
-                                    for (P(e, t - 257, 5), P(e, r - 1, 5), P(e, n - 4, 4), i = 0; i < n; i++) P(e, e.bl_tree[2 * S[i] + 1], 3);
-                                    V(e, e.dyn_ltree, t - 1), V(e, e.dyn_dtree, r - 1)
-                                }(e, e.l_desc.max_code + 1, e.d_desc.max_code + 1, a + 1), K(e, e.dyn_ltree, e.dyn_dtree)), W(e), n && M(e)
-                            }, r._tr_tally = function(e, t, r) {
-                                return e.pending_buf[e.d_buf + 2 * e.last_lit] = t >>> 8 & 255, e.pending_buf[e.d_buf + 2 * e.last_lit + 1] = 255 & t, e.pending_buf[e.l_buf + e.last_lit] = 255 & r, e.last_lit++, 0 === t ? e.dyn_ltree[2 * r]++ : (e.matches++, t--, e.dyn_ltree[2 * (A[r] + u + 1)]++, e.dyn_dtree[2 * N(t)]++), e.last_lit === e.lit_bufsize - 1
-                            }, r._tr_align = function(e) {
-                                P(e, 2, 3), L(e, m, z),
-                                    function(e) {
-                                        16 === e.bi_valid ? (U(e, e.bi_buf), e.bi_buf = 0, e.bi_valid = 0) : 8 <= e.bi_valid && (e.pending_buf[e.pending++] = 255 & e.bi_buf, e.bi_buf >>= 8, e.bi_valid -= 8)
-                                    }(e)
-                            }
-                        }, {
-                            "../utils/common": 41
-                        }],
-                        53: [function(e, t, r) {
-                            "use strict";
-                            t.exports = function() {
-                                this.input = null, this.next_in = 0, this.avail_in = 0, this.total_in = 0, this.output = null, this.next_out = 0, this.avail_out = 0, this.total_out = 0, this.msg = "", this.state = null, this.data_type = 2, this.adler = 0
-                            }
-                        }, {}],
-                        54: [function(e, t, r) {
-                            (function(e) {
-                                ! function(r, n) {
-                                    "use strict";
-                                    if (!r.setImmediate) {
-                                        var i, s, t, a, o = 1,
-                                            h = {},
-                                            u = !1,
-                                            l = r.document,
-                                            e = Object.getPrototypeOf && Object.getPrototypeOf(r);
-                                        e = e && e.setTimeout ? e : r, i = "[object process]" === {}.toString.call(r.process) ? function(e) {
-                                            process.nextTick(function() {
-                                                c(e)
-                                            })
-                                        } : function() {
-                                            if (r.postMessage && !r.importScripts) {
-                                                var e = !0,
-                                                    t = r.onmessage;
-                                                return r.onmessage = function() {
-                                                    e = !1
-                                                }, r.postMessage("", "*"), r.onmessage = t, e
-                                            }
-                                        }() ? (a = "setImmediate$" + Math.random() + "$", r.addEventListener ? r.addEventListener("message", d, !1) : r.attachEvent("onmessage", d), function(e) {
-                                            r.postMessage(a + e, "*")
-                                        }) : r.MessageChannel ? ((t = new MessageChannel).port1.onmessage = function(e) {
-                                            c(e.data)
-                                        }, function(e) {
-                                            t.port2.postMessage(e)
-                                        }) : l && "onreadystatechange" in l.createElement("script") ? (s = l.documentElement, function(e) {
-                                            var t = l.createElement("script");
-                                            t.onreadystatechange = function() {
-                                                c(e), t.onreadystatechange = null, s.removeChild(t), t = null
-                                            }, s.appendChild(t)
-                                        }) : function(e) {
-                                            setTimeout(c, 0, e)
-                                        }, e.setImmediate = function(e) {
-                                            "function" != typeof e && (e = new Function("" + e));
-                                            for (var t = new Array(arguments.length - 1), r = 0; r < t.length; r++) t[r] = arguments[r + 1];
-                                            var n = {
-                                                callback: e,
-                                                args: t
-                                            };
-                                            return h[o] = n, i(o), o++
-                                        }, e.clearImmediate = f
-                                    }
-
-                                    function f(e) {
-                                        delete h[e]
-                                    }
-
-                                    function c(e) {
-                                        if (u) setTimeout(c, 0, e);
-                                        else {
-                                            var t = h[e];
-                                            if (t) {
-                                                u = !0;
-                                                try {
-                                                    ! function(e) {
-                                                        var t = e.callback,
-                                                            r = e.args;
-                                                        switch (r.length) {
-                                                            case 0:
-                                                                t();
-                                                                break;
-                                                            case 1:
-                                                                t(r[0]);
-                                                                break;
-                                                            case 2:
-                                                                t(r[0], r[1]);
-                                                                break;
-                                                            case 3:
-                                                                t(r[0], r[1], r[2]);
-                                                                break;
-                                                            default:
-                                                                t.apply(n, r)
-                                                        }
-                                                    }(t)
-                                                } finally {
-                                                    f(e), u = !1
-                                                }
-                                            }
-                                        }
+                                            B = r.lens[r.have - 1], k = 3 + (3 & _), _ >>>= 2, g -= 2
+                                        } else if (17 === E) {
+                                            for (D = z + 3; g < D;) {
+                                                if (0 === p) break t;
+                                                p--, _ += l[c++] << g, g += 8
+                                            }
+                                            g -= z, B = 0, k = 3 + (7 & (_ >>>= z)), _ >>>= 3, g -= 3
+                                        } else {
+                                            for (D = z + 7; g < D;) {
+                                                if (0 === p) break t;
+                                                p--, _ += l[c++] << g, g += 8
+                                            }
+                                            g -= z, B = 0, k = 11 + (127 & (_ >>>= z)), _ >>>= 7, g -= 7
+                                        }
+                                        if (r.have + k > r.nlen + r.ndist) {
+                                            t.msg = "invalid bit length repeat", r.mode = 30;
+                                            break
+                                        }
+                                        for (; k--;) r.lens[r.have++] = B
+                                    }
+                                }
+                                if (30 === r.mode) break;
+                                if (0 === r.lens[256]) {
+                                    t.msg = "invalid code -- missing end-of-block", r.mode = 30;
+                                    break
+                                }
+                                if (r.lenbits = 9, R = {
+                                        bits: r.lenbits
+                                    }, T = o(1, r.lens, 0, r.nlen, r.lencode, 0, r.work, R), r.lenbits = R.bits, T) {
+                                    t.msg = "invalid literal/lengths set", r.mode = 30;
+                                    break
+                                }
+                                if (r.distbits = 6, r.distcode = r.distdyn, R = {
+                                        bits: r.distbits
+                                    }, T = o(2, r.lens, r.nlen, r.ndist, r.distcode, 0, r.work, R), r.distbits = R.bits, T) {
+                                    t.msg = "invalid distances set", r.mode = 30;
+                                    break
+                                }
+                                if (r.mode = 20, 6 === e) break t;
+                            case 20:
+                                r.mode = 21;
+                            case 21:
+                                if (6 <= p && 258 <= m) {
+                                    t.next_out = d, t.avail_out = m, t.next_in = c, t.avail_in = p, r.hold = _, r.bits = g, a(t, w), d = t.next_out, f = t.output, m = t.avail_out, c = t.next_in, l = t.input, p = t.avail_in, _ = r.hold, g = r.bits, 12 === r.mode && (r.back = -1);
+                                    break
+                                }
+                                for (r.back = 0; C = (F = r.lencode[_ & (1 << r.lenbits) - 1]) >>> 16 & 255, E = 65535 & F, !((z = F >>> 24) <= g);) {
+                                    if (0 === p) break t;
+                                    p--, _ += l[c++] << g, g += 8
+                                }
+                                if (C && 0 == (240 & C)) {
+                                    for (A = z, I = C, O = E; C = (F = r.lencode[O + ((_ & (1 << A + I) - 1) >> A)]) >>> 16 & 255, E = 65535 & F, !(A + (z = F >>> 24) <= g);) {
+                                        if (0 === p) break t;
+                                        p--, _ += l[c++] << g, g += 8
+                                    }
+                                    _ >>>= A, g -= A, r.back += A
+                                }
+                                if (_ >>>= z, g -= z, r.back += z, r.length = E, 0 === C) {
+                                    r.mode = 26;
+                                    break
+                                }
+                                if (32 & C) {
+                                    r.back = -1, r.mode = 12;
+                                    break
+                                }
+                                if (64 & C) {
+                                    t.msg = "invalid literal/length code", r.mode = 30;
+                                    break
+                                }
+                                r.extra = 15 & C, r.mode = 22;
+                            case 22:
+                                if (r.extra) {
+                                    for (D = r.extra; g < D;) {
+                                        if (0 === p) break t;
+                                        p--, _ += l[c++] << g, g += 8
+                                    }
+                                    r.length += _ & (1 << r.extra) - 1, _ >>>= r.extra, g -= r.extra, r.back += r.extra
+                                }
+                                r.was = r.length, r.mode = 23;
+                            case 23:
+                                for (; C = (F = r.distcode[_ & (1 << r.distbits) - 1]) >>> 16 & 255, E = 65535 & F, !((z = F >>> 24) <= g);) {
+                                    if (0 === p) break t;
+                                    p--, _ += l[c++] << g, g += 8
+                                }
+                                if (0 == (240 & C)) {
+                                    for (A = z, I = C, O = E; C = (F = r.distcode[O + ((_ & (1 << A + I) - 1) >> A)]) >>> 16 & 255, E = 65535 & F, !(A + (z = F >>> 24) <= g);) {
+                                        if (0 === p) break t;
+                                        p--, _ += l[c++] << g, g += 8
+                                    }
+                                    _ >>>= A, g -= A, r.back += A
+                                }
+                                if (_ >>>= z, g -= z, r.back += z, 64 & C) {
+                                    t.msg = "invalid distance code", r.mode = 30;
+                                    break
+                                }
+                                r.offset = E, r.extra = 15 & C, r.mode = 24;
+                            case 24:
+                                if (r.extra) {
+                                    for (D = r.extra; g < D;) {
+                                        if (0 === p) break t;
+                                        p--, _ += l[c++] << g, g += 8
+                                    }
+                                    r.offset += _ & (1 << r.extra) - 1, _ >>>= r.extra, g -= r.extra, r.back += r.extra
+                                }
+                                if (r.offset > r.dmax) {
+                                    t.msg = "invalid distance too far back", r.mode = 30;
+                                    break
+                                }
+                                r.mode = 25;
+                            case 25:
+                                if (0 === m) break t;
+                                if (k = w - m, r.offset > k) {
+                                    if ((k = r.offset - k) > r.whave && r.sane) {
+                                        t.msg = "invalid distance too far back", r.mode = 30;
+                                        break
                                     }
-
-                                    function d(e) {
-                                        e.source === r && "string" == typeof e.data && 0 === e.data.indexOf(a) && c(+e.data.slice(a.length))
+                                    x = k > r.wnext ? (k -= r.wnext, r.wsize - k) : r.wnext - k, k > r.length && (k = r.length), S = r.window
+                                } else S = f, x = d - r.offset, k = r.length;
+                                for (m < k && (k = m), m -= k, r.length -= k; f[d++] = S[x++], --k;);
+                                0 === r.length && (r.mode = 21);
+                                break;
+                            case 26:
+                                if (0 === m) break t;
+                                f[d++] = r.length, m--, r.mode = 21;
+                                break;
+                            case 27:
+                                if (r.wrap) {
+                                    for (; g < 32;) {
+                                        if (0 === p) break t;
+                                        p--, _ |= l[c++] << g, g += 8
+                                    }
+                                    if (w -= m, t.total_out += w, r.total += w, w && (t.adler = r.check = r.flags ? s(r.check, f, w, d - w) : i(r.check, f, w, d - w)), w = m, (r.flags ? _ : u(_)) !== r.check) {
+                                        t.msg = "incorrect data check", r.mode = 30;
+                                        break
+                                    }
+                                    g = _ = 0
+                                }
+                                r.mode = 28;
+                            case 28:
+                                if (r.wrap && r.flags) {
+                                    for (; g < 32;) {
+                                        if (0 === p) break t;
+                                        p--, _ += l[c++] << g, g += 8
+                                    }
+                                    if (_ !== (4294967295 & r.total)) {
+                                        t.msg = "incorrect length check", r.mode = 30;
+                                        break
                                     }
-                                }("undefined" == typeof self ? void 0 === e ? this : e : self)
-                            }).call(this, "undefined" != typeof __webpack_require__.g ? __webpack_require__.g : "undefined" != typeof self ? self : "undefined" != typeof window ? window : {})
-                        }, {}]
-                    }, {}, [10])(10)
-                });
-
-                /***/
-            }),
-
-        /***/
-        "./node_modules/process/browser.js":
-            /*!*****************************************!*\
-              !*** ./node_modules/process/browser.js ***!
-              \*****************************************/
-            /***/
-            ((module) => {
-
-                // shim for using process in browser
-                var process = module.exports = {};
-
-                // cached from whatever global is present so that test runners that stub it
-                // don't break things.  But we need to wrap it in a try catch in case it is
-                // wrapped in strict mode code which doesn't define any globals.  It's inside a
-                // function because try/catches deoptimize in certain engines.
+                                    g = _ = 0
+                                }
+                                r.mode = 29;
+                            case 29:
+                                T = 1;
+                                break t;
+                            case 30:
+                                T = -3;
+                                break t;
+                            case 31:
+                                return -4;
+                            default:
+                                return h
+                        }
+                        return t.next_out = d, t.avail_out = m, t.next_in = c, t.avail_in = p, r.hold = _, r.bits = g, (r.wsize || w !== t.avail_out && r.mode < 30 && (r.mode < 27 || 4 !== e)) && v(t, t.output, t.next_out, w - t.avail_out) ? (r.mode = 31, -4) : (y -= t.avail_in, w -= t.avail_out, t.total_in += y, t.total_out += w, r.total += w, r.wrap && w && (t.adler = r.check = r.flags ? s(r.check, f, w, t.next_out - w) : i(r.check, f, w, t.next_out - w)), t.data_type = r.bits + (r.last ? 64 : 0) + (12 === r.mode ? 128 : 0) + (20 === r.mode || 15 === r.mode ? 256 : 0), (0 == y && 0 === w || 4 === e) && 0 === T && (T = -5), T)
+                    }, r.inflateEnd = function(t) {
+                        if (!t || !t.state) return h;
+                        var e = t.state;
+                        return e.window && (e.window = null), t.state = null, 0
+                    }, r.inflateGetHeader = function(t, e) {
+                        var r;
+                        return t && t.state ? 0 == (2 & (r = t.state).wrap) ? h : ((r.head = e).done = !1, 0) : h
+                    }, r.inflateSetDictionary = function(t, e) {
+                        var r, n = e.length;
+                        return t && t.state ? 0 !== (r = t.state).wrap && 11 !== r.mode ? h : 11 === r.mode && i(1, e, n, 0) !== r.check ? -3 : v(t, e, n, n) ? (r.mode = 31, -4) : (r.havedict = 1, 0) : h
+                    }, r.inflateInfo = "pako inflate (from Nodeca project)"
+                }, {
+                    "../utils/common": 41,
+                    "./adler32": 43,
+                    "./crc32": 45,
+                    "./inffast": 48,
+                    "./inftrees": 50
+                }],
+                50: [function(t, e, r) {
+                    "use strict";
+                    var n = t("../utils/common"),
+                        i = [3, 4, 5, 6, 7, 8, 9, 10, 11, 13, 15, 17, 19, 23, 27, 31, 35, 43, 51, 59, 67, 83, 99, 115, 131, 163, 195, 227, 258, 0, 0],
+                        s = [16, 16, 16, 16, 16, 16, 16, 16, 17, 17, 17, 17, 18, 18, 18, 18, 19, 19, 19, 19, 20, 20, 20, 20, 21, 21, 21, 21, 16, 72, 78],
+                        a = [1, 2, 3, 4, 5, 7, 9, 13, 17, 25, 33, 49, 65, 97, 129, 193, 257, 385, 513, 769, 1025, 1537, 2049, 3073, 4097, 6145, 8193, 12289, 16385, 24577, 0, 0],
+                        o = [16, 16, 16, 16, 17, 17, 18, 18, 19, 19, 20, 20, 21, 21, 22, 22, 23, 23, 24, 24, 25, 25, 26, 26, 27, 27, 28, 28, 29, 29, 64, 64];
+                    e.exports = function(t, e, r, h, u, l, f, c) {
+                        var d, p, m, _, g, b, v, y, w, k = c.bits,
+                            x = 0,
+                            S = 0,
+                            z = 0,
+                            C = 0,
+                            E = 0,
+                            A = 0,
+                            I = 0,
+                            O = 0,
+                            B = 0,
+                            T = 0,
+                            R = null,
+                            D = 0,
+                            F = new n.Buf16(16),
+                            N = new n.Buf16(16),
+                            U = null,
+                            P = 0;
+                        for (x = 0; x <= 15; x++) F[x] = 0;
+                        for (S = 0; S < h; S++) F[e[r + S]]++;
+                        for (E = k, C = 15; 1 <= C && 0 === F[C]; C--);
+                        if (C < E && (E = C), 0 === C) return u[l++] = 20971520, u[l++] = 20971520, c.bits = 1, 0;
+                        for (z = 1; z < C && 0 === F[z]; z++);
+                        for (E < z && (E = z), x = O = 1; x <= 15; x++)
+                            if (O <<= 1, (O -= F[x]) < 0) return -1;
+                        if (0 < O && (0 === t || 1 !== C)) return -1;
+                        for (N[1] = 0, x = 1; x < 15; x++) N[x + 1] = N[x] + F[x];
+                        for (S = 0; S < h; S++) 0 !== e[r + S] && (f[N[e[r + S]]++] = S);
+                        if (b = 0 === t ? (R = U = f, 19) : 1 === t ? (R = i, D -= 257, U = s, P -= 257, 256) : (R = a, U = o, -1), x = z, g = l, I = S = T = 0, m = -1, _ = (B = 1 << (A = E)) - 1, 1 === t && 852 < B || 2 === t && 592 < B) return 1;
+                        for (;;) {
+                            for (v = x - I, w = f[S] < b ? (y = 0, f[S]) : f[S] > b ? (y = U[P + f[S]], R[D + f[S]]) : (y = 96, 0), d = 1 << x - I, z = p = 1 << A; u[g + (T >> I) + (p -= d)] = v << 24 | y << 16 | w | 0, 0 !== p;);
+                            for (d = 1 << x - 1; T & d;) d >>= 1;
+                            if (0 !== d ? (T &= d - 1, T += d) : T = 0, S++, 0 == --F[x]) {
+                                if (x === C) break;
+                                x = e[r + f[S]]
+                            }
+                            if (E < x && (T & _) !== m) {
+                                for (0 === I && (I = E), g += z, O = 1 << (A = x - I); A + I < C && !((O -= F[A + I]) <= 0);) A++, O <<= 1;
+                                if (B += 1 << A, 1 === t && 852 < B || 2 === t && 592 < B) return 1;
+                                u[m = T & _] = E << 24 | A << 16 | g - l | 0
+                            }
+                        }
+                        return 0 !== T && (u[g + T] = x - I << 24 | 64 << 16 | 0), c.bits = E, 0
+                    }
+                }, {
+                    "../utils/common": 41
+                }],
+                51: [function(t, e, r) {
+                    "use strict";
+                    e.exports = {
+                        2: "need dictionary",
+                        1: "stream end",
+                        0: "",
+                        "-1": "file error",
+                        "-2": "stream error",
+                        "-3": "data error",
+                        "-4": "insufficient memory",
+                        "-5": "buffer error",
+                        "-6": "incompatible version"
+                    }
+                }, {}],
+                52: [function(t, e, r) {
+                    "use strict";
+                    var n = t("../utils/common");
 
-                var cachedSetTimeout;
-                var cachedClearTimeout;
+                    function i(t) {
+                        for (var e = t.length; 0 <= --e;) t[e] = 0
+                    }
+                    var s = 256,
+                        a = 286,
+                        o = 30,
+                        h = 15,
+                        u = [0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 2, 2, 2, 2, 3, 3, 3, 3, 4, 4, 4, 4, 5, 5, 5, 5, 0],
+                        l = [0, 0, 0, 0, 1, 1, 2, 2, 3, 3, 4, 4, 5, 5, 6, 6, 7, 7, 8, 8, 9, 9, 10, 10, 11, 11, 12, 12, 13, 13],
+                        f = [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 2, 3, 7],
+                        c = [16, 17, 18, 0, 8, 7, 9, 6, 10, 5, 11, 4, 12, 3, 13, 2, 14, 1, 15],
+                        d = new Array(576);
+                    i(d);
+                    var p = new Array(60);
+                    i(p);
+                    var m = new Array(512);
+                    i(m);
+                    var _ = new Array(256);
+                    i(_);
+                    var g = new Array(29);
+                    i(g);
+                    var b, v, y, w = new Array(o);
 
-                function defaultSetTimout() {
-                    throw new Error('setTimeout has not been defined');
-                }
+                    function k(t, e, r, n, i) {
+                        this.static_tree = t, this.extra_bits = e, this.extra_base = r, this.elems = n, this.max_length = i, this.has_stree = t && t.length
+                    }
 
-                function defaultClearTimeout() {
-                    throw new Error('clearTimeout has not been defined');
-                }
-                (function() {
-                    try {
-                        if (typeof setTimeout === 'function') {
-                            cachedSetTimeout = setTimeout;
-                        } else {
-                            cachedSetTimeout = defaultSetTimout;
-                        }
-                    } catch (e) {
-                        cachedSetTimeout = defaultSetTimout;
+                    function x(t, e) {
+                        this.dyn_tree = t, this.max_code = 0, this.stat_desc = e
                     }
-                    try {
-                        if (typeof clearTimeout === 'function') {
-                            cachedClearTimeout = clearTimeout;
-                        } else {
-                            cachedClearTimeout = defaultClearTimeout;
-                        }
-                    } catch (e) {
-                        cachedClearTimeout = defaultClearTimeout;
-                    }
-                }())
-
-                function runTimeout(fun) {
-                    if (cachedSetTimeout === setTimeout) {
-                        //normal enviroments in sane situations
-                        return setTimeout(fun, 0);
-                    }
-                    // if setTimeout wasn't available but was latter defined
-                    if ((cachedSetTimeout === defaultSetTimout || !cachedSetTimeout) && setTimeout) {
-                        cachedSetTimeout = setTimeout;
-                        return setTimeout(fun, 0);
+
+                    function S(t) {
+                        return t < 256 ? m[t] : m[256 + (t >>> 7)]
                     }
-                    try {
-                        // when when somebody has screwed with setTimeout but no I.E. maddness
-                        return cachedSetTimeout(fun, 0);
-                    } catch (e) {
-                        try {
-                            // When we are in I.E. but the script has been evaled so I.E. doesn't trust the global object when called normally
-                            return cachedSetTimeout.call(null, fun, 0);
-                        } catch (e) {
-                            // same as above but when it's a version of I.E. that must have the global object for 'this', hopfully our context correct otherwise it will throw a global error
-                            return cachedSetTimeout.call(this, fun, 0);
-                        }
+
+                    function z(t, e) {
+                        t.pending_buf[t.pending++] = 255 & e, t.pending_buf[t.pending++] = e >>> 8 & 255
                     }
 
+                    function C(t, e, r) {
+                        t.bi_valid > 16 - r ? (t.bi_buf |= e << t.bi_valid & 65535, z(t, t.bi_buf), t.bi_buf = e >> 16 - t.bi_valid, t.bi_valid += r - 16) : (t.bi_buf |= e << t.bi_valid & 65535, t.bi_valid += r)
+                    }
 
-                }
+                    function E(t, e, r) {
+                        C(t, r[2 * e], r[2 * e + 1])
+                    }
 
-                function runClearTimeout(marker) {
-                    if (cachedClearTimeout === clearTimeout) {
-                        //normal enviroments in sane situations
-                        return clearTimeout(marker);
-                    }
-                    // if clearTimeout wasn't available but was latter defined
-                    if ((cachedClearTimeout === defaultClearTimeout || !cachedClearTimeout) && clearTimeout) {
-                        cachedClearTimeout = clearTimeout;
-                        return clearTimeout(marker);
+                    function A(t, e) {
+                        for (var r = 0; r |= 1 & t, t >>>= 1, r <<= 1, 0 < --e;);
+                        return r >>> 1
                     }
-                    try {
-                        // when when somebody has screwed with setTimeout but no I.E. maddness
-                        return cachedClearTimeout(marker);
-                    } catch (e) {
-                        try {
-                            // When we are in I.E. but the script has been evaled so I.E. doesn't  trust the global object when called normally
-                            return cachedClearTimeout.call(null, marker);
-                        } catch (e) {
-                            // same as above but when it's a version of I.E. that must have the global object for 'this', hopfully our context correct otherwise it will throw a global error.
-                            // Some versions of I.E. have different rules for clearTimeout vs setTimeout
-                            return cachedClearTimeout.call(this, marker);
+
+                    function I(t, e, r) {
+                        var n, i, s = new Array(16),
+                            a = 0;
+                        for (n = 1; n <= h; n++) s[n] = a = a + r[n - 1] << 1;
+                        for (i = 0; i <= e; i++) {
+                            var o = t[2 * i + 1];
+                            0 !== o && (t[2 * i] = A(s[o]++, o))
                         }
                     }
 
+                    function O(t) {
+                        var e;
+                        for (e = 0; e < a; e++) t.dyn_ltree[2 * e] = 0;
+                        for (e = 0; e < o; e++) t.dyn_dtree[2 * e] = 0;
+                        for (e = 0; e < 19; e++) t.bl_tree[2 * e] = 0;
+                        t.dyn_ltree[512] = 1, t.opt_len = t.static_len = 0, t.last_lit = t.matches = 0
+                    }
 
+                    function B(t) {
+                        8 < t.bi_valid ? z(t, t.bi_buf) : 0 < t.bi_valid && (t.pending_buf[t.pending++] = t.bi_buf), t.bi_buf = 0, t.bi_valid = 0
+                    }
 
-                }
-                var queue = [];
-                var draining = false;
-                var currentQueue;
-                var queueIndex = -1;
-
-                function cleanUpNextTick() {
-                    if (!draining || !currentQueue) {
-                        return;
-                    }
-                    draining = false;
-                    if (currentQueue.length) {
-                        queue = currentQueue.concat(queue);
-                    } else {
-                        queueIndex = -1;
+                    function T(t, e, r, n) {
+                        var i = 2 * e,
+                            s = 2 * r;
+                        return t[i] < t[s] || t[i] === t[s] && n[e] <= n[r]
                     }
-                    if (queue.length) {
-                        drainQueue();
+
+                    function R(t, e, r) {
+                        for (var n = t.heap[r], i = r << 1; i <= t.heap_len && (i < t.heap_len && T(e, t.heap[i + 1], t.heap[i], t.depth) && i++, !T(e, n, t.heap[i], t.depth));) t.heap[r] = t.heap[i], r = i, i <<= 1;
+                        t.heap[r] = n
                     }
-                }
 
-                function drainQueue() {
-                    if (draining) {
-                        return;
-                    }
-                    var timeout = runTimeout(cleanUpNextTick);
-                    draining = true;
-
-                    var len = queue.length;
-                    while (len) {
-                        currentQueue = queue;
-                        queue = [];
-                        while (++queueIndex < len) {
-                            if (currentQueue) {
-                                currentQueue[queueIndex].run();
-                            }
-                        }
-                        queueIndex = -1;
-                        len = queue.length;
-                    }
-                    currentQueue = null;
-                    draining = false;
-                    runClearTimeout(timeout);
-                }
+                    function D(t, e, r) {
+                        var n, i, a, o, h = 0;
+                        if (0 !== t.last_lit)
+                            for (; n = t.pending_buf[t.d_buf + 2 * h] << 8 | t.pending_buf[t.d_buf + 2 * h + 1], i = t.pending_buf[t.l_buf + h], h++, 0 === n ? E(t, i, e) : (E(t, (a = _[i]) + s + 1, e), 0 !== (o = u[a]) && C(t, i -= g[a], o), E(t, a = S(--n), r), 0 !== (o = l[a]) && C(t, n -= w[a], o)), h < t.last_lit;);
+                        E(t, 256, e)
+                    }
 
-                process.nextTick = function(fun) {
-                    var args = new Array(arguments.length - 1);
-                    if (arguments.length > 1) {
-                        for (var i = 1; i < arguments.length; i++) {
-                            args[i - 1] = arguments[i];
-                        }
-                    }
-                    queue.push(new Item(fun, args));
-                    if (queue.length === 1 && !draining) {
-                        runTimeout(drainQueue);
-                    }
-                };
-
-                // v8 likes predictible objects
-                function Item(fun, array) {
-                    this.fun = fun;
-                    this.array = array;
-                }
-                Item.prototype.run = function() {
-                    this.fun.apply(null, this.array);
-                };
-                process.title = 'browser';
-                process.browser = true;
-                process.env = {};
-                process.argv = [];
-                process.version = ''; // empty string to avoid regexp issues
-                process.versions = {};
-
-                function noop() {}
-
-                process.on = noop;
-                process.addListener = noop;
-                process.once = noop;
-                process.off = noop;
-                process.removeListener = noop;
-                process.removeAllListeners = noop;
-                process.emit = noop;
-                process.prependListener = noop;
-                process.prependOnceListener = noop;
+                    function F(t, e) {
+                        var r, n, i, s = e.dyn_tree,
+                            a = e.stat_desc.static_tree,
+                            o = e.stat_desc.has_stree,
+                            u = e.stat_desc.elems,
+                            l = -1;
+                        for (t.heap_len = 0, t.heap_max = 573, r = 0; r < u; r++) 0 !== s[2 * r] ? (t.heap[++t.heap_len] = l = r, t.depth[r] = 0) : s[2 * r + 1] = 0;
+                        for (; t.heap_len < 2;) s[2 * (i = t.heap[++t.heap_len] = l < 2 ? ++l : 0)] = 1, t.depth[i] = 0, t.opt_len--, o && (t.static_len -= a[2 * i + 1]);
+                        for (e.max_code = l, r = t.heap_len >> 1; 1 <= r; r--) R(t, s, r);
+                        for (i = u; r = t.heap[1], t.heap[1] = t.heap[t.heap_len--], R(t, s, 1), n = t.heap[1], t.heap[--t.heap_max] = r, t.heap[--t.heap_max] = n, s[2 * i] = s[2 * r] + s[2 * n], t.depth[i] = (t.depth[r] >= t.depth[n] ? t.depth[r] : t.depth[n]) + 1, s[2 * r + 1] = s[2 * n + 1] = i, t.heap[1] = i++, R(t, s, 1), 2 <= t.heap_len;);
+                        t.heap[--t.heap_max] = t.heap[1],
+                            function(t, e) {
+                                var r, n, i, s, a, o, u = e.dyn_tree,
+                                    l = e.max_code,
+                                    f = e.stat_desc.static_tree,
+                                    c = e.stat_desc.has_stree,
+                                    d = e.stat_desc.extra_bits,
+                                    p = e.stat_desc.extra_base,
+                                    m = e.stat_desc.max_length,
+                                    _ = 0;
+                                for (s = 0; s <= h; s++) t.bl_count[s] = 0;
+                                for (u[2 * t.heap[t.heap_max] + 1] = 0, r = t.heap_max + 1; r < 573; r++) m < (s = u[2 * u[2 * (n = t.heap[r]) + 1] + 1] + 1) && (s = m, _++), u[2 * n + 1] = s, l < n || (t.bl_count[s]++, a = 0, p <= n && (a = d[n - p]), o = u[2 * n], t.opt_len += o * (s + a), c && (t.static_len += o * (f[2 * n + 1] + a)));
+                                if (0 !== _) {
+                                    do {
+                                        for (s = m - 1; 0 === t.bl_count[s];) s--;
+                                        t.bl_count[s]--, t.bl_count[s + 1] += 2, t.bl_count[m]--, _ -= 2
+                                    } while (0 < _);
+                                    for (s = m; 0 !== s; s--)
+                                        for (n = t.bl_count[s]; 0 !== n;) l < (i = t.heap[--r]) || (u[2 * i + 1] !== s && (t.opt_len += (s - u[2 * i + 1]) * u[2 * i], u[2 * i + 1] = s), n--)
+                                }
+                            }(t, e), I(s, l, t.bl_count)
+                    }
 
-                process.listeners = function(name) {
-                    return []
-                }
+                    function N(t, e, r) {
+                        var n, i, s = -1,
+                            a = e[1],
+                            o = 0,
+                            h = 7,
+                            u = 4;
+                        for (0 === a && (h = 138, u = 3), e[2 * (r + 1) + 1] = 65535, n = 0; n <= r; n++) i = a, a = e[2 * (n + 1) + 1], ++o < h && i === a || (o < u ? t.bl_tree[2 * i] += o : 0 !== i ? (i !== s && t.bl_tree[2 * i]++, t.bl_tree[32]++) : o <= 10 ? t.bl_tree[34]++ : t.bl_tree[36]++, s = i, u = (o = 0) === a ? (h = 138, 3) : i === a ? (h = 6, 3) : (h = 7, 4))
+                    }
 
-                process.binding = function(name) {
-                    throw new Error('process.binding is not supported');
-                };
-
-                process.cwd = function() {
-                    return '/'
-                };
-                process.chdir = function(dir) {
-                    throw new Error('process.chdir is not supported');
-                };
-                process.umask = function() {
-                    return 0;
-                };
+                    function U(t, e, r) {
+                        var n, i, s = -1,
+                            a = e[1],
+                            o = 0,
+                            h = 7,
+                            u = 4;
+                        for (0 === a && (h = 138, u = 3), n = 0; n <= r; n++)
+                            if (i = a, a = e[2 * (n + 1) + 1], !(++o < h && i === a)) {
+                                if (o < u)
+                                    for (; E(t, i, t.bl_tree), 0 != --o;);
+                                else 0 !== i ? (i !== s && (E(t, i, t.bl_tree), o--), E(t, 16, t.bl_tree), C(t, o - 3, 2)) : o <= 10 ? (E(t, 17, t.bl_tree), C(t, o - 3, 3)) : (E(t, 18, t.bl_tree), C(t, o - 11, 7));
+                                s = i, u = (o = 0) === a ? (h = 138, 3) : i === a ? (h = 6, 3) : (h = 7, 4)
+                            }
+                    }
+                    i(w);
+                    var P = !1;
+
+                    function L(t, e, r, i) {
+                        C(t, 0 + (i ? 1 : 0), 3),
+                            function(t, e, r, i) {
+                                B(t), z(t, r), z(t, ~r), n.arraySet(t.pending_buf, t.window, e, r, t.pending), t.pending += r
+                            }(t, e, r)
+                    }
+                    r._tr_init = function(t) {
+                        P || (function() {
+                            var t, e, r, n, i, s = new Array(16);
+                            for (n = r = 0; n < 28; n++)
+                                for (g[n] = r, t = 0; t < 1 << u[n]; t++) _[r++] = n;
+                            for (_[r - 1] = n, n = i = 0; n < 16; n++)
+                                for (w[n] = i, t = 0; t < 1 << l[n]; t++) m[i++] = n;
+                            for (i >>= 7; n < o; n++)
+                                for (w[n] = i << 7, t = 0; t < 1 << l[n] - 7; t++) m[256 + i++] = n;
+                            for (e = 0; e <= h; e++) s[e] = 0;
+                            for (t = 0; t <= 143;) d[2 * t + 1] = 8, t++, s[8]++;
+                            for (; t <= 255;) d[2 * t + 1] = 9, t++, s[9]++;
+                            for (; t <= 279;) d[2 * t + 1] = 7, t++, s[7]++;
+                            for (; t <= 287;) d[2 * t + 1] = 8, t++, s[8]++;
+                            for (I(d, 287, s), t = 0; t < o; t++) p[2 * t + 1] = 5, p[2 * t] = A(t, 5);
+                            b = new k(d, u, 257, a, h), v = new k(p, l, 0, o, h), y = new k(new Array(0), f, 0, 19, 7)
+                        }(), P = !0), t.l_desc = new x(t.dyn_ltree, b), t.d_desc = new x(t.dyn_dtree, v), t.bl_desc = new x(t.bl_tree, y), t.bi_buf = 0, t.bi_valid = 0, O(t)
+                    }, r._tr_stored_block = L, r._tr_flush_block = function(t, e, r, n) {
+                        var i, a, o = 0;
+                        0 < t.level ? (2 === t.strm.data_type && (t.strm.data_type = function(t) {
+                            var e, r = 4093624447;
+                            for (e = 0; e <= 31; e++, r >>>= 1)
+                                if (1 & r && 0 !== t.dyn_ltree[2 * e]) return 0;
+                            if (0 !== t.dyn_ltree[18] || 0 !== t.dyn_ltree[20] || 0 !== t.dyn_ltree[26]) return 1;
+                            for (e = 32; e < s; e++)
+                                if (0 !== t.dyn_ltree[2 * e]) return 1;
+                            return 0
+                        }(t)), F(t, t.l_desc), F(t, t.d_desc), o = function(t) {
+                            var e;
+                            for (N(t, t.dyn_ltree, t.l_desc.max_code), N(t, t.dyn_dtree, t.d_desc.max_code), F(t, t.bl_desc), e = 18; 3 <= e && 0 === t.bl_tree[2 * c[e] + 1]; e--);
+                            return t.opt_len += 3 * (e + 1) + 5 + 5 + 4, e
+                        }(t), i = t.opt_len + 3 + 7 >>> 3, (a = t.static_len + 3 + 7 >>> 3) <= i && (i = a)) : i = a = r + 5, r + 4 <= i && -1 !== e ? L(t, e, r, n) : 4 === t.strategy || a === i ? (C(t, 2 + (n ? 1 : 0), 3), D(t, d, p)) : (C(t, 4 + (n ? 1 : 0), 3), function(t, e, r, n) {
+                            var i;
+                            for (C(t, e - 257, 5), C(t, r - 1, 5), C(t, n - 4, 4), i = 0; i < n; i++) C(t, t.bl_tree[2 * c[i] + 1], 3);
+                            U(t, t.dyn_ltree, e - 1), U(t, t.dyn_dtree, r - 1)
+                        }(t, t.l_desc.max_code + 1, t.d_desc.max_code + 1, o + 1), D(t, t.dyn_ltree, t.dyn_dtree)), O(t), n && B(t)
+                    }, r._tr_tally = function(t, e, r) {
+                        return t.pending_buf[t.d_buf + 2 * t.last_lit] = e >>> 8 & 255, t.pending_buf[t.d_buf + 2 * t.last_lit + 1] = 255 & e, t.pending_buf[t.l_buf + t.last_lit] = 255 & r, t.last_lit++, 0 === e ? t.dyn_ltree[2 * r]++ : (t.matches++, e--, t.dyn_ltree[2 * (_[r] + s + 1)]++, t.dyn_dtree[2 * S(e)]++), t.last_lit === t.lit_bufsize - 1
+                    }, r._tr_align = function(t) {
+                        C(t, 2, 3), E(t, 256, d),
+                            function(t) {
+                                16 === t.bi_valid ? (z(t, t.bi_buf), t.bi_buf = 0, t.bi_valid = 0) : 8 <= t.bi_valid && (t.pending_buf[t.pending++] = 255 & t.bi_buf, t.bi_buf >>= 8, t.bi_valid -= 8)
+                            }(t)
+                    }
+                }, {
+                    "../utils/common": 41
+                }],
+                53: [function(t, e, r) {
+                    "use strict";
+                    e.exports = function() {
+                        this.input = null, this.next_in = 0, this.avail_in = 0, this.total_in = 0, this.output = null, this.next_out = 0, this.avail_out = 0, this.total_out = 0, this.msg = "", this.state = null, this.data_type = 2, this.adler = 0
+                    }
+                }, {}],
+                54: [function(t, e, i) {
+                    (function(t) {
+                        ! function(t, e) {
+                            "use strict";
+                            if (!t.setImmediate) {
+                                var r, i, s, a, o = 1,
+                                    h = {},
+                                    u = !1,
+                                    l = t.document,
+                                    f = Object.getPrototypeOf && Object.getPrototypeOf(t);
+                                f = f && f.setTimeout ? f : t, r = "[object process]" === {}.toString.call(t.process) ? function(t) {
+                                    n.nextTick((function() {
+                                        d(t)
+                                    }))
+                                } : function() {
+                                    if (t.postMessage && !t.importScripts) {
+                                        var e = !0,
+                                            r = t.onmessage;
+                                        return t.onmessage = function() {
+                                            e = !1
+                                        }, t.postMessage("", "*"), t.onmessage = r, e
+                                    }
+                                }() ? (a = "setImmediate$" + Math.random() + "$", t.addEventListener ? t.addEventListener("message", p, !1) : t.attachEvent("onmessage", p), function(e) {
+                                    t.postMessage(a + e, "*")
+                                }) : t.MessageChannel ? ((s = new MessageChannel).port1.onmessage = function(t) {
+                                    d(t.data)
+                                }, function(t) {
+                                    s.port2.postMessage(t)
+                                }) : l && "onreadystatechange" in l.createElement("script") ? (i = l.documentElement, function(t) {
+                                    var e = l.createElement("script");
+                                    e.onreadystatechange = function() {
+                                        d(t), e.onreadystatechange = null, i.removeChild(e), e = null
+                                    }, i.appendChild(e)
+                                }) : function(t) {
+                                    setTimeout(d, 0, t)
+                                }, f.setImmediate = function(t) {
+                                    "function" != typeof t && (t = new Function("" + t));
+                                    for (var e = new Array(arguments.length - 1), n = 0; n < e.length; n++) e[n] = arguments[n + 1];
+                                    var i = {
+                                        callback: t,
+                                        args: e
+                                    };
+                                    return h[o] = i, r(o), o++
+                                }, f.clearImmediate = c
+                            }
+
+                            function c(t) {
+                                delete h[t]
+                            }
 
+                            function d(t) {
+                                if (u) setTimeout(d, 0, t);
+                                else {
+                                    var e = h[t];
+                                    if (e) {
+                                        u = !0;
+                                        try {
+                                            ! function(t) {
+                                                var e = t.callback,
+                                                    r = t.args;
+                                                switch (r.length) {
+                                                    case 0:
+                                                        e();
+                                                        break;
+                                                    case 1:
+                                                        e(r[0]);
+                                                        break;
+                                                    case 2:
+                                                        e(r[0], r[1]);
+                                                        break;
+                                                    case 3:
+                                                        e(r[0], r[1], r[2]);
+                                                        break;
+                                                    default:
+                                                        e.apply(undefined, r)
+                                                }
+                                            }(e)
+                                        } finally {
+                                            c(t), u = !1
+                                        }
+                                    }
+                                }
+                            }
 
-                /***/
-            })
+                            function p(e) {
+                                e.source === t && "string" == typeof e.data && 0 === e.data.indexOf(a) && d(+e.data.slice(a.length))
+                            }
+                        }("undefined" == typeof self ? void 0 === t ? this : t : self)
+                    }).call(this, void 0 !== r.g ? r.g : "undefined" != typeof self ? self : "undefined" != typeof window ? window : {})
+                }, {}]
+            }, {}, [10])(10)
+        },
+        4155: t => {
+            var e, r, n = t.exports = {};
+
+            function i() {
+                throw new Error("setTimeout has not been defined")
+            }
+
+            function s() {
+                throw new Error("clearTimeout has not been defined")
+            }
+
+            function a(t) {
+                if (e === setTimeout) return setTimeout(t, 0);
+                if ((e === i || !e) && setTimeout) return e = setTimeout, setTimeout(t, 0);
+                try {
+                    return e(t, 0)
+                } catch (r) {
+                    try {
+                        return e.call(null, t, 0)
+                    } catch (r) {
+                        return e.call(this, t, 0)
+                    }
+                }
+            }! function() {
+                try {
+                    e = "function" == typeof setTimeout ? setTimeout : i
+                } catch (t) {
+                    e = i
+                }
+                try {
+                    r = "function" == typeof clearTimeout ? clearTimeout : s
+                } catch (t) {
+                    r = s
+                }
+            }();
+            var o, h = [],
+                u = !1,
+                l = -1;
+
+            function f() {
+                u && o && (u = !1, o.length ? h = o.concat(h) : l = -1, h.length && c())
+            }
+
+            function c() {
+                if (!u) {
+                    var t = a(f);
+                    u = !0;
+                    for (var e = h.length; e;) {
+                        for (o = h, h = []; ++l < e;) o && o[l].run();
+                        l = -1, e = h.length
+                    }
+                    o = null, u = !1,
+                        function(t) {
+                            if (r === clearTimeout) return clearTimeout(t);
+                            if ((r === s || !r) && clearTimeout) return r = clearTimeout, clearTimeout(t);
+                            try {
+                                r(t)
+                            } catch (e) {
+                                try {
+                                    return r.call(null, t)
+                                } catch (e) {
+                                    return r.call(this, t)
+                                }
+                            }
+                        }(t)
+                }
+            }
 
+            function d(t, e) {
+                this.fun = t, this.array = e
+            }
+
+            function p() {}
+            n.nextTick = function(t) {
+                var e = new Array(arguments.length - 1);
+                if (arguments.length > 1)
+                    for (var r = 1; r < arguments.length; r++) e[r - 1] = arguments[r];
+                h.push(new d(t, e)), 1 !== h.length || u || a(c)
+            }, d.prototype.run = function() {
+                this.fun.apply(null, this.array)
+            }, n.title = "browser", n.browser = !0, n.env = {}, n.argv = [], n.version = "", n.versions = {}, n.on = p, n.addListener = p, n.once = p, n.off = p, n.removeListener = p, n.removeAllListeners = p, n.emit = p, n.prependListener = p, n.prependOnceListener = p, n.listeners = function(t) {
+                return []
+            }, n.binding = function(t) {
+                throw new Error("process.binding is not supported")
+            }, n.cwd = function() {
+                return "/"
+            }, n.chdir = function(t) {
+                throw new Error("process.chdir is not supported")
+            }, n.umask = function() {
+                return 0
+            }
+        }
     }
-]);
-//# sourceMappingURL=vendors-node_modules_jszip_dist_jszip_min_js.b3f8875733e3ec888679.js.map
+]);
```

### Comparing `jupyterlab_training-0.3.0/jupyterlab_training.egg-info/PKG-INFO` & `jupyterlab_training-0.3.1/jupyterlab_training.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-training
-Version: 0.3.0
+Version: 0.3.1
 Summary: jupyterlab training courses and exercices platform
 Home-page: https://gitlab.com/logilab/jupyterlab-training
 Author: Logilab
 Author-email: ogiorgis@logilab.fr
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `jupyterlab_training-0.3.0/jupyterlab_training.egg-info/SOURCES.txt` & `jupyterlab_training-0.3.1/jupyterlab_training.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -13,40 +13,31 @@
 jupyterlab_training/handlers.py
 jupyterlab_training.egg-info/PKG-INFO
 jupyterlab_training.egg-info/SOURCES.txt
 jupyterlab_training.egg-info/dependency_links.txt
 jupyterlab_training.egg-info/not-zip-safe
 jupyterlab_training.egg-info/requires.txt
 jupyterlab_training.egg-info/top_level.txt
-jupyterlab_training/labextension/build_log.json
 jupyterlab_training/labextension/package.json
+jupyterlab_training/labextension/static/147.61d247f0dd79cb5e6c03.js
+jupyterlab_training/labextension/static/147.61d247f0dd79cb5e6c03.js.LICENSE.txt
+jupyterlab_training/labextension/static/162.54797b341de4f60c5f53.js
+jupyterlab_training/labextension/static/169.dde25e4dfa365788e2d3.js
+jupyterlab_training/labextension/static/3.97e5ce5c6c551fd93ee6.js
+jupyterlab_training/labextension/static/320.e87de993e15ebd1d087e.js
+jupyterlab_training/labextension/static/320.e87de993e15ebd1d087e.js.LICENSE.txt
+jupyterlab_training/labextension/static/490.76b7872fc9815805fce9.js
+jupyterlab_training/labextension/static/71.b08e1d3adafbcb17349c.js
+jupyterlab_training/labextension/static/733.c4acd437d42492321d94.js
+jupyterlab_training/labextension/static/733.c4acd437d42492321d94.js.LICENSE.txt
+jupyterlab_training/labextension/static/747.d4b5f772f188f310ccf4.js
 jupyterlab_training/labextension/static/9c539cf459fdeaebf6835c214cb5cac1d43cd5d497cf4b96647401981d180043.png
-jupyterlab_training/labextension/static/lib_index_js.2449aa1867353f272d86.js
-jupyterlab_training/labextension/static/lib_index_js.2449aa1867353f272d86.js.map
-jupyterlab_training/labextension/static/node_modules_file-saver_dist_FileSaver_min_js.7a6e01f58ee54adc0a2d.js
-jupyterlab_training/labextension/static/node_modules_file-saver_dist_FileSaver_min_js.7a6e01f58ee54adc0a2d.js.map
-jupyterlab_training/labextension/static/remoteEntry.a514b68d4bfa7874093f.js
-jupyterlab_training/labextension/static/remoteEntry.a514b68d4bfa7874093f.js.map
+jupyterlab_training/labextension/static/remoteEntry.1860e2c61e01ab7c6b1c.js
 jupyterlab_training/labextension/static/style.js
-jupyterlab_training/labextension/static/style_index_js.90cbacf63e7b78baf3a0.js
-jupyterlab_training/labextension/static/style_index_js.90cbacf63e7b78baf3a0.js.map
-jupyterlab_training/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b34d146cd46239887005.js
-jupyterlab_training/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b34d146cd46239887005.js.map
-jupyterlab_training/labextension/static/vendors-node_modules_i18next-browser-languagedetector_dist_esm_i18nextBrowserLanguageDetector_js.461ad3153f790b00e805.js
-jupyterlab_training/labextension/static/vendors-node_modules_i18next-browser-languagedetector_dist_esm_i18nextBrowserLanguageDetector_js.461ad3153f790b00e805.js.map
-jupyterlab_training/labextension/static/vendors-node_modules_i18next_dist_esm_i18next_js.a7d4998d1b735c7aa976.js
-jupyterlab_training/labextension/static/vendors-node_modules_i18next_dist_esm_i18next_js.a7d4998d1b735c7aa976.js.map
-jupyterlab_training/labextension/static/vendors-node_modules_js-yaml_index_js.d7ae774bce0e28557217.js
-jupyterlab_training/labextension/static/vendors-node_modules_js-yaml_index_js.d7ae774bce0e28557217.js.map
-jupyterlab_training/labextension/static/vendors-node_modules_jszip_dist_jszip_min_js.b3f8875733e3ec888679.js
-jupyterlab_training/labextension/static/vendors-node_modules_jszip_dist_jszip_min_js.b3f8875733e3ec888679.js.map
-jupyterlab_training/labextension/static/vendors-node_modules_luxon_build_cjs-browser_luxon_js.fe773dc86647f20d9d58.js
-jupyterlab_training/labextension/static/vendors-node_modules_luxon_build_cjs-browser_luxon_js.fe773dc86647f20d9d58.js.map
-jupyterlab_training/labextension/static/vendors-node_modules_react-bootstrap_esm_index_js.6fbf310996ef2effea89.js
-jupyterlab_training/labextension/static/vendors-node_modules_react-bootstrap_esm_index_js.6fbf310996ef2effea89.js.map
+jupyterlab_training/labextension/static/third-party-licenses.json
 src/flake8.tsx
 src/index.ts
 src/menu.tsx
 src/model.tsx
 src/panel.tsx
 src/progressButton.tsx
 src/statsWidget.tsx
```

### Comparing `jupyterlab_training-0.3.0/package.json` & `jupyterlab_training-0.3.1/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.3.1'"}*

```diff
@@ -96,9 +96,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.0"
+    "version": "0.3.1"
 }
```

### Comparing `jupyterlab_training-0.3.0/pyproject.toml` & `jupyterlab_training-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/setup.py` & `jupyterlab_training-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/src/flake8.tsx` & `jupyterlab_training-0.3.1/src/flake8.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/src/i18n/index.ts` & `jupyterlab_training-0.3.1/src/i18n/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/src/index.ts` & `jupyterlab_training-0.3.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/src/menu.tsx` & `jupyterlab_training-0.3.1/src/menu.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/src/model.tsx` & `jupyterlab_training-0.3.1/src/model.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/src/panel.tsx` & `jupyterlab_training-0.3.1/src/panel.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/src/progressButton.tsx` & `jupyterlab_training-0.3.1/src/progressButton.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/src/statsWidget.tsx` & `jupyterlab_training-0.3.1/src/statsWidget.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/src/tour.tsx` & `jupyterlab_training-0.3.1/src/tour.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/src/utils.tsx` & `jupyterlab_training-0.3.1/src/utils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/.eslintrc.json` & `jupyterlab_training-0.3.1/style/bootstrap/.eslintrc.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/.github/CONTRIBUTING.md` & `jupyterlab_training-0.3.1/style/bootstrap/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/.github/ISSUE_TEMPLATE.md` & `jupyterlab_training-0.3.1/style/bootstrap/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/.gitignore` & `jupyterlab_training-0.3.1/style/bootstrap/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/.stylelintrc` & `jupyterlab_training-0.3.1/style/bootstrap/.stylelintrc`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/.travis.yml` & `jupyterlab_training-0.3.1/style/bootstrap/.travis.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/CODE_OF_CONDUCT.md` & `jupyterlab_training-0.3.1/style/bootstrap/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/Gemfile.lock` & `jupyterlab_training-0.3.1/style/bootstrap/Gemfile.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/LICENSE` & `jupyterlab_training-0.3.1/style/bootstrap/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/README.md` & `jupyterlab_training-0.3.1/style/bootstrap/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_config.yml` & `jupyterlab_training-0.3.1/style/bootstrap/_config.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_data/browser-bugs.yml` & `jupyterlab_training-0.3.1/style/bootstrap/_data/browser-bugs.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_data/browser-features.yml` & `jupyterlab_training-0.3.1/style/bootstrap/_data/browser-features.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_data/examples.yml` & `jupyterlab_training-0.3.1/style/bootstrap/_data/examples.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_data/nav.yml` & `jupyterlab_training-0.3.1/style/bootstrap/_data/nav.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_data/translations.yml` & `jupyterlab_training-0.3.1/style/bootstrap/_data/translations.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_includes/docs-navbar.html` & `jupyterlab_training-0.3.1/style/bootstrap/_includes/docs-navbar.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_includes/docs-sidebar.html` & `jupyterlab_training-0.3.1/style/bootstrap/_includes/docs-sidebar.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_includes/favicons.html` & `jupyterlab_training-0.3.1/style/bootstrap/_includes/favicons.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_includes/footer.html` & `jupyterlab_training-0.3.1/style/bootstrap/_includes/footer.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_includes/header.html` & `jupyterlab_training-0.3.1/style/bootstrap/_includes/header.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_includes/icons/bootstrap.svg` & `jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/bootstrap.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_includes/icons/github.svg` & `jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/github.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_includes/icons/slack.svg` & `jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/slack.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_includes/icons/twitter.svg` & `jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/twitter.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_includes/scripts.html` & `jupyterlab_training-0.3.1/style/bootstrap/_includes/scripts.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_includes/social.html` & `jupyterlab_training-0.3.1/style/bootstrap/_includes/social.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_layouts/default.html` & `jupyterlab_training-0.3.1/style/bootstrap/_layouts/default.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_layouts/docs.html` & `jupyterlab_training-0.3.1/style/bootstrap/_layouts/docs.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_layouts/examples.html` & `jupyterlab_training-0.3.1/style/bootstrap/_layouts/examples.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_layouts/redirect.html` & `jupyterlab_training-0.3.1/style/bootstrap/_layouts/redirect.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_plugins/bugify.rb` & `jupyterlab_training-0.3.1/style/bootstrap/_plugins/bugify.rb`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_plugins/callout.rb` & `jupyterlab_training-0.3.1/style/bootstrap/_plugins/callout.rb`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_plugins/example.rb` & `jupyterlab_training-0.3.1/style/bootstrap/_plugins/example.rb`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/_plugins/markdown-block.rb` & `jupyterlab_training-0.3.1/style/bootstrap/_plugins/markdown-block.rb`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/brand/bootstrap-outline.svg` & `jupyterlab_training-0.3.1/style/bootstrap/assets/brand/bootstrap-outline.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/brand/bootstrap-punchout.svg` & `jupyterlab_training-0.3.1/style/bootstrap/assets/brand/bootstrap-punchout.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/brand/bootstrap-social-logo.png` & `jupyterlab_training-0.3.1/style/bootstrap/assets/brand/bootstrap-social-logo.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/brand/bootstrap-social.png` & `jupyterlab_training-0.3.1/style/bootstrap/assets/brand/bootstrap-social.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/brand/bootstrap-solid.svg` & `jupyterlab_training-0.3.1/style/bootstrap/assets/brand/bootstrap-solid.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/css/docs.min.css` & `jupyterlab_training-0.3.1/style/bootstrap/assets/css/docs.min.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/css/docs.min.css.map` & `jupyterlab_training-0.3.1/style/bootstrap/assets/css/docs.min.css.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/img/bootstrap-stack.png` & `jupyterlab_training-0.3.1/style/bootstrap/assets/img/bootstrap-stack.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/img/bootstrap-themes.png` & `jupyterlab_training-0.3.1/style/bootstrap/assets/img/bootstrap-themes.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/android-chrome-192x192.png` & `jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/android-chrome-512x512.png` & `jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/apple-touch-icon.png` & `jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/manifest.json` & `jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/manifest.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/mstile-144x144.png` & `jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/mstile-144x144.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/mstile-150x150.png` & `jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/mstile-310x150.png` & `jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/mstile-310x150.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/mstile-310x310.png` & `jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/mstile-310x310.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/mstile-70x70.png` & `jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/mstile-70x70.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/img/favicons/safari-pinned-tab.svg` & `jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/js/docs.min.js` & `jupyterlab_training-0.3.1/style/bootstrap/assets/js/docs.min.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/js/src/application.js` & `jupyterlab_training-0.3.1/style/bootstrap/assets/js/src/application.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/js/src/ie-emulation-modes-warning.js` & `jupyterlab_training-0.3.1/style/bootstrap/assets/js/src/ie-emulation-modes-warning.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/js/src/pwa.js` & `jupyterlab_training-0.3.1/style/bootstrap/assets/js/src/pwa.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/js/vendor/anchor.min.js` & `jupyterlab_training-0.3.1/style/bootstrap/assets/js/vendor/anchor.min.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/js/vendor/clipboard.min.js` & `jupyterlab_training-0.3.1/style/bootstrap/assets/js/vendor/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/js/vendor/holder.min.js` & `jupyterlab_training-0.3.1/style/bootstrap/assets/js/vendor/holder.min.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/js/vendor/jquery-slim.min.js` & `jupyterlab_training-0.3.1/style/bootstrap/assets/js/vendor/jquery-slim.min.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/js/vendor/popper.min.js` & `jupyterlab_training-0.3.1/style/bootstrap/assets/js/vendor/popper.min.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_ads.scss` & `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_ads.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_algolia.scss` & `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_algolia.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_brand.scss` & `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_brand.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_callouts.scss` & `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_callouts.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_clipboard-js.scss` & `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_clipboard-js.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_component-examples.scss` & `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_component-examples.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_content.scss` & `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_content.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_masthead.scss` & `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_masthead.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_nav.scss` & `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_sidebar.scss` & `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_sidebar.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/scss/_syntax.scss` & `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_syntax.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/assets/scss/docs.scss` & `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/docs.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/build/.htmllintrc` & `jupyterlab_training-0.3.1/style/bootstrap/build/.htmllintrc`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/build/change-version.js` & `jupyterlab_training-0.3.1/style/bootstrap/build/change-version.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/build/gcp-key.json.enc` & `jupyterlab_training-0.3.1/style/bootstrap/build/gcp-key.json.enc`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/build/generate-sri.js` & `jupyterlab_training-0.3.1/style/bootstrap/build/generate-sri.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/build/lint-vars.js` & `jupyterlab_training-0.3.1/style/bootstrap/build/lint-vars.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/build/rollup.config.js` & `jupyterlab_training-0.3.1/style/bootstrap/build/rollup.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/build/sauce_browsers.json` & `jupyterlab_training-0.3.1/style/bootstrap/build/sauce_browsers.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/build/saucelabs-unit-test.js` & `jupyterlab_training-0.3.1/style/bootstrap/build/saucelabs-unit-test.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/build/ship.sh` & `jupyterlab_training-0.3.1/style/bootstrap/build/ship.sh`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/build/upload-preview.sh` & `jupyterlab_training-0.3.1/style/bootstrap/build/upload-preview.sh`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/build/vnu-jar.js` & `jupyterlab_training-0.3.1/style/bootstrap/build/vnu-jar.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/build/workbox.js` & `jupyterlab_training-0.3.1/style/bootstrap/build/workbox.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/composer.json` & `jupyterlab_training-0.3.1/style/bootstrap/composer.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap-grid.css` & `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap-grid.css.map` & `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap-grid.min.css` & `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap-grid.min.css.map` & `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap-reboot.css` & `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap-reboot.css.map` & `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap-reboot.min.css` & `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap-reboot.min.css.map` & `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap.css` & `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap.css.map` & `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap.min.css` & `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/dist/css/bootstrap.min.css.map` & `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/dist/js/bootstrap.bundle.js` & `jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/dist/js/bootstrap.bundle.js.map` & `jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/dist/js/bootstrap.bundle.min.js` & `jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/dist/js/bootstrap.bundle.min.js.map` & `jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/dist/js/bootstrap.js` & `jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/dist/js/bootstrap.js.map` & `jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/dist/js/bootstrap.min.js` & `jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/dist/js/bootstrap.min.js.map` & `jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/about/brand.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/about/brand.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/about/license.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/about/license.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/about/overview.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/about/overview.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/about/translations.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/about/translations.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/browser-bugs.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/browser-bugs.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/alerts.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/alerts.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/badge.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/badge.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/breadcrumb.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/breadcrumb.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/button-group.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/button-group.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/buttons.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/buttons.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/card.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/card.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/carousel.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/carousel.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/collapse.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/collapse.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/dropdowns.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/dropdowns.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/forms.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/forms.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/input-group.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/input-group.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/jumbotron.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/jumbotron.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/list-group.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/list-group.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/modal.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/modal.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/navbar.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/navbar.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/navs.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/navs.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/pagination.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/pagination.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/popovers.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/popovers.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/progress.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/progress.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/scrollspy.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/scrollspy.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/components/tooltips.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/tooltips.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/content/code.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/code.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/content/figures.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/figures.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/content/images.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/images.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/content/reboot.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/reboot.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/content/tables.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/tables.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/content/typography.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/typography.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/album/album.css` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/album/album.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/album/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/album/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/blog/blog.css` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/blog/blog.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/blog/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/blog/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/carousel/carousel.css` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/carousel/carousel.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/carousel/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/carousel/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/checkout/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/checkout/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/cover/cover.css` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/cover/cover.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/cover/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/cover/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/dashboard/dashboard.css` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/dashboard/dashboard.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/dashboard/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/dashboard/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/floating-labels/floating-labels.css` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/floating-labels/floating-labels.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/floating-labels/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/floating-labels/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/grid/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/grid/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/jumbotron/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/jumbotron/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/navbar-bottom/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbar-bottom/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/navbar-fixed/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbar-fixed/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/navbar-static/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbar-static/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/navbars/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbars/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/offcanvas/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/offcanvas/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/offcanvas/offcanvas.css` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/offcanvas/offcanvas.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/pricing/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/pricing/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/product/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/product/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/product/product.css` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/product/product.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/album.png` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/album.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/blog.png` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/blog.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/carousel.png` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/carousel.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/checkout.png` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/checkout.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/cover.png` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/cover.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/dashboard.png` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/dashboard.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/floating-labels.png` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/floating-labels.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/grid.png` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/grid.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/jumbotron.png` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/jumbotron.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/navbar-bottom.png` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/navbar-bottom.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/navbar-fixed.png` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/navbar-fixed.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/navbar-static.png` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/navbar-static.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/navbars.png` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/navbars.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/offcanvas.png` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/offcanvas.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/pricing.png` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/pricing.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/product.png` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/product.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/sign-in.png` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/sign-in.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/starter-template.png` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/starter-template.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/sticky-footer-navbar.png` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/sticky-footer-navbar.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/screenshots/sticky-footer.png` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/sticky-footer.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/sign-in/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sign-in/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/sign-in/signin.css` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sign-in/signin.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/starter-template/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/starter-template/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/sticky-footer/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sticky-footer/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/sticky-footer/sticky-footer.css` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sticky-footer/sticky-footer.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/sticky-footer-navbar/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sticky-footer-navbar/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/sticky-footer-navbar/sticky-footer-navbar.css` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sticky-footer-navbar/sticky-footer-navbar.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/tooltip-viewport/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/tooltip-viewport/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/examples/tooltip-viewport/tooltip-viewport.js` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/tooltip-viewport/tooltip-viewport.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/extend/approach.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/extend/approach.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/extend/icons.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/extend/icons.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/getting-started/accessibility.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/accessibility.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/getting-started/best-practices.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/best-practices.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/getting-started/browsers-devices.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/browsers-devices.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/getting-started/build-tools.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/build-tools.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/getting-started/contents.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/contents.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/getting-started/download.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/download.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/getting-started/introduction.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/introduction.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/getting-started/javascript.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/javascript.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/getting-started/theming.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/theming.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/getting-started/webpack.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/webpack.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/layout/grid.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/layout/grid.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/layout/media-object.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/layout/media-object.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/layout/overview.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/layout/overview.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/layout/utilities-for-layout.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/layout/utilities-for-layout.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/migration.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/migration.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/borders.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/borders.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/clearfix.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/clearfix.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/colors.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/colors.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/display.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/display.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/embed.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/embed.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/flex.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/flex.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/float.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/float.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/image-replacement.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/image-replacement.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/position.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/position.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/screenreaders.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/screenreaders.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/sizing.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/sizing.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/spacing.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/spacing.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/text.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/text.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/vertical-align.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/vertical-align.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/docs/4.0/utilities/visibility.md` & `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/visibility.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/favicon.ico` & `jupyterlab_training-0.3.1/style/bootstrap/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/alert.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/alert.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/alert.js.map` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/alert.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/button.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/button.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/button.js.map` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/button.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/carousel.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/carousel.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/carousel.js.map` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/carousel.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/collapse.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/collapse.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/collapse.js.map` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/collapse.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/dropdown.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/dropdown.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/dropdown.js.map` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/dropdown.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/index.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/index.js.map` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/index.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/modal.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/modal.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/modal.js.map` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/modal.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/popover.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/popover.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/popover.js.map` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/popover.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/scrollspy.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/scrollspy.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/scrollspy.js.map` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/scrollspy.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/tab.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/tab.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/tab.js.map` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/tab.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/tooltip.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/tooltip.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/tooltip.js.map` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/tooltip.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/util.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/util.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/dist/util.js.map` & `jupyterlab_training-0.3.1/style/bootstrap/js/dist/util.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/src/alert.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/src/alert.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/src/button.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/src/button.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/src/carousel.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/src/carousel.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/src/collapse.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/src/collapse.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/src/dropdown.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/src/dropdown.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/src/index.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/src/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/src/modal.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/src/modal.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/src/popover.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/src/popover.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/src/scrollspy.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/src/scrollspy.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/src/tab.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/src/tab.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/src/tooltip.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/src/tooltip.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/src/util.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/src/util.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/README.md` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/index.html` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/karma.conf.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/karma.conf.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/.eslintrc.json` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/.eslintrc.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/alert.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/alert.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/button.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/button.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/carousel.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/carousel.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/collapse.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/collapse.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/dropdown.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/dropdown.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/modal.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/modal.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/popover.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/popover.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/scrollspy.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/scrollspy.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/tab.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/tab.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/tooltip.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/tooltip.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/unit/util.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/util.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/vendor/jquery-1.9.1.min.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/vendor/jquery-1.9.1.min.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/vendor/qunit.css` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/vendor/qunit.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/vendor/qunit.js` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/vendor/qunit.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/visual/alert.html` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/alert.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/visual/button.html` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/button.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/visual/carousel.html` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/carousel.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/visual/collapse.html` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/collapse.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/visual/dropdown.html` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/dropdown.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/visual/modal.html` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/modal.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/visual/popover.html` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/popover.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/visual/scrollspy.html` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/scrollspy.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/visual/tab.html` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/tab.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/js/tests/visual/tooltip.html` & `jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/tooltip.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/nuget/MyGet.ps1` & `jupyterlab_training-0.3.1/style/bootstrap/nuget/MyGet.ps1`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/nuget/bootstrap.nuspec` & `jupyterlab_training-0.3.1/style/bootstrap/nuget/bootstrap.nuspec`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/nuget/bootstrap.sass.nuspec` & `jupyterlab_training-0.3.1/style/bootstrap/nuget/bootstrap.sass.nuspec`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/package-lock.json` & `jupyterlab_training-0.3.1/style/bootstrap/package-lock.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/package.js` & `jupyterlab_training-0.3.1/style/bootstrap/package.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/package.json` & `jupyterlab_training-0.3.1/style/bootstrap/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_alert.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_alert.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_badge.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_badge.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_breadcrumb.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_button-group.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_button-group.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_buttons.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_buttons.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_card.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_card.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_carousel.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_carousel.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_close.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_close.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_code.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_code.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_custom-forms.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_custom-forms.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_dropdown.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_forms.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_forms.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_functions.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_functions.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_grid.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_grid.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_images.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_images.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_input-group.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_input-group.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_list-group.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_list-group.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_mixins.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_modal.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_modal.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_nav.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_navbar.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_navbar.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_pagination.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_pagination.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_popover.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_popover.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_print.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_print.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_progress.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_progress.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_reboot.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_reboot.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_root.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_root.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_tables.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_tables.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_tooltip.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_type.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_type.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/_variables.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/bootstrap-grid.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/bootstrap.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_border-radius.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_breakpoints.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_buttons.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_caret.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_forms.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_gradients.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_grid-framework.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_grid-framework.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_grid.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_hover.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_hover.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_image.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_image.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_reset-text.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_reset-text.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_screen-reader.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_screen-reader.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/mixins/_table-row.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_table-row.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/utilities/_borders.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_borders.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/utilities/_display.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_display.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/utilities/_embed.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_embed.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/utilities/_flex.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_flex.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/utilities/_position.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_position.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/utilities/_spacing.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_spacing.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/bootstrap/scss/utilities/_text.scss` & `jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_text.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/homePage.png` & `jupyterlab_training-0.3.1/style/homePage.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/index.css` & `jupyterlab_training-0.3.1/style/index.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/logilab-icon.svg` & `jupyterlab_training-0.3.1/style/logilab-icon.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/logilab.ico` & `jupyterlab_training-0.3.1/style/logilab.ico`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/logilab.svg` & `jupyterlab_training-0.3.1/style/logilab.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/style/stop_app.png` & `jupyterlab_training-0.3.1/style/stop_app.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/tests/test_handlers.py` & `jupyterlab_training-0.3.1/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.0/tsconfig.json` & `jupyterlab_training-0.3.1/tsconfig.json`

 * *Files identical despite different names*

