# Comparing `tmp/invenio-records-marc21-0.9.1.tar.gz` & `tmp/invenio-records-marc21-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-records-marc21-0.9.1.tar", last modified: Mon Jan 23 14:01:05 2023, max compression
+gzip compressed data, was "invenio-records-marc21-0.9.2.tar", last modified: Thu Feb  9 15:33:19 2023, max compression
```

## Comparing `invenio-records-marc21-0.9.1.tar` & `invenio-records-marc21-0.9.2.tar`

### file list

```diff
@@ -1,258 +1,258 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.698479 invenio-records-marc21-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.670479 invenio-records-marc21-0.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.678479 invenio-records-marc21-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-01-23 14:01:05.698479 invenio-records-marc21-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.682479 invenio-records-marc21-0.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.682479 invenio-records-marc21-0.9.1/invenio_records_marc21/
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.682479 invenio-records-marc21-0.9.1/invenio_records_marc21/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3198 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/data/example-record.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/data/example-templates.json
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/data/fake-metadata.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/data/fake-record.json
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.682479 invenio-records-marc21-0.9.1/invenio_records_marc21/records/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.682479 invenio-records-marc21-0.9.1/invenio_records_marc21/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/records/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.682479 invenio-records-marc21-0.9.1/invenio_records_marc21/records/jsonschemas/marc21/
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/records/jsonschemas/marc21/definitions-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)   989189 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/records/jsonschemas/marc21/marc21-structure-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/records/jsonschemas/marc21/marc21-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/records/jsonschemas/marc21/parent-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.682479 invenio-records-marc21-0.9.1/invenio_records_marc21/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.682479 invenio-records-marc21-0.9.1/invenio_records_marc21/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.674479 invenio-records-marc21-0.9.1/invenio_records_marc21/records/mappings/os-v2/marc21records/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.682479 invenio-records-marc21-0.9.1/invenio_records_marc21/records/mappings/os-v2/marc21records/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/records/mappings/os-v2/marc21records/drafts/marc21-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.682479 invenio-records-marc21-0.9.1/invenio_records_marc21/records/mappings/os-v2/marc21records/marc21/
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/records/mappings/os-v2/marc21records/marc21/marc21-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.686479 invenio-records-marc21-0.9.1/invenio_records_marc21/records/systemfields/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/records/systemfields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/records/systemfields/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/records/systemfields/has_draft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/records/systemfields/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/records/systemfields/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/records/systemfields/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.686479 invenio-records-marc21-0.9.1/invenio_records_marc21/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.686479 invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.686479 invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/datacite/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/datacite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/datacite/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.686479 invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/fields/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/fields/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.686479 invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.686479 invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/ui/fields/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/ui/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/ui/fields/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/ui/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/ui/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.686479 invenio-records-marc21-0.9.1/invenio_records_marc21/services/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.686479 invenio-records-marc21-0.9.1/invenio_records_marc21/services/components/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/services/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/services/components/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/services/components/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/services/components/pids.py
--rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/services/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/services/customizations.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/services/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/services/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.686479 invenio-records-marc21-0.9.1/invenio_records_marc21/services/pids/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/services/pids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/services/pids/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.686479 invenio-records-marc21-0.9.1/invenio_records_marc21/services/record/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/services/record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/services/record/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/services/record/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/services/record/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.686479 invenio-records-marc21-0.9.1/invenio_records_marc21/services/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/services/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/services/schemas/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/services/schemas/pids.py
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/services/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/services/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.674479 invenio-records-marc21-0.9.1/invenio_records_marc21/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.674479 invenio-records-marc21-0.9.1/invenio_records_marc21/static/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.686479 invenio-records-marc21-0.9.1/invenio_records_marc21/static/templates/invenio_records_marc21/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/static/templates/invenio_records_marc21/results.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.690479 invenio-records-marc21-0.9.1/invenio_records_marc21/system/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/system/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/system/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/system/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.674479 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.690479 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/deposit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/record.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.690479 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.690479 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/details/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/details/subjects.html
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/export.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.690479 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/authors.html
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/description.html
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/details.html
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/files.html
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/side_bar.html
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/subjects.html
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/title.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.690479 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/macros/authors.html
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/macros/detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/macros/files.html
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/results.html
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/tombstone.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.690479 invenio-records-marc21-0.9.1/invenio_records_marc21/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.674479 invenio-records-marc21-0.9.1/invenio_records_marc21/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.690479 invenio-records-marc21-0.9.1/invenio_records_marc21/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.678479 invenio-records-marc21-0.9.1/invenio_records_marc21/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.690479 invenio-records-marc21-0.9.1/invenio_records_marc21/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/translations/en/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.690479 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.690479 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/records/
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/records/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/records/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/records/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/records/records.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/records/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.690479 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.678479 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.678479 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.678479 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.678479 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.694479 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/deposit/
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/deposit/Marc21DepositForm.js
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/deposit/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.694479 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/landing_page/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/landing_page/EditButton.js
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/landing_page/Marc21RecordManagement.js
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/landing_page/Marc21RecordVersionsList.js
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/landing_page/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.694479 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/search/
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/search/components.js
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/search/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.678479 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/less/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.694479 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/less/invenio_records_marc21/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/less/invenio_records_marc21/deposit.less
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/less/invenio_records_marc21/landing-page.less
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/less/invenio_records_marc21/theme.less
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/less/invenio_records_marc21/variables.less
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/deposit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/webpack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/invenio_records_marc21/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.682479 invenio-records-marc21-0.9.1/invenio_records_marc21.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-01-23 14:01:05.000000 invenio-records-marc21-0.9.1/invenio_records_marc21.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-01-23 14:01:05.000000 invenio-records-marc21-0.9.1/invenio_records_marc21.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 14:01:05.000000 invenio-records-marc21-0.9.1/invenio_records_marc21.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-01-23 14:01:05.000000 invenio-records-marc21-0.9.1/invenio_records_marc21.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 14:01:05.000000 invenio-records-marc21-0.9.1/invenio_records_marc21.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-01-23 14:01:05.000000 invenio-records-marc21-0.9.1/invenio_records_marc21.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-01-23 14:01:05.000000 invenio-records-marc21-0.9.1/invenio_records_marc21.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      777 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-01-23 14:01:05.698479 invenio-records-marc21-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.694479 invenio-records-marc21-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.694479 invenio-records-marc21-0.9.1/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/api/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/fake_datacite_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.694479 invenio-records-marc21-0.9.1/tests/records/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/records/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.694479 invenio-records-marc21-0.9.1/tests/records/systemfields/
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/records/systemfields/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/records/systemfields/test_systemfield_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/records/systemfields/test_systemfield_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/records/systemfields/test_systemfield_pid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/records/systemfields/test_systemfield_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/records/systemfields/test_systemfield_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/records/test-record.json
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/records/test_jsonschema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.678479 invenio-records-marc21-0.9.1/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.694479 invenio-records-marc21-0.9.1/tests/resources/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/resources/serializers/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/resources/serializers/test_datacite_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/resources/serializers/test_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.694479 invenio-records-marc21-0.9.1/tests/resources/serializers/ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.694479 invenio-records-marc21-0.9.1/tests/resources/serializers/ui/fields/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/resources/serializers/ui/fields/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/resources/serializers/ui/fields/test_ui_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/resources/serializers/ui/test_serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.694479 invenio-records-marc21-0.9.1/tests/services/
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/services/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.698479 invenio-records-marc21-0.9.1/tests/services/record/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/services/record/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/services/record/test_marc21_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.698479 invenio-records-marc21-0.9.1/tests/services/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 14:01:05.698479 invenio-records-marc21-0.9.1/tests/services/schemas/access/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/services/schemas/access/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/services/schemas/access/test_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/services/schemas/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/services/schemas/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/services/schemas/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/services/test-metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/services/test-metadata.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/services/test_create_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/services/test_pids_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/services/test_pids_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/services/test_record_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/test-metadata.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/test-record.json
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/test_invenio_records_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-01-23 14:01:01.000000 invenio-records-marc21-0.9.1/tests/test_invenio_records_marc21.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.435051 invenio-records-marc21-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.411050 invenio-records-marc21-0.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.419051 invenio-records-marc21-0.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-02-09 15:33:19.435051 invenio-records-marc21-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.419051 invenio-records-marc21-0.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.419051 invenio-records-marc21-0.9.2/invenio_records_marc21/
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.419051 invenio-records-marc21-0.9.2/invenio_records_marc21/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3198 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/data/example-record.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/data/example-templates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/data/fake-metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/data/fake-record.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.423050 invenio-records-marc21-0.9.2/invenio_records_marc21/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.423050 invenio-records-marc21-0.9.2/invenio_records_marc21/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/records/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.423050 invenio-records-marc21-0.9.2/invenio_records_marc21/records/jsonschemas/marc21/
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/records/jsonschemas/marc21/definitions-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)   989189 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/records/jsonschemas/marc21/marc21-structure-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/records/jsonschemas/marc21/marc21-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/records/jsonschemas/marc21/parent-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.423050 invenio-records-marc21-0.9.2/invenio_records_marc21/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.423050 invenio-records-marc21-0.9.2/invenio_records_marc21/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.411050 invenio-records-marc21-0.9.2/invenio_records_marc21/records/mappings/os-v2/marc21records/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.423050 invenio-records-marc21-0.9.2/invenio_records_marc21/records/mappings/os-v2/marc21records/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/records/mappings/os-v2/marc21records/drafts/marc21-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.423050 invenio-records-marc21-0.9.2/invenio_records_marc21/records/mappings/os-v2/marc21records/marc21/
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/records/mappings/os-v2/marc21records/marc21/marc21-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.423050 invenio-records-marc21-0.9.2/invenio_records_marc21/records/systemfields/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/records/systemfields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/records/systemfields/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/records/systemfields/has_draft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/records/systemfields/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/records/systemfields/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/records/systemfields/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.423050 invenio-records-marc21-0.9.2/invenio_records_marc21/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.423050 invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.423050 invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/datacite/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/datacite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/datacite/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.423050 invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/fields/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.423050 invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.423050 invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/ui/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/ui/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/ui/fields/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/ui/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/ui/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.427050 invenio-records-marc21-0.9.2/invenio_records_marc21/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.427050 invenio-records-marc21-0.9.2/invenio_records_marc21/services/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/services/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/services/components/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/services/components/pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/services/components/pids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/services/customizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/services/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/services/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.427050 invenio-records-marc21-0.9.2/invenio_records_marc21/services/pids/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/services/pids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/services/pids/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.427050 invenio-records-marc21-0.9.2/invenio_records_marc21/services/record/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/services/record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/services/record/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/services/record/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/services/record/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.427050 invenio-records-marc21-0.9.2/invenio_records_marc21/services/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/services/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/services/schemas/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/services/schemas/pids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/services/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/services/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.415050 invenio-records-marc21-0.9.2/invenio_records_marc21/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.415050 invenio-records-marc21-0.9.2/invenio_records_marc21/static/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.427050 invenio-records-marc21-0.9.2/invenio_records_marc21/static/templates/invenio_records_marc21/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/static/templates/invenio_records_marc21/results.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.427050 invenio-records-marc21-0.9.2/invenio_records_marc21/system/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/system/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/system/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/system/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.415050 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.427050 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/deposit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/record.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.427050 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.427050 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/details/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/details/subjects.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/export.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.427050 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/authors.html
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/description.html
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/details.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/files.html
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/side_bar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/subjects.html
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/title.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.431051 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/macros/authors.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/macros/detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/macros/files.html
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/results.html
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/tombstone.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.431051 invenio-records-marc21-0.9.2/invenio_records_marc21/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.415050 invenio-records-marc21-0.9.2/invenio_records_marc21/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.431051 invenio-records-marc21-0.9.2/invenio_records_marc21/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.415050 invenio-records-marc21-0.9.2/invenio_records_marc21/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.431051 invenio-records-marc21-0.9.2/invenio_records_marc21/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.431051 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.431051 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/records/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/records/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/records/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/records/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/records/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.431051 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.415050 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.415050 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.415050 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.415050 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.431051 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/deposit/
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/deposit/Marc21DepositForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/deposit/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.431051 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/landing_page/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/landing_page/EditButton.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/landing_page/Marc21RecordManagement.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/landing_page/Marc21RecordVersionsList.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/landing_page/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.431051 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/search/
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/search/components.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/search/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.415050 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.431051 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/less/invenio_records_marc21/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/less/invenio_records_marc21/deposit.less
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/less/invenio_records_marc21/landing-page.less
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/less/invenio_records_marc21/theme.less
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/less/invenio_records_marc21/variables.less
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/deposit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/webpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/invenio_records_marc21/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.419051 invenio-records-marc21-0.9.2/invenio_records_marc21.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-02-09 15:33:19.000000 invenio-records-marc21-0.9.2/invenio_records_marc21.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-02-09 15:33:19.000000 invenio-records-marc21-0.9.2/invenio_records_marc21.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 15:33:19.000000 invenio-records-marc21-0.9.2/invenio_records_marc21.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-02-09 15:33:19.000000 invenio-records-marc21-0.9.2/invenio_records_marc21.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 15:33:19.000000 invenio-records-marc21-0.9.2/invenio_records_marc21.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-02-09 15:33:19.000000 invenio-records-marc21-0.9.2/invenio_records_marc21.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-09 15:33:19.000000 invenio-records-marc21-0.9.2/invenio_records_marc21.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      777 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-02-09 15:33:19.435051 invenio-records-marc21-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.431051 invenio-records-marc21-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.431051 invenio-records-marc21-0.9.2/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/api/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/fake_datacite_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.431051 invenio-records-marc21-0.9.2/tests/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/records/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.435051 invenio-records-marc21-0.9.2/tests/records/systemfields/
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/records/systemfields/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/records/systemfields/test_systemfield_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/records/systemfields/test_systemfield_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/records/systemfields/test_systemfield_pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/records/systemfields/test_systemfield_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/records/systemfields/test_systemfield_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/records/test-record.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/records/test_jsonschema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.415050 invenio-records-marc21-0.9.2/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.435051 invenio-records-marc21-0.9.2/tests/resources/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/resources/serializers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/resources/serializers/test_datacite_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/resources/serializers/test_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.435051 invenio-records-marc21-0.9.2/tests/resources/serializers/ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.435051 invenio-records-marc21-0.9.2/tests/resources/serializers/ui/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/resources/serializers/ui/fields/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/resources/serializers/ui/fields/test_ui_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/resources/serializers/ui/test_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.435051 invenio-records-marc21-0.9.2/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/services/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.435051 invenio-records-marc21-0.9.2/tests/services/record/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/services/record/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/services/record/test_marc21_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.435051 invenio-records-marc21-0.9.2/tests/services/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 15:33:19.435051 invenio-records-marc21-0.9.2/tests/services/schemas/access/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/services/schemas/access/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/services/schemas/access/test_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/services/schemas/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/services/schemas/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/services/schemas/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/services/test-metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/services/test-metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/services/test_create_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/services/test_pids_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/services/test_pids_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/services/test_record_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/test-metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/test-record.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/test_invenio_records_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-02-09 15:33:11.000000 invenio-records-marc21-0.9.2/tests/test_invenio_records_marc21.py
```

### Comparing `invenio-records-marc21-0.9.1/.editorconfig` & `invenio-records-marc21-0.9.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/CHANGES.rst` & `invenio-records-marc21-0.9.2/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,21 @@
     Invenio-Records-Marc21 is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.9.2 (release 2023-02-09)
