# Comparing `tmp/autora-3.0.0a8.tar.gz` & `tmp/autora-3.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-3.0.0a8.tar", last modified: Thu May  4 16:56:06 2023, max compression
+gzip compressed data, was "autora-3.0.0a9.tar", last modified: Fri May  5 13:20:41 2023, max compression
```

## Comparing `autora-3.0.0a8.tar` & `autora-3.0.0a9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.494232 autora-3.0.0a8/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-04 16:55:38.000000 autora-3.0.0a8/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-04 16:55:38.000000 autora-3.0.0a8/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-04 16:55:38.000000 autora-3.0.0a8/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-04 16:55:38.000000 autora-3.0.0a8/.github/workflows/publish-documentation-gh-pages.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-04 16:55:38.000000 autora-3.0.0a8/.github/workflows/publish-package-anaconda-org.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-04 16:55:38.000000 autora-3.0.0a8/.github/workflows/publish-package-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-04 16:55:38.000000 autora-3.0.0a8/.github/workflows/test-conda-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-04 16:55:38.000000 autora-3.0.0a8/.github/workflows/test-poetry-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-04 16:55:38.000000 autora-3.0.0a8/.github/workflows/test-pre-commit-hooks.yml
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-04 16:55:38.000000 autora-3.0.0a8/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-04 16:55:38.000000 autora-3.0.0a8/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-04 16:55:38.000000 autora-3.0.0a8/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-04 16:55:38.000000 autora-3.0.0a8/.idea/autora.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-04 16:55:38.000000 autora-3.0.0a8/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 16:55:38.000000 autora-3.0.0a8/.idea/encodings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-04 16:55:38.000000 autora-3.0.0a8/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-04 16:55:38.000000 autora-3.0.0a8/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-04 16:55:38.000000 autora-3.0.0a8/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-04 16:55:38.000000 autora-3.0.0a8/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-04 16:55:38.000000 autora-3.0.0a8/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-04 16:55:38.000000 autora-3.0.0a8/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 16:55:38.000000 autora-3.0.0a8/.vscode/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-04 16:55:38.000000 autora-3.0.0a8/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-04 16:55:38.000000 autora-3.0.0a8/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-04 16:55:38.000000 autora-3.0.0a8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-05-04 16:56:06.494232 autora-3.0.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20247 2023-05-04 16:55:38.000000 autora-3.0.0a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.486232 autora-3.0.0a8/conda/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/conda/autora/
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-04 16:55:38.000000 autora-3.0.0a8/conda/autora/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 16:55:38.000000 autora-3.0.0a8/conda/autora/run_test.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/docs/experiment-runner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 16:55:38.000000 autora-3.0.0a8/docs/experiment-runner/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/docs/experimentalists/
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-04 16:55:38.000000 autora-3.0.0a8/docs/experimentalists/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)    31814 2023-05-04 16:55:38.000000 autora-3.0.0a8/docs/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   389908 2023-05-04 16:55:38.000000 autora-3.0.0a8/docs/img/overview.png
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-04 16:55:38.000000 autora-3.0.0a8/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-04 16:55:38.000000 autora-3.0.0a8/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/docs/theorist/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-04 16:55:38.000000 autora-3.0.0a8/docs/theorist/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-04 16:55:38.000000 autora-3.0.0a8/mkdocs/base.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.490232 autora-3.0.0a8/mkdocs/overrides/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-04 16:55:38.000000 autora-3.0.0a8/mkdocs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-04 16:55:38.000000 autora-3.0.0a8/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-04 16:55:38.000000 autora-3.0.0a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 16:56:06.494232 autora-3.0.0a8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.494232 autora-3.0.0a8/src/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-04 16:55:38.000000 autora-3.0.0a8/src/.keep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:56:06.494232 autora-3.0.0a8/src/autora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-05-04 16:56:06.000000 autora-3.0.0a8/src/autora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-04 16:56:06.000000 autora-3.0.0a8/src/autora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:56:06.000000 autora-3.0.0a8/src/autora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-04 16:56:06.000000 autora-3.0.0a8/src/autora.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:56:06.000000 autora-3.0.0a8/src/autora.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.009979 autora-3.0.0a9/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-05 13:20:29.000000 autora-3.0.0a9/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:40.997979 autora-3.0.0a9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-05 13:20:29.000000 autora-3.0.0a9/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-05 13:20:29.000000 autora-3.0.0a9/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:40.997979 autora-3.0.0a9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-05 13:20:29.000000 autora-3.0.0a9/.github/workflows/publish-documentation-gh-pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-05 13:20:29.000000 autora-3.0.0a9/.github/workflows/publish-package-anaconda-org.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-05 13:20:29.000000 autora-3.0.0a9/.github/workflows/publish-package-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-05 13:20:29.000000 autora-3.0.0a9/.github/workflows/test-conda-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-05 13:20:29.000000 autora-3.0.0a9/.github/workflows/test-poetry-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-05 13:20:29.000000 autora-3.0.0a9/.github/workflows/test-pre-commit-hooks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-05 13:20:29.000000 autora-3.0.0a9/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-05 13:20:29.000000 autora-3.0.0a9/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.001979 autora-3.0.0a9/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-05 13:20:29.000000 autora-3.0.0a9/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-05 13:20:29.000000 autora-3.0.0a9/.idea/autora.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.001979 autora-3.0.0a9/.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-05 13:20:29.000000 autora-3.0.0a9/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 13:20:29.000000 autora-3.0.0a9/.idea/encodings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.001979 autora-3.0.0a9/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-05 13:20:29.000000 autora-3.0.0a9/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 13:20:29.000000 autora-3.0.0a9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-05 13:20:29.000000 autora-3.0.0a9/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-05 13:20:29.000000 autora-3.0.0a9/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-05 13:20:29.000000 autora-3.0.0a9/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-05 13:20:29.000000 autora-3.0.0a9/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.001979 autora-3.0.0a9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:29.000000 autora-3.0.0a9/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 13:20:29.000000 autora-3.0.0a9/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-05 13:20:29.000000 autora-3.0.0a9/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-05 13:20:29.000000 autora-3.0.0a9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-05-05 13:20:41.009979 autora-3.0.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20247 2023-05-05 13:20:29.000000 autora-3.0.0a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:40.989979 autora-3.0.0a9/conda/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.001979 autora-3.0.0a9/conda/autora/
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-05 13:20:29.000000 autora-3.0.0a9/conda/autora/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-05 13:20:29.000000 autora-3.0.0a9/conda/autora/run_test.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.001979 autora-3.0.0a9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.001979 autora-3.0.0a9/docs/experiment-runner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:29.000000 autora-3.0.0a9/docs/experiment-runner/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.001979 autora-3.0.0a9/docs/experimentalists/
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-05 13:20:29.000000 autora-3.0.0a9/docs/experimentalists/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.005979 autora-3.0.0a9/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    31814 2023-05-05 13:20:29.000000 autora-3.0.0a9/docs/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   389908 2023-05-05 13:20:29.000000 autora-3.0.0a9/docs/img/overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-05 13:20:29.000000 autora-3.0.0a9/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.005979 autora-3.0.0a9/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-05 13:20:29.000000 autora-3.0.0a9/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.005979 autora-3.0.0a9/docs/theorist/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-05 13:20:29.000000 autora-3.0.0a9/docs/theorist/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.005979 autora-3.0.0a9/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-05 13:20:29.000000 autora-3.0.0a9/mkdocs/base.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.005979 autora-3.0.0a9/mkdocs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-05 13:20:29.000000 autora-3.0.0a9/mkdocs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-05 13:20:29.000000 autora-3.0.0a9/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-05 13:20:29.000000 autora-3.0.0a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:20:41.009979 autora-3.0.0a9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.005979 autora-3.0.0a9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-05 13:20:29.000000 autora-3.0.0a9/src/.keep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:20:41.009979 autora-3.0.0a9/src/autora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-05-05 13:20:40.000000 autora-3.0.0a9/src/autora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-05 13:20:40.000000 autora-3.0.0a9/src/autora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:20:40.000000 autora-3.0.0a9/src/autora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-05 13:20:40.000000 autora-3.0.0a9/src/autora.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:20:40.000000 autora-3.0.0a9/src/autora.egg-info/top_level.txt
```

### Comparing `autora-3.0.0a8/.github/pull_request_template.md` & `autora-3.0.0a9/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a8/.github/workflows/publish-documentation-gh-pages.yml` & `autora-3.0.0a9/.github/workflows/publish-documentation-gh-pages.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a8/.github/workflows/publish-package-anaconda-org.yml` & `autora-3.0.0a9/.github/workflows/publish-package-anaconda-org.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a8/.github/workflows/publish-package-pypi.yml` & `autora-3.0.0a9/.github/workflows/publish-package-pypi.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a8/.github/workflows/test-conda-build.yml` & `autora-3.0.0a9/.github/workflows/test-conda-build.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a8/.github/workflows/test-pre-commit-hooks.yml` & `autora-3.0.0a9/.github/workflows/test-pre-commit-hooks.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a8/.github/workflows/test-pytest.yml` & `autora-3.0.0a9/.github/workflows/test-pytest.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a8/.gitignore` & `autora-3.0.0a9/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a8/.idea/autora.iml` & `autora-3.0.0a9/.idea/autora.iml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a8/.idea/inspectionProfiles/Project_Default.xml` & `autora-3.0.0a9/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a8/.idea/modules.xml` & `autora-3.0.0a9/.idea/modules.xml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a8/.pre-commit-config.yaml` & `autora-3.0.0a9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a8/LICENSE.md` & `autora-3.0.0a9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a8/PKG-INFO` & `autora-3.0.0a9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora
-Version: 3.0.0a8
+Version: 3.0.0a9
 Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process.
 Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
 License: Copyright 2021, Brown University, Providence, RI.
         
                                 All Rights Reserved
         
         Permission to use, copy, modify, and distribute this software and
