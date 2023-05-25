# Comparing `tmp/imio.smartweb.core-1.1.8.tar.gz` & `tmp/imio.smartweb.core-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imio.smartweb.core-1.1.8.tar", last modified: Wed Mar 15 09:52:13 2023, max compression
+gzip compressed data, was "dist/imio.smartweb.core-1.1.9.tar", last modified: Fri Mar 17 15:05:01 2023, max compression
```

## Comparing `imio.smartweb.core-1.1.8.tar` & `imio.smartweb.core-1.1.9.tar`

### file list

```diff
@@ -1,780 +1,780 @@
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/docs/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7994 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/docs/conf.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       63 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/docs/index.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       64 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/requirements.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      522 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/DEVELOP.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    47716 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      169 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/CONTRIBUTORS.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3610 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/README.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/LICENSE.GPL
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    30223 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/CHANGES.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      188 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/MANIFEST.in
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3010 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/setup.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      653 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/LICENSE.rst
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/setup.cfg
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio.smartweb.core.egg-info/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio.smartweb.core.egg-info/top_level.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    47716 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio.smartweb.core.egg-info/PKG-INFO
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio.smartweb.core.egg-info/dependency_links.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      623 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio.smartweb.core.egg-info/requires.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       19 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio.smartweb.core.egg-info/namespace_packages.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    39313 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio.smartweb.core.egg-info/SOURCES.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio.smartweb.core.egg-info/not-zip-safe
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3636 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/testing.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/css/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2392 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/css/323.smartweb-webcomponents-compiled.css
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    19109 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/css/195.smartweb-webcomponents-compiled.css
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    17010 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/css/552.smartweb-webcomponents-compiled.css
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3786 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/css/510.smartweb-webcomponents-compiled.css
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4553 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/css/smartweb-webcomponents-compiled.css
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   158609 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/9.smartweb-webcomponents-compiled.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      149 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/323.smartweb-webcomponents-compiled.js.LICENSE.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    36695 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/195.smartweb-webcomponents-compiled.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    12270 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/842.smartweb-webcomponents-compiled.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      361 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/650.smartweb-webcomponents-compiled.js.LICENSE.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    26666 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/323.smartweb-webcomponents-compiled.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1035 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/smartweb-webcomponents-compiled.js.LICENSE.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    15195 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/969.smartweb-webcomponents-compiled.js.LICENSE.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   314986 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/smartweb-webcomponents-compiled.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    17480 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/144.smartweb-webcomponents-compiled.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      153 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/9.smartweb-webcomponents-compiled.js.LICENSE.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   131033 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/462.smartweb-webcomponents-compiled.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    29317 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/552.smartweb-webcomponents-compiled.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   168291 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/650.smartweb-webcomponents-compiled.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       59 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/144.smartweb-webcomponents-compiled.js.LICENSE.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   363927 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/969.smartweb-webcomponents-compiled.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      149 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/842.smartweb-webcomponents-compiled.js.LICENSE.txt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    30801 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/510.smartweb-webcomponents-compiled.js
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/assets/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1259 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/assets/layers-2x.8f2c4d11474275fbc1614b9098334eae.png
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1466 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/assets/marker-icon.2b3e1faf89f94a4835397e7a43b4f77d.png
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      696 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/assets/layers.416d91365b44e4b4f4777663e6f009f3.png
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      628 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/assets/next-react-white.819cb069ac8eec300a9db6a7707712d6.svg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      426 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/assets/search.57bdbf5b191499cd77514097d1c4972c.svg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      433 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/assets/oeil-big.f32cd1df1274a9593de0c4bd8e344216.svg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      336 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/assets/pin-react.fda934b5daf26dd4da2a71a7e7e44431.svg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      628 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/assets/next-react.17bc43ff4a6a86f4520f5782f6a89a72.svg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      348 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/assets/location-bla.1423bcce16ddcb21141430cac1428dc1.svg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9538 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/assets/img-placeholder-bla.a2b8b384c46ce56c99f042dc4625d309.png
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      330 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/assets/pin-react-active.07d154037a15be5525b823fdc626cf29.svg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2226 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/webpackPlonePlugin.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6853 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/webpack.config.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       92 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/.npmrc
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      621 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/Makefile
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      194 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/babel.config.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      101 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/postcss.config.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      343 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/.eslintrc.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2531 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/package.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       67 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/.prettierrc.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       31 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/README.md
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      263 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/hooks/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1215 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/hooks/useAxios.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      223 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/hooks/useFilterQuery.js
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactContent/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    16563 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactContent/ContactContent.jsx
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactList/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1675 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactList/ContactList.jsx
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactCard/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2043 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactCard/ContactCard.jsx
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8772 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/Events.jsx
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/Skeleton/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      656 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/Skeleton/Skeleton.jsx
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       95 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/index.js
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactMap/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactMap/ContactMap.scss
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5725 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactMap/ContactMap.jsx
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7166 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/Events.scss
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/Filters/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6272 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/Filters/Filter.jsx
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/ContactResult/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1853 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/ContactResult/ContactResult.jsx
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/Skeleton/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      656 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/Skeleton/Skeleton.jsx
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       95 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/index.js
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/NewsResult/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2502 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/NewsResult/NewsResult.jsx
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/WebResult/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1831 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/WebResult/WebResult.jsx
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2570 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/Search.scss
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/EventsResult/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2475 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/EventsResult/EventsResult.jsx
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2271 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/Search.jsx
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/Filters/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6510 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/Filters/Filter.jsx
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactContent/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    16354 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactContent/ContactContent.jsx
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4968 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Annuaire.scss
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactList/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1678 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactList/ContactList.jsx
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactCard/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3962 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactCard/ContactCard.jsx
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8751 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Annuaire.jsx
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Skeleton/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      656 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Skeleton/Skeleton.jsx
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      217 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Skeleton/LoaderCss.jsx
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       97 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/index.js
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactMap/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       73 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactMap/ContactMap.scss
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5770 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactMap/ContactMap.jsx
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Filters/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7637 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Filters/Filter.jsx
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactContent/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    12558 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactContent/ContactContent.jsx
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactList/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1493 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactList/ContactList.jsx
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactCard/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3039 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactCard/ContactCard.jsx
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3293 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/News.scss
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6840 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/News.jsx
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/Skeleton/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      656 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/Skeleton/Skeleton.jsx
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       93 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/index.js
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactMap/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       42 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactMap/ContactMap.scss
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4216 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactMap/ContactMap.jsx
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/Filters/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6249 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/Filters/Filter.jsx
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/assets/
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      426 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/assets/search.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      628 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/assets/next-react-white.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      336 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/assets/pin-react.svg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      799 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/assets/facebook-news.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      628 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/assets/next-react.svg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      884 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/assets/pin-active.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      453 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/assets/skeleton.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      348 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/assets/location-bla.svg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      890 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/assets/pin.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      369 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/assets/location-active-bla.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      433 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/assets/oeil-big.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)     9538 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/assets/img-placeholder-bla.png
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      478 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/assets/close.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      330 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/assets/pin-react-active.svg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      757 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/index.jsx
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4681 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/index.scss
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/utils/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      244 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/utils/url.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2694 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/utils/translation.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      858 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/interfaces.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/behaviors/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1865 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/behaviors/minisite.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1063 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/behaviors/quickaccess.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/behaviors/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1707 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/behaviors/subsite.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      760 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/behaviors/listing.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1459 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/behaviors/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5080 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/vocabularies.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      879 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/setuphandlers.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    10699 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_page.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2403 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2655 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_section_sendinblue.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4632 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_text.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7215 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_portal_page.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7787 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_banner.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3505 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_section_news.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4997 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_local_roles.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4921 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_cirkwiview.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4274 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_instance_behaviors.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2388 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_toolbar.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    14084 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_vocabularies.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2425 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_logo.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2194 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_rest_directory.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      369 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_search_one_news_entity.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      921 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_contacts_raw_mock.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4820 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_contact_empty_schedule_raw_mock.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3109 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_contact_images_raw_mock.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    24753 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/plone.png
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      150 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/cirkwi_bad_widget_mock.html
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      441 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_events_entities_raw_mock.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2346 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_rest_specific_events.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      783 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_news_newsfolder_raw_mock.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      749 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_directory_entities_raw_mock.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      726 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_news_entities_raw_mock.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      168 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_no_newsfolder_raw_mock.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2882 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_rest_specific_news.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      359 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_auth_sources_news_entity.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      127 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_no_contact_raw_mock.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      363 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_auth_sources_events_entity.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      390 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_events_types_raw_mock.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3974 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_rest_news.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_used_iam_vocabularies_jobseeker_tourist.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3823 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/plone.svg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3217 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_procedures_raw_mock.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    11488 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_contact_raw_mock.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      156 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_contact_no_image_raw_mock.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4399 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_rest_events.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3454 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_contact_category_raw_mock.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      369 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_auth_sources_directory_entity.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      769 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_events_agendas_raw_mock.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   333252 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/cirkwi_good_widget_mock.html
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3030 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_social.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    12782 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_folder.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2374 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2182 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_search.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    10784 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_indexes.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    12109 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_default_pages.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6799 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_navigation.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3193 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_section_events.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5940 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_herobanner.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/robot/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2548 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/robot/test_ct_page.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2003 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/robot/test_example.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2596 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/robot/test_ct_folder.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2712 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/robot/test_ct_procedure.robot
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5950 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_behaviors.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6474 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_procedure.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    20188 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_section_contact.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5120 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_faceted.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    22076 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_sections.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2779 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_icons.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2012 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_categories.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1161 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_chatbot.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    10950 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_footer.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    16632 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_minisite.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2092 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_setup.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5232 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_cropping.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9016 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_subsite.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    13823 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_rest.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      926 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_robot.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/faceted/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      395 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/faceted/layout.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      295 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/faceted/menu.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/faceted/config/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2906 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/faceted/config/collection.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/faceted/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      826 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/faceted/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/icons/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/icons/basic/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    17858 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/icons/basic/registry.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/uninstall/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      128 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/uninstall/browserlayer.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/testing/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      706 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/testing/registry.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/testing/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      215 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/testing/types/Document.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      468 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/testing/types/Collection.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      213 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/testing/types/Folder.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      163 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/testing/types.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      227 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/testing/metadata.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/taxonomies/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      320 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/taxonomies/procedure_category.cfg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2059 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/taxonomies/page_category.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3436 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/taxonomies/procedure_category.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      310 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/taxonomies/page_category.cfg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5877 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/actions.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      864 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/catalog.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1010 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/workflows.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1533 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionFiles.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2419 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Procedure.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1284 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionText.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1210 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionVideo.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1185 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionMap.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1508 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.DirectoryView.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1229 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionHTML.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1457 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionCollection.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1476 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.NewsView.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1493 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.EventsView.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2422 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Page.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1474 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.CirkwiView.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1185 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSendinblue.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1730 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Footer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1170 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSlide.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1500 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSelections.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2460 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Folder.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1177 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionContact.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1589 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionLinks.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2598 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.PortalPage.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1478 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionEvents.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1172 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionPostit.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1402 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.BlockLink.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1392 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionGallery.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1472 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionNews.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1604 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.HeroBanner.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1958 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      183 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/repositorytool.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      400 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/controlpanel.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1143 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/metadata.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2510 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/rolemap.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      179 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/browserlayer.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      253 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/registry/smartweb.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1251 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/registry/geolocation.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2562 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/registry/bundles.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2384 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/registry/plone.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/last_compilation/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      852 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/last_compilation/registry.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      821 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/subscribers.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      968 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/indexers.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1737 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1345 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/view_section.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4817 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/views.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      961 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/subscriber.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/footer/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1374 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/footer/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/footer/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/footer/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      464 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/pages.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/page/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      465 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/page/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/page/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/page/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/cirkwi/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      664 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/cirkwi/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/cirkwi/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      392 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/cirkwi/view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      378 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/cirkwi/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      482 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/cirkwi/view.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/procedure/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1297 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/procedure/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1291 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/procedure/utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/procedure/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      356 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/procedure/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      408 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/procedure/view.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/herobanner/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1077 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/herobanner/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/herobanner/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/herobanner/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2983 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/view.pt
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/portal_page/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      336 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/portal_page/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/portal_page/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      352 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/portal_page/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      147 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/portal_page/view.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2252 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/folder/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3348 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/folder/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5570 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/folder/views.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      342 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/folder/element_view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1743 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/folder/macros.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      920 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/folder/summary_view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1194 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/folder/block_view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/folder/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2961 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/folder/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/slide/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2181 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/slide/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/slide/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2440 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/slide/view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      417 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/slide/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      784 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/slide/view.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1989 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/views.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      642 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/subscriber.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/video/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      978 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/video/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      342 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/video/views.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/video/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1105 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/video/view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      418 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/video/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/postit/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2239 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/postit/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/postit/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      504 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/postit/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      936 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/postit/view.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/html/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1352 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/html/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/html/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1140 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/html/view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      413 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/html/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/files/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      868 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/files/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/files/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      501 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/files/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1196 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/files/view.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/common_templates/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6141 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/common_templates/table.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5132 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/common_templates/carousel.pt
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/text/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1564 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/text/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      372 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/text/views.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/text/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1576 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/text/view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1712 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/text/forms.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1423 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/text/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/events/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2911 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/events/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1522 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/events/macros.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/events/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1117 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/events/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3874 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/events/view.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4293 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/macros.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2486 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/base.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/gallery/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      784 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/gallery/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      415 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/gallery/views.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/gallery/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2150 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/gallery/view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      424 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/gallery/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/collection/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2376 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/collection/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1246 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/collection/views.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/collection/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      920 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/collection/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/contact/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2431 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/contact/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/contact/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9530 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/contact/view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1387 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/contact/forms.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1281 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/contact/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    11974 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/contact/view.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/links/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1051 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/links/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/links/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      918 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/links/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1285 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/links/view.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/selections/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1372 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/selections/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/selections/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      949 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/selections/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1420 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/selections/view.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/news/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2908 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/news/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/news/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      880 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/news/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3440 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/news/view.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/map/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      372 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/map/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      614 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/map/views.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/map/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1278 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/map/view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      412 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/map/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/sendinblue/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1088 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/sendinblue/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1731 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/sendinblue/views.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/sendinblue/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1180 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/sendinblue/view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      433 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/sendinblue/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2200 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/blocks/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      330 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/blocks/subscriber.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/blocks/link/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1407 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/blocks/link/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/blocks/link/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      703 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/blocks/link/icons_input.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      479 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/blocks/link/fields.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      552 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/blocks/link/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/blocks/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      732 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/blocks/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1940 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      735 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/cropping.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/directory/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      923 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/directory/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1979 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/directory/endpoint.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/directory/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      616 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/directory/view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1035 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/directory/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      302 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/directory/view.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/search/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8383 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/search/endpoint.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/search/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      951 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/search/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/events/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1100 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/events/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3721 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/events/endpoint.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/events/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      617 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/events/view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1017 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/events/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      293 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/events/view.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1411 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/base.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/__init__.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/news/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      753 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/news/content.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1858 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/news/endpoint.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/news/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      629 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/news/view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1005 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/news/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      287 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/news/view.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      200 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      567 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/view.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      665 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4483 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/utils.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      531 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/default_page_warning.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      872 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/footer.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      503 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/subsite_logo.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      602 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/procedure.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      872 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/messages.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3216 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/footer.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      577 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/header_actions.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      199 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/social.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3385 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/toolbar.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      137 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/subsite_header_viewlet.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      129 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/offcanvas.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      533 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/offcanvas.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      129 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/header_actions_viewlet.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      611 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/chatbot.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      308 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/menu.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      103 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/category.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2213 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/logo.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7284 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/navigation.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      688 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/herobanner.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      648 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/minisite.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2073 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/banner.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      403 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/searchbox.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      318 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/lead_image.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      661 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/actions.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1277 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/banner.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1359 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/herobanner.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      633 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/procedure.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      367 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/header.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      163 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/subsite_navigation.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      329 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/chatbot.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      370 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/minisite_link.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4218 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/subsite.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      308 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/category.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      738 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/logo.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      137 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/header_top_viewlet.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    11589 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    19917 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/vocabularies.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      337 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/config.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1611 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/permissions.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      173 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/workflows.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      311 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/imio.smartweb.Procedure.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      306 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/imio.smartweb.Page.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      312 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/imio.smartweb.PortalPage.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1157 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/imio.smartweb.SectionPostit.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      180 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1021_to_1022/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      298 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1021_to_1022/rolemap.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1021_to_1022/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      457 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1021_to_1022/registry/hero-banner.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1022_to_1023/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1022_to_1023/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      838 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1022_to_1023/registry/icons.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1474 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/types/imio.smartweb.CirkwiView.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      305 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/types/imio.smartweb.Folder.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      177 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/types.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      298 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/rolemap.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      403 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/registry/plone.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1029_to_1030/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      463 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1029_to_1030/actions.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      256 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1029_to_1030/rolemap.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1020_to_1021/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1020_to_1021/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      244 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1020_to_1021/types/imio.smartweb.SectionHTML.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      538 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1020_to_1021/rolemap.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      321 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.Procedure.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      325 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.DirectoryView.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      320 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.NewsView.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      322 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.EventsView.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      316 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.Page.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      318 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.Folder.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      322 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.PortalPage.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1025_to_1026/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1025_to_1026/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      249 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1025_to_1026/registry/propose-urls.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      249 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionFiles.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      256 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.Procedure.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      248 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionText.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      249 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionVideo.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      241 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionMap.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      252 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.DirectoryView.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      249 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionHTML.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      255 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionCollection.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      245 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.NewsView.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      252 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.EventsView.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      244 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.Page.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      249 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionSendinblue.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      250 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.Footer.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      246 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionSlide.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      254 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionSelections.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      241 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.Folder.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      253 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionContact.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      250 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionLinks.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      256 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.PortalPage.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      246 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionEvents.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      249 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionPostit.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      257 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.BlockLink.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      248 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionGallery.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      248 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionNews.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      247 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.HeroBanner.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1027_to_1028/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1027_to_1028/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      318 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1027_to_1028/registry/open-external-link-in-new-tab.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1036_to_1037/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      440 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1036_to_1037/actions.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      275 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1036_to_1037/rolemap.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1031_to_1032/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1031_to_1032/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      562 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1031_to_1032/registry/spotlight.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1015_to_1016/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1015_to_1016/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      481 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1015_to_1016/registry/e-guichet-icon.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1016_to_1017/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1016_to_1017/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      478 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1016_to_1017/registry/shop-icon.xml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1030_to_1031/
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1030_to_1031/registry/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1425 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1030_to_1031/registry/resources.xml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5245 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/upgrades.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    17069 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       24 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      172 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/testing.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2066 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/layout.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/banner/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      947 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/banner/settings.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/banner/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      389 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/banner/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/templates/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2808 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/templates/link_input.pt
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/search/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2369 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/search/search.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      450 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/search/search.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/search/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      423 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/search/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1582 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/gallery_view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1414 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/views.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4303 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/map.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1382 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/map.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2951 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/macros.pt
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/widgets/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      221 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/widgets/select.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/widgets/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2459 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/widgets/select.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      449 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/widgets/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1667 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/summary_view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1723 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/block_view.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2806 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4648 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/controlpanel.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   135631 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/swiper-bundle.min.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      737 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/smartweb-edit-compiled.css
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    15564 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/swiper-bundle.min.css
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      414 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/action-voir-plan.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      483 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/action-nous-contacter.svg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      873 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/action-e-guichet.svg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1355 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/action-engagement.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      561 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-mobilite.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      826 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/reseausocial-vimeo.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      313 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-avis-et-enquetes.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      294 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/organisation-academie-musique.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      284 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-exposition.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      350 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/vue-actualites.svg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1039 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/reseausocial-twitter.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      625 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/organisation-ecole-des-arts.svg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      302 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-mon-dossier.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      721 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/reseausocial-facebook.svg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1787 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-commerce.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      514 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-sport-trophee.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      522 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/organisation-bibliotheque.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      339 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/vue-agenda.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      662 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-primes.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      451 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/organisation-police.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      458 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-cinema.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)     2086 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/reseausocial-facebook-pouce.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      787 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/action-signaler-un-probleme.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)     1999 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/reseausocial-instagram.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      614 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/organisation-mobilite.svg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      453 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-infos-travaux.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      692 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-mandataires.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      367 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-culture.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      673 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-enseignement.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      307 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/action-organiser-un-evenement.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      419 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-parcs-et-jardins.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      302 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/organisation-ecole.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      252 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-environnement-gestion-des-dechets.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      925 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-sport-velo.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      739 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/organisation-centre-sportif.svg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      318 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-parc-de-stationnement.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)     1011 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-enfance.svg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      590 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/reseausocial-youtube.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      397 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-sport-courir.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      390 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-tourisme.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      274 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/action-email.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      409 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/action-nous-rejoindre.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      426 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-demarches.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      508 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-concert.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      259 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-horaires.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      313 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-associations.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      713 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-theatre.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      497 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/vue-annuaire.svg
--rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      879 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/organisation-cpas.svg
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    19615 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/spotlight-bundle.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1030 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/webpack.config.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      350 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/Makefile
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2608 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/smartweb-view-compiled.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2702 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/smartweb-view-compiled.css
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      695 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/package.json
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      354 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/smartweb-edit-compiled.js
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/src/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4211 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/src/view.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      918 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/src/edit.less
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2843 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/src/view.less
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      581 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/src/edit.js
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/.gitkeep
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/footer/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2492 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/footer/settings.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/footer/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      388 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/footer/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/instancebehaviors/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3052 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/instancebehaviors/form.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      742 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/instancebehaviors/utils.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/instancebehaviors/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      632 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/instancebehaviors/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/overrides/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      978 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/overrides/plone.app.layout.viewlets.sections.pt
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/overrides/.gitkeep
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2065 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/icons.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3058 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/utils.py
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/subsite/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1601 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/subsite/settings.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/subsite/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      414 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/subsite/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/minisite/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2766 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/minisite/settings.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/minisite/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      417 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/minisite/configure.zcml
-drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:13.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/herobanner/
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2884 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/herobanner/settings.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/herobanner/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      400 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/herobanner/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1089 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/forms.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2775 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3887 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/indexers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1818 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/subscribers.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1429 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/core/configure.zcml
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/smartweb/__init__.py
--rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-03-15 09:52:12.000000 imio.smartweb.core-1.1.8/src/imio/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/docs/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7994 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/docs/conf.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       63 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/docs/index.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       64 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/requirements.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      522 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/DEVELOP.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    47931 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      169 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/CONTRIBUTORS.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3610 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/README.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    18092 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/LICENSE.GPL
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    30382 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/CHANGES.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      188 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/MANIFEST.in
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3010 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/setup.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      653 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/LICENSE.rst
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      518 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/setup.cfg
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio.smartweb.core.egg-info/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        5 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio.smartweb.core.egg-info/top_level.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    47931 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio.smartweb.core.egg-info/PKG-INFO
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio.smartweb.core.egg-info/dependency_links.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      623 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio.smartweb.core.egg-info/requires.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       19 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio.smartweb.core.egg-info/namespace_packages.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    39313 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio.smartweb.core.egg-info/SOURCES.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        1 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio.smartweb.core.egg-info/not-zip-safe
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3636 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/testing.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/css/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2392 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/css/323.smartweb-webcomponents-compiled.css
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    19109 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/css/195.smartweb-webcomponents-compiled.css
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    17010 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/css/552.smartweb-webcomponents-compiled.css
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3786 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/css/510.smartweb-webcomponents-compiled.css
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4553 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/css/smartweb-webcomponents-compiled.css
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   158609 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/9.smartweb-webcomponents-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      149 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/323.smartweb-webcomponents-compiled.js.LICENSE.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    36695 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/195.smartweb-webcomponents-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    12270 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/842.smartweb-webcomponents-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      361 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/650.smartweb-webcomponents-compiled.js.LICENSE.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    26666 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/323.smartweb-webcomponents-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1035 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/smartweb-webcomponents-compiled.js.LICENSE.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    15195 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/969.smartweb-webcomponents-compiled.js.LICENSE.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   314986 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/smartweb-webcomponents-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    17480 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/144.smartweb-webcomponents-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      153 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/9.smartweb-webcomponents-compiled.js.LICENSE.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   131033 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/462.smartweb-webcomponents-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    29317 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/552.smartweb-webcomponents-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   168291 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/650.smartweb-webcomponents-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       59 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/144.smartweb-webcomponents-compiled.js.LICENSE.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   363927 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/969.smartweb-webcomponents-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      149 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/842.smartweb-webcomponents-compiled.js.LICENSE.txt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    30801 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/510.smartweb-webcomponents-compiled.js
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/assets/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1259 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/assets/layers-2x.8f2c4d11474275fbc1614b9098334eae.png
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1466 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/assets/marker-icon.2b3e1faf89f94a4835397e7a43b4f77d.png
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      696 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/assets/layers.416d91365b44e4b4f4777663e6f009f3.png
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      628 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/assets/next-react-white.819cb069ac8eec300a9db6a7707712d6.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      426 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/assets/search.57bdbf5b191499cd77514097d1c4972c.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      433 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/assets/oeil-big.f32cd1df1274a9593de0c4bd8e344216.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      336 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/assets/pin-react.fda934b5daf26dd4da2a71a7e7e44431.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      628 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/assets/next-react.17bc43ff4a6a86f4520f5782f6a89a72.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      348 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/assets/location-bla.1423bcce16ddcb21141430cac1428dc1.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9538 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/assets/img-placeholder-bla.a2b8b384c46ce56c99f042dc4625d309.png
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      330 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/assets/pin-react-active.07d154037a15be5525b823fdc626cf29.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2226 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/webpackPlonePlugin.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6853 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/webpack.config.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       92 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/.npmrc
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      621 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/Makefile
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      194 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/babel.config.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      101 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/postcss.config.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      343 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/.eslintrc.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2531 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/package.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       67 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/.prettierrc.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       31 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/README.md
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      263 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/hooks/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1215 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/hooks/useAxios.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      223 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/hooks/useFilterQuery.js
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactContent/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    16563 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactContent/ContactContent.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactList/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1675 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactList/ContactList.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactCard/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2043 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactCard/ContactCard.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8772 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/Events.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/Skeleton/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      656 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/Skeleton/Skeleton.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       95 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/index.js
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactMap/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactMap/ContactMap.scss
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5725 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactMap/ContactMap.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7166 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/Events.scss
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/Filters/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6272 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/Filters/Filter.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/ContactResult/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1853 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/ContactResult/ContactResult.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/Skeleton/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      656 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/Skeleton/Skeleton.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       95 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/index.js
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/NewsResult/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2502 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/NewsResult/NewsResult.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/WebResult/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1831 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/WebResult/WebResult.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2570 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/Search.scss
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/EventsResult/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2475 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/EventsResult/EventsResult.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2271 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/Search.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/Filters/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6510 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/Filters/Filter.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactContent/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    16354 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactContent/ContactContent.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4968 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Annuaire.scss
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactList/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1678 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactList/ContactList.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactCard/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3962 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactCard/ContactCard.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8751 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Annuaire.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Skeleton/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      656 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Skeleton/Skeleton.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      217 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Skeleton/LoaderCss.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       97 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/index.js
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactMap/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       73 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactMap/ContactMap.scss
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5770 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactMap/ContactMap.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Filters/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7637 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Filters/Filter.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactContent/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    12558 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactContent/ContactContent.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactList/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1493 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactList/ContactList.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactCard/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3039 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactCard/ContactCard.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3293 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/News.scss
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6840 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/News.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/Skeleton/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      656 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/Skeleton/Skeleton.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       93 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/index.js
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactMap/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       42 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactMap/ContactMap.scss
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4216 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactMap/ContactMap.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/Filters/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6249 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/Filters/Filter.jsx
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/assets/
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      426 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/assets/search.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      628 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/assets/next-react-white.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      336 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/assets/pin-react.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      799 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/assets/facebook-news.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      628 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/assets/next-react.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      884 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/assets/pin-active.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      453 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/assets/skeleton.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      348 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/assets/location-bla.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      890 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/assets/pin.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      369 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/assets/location-active-bla.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      433 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/assets/oeil-big.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)     9538 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/assets/img-placeholder-bla.png
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      478 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/assets/close.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      330 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/assets/pin-react-active.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      757 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/index.jsx
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4681 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/index.scss
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/utils/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      244 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/utils/url.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2694 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/utils/translation.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      858 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/interfaces.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/behaviors/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1865 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/behaviors/minisite.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1063 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/behaviors/quickaccess.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/behaviors/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1707 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/behaviors/subsite.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      760 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/behaviors/listing.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1459 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/behaviors/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5080 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/vocabularies.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      879 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/setuphandlers.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    10699 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_page.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2403 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2655 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_section_sendinblue.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4632 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_text.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7215 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_portal_page.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7787 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_banner.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3505 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_section_news.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4997 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_local_roles.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4921 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_cirkwiview.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4274 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_instance_behaviors.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2388 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_toolbar.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    14084 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_vocabularies.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2425 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_logo.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2194 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_rest_directory.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      369 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_search_one_news_entity.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      921 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_contacts_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4820 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_contact_empty_schedule_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3109 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_contact_images_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    24753 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/plone.png
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      150 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/cirkwi_bad_widget_mock.html
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      441 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_events_entities_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2346 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_rest_specific_events.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      783 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_news_newsfolder_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      749 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_directory_entities_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      726 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_news_entities_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      168 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_no_newsfolder_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2882 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_rest_specific_news.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      359 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_auth_sources_news_entity.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      127 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_no_contact_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      363 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_auth_sources_events_entity.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      390 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_events_types_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3974 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_rest_news.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      205 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_used_iam_vocabularies_jobseeker_tourist.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3823 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/plone.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3217 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_procedures_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    11488 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_contact_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      156 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_contact_no_image_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4399 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_rest_events.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3454 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_contact_category_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      369 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_auth_sources_directory_entity.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      769 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_events_agendas_raw_mock.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   333252 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/cirkwi_good_widget_mock.html
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3030 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_social.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    12782 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_folder.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2374 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2182 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_search.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    10784 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_indexes.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    12109 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_default_pages.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6799 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_navigation.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3193 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_section_events.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5940 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_herobanner.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/robot/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2548 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/robot/test_ct_page.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2003 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/robot/test_example.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2596 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/robot/test_ct_folder.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2712 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/robot/test_ct_procedure.robot
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5950 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_behaviors.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6474 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_procedure.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    20188 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_section_contact.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5120 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_faceted.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    22076 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_sections.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2779 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_icons.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2012 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_categories.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1161 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_chatbot.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    10950 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_footer.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    16632 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_minisite.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2092 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_setup.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5232 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_cropping.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9016 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_subsite.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    13823 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_rest.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      926 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_robot.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/faceted/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      395 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/faceted/layout.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      295 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/faceted/menu.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/faceted/config/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2906 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/faceted/config/collection.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/faceted/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      826 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/faceted/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/icons/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/icons/basic/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    17858 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/icons/basic/registry.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/uninstall/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      128 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/uninstall/browserlayer.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/testing/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      706 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/testing/registry.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/testing/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      215 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/testing/types/Document.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      468 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/testing/types/Collection.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      213 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/testing/types/Folder.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      163 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/testing/types.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      227 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/testing/metadata.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/taxonomies/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      320 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/taxonomies/procedure_category.cfg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2059 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/taxonomies/page_category.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3436 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/taxonomies/procedure_category.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      310 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/taxonomies/page_category.cfg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5877 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/actions.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      864 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/catalog.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1010 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/workflows.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1533 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionFiles.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2419 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Procedure.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1284 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionText.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1210 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionVideo.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1185 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionMap.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1508 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.DirectoryView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1229 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionHTML.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1457 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionCollection.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1476 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.NewsView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1493 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.EventsView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2422 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Page.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1474 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.CirkwiView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1185 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSendinblue.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1730 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Footer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1170 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSlide.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1500 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSelections.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2460 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Folder.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1177 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionContact.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1589 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionLinks.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2598 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.PortalPage.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1478 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionEvents.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1172 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionPostit.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1402 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.BlockLink.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1392 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionGallery.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1472 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionNews.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1604 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.HeroBanner.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1958 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      183 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/repositorytool.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      400 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/controlpanel.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1143 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/metadata.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2510 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/rolemap.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      179 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/browserlayer.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      253 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/registry/smartweb.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1251 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/registry/geolocation.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2562 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/registry/bundles.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2384 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/registry/plone.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/last_compilation/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      852 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/last_compilation/registry.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      821 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/subscribers.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      968 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/indexers.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1737 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1345 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/view_section.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4817 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/views.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      961 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/subscriber.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/footer/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1374 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/footer/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/footer/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/footer/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      464 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/pages.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/page/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      465 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/page/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/page/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/page/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/cirkwi/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      664 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/cirkwi/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/cirkwi/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      392 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/cirkwi/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      378 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/cirkwi/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      482 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/cirkwi/view.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/procedure/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1297 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/procedure/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1291 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/procedure/utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/procedure/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      356 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/procedure/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      408 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/procedure/view.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/herobanner/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1077 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/herobanner/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/herobanner/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       70 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/herobanner/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2983 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/view.pt
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/portal_page/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      336 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/portal_page/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/portal_page/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      352 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/portal_page/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      147 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/portal_page/view.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2252 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/folder/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3348 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/folder/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5570 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/folder/views.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      342 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/folder/element_view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1743 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/folder/macros.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      920 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/folder/summary_view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1194 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/folder/block_view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/folder/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2961 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/folder/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/slide/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2181 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/slide/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/slide/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2440 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/slide/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      417 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/slide/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      784 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/slide/view.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1989 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/views.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      642 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/subscriber.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/video/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      978 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/video/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      342 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/video/views.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/video/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1105 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/video/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      418 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/video/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/postit/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2239 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/postit/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/postit/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      504 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/postit/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      936 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/postit/view.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/html/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1352 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/html/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/html/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1140 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/html/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      413 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/html/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/files/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      868 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/files/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/files/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      501 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/files/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1196 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/files/view.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/common_templates/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     6141 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/common_templates/table.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5132 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/common_templates/carousel.pt
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/text/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1564 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/text/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      372 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/text/views.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/text/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1576 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/text/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1712 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/text/forms.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1423 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/text/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/events/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2911 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/events/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1522 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/events/macros.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/events/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1117 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/events/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3874 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/events/view.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4293 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/macros.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2486 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/base.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/gallery/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      784 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/gallery/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      415 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/gallery/views.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/gallery/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2150 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/gallery/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      424 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/gallery/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/collection/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2376 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/collection/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1246 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/collection/views.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/collection/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      920 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/collection/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/contact/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2431 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/contact/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/contact/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     9530 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/contact/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1387 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/contact/forms.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1281 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/contact/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    11974 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/contact/view.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/links/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1051 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/links/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/links/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      918 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/links/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1285 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/links/view.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/selections/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1372 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/selections/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/selections/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      949 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/selections/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1420 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/selections/view.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/news/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2908 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/news/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/news/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      880 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/news/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3440 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/news/view.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/map/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      372 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/map/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      614 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/map/views.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/map/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1278 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/map/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      412 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/map/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/sendinblue/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1088 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/sendinblue/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1731 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/sendinblue/views.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/sendinblue/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1180 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/sendinblue/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      433 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/sendinblue/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2200 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/blocks/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      330 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/blocks/subscriber.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/blocks/link/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1407 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/blocks/link/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/blocks/link/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      703 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/blocks/link/icons_input.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      479 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/blocks/link/fields.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      552 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/blocks/link/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/blocks/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      732 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/blocks/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1940 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      735 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/cropping.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/directory/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      923 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/directory/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1979 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/directory/endpoint.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/directory/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      616 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/directory/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1035 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/directory/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      302 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/directory/view.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/search/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     8383 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/search/endpoint.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/search/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      951 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/search/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/events/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1100 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/events/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3721 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/events/endpoint.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/events/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      617 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/events/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1017 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/events/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      293 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/events/view.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1411 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/base.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/__init__.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/news/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      753 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/news/content.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1858 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/news/endpoint.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/news/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      629 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/news/view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1005 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/news/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      287 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/news/view.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      200 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      567 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/view.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      665 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4483 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/utils.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      531 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/default_page_warning.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      872 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/footer.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      503 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/subsite_logo.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      602 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/procedure.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      872 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/messages.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3216 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/footer.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      577 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/header_actions.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      199 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/social.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3385 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/toolbar.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      137 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/subsite_header_viewlet.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      129 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/offcanvas.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      533 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/offcanvas.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      129 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/header_actions_viewlet.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      611 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/chatbot.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      308 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/menu.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      103 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/category.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2213 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/logo.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     7284 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/navigation.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      688 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/herobanner.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      648 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/minisite.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2229 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/banner.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      403 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/searchbox.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      318 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/lead_image.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      661 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/actions.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1277 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/banner.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1359 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/herobanner.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      633 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/procedure.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      367 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/header.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      163 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/subsite_navigation.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      329 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/chatbot.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      370 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/minisite_link.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4218 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/subsite.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      308 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/category.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      738 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/logo.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      137 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/header_top_viewlet.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    11589 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    19917 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/vocabularies.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      337 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/config.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1611 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/permissions.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      173 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/workflows.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      311 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/imio.smartweb.Procedure.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      306 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/imio.smartweb.Page.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      312 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/imio.smartweb.PortalPage.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1157 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/imio.smartweb.SectionPostit.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      180 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1021_to_1022/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      298 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1021_to_1022/rolemap.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1021_to_1022/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      457 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1021_to_1022/registry/hero-banner.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1022_to_1023/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1022_to_1023/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      838 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1022_to_1023/registry/icons.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1474 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/types/imio.smartweb.CirkwiView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      305 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/types/imio.smartweb.Folder.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      177 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/types.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      298 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/rolemap.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      403 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/registry/plone.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1029_to_1030/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      463 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1029_to_1030/actions.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      256 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1029_to_1030/rolemap.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1020_to_1021/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1020_to_1021/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      244 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1020_to_1021/types/imio.smartweb.SectionHTML.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      538 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1020_to_1021/rolemap.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      321 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.Procedure.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      325 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.DirectoryView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      320 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.NewsView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      322 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.EventsView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      316 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.Page.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      318 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.Folder.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      322 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1034_to_1035/types/imio.smartweb.PortalPage.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1025_to_1026/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1025_to_1026/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      249 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1025_to_1026/registry/propose-urls.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      249 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionFiles.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      256 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.Procedure.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      248 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionText.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      249 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionVideo.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      241 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionMap.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      252 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.DirectoryView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      249 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionHTML.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      255 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionCollection.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      245 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.NewsView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      252 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.EventsView.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      244 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.Page.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      249 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionSendinblue.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      250 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.Footer.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      246 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionSlide.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      254 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionSelections.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      241 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.Folder.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      253 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionContact.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      250 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionLinks.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      256 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.PortalPage.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      246 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionEvents.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      249 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionPostit.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      257 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.BlockLink.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      248 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionGallery.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      248 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.SectionNews.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      247 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1033_to_1034/types/imio.smartweb.HeroBanner.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1027_to_1028/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1027_to_1028/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      318 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1027_to_1028/registry/open-external-link-in-new-tab.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1036_to_1037/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      440 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1036_to_1037/actions.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      275 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1036_to_1037/rolemap.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1031_to_1032/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1031_to_1032/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      562 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1031_to_1032/registry/spotlight.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1015_to_1016/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1015_to_1016/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      481 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1015_to_1016/registry/e-guichet-icon.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1016_to_1017/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1016_to_1017/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      478 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1016_to_1017/registry/shop-icon.xml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1030_to_1031/
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1030_to_1031/registry/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1425 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1030_to_1031/registry/resources.xml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     5245 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/upgrades.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    17069 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       24 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      172 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/testing.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2066 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/layout.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/banner/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      947 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/banner/settings.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/banner/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      389 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/banner/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/templates/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2808 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/templates/link_input.pt
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/search/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2369 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/search/search.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      450 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/search/search.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/search/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      423 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/search/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1582 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/gallery_view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1414 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/views.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4303 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/map.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1382 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/map.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2951 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/macros.pt
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/widgets/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      221 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/widgets/select.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/widgets/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2459 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/widgets/select.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      449 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/widgets/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1667 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/summary_view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1723 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/block_view.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2806 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4648 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/controlpanel.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)   135631 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/swiper-bundle.min.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      737 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/smartweb-edit-compiled.css
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    15564 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/swiper-bundle.min.css
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      414 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/action-voir-plan.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      483 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/action-nous-contacter.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      873 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/action-e-guichet.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1355 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/action-engagement.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      561 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-mobilite.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      826 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/reseausocial-vimeo.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      313 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-avis-et-enquetes.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      294 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/organisation-academie-musique.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      284 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-exposition.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      350 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/vue-actualites.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1039 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/reseausocial-twitter.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      625 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/organisation-ecole-des-arts.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      302 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-mon-dossier.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      721 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/reseausocial-facebook.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1787 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-commerce.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      514 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-sport-trophee.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      522 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/organisation-bibliotheque.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      339 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/vue-agenda.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      662 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-primes.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      451 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/organisation-police.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      458 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-cinema.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)     2086 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/reseausocial-facebook-pouce.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      787 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/action-signaler-un-probleme.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)     1999 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/reseausocial-instagram.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      614 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/organisation-mobilite.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      453 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-infos-travaux.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      692 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-mandataires.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      367 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-culture.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      673 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-enseignement.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      307 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/action-organiser-un-evenement.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      419 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-parcs-et-jardins.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      302 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/organisation-ecole.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      252 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-environnement-gestion-des-dechets.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      925 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-sport-velo.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      739 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/organisation-centre-sportif.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      318 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-parc-de-stationnement.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)     1011 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-enfance.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      590 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/reseausocial-youtube.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      397 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-sport-courir.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      390 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-tourisme.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      274 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/action-email.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      409 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/action-nous-rejoindre.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      426 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-demarches.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      508 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-concert.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      259 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-horaires.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      313 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-associations.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      713 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-theatre.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      497 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/vue-annuaire.svg
+-rwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)      879 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/organisation-cpas.svg
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)    19615 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/spotlight-bundle.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1030 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/webpack.config.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      350 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/Makefile
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2608 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/smartweb-view-compiled.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2702 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/smartweb-view-compiled.css
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      695 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/package.json
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      354 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/smartweb-edit-compiled.js
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/src/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     4211 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/src/view.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      918 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/src/edit.less
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2843 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/src/view.less
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      581 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/src/edit.js
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/.gitkeep
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/footer/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2492 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/footer/settings.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/footer/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      388 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/footer/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/instancebehaviors/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3052 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/instancebehaviors/form.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      742 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/instancebehaviors/utils.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/instancebehaviors/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      632 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/instancebehaviors/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/overrides/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      978 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/overrides/plone.app.layout.viewlets.sections.pt
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/overrides/.gitkeep
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2065 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/icons.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3058 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/utils.py
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/subsite/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1601 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/subsite/settings.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/subsite/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      414 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/subsite/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/minisite/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2766 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/minisite/settings.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/minisite/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      417 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/minisite/configure.zcml
+drwxrwxr-x   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/herobanner/
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2884 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/herobanner/settings.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/herobanner/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)      400 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/herobanner/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)        0 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1089 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/forms.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     2775 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     3887 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/indexers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1818 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/subscribers.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)     1429 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/core/configure.zcml
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/smartweb/__init__.py
+-rw-rw-r--   0 cboulanger  (1000) cboulanger  (1000)       80 2023-03-17 15:05:01.000000 imio.smartweb.core-1.1.9/src/imio/__init__.py
```

### Comparing `imio.smartweb.core-1.1.8/docs/conf.py` & `imio.smartweb.core-1.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/DEVELOP.rst` & `imio.smartweb.core-1.1.9/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/PKG-INFO` & `imio.smartweb.core-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.smartweb.core
-Version: 1.1.8
+Version: 1.1.9
 Summary: Core product for iMio websites
 Home-page: https://github.com/imio/imio.smartweb.core
 Author: Christophe Boulanger
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: Source, https://github.com/imio/imio.smartweb.core
 Project-URL: Tracker, https://github.com/imio/imio.smartweb.core/issues