+
+- fix: sort xml subfields generation
+- fix: the value in subfs is a list
+- fix: unify order of et.Element attributes
+
+
 Version v0.9.1 (release 2023-01-23)
 
 - fix: wrong alias for drafts and records
 - modification: record status in deposit
 
 
 Version v0.9.0 (release 2023-01-11)
```

### Comparing `invenio-records-marc21-0.9.1/CONTRIBUTING.rst` & `invenio-records-marc21-0.9.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/INSTALL.rst` & `invenio-records-marc21-0.9.2/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/LICENSE` & `invenio-records-marc21-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/MANIFEST.in` & `invenio-records-marc21-0.9.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/PKG-INFO` & `invenio-records-marc21-0.9.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-records-marc21
-Version: 0.9.1
+Version: 0.9.2
 Summary: "Invenio Marc21 datamodel."
 Home-page: https://github.com/tu-graz-library/invenio-records-marc21
 Author: "Graz University of Technology"
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio Marc21 record
 Platform: any
@@ -77,14 +77,21 @@
     Invenio-Records-Marc21 is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.9.2 (release 2023-02-09)
+
+- fix: sort xml subfields generation
+- fix: the value in subfs is a list
+- fix: unify order of et.Element attributes
+
+
 Version v0.9.1 (release 2023-01-23)
 
 - fix: wrong alias for drafts and records
 - modification: record status in deposit
 
 
 Version v0.9.0 (release 2023-01-11)
