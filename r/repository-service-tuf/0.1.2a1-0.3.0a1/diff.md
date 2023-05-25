# Comparing `tmp/repository_service_tuf-0.1.2a1.tar.gz` & `tmp/repository_service_tuf-0.3.0a1.tar.gz`

## Comparing `repository_service_tuf-0.1.2a1.tar` & `repository_service_tuf-0.3.0a1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.gitignore
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.readthedocs.yaml
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/CODE_OF_CONDUCT.rst
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/LICENSE
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/MAINTAINERS.rst
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/Makefile
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/Pipfile
--rw-r--r--   0        0        0    80651 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/Pipfile.lock
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/README.rst
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/pyproject.toml
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/requirements-dev.txt
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/requirements.txt
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tox.ini
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.github/dependabot.yml
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.github/ISSUE_TEMPLATE/other.yml
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.github/ISSUE_TEMPLATE/task.yml
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.github/PULL_REQUEST_TEMPLATE/pr.yml
--rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.github/workflows/cd.yml
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.github/workflows/update-python-deps.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/Makefile
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/make.bat
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/requirements.txt
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/diagrams/repository-service-tuf-cli-C1.puml
--rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/diagrams/repository-service-tuf-cli-C2.puml
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/diagrams/repository-service-tuf-cli-C3.puml
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/conf.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/index.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/_static/INFO
--rw-r--r--   0        0        0    19648 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/_static/repository-service-tuf-cli-C1.png
--rw-r--r--   0        0        0    41916 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/_static/repository-service-tuf-cli-C2.png
--rw-r--r--   0        0        0    94852 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/_static/repository-service-tuf-cli-C3.png
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/devel/design.rst
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/devel/index.rst
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/devel/modules.rst
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/devel/repository_service_tuf.cli.admin.rst
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/devel/repository_service_tuf.cli.key.rst
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/devel/repository_service_tuf.cli.rst
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/devel/repository_service_tuf.helpers.rst
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/devel/repository_service_tuf.rst
--rw-r--r--   0        0        0    45538 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/guide/index.rst
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/__version__.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/constants.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/cli/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/cli/admin/__init__.py
--rw-r--r--   0        0        0    25465 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/cli/admin/ceremony.py
--rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/cli/admin/import_targets.py
--rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/cli/admin/login.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/cli/admin/token.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/cli/key/__init__.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/cli/key/generate_key.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/helpers/__init__.py
--rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/helpers/api_client.py
--rw-r--r--   0        0        0     8014 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/helpers/tuf.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/conftest.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/test_tuf_repository_service.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/files/README.md
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/files/key_storage/JanisJoplin.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/files/key_storage/JanisJoplin.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/files/key_storage/JimiHendrix.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/files/key_storage/JimiHendrix.pub
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/files/key_storage/online-rsa.key
--rwxr-xr-x   0        0        0      624 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/files/key_storage/online-rsa.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/files/key_storage/online.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/files/key_storage/online.pub
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/unit/cli/test__init__.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/unit/cli/admin/__init__.py
--rw-r--r--   0        0        0    32379 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/unit/cli/admin/test_ceremony.py
--rw-r--r--   0        0        0    15993 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/unit/cli/admin/test_import_targets.py
--rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/unit/cli/admin/test_login.py
--rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/unit/cli/key/test_generate_key.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/unit/helpers/__init__.py
--rw-r--r--   0        0        0    21182 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/unit/helpers/test_api_client.py
--rw-r--r--   0        0        0    13747 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/unit/helpers/test_tuf.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/PKG-INFO
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.gitignore
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.readthedocs.yaml
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/LICENSE
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/MAINTAINERS.rst
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/Makefile
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/Pipfile
+-rw-r--r--   0        0        0    80650 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/Pipfile.lock
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/README.rst
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/pyproject.toml
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/requirements-dev.txt
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/requirements.txt
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tox.ini
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.github/ISSUE_TEMPLATE/other.yml
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.github/ISSUE_TEMPLATE/task.yml
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.github/PULL_REQUEST_TEMPLATE/pr.yml
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.github/workflows/cd.yml
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/.github/workflows/update-python-deps.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/make.bat
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/requirements.txt
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/diagrams/repository-service-tuf-cli-C1.puml
+-rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/diagrams/repository-service-tuf-cli-C2.puml
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/diagrams/repository-service-tuf-cli-C3.puml
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/conf.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/_static/INFO
+-rw-r--r--   0        0        0    19648 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/_static/repository-service-tuf-cli-C1.png
+-rw-r--r--   0        0        0    41916 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/_static/repository-service-tuf-cli-C2.png
+-rw-r--r--   0        0        0    94852 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/_static/repository-service-tuf-cli-C3.png
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/devel/design.rst
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/devel/index.rst
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/devel/modules.rst
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/devel/repository_service_tuf.cli.admin.rst
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/devel/repository_service_tuf.cli.key.rst
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/devel/repository_service_tuf.cli.rst
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/devel/repository_service_tuf.helpers.rst
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/devel/repository_service_tuf.rst
+-rw-r--r--   0        0        0    48362 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/docs/source/guide/index.rst
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/__version__.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/constants.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/cli/__init__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/cli/admin/__init__.py
+-rw-r--r--   0        0        0    25461 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/cli/admin/ceremony.py
+-rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/cli/admin/import_targets.py
+-rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/cli/admin/login.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/cli/admin/token.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/cli/key/__init__.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/cli/key/generate_key.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/helpers/__init__.py
+-rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/helpers/api_client.py
+-rw-r--r--   0        0        0     8014 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/repository_service_tuf/helpers/tuf.py
+-rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/conftest.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/test_tuf_repository_service.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/files/README.md
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/files/key_storage/JanisJoplin.key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/files/key_storage/JanisJoplin.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/files/key_storage/JimiHendrix.key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/files/key_storage/JimiHendrix.pub
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/files/key_storage/online-rsa.key
+-rwxr-xr-x   0        0        0      624 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/files/key_storage/online-rsa.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/files/key_storage/online.key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/files/key_storage/online.pub
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/unit/cli/test__init__.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/unit/cli/admin/__init__.py
+-rw-r--r--   0        0        0    32354 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/unit/cli/admin/test_ceremony.py
+-rw-r--r--   0        0        0    15993 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/unit/cli/admin/test_import_targets.py
+-rw-r--r--   0        0        0    12272 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/unit/cli/admin/test_login.py
+-rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/unit/cli/key/test_generate_key.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/unit/helpers/__init__.py
+-rw-r--r--   0        0        0    21413 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/unit/helpers/test_api_client.py
+-rw-r--r--   0        0        0    13747 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/tests/unit/helpers/test_tuf.py
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 repository_service_tuf-0.3.0a1/PKG-INFO
```

### Comparing `repository_service_tuf-0.1.2a1/.gitignore` & `repository_service_tuf-0.3.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/.pre-commit-config.yaml` & `repository_service_tuf-0.3.0a1/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     files: 'repository_service_tuf/'
   - id: check-yaml
     files: '.github/'
 - repo: https://github.com/pycqa/flake8
   rev: '6.0.0'
   hooks:
   - id: flake8