@@ -138,14 +138,21 @@
         - Thomas Lambert, thomas.lambert@imio.be
         
         
         Changelog
         =========
         
         
+        1.1.9 (2023-03-17)
+        ------------------
+        
+        - WEB-3898 : Prevent error (error while rendering imio.smartweb.banner) if a content has his id = "banner"
+          [boulch]
+        
+        
         1.1.8 (2023-03-15)
         ------------------
         
         - WEB-3888 : We overrided link_input template widget to allow any link format in external tab (without browser blocking)
           [boulch]
         
         - WEB-3769 : Get fullsize picture if scale is not present (ex: picture too small)
```

### Comparing `imio.smartweb.core-1.1.8/README.rst` & `imio.smartweb.core-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/LICENSE.GPL` & `imio.smartweb.core-1.1.9/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/CHANGES.rst` & `imio.smartweb.core-1.1.9/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+1.1.9 (2023-03-17)
+------------------
+
+- WEB-3898 : Prevent error (error while rendering imio.smartweb.banner) if a content has his id = "banner"
+  [boulch]
+
+
 1.1.8 (2023-03-15)
 ------------------
 
 - WEB-3888 : We overrided link_input template widget to allow any link format in external tab (without browser blocking)
   [boulch]
 
 - WEB-3769 : Get fullsize picture if scale is not present (ex: picture too small)
