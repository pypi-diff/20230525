# Comparing `tmp/bulma_sphinx_theme-0.0.1.tar.gz` & `tmp/bulma_sphinx_theme-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bulma_sphinx_theme-0.0.1.tar", last modified: Wed May 24 14:32:03 2023, max compression
+gzip compressed data, was "bulma_sphinx_theme-0.0.2.tar", last modified: Thu May 25 08:29:01 2023, max compression
```

## Comparing `bulma_sphinx_theme-0.0.1.tar` & `bulma_sphinx_theme-0.0.2.tar`

### file list

```diff
@@ -1,161 +1,167 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:32:03.476083 bulma_sphinx_theme-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/_static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/_static/logo-.png
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/develop.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/admonitions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/blocks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/generic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/images.rst
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/lists.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/really-long.md
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/sphinx-design.md
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/tables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/typography.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/reference/admonitions.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/reference/code-blocks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/reference/hyperlinks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/reference/images.md
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/reference/lists.md
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/reference/tables.md
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/reference/tabs.md
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/examples/reference/text-formatting.md
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/docs/web-components.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-24 14:31:45.667967 bulma_sphinx_theme-0.0.1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)   130410 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/postcss.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/_toctree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/_translations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/base/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/base/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/base/_theme.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/base/_typography.scss
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/bulma-sphinx-theme.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/components/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/components/_article-bottom.scss
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/components/_article-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/components/_breadcrumbs.scss
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/components/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/components/_scrollbar.scss
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/components/_search-field.sass
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/components/_search-results.scss
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/components/_search.sass
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/components/_sidenav-panel.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_admonitions.sass
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_api.sass
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_blocks.sass
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_code.sass
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_gui-labels.sass
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_images.sass
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_indexes.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_lists.scss
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_math.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_misc.sass
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_rubrics.sass
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_tables.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_target.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/extensions/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/extensions/_togglebutton.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-content.scss
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-main.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/sections/_footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/sections/_index.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/variables/_colors.scss
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/variables/_definition.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/variables/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/variables/_layout.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/translations/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/translations/jsons/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/translations/jsons/Back to top.json
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/translations/jsons/with.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/demo/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/demo/sphinxext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/back-to-top.html
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/copyright.html
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/header-icons.html
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/navbar-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-wrapper.html
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/searchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-panel.html
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sphinx-version.html
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-24 14:31:45.671967 bulma_sphinx_theme-0.0.1/webpack.config.js
--rw-r--r--   0        0        0     3758 1970-01-01 00:00:00.000000 bulma_sphinx_theme-0.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:29:01.740501 bulma_sphinx_theme-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-25 08:28:40.760233 bulma_sphinx_theme-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-25 08:28:40.760233 bulma_sphinx_theme-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-25 08:28:40.760233 bulma_sphinx_theme-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-25 08:28:40.760233 bulma_sphinx_theme-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.760233 bulma_sphinx_theme-0.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-05-25 08:28:40.760233 bulma_sphinx_theme-0.0.2/docs/_static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-25 08:28:40.760233 bulma_sphinx_theme-0.0.2/docs/_static/logo-.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-25 08:28:40.760233 bulma_sphinx_theme-0.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-25 08:28:40.760233 bulma_sphinx_theme-0.0.2/docs/develop.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-25 08:28:40.760233 bulma_sphinx_theme-0.0.2/docs/examples/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/admonitions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/blocks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/generic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/images.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/lists.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/really-long.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/sphinx-design.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/typography.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/reference/admonitions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/reference/code-blocks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/reference/hyperlinks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/reference/images.md
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/reference/lists.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/reference/tables.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/reference/tabs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/examples/reference/text-formatting.md
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/docs/web-components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130410 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/postcss.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/_toctree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/_translations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/base/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/base/_theme.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/base/_typography.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/bulma-sphinx-theme.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_article-bottom.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_article-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_brand-logo.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_breadcrumbs.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_last-updated.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_scrollbar.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_search-field.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_search-results.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_search.sass
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_sidenav-brand.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_sidenav-panel.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_admonitions.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_api.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_blocks.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_code.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_gui-labels.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_images.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_indexes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_lists.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_math.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_misc.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_rubrics.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_tables.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_target.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/extensions/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/extensions/_togglebutton.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/sections/_bulma-content.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/sections/_bulma-main.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/sections/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/sections/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/_colors.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/_definition.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/_layout.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/_spacing.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/translations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/translations/jsons/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/translations/jsons/Back to top.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/translations/jsons/with.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.764232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/demo/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/demo/sphinxext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/back-to-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/copyright.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/header-icons.html
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/navbar-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-wrapper.html
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sphinx-version.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/sidenav.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-25 08:28:40.768232 bulma_sphinx_theme-0.0.2/webpack.config.js
+-rw-r--r--   0        0        0     4297 1970-01-01 00:00:00.000000 bulma_sphinx_theme-0.0.2/PKG-INFO
```

### Comparing `bulma_sphinx_theme-0.0.1/LICENSE` & `bulma_sphinx_theme-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/README.md` & `bulma_sphinx_theme-0.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -4,36 +4,41 @@
 
 <p align="center">
   <strong>
     A <a href="https://bulma.io/">bulma</a> based <a href="https://www.sphinx-doc.org/en/master/">sphinx</a> theme.
   </strong>
 </p>
 
