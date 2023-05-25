# Comparing `tmp/jupyterlab_training-0.3.1.tar.gz` & `tmp/jupyterlab_training-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_training-0.3.1.tar", last modified: Thu May 25 15:00:52 2023, max compression
+gzip compressed data, was "jupyterlab_training-0.3.2.tar", last modified: Thu May 25 15:17:05 2023, max compression
```

## Comparing `jupyterlab_training-0.3.1.tar` & `jupyterlab_training-0.3.2.tar`

### file list

```diff
@@ -1,565 +1,565 @@
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.737838 jupyterlab_training-0.3.1/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1516 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/LICENSE
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      435 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/MANIFEST.in
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3133 2023-05-25 15:00:52.737838 jupyterlab_training-0.3.1/PKG-INFO
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2375 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/README.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      199 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/install.json
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.865829 jupyterlab_training-0.3.1/jupyter-config/
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.869829 jupyterlab_training-0.3.1/jupyter-config/server-config/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       94 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/jupyter-config/server-config/jupyterlab-training.json
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.873829 jupyterlab_training-0.3.1/jupyterlab_training/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4311 2022-04-26 13:53:46.000000 jupyterlab_training-0.3.1/jupyterlab_training/__init__.py
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      473 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/jupyterlab_training/_version.py
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2277 2023-04-14 08:02:10.000000 jupyterlab_training-0.3.1/jupyterlab_training/db.py
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8227 2023-05-25 09:07:08.000000 jupyterlab_training-0.3.1/jupyterlab_training/handlers.py
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.873829 jupyterlab_training-0.3.1/jupyterlab_training/labextension/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3710 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/package.json
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.873829 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   115723 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/147.61d247f0dd79cb5e6c03.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      121 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/147.61d247f0dd79cb5e6c03.js.LICENSE.txt
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2686 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/162.54797b341de4f60c5f53.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    44687 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/169.dde25e4dfa365788e2d3.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   242635 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/3.97e5ce5c6c551fd93ee6.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   197062 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/320.e87de993e15ebd1d087e.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      225 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/320.e87de993e15ebd1d087e.js.LICENSE.txt
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    72799 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/490.76b7872fc9815805fce9.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7272 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/71.b08e1d3adafbcb17349c.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    98509 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/733.c4acd437d42492321d94.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      383 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/733.c4acd437d42492321d94.js.LICENSE.txt
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3378 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/747.d4b5f772f188f310ccf4.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4436 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/9c539cf459fdeaebf6835c214cb5cac1d43cd5d497cf4b96647401981d180043.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9396 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/remoteEntry.1860e2c61e01ab7c6b1c.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      162 2023-05-25 15:00:41.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/style.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    69137 2023-05-25 15:00:47.000000 jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.873829 jupyterlab_training-0.3.1/jupyterlab_training.egg-info/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3133 2023-05-25 15:00:51.000000 jupyterlab_training-0.3.1/jupyterlab_training.egg-info/PKG-INFO
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    21243 2023-05-25 15:00:51.000000 jupyterlab_training-0.3.1/jupyterlab_training.egg-info/SOURCES.txt
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)        1 2023-05-25 15:00:51.000000 jupyterlab_training-0.3.1/jupyterlab_training.egg-info/dependency_links.txt
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)        1 2023-05-25 15:00:51.000000 jupyterlab_training-0.3.1/jupyterlab_training.egg-info/not-zip-safe
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      158 2023-05-25 15:00:51.000000 jupyterlab_training-0.3.1/jupyterlab_training.egg-info/requires.txt
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       20 2023-05-25 15:00:51.000000 jupyterlab_training-0.3.1/jupyterlab_training.egg-info/top_level.txt
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3804 2023-05-25 14:59:50.000000 jupyterlab_training-0.3.1/package.json
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      610 2022-04-26 12:17:31.000000 jupyterlab_training-0.3.1/pyproject.toml
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       38 2023-05-25 15:00:52.737838 jupyterlab_training-0.3.1/setup.cfg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2671 2022-04-26 13:51:23.000000 jupyterlab_training-0.3.1/setup.py
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.873829 jupyterlab_training-0.3.1/src/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1481 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/src/flake8.tsx
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.877829 jupyterlab_training-0.3.1/src/i18n/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    17168 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/src/i18n/index.ts
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3457 2023-04-14 10:37:08.000000 jupyterlab_training-0.3.1/src/index.ts
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7641 2023-05-25 13:39:32.000000 jupyterlab_training-0.3.1/src/menu.tsx
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1870 2023-04-04 13:29:43.000000 jupyterlab_training-0.3.1/src/model.tsx
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    19967 2023-04-05 08:23:46.000000 jupyterlab_training-0.3.1/src/panel.tsx
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4415 2022-04-26 12:49:05.000000 jupyterlab_training-0.3.1/src/progressButton.tsx
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4664 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/src/statsWidget.tsx
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8902 2023-05-09 07:57:45.000000 jupyterlab_training-0.3.1/src/tour.tsx
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1009 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/src/utils.tsx
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.877829 jupyterlab_training-0.3.1/style/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)        0 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/base.css
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.881829 jupyterlab_training-0.3.1/style/bootstrap/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      313 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/.babelrc.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      208 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/.editorconfig
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       56 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/.eslintignore
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7131 2023-04-04 13:29:43.000000 jupyterlab_training-0.3.1/style/bootstrap/.eslintrc.json
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      359 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/.gitattributes
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.881829 jupyterlab_training-0.3.1/style/bootstrap/.github/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    14268 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/.github/CONTRIBUTING.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1178 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      517 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/.gitignore
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       45 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/.stylelintignore
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6685 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/.stylelintrc
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      782 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/.travis.yml
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       17 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/CNAME
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3217 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/CODE_OF_CONDUCT.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      199 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/Gemfile
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1905 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/Gemfile.lock
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1131 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/LICENSE
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9138 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/README.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2505 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_config.yml
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.881829 jupyterlab_training-0.3.1/style/bootstrap/_data/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      418 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_data/breakpoints.yml
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9113 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_data/browser-bugs.yml
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3244 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_data/browser-features.yml
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      401 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_data/colors.yml
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2870 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_data/examples.yml
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      261 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_data/grays.yml
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1657 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_data/nav.yml
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      257 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_data/theme-colors.yml
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      519 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_data/translations.yml
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.881829 jupyterlab_training-0.3.1/style/bootstrap/_includes/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      137 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/ads.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      445 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/callout-danger-async-methods.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      451 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/callout-info-mediaqueries-breakpoints.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      454 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/callout-warning-color-assistive-technologies.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3520 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/docs-navbar.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2269 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/docs-sidebar.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      748 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/favicons.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1148 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/footer.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1540 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/header.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.881829 jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      890 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/bootstrap.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      482 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/download.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1116 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/github.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      441 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/import.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      442 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/lightning.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      410 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/menu.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1362 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/slack.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      861 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/twitter.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1376 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/scripts.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1290 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_includes/social.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.881829 jupyterlab_training-0.3.1/style/bootstrap/_layouts/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      556 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_layouts/default.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1040 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_layouts/docs.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      538 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_layouts/examples.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      412 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_layouts/home.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1134 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_layouts/redirect.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      288 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_layouts/simple.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.885829 jupyterlab_training-0.3.1/style/bootstrap/_plugins/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1326 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_plugins/bugify.rb
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      827 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_plugins/callout.rb
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3402 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_plugins/example.rb
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      525 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/_plugins/markdown-block.rb
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.865829 jupyterlab_training-0.3.1/style/bootstrap/assets/
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.885829 jupyterlab_training-0.3.1/style/bootstrap/assets/brand/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1306 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/brand/bootstrap-outline.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1140 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/brand/bootstrap-punchout.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    23959 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/brand/bootstrap-social-logo.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   231733 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/brand/bootstrap-social.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1127 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/brand/bootstrap-solid.svg
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.885829 jupyterlab_training-0.3.1/style/bootstrap/assets/css/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    21574 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/css/docs.min.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    40321 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/css/docs.min.css.map
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.885829 jupyterlab_training-0.3.1/style/bootstrap/assets/img/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    52160 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/bootstrap-stack.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    80588 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/bootstrap-themes.png
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.885829 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1935 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/android-chrome-192x192.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4269 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/android-chrome-512x512.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1738 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/apple-touch-icon.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      292 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/browserconfig.xml
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      310 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/favicon-16x16.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      491 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/favicon-32x32.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      550 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/manifest.json
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1479 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/mstile-144x144.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1428 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/mstile-150x150.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1746 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/mstile-310x150.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3085 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/mstile-310x310.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1104 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/mstile-70x70.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1025 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/safari-pinned-tab.svg
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.885829 jupyterlab_training-0.3.1/style/bootstrap/assets/js/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      490 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/js/.eslintrc.json
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    52015 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/js/docs.min.js
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.885829 jupyterlab_training-0.3.1/style/bootstrap/assets/js/src/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4518 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/js/src/application.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2005 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/js/src/ie-emulation-modes-warning.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      545 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/js/src/pwa.js
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.885829 jupyterlab_training-0.3.1/style/bootstrap/assets/js/vendor/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5389 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/js/vendor/anchor.min.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10917 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/js/vendor/clipboard.min.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    32283 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/js/vendor/holder.min.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    69597 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/js/vendor/jquery-slim.min.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    19188 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/js/vendor/popper.min.js
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.069831 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      593 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_ads.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3422 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_algolia.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      172 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_anchor.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1827 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_brand.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      195 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_browser-bugs.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      487 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_buttons.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      695 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_callouts.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      574 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_clipboard-js.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      419 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_colors.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6341 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_component-examples.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1995 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_content.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      363 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_examples.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      459 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_footer.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      887 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_masthead.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1685 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_nav.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2724 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_sidebar.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      213 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_skiplink.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1669 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_syntax.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      382 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_variables.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1520 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/assets/scss/docs.scss
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.073831 jupyterlab_training-0.3.1/style/bootstrap/build/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      385 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/.eslintrc.json
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1260 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/.htmllintrc
--rwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)     2758 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/change-version.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2304 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/gcp-key.json.enc
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1505 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/generate-sri.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2070 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/lint-vars.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      238 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/postcss.config.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1379 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/rollup.config.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1221 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/sauce_browsers.json
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3116 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/saucelabs-unit-test.js
--rwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)     2778 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/ship.sh
--rwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)      701 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/upload-preview.sh
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2605 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/vnu-jar.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      156 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/workbox.config.json
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1282 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/build/workbox.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      744 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/composer.json
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.865829 jupyterlab_training-0.3.1/style/bootstrap/dist/
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.077831 jupyterlab_training-0.3.1/style/bootstrap/dist/css/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    43852 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-grid.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    95910 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-grid.css.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    34243 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-grid.min.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    76209 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-grid.min.css.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4798 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-reboot.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    57721 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-reboot.css.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3936 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-reboot.min.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    25881 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   178152 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   411645 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap.css.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   144877 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap.min.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   551641 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap.min.css.map
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.077831 jupyterlab_training-0.3.1/style/bootstrap/dist/js/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   195855 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.bundle.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   326634 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.bundle.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    67742 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.bundle.min.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   273872 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   115048 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   195373 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    48944 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.min.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   161998 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.min.js.map
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.865829 jupyterlab_training-0.3.1/style/bootstrap/docs/
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.077831 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.081831 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/about/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2940 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/about/brand.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1717 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/about/license.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2495 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/about/overview.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      630 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/about/translations.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2474 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/browser-bugs.md
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.081831 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4439 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/alerts.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3450 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/badge.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1503 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/breadcrumb.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9208 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/button-group.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7445 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/buttons.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    26080 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/card.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12440 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/carousel.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12091 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/collapse.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    33022 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/dropdowns.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    51564 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/forms.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12974 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/input-group.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1199 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/jumbotron.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    18093 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/list-group.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    29516 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/modal.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    23281 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/navbar.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    35152 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/navs.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6170 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/pagination.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    15225 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/popovers.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6318 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/progress.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    18827 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/scrollspy.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    15834 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/tooltips.md
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.081831 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1436 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/code.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1329 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/figures.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3349 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/images.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12826 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/reboot.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    16669 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/tables.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10926 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/typography.md
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.121832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      185 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/.eslintrc.json
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      339 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/.stylelintrc
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.125832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/album/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      655 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/album/album.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12744 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/album/index.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.125832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/blog/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2133 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/blog/blog.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12774 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/blog/index.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.125832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/carousel/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1658 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/carousel/carousel.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10159 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/carousel/index.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.125832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/checkout/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      287 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/checkout/form-validation.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11933 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/checkout/index.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.125832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/cover/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1503 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/cover/cover.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2340 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/cover/index.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.129832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/dashboard/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1539 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/dashboard/dashboard.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10152 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/dashboard/index.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.129832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/floating-labels/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1716 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/floating-labels/floating-labels.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1824 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/floating-labels/index.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.129832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/grid/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      372 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/grid/grid.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5271 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/grid/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1001 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/index.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.129832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/jumbotron/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4989 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/jumbotron/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      107 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/jumbotron/jumbotron.css
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.129832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbar-bottom/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2852 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbar-bottom/index.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.129832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbar-fixed/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2777 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbar-fixed/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       87 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbar-fixed/navbar-top-fixed.css
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.133832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbar-static/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2783 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbar-static/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       67 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbar-static/navbar-top.css
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.133832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbars/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    16619 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbars/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       69 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbars/navbar.css
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.133832 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/offcanvas/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7697 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/offcanvas/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1756 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/offcanvas/offcanvas.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      148 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/offcanvas/offcanvas.js
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.325834 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/pricing/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6160 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/pricing/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      377 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/pricing/pricing.css
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.325834 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/product/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9286 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/product/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1383 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/product/product.css
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.337834 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    26370 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/album.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    36944 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/blog.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    31465 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/carousel.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    28180 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/checkout.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    17953 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/cover.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    26556 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/dashboard.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11053 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/floating-labels.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    33860 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/grid.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    38408 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/jumbotron.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11316 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/navbar-bottom.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    13616 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/navbar-fixed.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    14893 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/navbar-static.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    27187 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/navbars.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    23975 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/offcanvas.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    29128 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/pricing.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    27953 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/product.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5680 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/sign-in.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11334 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/starter-template.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    15836 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/sticky-footer-navbar.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9665 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/sticky-footer.png
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.337834 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sign-in/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1462 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sign-in/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      902 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sign-in/signin.css
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.337834 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/starter-template/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3196 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/starter-template/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       98 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/starter-template/starter-template.css
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.337834 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sticky-footer/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1122 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sticky-footer/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      613 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sticky-footer/sticky-footer.css
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.337834 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sticky-footer-navbar/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3104 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sticky-footer-navbar/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      693 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sticky-footer-navbar/sticky-footer-navbar.css
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.341834 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/tooltip-viewport/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2417 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/tooltip-viewport/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      385 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/tooltip-viewport/tooltip-viewport.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      583 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/tooltip-viewport/tooltip-viewport.js
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.341834 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/extend/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6986 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/extend/approach.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      987 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/extend/icons.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       59 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/extend/index.md
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.345834 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4099 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/accessibility.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      617 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/best-practices.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9246 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/browsers-devices.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3527 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/build-tools.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5408 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/contents.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4716 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/download.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7193 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/introduction.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6596 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/javascript.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    17078 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/theming.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3364 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/webpack.md
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.345834 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/layout/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    24684 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/layout/grid.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7742 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/layout/media-object.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6737 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/layout/overview.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2039 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/layout/utilities-for-layout.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    27814 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/migration.md
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.433835 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2381 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/borders.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      985 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/clearfix.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      378 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/close-icon.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2758 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/colors.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3915 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/display.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1655 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/embed.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    20834 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/flex.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1607 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/float.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      758 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/image-replacement.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1525 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/position.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      811 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/screenreaders.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1722 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/sizing.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3078 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/spacing.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2825 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/text.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1285 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/vertical-align.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      751 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/visibility.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5430 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/favicon.ico
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4384 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/index.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:51.869829 jupyterlab_training-0.3.1/style/bootstrap/js/
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.441835 jupyterlab_training-0.3.1/style/bootstrap/js/dist/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4948 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/alert.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8180 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/alert.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5221 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/button.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8975 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/button.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    15569 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/carousel.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    28130 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/carousel.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11524 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/collapse.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    21118 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/collapse.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    15011 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/dropdown.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    26869 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/dropdown.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      921 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/index.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2222 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/index.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    18307 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/modal.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    33324 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/modal.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6301 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/popover.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9090 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/popover.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10254 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/scrollspy.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    18393 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/scrollspy.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7472 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/tab.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    13674 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/tab.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    19826 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/tooltip.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    37424 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/tooltip.js.map
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4359 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/util.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8425 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/dist/util.js.map
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.633837 jupyterlab_training-0.3.1/style/bootstrap/js/src/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4148 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/alert.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4672 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/button.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    14305 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/carousel.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10530 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/collapse.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    14017 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/dropdown.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1373 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/index.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    16753 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/modal.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4710 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/popover.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9218 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/scrollspy.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6922 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/tab.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    18575 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/tooltip.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4185 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/src/util.js
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.633837 jupyterlab_training-0.3.1/style/bootstrap/js/tests/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2769 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/README.md
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4330 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/index.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1602 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/karma.conf.js
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.641837 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      632 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/.eslintrc.json
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2760 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/alert.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7344 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/button.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    36530 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/carousel.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    34057 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/collapse.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    33910 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/dropdown.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    26038 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/modal.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    16308 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/popover.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    27058 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/scrollspy.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    16396 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/tab.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    29666 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/tooltip.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2473 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/util.js
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.641837 jupyterlab_training-0.3.1/style/bootstrap/js/tests/vendor/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    92629 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/vendor/jquery-1.9.1.min.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7875 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/vendor/qunit.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   145326 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/vendor/qunit.js
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.641837 jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2185 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/alert.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3011 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/button.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2301 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/carousel.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4128 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/collapse.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8864 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/dropdown.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    13438 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/modal.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1960 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/popover.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    19115 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/scrollspy.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    32329 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/tab.html
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3147 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/tooltip.html
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.641837 jupyterlab_training-0.3.1/style/bootstrap/nuget/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      935 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/nuget/MyGet.ps1
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1385 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/nuget/bootstrap.nuspec
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1409 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/nuget/bootstrap.sass.nuspec
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   433474 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/package-lock.json
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      530 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/package.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9152 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/package.json
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      123 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/robots.txt
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      249 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/sache.json
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.645837 jupyterlab_training-0.3.1/style/bootstrap/scss/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1150 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_alert.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      982 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_badge.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1249 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_breadcrumb.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3647 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_button-group.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2714 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_buttons.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5693 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_card.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4221 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_carousel.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      860 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_close.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1065 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_code.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7797 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_custom-forms.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3092 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_dropdown.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8766 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_forms.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2657 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_functions.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1016 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_grid.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1146 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_images.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4864 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_input-group.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      378 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_jumbotron.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2887 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_list-group.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       83 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_media.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1018 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_mixins.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4623 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_modal.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2022 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_nav.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6781 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_navbar.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1834 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_pagination.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4536 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_popover.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2768 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_print.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      841 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_progress.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11591 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_reboot.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      572 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_root.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3426 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_tables.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2503 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_tooltip.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      452 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_transitions.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2115 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_type.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      407 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_utilities.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    35747 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/_variables.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      648 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/bootstrap-grid.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      410 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/bootstrap-reboot.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      881 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/bootstrap.scss
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.733838 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      242 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_alert.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      474 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_background-variant.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      230 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_badge.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      722 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_border-radius.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       87 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_box-shadow.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4468 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_breakpoints.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3182 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_buttons.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1459 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_caret.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       93 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_clearfix.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      193 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_float.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3199 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_forms.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2024 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_gradients.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1899 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_grid-framework.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1606 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_grid.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      783 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_hover.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1172 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_image.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      429 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_list-group.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      168 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_lists.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      220 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_nav-divider.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      385 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_navbar-align.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      453 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_pagination.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      547 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_reset-text.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      202 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_resize.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      778 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_screen-reader.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       98 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_size.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      647 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_table-row.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      259 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_text-emphasis.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      231 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_text-hide.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      168 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_text-truncate.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      192 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_transition.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      134 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_visibility.scss
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.737838 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      420 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_align.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      397 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_background.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1551 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_borders.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       37 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_clearfix.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1409 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_display.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      727 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_embed.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2458 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_flex.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      320 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_float.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      614 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_position.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      115 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_screenreaders.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      298 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_sizing.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1406 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_spacing.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1338 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_text.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      121 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_visibility.scss
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      114 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/bootstrap/sw.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    39502 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/homePage.png
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3761 2022-11-16 10:58:25.000000 jupyterlab_training-0.3.1/style/index.css
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       21 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/index.js
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1051 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/logilab-icon.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1150 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/logilab.ico
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7498 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/logilab.svg
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4436 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.1/style/stop_app.png
-drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:00:52.737838 jupyterlab_training-0.3.1/tests/
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1138 2022-01-12 11:00:40.000000 jupyterlab_training-0.3.1/tests/test_handlers.py
--rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      569 2023-04-04 13:32:50.000000 jupyterlab_training-0.3.1/tsconfig.json
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:05.172433 jupyterlab_training-0.3.2/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1516 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/LICENSE
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      435 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/MANIFEST.in
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3133 2023-05-25 15:17:05.168433 jupyterlab_training-0.3.2/PKG-INFO
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2375 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/README.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      199 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/install.json
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.540426 jupyterlab_training-0.3.2/jupyter-config/
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.544426 jupyterlab_training-0.3.2/jupyter-config/server-config/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       94 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/jupyter-config/server-config/jupyterlab-training.json
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.544426 jupyterlab_training-0.3.2/jupyterlab_training/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4311 2022-04-26 13:53:46.000000 jupyterlab_training-0.3.2/jupyterlab_training/__init__.py
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      473 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/jupyterlab_training/_version.py
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2277 2023-04-14 08:02:10.000000 jupyterlab_training-0.3.2/jupyterlab_training/db.py
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8227 2023-05-25 09:07:08.000000 jupyterlab_training-0.3.2/jupyterlab_training/handlers.py
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.544426 jupyterlab_training-0.3.2/jupyterlab_training/labextension/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3710 2023-05-25 15:16:35.000000 jupyterlab_training-0.3.2/jupyterlab_training/labextension/package.json
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.548426 jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   115723 2023-05-25 15:16:35.000000 jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/147.61d247f0dd79cb5e6c03.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      121 2023-05-25 15:16:35.000000 jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/147.61d247f0dd79cb5e6c03.js.LICENSE.txt
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2686 2023-05-25 15:16:35.000000 jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/162.54797b341de4f60c5f53.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    44687 2023-05-25 15:16:35.000000 jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/169.dde25e4dfa365788e2d3.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   242635 2023-05-25 15:16:35.000000 jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/3.97e5ce5c6c551fd93ee6.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   197062 2023-05-25 15:16:35.000000 jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/320.e87de993e15ebd1d087e.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      225 2023-05-25 15:16:35.000000 jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/320.e87de993e15ebd1d087e.js.LICENSE.txt
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    72799 2023-05-25 15:16:35.000000 jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/490.76b7872fc9815805fce9.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7272 2023-05-25 15:16:35.000000 jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/71.b08e1d3adafbcb17349c.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    98509 2023-05-25 15:16:35.000000 jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/733.c4acd437d42492321d94.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      383 2023-05-25 15:16:35.000000 jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/733.c4acd437d42492321d94.js.LICENSE.txt
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3378 2023-05-25 15:16:35.000000 jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/747.d4b5f772f188f310ccf4.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4436 2023-05-25 15:16:35.000000 jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/9c539cf459fdeaebf6835c214cb5cac1d43cd5d497cf4b96647401981d180043.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9396 2023-05-25 15:16:35.000000 jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/remoteEntry.eae807b4abaa17c88aae.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      162 2023-05-25 15:16:29.000000 jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/style.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    69137 2023-05-25 15:16:35.000000 jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.544426 jupyterlab_training-0.3.2/jupyterlab_training.egg-info/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3133 2023-05-25 15:17:04.000000 jupyterlab_training-0.3.2/jupyterlab_training.egg-info/PKG-INFO
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    21243 2023-05-25 15:17:04.000000 jupyterlab_training-0.3.2/jupyterlab_training.egg-info/SOURCES.txt
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)        1 2023-05-25 15:17:04.000000 jupyterlab_training-0.3.2/jupyterlab_training.egg-info/dependency_links.txt
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)        1 2023-05-25 15:17:04.000000 jupyterlab_training-0.3.2/jupyterlab_training.egg-info/not-zip-safe
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      119 2023-05-25 15:17:04.000000 jupyterlab_training-0.3.2/jupyterlab_training.egg-info/requires.txt
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       20 2023-05-25 15:17:04.000000 jupyterlab_training-0.3.2/jupyterlab_training.egg-info/top_level.txt
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3804 2023-05-25 15:15:42.000000 jupyterlab_training-0.3.2/package.json
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      610 2023-05-25 15:08:05.000000 jupyterlab_training-0.3.2/pyproject.toml
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       38 2023-05-25 15:17:05.172433 jupyterlab_training-0.3.2/setup.cfg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2671 2022-04-26 13:51:23.000000 jupyterlab_training-0.3.2/setup.py
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.548426 jupyterlab_training-0.3.2/src/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1481 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/src/flake8.tsx
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.548426 jupyterlab_training-0.3.2/src/i18n/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    17168 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/src/i18n/index.ts
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3457 2023-04-14 10:37:08.000000 jupyterlab_training-0.3.2/src/index.ts
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7641 2023-05-25 13:39:32.000000 jupyterlab_training-0.3.2/src/menu.tsx
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1870 2023-04-04 13:29:43.000000 jupyterlab_training-0.3.2/src/model.tsx
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    19967 2023-04-05 08:23:46.000000 jupyterlab_training-0.3.2/src/panel.tsx
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4415 2022-04-26 12:49:05.000000 jupyterlab_training-0.3.2/src/progressButton.tsx
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4664 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/src/statsWidget.tsx
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8902 2023-05-09 07:57:45.000000 jupyterlab_training-0.3.2/src/tour.tsx
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1009 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/src/utils.tsx
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.548426 jupyterlab_training-0.3.2/style/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)        0 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/base.css
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.552426 jupyterlab_training-0.3.2/style/bootstrap/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      313 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/.babelrc.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      208 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/.editorconfig
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       56 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/.eslintignore
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7131 2023-04-04 13:29:43.000000 jupyterlab_training-0.3.2/style/bootstrap/.eslintrc.json
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      359 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/.gitattributes
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.552426 jupyterlab_training-0.3.2/style/bootstrap/.github/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    14268 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/.github/CONTRIBUTING.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1178 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      517 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/.gitignore
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       45 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/.stylelintignore
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6685 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/.stylelintrc
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      782 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/.travis.yml
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       17 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/CNAME
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3217 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/CODE_OF_CONDUCT.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      199 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/Gemfile
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1905 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/Gemfile.lock
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1131 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/LICENSE
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9138 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/README.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2505 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_config.yml
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.552426 jupyterlab_training-0.3.2/style/bootstrap/_data/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      418 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_data/breakpoints.yml
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9113 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_data/browser-bugs.yml
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3244 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_data/browser-features.yml
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      401 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_data/colors.yml
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2870 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_data/examples.yml
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      261 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_data/grays.yml
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1657 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_data/nav.yml
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      257 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_data/theme-colors.yml
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      519 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_data/translations.yml
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.552426 jupyterlab_training-0.3.2/style/bootstrap/_includes/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      137 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_includes/ads.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      445 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_includes/callout-danger-async-methods.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      451 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_includes/callout-info-mediaqueries-breakpoints.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      454 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_includes/callout-warning-color-assistive-technologies.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3520 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_includes/docs-navbar.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2269 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_includes/docs-sidebar.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      748 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_includes/favicons.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1148 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_includes/footer.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1540 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_includes/header.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.556426 jupyterlab_training-0.3.2/style/bootstrap/_includes/icons/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      890 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_includes/icons/bootstrap.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      482 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_includes/icons/download.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1116 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_includes/icons/github.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      441 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_includes/icons/import.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      442 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_includes/icons/lightning.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      410 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_includes/icons/menu.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1362 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_includes/icons/slack.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      861 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_includes/icons/twitter.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1376 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_includes/scripts.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1290 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_includes/social.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.556426 jupyterlab_training-0.3.2/style/bootstrap/_layouts/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      556 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_layouts/default.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1040 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_layouts/docs.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      538 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_layouts/examples.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      412 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_layouts/home.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1134 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_layouts/redirect.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      288 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_layouts/simple.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.556426 jupyterlab_training-0.3.2/style/bootstrap/_plugins/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1326 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_plugins/bugify.rb
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      827 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_plugins/callout.rb
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3402 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_plugins/example.rb
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      525 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/_plugins/markdown-block.rb
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.540426 jupyterlab_training-0.3.2/style/bootstrap/assets/
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.556426 jupyterlab_training-0.3.2/style/bootstrap/assets/brand/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1306 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/brand/bootstrap-outline.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1140 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/brand/bootstrap-punchout.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    23959 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/brand/bootstrap-social-logo.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   231733 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/brand/bootstrap-social.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1127 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/brand/bootstrap-solid.svg
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.556426 jupyterlab_training-0.3.2/style/bootstrap/assets/css/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    21574 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/css/docs.min.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    40321 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/css/docs.min.css.map
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.556426 jupyterlab_training-0.3.2/style/bootstrap/assets/img/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    52160 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/img/bootstrap-stack.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    80588 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/img/bootstrap-themes.png
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.568426 jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1935 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/android-chrome-192x192.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4269 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/android-chrome-512x512.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1738 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/apple-touch-icon.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      292 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/browserconfig.xml
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      310 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/favicon-16x16.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      491 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/favicon-32x32.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      550 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/manifest.json
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1479 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/mstile-144x144.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1428 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/mstile-150x150.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1746 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/mstile-310x150.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3085 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/mstile-310x310.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1104 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/mstile-70x70.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1025 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/safari-pinned-tab.svg
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.568426 jupyterlab_training-0.3.2/style/bootstrap/assets/js/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      490 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/js/.eslintrc.json
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    52015 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/js/docs.min.js
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.568426 jupyterlab_training-0.3.2/style/bootstrap/assets/js/src/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4518 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/js/src/application.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2005 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/js/src/ie-emulation-modes-warning.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      545 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/js/src/pwa.js
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.568426 jupyterlab_training-0.3.2/style/bootstrap/assets/js/vendor/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5389 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/js/vendor/anchor.min.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10917 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/js/vendor/clipboard.min.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    32283 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/js/vendor/holder.min.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    69597 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/js/vendor/jquery-slim.min.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    19188 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/js/vendor/popper.min.js
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.680428 jupyterlab_training-0.3.2/style/bootstrap/assets/scss/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      593 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_ads.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3422 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_algolia.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      172 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_anchor.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1827 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_brand.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      195 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_browser-bugs.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      487 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_buttons.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      695 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_callouts.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      574 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_clipboard-js.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      419 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_colors.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6341 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_component-examples.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1995 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_content.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      363 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_examples.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      459 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_footer.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      887 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_masthead.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1685 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_nav.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2724 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_sidebar.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      213 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_skiplink.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1669 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_syntax.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      382 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_variables.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1520 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/assets/scss/docs.scss
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.688428 jupyterlab_training-0.3.2/style/bootstrap/build/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      385 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/build/.eslintrc.json
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1260 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/build/.htmllintrc
+-rwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)     2758 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/build/change-version.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2304 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/build/gcp-key.json.enc
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1505 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/build/generate-sri.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2070 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/build/lint-vars.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      238 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/build/postcss.config.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1379 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/build/rollup.config.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1221 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/build/sauce_browsers.json
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3116 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/build/saucelabs-unit-test.js
+-rwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)     2778 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/build/ship.sh
+-rwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)      701 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/build/upload-preview.sh
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2605 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/build/vnu-jar.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      156 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/build/workbox.config.json
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1282 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/build/workbox.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      744 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/composer.json
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.540426 jupyterlab_training-0.3.2/style/bootstrap/dist/
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.696428 jupyterlab_training-0.3.2/style/bootstrap/dist/css/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    43852 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap-grid.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    95910 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap-grid.css.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    34243 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap-grid.min.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    76209 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4798 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap-reboot.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    57721 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap-reboot.css.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3936 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap-reboot.min.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    25881 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   178152 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   411645 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap.css.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   144877 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap.min.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   551641 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap.min.css.map
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.708428 jupyterlab_training-0.3.2/style/bootstrap/dist/js/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   195855 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/dist/js/bootstrap.bundle.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   326634 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/dist/js/bootstrap.bundle.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    67742 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/dist/js/bootstrap.bundle.min.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   273872 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/dist/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   115048 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/dist/js/bootstrap.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   195373 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/dist/js/bootstrap.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    48944 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/dist/js/bootstrap.min.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   161998 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/dist/js/bootstrap.min.js.map
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.540426 jupyterlab_training-0.3.2/style/bootstrap/docs/
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.708428 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.708428 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/about/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2940 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/about/brand.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1717 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/about/license.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2495 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/about/overview.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      630 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/about/translations.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2474 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/browser-bugs.md
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.716428 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4439 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/alerts.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3450 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/badge.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1503 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/breadcrumb.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9208 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/button-group.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7445 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/buttons.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    26080 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/card.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12440 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/carousel.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12091 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/collapse.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    33022 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/dropdowns.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    51564 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/forms.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12974 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/input-group.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1199 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/jumbotron.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    18093 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/list-group.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    29516 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/modal.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    23281 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/navbar.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    35152 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/navs.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6170 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/pagination.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    15225 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/popovers.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6318 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/progress.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    18827 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/scrollspy.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    15834 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/tooltips.md
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.716428 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/content/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1436 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/content/code.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1329 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/content/figures.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3349 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/content/images.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12826 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/content/reboot.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    16669 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/content/tables.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10926 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/content/typography.md
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.784429 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      185 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/.eslintrc.json
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      339 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/.stylelintrc
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.784429 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/album/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      655 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/album/album.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12744 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/album/index.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.784429 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/blog/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2133 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/blog/blog.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    12774 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/blog/index.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.784429 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/carousel/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1658 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/carousel/carousel.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10159 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/carousel/index.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.784429 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/checkout/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      287 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/checkout/form-validation.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11933 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/checkout/index.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.784429 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/cover/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1503 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/cover/cover.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2340 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/cover/index.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.784429 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/dashboard/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1539 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/dashboard/dashboard.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10152 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/dashboard/index.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.784429 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/floating-labels/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1716 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/floating-labels/floating-labels.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1824 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/floating-labels/index.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.784429 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/grid/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      372 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/grid/grid.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5271 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/grid/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1001 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/index.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.784429 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/jumbotron/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4989 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/jumbotron/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      107 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/jumbotron/jumbotron.css
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.784429 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/navbar-bottom/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2852 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/navbar-bottom/index.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.784429 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/navbar-fixed/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2777 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/navbar-fixed/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       87 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/navbar-fixed/navbar-top-fixed.css
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.784429 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/navbar-static/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2783 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/navbar-static/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       67 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/navbar-static/navbar-top.css
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.784429 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/navbars/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    16619 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/navbars/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       69 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/navbars/navbar.css
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.784429 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/offcanvas/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7697 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/offcanvas/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1756 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/offcanvas/offcanvas.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      148 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/offcanvas/offcanvas.js
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.912430 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/pricing/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6160 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/pricing/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      377 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/pricing/pricing.css
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.912430 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/product/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9286 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/product/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1383 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/product/product.css
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.912430 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    26370 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/album.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    36944 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/blog.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    31465 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/carousel.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    28180 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/checkout.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    17953 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/cover.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    26556 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/dashboard.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11053 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/floating-labels.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    33860 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/grid.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    38408 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/jumbotron.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11316 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/navbar-bottom.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    13616 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/navbar-fixed.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    14893 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/navbar-static.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    27187 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/navbars.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    23975 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/offcanvas.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    29128 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/pricing.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    27953 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/product.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5680 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/sign-in.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11334 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/starter-template.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    15836 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/sticky-footer-navbar.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9665 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/sticky-footer.png
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.912430 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/sign-in/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1462 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/sign-in/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      902 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/sign-in/signin.css
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.912430 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/starter-template/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3196 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/starter-template/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       98 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/starter-template/starter-template.css
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.912430 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/sticky-footer/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1122 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/sticky-footer/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      613 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/sticky-footer/sticky-footer.css
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.912430 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/sticky-footer-navbar/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3104 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/sticky-footer-navbar/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      693 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/sticky-footer-navbar/sticky-footer-navbar.css
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.912430 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/tooltip-viewport/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2417 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/tooltip-viewport/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      385 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/tooltip-viewport/tooltip-viewport.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      583 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/tooltip-viewport/tooltip-viewport.js
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.912430 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/extend/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6986 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/extend/approach.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      987 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/extend/icons.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       59 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/extend/index.md
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.916430 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/getting-started/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4099 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/getting-started/accessibility.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      617 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/getting-started/best-practices.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9246 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/getting-started/browsers-devices.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3527 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/getting-started/build-tools.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5408 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/getting-started/contents.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4716 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/getting-started/download.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7193 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/getting-started/introduction.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6596 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/getting-started/javascript.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    17078 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/getting-started/theming.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3364 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/getting-started/webpack.md
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.916430 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/layout/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    24684 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/layout/grid.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7742 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/layout/media-object.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6737 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/layout/overview.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2039 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/layout/utilities-for-layout.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    27814 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/migration.md
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.984431 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2381 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/borders.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      985 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/clearfix.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      378 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/close-icon.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2758 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/colors.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3915 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/display.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1655 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/embed.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    20834 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/flex.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1607 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/float.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      758 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/image-replacement.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1525 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/position.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      811 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/screenreaders.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1722 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/sizing.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3078 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/spacing.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2825 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/text.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1285 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/vertical-align.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      751 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/visibility.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5430 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/favicon.ico
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4384 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/index.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.544426 jupyterlab_training-0.3.2/style/bootstrap/js/
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:04.988431 jupyterlab_training-0.3.2/style/bootstrap/js/dist/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4948 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/alert.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8180 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/alert.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5221 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/button.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8975 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/button.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    15569 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/carousel.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    28130 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/carousel.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11524 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/collapse.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    21118 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/collapse.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    15011 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/dropdown.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    26869 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/dropdown.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      921 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/index.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2222 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/index.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    18307 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/modal.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    33324 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/modal.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6301 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/popover.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9090 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/popover.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10254 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/scrollspy.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    18393 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/scrollspy.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7472 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/tab.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    13674 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/tab.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    19826 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/tooltip.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    37424 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/tooltip.js.map
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4359 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/util.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8425 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/dist/util.js.map
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:05.044432 jupyterlab_training-0.3.2/style/bootstrap/js/src/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4148 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/src/alert.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4672 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/src/button.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    14305 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/src/carousel.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    10530 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/src/collapse.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    14017 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/src/dropdown.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1373 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/src/index.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    16753 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/src/modal.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4710 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/src/popover.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9218 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/src/scrollspy.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6922 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/src/tab.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    18575 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/src/tooltip.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4185 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/src/util.js
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:05.044432 jupyterlab_training-0.3.2/style/bootstrap/js/tests/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2769 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/README.md
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4330 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/index.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1602 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/karma.conf.js
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:05.044432 jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      632 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/.eslintrc.json
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2760 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/alert.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7344 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/button.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    36530 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/carousel.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    34057 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/collapse.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    33910 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/dropdown.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    26038 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/modal.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    16308 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/popover.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    27058 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/scrollspy.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    16396 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/tab.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    29666 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/tooltip.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2473 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/util.js
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:05.044432 jupyterlab_training-0.3.2/style/bootstrap/js/tests/vendor/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    92629 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/vendor/jquery-1.9.1.min.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7875 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/vendor/qunit.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   145326 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/vendor/qunit.js
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:05.048432 jupyterlab_training-0.3.2/style/bootstrap/js/tests/visual/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2185 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/visual/alert.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3011 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/visual/button.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2301 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/visual/carousel.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4128 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/visual/collapse.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8864 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/visual/dropdown.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    13438 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/visual/modal.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1960 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/visual/popover.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    19115 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/visual/scrollspy.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    32329 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/visual/tab.html
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3147 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/js/tests/visual/tooltip.html
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:05.048432 jupyterlab_training-0.3.2/style/bootstrap/nuget/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      935 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/nuget/MyGet.ps1
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1385 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/nuget/bootstrap.nuspec
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1409 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/nuget/bootstrap.sass.nuspec
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)   433474 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/package-lock.json
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      530 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/package.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     9152 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/package.json
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      123 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/robots.txt
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      249 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/sache.json
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:05.156433 jupyterlab_training-0.3.2/style/bootstrap/scss/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1150 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_alert.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      982 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_badge.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1249 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_breadcrumb.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3647 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_button-group.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2714 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_buttons.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     5693 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_card.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4221 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_carousel.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      860 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_close.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1065 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_code.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7797 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_custom-forms.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3092 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_dropdown.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     8766 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_forms.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2657 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_functions.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1016 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_grid.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1146 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_images.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4864 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_input-group.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      378 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_jumbotron.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2887 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_list-group.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       83 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_media.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1018 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_mixins.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4623 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_modal.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2022 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_nav.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     6781 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_navbar.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1834 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_pagination.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4536 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_popover.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2768 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_print.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      841 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_progress.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    11591 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_reboot.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      572 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_root.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3426 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_tables.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2503 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_tooltip.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      452 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_transitions.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2115 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_type.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      407 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_utilities.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    35747 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/_variables.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      648 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/bootstrap-grid.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      410 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/bootstrap-reboot.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      881 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/bootstrap.scss
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:05.168433 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      242 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_alert.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      474 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_background-variant.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      230 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_badge.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      722 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_border-radius.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       87 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_box-shadow.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4468 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_breakpoints.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3182 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_buttons.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1459 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_caret.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       93 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_clearfix.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      193 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_float.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3199 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_forms.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2024 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_gradients.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1899 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_grid-framework.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1606 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_grid.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      783 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_hover.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1172 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_image.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      429 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_list-group.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      168 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_lists.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      220 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_nav-divider.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      385 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_navbar-align.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      453 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_pagination.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      547 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_reset-text.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      202 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_resize.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      778 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_screen-reader.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       98 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_size.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      647 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_table-row.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      259 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_text-emphasis.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      231 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_text-hide.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      168 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_text-truncate.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      192 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_transition.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      134 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_visibility.scss
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:05.168433 jupyterlab_training-0.3.2/style/bootstrap/scss/utilities/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      420 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/utilities/_align.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      397 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/utilities/_background.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1551 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/utilities/_borders.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       37 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/utilities/_clearfix.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1409 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/utilities/_display.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      727 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/utilities/_embed.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     2458 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/utilities/_flex.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      320 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/utilities/_float.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      614 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/utilities/_position.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      115 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/utilities/_screenreaders.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      298 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/utilities/_sizing.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1406 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/utilities/_spacing.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1338 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/utilities/_text.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      121 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/scss/utilities/_visibility.scss
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      114 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/bootstrap/sw.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)    39502 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/homePage.png
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     3761 2022-11-16 10:58:25.000000 jupyterlab_training-0.3.2/style/index.css
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)       21 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/index.js
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1051 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/logilab-icon.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1150 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/logilab.ico
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     7498 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/logilab.svg
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     4436 2022-04-04 12:14:55.000000 jupyterlab_training-0.3.2/style/stop_app.png
+drwxr-xr-x   0 ogiorgis  (1000) ogiorgis  (1000)        0 2023-05-25 15:17:05.168433 jupyterlab_training-0.3.2/tests/
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)     1138 2022-01-12 11:00:40.000000 jupyterlab_training-0.3.2/tests/test_handlers.py
+-rw-r--r--   0 ogiorgis  (1000) ogiorgis  (1000)      569 2023-04-04 13:32:50.000000 jupyterlab_training-0.3.2/tsconfig.json
```

### Comparing `jupyterlab_training-0.3.1/LICENSE` & `jupyterlab_training-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/PKG-INFO` & `jupyterlab_training-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_training
-Version: 0.3.1
+Version: 0.3.2
 Summary: jupyterlab training courses and exercices platform
 Home-page: https://gitlab.com/logilab/jupyterlab-training
 Author: Logilab
 Author-email: ogiorgis@logilab.fr
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `jupyterlab_training-0.3.1/README.md` & `jupyterlab_training-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/jupyterlab_training/__init__.py` & `jupyterlab_training-0.3.2/jupyterlab_training/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/jupyterlab_training/db.py` & `jupyterlab_training-0.3.2/jupyterlab_training/db.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/jupyterlab_training/handlers.py` & `jupyterlab_training-0.3.2/jupyterlab_training/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/jupyterlab_training/labextension/package.json` & `jupyterlab_training-0.3.2/jupyterlab_training/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9743055555555555%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.eae807b4abaa17c88aae.js'}}",*

 * * "'version'": "'0.3.2'"}*

```diff
@@ -52,15 +52,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://gitlab.com/logilab/jupyterlab-training",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.1860e2c61e01ab7c6b1c.js",
+            "load": "static/remoteEntry.eae807b4abaa17c88aae.js",
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
-    "version": "0.3.1"
+    "version": "0.3.2"
 }