-    exclude: repository_service_tuf/__init__.py|venv|.venv|setting.py|.git|.tox|dist|docs|/*lib/python*|/*egg|build|tools
+    exclude: docs
 - repo: https://github.com/PyCQA/isort
   rev: '5.12.0'
   hooks:
   - id: isort
     args: [-l79, --profile, black, --check, --diff]
 - repo: https://github.com/psf/black
   rev: '22.12.0'
```

### Comparing `repository_service_tuf-0.1.2a1/.readthedocs.yaml` & `repository_service_tuf-0.3.0a1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/CODE_OF_CONDUCT.rst` & `repository_service_tuf-0.3.0a1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/CONTRIBUTING.rst` & `repository_service_tuf-0.3.0a1/CONTRIBUTING.rst`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 Development
 ===========
 
 Requirements
 -------------
 
-- Python >=3.8
+- Python >=3.9
 - Pipenv
 
 Getting the source code
 -----------------------
 
 `Fork <https://docs.github.com/en/get-started/quickstart/fork-a-repo>`_ the
 repository on `GitHub <https://github.com/repository-service-tuf/repository-service-tuf-cli>`_ and
```

### Comparing `repository_service_tuf-0.1.2a1/LICENSE` & `repository_service_tuf-0.3.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/Pipfile` & `repository_service_tuf-0.3.0a1/Pipfile`

 * *Files 1% similar despite different names*

```diff
@@ -38,8 +38,8 @@
 hatchling = "==0.22.0"
 build = "*"
 pre-commit = "*"
 bandit = "*"
 types-requests = "*"
 
 [requires]
-python_version = "3.8"
+python_version = "3.9"
```

### Comparing `repository_service_tuf-0.1.2a1/Pipfile.lock` & `repository_service_tuf-0.3.0a1/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975962709284627%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'cfa21df3cb514741120ccf93fa49e9082cb5dfa093cc161b508130e0418a0c32'}, 'requires': "*

 * *            "{'python_version': '3.9'}}",*

 * * "'default'": "{'sqlalchemy': {'hashes': "*

 * *              "['sha256:0aa2cbde85a6eab9263ab480f19e8882d022d30ebcdc14d69e6a8d7c07b0a871', "*

 * *              "'sha256:0d6979c9707f8b82366ba34b38b5a6fe32f75766b2e901f9820e271e95384070', "*

 * *              "'sha256:0eb14a386a5b610305bec6639b35540b47f408b0a59f75999199aed5b3d40079', "*

 * *              "'sha […]*

```diff
@@ -1,15 +1,15 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "458a229a12808fb1a4797d0fae298fbc85106e59e59b18d7887279e8e4412b2c"
+            "sha256": "cfa21df3cb514741120ccf93fa49e9082cb5dfa093cc161b508130e0418a0c32"
         },
         "pipfile-spec": 6,
         "requires": {
-            "python_version": "3.10"
+            "python_version": "3.9"
         },
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
@@ -414,58 +414,58 @@
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.16.0"
         },
         "sqlalchemy": {
             "hashes": [
-                "sha256:03206576ca53f55b9de6e890273e498f4b2e6e687a9db9859bdcd21df5a63e53",
-                "sha256:09205893a84b6bedae0453d3f384f5d2a6499b6e45ad977549894cdcd85d8f1c",
-                "sha256:0e5501c78b5ab917f0f0f75ce7f0018f683a0a76e95f30e6561bf61c9ff69d43",
-                "sha256:10f1ff0ebe21d2cea89ead231ba3ecf75678463ab85f19ce2ce91207620737f3",
-                "sha256:1fac17c866111283cbcdb7024d646abb71fdd95f3ce975cf3710258bc55742fd",
-                "sha256:297b752d4f30350b64175bbbd57dc94c061a35f5d1dba088d0a367dbbebabc94",
-                "sha256:2a3101252f3de9a18561c1fb0a68b1ee465485990aba458d4510f214bd5a582c",
-                "sha256:32762dba51b663609757f861584a722093487f53737e76474cc6e190904dc31b",
-                "sha256:369f6564e68a9c60f0b9dde121def491e651a4ba8dcdd652a93f1cd5977cd85c",
-                "sha256:3745dee26a7ee012598577ad3b8f6e6cd50a49b2afa0cde9db668da6bf2c2319",
-                "sha256:3c053c3f4c4e45d4c8b27977647566c140d6de3f61a4e2acb92ea24cf9911c7f",
-                "sha256:4ad525b9dd17b478a2ed8580d7f2bc46b0f5889153c6b1c099729583e395b4b9",
-                "sha256:53b2c8adbcbb59732fb21a024aaa261983655845d86e3fc26a5676cec0ebaa09",
-                "sha256:5d709f43caee115b03b707b8cbbcb8b303045dd7cdc825b6d29857d71f3425ae",
-                "sha256:5e9d390727c11b9a7e583bf6770de36895c0936bddb98ae93ae99282e6428d5f",
-                "sha256:6b1fa0ffc378a7061c452cb4a1f804fad1b3b8aa8d0552725531d27941b2e3ed",
-                "sha256:6e1d50592cb24d1947c374c666add65ded7c181ec98a89ed17abbe9b8b2e2ff4",
-                "sha256:77a06b0983faf9aa48ee6219d41ade39dee16ce90857cc181dbcf6918acd234d",
-                "sha256:7eb25b981cbc9e7df9f56ad7ec4c6d77323090ca4b7147fcdc09d66535377759",
-                "sha256:85b0efe1c71459ba435a6593f54a0e39334b16ba383e8010fdb9d0127ca51ba8",
-                "sha256:87b2c2d13c3d1384859b60eabb3139e169ce68ada1d2963dbd0c7af797f16efe",
-                "sha256:8aad66215a3817a7a1d535769773333250de2653c89b53f7e2d42b677d398027",
-                "sha256:91f4b1bdc987ef85fe3a0ce5d26ac72ff8f60207b08272aa2a65494836391d69",
-                "sha256:978bee4ecbcdadf087220618409fb9be9509458df479528b70308f0599c7c519",
-                "sha256:9fe98e9d26778d7711ceee2c671741b4f54c74677668481d733d6f70747d7690",
-                "sha256:a022c588c0f413f8cddf9fcc597dbf317efeac4186d8bff9aa7f3219258348b0",
-                "sha256:a4709457f1c317e347051498b91fa2b86c4bcdebf93c84e6d121a4fc8a397307",
-                "sha256:aec5fb36b53125554ecc2285526eb5cc31b21f6cb059993c1c5ca831959de052",
-                "sha256:b6ceca432ce88ad12aab5b5896c343a1993c90b325d9193dcd055e73e18a0439",
-                "sha256:b76c2fde827522e21922418325c1b95c2d795cdecfb4bc261e4d37965199ee7f",
-                "sha256:bddfc5bd1dee5db0fddc9dab26f800c283f3243e7281bbf107200fed30125f9c",
-                "sha256:bf83700faa9642388fbd3167db3f6cbb2e88cc8367b8c22204f3f408ee782d25",
-                "sha256:c5268ec05c21e2ecf5bca09314bcaadfec01f02163088cd602db4379862958dd",
-                "sha256:d9796d5c13b2b7f05084d0ce52528cf919f9bde9e0f10672a6393a4490415695",
-                "sha256:dc67efd00ce7f428a446ce012673c03c63c5abb5dec3f33750087b8bdc173bf0",
-                "sha256:dfd6385b662aea83e63dd4db5fe116eb11914022deb1745f0b57fa8470c18ffe",
-                "sha256:e495ad05a13171fbb5d72fe5993469c8bceac42bcf6b8f9f117a518ee7fbc353",
-                "sha256:e752c34f7a2057ebe82c856698b9f277c633d4aad006bddf7af74598567c8931",
-                "sha256:f0843132168b44ca33c5e5a2046c954775dde8c580ce27f5cf2e134d0d9919e4",
-                "sha256:f30c5608c64fc9c1fa9a16277eb4784f782362566fe40ff8d283358c8f2c5fe0",
-                "sha256:f6ebadefc4331dda83c22519e1ea1e61104df6eb38abbb80ab91b0a8527a5c19"
+                "sha256:0aa2cbde85a6eab9263ab480f19e8882d022d30ebcdc14d69e6a8d7c07b0a871",
+                "sha256:0d6979c9707f8b82366ba34b38b5a6fe32f75766b2e901f9820e271e95384070",
+                "sha256:0eb14a386a5b610305bec6639b35540b47f408b0a59f75999199aed5b3d40079",
+                "sha256:2424a84f131901fbb20a99844d47b38b517174c6e964c8efb15ea6bb9ced8c2b",
+                "sha256:2ad9688debf1f0ae9c6e0706a4e2d33b1a01281317cee9bd1d7eef8020c5baac",
+                "sha256:2f0a355264af0952570f18457102984e1f79510f856e5e0ae652e63316d1ca23",
+                "sha256:31f72bb300eed7bfdb373c7c046121d84fa0ae6f383089db9505ff553ac27cef",
+                "sha256:375b7ba88f261dbd79d044f20cbcd919d88befb63f26af9d084614f10cdf97a6",
+                "sha256:37de4010f53f452e94e5ed6684480432cfe6a7a8914307ef819cd028b05b98d5",
+                "sha256:49c138856035cb97f0053e5e57ba90ec936b28a0b8b0020d44965c7b0c0bf03a",
+                "sha256:4f9832815257969b3ca9bf0501351e4c02c8d60cbd3ec9f9070d5b0f8852900e",
+                "sha256:566a0ac347cf4632f551e7b28bbd0d215af82e6ffaa2556f565a3b6b51dc3f81",
+                "sha256:6777673d346071451bf7cccf8d0499024f1bd6a835fc90b4fe7af50373d92ce6",
+                "sha256:72746ec17a7d9c5acf2c57a6e6190ceba3dad7127cd85bb17f24e90acc0e8e3f",
+                "sha256:755f653d693f9b8f4286d987aec0d4279821bf8d179a9de8e8a5c685e77e57d6",
+                "sha256:7612a7366a0855a04430363fb4ab392dc6818aaece0b2e325ff30ee77af9b21f",
+                "sha256:7ad24c85f2a1caf0cd1ae8c2fdb668777a51a02246d9039420f94bd7dbfd37ed",
+                "sha256:881cc388dded44ae6e17a1666364b98bd76bcdc71b869014ae725f06ba298e0e",
+                "sha256:8d97b37b4e60073c38bcf94e289e3be09ef9be870de88d163f16e08f2b9ded1a",
+                "sha256:9119795d2405eb23bf7e6707e228fe38124df029494c1b3576459aa3202ea432",
+                "sha256:9136d596111c742d061c0f99bab95c5370016c4101a32e72c2b634ad5e0757e6",
+                "sha256:9ad883ac4f5225999747f0849643c4d0ec809d9ffe0ddc81a81dd3e68d0af463",
+                "sha256:a25b4c4fdd633501233924f873e6f6cd8970732859ecfe4ecfb60635881f70be",
+                "sha256:a30e4db983faa5145e00ef6eaf894a2d503b3221dbf40a595f3011930d3d0bac",
+                "sha256:a5e9e78332a5d841422b88b8c490dfd7f761e64b3430249b66c05d02f72ceab0",
+                "sha256:b4e08e3831671008888bad5d160d757ef35ce34dbb73b78c3998d16aa1334c97",
+                "sha256:bf1aae95e80acea02a0a622e1c12d3fefc52ffd0fe7bda70a30d070373fbb6c3",
+                "sha256:c61b89803a87a3b2a394089a7dadb79a6c64c89f2e8930cc187fec43b319f8d2",
+                "sha256:cdf80359b641185ae7e580afb9f88cf560298f309a38182972091165bfe1225d",
+                "sha256:d93ebbff3dcf05274843ad8cf650b48ee634626e752c5d73614e5ec9df45f0ce",
+                "sha256:db24d2738add6db19d66ca820479d2f8f96d3f5a13c223f27fa28dd2f268a4bd",
+                "sha256:e0d20f27edfd6f35b388da2bdcd7769e4ffa374fef8994980ced26eb287e033a",
+                "sha256:e2f3b5236079bc3e318a92bab2cc3f669cc32127075ab03ff61cacbae1c392b8",
+                "sha256:e481e54db8cec1457ee7c05f6d2329e3298a304a70d3b5e2e82e77170850b385",
+                "sha256:e5e5dc300a0ca8755ada1569f5caccfcdca28607dfb98b86a54996b288a8ebd3",
+                "sha256:ec2f525273528425ed2f51861b7b88955160cb95dddb17af0914077040aff4a5",
+                "sha256:f234ba3bb339ad17803009c8251f5ee65dcf283a380817fe486823b08b26383d",
+                "sha256:f463598f9e51ccc04f0fe08500f9a0c3251a7086765350be418598b753b5561d",
+                "sha256:f717944aee40e9f48776cf85b523bb376aa2d9255a268d6d643c57ab387e7264",
+                "sha256:fd0febae872a4042da44e972c070f0fd49a85a0a7727ab6b85425f74348be14e",
+                "sha256:fec56c7d1b6a22c8f01557de3975d962ee40270b81b60d1cfdadf2a105d10e84"
             ],
             "index": "pypi",
-            "version": "==2.0.12"
+            "version": "==2.0.13"
         },
         "tuf": {
             "hashes": [
                 "sha256:1524b0fbd8504245f600f121daf86b8fdcb30df74410acc9655944c4868e461c",
                 "sha256:76e7f2a7aced84466865fac2a7127b6085afae51d4328af896fb46f952dd3a53"
             ],
             "index": "pypi",
@@ -935,59 +935,59 @@
                 "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.1.2"
         },
         "mypy": {
             "hashes": [
-                "sha256:023fe9e618182ca6317ae89833ba422c411469156b690fde6a315ad10695a521",
-                "sha256:031fc69c9a7e12bcc5660b74122ed84b3f1c505e762cc4296884096c6d8ee140",
-                "sha256:2de7babe398cb7a85ac7f1fd5c42f396c215ab3eff731b4d761d68d0f6a80f48",
-                "sha256:2e93a8a553e0394b26c4ca683923b85a69f7ccdc0139e6acd1354cc884fe0128",
-                "sha256:390bc685ec209ada4e9d35068ac6988c60160b2b703072d2850457b62499e336",
-                "sha256:3a2d219775a120581a0ae8ca392b31f238d452729adbcb6892fa89688cb8306a",
-                "sha256:3efde4af6f2d3ccf58ae825495dbb8d74abd6d176ee686ce2ab19bd025273f41",
-                "sha256:4a99fe1768925e4a139aace8f3fb66db3576ee1c30b9c0f70f744ead7e329c9f",
-                "sha256:4b41412df69ec06ab141808d12e0bf2823717b1c363bd77b4c0820feaa37249e",
-                "sha256:4c8d8c6b80aa4a1689f2a179d31d86ae1367ea4a12855cc13aa3ba24bb36b2d8",
-                "sha256:4d19f1a239d59f10fdc31263d48b7937c585810288376671eaf75380b074f238",
-                "sha256:4e4a682b3f2489d218751981639cffc4e281d548f9d517addfd5a2917ac78119",
-                "sha256:695c45cea7e8abb6f088a34a6034b1d273122e5530aeebb9c09626cea6dca4cb",
-                "sha256:701189408b460a2ff42b984e6bd45c3f41f0ac9f5f58b8873bbedc511900086d",
-                "sha256:70894c5345bea98321a2fe84df35f43ee7bb0feec117a71420c60459fc3e1eed",
-                "sha256:8293a216e902ac12779eb7a08f2bc39ec6c878d7c6025aa59464e0c4c16f7eb9",
-                "sha256:8d26b513225ffd3eacece727f4387bdce6469192ef029ca9dd469940158bc89e",
-                "sha256:a197ad3a774f8e74f21e428f0de7f60ad26a8d23437b69638aac2764d1e06a6a",
-                "sha256:bea55fc25b96c53affab852ad94bf111a3083bc1d8b0c76a61dd101d8a388cf5",
-                "sha256:c9a084bce1061e55cdc0493a2ad890375af359c766b8ac311ac8120d3a472950",
-                "sha256:d0e9464a0af6715852267bf29c9553e4555b61f5904a4fc538547a4d67617937",
-                "sha256:d8e9187bfcd5ffedbe87403195e1fc340189a68463903c39e2b63307c9fa0394",
-                "sha256:eaeaa0888b7f3ccb7bcd40b50497ca30923dba14f385bde4af78fac713d6d6f6",
-                "sha256:f46af8d162f3d470d8ffc997aaf7a269996d205f9d746124a179d3abe05ac602",
-                "sha256:f70a40410d774ae23fcb4afbbeca652905a04de7948eaf0b1789c8d1426b72d1",
-                "sha256:fe91be1c51c90e2afe6827601ca14353bbf3953f343c2129fa1e247d55fd95ba"
+                "sha256:1c4c42c60a8103ead4c1c060ac3cdd3ff01e18fddce6f1016e08939647a0e703",
+                "sha256:44797d031a41516fcf5cbfa652265bb994e53e51994c1bd649ffcd0c3a7eccbf",
+                "sha256:473117e310febe632ddf10e745a355714e771ffe534f06db40702775056614c4",
+                "sha256:4c99c3ecf223cf2952638da9cd82793d8f3c0c5fa8b6ae2b2d9ed1e1ff51ba85",
+                "sha256:550a8b3a19bb6589679a7c3c31f64312e7ff482a816c96e0cecec9ad3a7564dd",
+                "sha256:658fe7b674769a0770d4b26cb4d6f005e88a442fe82446f020be8e5f5efb2fae",
+                "sha256:6e33bb8b2613614a33dff70565f4c803f889ebd2f859466e42b46e1df76018dd",
+                "sha256:6e42d29e324cdda61daaec2336c42512e59c7c375340bd202efa1fe0f7b8f8ca",
+                "sha256:74bc9b6e0e79808bf8678d7678b2ae3736ea72d56eede3820bd3849823e7f305",
+                "sha256:76ec771e2342f1b558c36d49900dfe81d140361dd0d2df6cd71b3db1be155409",
+                "sha256:7d23370d2a6b7a71dc65d1266f9a34e4cde9e8e21511322415db4b26f46f6b8c",
+                "sha256:87df44954c31d86df96c8bd6e80dfcd773473e877ac6176a8e29898bfb3501cb",
+                "sha256:8c5979d0deb27e0f4479bee18ea0f83732a893e81b78e62e2dda3e7e518c92ee",
+                "sha256:95d8d31a7713510685b05fbb18d6ac287a56c8f6554d88c19e73f724a445448a",
+                "sha256:a22435632710a4fcf8acf86cbd0d69f68ac389a3892cb23fbad176d1cddaf228",
+                "sha256:a8763e72d5d9574d45ce5881962bc8e9046bf7b375b0abf031f3e6811732a897",
+                "sha256:c1eb485cea53f4f5284e5baf92902cd0088b24984f4209e25981cc359d64448d",
+                "sha256:c5d2cc54175bab47011b09688b418db71403aefad07cbcd62d44010543fc143f",
+                "sha256:cbc07246253b9e3d7d74c9ff948cd0fd7a71afcc2b77c7f0a59c26e9395cb152",
+                "sha256:d0b6c62206e04061e27009481cb0ec966f7d6172b5b936f3ead3d74f29fe3dcf",
+                "sha256:ddae0f39ca146972ff6bb4399f3b2943884a774b8771ea0a8f50e971f5ea5ba8",
+                "sha256:e1f4d16e296f5135624b34e8fb741eb0eadedca90862405b1f1fde2040b9bd11",
+                "sha256:e86c2c6852f62f8f2b24cb7a613ebe8e0c7dc1402c61d36a609174f63e0ff017",
+                "sha256:ebc95f8386314272bbc817026f8ce8f4f0d2ef7ae44f947c4664efac9adec929",
+                "sha256:f9dca1e257d4cc129517779226753dbefb4f2266c4eaad610fc15c6a7e14283e",
+                "sha256:faff86aa10c1aa4a10e1a301de160f3d8fc8703b88c7e98de46b531ff1276a9a"
             ],
             "index": "pypi",
-            "version": "==1.2.0"
+            "version": "==1.3.0"
         },
         "mypy-extensions": {
             "hashes": [
                 "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
                 "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.0"
         },
         "nodeenv": {
             "hashes": [
-                "sha256:27083a7b96a25f2f5e1d8cb4b6317ee8aeda3bdd121394e5ac54e498028a042e",
-                "sha256:e0e7f7dfb85fc5394c6fe1e8fa98131a2473e04311a45afb6508f7cf1836fa2b"
+                "sha256:d51e0c37e64fbf47d017feac3145cdbb58836d7eee8c6f6d3b6880c5456227d2",
+                "sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
-            "version": "==1.7.0"
+            "version": "==1.8.0"
         },
         "packaging": {
             "hashes": [
                 "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
                 "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.1'",
@@ -1015,19 +1015,19 @@
                 "sha256:3ef6ac33239e4027d9a5598a381b9d30880a1477e50039db2eac6e8a8f6d1b18"
             ],
             "index": "pypi",
             "version": "==23.1.2"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:47692bc24c1958e8b0f13dd727307cff1db103fca36399f457da8e05f222fdc4",
-                "sha256:7954a68d0ba23558d753f73437c55f89027cf8f5108c19844d4b82e5af396335"
+                "sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f",
+                "sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.5.0"
+            "version": "==3.5.1"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.1'",
@@ -1259,19 +1259,19 @@
                 "sha256:aa5f6de5dfdf809ef505c4895e51ef5c9eac17d0f287933eb49ec495280b6952"
             ],
             "index": "pypi",
             "version": "==1.1.5"
         },
         "stevedore": {
             "hashes": [
-                "sha256:2c428d2338976279e8eb2196f7a94910960d9f7ba2f41f3988511e95ca447021",
-                "sha256:bd5a71ff5e5e5f5ea983880e4a1dd1bb47f8feebbb3d95b592398e2f02194771"
+                "sha256:8cc040628f3cea5d7128f2e76cf486b2251a4e543c7b938f58d9a377f6694a2d",
+                "sha256:a54534acf9b89bc7ed264807013b505bf07f74dbe4bcfa37d32bd063870b087c"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==5.0.0"
+            "version": "==5.1.0"
         },
         "tomli": {
             "hashes": [
                 "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version >= '3.1'",
@@ -1291,18 +1291,18 @@
                 "sha256:dec781054324a70ba64430ae9e62e7e9c8e4618c185a5cb3f87a6738251b5a31"
             ],
             "index": "pypi",
             "version": "==2.30.0.0"
         },
         "types-urllib3": {
             "hashes": [
-                "sha256:3ba3d3a8ee46e0d5512c6bd0594da4f10b2584b47a470f8422044a2ab462f1df",
-                "sha256:a1557355ce8d350a555d142589f3001903757d2d36c18a66f588d9659bbc917d"
+                "sha256:3300538c9dc11dad32eae4827ac313f5d986b8b21494801f1bf97a1ac6c03ae5",
+                "sha256:5dbd1d2bef14efee43f5318b5d36d805a489f6600252bb53626d4bfafd95e27c"
             ],
-            "version": "==1.26.25.12"
+            "version": "==1.26.25.13"
         },
         "typing-extensions": {
             "hashes": [
                 "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
                 "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version >= '3.7'",
```

### Comparing `repository_service_tuf-0.1.2a1/README.rst` & `repository_service_tuf-0.3.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/pyproject.toml` & `repository_service_tuf-0.3.0a1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 requires = ["hatchling==0.22.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "repository-service-tuf"
 description = 'Repository Service for TUF Command Line Interface'
 readme = "README.rst"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = { text = "MIT"}
 keywords = []
 authors = [
   { name = "Kairo de Araujo", email = "kairo@dearaujo.nl" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
```

### Comparing `repository_service_tuf-0.1.2a1/requirements-dev.txt` & `repository_service_tuf-0.3.0a1/requirements-dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,22 +27,22 @@
 iniconfig==2.0.0 ; python_version >= '3.7'
 isort==5.12.0
 jinja2==3.1.2 ; python_version >= '3.7'
 markdown-it-py==2.2.0 ; python_version >= '3.7'
 markupsafe==2.1.2 ; python_version >= '3.7'
 mccabe==0.7.0 ; python_version >= '3.6'
 mdurl==0.1.2 ; python_version >= '3.7'
-mypy==1.2.0
+mypy==1.3.0
 mypy-extensions==1.0.0 ; python_version >= '3.5'
-nodeenv==1.7.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'
+nodeenv==1.8.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'
 packaging==23.1 ; python_version >= '3.1'
 pathspec==0.11.1 ; python_version >= '3.7'
 pbr==5.11.1 ; python_version >= '2.6'
 pip==23.1.2
-platformdirs==3.5.0 ; python_version >= '3.7'
+platformdirs==3.5.1 ; python_version >= '3.7'
 pluggy==1.0.0 ; python_version >= '3.1'
 pre-commit==3.3.1
 pretend==1.0.9
 pycodestyle==2.10.0 ; python_version >= '3.6'
 pyflakes==3.0.1 ; python_version >= '3.6'
 pygments==2.15.1 ; python_version >= '3.7'
 pyproject-api==1.5.1 ; python_version >= '3.7'
@@ -60,28 +60,28 @@
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jquery==4.1 ; python_version >= '3.1'
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-plantuml==0.25
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
-stevedore==5.0.0 ; python_version >= '3.8'
+stevedore==5.1.0 ; python_version >= '3.8'
 tomli==2.0.1 ; python_version >= '3.1'
 tox==4.5.1
 types-requests==2.30.0.0
-types-urllib3==1.26.25.12
+types-urllib3==1.26.25.13
 typing-extensions==4.5.0 ; python_version >= '3.7'
 urllib3==2.0.2 ; python_version >= '3.7'
 virtualenv==20.23.0 ; python_version >= '3.7'
 cffi==1.15.1
 configobj==5.0.8
 cryptography==40.0.2
 dynaconf[ini]==3.1.12
 greenlet==2.0.2 ; platform_machine == 'aarch64' or (platform_machine == 'ppc64le' or (platform_machine == 'x86_64' or (platform_machine == 'amd64' or (platform_machine == 'AMD64' or (platform_machine == 'win32' or platform_machine == 'WIN32')))))
 psycopg2==2.9.6
 pycparser==2.21
 pynacl==1.5.0
 rich-click==1.6.1
 securesystemslib[crypto]==0.28.0
 six==1.16.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
-sqlalchemy==2.0.12
+sqlalchemy==2.0.13
 tuf==2.0.0
```

### Comparing `repository_service_tuf-0.1.2a1/requirements.txt` & `repository_service_tuf-0.3.0a1/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -16,11 +16,11 @@
 pygments==2.15.1 ; python_version >= '3.7'
 pynacl==1.5.0
 requests==2.30.0
 rich==13.3.5
 rich-click==1.6.1
 securesystemslib[crypto]==0.28.0
 six==1.16.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
-sqlalchemy==2.0.12
+sqlalchemy==2.0.13
 tuf==2.0.0
 typing-extensions==4.5.0 ; python_version >= '3.7'
 urllib3==2.0.2 ; python_version >= '3.7'
```

### Comparing `repository_service_tuf-0.1.2a1/tox.ini` & `repository_service_tuf-0.3.0a1/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 [tox]
 isolated_build = true
-envlist = py38,py39,py310,py311,lint,typing,requirements,test
+envlist = py39,py310,py311,lint,typing,requirements,test
 skipsdist = true
 
-
-[flake8]
-exclude = repository_service_tuf/__init__.py,venv,.venv,settings.py,.git,.tox,dist,docs,*lib/python*,*egg,build,tools
-
 [testenv]
 deps = -r{toxinidir}/requirements.txt
        -r{toxinidir}/requirements-dev.txt
 
 [testenv:lint]
 deps = pre-commit
 commands =
@@ -50,11 +46,10 @@
 commands =
     plantuml -o ../source/_static/ -tpng docs/diagrams/*.puml
 	sphinx-apidoc -o  docs/source/devel/ repository_service_tuf
 	sphinx-build -E -W -b html docs/source docs/build/html
 
 [gh-actions]
 python =
-    3.8: py38,pep8,lint,typing,requirements,test,docs
     3.9: py39,pep8,lint,typing,requirements,test,docs
     3.10: py310,pep8,lint,typing,requirements,test,docs
     3.11: py311,pep8,lint,typing,requirements,test,docs
```

### Comparing `repository_service_tuf-0.1.2a1/.github/ISSUE_TEMPLATE/bug.yml` & `repository_service_tuf-0.3.0a1/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/.github/ISSUE_TEMPLATE/other.yml` & `repository_service_tuf-0.3.0a1/.github/ISSUE_TEMPLATE/other.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/.github/ISSUE_TEMPLATE/task.yml` & `repository_service_tuf-0.3.0a1/.github/ISSUE_TEMPLATE/task.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/.github/PULL_REQUEST_TEMPLATE/pr.yml` & `repository_service_tuf-0.3.0a1/.github/PULL_REQUEST_TEMPLATE/pr.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/.github/workflows/cd.yml` & `repository_service_tuf-0.3.0a1/.github/workflows/cd.yml`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 jobs:
   functional-latest:
     uses: repository-service-tuf/repository-service-tuf/.github/workflows/functional.yml@main
     with:
       worker_version: latest
       api_version: latest
       cli_version: dev
+    secrets:
+      RSTUF_ONLINE_KEY: ${{ secrets.RSTUF_ONLINE_KEY }}
 
   build:
     name: Build
     runs-on: ubuntu-latest
     needs: functional-latest
     outputs:
       release_id: ${{ steps.gh-release.outputs.id }}
```

### Comparing `repository_service_tuf-0.1.2a1/.github/workflows/ci.yml` & `repository_service_tuf-0.3.0a1/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
       - "main"
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-versions: [ "3.10", "3.11" ]
+        python-versions: [ "3.9", "3.10", "3.11" ]
 
     steps:
     - uses: actions/checkout@8e5e7e5ab8b370d6c329ec480221332ada57f0ab
     - uses: actions/setup-python@57ded4d7d5e986d7296eab16560982c6dd7c923b
       with:
         python-version: ${{ matrix.python-versions }}
 
@@ -29,12 +29,12 @@
     - name: Test Build binary wheel and source tarball
       run: python3 -m build --sdist --wheel --outdir dist/ .
 
     - name: Run Python tests
       run: make tests
 
     - name: Codecov
-      uses: codecov/codecov-action@894ff025c7b54547a9a2a1e9f228beae737ad3c2
+      uses: codecov/codecov-action@eaaf4bedf32dbdc6b720b63067d99c4d77d6047d
       with:
         files: coverage.xml
         fail_ci_if_error: false
         verbose: true
```

### Comparing `repository_service_tuf-0.1.2a1/.github/workflows/update-python-deps.yml` & `repository_service_tuf-0.3.0a1/.github/workflows/update-python-deps.yml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   schedule:
     - cron: "0 8 * * *"
 jobs:
   update-dep:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-versions: ["3.10"]
+        python-versions: [ "3.9", "3.10", "3.11"]
     steps:
       - uses: actions/checkout@8e5e7e5ab8b370d6c329ec480221332ada57f0ab
       - uses: actions/setup-python@57ded4d7d5e986d7296eab16560982c6dd7c923b
         with:
           python-version: ${{ matrix.python-versions }}
       - name: Install prerequisites
         run: |
```

### Comparing `repository_service_tuf-0.1.2a1/docs/Makefile` & `repository_service_tuf-0.3.0a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/docs/make.bat` & `repository_service_tuf-0.3.0a1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/docs/diagrams/repository-service-tuf-cli-C1.puml` & `repository_service_tuf-0.3.0a1/docs/diagrams/repository-service-tuf-cli-C1.puml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/docs/diagrams/repository-service-tuf-cli-C2.puml` & `repository_service_tuf-0.3.0a1/docs/diagrams/repository-service-tuf-cli-C2.puml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/docs/diagrams/repository-service-tuf-cli-C3.puml` & `repository_service_tuf-0.3.0a1/docs/diagrams/repository-service-tuf-cli-C3.puml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/docs/source/conf.py` & `repository_service_tuf-0.3.0a1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/docs/source/_static/repository-service-tuf-cli-C1.png` & `repository_service_tuf-0.3.0a1/docs/source/_static/repository-service-tuf-cli-C1.png`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/docs/source/_static/repository-service-tuf-cli-C2.png` & `repository_service_tuf-0.3.0a1/docs/source/_static/repository-service-tuf-cli-C2.png`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/docs/source/_static/repository-service-tuf-cli-C3.png` & `repository_service_tuf-0.3.0a1/docs/source/_static/repository-service-tuf-cli-C3.png`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/docs/source/devel/design.rst` & `repository_service_tuf-0.3.0a1/docs/source/devel/design.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/docs/source/devel/repository_service_tuf.cli.admin.rst` & `repository_service_tuf-0.3.0a1/docs/source/devel/repository_service_tuf.cli.admin.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/docs/source/devel/repository_service_tuf.helpers.rst` & `repository_service_tuf-0.3.0a1/docs/source/devel/repository_service_tuf.helpers.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/docs/source/guide/index.rst` & `repository_service_tuf-0.3.0a1/docs/source/guide/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -18,24 +18,24 @@
 
     ❯ rstuf
 
     Usage: rstuf [OPTIONS] COMMAND [ARGS]...
 
     Repository Service for TUF Command Line Interface (CLI).
 
-    ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-    │ --config   -c  TEXT  Repository Service for TUF config file                                                                      │
-    │ --no-auth            Skips the use of RSTUF built-in authentication.                                                             │
-    │ --version            Show the version and exit.                                                                                  │
-    │ --help     -h        Show this message and exit.                                                                                 │
-    ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-    ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-    │ admin                      Administrative Commands                                                                               │
-    │ key                        Cryptographic Key Commands                                                                            │
-    ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+    ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+    │ --config   -c  TEXT  Repository Service for TUF config file.                                                                                                                                                                 │
+    │ --auth               Use of RSTUF built-in authentication.                                                                                                                                                                   │
+    │ --version            Show the version and exit.                                                                                                                                                                              │
+    │ --help     -h        Show this message and exit.                                                                                                                                                                             │
+    ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+    ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+    │ admin                                    Administrative Commands                                                                                                                                                             │
+    │ key                                      Cryptographic Key Commands                                                                                                                                                          │
+    ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 
 .. rstuf-cli-admin
 
 Administration (``admin``)
 ==========================
 
 It executes administrative commands to the Repository Service for TUF.
@@ -44,29 +44,30 @@
 
     ❯ rstuf admin
 
     Usage: rstuf admin [OPTIONS] COMMAND [ARGS]...
 
     Administrative Commands
 
-    ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-    │ --help  -h    Show this message and exit.                                                                                        │
-    ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-    ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-    │ ceremony                        Start a new Metadata Ceremony.                                                                   │
-    │ import-targets                  Import targets to RSTUF from exported CSV file.                                                  │
-    │ login                           Login to Repository Service for TUF (API).                                                       │
-    │ token                           Token Management.                                                                                │
-    ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+    ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+    │ --help  -h    Show this message and exit.                                                                                                                                                                                    │
+    ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+    ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+    │ ceremony                                              Start a new Metadata Ceremony.                                                                                                                                         │
+    │ import-targets                                        Import targets to RSTUF from exported CSV file.                                                                                                                        │
+    ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 
 .. rstuf-cli-admin-login
 
 Login to Server (``login``)
 ---------------------------
 
+.. note::
+    requires ``--auth``
+
 This command will log in to Repository Service for TUF and give you a token to run other commands
 such as Ceremony, Token Generation, etc.
 
 .. code:: shell
 
     ❯ rstuf admin login
     ╔══════════════════════════════════════════════════════════════════════════════════════╗
@@ -382,14 +383,17 @@
 .. rstuf-cli-admin-token
 
 Token (``token``)
 -----------------
 
 Token Management
 
+.. note::
+    requires ``--auth``
+
 .. code::
 
     ❯ rstuf admin token
 
     Usage: rstuf admin token [OPTIONS] COMMAND [ARGS]...
 
     Token Management.
```

### Comparing `repository_service_tuf-0.1.2a1/repository_service_tuf/constants.py` & `repository_service_tuf-0.3.0a1/repository_service_tuf/constants.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/repository_service_tuf/cli/__init__.py` & `repository_service_tuf-0.3.0a1/repository_service_tuf/cli/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,19 +40,19 @@
     "--config",
     "config",
     default=os.path.join(HOME, ".rstuf.ini"),
     help="Repository Service for TUF config file.",
     required=False,
 )
 @click.option(
-    "--no-auth",
+    "--auth",
     "auth",
-    help="Skips the use of RSTUF built-in authentication.",
+    help="Use of RSTUF built-in authentication.",
     is_flag=True,
-    default=True,
+    default=False,
     required=False,
 )
 # adds the --version parameter
 @click.version_option(prog_name=prog_name, version=version)
 @click.pass_context
 def rstuf(context, config, auth):
     """
@@ -60,18 +60,18 @@
     """
     context.obj = {
         "settings": Dynaconf(settings_files=[config]),
         "config": config,
         "auth": auth,
     }
     settings = context.obj["settings"]
-    if auth is False:
+    if auth is True:
         console.print(
             Panel(
-                "[white]Skipping RSTUF authentication (--no-auth)[/]",
+                "[white]Using RSTUF built-in authentication (--auth)[/]",
                 title="[green]Info[/]",
                 title_align="left",
                 style="green",
             )
         )
     settings.AUTH = auth
 
@@ -80,11 +80,11 @@
 groups_required_auth = [
     "repository_service_tuf.cli.admin.token",
     "repository_service_tuf.cli.admin.login",
 ]
 for _, name, _ in pkgutil.walk_packages(  # type: ignore
     __path__, prefix=__name__ + "."
 ):
-    if name in groups_required_auth and "--no-auth" in sys.argv:
+    if name in groups_required_auth and "--auth" not in sys.argv:
         continue
     else:
         importlib.import_module(name)
```

### Comparing `repository_service_tuf-0.1.2a1/repository_service_tuf/cli/admin/ceremony.py` & `repository_service_tuf-0.3.0a1/repository_service_tuf/cli/admin/ceremony.py`

 * *Files 0% similar despite different names*

```diff
@@ -735,17 +735,17 @@
 
     # option upload: it requires -b/--bootstrap
     if upload is True and bootstrap is False:
         raise click.ClickException("Requires '-b/--bootstrap' option.")
 
     # option bootstrap: checks if the server accepts it beforehand
     if bootstrap:
-        if settings.AUTH is False and upload_server is None:
+        if settings.AUTH is True and upload_server is None:
             raise click.ClickException(
-                "Requires '--upload-server' when using '--no-auth'. "
+                "Requires '--upload-server' when using '--auth'. "
                 "Example: --upload-server https://rstuf-api.example.com"
             )
         elif upload_server:
             settings.SERVER = upload_server
 
         bs_status = bootstrap_status(settings)
         if bs_status.get("data", {}).get("bootstrap") is True:
```

### Comparing `repository_service_tuf-0.1.2a1/repository_service_tuf/cli/admin/import_targets.py` & `repository_service_tuf-0.3.0a1/repository_service_tuf/cli/admin/import_targets.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/repository_service_tuf/cli/admin/login.py` & `repository_service_tuf-0.3.0a1/repository_service_tuf/cli/admin/login.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/repository_service_tuf/cli/admin/token.py` & `repository_service_tuf-0.3.0a1/repository_service_tuf/cli/admin/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 @click.pass_context
 def token(context):
     """
     Token Management.
     """
     settings = context.obj.get("settings")
     if settings.get("AUTH") is False:
-        console.print("[INFO] admin token is disabled with `--no-auth`")
+        console.print("[INFO] admin token is disabled, use `--auth`")
         raise click.Abort()
 
 
 @token.command()
 @click.option(
     "-e",
     "--expires",
@@ -50,15 +50,15 @@
     Generate new token.
     """
     settings = context.obj.get("settings")
     server = settings.get("SERVER")
     logged_token = settings.get("TOKEN")
     login = is_logged(settings)
     if login.state is False:
-        raise click.ClickException("Not logged. Use 'rstuf-cli admin login'")
+        raise click.ClickException("Not logged. Use 'rstuf admin login'")
 
     headers = {"Authorization": f"Bearer {logged_token}"}
     payload = {"scopes": list(scope), "expires": expires}
     response = request_server(
         server,
         f"{URL.token.value}new/",
         Methods.post,
@@ -84,15 +84,15 @@
     "Show token information details."
 
     settings = context.obj.get("settings")
     server = settings.get("SERVER")
     logged_token = settings.get("TOKEN")
     login = is_logged(settings)
     if login.state is False:
-        raise click.ClickException("Not logged. Use 'rstuf-cli admin login'")
+        raise click.ClickException("Not logged. Use 'rstuf admin login'")
 
     headers = {"Authorization": f"Bearer {logged_token}"}
     response = request_server(
         server,
         f"{URL.token.value}?token={token}",
         Methods.get,
         headers=headers,
```

### Comparing `repository_service_tuf-0.1.2a1/repository_service_tuf/cli/key/generate_key.py` & `repository_service_tuf-0.3.0a1/repository_service_tuf/cli/key/generate_key.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/repository_service_tuf/helpers/api_client.py` & `repository_service_tuf-0.3.0a1/repository_service_tuf/helpers/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 def is_logged(settings: LazySettings):
     if settings.get("AUTH") is False:
         return None
 
     token = settings.get("TOKEN")
     server = settings.get("SERVER")
     headers = {"Authorization": f"Bearer {token}"}
+
     url = f"{URL.token.value}?token={token}"
     response = request_server(server, url, Methods.get, headers=headers)
     if response.status_code == 401 or response.status_code == 403:
         return Login(state=False)
 
     elif response.status_code == 200:
         data = response.json().get("data", {})
```

### Comparing `repository_service_tuf-0.1.2a1/repository_service_tuf/helpers/tuf.py` & `repository_service_tuf-0.3.0a1/repository_service_tuf/helpers/tuf.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/tests/conftest.py` & `repository_service_tuf-0.3.0a1/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 )
 
 
 @pytest.fixture
 def test_context() -> Dict[str, Any]:
     setting_file = os.path.join(TemporaryDirectory().name, "test_settings.ini")
     test_settings = Dynaconf(settings_files=[setting_file])
-    test_settings.AUTH = True
+    test_settings.AUTH = False
     return {"settings": test_settings, "config": setting_file}
 
 
 @pytest.fixture
 def client() -> CliRunner:
     runner = CliRunner()
     return runner
```

### Comparing `repository_service_tuf-0.1.2a1/tests/test_tuf_repository_service.py` & `repository_service_tuf-0.3.0a1/tests/test_tuf_repository_service.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/tests/files/key_storage/JanisJoplin.key` & `repository_service_tuf-0.3.0a1/tests/files/key_storage/JanisJoplin.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/tests/files/key_storage/JimiHendrix.key` & `repository_service_tuf-0.3.0a1/tests/files/key_storage/JimiHendrix.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/tests/files/key_storage/online-rsa.key` & `repository_service_tuf-0.3.0a1/tests/files/key_storage/online-rsa.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/tests/files/key_storage/online-rsa.pub` & `repository_service_tuf-0.3.0a1/tests/files/key_storage/online-rsa.pub`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/tests/files/key_storage/online.key` & `repository_service_tuf-0.3.0a1/tests/files/key_storage/online.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/tests/unit/cli/test__init__.py` & `repository_service_tuf-0.3.0a1/tests/unit/cli/test__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,11 +15,11 @@
         """Tests the CLI --version parameter existence and output format."""
 
         result = client.invoke(rstuf, ["--version"])
 
         assert result.exit_code == 0
         assert result.output == f"rstuf, version {version}\n"
 
-    def test_no_auth_parameter(self, client):
-        result = client.invoke(rstuf, ["--no-auth", "admin"])
+    def test_auth_parameter(self, client):
+        result = client.invoke(rstuf, ["--auth", "admin"])
         assert result.exit_code == 0
-        assert "Skipping RSTUF authentication (--no-auth)" in result.output
+        assert "Using RSTUF built-in authentication (--auth)" in result.output
```

### Comparing `repository_service_tuf-0.1.2a1/tests/unit/cli/admin/test_ceremony.py` & `repository_service_tuf-0.3.0a1/tests/unit/cli/admin/test_ceremony.py`

 * *Files 0% similar despite different names*

```diff
@@ -778,29 +778,27 @@
             pretend.call(
                 "fake_task_id", test_context["settings"], "Bootstrap status: "
             )
         ]
         # test regression https://github.com/repository-service-tuf/repository-service-tuf-cli/pull/259  # noqa
         assert test_context["settings"].SERVER is not None
 
-    def test_ceremony_option_bootstrap_upload_no_auth(
-        self, client, test_context
-    ):
+    def test_ceremony_option_bootstrap_upload_auth(self, client, test_context):
         ceremony.bootstrap_status = pretend.call_recorder(
             lambda *a: {"data": {"bootstrap": False}}
         )
         ceremony._load_bootstrap_payload = pretend.call_recorder(
             lambda *a: {"k": "v"}
         )
         ceremony._send_bootstrap = pretend.call_recorder(
             lambda *a: "fake_task_id"
         )
         ceremony.task_status = pretend.call_recorder(lambda *a: None)
 
-        test_context["settings"].AUTH = False
+        test_context["settings"].AUTH = True
 
         test_result = client.invoke(
             ceremony.ceremony,
             ["--bootstrap", "--upload", "--upload-server", "http://rstuf"],
             input=None,
             obj=test_context,
         )
@@ -821,29 +819,29 @@
         ]
         assert ceremony.task_status.calls == [
             pretend.call(
                 "fake_task_id", test_context["settings"], "Bootstrap status: "
             )
         ]
 
-    def test_ceremony_option_bootstrap_upload_no_auth_missing_upload_server(
+    def test_ceremony_option_bootstrap_upload_auth_missing_upload_server(
         self, client, test_context
     ):
-        test_context["settings"].AUTH = False
+        test_context["settings"].AUTH = True
 
         test_result = client.invoke(
             ceremony.ceremony,
             ["--bootstrap", "--upload"],
             input=None,
             obj=test_context,
         )
 
         assert test_result.exit_code == 1, test_result.output
         assert (
-            "Requires '--upload-server' when using '--no-auth'"
+            "Requires '--upload-server' when using '--auth'"
             in test_result.output
         )
 
     def test_ceremony_option_upload_missing_bootstrap(
         self, client, test_context, test_inputs, test_setup
     ):
         ceremony.setup = test_setup
```

### Comparing `repository_service_tuf-0.1.2a1/tests/unit/cli/admin/test_import_targets.py` & `repository_service_tuf-0.3.0a1/tests/unit/cli/admin/test_import_targets.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/tests/unit/cli/admin/test_login.py` & `repository_service_tuf-0.3.0a1/tests/unit/cli/admin/test_login.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,18 +58,19 @@
             "admin",
             "pass",
             "1",
         ]
         login._login = pretend.call_recorder(
             lambda *a: {"access_token": "fake-token"}
         )
-
         login.loaders = pretend.stub(
             write=pretend.call_recorder(lambda *a: None)
         )
+        test_context["settings"].AUTH = True
+
         test_result = client.invoke(
             login.login, input="\n".join(steps), obj=test_context
         )
 
         assert test_result.exit_code == 0
         assert "Login successful." in test_result.output
         assert login.loaders.write.calls == [
@@ -84,15 +85,14 @@
             "admin",
             "pass",
             "1",
         ]
         login._login = pretend.call_recorder(
             lambda *a: {"access_token": "fake-token"}
         )
-        test_context["settings"].AUTH = False
         login.loaders = pretend.stub(
             write=pretend.call_recorder(lambda *a: None)
         )
         test_result = client.invoke(
             login.login, input="\n".join(steps), obj=test_context
         )
 
@@ -113,14 +113,15 @@
         login._login = pretend.call_recorder(
             lambda *a: {"access_token": "fake-token"}
         )
 
         login.loaders = pretend.stub(
             write=pretend.call_recorder(lambda *a: None)
         )
+        test_context["settings"].AUTH = True
         test_result = client.invoke(
             login.login, ["--force"], input="\n".join(steps), obj=test_context
         )
 
         assert test_result.exit_code == 0
         assert "Login successful." in test_result.output
         assert login.loaders.write.calls == [
@@ -146,14 +147,15 @@
         )
         login._login = pretend.call_recorder(
             lambda *a: {"access_token": "fake-token"}
         )
         login.loaders = pretend.stub(
             write=pretend.call_recorder(lambda *a: None)
         )
+        test_context["settings"].AUTH = True
 
         test_result = client.invoke(
             login.login, input="\n".join(steps), obj=test_context
         )
 
         assert test_result.exit_code == 0
         assert "Login successful." in test_result.output
@@ -186,14 +188,15 @@
         )
         login._login = pretend.call_recorder(
             lambda *a: {"access_token": "fake-token"}
         )
         login.loaders = pretend.stub(
             write=pretend.call_recorder(lambda *a: None)
         )
+        test_context["settings"].AUTH = True
 
         test_result = client.invoke(
             login.login, input="\n".join(steps), obj=test_context
         )
 
         assert test_result.exit_code == 0
         assert (
@@ -215,14 +218,16 @@
 
         login._login = pretend.call_recorder(
             lambda *a: {"access_token": "fake-token"}
         )
         login.loaders = pretend.stub(
             write=pretend.call_recorder(lambda *a: None)
         )
+        test_context["settings"].AUTH = True
+
         test_result = client.invoke(
             login.login, input="\n".join(steps), obj=test_context
         )
         assert test_result.exit_code == 0
         assert "Login successful." in test_result.output
 
     def test_login_with_server(self, client, test_context):
@@ -234,14 +239,16 @@
         login._login = pretend.call_recorder(
             lambda *a: {"access_token": "fake-token"}
         )
 
         login.loaders = pretend.stub(
             write=pretend.call_recorder(lambda *a: None)
         )
+        test_context["settings"].AUTH = True
+
         test_result = client.invoke(
             login.login,
             ["-s", "http://test-rstuf"],
             input="\n".join(steps),
             obj=test_context,
         )
 
@@ -258,14 +265,15 @@
             "admin",
             "pass",
             "1",
         ]
         login._login = pretend.call_recorder(
             lambda *a: {"access_token": "fake-token"}
         )
+        test_context["settings"].AUTH = True
 
         test_result = client.invoke(
             login.login,
             ["-s", "test-rstuf"],
             input="\n".join(steps),
             obj=test_context,
         )
@@ -288,14 +296,16 @@
         login._login = pretend.call_recorder(
             lambda *a: {"access_token": "fake-token"}
         )
 
         login.loaders = pretend.stub(
             write=pretend.call_recorder(lambda *a: None)
         )
+        test_context["settings"].AUTH = True
+
         test_result = client.invoke(
             login.login,
             ["-s", "test-rstuf"],
             input="\n".join(steps),
             obj=test_context,
         )
 
@@ -315,14 +325,16 @@
         login._login = pretend.call_recorder(
             lambda *a: {"access_token": "fake-token"}
         )
 
         login.loaders = pretend.stub(
             write=pretend.call_recorder(lambda *a: None)
         )
+        test_context["settings"].AUTH = True
+
         test_result = client.invoke(
             login.login,
             ["-s", "http://test-rstuf", "-u", "admin"],
             input="\n".join(steps),
             obj=test_context,
         )
 
@@ -342,14 +354,16 @@
         login._login = pretend.call_recorder(
             lambda *a: {"access_token": "fake-token"}
         )
 
         login.loaders = pretend.stub(
             write=pretend.call_recorder(lambda *a: None)
         )
+        test_context["settings"].AUTH = True
+
         test_result = client.invoke(
             login.login,
             ["-s", "http://test-rstuf", "-u", "admin", "-p", "pass"],
             input="\n".join(steps),
             obj=test_context,
         )
 
@@ -365,14 +379,16 @@
         login._login = pretend.call_recorder(
             lambda *a: {"access_token": "fake-token"}
         )
 
         login.loaders = pretend.stub(
             write=pretend.call_recorder(lambda *a: None)
         )
+        test_context["settings"].AUTH = True
+
         test_result = client.invoke(
             login.login,
             [
                 "-s",
                 "http://test-rstuf",
                 "-u",
                 "admin",
```

### Comparing `repository_service_tuf-0.1.2a1/tests/unit/cli/key/test_generate_key.py` & `repository_service_tuf-0.3.0a1/tests/unit/cli/key/test_generate_key.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/tests/unit/helpers/test_api_client.py` & `repository_service_tuf-0.3.0a1/tests/unit/helpers/test_api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,42 +76,46 @@
         )
         api_client.request_server = pretend.call_recorder(
             lambda *a, **kw: fake_response
         )
 
         test_context["settings"].SERVER = "http://server"
         test_context["settings"].TOKEN = "fake_token"
+        test_context["settings"].AUTH = True
+
         result = api_client.is_logged(test_context["settings"])
         assert result == api_client.Login(state=True, data={"expired": False})
         assert api_client.request_server.calls == [
             pretend.call(
                 "http://server",
                 "api/v1/token/?token=fake_token",
                 api_client.Methods.get,
                 headers={"Authorization": "Bearer fake_token"},
             )
         ]
 
     def test_is_logged_no_auth(self, test_context):
         test_context["settings"].SERVER = "http://server"
         test_context["settings"].TOKEN = "fake_token"
-        test_context["settings"].AUTH = False
+
         result = api_client.is_logged(test_context["settings"])
         assert result is None
 
     def test_is_logged_401(self, test_context):
         fake_response = pretend.stub(
             status_code=401,
         )
         api_client.request_server = pretend.call_recorder(
             lambda *a, **kw: fake_response
         )
 
         test_context["settings"].SERVER = "http://server"
         test_context["settings"].TOKEN = "fake_token"
+        test_context["settings"].AUTH = True
+
         result = api_client.is_logged(test_context["settings"])
         assert result == api_client.Login(state=False, data=None)
         assert api_client.request_server.calls == [
             pretend.call(
                 "http://server",
                 "api/v1/token/?token=fake_token",
                 api_client.Methods.get,
@@ -126,14 +130,16 @@
         )
         api_client.request_server = pretend.call_recorder(
             lambda *a, **kw: fake_response
         )
 
         test_context["settings"].SERVER = "http://server"
         test_context["settings"].TOKEN = "fake_token"
+        test_context["settings"].AUTH = True
+
         with pytest.raises(api_client.click.ClickException) as err:
             api_client.is_logged(test_context["settings"])
 
         assert "Error 500 body" in str(err)
         assert api_client.request_server.calls == [
             pretend.call(
                 "http://server",
@@ -151,14 +157,16 @@
         )
         api_client.request_server = pretend.call_recorder(
             lambda *a, **kw: pretend.stub(status_code=200)
         )
 
         test_context["settings"].SERVER = "http://server"
         test_context["settings"].TOKEN = "fake_token"
+        test_context["settings"].AUTH = True
+
         result = api_client.get_headers(test_context["settings"])
 
         assert result == {"Authorization": "Bearer fake_token"}
         assert api_client.is_logged.calls == [
             pretend.call(test_context["settings"])
         ]
         assert api_client.request_server.calls == [
@@ -167,15 +175,14 @@
                 api_client.URL.bootstrap.value,
                 api_client.Methods.get,
                 headers={"Authorization": "Bearer fake_token"},
             )
         ]
 
     def test_get_headers_no_auth(self, test_context):
-        test_context["settings"].AUTH = False
         result = api_client.get_headers(test_context["settings"])
 
         assert result == {}
 
     def test_get_headers_never_logged(self):
         with pytest.raises(api_client.click.ClickException) as err:
             api_client.get_headers({})
@@ -185,14 +192,16 @@
     def test_get_headers_is_logged_state_false(self, test_context):
         api_client.is_logged = pretend.call_recorder(
             lambda *a: api_client.Login(state=False, data={"expired": False})
         )
 
         test_context["settings"].SERVER = "http://server"
         test_context["settings"].TOKEN = "fake_token"
+        test_context["settings"].AUTH = True
+
         with pytest.raises(api_client.click.ClickException) as err:
             api_client.get_headers(test_context["settings"])
 
         assert "re-login" in str(err)
         assert api_client.is_logged.calls == [
             pretend.call(test_context["settings"])
         ]
@@ -202,14 +211,16 @@
     ):
         api_client.is_logged = pretend.call_recorder(
             lambda *a: api_client.Login(state=True, data={"expired": True})
         )
 
         test_context["settings"].SERVER = "http://server"
         test_context["settings"].TOKEN = "fake_token"
+        test_context["settings"].AUTH = True
+
         with pytest.raises(api_client.click.ClickException) as err:
             api_client.get_headers(test_context["settings"])
 
         assert "The token has expired" in str(err)
         assert api_client.is_logged.calls == [
             pretend.call(test_context["settings"])
         ]
@@ -220,14 +231,16 @@
         )
         api_client.request_server = pretend.call_recorder(
             lambda *a, **kw: pretend.stub(status_code=500, text="error body")
         )
 
         test_context["settings"].SERVER = "http://server"
         test_context["settings"].TOKEN = "fake_token"
+        test_context["settings"].AUTH = True
+
         with pytest.raises(api_client.click.ClickException) as err:
             api_client.get_headers(test_context["settings"])
 
         assert "Unexpected error" in str(err)
         assert api_client.is_logged.calls == [
             pretend.call(test_context["settings"])
         ]
```

### Comparing `repository_service_tuf-0.1.2a1/tests/unit/helpers/test_tuf.py` & `repository_service_tuf-0.3.0a1/tests/unit/helpers/test_tuf.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.2a1/PKG-INFO` & `repository_service_tuf-0.3.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: repository-service-tuf
-Version: 0.1.2a1
+Version: 0.3.0a1
 Summary: Repository Service for TUF Command Line Interface
 Author-email: Kairo de Araujo <kairo@dearaujo.nl>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Requires-Dist: click
 Requires-Dist: dynaconf[ini]==3.1.9
 Requires-Dist: pynacl
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: rich-click
 Requires-Dist: securesystemslib[crypto]
```