```

### Comparing `imio.smartweb.core-1.1.8/setup.py` & `imio.smartweb.core-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="imio.smartweb.core",
-    version="1.1.8",
+    version="1.1.9",
     description="Core product for iMio websites",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `imio.smartweb.core-1.1.8/LICENSE.rst` & `imio.smartweb.core-1.1.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/setup.cfg` & `imio.smartweb.core-1.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio.smartweb.core.egg-info/PKG-INFO` & `imio.smartweb.core-1.1.9/src/imio.smartweb.core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imio.smartweb.core
-Version: 1.1.8
+Version: 1.1.9
 Summary: Core product for iMio websites
 Home-page: https://github.com/imio/imio.smartweb.core
 Author: Christophe Boulanger
 Author-email: christophe.boulanger@imio.be
 License: GPL version 2
 Project-URL: Source, https://github.com/imio/imio.smartweb.core
 Project-URL: Tracker, https://github.com/imio/imio.smartweb.core/issues
@@ -138,14 +138,21 @@
         - Thomas Lambert, thomas.lambert@imio.be
         
         
         Changelog
         =========
         
         
+        1.1.9 (2023-03-17)
+        ------------------
+        
+        - WEB-3898 : Prevent error (error while rendering imio.smartweb.banner) if a content has his id = "banner"
+          [boulch]
+        
+        
         1.1.8 (2023-03-15)
         ------------------
         
         - WEB-3888 : We overrided link_input template widget to allow any link format in external tab (without browser blocking)
           [boulch]
         
         - WEB-3769 : Get fullsize picture if scale is not present (ex: picture too small)
```