+<!-- start badges -->
+
+[![deploy](https://img.shields.io/readthedocs/bulma-sphinx-theme?style=flat-square&logo=readthedocs&logoColor=white)](https://bulma-sphinx-theme.readthedocs.io/en/latest/)
+[![Downloads](https://img.shields.io/pypi/dm/bulma-sphinx-theme.svg?style=flat-square)](https://pypistats.org/packages/bulma-sphinx-theme)
 [![PyPI](https://img.shields.io/pypi/v/bulma-sphinx-theme?style=flat-square&logo=python&logoColor=white&color=orange)](https://pypi.org/project/bulma-sphinx-theme/)
 [![status](https://img.shields.io/pypi/status/bulma-sphinx-theme.svg?style=flat-square)](https://pypi.org/project/bulma-sphinx-theme/)
 [![license](https://img.shields.io/pypi/l/bulma-sphinx-theme.svg?style=flat-square&logo=opensourceinitiative&logoColor=white)](https://github.com/zclab/bulma-sphinx-theme/blob/main/LICENSE)
+[![Github Stars](https://img.shields.io/github/stars/zclab/bulma-sphinx-theme?style=flat-square&logo=github)](https://github.com/zclab/bulma-sphinx-theme)
 
-## Installation and usage
+<!-- end badges -->
 
-<!-- start quickstart -->
+## Get started
 
-To use this theme in the repository, follow these steps:
+<!-- start quickstart -->
 
-1. Install the `bulma-sphinx-theme` in your doc build environment:
+To use this theme in your documentation build environment, first install the `bulma-sphinx-theme` with `pip`:
 
-   ```
-   pip install bulma-sphinx-theme
-   ```
+```
+pip install bulma-sphinx-theme
+```
 
-2. Configure the Sphinx docs to use the theme by editing `conf.py`
+then, configure the Sphinx docs to use the theme by editing `conf.py`
 
-   ```python
-   html_theme = "bulma_sphinx_theme"
-   ```
+```python
+html_theme = "bulma_sphinx_theme"
+```
 
-3. Your Sphinx documentation's HTML pages will now be generated with this theme! 🎉
+Your Sphinx documentation's HTML pages will now be generated with this theme! 🎉
 
 <!-- end quickstart -->
 
-## Bulma Documentation
+## Documentation
 
-See [Bulma Documentation](https://bulma.io/). [Free Bulma Templates](https://bulmatemplates.github.io/bulma-templates/).
+See [the bulma sphinx theme](https://bulma-sphinx-theme.readthedocs.io/en/latest/) for more information. Your can also refer to [Bulma Documentation](https://bulma.io/) for more sophisticated change.
```

#### html2text {}

```diff
@@ -1,16 +1,23 @@
                        ****** Bulma Sphinx Theme ******
                           A bulma based sphinx theme.
-[![PyPI](https://img.shields.io/pypi/v/bulma-sphinx-theme?style=flat-
-square&logo=python&logoColor=white&color=orange)](https://pypi.org/project/
-bulma-sphinx-theme/) [![status](https://img.shields.io/pypi/status/bulma-
-sphinx-theme.svg?style=flat-square)](https://pypi.org/project/bulma-sphinx-
-theme/) [![license](https://img.shields.io/pypi/l/bulma-sphinx-
+ [![deploy](https://img.shields.io/readthedocs/bulma-sphinx-theme?style=flat-
+square&logo=readthedocs&logoColor=white)](https://bulma-sphinx-
+theme.readthedocs.io/en/latest/) [![Downloads](https://img.shields.io/pypi/dm/
+bulma-sphinx-theme.svg?style=flat-square)](https://pypistats.org/packages/
+bulma-sphinx-theme) [![PyPI](https://img.shields.io/pypi/v/bulma-sphinx-
+theme?style=flat-square&logo=python&logoColor=white&color=orange)](https://
+pypi.org/project/bulma-sphinx-theme/) [![status](https://img.shields.io/pypi/
+status/bulma-sphinx-theme.svg?style=flat-square)](https://pypi.org/project/
+bulma-sphinx-theme/) [![license](https://img.shields.io/pypi/l/bulma-sphinx-
 theme.svg?style=flat-square&logo=opensourceinitiative&logoColor=white)](https:/
-/github.com/zclab/bulma-sphinx-theme/blob/main/LICENSE) ## Installation and
-usage  To use this theme in the repository, follow these steps: 1. Install the
-`bulma-sphinx-theme` in your doc build environment: ``` pip install bulma-
-sphinx-theme ``` 2. Configure the Sphinx docs to use the theme by editing
-`conf.py` ```python html_theme = "bulma_sphinx_theme" ``` 3. Your Sphinx
-documentation's HTML pages will now be generated with this theme! ð  ##
-Bulma Documentation See [Bulma Documentation](https://bulma.io/). [Free Bulma
-Templates](https://bulmatemplates.github.io/bulma-templates/).
+/github.com/zclab/bulma-sphinx-theme/blob/main/LICENSE) [![Github Stars](https:
+//img.shields.io/github/stars/zclab/bulma-sphinx-theme?style=flat-
+square&logo=github)](https://github.com/zclab/bulma-sphinx-theme)  ## Get
+started  To use this theme in your documentation build environment, first
+install the `bulma-sphinx-theme` with `pip`: ``` pip install bulma-sphinx-theme
+``` then, configure the Sphinx docs to use the theme by editing `conf.py`
+```python html_theme = "bulma_sphinx_theme" ``` Your Sphinx documentation's
+HTML pages will now be generated with this theme! ð  ## Documentation See
+[the bulma sphinx theme](https://bulma-sphinx-theme.readthedocs.io/en/latest/
+) for more information. Your can also refer to [Bulma Documentation](https://
+bulma.io/) for more sophisticated change.
```

### Comparing `bulma_sphinx_theme-0.0.1/docs/_static/favicon.png` & `bulma_sphinx_theme-0.0.2/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/_static/logo-.png` & `bulma_sphinx_theme-0.0.2/docs/_static/logo-.png`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/conf.py` & `bulma_sphinx_theme-0.0.2/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import sys
+import datetime
 from os.path import abspath, join, dirname
 import bulma_sphinx_theme
 
 sys.path.insert(0, abspath(join(dirname(__file__), "../src")))
 
 project = "A sphinx theme based on bulma"
-copyright = "2023"
 author = "zclab"
+year = str(datetime.date.today().year)
+copyright = year + " " + author
 master_doc = "index"
 version = bulma_sphinx_theme.__version__
 language = "en"  #'zh_CN'
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.extlinks",
@@ -55,38 +57,48 @@
 html_css_files = [
     "https://cdn.jsdelivr.net/gh/duyplus/fontawesome-pro/css/all.min.css",
 ]
 
 html_theme_options = {
     "header_links_before_dropdown": 3,
     "navbar_color_style": "is-white",  # see styles: https://bulma.io/documentation/components/navbar/#colors
+    "logo": {"text": "Bulma Sphinx", "logo": "_static/logo-.png"},
     "header_icons": [
         {
             "name": "Github",
             "url": "https://github.com/zclab/bulma-sphinx-theme",
-            "fontawesome": "fa-brands fa-lg fa-github",
+            "image": "https://www.svgrepo.com/show/433505/github-o.svg",
+        },
+        {
+            "name": "Bulma",
+            "url": "https://bulma.io/",
+            "image": "https://bulma.io/favicons/favicon.ico",
+        },
+        {
+            "name": "Pydata",
+            "url": "https://pydata-sphinx-theme.readthedocs.io/en/latest/",
+            "image": "https://pydata-sphinx-theme.readthedocs.io/en/latest/_static/pydata-logo.png",
         },
     ],
     "external_links": [
         {"name": "Furo", "url": "https://pradyunsg.me/furo/quickstart/"},
         {
             "name": "Sphinx book theme",
             "url": "https://sphinx-book-theme.readthedocs.io/en/latest/",
         },
         {
-            "name": "Pydata sphinx theme",
-            "url": "https://pydata-sphinx-theme.readthedocs.io/",
-        },
-        {
             "name": "Hugging Face community",
             "url": "https://huggingface.co/docs/transformers/index",
         },
         {
             "name": " Docusaurus",
             "url": "https://docusaurus.io/",
         },
     ],
     "source_repository": "https://github.com/zclab/bulma-sphinx-theme",
     "source_branch": "main",
     "source_directory": "docs/",
     "use_edit_page_button": True,
+    "fix_navbar": True,
+    "navbar_start": [],
+    "navbar_end": ["navbar-nav.html", "header-icons.html"],
 }
```

### Comparing `bulma_sphinx_theme-0.0.1/docs/develop.md` & `bulma_sphinx_theme-0.0.2/docs/develop.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/admonitions.rst` & `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/admonitions.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/api.rst` & `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/api.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/blocks.rst` & `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/blocks.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/generic.rst` & `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/generic.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/images.rst` & `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/images.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/index.md` & `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/lists.rst` & `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/lists.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/really-long.md` & `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/really-long.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/sphinx-design.md` & `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/sphinx-design.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/structure.rst` & `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/structure.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/tables.rst` & `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/tables.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/examples/kitchen-sink/typography.rst` & `bulma_sphinx_theme-0.0.2/docs/examples/kitchen-sink/typography.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/examples/reference/admonitions.md` & `bulma_sphinx_theme-0.0.2/docs/examples/reference/admonitions.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/examples/reference/api.md` & `bulma_sphinx_theme-0.0.2/docs/examples/reference/api.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/examples/reference/code-blocks.md` & `bulma_sphinx_theme-0.0.2/docs/examples/reference/code-blocks.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/examples/reference/hyperlinks.md` & `bulma_sphinx_theme-0.0.2/docs/examples/reference/hyperlinks.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/examples/reference/images.md` & `bulma_sphinx_theme-0.0.2/docs/examples/reference/images.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/examples/reference/index.md` & `bulma_sphinx_theme-0.0.2/docs/examples/reference/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/examples/reference/lists.md` & `bulma_sphinx_theme-0.0.2/docs/examples/reference/lists.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/examples/reference/tables.md` & `bulma_sphinx_theme-0.0.2/docs/examples/reference/tables.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/examples/reference/tabs.md` & `bulma_sphinx_theme-0.0.2/docs/examples/reference/tabs.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/examples/reference/text-formatting.md` & `bulma_sphinx_theme-0.0.2/docs/examples/reference/text-formatting.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/docs/web-components.rst` & `bulma_sphinx_theme-0.0.2/docs/web-components.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/noxfile.py` & `bulma_sphinx_theme-0.0.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/package-lock.json` & `bulma_sphinx_theme-0.0.2/package-lock.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/package.json` & `bulma_sphinx_theme-0.0.2/package.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/pyproject.toml` & `bulma_sphinx_theme-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/__init__.py` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Any, Dict, List
 from sphinx.builders.html import StandaloneHTMLBuilder
 from sphinx.locale import get_translation
 from ._toctree import add_toctree_functions
 from ._transforms import ShortenLinkTransform, WrapTableAndMathInAContainerTransform
 from .utils import get_theme_options
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 logger = logging.getLogger(__name__)
 MESSAGE_CATALOG_NAME = "bulmasphinxtheme"
 
 
 def _get_html_theme_path():
     """Return list of HTML theme paths."""
     parent = Path(__file__).parent.resolve()
```

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/_toctree.py` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/_toctree.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/_transforms.py` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/_transforms.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/_translations.py` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/_translations.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -235,19 +235,59 @@
     // Add the search button overlay event callback
     let overlay = document.querySelector(".search-button__overlay");
     if (overlay) {
         overlay.onclick = toggleSearchField;
     }
 };
 
+/*******************************************************************************
+ * dropdown trigger setup for bulma, see https://bulma.io/lib/main.js?v=202305240833
+ */
+
+function getAll(selector) {
+    var parent =
+        arguments.length > 1 && arguments[1] !== undefined ?
+        arguments[1] :
+        document;
+
+    return Array.prototype.slice.call(parent.querySelectorAll(selector), 0);
+}
+
+var setupDropdwon = () => {
+    var $dropdowns = getAll(".dropdown:not(.is-hoverable)");
+
+    if ($dropdowns.length > 0) {
+        $dropdowns.forEach(function($el) {
+            $el.addEventListener("click", function(event) {
+                event.stopPropagation();
+                $el.classList.toggle("is-active");
+            });
+        });
+
+        document.addEventListener("click", function(event) {
+            closeDropdowns();
+        });
+    }
+
+    function closeDropdowns() {
+        $dropdowns.forEach(function($el) {
+            $el.classList.remove("is-active");
+        });
+    }
+};
+/*******************************************************************************
+ * dropdown trigger ended
+ */
+
 ////////////////////////////////////////////////////////////////////////////////
 // Main entrypoint
 ////////////////////////////////////////////////////////////////////////////////
 function main() {
     document.body.parentNode.classList.remove("no-js");
     setupSearchButtons();
+    setupDropdwon();
     header = document.querySelector(".navbar");
     tocScroll = document.querySelector(".toc-scroll");
     setup();
 }
 
 document.addEventListener("DOMContentLoaded", main);
```

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/base/_typography.scss` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/base/_typography.scss`

 * *Files 8% similar despite different names*

```diff
@@ -76,16 +76,16 @@
 
 p {
   margin-top: 0.5rem;
   margin-bottom: 0.75rem;
 }
 
 .columns {
-  margin-left: 2rem;
-  margin-right: 2rem;
+  margin-left: 1rem;
+  margin-right: 1rem;
   margin-top: 0;
 
   /* the columns:last-child fix body height have a small gap to screen bottom */
   &:last-child {
     margin-bottom: 0;
   }
 }
```

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .back-to-top {
   text-decoration: none;
-  top: calc($navbar-height + 1.5rem);
+  top: calc(var(--navbar-height) + var(--top-content-to-navbar-gap));
 
   display: none;
   position: fixed;
   left: 0;
   // top: 1rem;
   padding: 0.5rem;
   padding-right: 0.75rem;
```

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_admonitions.sass` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_admonitions.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_api.sass` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_api.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_code.sass` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_code.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_images.sass` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_images.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_lists.scss` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_lists.scss`

 * *Files 6% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         content: ":";
         margin-left: 0.2rem;
         margin-right: 0.2rem;
       }
     }
 
     dd {
-      padding-left: 1.2rem;
+      margin-left: 1.2rem;
 
       > p:first-child,
       ul {
         margin-top: 0.125rem;
       }
 
       ul {
```

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_misc.sass` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_misc.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_tables.sass` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_tables.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/content/_target.sass` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/content/_target.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 .bulma-sidenav {
   display: block;
   clip-path: inset(0);
   background-color: var(--color-background-sidenav);
   width: var(--sidenav-width);
   border-right: 1px solid var(--color-background-border);
-  z-index: 100;
+  margin-top: calc(
+    var(--navbar-height) * var(--sidenav-sticky-top-factor) * -1
+  );
 
   .sidenav-viewport {
     height: 100%;
     max-height: 100vh;
     position: sticky;
     top: 0;
```

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 .bulma-tocnav {
   width: var(--tocnav-width);
-  padding: 2rem 1rem 1rem;
+  padding: 0 1rem;
 
   .toc-wrapper {
     position: sticky;
-    top: calc($navbar-height + 2rem);
+    top: calc(var(--navbar-height) + var(--top-content-to-navbar-gap));
     overflow: hidden;
   }
 
   ul.table-of-contents {
     font-size: var(--toc-font-size);
 
     li {
```

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/variables/_colors.scss` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/_colors.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/translations/README.md` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/translations/README.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/demo/module.py` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/demo/module.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/demo/sphinxext.py` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/demo/sphinxext.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,22 +74,22 @@
 
     string_list.extend(_rst_demo(rst))
     string_list.extend(_md_demo(md))
 
     return string_list
 
 
-class _STMbDemoDirective(SphinxDirective):
+class _BULMASPHINXDemoDirective(SphinxDirective):
     has_content = True
 
     def run(self) -> Any:
         self.assert_has_content()
 
         container = nodes.container()
         transated_content = _translate_into_tab_demo(self.block_text)
         self.state.nested_parse(transated_content, 0, container)
         return [container]
 
 
 def setup(app: Sphinx) -> None:
     """For setting up the directive."""
-    app.add_directive("bulma-demo", _STMbDemoDirective)
+    app.add_directive("bulma-demo", _BULMASPHINXDemoDirective)
```

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html`

 * *Files 5% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     <link rel="stylesheet" href="{{ pathto(css, 1)|e }}" type="text/css" />
     {%- endif %}
     {% endfor -%}
     {%- endblock regular_styles -%}
 
     {#- Theme-related stylesheets -#}
     {%- block theme_styles %}
+    {% include "partials/_css_variables_define.html" with context %}
     {%- endblock theme_styles -%}
 
     {%- block extra_styles %}
     {%- endblock extra_styles -%}
 
     {{ _webpack.head_js_preload() }}
     {%- endblock styles -%}
```

#### html2text {}

```diff
@@ -21,15 +21,16 @@
 htmltitle -%} {% if not docstitle %}
 {% elif pagename == master_doc %}
 {% else %}
 {% endif %} {%- endblock htmltitle -%} {%- block styles -%} {# Custom
 stylesheets #} {%- block regular_styles -%} {%- for css in css_files -%} {% if
 css|attr("filename") -%} {{ css_tag(css) }} {%- else -%}
  {%- endif %} {% endfor -%} {%- endblock regular_styles -%} {#- Theme-related
-stylesheets -#} {%- block theme_styles %} {%- endblock theme_styles -%} {%-
+stylesheets -#} {%- block theme_styles %} {% include "partials/
+_css_variables_define.html" with context %} {%- endblock theme_styles -%} {%-
 block extra_styles %} {%- endblock extra_styles -%} {{ _webpack.head_js_preload
 () }} {%- endblock styles -%} {#- Custom front matter #} {%- block extrahead -
 %}{%- endblock extrahead -%}
 {% block htmlbody %} {% endblock htmlbody %} {%- block scripts -%} {# Custom JS
 #} {%- block regular_scripts -%} {% for path in script_files -%} {{ js_tag
 (path) }} {% endfor -%} {%- endblock regular_scripts -%} {# Theme-related
 JavaScript code #} {%- block theme_scripts -%} {{ _webpack.body_post() }} {%-
```

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-panel.html` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-panel.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,17 @@
                 <article role="main" class="column is-three-quarters article-container">
                     {% include "sections/article-top.html" %}
                     {% include "components/searchbox.html" %}
 
                     {% block body %}{{ body }}{% endblock body %}
 
                     {% include "sections/article-bottom.html" %}
+                    {% if theme_show_prev_next %}
                     {% include "components/prev-next.html" %}
+                    {% endif %}
                 </article>
 
                 {% set page_toc = generate_toc_html() %}
                 {%- if page_toc | length >= 1 %}
                 <aside class="column is-one-quarter bulma-tocnav is-hidden-mobile">
                     <div class="toc-wrapper toc-scroll">
                         {% if theme_toc_title %}
```

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html`

 * *Files 2% similar despite different names*

```diff
@@ -8,13 +8,13 @@
     {% if icon_dict.class %}
     <i class="{{ icon_dict.class }}"></i>
     {% elif icon_dict.material_icons %}
     <i class="material-icons">{{ icon_dict.material_icons }}</i>
     {% elif icon_dict.fontawesome %}
     <i class="{{ icon_dict.fontawesome }}"></i>
     {% elif icon_dict.image %}
-    <img src="{{ icon_dict.image }}" class="stm-icon-image" alt="{{ icon_dict.name }}" />
+    <img src="{{ icon_dict.image }}" class="bulma-icon-image" alt="{{ icon_dict.name }}" />
     {% endif %}
 </a>
 {% endfor %}
 {%- endif %}
 {%- endmacro %}
```

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf`

 * *Files 11% similar despite different names*

```diff
@@ -9,16 +9,19 @@
 [options]
 navigation_depth = 4
 show_nav_level = 1
 show_toc_level = 1
 header_links_before_dropdown = 4
 external_links =
 header_icons =
+logo =
 fix_navbar =
-navbar_color_style = is-link
+
+# see navbar color styles: https://bulma.io/documentation/components/navbar/#colors
+navbar_color_style = is-white
 navbar_start = navbar-nav.html
 navbar_end = header-icons.html
 analytics =
 footer = copyright.html, sphinx-version.html
 toc_title = On this page
 dropdown_label_name = More
 navigation_with_keys = True
@@ -29,7 +32,10 @@
 article_bottom_left = last-updated.html
 article_bottom_right = sourcelink.html
 use_edit_page_button =
 source_repository =
 source_branch =
 source_directory =
 source_edit_link =
+show_prev_next = True
+css_variables =
+dark_css_variables =
```

### Comparing `bulma_sphinx_theme-0.0.1/src/bulma_sphinx_theme/utils.py` & `bulma_sphinx_theme-0.0.2/src/bulma_sphinx_theme/utils.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.1/webpack.config.js` & `bulma_sphinx_theme-0.0.2/webpack.config.js`

 * *Files identical despite different names*