```

### Comparing `invenio-records-marc21-0.9.1/README.rst` & `invenio-records-marc21-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/babel.ini` & `invenio-records-marc21-0.9.2/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/docs/Makefile` & `invenio-records-marc21-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/docs/conf.py` & `invenio-records-marc21-0.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/docs/index.rst` & `invenio-records-marc21-0.9.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/docs/make.bat` & `invenio-records-marc21-0.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/__init__.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,15 +218,15 @@
     add_file_to_record,
     check_about_duplicate,
     convert_json_to_marc21xml,
     convert_marc21xml_to_json,
     create_record,
 )
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 __all__ = (
     "__version__",
     "InvenioRecordsMARC21",
     "current_records_marc21",
     "Marc21Metadata",
     "add_file_to_record",
```

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/cli.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/config.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/data/example-record.xml` & `invenio-records-marc21-0.9.2/invenio_records_marc21/data/example-record.xml`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/data/example-templates.json` & `invenio-records-marc21-0.9.2/invenio_records_marc21/data/example-templates.json`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/data/fake-metadata.xml` & `invenio-records-marc21-0.9.2/invenio_records_marc21/data/fake-metadata.xml`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/data/fake-record.json` & `invenio-records-marc21-0.9.2/invenio_records_marc21/data/fake-record.json`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/errors.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ext.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/proxies.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/records/__init__.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/records/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/records/api.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/records/api.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/records/jsonschemas/__init__.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/records/jsonschemas/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/records/jsonschemas/marc21/definitions-v1.0.0.json` & `invenio-records-marc21-0.9.2/invenio_records_marc21/records/jsonschemas/marc21/definitions-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/records/jsonschemas/marc21/marc21-structure-v1.0.0.json` & `invenio-records-marc21-0.9.2/invenio_records_marc21/records/jsonschemas/marc21/marc21-structure-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/records/jsonschemas/marc21/marc21-v1.0.0.json` & `invenio-records-marc21-0.9.2/invenio_records_marc21/records/jsonschemas/marc21/marc21-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/records/jsonschemas/marc21/parent-v1.0.0.json` & `invenio-records-marc21-0.9.2/invenio_records_marc21/records/jsonschemas/marc21/parent-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/records/mappings/__init__.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/records/mappings/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/records/mappings/os-v2/marc21records/drafts/marc21-v1.0.0.json` & `invenio-records-marc21-0.9.2/invenio_records_marc21/records/mappings/os-v2/marc21records/drafts/marc21-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/records/mappings/os-v2/marc21records/marc21/marc21-v1.0.0.json` & `invenio-records-marc21-0.9.2/invenio_records_marc21/records/mappings/os-v2/marc21records/marc21/marc21-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/records/models.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/records/systemfields/__init__.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/records/systemfields/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/records/systemfields/context.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/records/systemfields/context.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/records/systemfields/has_draft.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/records/systemfields/has_draft.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/records/systemfields/providers.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/records/systemfields/providers.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/records/systemfields/resolver.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/records/systemfields/resolver.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/records/systemfields/status.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/records/systemfields/status.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/resources/__init__.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/resources/config.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/resources/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/resources/resources.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/resources/resources.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/__init__.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/datacite/__init__.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/datacite/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/datacite/schema.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/datacite/schema.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/fields/metadata.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/fields/metadata.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/schema.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/schema.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/serializer.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/serializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,14 @@
         for key, value in fields.items():
             # Control fields
             if key in self.controlfields:
                 controlfield = E.controlfield(value)
                 controlfield.attrib["tag"] = key
                 rec.append(controlfield)
             else:
-
                 for subfields in value:
                     datafield = E.datafield()
                     datafield.attrib["tag"] = key
 
                     indicator1 = subfields.get("ind1", " ")
                     indicator2 = subfields.get("ind2", " ")
```

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/ui/__init__.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/ui/fields/metadata.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/ui/fields/metadata.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/ui/schema.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/ui/schema.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/resources/serializers/ui/serializers.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/resources/serializers/ui/serializers.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/services/__init__.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/services/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/services/components/metadata.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/services/components/metadata.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/services/components/pid.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/services/components/pid.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/services/components/pids.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/services/components/pids.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/services/config.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/services/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/services/customizations.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/services/customizations.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/services/errors.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/services/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/services/permissions.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/services/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/services/pids/tasks.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/services/pids/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/services/record/__init__.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/services/record/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/services/record/metadata.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/services/record/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,17 +67,17 @@
         self.record.append(controlfield)
 
     def visit_datafield(self, category, items):
         """Visit datafield."""
         for item in items:
             datafield = Element(
                 "datafield",
-                {"ind1": item["ind1"], "ind2": item["ind2"], "tag": category},
+                {"tag": category, "ind1": item["ind1"], "ind2": item["ind2"]},
             )
-            for subfn, subfv in item["subfields"].items():
+            for subfn, subfv in sorted(item["subfields"].items()):
                 subfield = Element("subfield", {"code": subfn})
                 subfield.text = " ".join(subfv)
                 datafield.append(subfield)
 
             self.record.append(datafield)
 
 
@@ -274,17 +274,17 @@
         datafield = Element("datafield", tag=tag, ind1=ind1, ind2=ind2)
         if value:
             subfield = Element("subfield", code=code)
             subfield.text = value
             datafield.append(subfield)
 
         elif subfs:
-            for key, val in subfs.items():
+            for key, val in sorted(subfs.items()):
                 subfield = Element("subfield", code=key)
-                subfield.text = val
+                subfield.text = " ".join(val)
                 datafield.append(subfield)
 
         else:
             raise RuntimeError("Neither of value or subfs is set.")
 
         # double check
         if self.exists(datafield, "datafield"):
```

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/services/record/types.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/services/record/types.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/services/record/utils.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/services/record/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/services/schemas/__init__.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/services/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/services/schemas/metadata.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/services/schemas/metadata.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/services/schemas/pids.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/services/schemas/pids.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/services/services.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/services/services.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/services/tasks.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/services/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/static/templates/invenio_records_marc21/results.html` & `invenio-records-marc21-0.9.2/invenio_records_marc21/static/templates/invenio_records_marc21/results.html`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/system/models.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/system/models.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/system/service.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/system/service.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/deposit.html` & `invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/deposit.html`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/index.html` & `invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/index.html`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/record.html` & `invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/record.html`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/details/subjects.html` & `invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/details/subjects.html`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/export.html` & `invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/export.html`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/authors.html` & `invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/authors.html`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/details.html` & `invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/details.html`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/files.html` & `invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/files.html`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/footer.html` & `invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/footer.html`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/side_bar.html` & `invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/side_bar.html`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/subjects.html` & `invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/subjects.html`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/title.html` & `invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/helpers/title.html`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/macros/detail.html` & `invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/macros/detail.html`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/records/macros/files.html` & `invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/records/macros/files.html`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/results.html` & `invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/results.html`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/search.html` & `invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/search.html`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/templates/invenio_records_marc21/tombstone.html` & `invenio-records-marc21-0.9.2/invenio_records_marc21/templates/invenio_records_marc21/tombstone.html`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/translations/de/LC_MESSAGES/messages.po` & `invenio-records-marc21-0.9.2/invenio_records_marc21/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/translations/en/LC_MESSAGES/messages.po` & `invenio-records-marc21-0.9.2/invenio_records_marc21/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/translations/messages.pot` & `invenio-records-marc21-0.9.2/invenio_records_marc21/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ui/__init__.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ui/records/__init__.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ui/records/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ui/records/decorators.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ui/records/decorators.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ui/records/errors.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ui/records/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ui/records/filters.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ui/records/filters.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ui/records/records.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ui/records/records.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ui/records/wrappers.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ui/records/wrappers.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/__init__.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/deposit/Marc21DepositForm.js` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/deposit/Marc21DepositForm.js`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/deposit/index.js` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/deposit/index.js`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/landing_page/EditButton.js` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/landing_page/EditButton.js`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/landing_page/Marc21RecordManagement.js` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/landing_page/Marc21RecordManagement.js`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/landing_page/Marc21RecordVersionsList.js` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/landing_page/Marc21RecordVersionsList.js`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/landing_page/index.js` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/landing_page/index.js`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/search/components.js` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/search/components.js`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/search/index.js` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/js/invenio_records_marc21/search/index.js`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/less/invenio_records_marc21/deposit.less` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/less/invenio_records_marc21/deposit.less`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/assets/semantic-ui/less/invenio_records_marc21/landing-page.less` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/assets/semantic-ui/less/invenio_records_marc21/landing-page.less`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/config.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/decorators.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/decorators.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/deposit.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/deposit.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/views.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/views.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/ui/theme/webpack.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/ui/theme/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21/views.py` & `invenio-records-marc21-0.9.2/invenio_records_marc21/views.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21.egg-info/PKG-INFO` & `invenio-records-marc21-0.9.2/invenio_records_marc21.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-records-marc21
-Version: 0.9.1
+Version: 0.9.2
 Summary: "Invenio Marc21 datamodel."
 Home-page: https://github.com/tu-graz-library/invenio-records-marc21
 Author: "Graz University of Technology"
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio Marc21 record
 Platform: any
@@ -77,14 +77,21 @@
     Invenio-Records-Marc21 is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v0.9.2 (release 2023-02-09)
+
+- fix: sort xml subfields generation
+- fix: the value in subfs is a list
+- fix: unify order of et.Element attributes
+
+
 Version v0.9.1 (release 2023-01-23)
 
 - fix: wrong alias for drafts and records
 - modification: record status in deposit
 
 
 Version v0.9.0 (release 2023-01-11)
```

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21.egg-info/SOURCES.txt` & `invenio-records-marc21-0.9.2/invenio_records_marc21.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/invenio_records_marc21.egg-info/entry_points.txt` & `invenio-records-marc21-0.9.2/invenio_records_marc21.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/requirements-devel.txt` & `invenio-records-marc21-0.9.2/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/run-tests.sh` & `invenio-records-marc21-0.9.2/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/setup.cfg` & `invenio-records-marc21-0.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/api/conftest.py` & `invenio-records-marc21-0.9.2/tests/api/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/conftest.py` & `invenio-records-marc21-0.9.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/fake_datacite_client.py` & `invenio-records-marc21-0.9.2/tests/fake_datacite_client.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/records/conftest.py` & `invenio-records-marc21-0.9.2/tests/records/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/records/systemfields/conftest.py` & `invenio-records-marc21-0.9.2/tests/records/systemfields/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/records/systemfields/test_systemfield_access.py` & `invenio-records-marc21-0.9.2/tests/records/systemfields/test_systemfield_access.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/records/systemfields/test_systemfield_files.py` & `invenio-records-marc21-0.9.2/tests/records/systemfields/test_systemfield_files.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/records/systemfields/test_systemfield_pid.py` & `invenio-records-marc21-0.9.2/tests/records/systemfields/test_systemfield_pid.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/records/systemfields/test_systemfield_providers.py` & `invenio-records-marc21-0.9.2/tests/records/systemfields/test_systemfield_providers.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/records/systemfields/test_systemfield_resolver.py` & `invenio-records-marc21-0.9.2/tests/records/systemfields/test_systemfield_resolver.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/records/test_jsonschema.py` & `invenio-records-marc21-0.9.2/tests/records/test_jsonschema.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/resources/serializers/conftest.py` & `invenio-records-marc21-0.9.2/tests/resources/serializers/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/resources/serializers/test_datacite_serializer.py` & `invenio-records-marc21-0.9.2/tests/resources/serializers/test_datacite_serializer.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/resources/serializers/test_serializer.py` & `invenio-records-marc21-0.9.2/tests/resources/serializers/test_serializer.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/resources/serializers/ui/fields/test_ui_metadata.py` & `invenio-records-marc21-0.9.2/tests/resources/serializers/ui/fields/test_ui_metadata.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/resources/serializers/ui/test_serializers.py` & `invenio-records-marc21-0.9.2/tests/resources/serializers/ui/test_serializers.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/services/conftest.py` & `invenio-records-marc21-0.9.2/tests/services/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/services/record/test_marc21_metadata.py` & `invenio-records-marc21-0.9.2/tests/services/record/test_marc21_metadata.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/services/schemas/access/test_record.py` & `invenio-records-marc21-0.9.2/tests/services/schemas/access/test_record.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/services/schemas/test_utils.py` & `invenio-records-marc21-0.9.2/tests/services/schemas/test_utils.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/services/test-metadata.json` & `invenio-records-marc21-0.9.2/tests/services/test-metadata.json`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/services/test-metadata.xml` & `invenio-records-marc21-0.9.2/tests/services/test-metadata.xml`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/services/test_create_record.py` & `invenio-records-marc21-0.9.2/tests/services/test_create_record.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/services/test_pids_service.py` & `invenio-records-marc21-0.9.2/tests/services/test_pids_service.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/services/test_pids_tasks.py` & `invenio-records-marc21-0.9.2/tests/services/test_pids_tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/services/test_record_service.py` & `invenio-records-marc21-0.9.2/tests/services/test_record_service.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/test-metadata.xml` & `invenio-records-marc21-0.9.2/tests/test-metadata.xml`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/test-record.json` & `invenio-records-marc21-0.9.2/tests/test-record.json`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/test_invenio_records_cli.py` & `invenio-records-marc21-0.9.2/tests/test_invenio_records_cli.py`

 * *Files identical despite different names*

### Comparing `invenio-records-marc21-0.9.1/tests/test_invenio_records_marc21.py` & `invenio-records-marc21-0.9.2/tests/test_invenio_records_marc21.py`

 * *Files identical despite different names*

