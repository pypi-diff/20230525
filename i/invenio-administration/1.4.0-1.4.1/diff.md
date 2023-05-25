# Comparing `tmp/invenio-administration-1.4.0.tar.gz` & `tmp/invenio-administration-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-administration-1.4.0.tar", last modified: Tue Apr 25 08:38:47 2023, max compression
+gzip compressed data, was "dist/invenio-administration-1.4.1.tar", last modified: Thu May 25 07:42:43 2023, max compression
```

## Comparing `invenio-administration-1.4.0.tar` & `invenio-administration-1.4.1.tar`

### file list

```diff
@@ -1,379 +1,379 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/.eslintrc.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/.eslintrc.yml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ActionModal.js
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Actions.js
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Delete.js
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModal.js
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModalTrigger.js
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Edit.js
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ResourceActions.js
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/actions.js
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/routes.js
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/serializers.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/BoolFormatter.js
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/DateFormatter.js
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/ErrorPage.js
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.js
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.test.js
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Loader.js
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/CreatePage.js
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/create.js
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/AdminDetailsView.js
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/DetailsComponent.js
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/details.js
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/EditPage.js
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/edit.js
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/ActionForm.js
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/AdminForm.js
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/GenerateForm.js
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/array.js
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/routes.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBar.js
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBarElement.js
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchComponents.js
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchEmptyResults.js
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchFacets.js
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResults.js
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultsContainer.js
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/search.js
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/theme.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/context.js
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/messages.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next-scanner.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/translations.json
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/translations.json
--rw-r--r--   0 runner    (1001) docker     (123)   132884 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/compileCatalog.js
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/initCatalog.js
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/translations.pot
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/marshmallow_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/menu/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/menu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/menu/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    32571 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/static/images/dashboard.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_administration/
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_administration/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_administration/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_administration/details.html
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_administration/edit.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_administration/header/
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_administration/header/header.html
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_administration/header/side_bar_toggle.html
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_administration/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_administration/macros.html
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_administration/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_administration/sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_administration/sidebar/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_theme/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_theme/header_login.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/translations/zh_TW/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration/views/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13925 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/views/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/views/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/invenio_administration/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17614 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/invenio_administration.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/pytest.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)      701 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/run-js-linter.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      980 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/tests/mock_module/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/tests/mock_module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:47.000000 invenio-administration-1.4.0/tests/mock_module/administration/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/tests/mock_module/administration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/tests/mock_module/administration/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/tests/mock_module/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/tests/mock_module/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/tests/test_admin_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/tests/test_details_view.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/tests/test_invenio_administration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:38:41.000000 invenio-administration-1.4.0/tests/test_list_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/.eslintrc.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:42.000000 invenio-administration-1.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/.tx/
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:42.000000 invenio-administration-1.4.1/invenio_administration/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:42.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:42.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/.eslintrc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ActionModal.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Actions.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Delete.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModal.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModalTrigger.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Edit.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ResourceActions.js
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/actions.js
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/routes.js
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/serializers.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/BoolFormatter.js
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/DateFormatter.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/ErrorPage.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.test.js
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Loader.js
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/CreatePage.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/create.js
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/AdminDetailsView.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/DetailsComponent.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/details.js
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/EditPage.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/edit.js
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/ActionForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/AdminForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/GenerateForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/array.js
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/routes.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBar.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBarElement.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchComponents.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchEmptyResults.js
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchFacets.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResults.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultsContainer.js
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/search.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/theme.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/context.js
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/messages.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:42.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next-scanner.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/en/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/translations.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/translations.json
+-rw-r--r--   0 runner    (1001) docker     (123)   132884 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/compileCatalog.js
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/initCatalog.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/translations.pot
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/marshmallow_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/menu/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/menu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/menu/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:42.000000 invenio-administration-1.4.1/invenio_administration/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    32571 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/static/images/dashboard.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:42.000000 invenio-administration-1.4.1/invenio_administration/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:42.000000 invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_administration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_administration/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_administration/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_administration/details.html
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_administration/edit.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_administration/header/
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_administration/header/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_administration/header/side_bar_toggle.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_administration/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_administration/macros.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_administration/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_administration/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_administration/sidebar/sidenav.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_theme/header_login.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:42.000000 invenio-administration-1.4.1/invenio_administration/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:42.000000 invenio-administration-1.4.1/invenio_administration/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:42.000000 invenio-administration-1.4.1/invenio_administration/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-25 07:42:42.000000 invenio-administration-1.4.1/invenio_administration/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/translations/zh_TW/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13925 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/views/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/invenio_administration/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/invenio_administration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-05-25 07:42:42.000000 invenio-administration-1.4.1/invenio_administration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17614 2023-05-25 07:42:42.000000 invenio-administration-1.4.1/invenio_administration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:42:42.000000 invenio-administration-1.4.1/invenio_administration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-25 07:42:42.000000 invenio-administration-1.4.1/invenio_administration.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:42:42.000000 invenio-administration-1.4.1/invenio_administration.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-25 07:42:42.000000 invenio-administration-1.4.1/invenio_administration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 07:42:42.000000 invenio-administration-1.4.1/invenio_administration.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/pytest.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)      701 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/run-js-linter.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      980 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/tests/mock_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/tests/mock_module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:43.000000 invenio-administration-1.4.1/tests/mock_module/administration/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/tests/mock_module/administration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/tests/mock_module/administration/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/tests/mock_module/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/tests/mock_module/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/tests/test_admin_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/tests/test_details_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/tests/test_invenio_administration.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:42:36.000000 invenio-administration-1.4.1/tests/test_list_view.py
```

### Comparing `invenio-administration-1.4.0/.editorconfig` & `invenio-administration-1.4.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/.github/workflows/pypi-publish.yml` & `invenio-administration-1.4.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/.github/workflows/tests.yml` & `invenio-administration-1.4.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/.tx/config` & `invenio-administration-1.4.1/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/CHANGES.rst` & `invenio-administration-1.4.1/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,18 @@
     invenio-administration is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version 1.4.1 (2023-05-25)