### Comparing `imio.smartweb.core-1.1.8/src/imio.smartweb.core.egg-info/requires.txt` & `imio.smartweb.core-1.1.9/src/imio.smartweb.core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio.smartweb.core.egg-info/SOURCES.txt` & `imio.smartweb.core-1.1.9/src/imio.smartweb.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/testing.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/testing.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/css/323.smartweb-webcomponents-compiled.css` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/css/323.smartweb-webcomponents-compiled.css`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/css/195.smartweb-webcomponents-compiled.css` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/css/195.smartweb-webcomponents-compiled.css`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/css/552.smartweb-webcomponents-compiled.css` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/css/552.smartweb-webcomponents-compiled.css`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/css/510.smartweb-webcomponents-compiled.css` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/css/510.smartweb-webcomponents-compiled.css`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/css/smartweb-webcomponents-compiled.css` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/css/smartweb-webcomponents-compiled.css`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/9.smartweb-webcomponents-compiled.js` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/9.smartweb-webcomponents-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/195.smartweb-webcomponents-compiled.js` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/195.smartweb-webcomponents-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/842.smartweb-webcomponents-compiled.js` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/842.smartweb-webcomponents-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/323.smartweb-webcomponents-compiled.js` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/323.smartweb-webcomponents-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/smartweb-webcomponents-compiled.js.LICENSE.txt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/smartweb-webcomponents-compiled.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/969.smartweb-webcomponents-compiled.js.LICENSE.txt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/969.smartweb-webcomponents-compiled.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/smartweb-webcomponents-compiled.js` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/smartweb-webcomponents-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/144.smartweb-webcomponents-compiled.js` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/144.smartweb-webcomponents-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/462.smartweb-webcomponents-compiled.js` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/462.smartweb-webcomponents-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/552.smartweb-webcomponents-compiled.js` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/552.smartweb-webcomponents-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/650.smartweb-webcomponents-compiled.js` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/650.smartweb-webcomponents-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/969.smartweb-webcomponents-compiled.js` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/969.smartweb-webcomponents-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/js/510.smartweb-webcomponents-compiled.js` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/js/510.smartweb-webcomponents-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/assets/layers-2x.8f2c4d11474275fbc1614b9098334eae.png` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/assets/layers-2x.8f2c4d11474275fbc1614b9098334eae.png`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/assets/marker-icon.2b3e1faf89f94a4835397e7a43b4f77d.png` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/assets/marker-icon.2b3e1faf89f94a4835397e7a43b4f77d.png`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/assets/layers.416d91365b44e4b4f4777663e6f009f3.png` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/assets/layers.416d91365b44e4b4f4777663e6f009f3.png`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/assets/next-react-white.819cb069ac8eec300a9db6a7707712d6.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/assets/next-react-white.819cb069ac8eec300a9db6a7707712d6.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/assets/next-react.17bc43ff4a6a86f4520f5782f6a89a72.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/assets/next-react.17bc43ff4a6a86f4520f5782f6a89a72.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/build/assets/img-placeholder-bla.a2b8b384c46ce56c99f042dc4625d309.png` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/build/assets/img-placeholder-bla.a2b8b384c46ce56c99f042dc4625d309.png`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/webpackPlonePlugin.js` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/webpackPlonePlugin.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/webpack.config.js` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/webpack.config.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/Makefile` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/Makefile`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/package.json` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/package.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/hooks/useAxios.js` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/hooks/useAxios.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactContent/ContactContent.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactContent/ContactContent.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactList/ContactList.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactList/ContactList.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactCard/ContactCard.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactCard/ContactCard.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/Events.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/Events.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/Skeleton/Skeleton.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/Skeleton/Skeleton.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/ContactMap/ContactMap.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/ContactMap/ContactMap.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/Events.scss` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/Events.scss`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Events/Filters/Filter.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Events/Filters/Filter.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/ContactResult/ContactResult.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/ContactResult/ContactResult.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/Skeleton/Skeleton.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/Skeleton/Skeleton.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/NewsResult/NewsResult.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/NewsResult/NewsResult.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/WebResult/WebResult.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/WebResult/WebResult.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/Search.scss` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/Search.scss`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/EventsResult/EventsResult.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/EventsResult/EventsResult.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/Search.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/Search.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Search/Filters/Filter.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Search/Filters/Filter.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactContent/ContactContent.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactContent/ContactContent.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Annuaire.scss` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Annuaire.scss`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactList/ContactList.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactList/ContactList.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactCard/ContactCard.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactCard/ContactCard.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Annuaire.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Annuaire.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Skeleton/Skeleton.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Skeleton/Skeleton.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactMap/ContactMap.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/ContactMap/ContactMap.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Filters/Filter.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/Annuaire/Filters/Filter.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactContent/ContactContent.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactContent/ContactContent.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactList/ContactList.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactList/ContactList.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactCard/ContactCard.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactCard/ContactCard.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/News.scss` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/News.scss`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/News.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/News.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/Skeleton/Skeleton.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/Skeleton/Skeleton.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/ContactMap/ContactMap.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/ContactMap/ContactMap.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/components/News/Filters/Filter.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/components/News/Filters/Filter.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/assets/next-react-white.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/assets/next-react-white.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/assets/facebook-news.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/assets/facebook-news.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/assets/next-react.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/assets/next-react.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/assets/pin-active.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/assets/pin-active.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/assets/pin.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/assets/pin.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/assets/img-placeholder-bla.png` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/assets/img-placeholder-bla.png`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/index.jsx` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/index.jsx`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/index.scss` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/index.scss`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/webcomponents/src/utils/translation.js` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/webcomponents/src/utils/translation.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/interfaces.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/interfaces.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/behaviors/minisite.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/behaviors/minisite.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/behaviors/quickaccess.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/behaviors/quickaccess.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/behaviors/subsite.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/behaviors/subsite.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/behaviors/listing.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/behaviors/listing.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/behaviors/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/vocabularies.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/vocabularies.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/setuphandlers.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_page.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_utils.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_section_sendinblue.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_section_sendinblue.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_text.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_portal_page.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_portal_page.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_banner.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_banner.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_section_news.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_section_news.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_local_roles.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_local_roles.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_cirkwiview.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_cirkwiview.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_instance_behaviors.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_instance_behaviors.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_toolbar.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_toolbar.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_vocabularies.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_logo.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_logo.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_rest_directory.json` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_rest_directory.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_contacts_raw_mock.json` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_contacts_raw_mock.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_contact_empty_schedule_raw_mock.json` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_contact_empty_schedule_raw_mock.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_contact_images_raw_mock.json` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_contact_images_raw_mock.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/plone.png` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/plone.png`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_rest_specific_events.json` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_rest_specific_events.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_news_newsfolder_raw_mock.json` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_news_newsfolder_raw_mock.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_directory_entities_raw_mock.json` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_directory_entities_raw_mock.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_news_entities_raw_mock.json` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_news_entities_raw_mock.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_rest_specific_news.json` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_rest_specific_news.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_rest_news.json` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_rest_news.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/plone.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/plone.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_procedures_raw_mock.json` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_procedures_raw_mock.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_contact_raw_mock.json` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_contact_raw_mock.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_rest_events.json` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_rest_events.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_contact_category_raw_mock.json` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_contact_category_raw_mock.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/json_events_agendas_raw_mock.json` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/json_events_agendas_raw_mock.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/resources/cirkwi_good_widget_mock.html` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/resources/cirkwi_good_widget_mock.html`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_social.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_social.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_folder.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_folder.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/utils.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/utils.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_search.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_indexes.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_default_pages.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_default_pages.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_navigation.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_navigation.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_section_events.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_section_events.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_herobanner.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_herobanner.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/robot/test_ct_page.robot` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/robot/test_ct_page.robot`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/robot/test_example.robot` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/robot/test_ct_folder.robot` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/robot/test_ct_folder.robot`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/robot/test_ct_procedure.robot` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/robot/test_ct_procedure.robot`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_behaviors.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_behaviors.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_procedure.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_procedure.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_section_contact.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_section_contact.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_faceted.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_faceted.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_sections.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_sections.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_icons.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_icons.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_categories.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_categories.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_chatbot.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_chatbot.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_footer.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_footer.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_minisite.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_minisite.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_setup.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_cropping.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_cropping.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_subsite.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_subsite.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_rest.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/tests/test_robot.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/faceted/config/collection.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/faceted/config/collection.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/faceted/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/faceted/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/icons/basic/registry.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/icons/basic/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/testing/registry.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/testing/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/taxonomies/page_category.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/taxonomies/page_category.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/taxonomies/procedure_category.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/taxonomies/procedure_category.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/actions.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/catalog.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/workflows.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionFiles.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionFiles.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Procedure.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Procedure.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionText.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionText.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionVideo.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionVideo.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionMap.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionMap.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.DirectoryView.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.DirectoryView.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionHTML.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionHTML.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionCollection.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionCollection.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.NewsView.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.NewsView.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.EventsView.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.EventsView.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Page.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Page.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.CirkwiView.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.CirkwiView.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSendinblue.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSendinblue.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Footer.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Footer.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSlide.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSlide.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSelections.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionSelections.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Folder.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.Folder.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionContact.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionContact.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionLinks.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionLinks.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.PortalPage.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.PortalPage.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionEvents.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionEvents.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionPostit.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionPostit.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.BlockLink.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.BlockLink.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionGallery.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionGallery.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionNews.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.SectionNews.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types/imio.smartweb.HeroBanner.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types/imio.smartweb.HeroBanner.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/types.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/types.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/metadata.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/metadata.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/rolemap.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/registry/geolocation.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/registry/geolocation.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/registry/bundles.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/registry/bundles.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/default/registry/plone.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/default/registry/plone.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles/last_compilation/registry.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles/last_compilation/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/subscribers.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/subscribers.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/indexers.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/indexers.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/profiles.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/profiles.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/view_section.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/view_section.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/views.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/views.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/subscriber.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/subscriber.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/footer/content.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/footer/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/cirkwi/content.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/cirkwi/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/procedure/content.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/procedure/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/procedure/utils.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/procedure/utils.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/herobanner/content.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/herobanner/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/view.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/pages/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/pages/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/folder/content.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/folder/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/folder/views.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/folder/views.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/folder/macros.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/folder/macros.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/folder/summary_view.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/folder/summary_view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/folder/block_view.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/folder/block_view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/folder/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/folder/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/slide/content.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/slide/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/slide/view.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/slide/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/slide/view.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/slide/view.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/views.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/views.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/subscriber.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/subscriber.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/video/content.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/video/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/video/view.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/video/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/postit/content.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/postit/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/postit/view.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/postit/view.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/html/content.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/html/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/html/view.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/html/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/files/content.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/files/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/files/view.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/files/view.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/common_templates/table.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/common_templates/table.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/common_templates/carousel.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/common_templates/carousel.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/text/content.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/text/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/text/view.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/text/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/text/forms.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/text/forms.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/text/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/text/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/events/content.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/events/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/events/macros.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/events/macros.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/events/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/events/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/events/view.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/events/view.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/macros.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/macros.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/base.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/base.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/gallery/content.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/gallery/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/gallery/view.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/gallery/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/collection/content.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/collection/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/collection/views.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/collection/views.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/collection/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/collection/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/contact/content.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/contact/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/contact/view.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/contact/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/contact/forms.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/contact/forms.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/contact/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/contact/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/contact/view.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/contact/view.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/links/content.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/links/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/links/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/links/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/links/view.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/links/view.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/selections/content.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/selections/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/selections/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/selections/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/selections/view.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/selections/view.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/news/content.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/news/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/news/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/news/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/news/view.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/news/view.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/map/views.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/map/views.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/map/view.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/map/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/sendinblue/content.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/sendinblue/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/sendinblue/views.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/sendinblue/views.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/sendinblue/view.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/sendinblue/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/sections/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/sections/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/blocks/link/content.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/blocks/link/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/blocks/link/icons_input.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/blocks/link/icons_input.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/blocks/link/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/blocks/link/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/blocks/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/blocks/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/__init__.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/cropping.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/cropping.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/directory/content.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/directory/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/directory/endpoint.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/directory/endpoint.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/directory/view.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/directory/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/directory/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/directory/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/search/endpoint.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/search/endpoint.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/search/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/search/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/events/content.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/events/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/events/endpoint.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/events/endpoint.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/events/view.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/events/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/events/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/events/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/base.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/base.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/news/content.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/news/content.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/news/endpoint.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/news/endpoint.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/news/view.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/news/view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/news/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/news/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/rest/view.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/rest/view.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/contents/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/contents/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/utils.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/utils.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/default_page_warning.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/default_page_warning.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/footer.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/footer.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/procedure.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/procedure.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/messages.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/messages.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/footer.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/footer.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/header_actions.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/header_actions.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/toolbar.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/toolbar.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/offcanvas.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/offcanvas.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/chatbot.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/chatbot.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/logo.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/logo.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/navigation.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/navigation.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/herobanner.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/herobanner.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/minisite.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/minisite.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/banner.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/banner.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from imio.smartweb.core.browser.banner.settings import ILocallyHiddenBanner
 from plone import api
 from plone.app.layout.navigation.interfaces import INavigationRoot
 from plone.app.layout.viewlets import common