@@ -27,24 +27,25 @@
 Project-URL: repository, https://github.com/AutoResearch/autora
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: all
 Provides-Extra: all-theorists
 Provides-Extra: theorist-darts
+Provides-Extra: theorist-bms
 Provides-Extra: all-experimentalists
 Provides-Extra: experimentalist-novelty-sampler
 Provides-Extra: experimentalist-inequality-sampler
 Provides-Extra: all-experiment-runners
 Provides-Extra: synthetic-experiments
 License-File: LICENSE.md
 
 # Automated Research Assistant
 
-<b>[AutoRA](https://pypi.org/project/autora/)</b> (<b>Au</b>tomated <b>R</b>esearch <b>A</b>ssistant) is an open-source framework for 
+<b>[AutoRA](https://pypi.org/project/autora/)</b> (<b>Auto</b>mated <b>R</b>esearch <b>A</b>ssistant) is an open-source framework for 
 automating multiple stages of the empirical research process, including model discovery, experimental design, data collection, and documentation for open science.
 
 ![Autonomous Empirical Research Paradigm](img/overview.png)
 
 AutoRA implements the <b>Autonomous Empirical Research Paradigm</b>, which involves a dynamic interplay
 between two artificial agents. The first agent, a theorist, is primarily responsible for constructing 
 computational models by relying on existing data to link experimental conditions to dependent measures.
```

### Comparing `autora-3.0.0a8/README.md` & `autora-3.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a8/conda/autora/meta.yaml` & `autora-3.0.0a9/conda/autora/meta.yaml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a8/docs/experimentalists/overview.md` & `autora-3.0.0a9/docs/experimentalists/index.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a8/docs/img/logo.png` & `autora-3.0.0a9/docs/img/logo.png`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a8/docs/img/overview.png` & `autora-3.0.0a9/docs/img/overview.png`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a8/docs/index.md` & `autora-3.0.0a9/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Automated Research Assistant
 
-<b>[AutoRA](https://pypi.org/project/autora/)</b> (<b>Au</b>tomated <b>R</b>esearch <b>A</b>ssistant) is an open-source framework for 
+<b>[AutoRA](https://pypi.org/project/autora/)</b> (<b>Auto</b>mated <b>R</b>esearch <b>A</b>ssistant) is an open-source framework for 
 automating multiple stages of the empirical research process, including model discovery, experimental design, data collection, and documentation for open science.
 
 ![Autonomous Empirical Research Paradigm](img/overview.png)
 
 AutoRA implements the <b>Autonomous Empirical Research Paradigm</b>, which involves a dynamic interplay
 between two artificial agents. The first agent, a theorist, is primarily responsible for constructing 
 computational models by relying on existing data to link experimental conditions to dependent measures.
```

### Comparing `autora-3.0.0a8/docs/theorist/overview.md` & `autora-3.0.0a9/docs/theorist/index.md`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a8/mkdocs/base.yml` & `autora-3.0.0a9/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-3.0.0a8/mkdocs.yml` & `autora-3.0.0a9/mkdocs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -35,23 +35,23 @@
 - Introduction: 'index.md'
 - Tutorials:
   - Automated Theorist
   - Automated Experimentalist
   - Closed-Loop Discovery
 - User Guide:
   - Theorists:
-    - Overview: 'theorist/overview.md'
+    - Home: 'theorist/index.md'
     - DARTS: '!import https://github.com/autoresearch/autora-theorist-darts/?branch=main&extra_imports=["mkdocs/base.yml"]'
+    - BMS: '!import https://github.com/autoresearch/autora-theorist-bms/?branch=main&extra_imports=["mkdocs/base.yml"]'
     - BSR
-    - BMS
   - Experimentalists:
-    - Overview: 'experimentalists/overview.md'
+    - Home: 'experimentalists/index.md'
     - Novelty Sampler: '!import https://github.com/autoresearch/autora-novelty-sampler/?branch=main&extra_imports=["mkdocs/base.yml"]'
     - Inequality Sampler: '!import https://github.com/autoresearch/autora-experimentalist-inequality-sampler/?branch=main&extra_imports=["mkdocs/base.yml"]'
   - Experiment Runners:
-    - Overview: 'experiment-runner/overview.md'
+    - Home: 'experiment-runner/index.md'
   - Synthetic Datasets: '!import https://github.com/autoresearch/autora-synthetic-data/?branch=main&extra_imports=["mkdocs/base.yml"]'
   - Workflow: '!import https://github.com/autoresearch/autora-workflow/?branch=main&extra_imports=["mkdocs/base.yml"]'
 - Contributor Guide:
   - Module Contributions
   - Core Contributions
```

### Comparing `autora-3.0.0a8/pyproject.toml` & `autora-3.0.0a9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,18 +24,22 @@
   "autora[all-experimentalists]",
   "autora[all-experiment-runners]",
   "autora[synthetic-experiments]",
 ]
 
 all-theorists = [
   "autora[theorist-darts]",
+  "autora[theorist-bms]",
 ]
 theorist-darts = [
   "autora-theorist-darts",
 ]
+theorist-bms = [
+  "autora-theorist-bms",
+]
 all-experimentalists = [
   "autora[experimentalist-inequality-sampler]",
   "autora[experimentalist-novelty-sampler]",
 ]
 experimentalist-novelty-sampler =[
   "autora-novelty-sampler"
 ]
```

### Comparing `autora-3.0.0a8/src/autora.egg-info/PKG-INFO` & `autora-3.0.0a9/src/autora.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora
-Version: 3.0.0a8
+Version: 3.0.0a9
 Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process.
 Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
 License: Copyright 2021, Brown University, Providence, RI.
         
                                 All Rights Reserved
         
         Permission to use, copy, modify, and distribute this software and
@@ -27,24 +27,25 @@
 Project-URL: repository, https://github.com/AutoResearch/autora
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: all
 Provides-Extra: all-theorists
 Provides-Extra: theorist-darts
+Provides-Extra: theorist-bms
 Provides-Extra: all-experimentalists
 Provides-Extra: experimentalist-novelty-sampler
 Provides-Extra: experimentalist-inequality-sampler
 Provides-Extra: all-experiment-runners
 Provides-Extra: synthetic-experiments
 License-File: LICENSE.md
 
 # Automated Research Assistant
 
-<b>[AutoRA](https://pypi.org/project/autora/)</b> (<b>Au</b>tomated <b>R</b>esearch <b>A</b>ssistant) is an open-source framework for 
+<b>[AutoRA](https://pypi.org/project/autora/)</b> (<b>Auto</b>mated <b>R</b>esearch <b>A</b>ssistant) is an open-source framework for 
 automating multiple stages of the empirical research process, including model discovery, experimental design, data collection, and documentation for open science.
 
 ![Autonomous Empirical Research Paradigm](img/overview.png)
 
 AutoRA implements the <b>Autonomous Empirical Research Paradigm</b>, which involves a dynamic interplay
 between two artificial agents. The first agent, a theorist, is primarily responsible for constructing 
 computational models by relying on existing data to link experimental conditions to dependent measures.
```

### Comparing `autora-3.0.0a8/src/autora.egg-info/SOURCES.txt` & `autora-3.0.0a9/src/autora.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -25,20 +25,20 @@
 .idea/inspectionProfiles/profiles_settings.xml
 .vscode/.gitignore
 .vscode/extensions.json
 .vscode/launch.json
 conda/autora/meta.yaml
 conda/autora/run_test.sh
 docs/index.md
-docs/experiment-runner/overview.md
-docs/experimentalists/overview.md
+docs/experiment-runner/index.md
+docs/experimentalists/index.md
 docs/img/logo.png
 docs/img/overview.png
 docs/javascripts/mathjax.js
-docs/theorist/overview.md
+docs/theorist/index.md
 mkdocs/base.yml
 mkdocs/overrides/main.html
 src/.keep
 src/autora.egg-info/PKG-INFO
 src/autora.egg-info/SOURCES.txt
 src/autora.egg-info/dependency_links.txt
 src/autora.egg-info/requires.txt
```

### Comparing `autora-3.0.0a8/src/autora.egg-info/requires.txt` & `autora-3.0.0a9/src/autora.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,22 +11,26 @@
 
 [all-experimentalists]
 autora[experimentalist-inequality-sampler]
 autora[experimentalist-novelty-sampler]
 
 [all-theorists]
 autora[theorist-darts]
+autora[theorist-bms]
 
 [dev]
 autora-core[dev]
 
 [experimentalist-inequality-sampler]
 autora-experimentalist-inequality-sampler
 
 [experimentalist-novelty-sampler]
 autora-novelty-sampler
 
 [synthetic-experiments]
 autora-synthetic-data
 
+[theorist-bms]
+autora-theorist-bms
+
 [theorist-darts]
 autora-theorist-darts
```