```

### Comparing `jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/147.61d247f0dd79cb5e6c03.js` & `jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/147.61d247f0dd79cb5e6c03.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/162.54797b341de4f60c5f53.js` & `jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/162.54797b341de4f60c5f53.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/169.dde25e4dfa365788e2d3.js` & `jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/169.dde25e4dfa365788e2d3.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/3.97e5ce5c6c551fd93ee6.js` & `jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/3.97e5ce5c6c551fd93ee6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/320.e87de993e15ebd1d087e.js` & `jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/320.e87de993e15ebd1d087e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/490.76b7872fc9815805fce9.js` & `jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/490.76b7872fc9815805fce9.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/71.b08e1d3adafbcb17349c.js` & `jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/71.b08e1d3adafbcb17349c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/733.c4acd437d42492321d94.js` & `jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/733.c4acd437d42492321d94.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/747.d4b5f772f188f310ccf4.js` & `jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/747.d4b5f772f188f310ccf4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/9c539cf459fdeaebf6835c214cb5cac1d43cd5d497cf4b96647401981d180043.png` & `jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/9c539cf459fdeaebf6835c214cb5cac1d43cd5d497cf4b96647401981d180043.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/remoteEntry.1860e2c61e01ab7c6b1c.js` & `jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/remoteEntry.eae807b4abaa17c88aae.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -123,15 +123,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (l("file-saver", "2.0.5", (() => P.e(162).then((() => () => P(3162))))), l("i18next-browser-languagedetector", "6.1.8", (() => P.e(71).then((() => () => P(6071))))), l("i18next", "20.6.1", (() => P.e(169).then((() => () => P(8169))))), l("js-yaml", "3.14.1", (() => P.e(320).then((() => () => P(3320))))), l("jszip", "3.10.1", (() => P.e(733).then((() => () => P(5733))))), l("jupyterlab-training", "0.3.1", (() => Promise.all([P.e(832), P.e(3)]).then((() => () => P(9003))))), l("luxon", "1.28.1", (() => P.e(490).then((() => () => P(9490))))), l("react-bootstrap", "1.6.6", (() => Promise.all([P.e(147), P.e(832)]).then((() => () => P(8147)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("file-saver", "2.0.5", (() => P.e(162).then((() => () => P(3162))))), l("i18next-browser-languagedetector", "6.1.8", (() => P.e(71).then((() => () => P(6071))))), l("i18next", "20.6.1", (() => P.e(169).then((() => () => P(8169))))), l("js-yaml", "3.14.1", (() => P.e(320).then((() => () => P(3320))))), l("jszip", "3.10.1", (() => P.e(733).then((() => () => P(5733))))), l("jupyterlab-training", "0.3.2", (() => Promise.all([P.e(832), P.e(3)]).then((() => () => P(9003))))), l("luxon", "1.28.1", (() => P.e(490).then((() => () => P(9490))))), l("react-bootstrap", "1.6.6", (() => Promise.all([P.e(147), P.e(832)]).then((() => () => P(8147)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var r = P.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_training-0.3.1/jupyterlab_training/labextension/static/third-party-licenses.json` & `jupyterlab_training-0.3.2/jupyterlab_training/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/jupyterlab_training.egg-info/PKG-INFO` & `jupyterlab_training-0.3.2/jupyterlab_training.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-training
-Version: 0.3.1
+Version: 0.3.2
 Summary: jupyterlab training courses and exercices platform
 Home-page: https://gitlab.com/logilab/jupyterlab-training
 Author: Logilab
 Author-email: ogiorgis@logilab.fr
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `jupyterlab_training-0.3.1/jupyterlab_training.egg-info/SOURCES.txt` & `jupyterlab_training-0.3.2/jupyterlab_training.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 jupyterlab_training/labextension/static/320.e87de993e15ebd1d087e.js.LICENSE.txt
 jupyterlab_training/labextension/static/490.76b7872fc9815805fce9.js
 jupyterlab_training/labextension/static/71.b08e1d3adafbcb17349c.js
 jupyterlab_training/labextension/static/733.c4acd437d42492321d94.js
 jupyterlab_training/labextension/static/733.c4acd437d42492321d94.js.LICENSE.txt
 jupyterlab_training/labextension/static/747.d4b5f772f188f310ccf4.js
 jupyterlab_training/labextension/static/9c539cf459fdeaebf6835c214cb5cac1d43cd5d497cf4b96647401981d180043.png
-jupyterlab_training/labextension/static/remoteEntry.1860e2c61e01ab7c6b1c.js
+jupyterlab_training/labextension/static/remoteEntry.eae807b4abaa17c88aae.js
 jupyterlab_training/labextension/static/style.js
 jupyterlab_training/labextension/static/third-party-licenses.json
 src/flake8.tsx
 src/index.ts
 src/menu.tsx
 src/model.tsx
 src/panel.tsx
```

### Comparing `jupyterlab_training-0.3.1/package.json` & `jupyterlab_training-0.3.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.3.2'"}*

```diff
@@ -96,9 +96,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.1"
+    "version": "0.3.2"
 }
```

### Comparing `jupyterlab_training-0.3.1/pyproject.toml` & `jupyterlab_training-0.3.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["jupyter_packaging~=0.10,<2", "jupyterlab~=3.1"]
+requires = ["jupyter_packaging~=0.10,<2", "jupyterlab>=3.6"]
 build-backend = "jupyter_packaging.build_api"
 
 [tool.jupyter-packaging.options]
 skip-if-exists = ["jupyterlab_training/labextension/static/style.js"]
 ensured-targets = ["jupyterlab_training/labextension/static/style.js", "jupyterlab_training/labextension/package.json"]
 
 [tool.jupyter-packaging.builder]
```

### Comparing `jupyterlab_training-0.3.1/setup.py` & `jupyterlab_training-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/src/flake8.tsx` & `jupyterlab_training-0.3.2/src/flake8.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/src/i18n/index.ts` & `jupyterlab_training-0.3.2/src/i18n/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/src/index.ts` & `jupyterlab_training-0.3.2/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/src/menu.tsx` & `jupyterlab_training-0.3.2/src/menu.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/src/model.tsx` & `jupyterlab_training-0.3.2/src/model.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/src/panel.tsx` & `jupyterlab_training-0.3.2/src/panel.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/src/progressButton.tsx` & `jupyterlab_training-0.3.2/src/progressButton.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/src/statsWidget.tsx` & `jupyterlab_training-0.3.2/src/statsWidget.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/src/tour.tsx` & `jupyterlab_training-0.3.2/src/tour.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/src/utils.tsx` & `jupyterlab_training-0.3.2/src/utils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/.eslintrc.json` & `jupyterlab_training-0.3.2/style/bootstrap/.eslintrc.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/.github/CONTRIBUTING.md` & `jupyterlab_training-0.3.2/style/bootstrap/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/.github/ISSUE_TEMPLATE.md` & `jupyterlab_training-0.3.2/style/bootstrap/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/.gitignore` & `jupyterlab_training-0.3.2/style/bootstrap/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/.stylelintrc` & `jupyterlab_training-0.3.2/style/bootstrap/.stylelintrc`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/.travis.yml` & `jupyterlab_training-0.3.2/style/bootstrap/.travis.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/CODE_OF_CONDUCT.md` & `jupyterlab_training-0.3.2/style/bootstrap/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/Gemfile.lock` & `jupyterlab_training-0.3.2/style/bootstrap/Gemfile.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/LICENSE` & `jupyterlab_training-0.3.2/style/bootstrap/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/README.md` & `jupyterlab_training-0.3.2/style/bootstrap/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_config.yml` & `jupyterlab_training-0.3.2/style/bootstrap/_config.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_data/browser-bugs.yml` & `jupyterlab_training-0.3.2/style/bootstrap/_data/browser-bugs.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_data/browser-features.yml` & `jupyterlab_training-0.3.2/style/bootstrap/_data/browser-features.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_data/examples.yml` & `jupyterlab_training-0.3.2/style/bootstrap/_data/examples.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_data/nav.yml` & `jupyterlab_training-0.3.2/style/bootstrap/_data/nav.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_data/translations.yml` & `jupyterlab_training-0.3.2/style/bootstrap/_data/translations.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_includes/docs-navbar.html` & `jupyterlab_training-0.3.2/style/bootstrap/_includes/docs-navbar.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_includes/docs-sidebar.html` & `jupyterlab_training-0.3.2/style/bootstrap/_includes/docs-sidebar.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_includes/favicons.html` & `jupyterlab_training-0.3.2/style/bootstrap/_includes/favicons.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_includes/footer.html` & `jupyterlab_training-0.3.2/style/bootstrap/_includes/footer.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_includes/header.html` & `jupyterlab_training-0.3.2/style/bootstrap/_includes/header.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/bootstrap.svg` & `jupyterlab_training-0.3.2/style/bootstrap/_includes/icons/bootstrap.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/github.svg` & `jupyterlab_training-0.3.2/style/bootstrap/_includes/icons/github.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/slack.svg` & `jupyterlab_training-0.3.2/style/bootstrap/_includes/icons/slack.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_includes/icons/twitter.svg` & `jupyterlab_training-0.3.2/style/bootstrap/_includes/icons/twitter.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_includes/scripts.html` & `jupyterlab_training-0.3.2/style/bootstrap/_includes/scripts.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_includes/social.html` & `jupyterlab_training-0.3.2/style/bootstrap/_includes/social.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_layouts/default.html` & `jupyterlab_training-0.3.2/style/bootstrap/_layouts/default.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_layouts/docs.html` & `jupyterlab_training-0.3.2/style/bootstrap/_layouts/docs.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_layouts/examples.html` & `jupyterlab_training-0.3.2/style/bootstrap/_layouts/examples.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_layouts/redirect.html` & `jupyterlab_training-0.3.2/style/bootstrap/_layouts/redirect.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_plugins/bugify.rb` & `jupyterlab_training-0.3.2/style/bootstrap/_plugins/bugify.rb`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_plugins/callout.rb` & `jupyterlab_training-0.3.2/style/bootstrap/_plugins/callout.rb`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_plugins/example.rb` & `jupyterlab_training-0.3.2/style/bootstrap/_plugins/example.rb`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/_plugins/markdown-block.rb` & `jupyterlab_training-0.3.2/style/bootstrap/_plugins/markdown-block.rb`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/brand/bootstrap-outline.svg` & `jupyterlab_training-0.3.2/style/bootstrap/assets/brand/bootstrap-outline.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/brand/bootstrap-punchout.svg` & `jupyterlab_training-0.3.2/style/bootstrap/assets/brand/bootstrap-punchout.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/brand/bootstrap-social-logo.png` & `jupyterlab_training-0.3.2/style/bootstrap/assets/brand/bootstrap-social-logo.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/brand/bootstrap-social.png` & `jupyterlab_training-0.3.2/style/bootstrap/assets/brand/bootstrap-social.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/brand/bootstrap-solid.svg` & `jupyterlab_training-0.3.2/style/bootstrap/assets/brand/bootstrap-solid.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/css/docs.min.css` & `jupyterlab_training-0.3.2/style/bootstrap/assets/css/docs.min.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/css/docs.min.css.map` & `jupyterlab_training-0.3.2/style/bootstrap/assets/css/docs.min.css.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/img/bootstrap-stack.png` & `jupyterlab_training-0.3.2/style/bootstrap/assets/img/bootstrap-stack.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/img/bootstrap-themes.png` & `jupyterlab_training-0.3.2/style/bootstrap/assets/img/bootstrap-themes.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/android-chrome-192x192.png` & `jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/android-chrome-512x512.png` & `jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/apple-touch-icon.png` & `jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/manifest.json` & `jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/manifest.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/mstile-144x144.png` & `jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/mstile-144x144.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/mstile-150x150.png` & `jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/mstile-310x150.png` & `jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/mstile-310x150.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/mstile-310x310.png` & `jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/mstile-310x310.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/mstile-70x70.png` & `jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/mstile-70x70.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/img/favicons/safari-pinned-tab.svg` & `jupyterlab_training-0.3.2/style/bootstrap/assets/img/favicons/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/js/docs.min.js` & `jupyterlab_training-0.3.2/style/bootstrap/assets/js/docs.min.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/js/src/application.js` & `jupyterlab_training-0.3.2/style/bootstrap/assets/js/src/application.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/js/src/ie-emulation-modes-warning.js` & `jupyterlab_training-0.3.2/style/bootstrap/assets/js/src/ie-emulation-modes-warning.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/js/src/pwa.js` & `jupyterlab_training-0.3.2/style/bootstrap/assets/js/src/pwa.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/js/vendor/anchor.min.js` & `jupyterlab_training-0.3.2/style/bootstrap/assets/js/vendor/anchor.min.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/js/vendor/clipboard.min.js` & `jupyterlab_training-0.3.2/style/bootstrap/assets/js/vendor/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/js/vendor/holder.min.js` & `jupyterlab_training-0.3.2/style/bootstrap/assets/js/vendor/holder.min.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/js/vendor/jquery-slim.min.js` & `jupyterlab_training-0.3.2/style/bootstrap/assets/js/vendor/jquery-slim.min.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/js/vendor/popper.min.js` & `jupyterlab_training-0.3.2/style/bootstrap/assets/js/vendor/popper.min.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_ads.scss` & `jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_ads.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_algolia.scss` & `jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_algolia.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_brand.scss` & `jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_brand.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_callouts.scss` & `jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_callouts.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_clipboard-js.scss` & `jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_clipboard-js.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_component-examples.scss` & `jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_component-examples.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_content.scss` & `jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_content.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_masthead.scss` & `jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_masthead.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_nav.scss` & `jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_sidebar.scss` & `jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_sidebar.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/_syntax.scss` & `jupyterlab_training-0.3.2/style/bootstrap/assets/scss/_syntax.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/assets/scss/docs.scss` & `jupyterlab_training-0.3.2/style/bootstrap/assets/scss/docs.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/build/.htmllintrc` & `jupyterlab_training-0.3.2/style/bootstrap/build/.htmllintrc`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/build/change-version.js` & `jupyterlab_training-0.3.2/style/bootstrap/build/change-version.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/build/gcp-key.json.enc` & `jupyterlab_training-0.3.2/style/bootstrap/build/gcp-key.json.enc`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/build/generate-sri.js` & `jupyterlab_training-0.3.2/style/bootstrap/build/generate-sri.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/build/lint-vars.js` & `jupyterlab_training-0.3.2/style/bootstrap/build/lint-vars.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/build/rollup.config.js` & `jupyterlab_training-0.3.2/style/bootstrap/build/rollup.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/build/sauce_browsers.json` & `jupyterlab_training-0.3.2/style/bootstrap/build/sauce_browsers.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/build/saucelabs-unit-test.js` & `jupyterlab_training-0.3.2/style/bootstrap/build/saucelabs-unit-test.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/build/ship.sh` & `jupyterlab_training-0.3.2/style/bootstrap/build/ship.sh`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/build/upload-preview.sh` & `jupyterlab_training-0.3.2/style/bootstrap/build/upload-preview.sh`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/build/vnu-jar.js` & `jupyterlab_training-0.3.2/style/bootstrap/build/vnu-jar.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/build/workbox.js` & `jupyterlab_training-0.3.2/style/bootstrap/build/workbox.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/composer.json` & `jupyterlab_training-0.3.2/style/bootstrap/composer.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-grid.css` & `jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-grid.css.map` & `jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-grid.min.css` & `jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-grid.min.css.map` & `jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-reboot.css` & `jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-reboot.css.map` & `jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-reboot.min.css` & `jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap-reboot.min.css.map` & `jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap.css` & `jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap.css.map` & `jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap.min.css` & `jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/dist/css/bootstrap.min.css.map` & `jupyterlab_training-0.3.2/style/bootstrap/dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.bundle.js` & `jupyterlab_training-0.3.2/style/bootstrap/dist/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.bundle.js.map` & `jupyterlab_training-0.3.2/style/bootstrap/dist/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.bundle.min.js` & `jupyterlab_training-0.3.2/style/bootstrap/dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.bundle.min.js.map` & `jupyterlab_training-0.3.2/style/bootstrap/dist/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.js` & `jupyterlab_training-0.3.2/style/bootstrap/dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.js.map` & `jupyterlab_training-0.3.2/style/bootstrap/dist/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.min.js` & `jupyterlab_training-0.3.2/style/bootstrap/dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/dist/js/bootstrap.min.js.map` & `jupyterlab_training-0.3.2/style/bootstrap/dist/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/about/brand.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/about/brand.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/about/license.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/about/license.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/about/overview.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/about/overview.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/about/translations.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/about/translations.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/browser-bugs.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/browser-bugs.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/alerts.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/alerts.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/badge.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/badge.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/breadcrumb.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/breadcrumb.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/button-group.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/button-group.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/buttons.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/buttons.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/card.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/card.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/carousel.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/carousel.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/collapse.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/collapse.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/dropdowns.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/dropdowns.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/forms.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/forms.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/input-group.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/input-group.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/jumbotron.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/jumbotron.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/list-group.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/list-group.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/modal.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/modal.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/navbar.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/navbar.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/navs.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/navs.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/pagination.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/pagination.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/popovers.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/popovers.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/progress.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/progress.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/scrollspy.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/scrollspy.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/components/tooltips.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/components/tooltips.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/code.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/content/code.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/figures.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/content/figures.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/images.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/content/images.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/reboot.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/content/reboot.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/tables.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/content/tables.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/content/typography.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/content/typography.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/album/album.css` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/album/album.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/album/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/album/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/blog/blog.css` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/blog/blog.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/blog/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/blog/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/carousel/carousel.css` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/carousel/carousel.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/carousel/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/carousel/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/checkout/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/checkout/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/cover/cover.css` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/cover/cover.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/cover/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/cover/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/dashboard/dashboard.css` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/dashboard/dashboard.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/dashboard/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/dashboard/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/floating-labels/floating-labels.css` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/floating-labels/floating-labels.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/floating-labels/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/floating-labels/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/grid/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/grid/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/jumbotron/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/jumbotron/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbar-bottom/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/navbar-bottom/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbar-fixed/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/navbar-fixed/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbar-static/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/navbar-static/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/navbars/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/navbars/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/offcanvas/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/offcanvas/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/offcanvas/offcanvas.css` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/offcanvas/offcanvas.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/pricing/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/pricing/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/product/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/product/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/product/product.css` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/product/product.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/album.png` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/album.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/blog.png` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/blog.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/carousel.png` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/carousel.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/checkout.png` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/checkout.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/cover.png` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/cover.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/dashboard.png` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/dashboard.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/floating-labels.png` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/floating-labels.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/grid.png` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/grid.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/jumbotron.png` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/jumbotron.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/navbar-bottom.png` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/navbar-bottom.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/navbar-fixed.png` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/navbar-fixed.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/navbar-static.png` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/navbar-static.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/navbars.png` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/navbars.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/offcanvas.png` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/offcanvas.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/pricing.png` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/pricing.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/product.png` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/product.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/sign-in.png` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/sign-in.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/starter-template.png` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/starter-template.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/sticky-footer-navbar.png` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/sticky-footer-navbar.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/screenshots/sticky-footer.png` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/screenshots/sticky-footer.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sign-in/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/sign-in/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sign-in/signin.css` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/sign-in/signin.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/starter-template/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/starter-template/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sticky-footer/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/sticky-footer/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sticky-footer/sticky-footer.css` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/sticky-footer/sticky-footer.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sticky-footer-navbar/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/sticky-footer-navbar/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/sticky-footer-navbar/sticky-footer-navbar.css` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/sticky-footer-navbar/sticky-footer-navbar.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/tooltip-viewport/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/tooltip-viewport/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/examples/tooltip-viewport/tooltip-viewport.js` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/examples/tooltip-viewport/tooltip-viewport.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/extend/approach.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/extend/approach.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/extend/icons.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/extend/icons.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/accessibility.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/getting-started/accessibility.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/best-practices.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/getting-started/best-practices.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/browsers-devices.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/getting-started/browsers-devices.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/build-tools.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/getting-started/build-tools.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/contents.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/getting-started/contents.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/download.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/getting-started/download.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/introduction.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/getting-started/introduction.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/javascript.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/getting-started/javascript.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/theming.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/getting-started/theming.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/getting-started/webpack.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/getting-started/webpack.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/layout/grid.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/layout/grid.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/layout/media-object.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/layout/media-object.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/layout/overview.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/layout/overview.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/layout/utilities-for-layout.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/layout/utilities-for-layout.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/migration.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/migration.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/borders.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/borders.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/clearfix.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/clearfix.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/colors.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/colors.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/display.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/display.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/embed.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/embed.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/flex.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/flex.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/float.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/float.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/image-replacement.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/image-replacement.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/position.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/position.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/screenreaders.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/screenreaders.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/sizing.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/sizing.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/spacing.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/spacing.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/text.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/text.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/vertical-align.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/vertical-align.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/docs/4.0/utilities/visibility.md` & `jupyterlab_training-0.3.2/style/bootstrap/docs/4.0/utilities/visibility.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/favicon.ico` & `jupyterlab_training-0.3.2/style/bootstrap/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/alert.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/alert.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/alert.js.map` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/alert.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/button.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/button.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/button.js.map` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/button.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/carousel.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/carousel.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/carousel.js.map` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/carousel.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/collapse.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/collapse.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/collapse.js.map` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/collapse.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/dropdown.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/dropdown.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/dropdown.js.map` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/dropdown.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/index.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/index.js.map` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/index.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/modal.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/modal.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/modal.js.map` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/modal.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/popover.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/popover.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/popover.js.map` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/popover.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/scrollspy.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/scrollspy.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/scrollspy.js.map` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/scrollspy.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/tab.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/tab.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/tab.js.map` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/tab.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/tooltip.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/tooltip.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/tooltip.js.map` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/tooltip.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/util.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/util.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/dist/util.js.map` & `jupyterlab_training-0.3.2/style/bootstrap/js/dist/util.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/src/alert.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/src/alert.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/src/button.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/src/button.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/src/carousel.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/src/carousel.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/src/collapse.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/src/collapse.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/src/dropdown.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/src/dropdown.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/src/index.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/src/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/src/modal.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/src/modal.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/src/popover.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/src/popover.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/src/scrollspy.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/src/scrollspy.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/src/tab.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/src/tab.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/src/tooltip.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/src/tooltip.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/src/util.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/src/util.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/README.md` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/index.html` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/karma.conf.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/karma.conf.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/.eslintrc.json` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/.eslintrc.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/alert.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/alert.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/button.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/button.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/carousel.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/carousel.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/collapse.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/collapse.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/dropdown.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/dropdown.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/modal.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/modal.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/popover.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/popover.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/scrollspy.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/scrollspy.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/tab.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/tab.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/tooltip.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/tooltip.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/unit/util.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/unit/util.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/vendor/jquery-1.9.1.min.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/vendor/jquery-1.9.1.min.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/vendor/qunit.css` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/vendor/qunit.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/vendor/qunit.js` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/vendor/qunit.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/alert.html` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/visual/alert.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/button.html` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/visual/button.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/carousel.html` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/visual/carousel.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/collapse.html` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/visual/collapse.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/dropdown.html` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/visual/dropdown.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/modal.html` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/visual/modal.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/popover.html` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/visual/popover.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/scrollspy.html` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/visual/scrollspy.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/tab.html` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/visual/tab.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/js/tests/visual/tooltip.html` & `jupyterlab_training-0.3.2/style/bootstrap/js/tests/visual/tooltip.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/nuget/MyGet.ps1` & `jupyterlab_training-0.3.2/style/bootstrap/nuget/MyGet.ps1`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/nuget/bootstrap.nuspec` & `jupyterlab_training-0.3.2/style/bootstrap/nuget/bootstrap.nuspec`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/nuget/bootstrap.sass.nuspec` & `jupyterlab_training-0.3.2/style/bootstrap/nuget/bootstrap.sass.nuspec`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/package-lock.json` & `jupyterlab_training-0.3.2/style/bootstrap/package-lock.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/package.js` & `jupyterlab_training-0.3.2/style/bootstrap/package.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/package.json` & `jupyterlab_training-0.3.2/style/bootstrap/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_alert.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_alert.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_badge.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_badge.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_breadcrumb.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_button-group.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_button-group.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_buttons.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_buttons.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_card.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_card.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_carousel.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_carousel.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_close.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_close.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_code.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_code.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_custom-forms.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_custom-forms.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_dropdown.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_forms.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_forms.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_functions.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_functions.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_grid.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_grid.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_images.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_images.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_input-group.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_input-group.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_list-group.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_list-group.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_mixins.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_modal.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_modal.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_nav.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_navbar.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_navbar.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_pagination.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_pagination.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_popover.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_popover.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_print.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_print.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_progress.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_progress.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_reboot.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_reboot.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_root.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_root.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_tables.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_tables.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_tooltip.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_type.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_type.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/_variables.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/bootstrap-grid.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/bootstrap.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_border-radius.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_breakpoints.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_buttons.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_caret.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_forms.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_gradients.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_grid-framework.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_grid-framework.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_grid.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_hover.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_hover.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_image.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_image.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_reset-text.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_reset-text.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_screen-reader.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_screen-reader.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/mixins/_table-row.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/mixins/_table-row.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_borders.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/utilities/_borders.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_display.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/utilities/_display.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_embed.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/utilities/_embed.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_flex.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/utilities/_flex.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_position.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/utilities/_position.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_spacing.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/utilities/_spacing.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/bootstrap/scss/utilities/_text.scss` & `jupyterlab_training-0.3.2/style/bootstrap/scss/utilities/_text.scss`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/homePage.png` & `jupyterlab_training-0.3.2/style/homePage.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/index.css` & `jupyterlab_training-0.3.2/style/index.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/logilab-icon.svg` & `jupyterlab_training-0.3.2/style/logilab-icon.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/logilab.ico` & `jupyterlab_training-0.3.2/style/logilab.ico`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/logilab.svg` & `jupyterlab_training-0.3.2/style/logilab.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/style/stop_app.png` & `jupyterlab_training-0.3.2/style/stop_app.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/tests/test_handlers.py` & `jupyterlab_training-0.3.2/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_training-0.3.1/tsconfig.json` & `jupyterlab_training-0.3.2/tsconfig.json`

 * *Files identical despite different names*