+
+- fix action form creation
+
 Version 1.4.0 (2023-04-25)
 
 - upgrade invenio-records-resources
 
 Version 1.3.0 (2023-04-20)
 
 - upgrade invenio-records-resources
```

### Comparing `invenio-administration-1.4.0/CONTRIBUTING.rst` & `invenio-administration-1.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/MANIFEST.in` & `invenio-administration-1.4.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/PKG-INFO` & `invenio-administration-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-administration
-Version: 1.4.0
+Version: 1.4.1
 Summary: "Invenio module that adds administration panel to the system."
 Home-page: https://github.com/inveniosoftware/invenio-administration
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
@@ -42,14 +42,18 @@
             invenio-administration is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 1.4.1 (2023-05-25)
+        
+        - fix action form creation
+        
         Version 1.4.0 (2023-04-25)
         
         - upgrade invenio-records-resources
         
         Version 1.3.0 (2023-04-20)
         
         - upgrade invenio-records-resources
```

### Comparing `invenio-administration-1.4.0/README.rst` & `invenio-administration-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/docs/Makefile` & `invenio-administration-1.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/docs/conf.py` & `invenio-administration-1.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/docs/index.rst` & `invenio-administration-1.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/docs/make.bat` & `invenio-administration-1.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/admin.py` & `invenio-administration-1.4.1/invenio_administration/admin.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/package.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/package.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ActionModal.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ActionModal.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Actions.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Actions.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Delete.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Delete.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModal.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModal.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModalTrigger.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/DeleteModalTrigger.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Edit.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/Edit.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ResourceActions.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/ResourceActions.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/index.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/actions/index.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/actions.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/api/actions.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/BoolFormatter.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/BoolFormatter.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/DateFormatter.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/DateFormatter.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/ErrorPage.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/ErrorPage.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.test.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Formatter.test.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Loader.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/Loader.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/utils.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/components/utils.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/CreatePage.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/CreatePage.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/create.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/create/create.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/AdminDetailsView.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/AdminDetailsView.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/DetailsComponent.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/DetailsComponent.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/details.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/details/details.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/EditPage.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/EditPage.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/edit.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/edit/edit.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/ActionForm.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/ActionForm.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -143,15 +143,15 @@
                         props.handleSubmit
                     } >
                     <
                     GenerateForm jsonSchema = {
                         actionSchema
                     }
                     formFields = {
-                        formFields
+                        actionSchema
                     }
                     create dropDumpOnly /
                     > {
                         !isEmpty(error) && ( <
                             ErrorMessage {
                                 ...error
                             }
```

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/AdminForm.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/AdminForm.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/GenerateForm.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/GenerateForm.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/array.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/formik/array.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBar.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBar.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBarElement.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchBarElement.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchComponents.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchComponents.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchEmptyResults.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchEmptyResults.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchFacets.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchFacets.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultItem.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultItem.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResults.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResults.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultsContainer.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/SearchResultsContainer.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/index.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/index.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/search.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/search/search.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/theme.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/theme.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/context.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/context.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/messages.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/js/invenio_administration/src/ui_messages/messages.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next-scanner.config.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next-scanner.config.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/i18next.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/af/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ar/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/bg/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ca/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/cs/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/da/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/de/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/el/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/es/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/et_EE/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fa/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/fr/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/gl/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hr/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/hu/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/index.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/index.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/it/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ja/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ka/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/lt/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/no/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pl/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/pt/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ro/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/ru/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/rw/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sk/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/sv/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/tr/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/uk/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_CN/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/messages.po` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/translations.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/messages/zh_TW/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/package-lock.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/package-lock.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/package.json` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/package.json`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/compileCatalog.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/compileCatalog.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/initCatalog.js` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/scripts/initCatalog.js`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/assets/semantic-ui/translations/invenio_administration/translations.pot` & `invenio-administration-1.4.1/invenio_administration/assets/semantic-ui/translations/invenio_administration/translations.pot`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/config.py` & `invenio-administration-1.4.1/invenio_administration/config.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/errors.py` & `invenio-administration-1.4.1/invenio_administration/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/ext.py` & `invenio-administration-1.4.1/invenio_administration/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/generators.py` & `invenio-administration-1.4.1/invenio_administration/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/marshmallow_utils.py` & `invenio-administration-1.4.1/invenio_administration/marshmallow_utils.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/menu/menu.py` & `invenio-administration-1.4.1/invenio_administration/menu/menu.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/static/images/dashboard.png` & `invenio-administration-1.4.1/invenio_administration/static/images/dashboard.png`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_administration/base.html` & `invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_administration/base.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_administration/create.html` & `invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_administration/create.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_administration/details.html` & `invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_administration/details.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_administration/edit.html` & `invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_administration/edit.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_administration/header/header.html` & `invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_administration/header/header.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html` & `invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_administration/header/header_login.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_administration/index.html` & `invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_administration/index.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_administration/search.html` & `invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_administration/search.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_administration/sidebar/sidenav.html` & `invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_administration/sidebar/sidenav.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/templates/semantic-ui/invenio_theme/header_login.html` & `invenio-administration-1.4.1/invenio_administration/templates/semantic-ui/invenio_theme/header_login.html`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/af/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/ar/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/bg/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/ca/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/cs/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/da/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/de/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/el/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/en/LC_MESSAGES/messages.mo` & `invenio-administration-1.4.1/invenio_administration/translations/en/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/en/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/es/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/et/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/fa/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/fr/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/gl/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/hr/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/hu/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/it/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/ja/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/ka/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/lt/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/messages.pot` & `invenio-administration-1.4.1/invenio_administration/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/no/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/pl/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/pt/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/ro/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/ru/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/rw/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/sk/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/sv/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/tr/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/uk/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-administration-1.4.1/invenio_administration/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/views/base.py` & `invenio-administration-1.4.1/invenio_administration/views/base.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/views/dashboard.py` & `invenio-administration-1.4.1/invenio_administration/views/dashboard.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration/webpack.py` & `invenio-administration-1.4.1/invenio_administration/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration.egg-info/PKG-INFO` & `invenio-administration-1.4.1/invenio_administration.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-administration
-Version: 1.4.0
+Version: 1.4.1
 Summary: "Invenio module that adds administration panel to the system."
 Home-page: https://github.com/inveniosoftware/invenio-administration
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
@@ -42,14 +42,18 @@
             invenio-administration is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 1.4.1 (2023-05-25)
+        
+        - fix action form creation
+        
         Version 1.4.0 (2023-04-25)
         
         - upgrade invenio-records-resources
         
         Version 1.3.0 (2023-04-20)
         
         - upgrade invenio-records-resources
```

### Comparing `invenio-administration-1.4.0/invenio_administration.egg-info/SOURCES.txt` & `invenio-administration-1.4.1/invenio_administration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/invenio_administration.egg-info/requires.txt` & `invenio-administration-1.4.1/invenio_administration.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/run-js-linter.sh` & `invenio-administration-1.4.1/run-js-linter.sh`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/run-tests.sh` & `invenio-administration-1.4.1/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/setup.cfg` & `invenio-administration-1.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/tests/conftest.py` & `invenio-administration-1.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/tests/mock_module/administration/mock.py` & `invenio-administration-1.4.1/tests/mock_module/administration/mock.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/tests/mock_module/config.py` & `invenio-administration-1.4.1/tests/mock_module/config.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/tests/test_admin_menu.py` & `invenio-administration-1.4.1/tests/test_admin_menu.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/tests/test_base.py` & `invenio-administration-1.4.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `invenio-administration-1.4.0/tests/test_invenio_administration.py` & `invenio-administration-1.4.1/tests/test_invenio_administration.py`

 * *Files identical despite different names*