+from plone.namedfile.file import NamedBlobImage
 from Products.CMFPlone.utils import base_hasattr
 from zope.component import queryMultiAdapter
 
 
 class BannerViewlet(common.ViewletBase):
     _banner_item = None
     _banner_is_hidden = False
@@ -28,15 +29,19 @@
     @property
     def banner_item(self):
         if self._banner_item is not None:
             return self._banner_item
         for item in self.context.aq_chain:
             if ILocallyHiddenBanner.providedBy(item):
                 self._banner_is_hidden = True
-            if base_hasattr(item, "banner") and item.banner is not None:
+            if (
+                base_hasattr(item, "banner")
+                and item.banner is not None
+                and isinstance(item.banner, NamedBlobImage)
+            ):
                 self._banner_item = item
                 return item
             if INavigationRoot.providedBy(item):
                 return
 
     @property
     def is_banner_hidden(self):
```

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/actions.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/actions.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/banner.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/banner.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/herobanner.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/herobanner.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/procedure.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/procedure.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/subsite.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/subsite.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/logo.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/logo.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/viewlets/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/viewlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/vocabularies.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/permissions.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/permissions.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/imio.smartweb.SectionPostit.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1023_to_1024/types/imio.smartweb.SectionPostit.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1022_to_1023/registry/icons.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1022_to_1023/registry/icons.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/types/imio.smartweb.CirkwiView.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1035_to_1036/types/imio.smartweb.CirkwiView.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1020_to_1021/rolemap.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1020_to_1021/rolemap.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1031_to_1032/registry/spotlight.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1031_to_1032/registry/spotlight.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/profiles/1030_to_1031/registry/resources.xml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/profiles/1030_to_1031/registry/resources.xml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/upgrades.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/upgrades/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/layout.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/layout.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/banner/settings.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/banner/settings.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/templates/link_input.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/templates/link_input.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/search/search.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/search/search.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/gallery_view.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/gallery_view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/views.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/views.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/map.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/map.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/map.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/map.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/macros.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/macros.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/widgets/select.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/widgets/select.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/summary_view.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/summary_view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/block_view.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/block_view.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/faceted/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/faceted/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/controlpanel.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/swiper-bundle.min.js` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/swiper-bundle.min.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/smartweb-edit-compiled.css` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/smartweb-edit-compiled.css`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/swiper-bundle.min.css` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/swiper-bundle.min.css`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/action-e-guichet.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/action-e-guichet.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/action-engagement.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/action-engagement.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-mobilite.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-mobilite.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/reseausocial-vimeo.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/reseausocial-vimeo.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/reseausocial-twitter.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/reseausocial-twitter.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/organisation-ecole-des-arts.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/organisation-ecole-des-arts.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/reseausocial-facebook.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/reseausocial-facebook.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-commerce.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-commerce.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-sport-trophee.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-sport-trophee.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/organisation-bibliotheque.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/organisation-bibliotheque.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-primes.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-primes.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/reseausocial-facebook-pouce.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/reseausocial-facebook-pouce.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/action-signaler-un-probleme.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/action-signaler-un-probleme.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/reseausocial-instagram.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/reseausocial-instagram.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/organisation-mobilite.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/organisation-mobilite.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-mandataires.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-mandataires.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-enseignement.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-enseignement.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-sport-velo.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-sport-velo.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/organisation-centre-sportif.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/organisation-centre-sportif.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-enfance.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-enfance.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/reseausocial-youtube.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/reseausocial-youtube.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/categorie-theatre.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/categorie-theatre.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/icons/organisation-cpas.svg` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/icons/organisation-cpas.svg`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/spotlight-bundle.js` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/spotlight-bundle.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/webpack.config.js` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/webpack.config.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/smartweb-view-compiled.js` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/smartweb-view-compiled.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/smartweb-view-compiled.css` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/smartweb-view-compiled.css`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/package.json` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/package.json`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/src/view.js` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/src/view.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/src/edit.less` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/src/edit.less`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/src/view.less` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/src/view.less`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/static/src/edit.js` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/static/src/edit.js`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/footer/settings.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/footer/settings.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/instancebehaviors/form.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/instancebehaviors/form.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/instancebehaviors/utils.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/instancebehaviors/utils.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/instancebehaviors/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/instancebehaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/overrides/plone.app.layout.viewlets.sections.pt` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/overrides/plone.app.layout.viewlets.sections.pt`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/icons.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/icons.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/utils.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/utils.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/subsite/settings.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/subsite/settings.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/minisite/settings.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/minisite/settings.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/herobanner/settings.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/herobanner/settings.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/forms.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/forms.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/browser/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/indexers.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/indexers.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/subscribers.py` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/subscribers.py`

 * *Files identical despite different names*

### Comparing `imio.smartweb.core-1.1.8/src/imio/smartweb/core/configure.zcml` & `imio.smartweb.core-1.1.9/src/imio/smartweb/core/configure.zcml`

 * *Files identical despite different names*

