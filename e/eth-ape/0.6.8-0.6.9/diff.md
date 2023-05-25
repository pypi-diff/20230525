# Comparing `tmp/eth-ape-0.6.8.tar.gz` & `tmp/eth-ape-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-ape-0.6.8.tar", last modified: Thu Apr 13 21:33:07 2023, max compression
+gzip compressed data, was "eth-ape-0.6.9.tar", last modified: Thu May 18 17:06:29 2023, max compression
```

## Comparing `eth-ape-0.6.8.tar` & `eth-ape-0.6.9.tar`

### file list

```diff
@@ -1,433 +1,439 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.229924 eth-ape-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 21:32:08.000000 eth-ape-0.6.8/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.185920 eth-ape-0.6.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-13 21:32:08.000000 eth-ape-0.6.8/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.185920 eth-ape-0.6.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-13 21:32:08.000000 eth-ape-0.6.8/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-13 21:32:08.000000 eth-ape-0.6.8/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-13 21:32:08.000000 eth-ape-0.6.8/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-13 21:32:08.000000 eth-ape-0.6.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-13 21:32:08.000000 eth-ape-0.6.8/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.189921 eth-ape-0.6.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-13 21:32:08.000000 eth-ape-0.6.8/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-13 21:32:08.000000 eth-ape-0.6.8/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-13 21:32:08.000000 eth-ape-0.6.8/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-13 21:32:08.000000 eth-ape-0.6.8/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-13 21:32:08.000000 eth-ape-0.6.8/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-13 21:32:08.000000 eth-ape-0.6.8/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-13 21:32:08.000000 eth-ape-0.6.8/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-04-13 21:32:08.000000 eth-ape-0.6.8/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-13 21:32:08.000000 eth-ape-0.6.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 21:32:08.000000 eth-ape-0.6.8/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-13 21:32:08.000000 eth-ape-0.6.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-13 21:32:08.000000 eth-ape-0.6.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-13 21:32:08.000000 eth-ape-0.6.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-13 21:32:08.000000 eth-ape-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9078 2023-04-13 21:33:07.229924 eth-ape-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6355 2023-04-13 21:32:08.000000 eth-ape-0.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-13 21:32:08.000000 eth-ape-0.6.8/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-13 21:32:08.000000 eth-ape-0.6.8/build_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-13 21:32:08.000000 eth-ape-0.6.8/codeql-config.yml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-13 21:32:08.000000 eth-ape-0.6.8/cz-requirement.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.189921 eth-ape-0.6.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.189921 eth-ape-0.6.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.189921 eth-ape-0.6.8/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.189921 eth-ape-0.6.8/docs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/commands/accounts.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/commands/compile.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/commands/console.rst
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/commands/init.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/commands/networks.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/commands/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/commands/run.rst
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/commands/test.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.189921 eth-ape-0.6.8/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/methoddocs/ape.md
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/methoddocs/api.md
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/methoddocs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/methoddocs/contracts.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/methoddocs/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/methoddocs/managers.md
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/methoddocs/plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/methoddocs/types.md
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/methoddocs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.193921 eth-ape-0.6.8/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/userguides/accounts.md
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/userguides/compile.md
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/userguides/config.md
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/userguides/console.md
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/userguides/contracts.md
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/userguides/data.md
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/userguides/developing_plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/userguides/installing_plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/userguides/networks.md
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/userguides/projects.md
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/userguides/publishing.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/userguides/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/userguides/scripts.md
--rw-r--r--   0 runner    (1001) docker     (123)    17146 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/userguides/testing.md
--rw-r--r--   0 runner    (1001) docker     (123)    19609 2023-04-13 21:32:08.000000 eth-ape-0.6.8/docs/userguides/transactions.md
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-13 21:32:08.000000 eth-ape-0.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 21:32:08.000000 eth-ape-0.6.8/recommended-plugins.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-13 21:33:07.229924 eth-ape-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-04-13 21:32:08.000000 eth-ape-0.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.181920 eth-ape-0.6.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.193921 eth-ape-0.6.8/src/ape/
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/__modules__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.193921 eth-ape-0.6.8/src/ape/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16470 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/api/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/api/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/api/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/api/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/api/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/api/explorers.py
--rw-r--r--   0 runner    (1001) docker     (123)    31054 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/api/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17481 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/api/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)    54303 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/api/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/api/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    14119 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/api/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.193921 eth-ape-0.6.8/src/ape/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/cli/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/cli/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/cli/paramtype.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.193921 eth-ape-0.6.8/src/ape/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45547 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/contracts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17324 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/harambe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.197921 eth-ape-0.6.8/src/ape/managers/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/managers/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    55355 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/managers/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/managers/compilers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/managers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/managers/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    20422 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/managers/networks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.197921 eth-ape-0.6.8/src/ape/managers/project/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/managers/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/managers/project/dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)    27229 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/managers/project/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12870 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/managers/project/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/managers/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.197921 eth-ape-0.6.8/src/ape/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/plugins/account.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/plugins/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/plugins/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/plugins/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/plugins/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/plugins/pluggy_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/plugins/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/plugins/query.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.197921 eth-ape-0.6.8/src/ape/pytest/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/pytest/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/pytest/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/pytest/contextmanagers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/pytest/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/pytest/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/pytest/runners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.197921 eth-ape-0.6.8/src/ape/types/
--rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/types/signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/types/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.201922 eth-ape-0.6.8/src/ape/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12343 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/utils/abi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/utils/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/utils/github.py
--rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/utils/os.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape/utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 21:33:06.000000 eth-ape-0.6.8/src/ape/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.201922 eth-ape-0.6.8/src/ape_accounts/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_accounts/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_accounts/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_accounts/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.201922 eth-ape-0.6.8/src/ape_cache/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_cache/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_cache/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_cache/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    17765 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_cache/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.201922 eth-ape-0.6.8/src/ape_compile/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_compile/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_compile/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.201922 eth-ape-0.6.8/src/ape_console/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_console/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_console/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_console/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.201922 eth-ape-0.6.8/src/ape_ethereum/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_ethereum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_ethereum/_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    28449 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_ethereum/ecosystem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.201922 eth-ape-0.6.8/src/ape_ethereum/multicall/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_ethereum/multicall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10221 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_ethereum/multicall/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_ethereum/multicall/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_ethereum/multicall/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_ethereum/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_ethereum/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.201922 eth-ape-0.6.8/src/ape_geth/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_geth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_geth/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_geth/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.201922 eth-ape-0.6.8/src/ape_init/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_init/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.201922 eth-ape-0.6.8/src/ape_networks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_networks/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.205922 eth-ape-0.6.8/src/ape_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_plugins/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_plugins/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.205922 eth-ape-0.6.8/src/ape_pm/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_pm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_pm/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_pm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.205922 eth-ape-0.6.8/src/ape_run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_run/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_run/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.205922 eth-ape-0.6.8/src/ape_test/
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_test/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_test/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_test/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:32:08.000000 eth-ape-0.6.8/src/ape_test/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.205922 eth-ape-0.6.8/src/eth_ape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9078 2023-04-13 21:33:06.000000 eth-ape-0.6.8/src/eth_ape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-04-13 21:33:07.000000 eth-ape-0.6.8/src/eth_ape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:33:06.000000 eth-ape-0.6.8/src/eth_ape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-13 21:33:06.000000 eth-ape-0.6.8/src/eth_ape.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:33:06.000000 eth-ape-0.6.8/src/eth_ape.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-13 21:33:06.000000 eth-ape-0.6.8/src/eth_ape.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-13 21:33:06.000000 eth-ape-0.6.8/src/eth_ape.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.205922 eth-ape-0.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.209922 eth-ape-0.6.8/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15606 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.209922 eth-ape-0.6.8/tests/functional/conversion/
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/conversion/test_encode_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/conversion/test_ether.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/conversion/test_timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.209922 eth-ape-0.6.8/tests/functional/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.181920 eth-ape-0.6.8/tests/functional/data/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.181920 eth-ape-0.6.8/tests/functional/data/contracts/ethereum/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.209922 eth-ape-0.6.8/tests/functional/data/contracts/ethereum/local/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/contracts/ethereum/local/Interface.json
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/contracts/ethereum/local/InterfaceImplementation.json
--rw-r--r--   0 runner    (1001) docker     (123)    21835 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/contracts/ethereum/local/contract_a.json
--rw-r--r--   0 runner    (1001) docker     (123)    21849 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/contracts/ethereum/local/contract_b.json
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/contracts/ethereum/local/contract_c.json
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/contracts/ethereum/local/ds_note_test.json
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/contracts/ethereum/local/has_error.json
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/contracts/ethereum/local/proxy.json
--rw-r--r--   0 runner    (1001) docker     (123)    28494 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/contracts/ethereum/local/reverts_contract.json
--rw-r--r--   0 runner    (1001) docker     (123)    43460 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/contracts/ethereum/local/solidity_contract.json
--rw-r--r--   0 runner    (1001) docker     (123)   220466 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/contracts/ethereum/local/vyper_contract.json
--rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/contracts/ethereum/local/vyper_math_dev_checks.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.181920 eth-ape-0.6.8/tests/functional/data/manifests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.181920 eth-ape-0.6.8/tests/functional/data/manifests/OpenZeppelin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.209922 eth-ape-0.6.8/tests/functional/data/manifests/OpenZeppelin/v3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)  1689272 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/manifests/OpenZeppelin/v3.1.0/OpenZeppelin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.213923 eth-ape-0.6.8/tests/functional/data/manifests/OpenZeppelin/v4.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)  3230874 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/manifests/OpenZeppelin/v4.4.2/OpenZeppelin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.181920 eth-ape-0.6.8/tests/functional/data/projects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.217923 eth-ape-0.6.8/tests/functional/data/projects/ApeProject/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/projects/ApeProject/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.217923 eth-ape-0.6.8/tests/functional/data/projects/ApeProject/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/projects/ApeProject/contracts/ApeContract0.json
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/projects/ApeProject/contracts/ApeContract1.json
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/projects/ApeProject/contracts/Contract.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.217923 eth-ape-0.6.8/tests/functional/data/projects/BrownieProject/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/projects/BrownieProject/brownie-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.217923 eth-ape-0.6.8/tests/functional/data/projects/BrownieProject/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/projects/BrownieProject/contracts/brownie.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.181920 eth-ape-0.6.8/tests/functional/data/projects/LongContractsFolder/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.181920 eth-ape-0.6.8/tests/functional/data/projects/LongContractsFolder/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.217923 eth-ape-0.6.8/tests/functional/data/projects/LongContractsFolder/source/v0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/projects/LongContractsFolder/source/v0.1/long_contracts_folder.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.217923 eth-ape-0.6.8/tests/functional/data/python/
--rw-r--r--   0 runner    (1001) docker     (123)    37462 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.217923 eth-ape-0.6.8/tests/functional/data/sources/
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/sources/ContractA.sol
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/sources/ContractB.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/sources/ContractC.sol
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/sources/HasError.sol
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/sources/Proxy.sol
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/sources/RevertsContractVy.vy
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/sources/TestContractSol.sol
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/sources/TestContractVy.vy
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/data/sources/VyperMathDevChecks.vy
--rw-r--r--   0 runner    (1001) docker     (123)    15321 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)    24198 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/test_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/test_compilers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/test_contract_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/test_contract_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    23810 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/test_contract_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/test_default_sender_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)    32505 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/test_ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13877 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/test_geth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/test_networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/test_receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/test_revert_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/test_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/test_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.221923 eth-ape-0.6.8/tests/functional/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/utils/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/utils/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/functional/utils/test_os.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.221923 eth-ape-0.6.8/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.221923 eth-ape-0.6.8/tests/integration/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.185920 eth-ape-0.6.8/tests/integration/cli/projects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.181920 eth-ape-0.6.8/tests/integration/cli/projects/bad-contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.221923 eth-ape-0.6.8/tests/integration/cli/projects/bad-contracts/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/bad-contracts/contracts/Contract.test
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/bad-contracts/contracts/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.221923 eth-ape-0.6.8/tests/integration/cli/projects/bad-contracts/contracts/subdir/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/bad-contracts/contracts/subdir/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.221923 eth-ape-0.6.8/tests/integration/cli/projects/bad-contracts/contracts/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/bad-contracts/contracts/tests/TestContract.foobar
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.221923 eth-ape-0.6.8/tests/integration/cli/projects/empty-config/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/empty-config/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.221923 eth-ape-0.6.8/tests/integration/cli/projects/geth/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/geth/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.221923 eth-ape-0.6.8/tests/integration/cli/projects/geth/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)    28133 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/geth/contracts/contract.json
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/geth/contracts/token_a.json
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/geth/contracts/token_b.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.221923 eth-ape-0.6.8/tests/integration/cli/projects/geth/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/geth/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/geth/tests/test_using_local_geth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.181920 eth-ape-0.6.8/tests/integration/cli/projects/multiple-interfaces/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.221923 eth-ape-0.6.8/tests/integration/cli/projects/multiple-interfaces/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/multiple-interfaces/contracts/Interface-with-hyphens.json
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/multiple-interfaces/contracts/Interface.exclude.json
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/multiple-interfaces/contracts/Interface.json
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/multiple-interfaces/contracts/InterfaceWithNumber123.json
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/multiple-interfaces/contracts/Interface_with_underscores.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.221923 eth-ape-0.6.8/tests/integration/cli/projects/no-config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/no-config/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.221923 eth-ape-0.6.8/tests/integration/cli/projects/only-dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/only-dependencies/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.221923 eth-ape-0.6.8/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/importme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.225924 eth-ape-0.6.8/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/sources/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/sources/DependencyInProjectOnly.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.181920 eth-ape-0.6.8/tests/integration/cli/projects/only-script-subdirs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.181920 eth-ape-0.6.8/tests/integration/cli/projects/only-script-subdirs/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.225924 eth-ape-0.6.8/tests/integration/cli/projects/only-script-subdirs/scripts/subdirectory/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/only-script-subdirs/scripts/subdirectory/subdirectory_click_print.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/only-script-subdirs/scripts/subdirectory/subdirectory_main_print.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.181920 eth-ape-0.6.8/tests/integration/cli/projects/script/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.225924 eth-ape-0.6.8/tests/integration/cli/projects/script/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/script/scripts/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/script/scripts/click.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/script/scripts/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/script/scripts/error_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/script/scripts/error_forgot_click.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/script/scripts/error_main.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/script/scripts/error_no_def.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/script/scripts/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.225924 eth-ape-0.6.8/tests/integration/cli/projects/script/scripts/subdirectory/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/script/scripts/subdirectory/subdirectory_click_print.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/script/scripts/subdirectory/subdirectory_main_print.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.225924 eth-ape-0.6.8/tests/integration/cli/projects/test/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/test/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.225924 eth-ape-0.6.8/tests/integration/cli/projects/test/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/test/tests/test_fixture_isolation.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/test/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/test/tests/test_networks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.225924 eth-ape-0.6.8/tests/integration/cli/projects/with-contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/with-contracts/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.225924 eth-ape-0.6.8/tests/integration/cli/projects/with-contracts/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/with-contracts/contracts/ContractA.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.225924 eth-ape-0.6.8/tests/integration/cli/projects/with-contracts/contracts/DirectoryWithJSONExtension.json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/with-contracts/contracts/DirectoryWithJSONExtension.json/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)    41634 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/with-contracts/contracts/RawSolidityOutput.json
--rw-r--r--   0 runner    (1001) docker     (123)    64327 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/with-contracts/contracts/RawVyperOutput.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.225924 eth-ape-0.6.8/tests/integration/cli/projects/with-contracts/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/with-contracts/scripts/txerr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.225924 eth-ape-0.6.8/tests/integration/cli/projects/with-contracts/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/with-contracts/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/with-contracts/tests/test_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.225924 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.225924 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.225924 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/contracts/containing_sub_dependencies.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.185920 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/sub_dependency/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.225924 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/sub_dependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/sub_dependency/contracts/SubDependency.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.225924 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/contracts/Other.json
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/contracts/Project.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.185920 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/default/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.225924 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/default/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/default/contracts/default.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.185920 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.185920 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.185920 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.225924 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/src/v0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/src/v0.1/renamed_complex_contracts_folder.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.185920 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.225924 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder/sources/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder/sources/renamed_contracts_folder.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.225924 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:33:07.225924 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/my_contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/my_contracts/renamed_contracts_folder_specified_in_config.json
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10755 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/test_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/test_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/test_networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/test_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-13 21:32:08.000000 eth-ape-0.6.8/tests/integration/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.586583 eth-ape-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-18 17:05:05.000000 eth-ape-0.6.9/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.530582 eth-ape-0.6.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-18 17:05:05.000000 eth-ape-0.6.9/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.530582 eth-ape-0.6.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-18 17:05:05.000000 eth-ape-0.6.9/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-18 17:05:05.000000 eth-ape-0.6.9/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-18 17:05:05.000000 eth-ape-0.6.9/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-18 17:05:05.000000 eth-ape-0.6.9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-18 17:05:05.000000 eth-ape-0.6.9/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.534582 eth-ape-0.6.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-18 17:05:05.000000 eth-ape-0.6.9/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-18 17:05:05.000000 eth-ape-0.6.9/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-18 17:05:05.000000 eth-ape-0.6.9/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-18 17:05:05.000000 eth-ape-0.6.9/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-18 17:05:05.000000 eth-ape-0.6.9/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-18 17:05:05.000000 eth-ape-0.6.9/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-18 17:05:05.000000 eth-ape-0.6.9/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-18 17:05:05.000000 eth-ape-0.6.9/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-18 17:05:05.000000 eth-ape-0.6.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 17:05:05.000000 eth-ape-0.6.9/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-18 17:05:05.000000 eth-ape-0.6.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-18 17:05:05.000000 eth-ape-0.6.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-18 17:05:05.000000 eth-ape-0.6.9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-18 17:05:05.000000 eth-ape-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-05-18 17:06:29.586583 eth-ape-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-05-18 17:05:05.000000 eth-ape-0.6.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-18 17:05:05.000000 eth-ape-0.6.9/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-18 17:05:05.000000 eth-ape-0.6.9/build_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-18 17:05:05.000000 eth-ape-0.6.9/codeql-config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-18 17:05:05.000000 eth-ape-0.6.9/cz-requirement.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.534582 eth-ape-0.6.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.534582 eth-ape-0.6.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.534582 eth-ape-0.6.9/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.534582 eth-ape-0.6.9/docs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/commands/accounts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/commands/compile.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/commands/console.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/commands/init.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/commands/networks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/commands/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/commands/run.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/commands/test.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.538582 eth-ape-0.6.9/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/methoddocs/ape.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/methoddocs/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/methoddocs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/methoddocs/contracts.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/methoddocs/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/methoddocs/managers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/methoddocs/plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/methoddocs/types.md
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/methoddocs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.538582 eth-ape-0.6.9/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/userguides/accounts.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/userguides/compile.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/userguides/config.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/userguides/console.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/userguides/contracts.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/userguides/data.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/userguides/developing_plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/userguides/installing_plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/userguides/networks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/userguides/projects.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/userguides/publishing.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/userguides/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/userguides/scripts.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17899 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/userguides/testing.md
+-rw-r--r--   0 runner    (1001) docker     (123)    19609 2023-05-18 17:05:05.000000 eth-ape-0.6.9/docs/userguides/transactions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-18 17:05:05.000000 eth-ape-0.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-18 17:05:05.000000 eth-ape-0.6.9/recommended-plugins.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-18 17:06:29.586583 eth-ape-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-05-18 17:05:05.000000 eth-ape-0.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.514582 eth-ape-0.6.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.542582 eth-ape-0.6.9/src/ape/
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/__modules__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.542582 eth-ape-0.6.9/src/ape/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16566 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/api/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/api/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/api/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/api/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/api/explorers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31098 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/api/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17716 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/api/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55546 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/api/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/api/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15270 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/api/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.542582 eth-ape-0.6.9/src/ape/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/cli/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/cli/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/cli/paramtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.542582 eth-ape-0.6.9/src/ape/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45767 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/contracts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21275 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/harambe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.546582 eth-ape-0.6.9/src/ape/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/managers/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56164 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/managers/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/managers/compilers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/managers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/managers/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20422 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/managers/networks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.546582 eth-ape-0.6.9/src/ape/managers/project/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/managers/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/managers/project/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28105 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/managers/project/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13131 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/managers/project/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/managers/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.546582 eth-ape-0.6.9/src/ape/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/plugins/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/plugins/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/plugins/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/plugins/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/plugins/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/plugins/pluggy_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/plugins/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/plugins/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.550582 eth-ape-0.6.9/src/ape/pytest/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/pytest/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/pytest/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/pytest/contextmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/pytest/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/pytest/gas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/pytest/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/pytest/runners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.550582 eth-ape-0.6.9/src/ape/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/types/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/types/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20947 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/types/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.550582 eth-ape-0.6.9/src/ape/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12343 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/utils/abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/utils/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/utils/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/utils/os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape/utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 17:06:28.000000 eth-ape-0.6.9/src/ape/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.550582 eth-ape-0.6.9/src/ape_accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_accounts/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_accounts/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_accounts/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.554582 eth-ape-0.6.9/src/ape_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_cache/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_cache/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17765 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_cache/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.554582 eth-ape-0.6.9/src/ape_compile/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_compile/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_compile/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.554582 eth-ape-0.6.9/src/ape_console/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_console/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_console/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_console/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.554582 eth-ape-0.6.9/src/ape_ethereum/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_ethereum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_ethereum/_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28601 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_ethereum/ecosystem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.554582 eth-ape-0.6.9/src/ape_ethereum/multicall/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_ethereum/multicall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10221 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_ethereum/multicall/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_ethereum/multicall/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_ethereum/multicall/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_ethereum/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_ethereum/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.554582 eth-ape-0.6.9/src/ape_geth/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_geth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21466 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_geth/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_geth/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.554582 eth-ape-0.6.9/src/ape_init/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_init/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.554582 eth-ape-0.6.9/src/ape_networks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_networks/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.558582 eth-ape-0.6.9/src/ape_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_plugins/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_plugins/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.558582 eth-ape-0.6.9/src/ape_pm/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_pm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_pm/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_pm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.558582 eth-ape-0.6.9/src/ape_run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_run/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_run/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.558582 eth-ape-0.6.9/src/ape_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_test/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_test/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_test/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:05:05.000000 eth-ape-0.6.9/src/ape_test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.558582 eth-ape-0.6.9/src/eth_ape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-05-18 17:06:29.000000 eth-ape-0.6.9/src/eth_ape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-05-18 17:06:29.000000 eth-ape-0.6.9/src/eth_ape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:06:29.000000 eth-ape-0.6.9/src/eth_ape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-18 17:06:29.000000 eth-ape-0.6.9/src/eth_ape.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:06:29.000000 eth-ape-0.6.9/src/eth_ape.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-18 17:06:29.000000 eth-ape-0.6.9/src/eth_ape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-18 17:06:29.000000 eth-ape-0.6.9/src/eth_ape.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.558582 eth-ape-0.6.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.562582 eth-ape-0.6.9/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16088 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.562582 eth-ape-0.6.9/tests/functional/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/conversion/test_encode_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/conversion/test_ether.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/conversion/test_timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.562582 eth-ape-0.6.9/tests/functional/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.518582 eth-ape-0.6.9/tests/functional/data/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.518582 eth-ape-0.6.9/tests/functional/data/contracts/ethereum/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.566582 eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/Interface.json
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/InterfaceImplementation.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21835 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/contract_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21849 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/contract_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/contract_c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/ds_note_test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/has_error.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/proxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)    46746 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/reverts_contract.json
+-rw-r--r--   0 runner    (1001) docker     (123)    43460 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/solidity_contract.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/sub_reverts_contract.json
+-rw-r--r--   0 runner    (1001) docker     (123)   220466 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/vyper_contract.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/vyper_math_dev_checks.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.518582 eth-ape-0.6.9/tests/functional/data/manifests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.518582 eth-ape-0.6.9/tests/functional/data/manifests/OpenZeppelin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.566582 eth-ape-0.6.9/tests/functional/data/manifests/OpenZeppelin/v3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)  1689272 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/manifests/OpenZeppelin/v3.1.0/OpenZeppelin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.570582 eth-ape-0.6.9/tests/functional/data/manifests/OpenZeppelin/v4.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)  3230874 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/manifests/OpenZeppelin/v4.4.2/OpenZeppelin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.522582 eth-ape-0.6.9/tests/functional/data/projects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.574582 eth-ape-0.6.9/tests/functional/data/projects/ApeProject/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/projects/ApeProject/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.574582 eth-ape-0.6.9/tests/functional/data/projects/ApeProject/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/projects/ApeProject/contracts/ApeContract0.json
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/projects/ApeProject/contracts/ApeContract1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/projects/ApeProject/contracts/Contract.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.574582 eth-ape-0.6.9/tests/functional/data/projects/BrownieProject/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/projects/BrownieProject/brownie-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.574582 eth-ape-0.6.9/tests/functional/data/projects/BrownieProject/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/projects/BrownieProject/contracts/brownie.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.522582 eth-ape-0.6.9/tests/functional/data/projects/LongContractsFolder/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.522582 eth-ape-0.6.9/tests/functional/data/projects/LongContractsFolder/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.574582 eth-ape-0.6.9/tests/functional/data/projects/LongContractsFolder/source/v0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/projects/LongContractsFolder/source/v0.1/long_contracts_folder.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.574582 eth-ape-0.6.9/tests/functional/data/python/
+-rw-r--r--   0 runner    (1001) docker     (123)    37462 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.574582 eth-ape-0.6.9/tests/functional/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/sources/ContractA.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/sources/ContractB.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/sources/ContractC.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/sources/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/sources/Proxy.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/sources/RevertsContractVy.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/sources/SubRevertsVy.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/sources/TestContractSol.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/sources/TestContractVy.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/sources/VyperMathDevChecks.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.574582 eth-ape-0.6.9/tests/functional/data/sources/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/data/sources/interfaces/ISubRevertsVy.vy
+-rw-r--r--   0 runner    (1001) docker     (123)    16298 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24198 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/test_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/test_compilers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/test_contract_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/test_contract_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24524 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/test_contract_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/test_default_sender_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32878 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/test_ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16507 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/test_geth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/test_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/test_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/test_revert_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/test_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.578582 eth-ape-0.6.9/tests/functional/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/utils/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/utils/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/functional/utils/test_os.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.578582 eth-ape-0.6.9/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.578582 eth-ape-0.6.9/tests/integration/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.526582 eth-ape-0.6.9/tests/integration/cli/projects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.522582 eth-ape-0.6.9/tests/integration/cli/projects/bad-contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.578582 eth-ape-0.6.9/tests/integration/cli/projects/bad-contracts/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/bad-contracts/contracts/Contract.test
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/bad-contracts/contracts/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.578582 eth-ape-0.6.9/tests/integration/cli/projects/bad-contracts/contracts/subdir/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/bad-contracts/contracts/subdir/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.578582 eth-ape-0.6.9/tests/integration/cli/projects/bad-contracts/contracts/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/bad-contracts/contracts/tests/TestContract.foobar
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.578582 eth-ape-0.6.9/tests/integration/cli/projects/empty-config/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/empty-config/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.578582 eth-ape-0.6.9/tests/integration/cli/projects/geth/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/geth/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.578582 eth-ape-0.6.9/tests/integration/cli/projects/geth/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)    28133 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/geth/contracts/contract.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/geth/contracts/token_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/geth/contracts/token_b.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.582582 eth-ape-0.6.9/tests/integration/cli/projects/geth/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/geth/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/geth/tests/test_using_local_geth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.526582 eth-ape-0.6.9/tests/integration/cli/projects/multiple-interfaces/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.582582 eth-ape-0.6.9/tests/integration/cli/projects/multiple-interfaces/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/multiple-interfaces/contracts/Interface-with-hyphens.json
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/multiple-interfaces/contracts/Interface.exclude.json
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/multiple-interfaces/contracts/Interface.json
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/multiple-interfaces/contracts/InterfaceWithNumber123.json
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/multiple-interfaces/contracts/Interface_with_underscores.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.582582 eth-ape-0.6.9/tests/integration/cli/projects/no-config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/no-config/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.582582 eth-ape-0.6.9/tests/integration/cli/projects/only-dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/only-dependencies/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.582582 eth-ape-0.6.9/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/importme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.582582 eth-ape-0.6.9/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/sources/DependencyInProjectOnly.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.526582 eth-ape-0.6.9/tests/integration/cli/projects/only-script-subdirs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.526582 eth-ape-0.6.9/tests/integration/cli/projects/only-script-subdirs/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.582582 eth-ape-0.6.9/tests/integration/cli/projects/only-script-subdirs/scripts/subdirectory/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/only-script-subdirs/scripts/subdirectory/subdirectory_click_print.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/only-script-subdirs/scripts/subdirectory/subdirectory_main_print.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.526582 eth-ape-0.6.9/tests/integration/cli/projects/script/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.582582 eth-ape-0.6.9/tests/integration/cli/projects/script/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/script/scripts/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/script/scripts/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/script/scripts/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/script/scripts/error_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/script/scripts/error_forgot_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/script/scripts/error_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/script/scripts/error_no_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/script/scripts/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.582582 eth-ape-0.6.9/tests/integration/cli/projects/script/scripts/subdirectory/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/script/scripts/subdirectory/subdirectory_click_print.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/script/scripts/subdirectory/subdirectory_main_print.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.582582 eth-ape-0.6.9/tests/integration/cli/projects/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/test/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.586583 eth-ape-0.6.9/tests/integration/cli/projects/test/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/test/tests/test_fixture_isolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/test/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/test/tests/test_networks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.586583 eth-ape-0.6.9/tests/integration/cli/projects/with-contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/with-contracts/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.586583 eth-ape-0.6.9/tests/integration/cli/projects/with-contracts/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/with-contracts/contracts/ContractA.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.586583 eth-ape-0.6.9/tests/integration/cli/projects/with-contracts/contracts/DirectoryWithJSONExtension.json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/with-contracts/contracts/DirectoryWithJSONExtension.json/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)    41634 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/with-contracts/contracts/RawSolidityOutput.json
+-rw-r--r--   0 runner    (1001) docker     (123)    64327 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/with-contracts/contracts/RawVyperOutput.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.586583 eth-ape-0.6.9/tests/integration/cli/projects/with-contracts/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/with-contracts/scripts/txerr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.586583 eth-ape-0.6.9/tests/integration/cli/projects/with-contracts/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/with-contracts/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/with-contracts/tests/test_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.586583 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.586583 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.586583 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/contracts/containing_sub_dependencies.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.526582 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/sub_dependency/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.586583 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/sub_dependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/sub_dependency/contracts/SubDependency.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.586583 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/contracts/Other.json
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/contracts/Project.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.526582 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/default/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.586583 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/default/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/default/contracts/default.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.526582 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.526582 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.526582 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.586583 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/src/v0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/src/v0.1/renamed_complex_contracts_folder.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.526582 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.586583 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder/sources/renamed_contracts_folder.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.586583 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:06:29.586583 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/my_contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/my_contracts/renamed_contracts_folder_specified_in_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/test_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/test_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/test_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-05-18 17:05:05.000000 eth-ape-0.6.9/tests/integration/cli/utils.py
```

### Comparing `eth-ape-0.6.8/.github/ISSUE_TEMPLATE/bug.md` & `eth-ape-0.6.9/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/.github/ISSUE_TEMPLATE/feature.md` & `eth-ape-0.6.9/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/.github/ISSUE_TEMPLATE/work-item.md` & `eth-ape-0.6.9/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/.github/PULL_REQUEST_TEMPLATE.md` & `eth-ape-0.6.9/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/.github/release-drafter.yml` & `eth-ape-0.6.9/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/.github/workflows/codeql.yml` & `eth-ape-0.6.9/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/.github/workflows/commitlint.yaml` & `eth-ape-0.6.9/.github/workflows/commitlint.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         - uses: actions/checkout@v3
           with:
               fetch-depth: 0
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install -r cz-requirement.txt
 
         - name: Check commit history
```

### Comparing `eth-ape-0.6.8/.github/workflows/docs.yaml` & `eth-ape-0.6.9/.github/workflows/docs.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[doc]
 
         - name: Build HTML artifact
```

### Comparing `eth-ape-0.6.8/.github/workflows/prtitle.yaml` & `eth-ape-0.6.9/.github/workflows/prtitle.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install -r cz-requirement.txt
 
         - name: Check PR Title
```

### Comparing `eth-ape-0.6.8/.github/workflows/publish.yaml` & `eth-ape-0.6.9/.github/workflows/publish.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: 3.8
+        python-version: "3.10"
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
 
     - name: Build
```

### Comparing `eth-ape-0.6.8/.github/workflows/stale-prs.yml` & `eth-ape-0.6.9/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/.github/workflows/test.yaml` & `eth-ape-0.6.9/.github/workflows/test.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint]
 
         - name: Run Black
@@ -43,15 +43,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint,test]
 
         - name: Run MyPy
@@ -59,15 +59,15 @@
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, "3.10"]
+                python-version: [3.8, 3.9, "3.10", "3.11"]
 
         env:
           GITHUB_ACCESS_TOKEN: ${{ secrets.GITHUB_TOKEN }}
           GETH_VERSION: 1.11.5
 
         steps:
         - uses: actions/checkout@v3
@@ -119,15 +119,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[test]
 
         - name: Run Tests
```

### Comparing `eth-ape-0.6.8/.gitignore` & `eth-ape-0.6.9/.gitignore`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/.pre-commit-config.yaml` & `eth-ape-0.6.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/CONTRIBUTING.md` & `eth-ape-0.6.9/CONTRIBUTING.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 python3 -m venv venv
 source venv/bin/activate
 
 # install the developer dependencies (-e is interactive mode)
 pip install -e .'[dev]'
 ```
 
+**NOTE**: You might run into issues where you have a local install and are trying to work with a plugin pinned to a specific version.
+
+[The easiest solution](https://github.com/ApeWorX/ape/issues/90) to this is to fetch the tags via `git fetch upstream --tags` and reinstall via `pip install .`.
+You will then have the correct version.
+
 ## Pre-Commit Hooks
 
 We use [`pre-commit`](https://pre-commit.com/) hooks to simplify linting and ensure consistent formatting among contributors.
 Use of `pre-commit` is not a requirement, but is highly recommended.
 
 Install `pre-commit` locally from the root folder:
```

### Comparing `eth-ape-0.6.8/Dockerfile` & `eth-ape-0.6.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/LICENSE` & `eth-ape-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/PKG-INFO` & `eth-ape-0.6.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,223 +1,224 @@
 Metadata-Version: 2.1
 Name: eth-ape
-Version: 0.6.8
+Version: 0.6.9
 Summary: Ape Ethereum Framework
 Home-page: https://apeworx.io
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Project-URL: Documentation, https://docs.apeworx.io/ape/
 Project-URL: Funding, https://gitcoin.co/grants/5958/ape-maintenance-fund
 Project-URL: Source, https://github.com/ApeWorX/ape
 Project-URL: Tracker, https://github.com/ApeWorX/ape/issues
 Project-URL: Twitter, https://twitter.com/ApeFramework
-Description: # Overview
-        
-        **Ape Framework** is an easy-to-use Web3 development tool.
-        Users can compile, test, and interact with smart contracts all in one command line session.
-        With our **modular plugin system**, Ape supports multiple contract languages and chains.
-        
-        Ape is built by [ApeWorX LTD](https://www.apeworx.io/).
-        
-        Join our [ApeWorX Discord server](https://discord.gg/apeworx) to stay up to date on new releases, plugins and tutorials.
-        
-        If you want to just get started, jump down to the [Playing with Ape](#playing-with-ape)
-        
-        ## Documentation
-        
-        Read our [technical documentation](https://docs.apeworx.io/ape/stable/) to get a deeper understanding of our open source Framework.
-        
-        Read our [academic platform](https://academy.apeworx.io/) will help you master Ape Framework with tutorials and challenges.
-        
-        ## Prerequisite
-        
-        In the latest release, Ape requires:
-        
-        - Linux or macOS
-        - Python 3.8 or later
-        - **Windows**: Install Windows Subsystem Linux [(WSL)](https://docs.microsoft.com/en-us/windows/wsl/install) with Python 3.8 or later
-        
-        Check your python version in a terminal with `python3 --version`
-        
-        ## Installation
-        
-        There are three ways to install ape: `pipx`, `pip`, or `Docker`.
-        
-        ### Considerations for Installing:
-        
-        - We advise installing in a [virtualenv](https://pypi.org/project/virtualenv/) or [venv](https://docs.python.org/3/library/venv.html) to avoid interfering with *OS-level site packages*.
-        
-        - We advise installing **`ape`** with recommended plugins `pip install eth-ape'[recommended-plugins]'`
-        
-        - We advise for **macOS** users to install virtual env via [homebrew](https://formulae.brew.sh/formula/virtualenv)
-        
-        ### via `pipx` or `pip`
-        
-        1. Install `pipx` via their [installation instructions](https://pypa.github.io/pipx/) or `pip` via their [installation instructions](https://pip.pypa.io/en/stable/cli/pip_install/)
-        
-        2. Install **`ape`** via `pipx install eth-ape` or `pip install eth-ape`
-        
-        ### via `docker`
-        
-        Ape can also run in a docker container.
-        
-        Please visit our [Dockerhub](https://hub.docker.com/repository/docker/apeworx/ape) for more details on using Ape with Docker.
-        
-        ```bash
-        docker run \
-        --volume $HOME/.ape:/home/harambe/.ape \
-        --volume $HOME/.vvm:/home/harambe/.vvm \
-        --volume $HOME/.solcx:/home/harambe/.solcx \
-        --volume $PWD:/home/harambe/project \
-        --workdir /home/harambe/project \
-        apeworx/ape compile
-        ```
-        
-        ## Playing with Ape
-        
-        After you installed Ape, you can run `ape --version` to make sure it works and is the latest version.
-        
-        There are two ways to interact with Ape:
-        
-        - [CLI Reference](https://docs.apeworx.io/ape/latest/index.html)
-        
-        - [Python Reference](https://docs.apeworx.io/ape/latest/index.html)
-        
-        Ape is both a CLI tool and a Python SDK.
-        
-        The CLI tool contains all the Ape commands and the Python SDK contains the classes and types needed to compose scripts, console actions, and tests.
-        
-        ## **Ape Modular Plugin System:**
-        
-        Our [list of plugins](https://www.apeworx.io/#plugins) is the best way to have the most interoperable experience with Web3.
-        
-        **NOTE**: If a plugin does not originate from the [ApeWorX GitHub Organization](https://github.com/ApeWorX?q=ape&type=all), you will get a warning about installing 3rd-party plugins.
-        
-        Install 3rd party plugins at your own risk.
-        
-        Additionally, plugins that come bundled with **`ape`** in the core installation cannot be removed and are part of the **`ape`** core software.
-        
-        - Learn more about **installing** plugins from following this [installing user guide](https://docs.apeworx.io/ape/stable/userguides/installing_plugins.html).
-        
-        - Learn more about **developing** your own plugins from this [developing user guide](https://docs.apeworx.io/ape/stable/userguides/developing_plugins.html).
-        
-        ### Accounts
-        
-        In Ape, you will need accounts to make transactions.
-        You can import or generate accounts using the core `accounts` plugin:
-        
-        ```bash
-        ape accounts import acc0   # Will prompt for a private key
-        ape accounts generate acc1
-        ```
-        
-        List all your accounts with the `list` command.
-        
-        ```bash
-        ape accounts list
-        ```
-        
-        Learn more about accounts in Ape by following the [accounts guide](https://docs.apeworx.io/ape/stable/userguides/accounts.html).
-        
-        ### Plugins
-        
-        Add any plugins you may need, such as `vyper`.
-        
-        ```bash
-        ape plugins list -a
-        ape plugins install vyper
-        ape plugins list -a
-        ```
-        
-        ## Projects
-        
-        When using Ape, you generally will work with a project.
-        
-        Learn more about smart-contract **projects** from this [projects guide](https://docs.apeworx.io/ape/stable/userguides/projects.html).
-        
-        ### Compiling
-        
-        You can compile contracts within the `contracts/` directory of your project.
-        The `--size` option will display you the size of the contract.
-        
-        ```bash
-        ape compile --size
-        ```
-        
-        Learn more about compiling in Ape by following the [compile guide](https://docs.apeworx.io/ape/stable/userguides/compile.html).
-        
-        ### Testing
-        
-        Use Ape to test your smart-contract projects.
-        Provide the same arguments to `pytest` as you would to the `ape test` command.
-        
-        For example:
-        
-        ```bash
-        ape test -k test_only_one_thing
-        ```
-        
-        Visit the [testing guide](https://docs.apeworx.io/ape/stable/userguides/testing.html) to learn more about testing using Ape.
-        
-        ### Console
-        
-        Ape provides an `IPython` interactive console with useful pre-defined locals to interact with your project.
-        To interact with a deployed contract in a local environment, start by opening the console:
-        
-        ```bash
-        ape console --network ethereum:mainnet:infura
-        ```
-        
-        Visit [Ape Console](https://docs.apeworx.io/ape/stable/commands/console.html) to learn how to use Ape Console.
-        
-        ### Scripts
-        
-        If you want to run specific files in a `scripts/` directory, you can do it using the `ape run` command.
-        
-        ```bash
-        # This command will run a file named deploy in the scripts/ directory
-        $ ape run deploy
-        ```
-        
-        Learn more about scripting using Ape by following the [scripting guide](https://docs.apeworx.io/ape/stable/userguides/scripts.html).
-        
-        ### Logging
-        
-        To enable debug logging, run your command with the `--verbosity` flag using `DEBUG` as the value:
-        
-        ```bash
-        ape --verbosity DEBUG run
-        ```
-        
-        ### Networks
-        
-        You can work with registered networks, providers, and blockchain ecosystems (like Ethereum):
-        
-        ```python
-        from ape import networks
-        with networks.ethereum.mainnet.use_provider("infura"):
-            ...  # Work with the infura provider here
-        ```
-        
-        To learn more about networks in Ape, see [this guide](https://docs.apeworx.io/ape/stable/commands/networks.html).
-        
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8,<3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
 Provides-Extra: recommended-plugins
+License-File: LICENSE
+
+# Overview
+
+**Ape Framework** is an easy-to-use Web3 development tool.
+Users can compile, test, and interact with smart contracts all in one command line session.
+With our **modular plugin system**, Ape supports multiple contract languages and chains.
+
+Ape is built by [ApeWorX LTD](https://www.apeworx.io/).
+
+Join our [ApeWorX Discord server](https://discord.gg/apeworx) to stay up to date on new releases, plugins and tutorials.
+
+If you want to just get started, jump down to the [Playing with Ape](#playing-with-ape).
+
+## Documentation
+
+Read our [technical documentation](https://docs.apeworx.io/ape/stable/) to get a deeper understanding of our open source Framework.
+
+Read our [academic platform](https://academy.apeworx.io/) will help you master Ape Framework with tutorials and challenges.
+
+## Prerequisite
+
+In the latest release, Ape requires:
+
+- Linux or macOS
+- Python 3.8 up to 3.11
+- **Windows**: Install Windows Subsystem Linux [(WSL)](https://docs.microsoft.com/en-us/windows/wsl/install)
+
+Check your python version in a terminal with `python3 --version`.
+
+## Installation
+
+There are three ways to install ape: `pipx`, `pip`, or `Docker`.
+
+### Considerations for Installing:
+
+- We advise installing in a [virtualenv](https://pypi.org/project/virtualenv/) or [venv](https://docs.python.org/3/library/venv.html) to avoid interfering with *OS-level site packages*.
+
+- We advise installing **`ape`** with recommended plugins `pip install eth-ape'[recommended-plugins]'`.
+
+- We advise for **macOS** users to install virtual env via [homebrew](https://formulae.brew.sh/formula/virtualenv).
+
+### via `pipx` or `pip`
+
+1. Install `pipx` via their [installation instructions](https://pypa.github.io/pipx/) or `pip` via their [installation instructions](https://pip.pypa.io/en/stable/cli/pip_install/).
+
+2. Install **`ape`** via `pipx install eth-ape` or `pip install eth-ape`.
+
+### via `docker`
+
+Ape can also run in a docker container.
+
+Please visit our [Dockerhub](https://hub.docker.com/repository/docker/apeworx/ape) for more details on using Ape with Docker.
+
+```bash
+docker run \
+--volume $HOME/.ape:/home/harambe/.ape \
+--volume $HOME/.vvm:/home/harambe/.vvm \
+--volume $HOME/.solcx:/home/harambe/.solcx \
+--volume $PWD:/home/harambe/project \
+--workdir /home/harambe/project \
+apeworx/ape compile
+```
+
+## Playing with Ape
+
+After you installed Ape, you can run `ape --version` to make sure it works and is the latest version.
+
+There are two ways to interact with Ape:
+
+- [CLI Reference](https://docs.apeworx.io/ape/latest/index.html)
+
+- [Python Reference](https://docs.apeworx.io/ape/latest/index.html)
+
+Ape is both a CLI tool and a Python SDK.
+
+The CLI tool contains all the Ape commands and the Python SDK contains the classes and types needed to compose scripts, console actions, and tests.
+
+## **Ape Modular Plugin System:**
+
+Our [list of plugins](https://www.apeworx.io/#plugins) is the best way to have the most interoperable experience with Web3.
+
+**NOTE**: If a plugin does not originate from the [ApeWorX GitHub Organization](https://github.com/ApeWorX?q=ape&type=all), you will get a warning about installing 3rd-party plugins.
+
+Install 3rd party plugins at your own risk.
+
+Additionally, plugins that come bundled with **`ape`** in the core installation cannot be removed and are part of the **`ape`** core software.
+
+- Learn more about **installing** plugins from following this [installing user guide](https://docs.apeworx.io/ape/stable/userguides/installing_plugins.html).
+
+- Learn more about **developing** your own plugins from this [developing user guide](https://docs.apeworx.io/ape/stable/userguides/developing_plugins.html).
+
+### Accounts
+
+In Ape, you will need accounts to make transactions.
+You can import or generate accounts using the core `accounts` plugin:
+
+```bash
+ape accounts import acc0   # Will prompt for a private key
+ape accounts generate acc1
+```
+
+List all your accounts with the `list` command.
+
+```bash
+ape accounts list
+```
+
+Learn more about accounts in Ape by following the [accounts guide](https://docs.apeworx.io/ape/stable/userguides/accounts.html).
+
+### Plugins
+
+Add any plugins you may need, such as `vyper`.
+
+```bash
+ape plugins list -a
+ape plugins install vyper
+ape plugins list -a
+```
+
+## Projects
+
+When using Ape, you generally will work with a project.
+
+Learn more about smart-contract **projects** from this [projects guide](https://docs.apeworx.io/ape/stable/userguides/projects.html).
+
+### Compiling
+
+You can compile contracts within the `contracts/` directory of your project.
+The `--size` option will display you the size of the contract.
+
+```bash
+ape compile --size
+```
+
+Learn more about compiling in Ape by following the [compile guide](https://docs.apeworx.io/ape/stable/userguides/compile.html).
+
+### Testing
+
+Use Ape to test your smart-contract projects.
+Provide the same arguments to `pytest` as you would to the `ape test` command.
+
+For example:
+
+```bash
+ape test -k test_only_one_thing
+```
+
+Visit the [testing guide](https://docs.apeworx.io/ape/stable/userguides/testing.html) to learn more about testing using Ape.
+
+### Console
+
+Ape provides an `IPython` interactive console with useful pre-defined locals to interact with your project.
+To interact with a deployed contract in a local environment, start by opening the console:
+
+```bash
+ape console --network ethereum:mainnet:infura
+```
+
+Visit [Ape Console](https://docs.apeworx.io/ape/stable/commands/console.html) to learn how to use Ape Console.
+
+### Scripts
+
+If you want to run specific files in a `scripts/` directory, you can do it using the `ape run` command.
+
+```bash
+# This command will run a file named deploy in the scripts/ directory
+$ ape run deploy
+```
+
+Learn more about scripting using Ape by following the [scripting guide](https://docs.apeworx.io/ape/stable/userguides/scripts.html).
+
+### Logging
+
+To enable debug logging, run your command with the `--verbosity` flag using `DEBUG` as the value:
+
+```bash
+ape --verbosity DEBUG run
+```
+
+### Networks
+
+You can work with registered networks, providers, and blockchain ecosystems (like Ethereum):
+
+```python
+from ape import networks
+with networks.ethereum.mainnet.use_provider("infura"):
+    ...  # Work with the infura provider here
+```
+
+To learn more about networks in Ape, see [this guide](https://docs.apeworx.io/ape/stable/commands/networks.html).
```

### Comparing `eth-ape-0.6.8/README.md` & `eth-ape-0.6.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,49 +4,49 @@
 Users can compile, test, and interact with smart contracts all in one command line session.
 With our **modular plugin system**, Ape supports multiple contract languages and chains.
 
 Ape is built by [ApeWorX LTD](https://www.apeworx.io/).
 
 Join our [ApeWorX Discord server](https://discord.gg/apeworx) to stay up to date on new releases, plugins and tutorials.
 
-If you want to just get started, jump down to the [Playing with Ape](#playing-with-ape)
+If you want to just get started, jump down to the [Playing with Ape](#playing-with-ape).
 
 ## Documentation
 
 Read our [technical documentation](https://docs.apeworx.io/ape/stable/) to get a deeper understanding of our open source Framework.
 
 Read our [academic platform](https://academy.apeworx.io/) will help you master Ape Framework with tutorials and challenges.
 
 ## Prerequisite
 
 In the latest release, Ape requires:
 
 - Linux or macOS
-- Python 3.8 or later
-- **Windows**: Install Windows Subsystem Linux [(WSL)](https://docs.microsoft.com/en-us/windows/wsl/install) with Python 3.8 or later
+- Python 3.8 up to 3.11
+- **Windows**: Install Windows Subsystem Linux [(WSL)](https://docs.microsoft.com/en-us/windows/wsl/install)
 
-Check your python version in a terminal with `python3 --version`
+Check your python version in a terminal with `python3 --version`.
 
 ## Installation
 
 There are three ways to install ape: `pipx`, `pip`, or `Docker`.
 
 ### Considerations for Installing:
 
 - We advise installing in a [virtualenv](https://pypi.org/project/virtualenv/) or [venv](https://docs.python.org/3/library/venv.html) to avoid interfering with *OS-level site packages*.
 
-- We advise installing **`ape`** with recommended plugins `pip install eth-ape'[recommended-plugins]'`
+- We advise installing **`ape`** with recommended plugins `pip install eth-ape'[recommended-plugins]'`.
 
-- We advise for **macOS** users to install virtual env via [homebrew](https://formulae.brew.sh/formula/virtualenv)
+- We advise for **macOS** users to install virtual env via [homebrew](https://formulae.brew.sh/formula/virtualenv).
 
 ### via `pipx` or `pip`
 
-1. Install `pipx` via their [installation instructions](https://pypa.github.io/pipx/) or `pip` via their [installation instructions](https://pip.pypa.io/en/stable/cli/pip_install/)
+1. Install `pipx` via their [installation instructions](https://pypa.github.io/pipx/) or `pip` via their [installation instructions](https://pip.pypa.io/en/stable/cli/pip_install/).
 
-2. Install **`ape`** via `pipx install eth-ape` or `pip install eth-ape`
+2. Install **`ape`** via `pipx install eth-ape` or `pip install eth-ape`.
 
 ### via `docker`
 
 Ape can also run in a docker container.
 
 Please visit our [Dockerhub](https://hub.docker.com/repository/docker/apeworx/ape) for more details on using Ape with Docker.
```

### Comparing `eth-ape-0.6.8/SECURITY.md` & `eth-ape-0.6.9/SECURITY.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/build_docs.py` & `eth-ape-0.6.9/build_docs.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/_static/custom.css` & `eth-ape-0.6.9/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/_static/custom.js` & `eth-ape-0.6.9/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/_templates/layout.html` & `eth-ape-0.6.9/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/conf.py` & `eth-ape-0.6.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/favicon.ico` & `eth-ape-0.6.9/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/index.md` & `eth-ape-0.6.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/logo.gif` & `eth-ape-0.6.9/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/methoddocs/api.md` & `eth-ape-0.6.9/docs/methoddocs/api.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/methoddocs/cli.md` & `eth-ape-0.6.9/docs/methoddocs/cli.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/methoddocs/contracts.md` & `eth-ape-0.6.9/docs/methoddocs/contracts.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/methoddocs/managers.md` & `eth-ape-0.6.9/docs/methoddocs/managers.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/methoddocs/plugins.md` & `eth-ape-0.6.9/docs/methoddocs/plugins.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/userguides/accounts.md` & `eth-ape-0.6.9/docs/userguides/accounts.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/userguides/compile.md` & `eth-ape-0.6.9/docs/userguides/compile.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/userguides/config.md` & `eth-ape-0.6.9/docs/userguides/config.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/userguides/console.md` & `eth-ape-0.6.9/docs/userguides/console.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/userguides/contracts.md` & `eth-ape-0.6.9/docs/userguides/contracts.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/userguides/data.md` & `eth-ape-0.6.9/docs/userguides/data.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/userguides/developing_plugins.md` & `eth-ape-0.6.9/docs/userguides/developing_plugins.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/userguides/installing_plugins.md` & `eth-ape-0.6.9/docs/userguides/installing_plugins.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/userguides/networks.md` & `eth-ape-0.6.9/docs/userguides/networks.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/userguides/projects.md` & `eth-ape-0.6.9/docs/userguides/projects.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/userguides/publishing.md` & `eth-ape-0.6.9/docs/userguides/publishing.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/userguides/scripts.md` & `eth-ape-0.6.9/docs/userguides/scripts.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/docs/userguides/testing.md` & `eth-ape-0.6.9/docs/userguides/testing.md`

 * *Files 3% similar despite different names*

```diff
@@ -165,14 +165,26 @@
 def my_contract(project, owner):
     #           ^ use the 'project' fixture from the 'ape-test' plugin
     return owner.deploy(project.MyContract)
 ```
 
 It has the same interface as the [ProjectManager](../methoddocs/managers.html#module-ape.managers.project.manager).
 
+### Contract fixture
+
+Use the `Contract` fixture to create contract instances:
+
+```python
+@pytest.fixture
+def my_contract(Contract):
+    return Contract(<address>)
+```
+
+It has the same interface as the [ChainManager](../methoddocs/managers.html#ape.managers.chain.ChainManager).
+
 ## Ape testing commands
 
 ```bash
 ape test
 ```
 
 To run a particular test:
@@ -382,32 +394,50 @@
 def test_unauthorized_withdraw(contract, hacker):
     with ape.reverts(contract.Unauthorized, addr=hacker.address):
         contract.withdraw(sender=hacker)
 ```
 
 ## Multi-chain Testing
 
-The Ape framework supports connecting to alternative providers in tests.
-The easiest way to achieve this is to use the `networks` provider context-manager.
+The Ape framework supports connecting to alternative networks / providers in tests.
+
+To run an entire test using a specific network / provider combination, use the `use_network` pytest marker:
+
+```python
+import pytest
+
+
+@pytest.mark.use_network("fantom:local:test")
+def test_my_fantom_test(chain):
+    assert chain.provider.network.ecosystem.name == "fantom"
+
+
+@pytest.mark.use_network("ethereum:local:test")
+def test_my_ethereum_test(chain):
+    assert chain.provider.network.ecosystem.name == "ethereum"
+```
+
+To switch networks mid-test, use the `networks` context-manager:
 
 ```python
 # Switch to Fantom mid test
-def test_my_fantom_test(networks):
+def test_my_multichain_test(networks):
     # The test starts in 1 ecosystem but switches to another
     assert networks.provider.network.ecosystem.name == "ethereum"
 
     with networks.fantom.local.use_provider("test") as provider:
         assert provider.network.ecosystem.name == "fantom"
 
     # You can also use the context manager like this:
     with networks.parse_network_choice("fantom:local:test") as provider:
        assert provider.network.ecosystem.name == "fantom"
 ```
 
-You can also set the network context in a context-manager pytest fixture:
+You can also set the network context in a pytest fixture.
+This is useful if certain fixtures must run in certain networks.
 
 ```python
 import pytest
 
 
 @pytest.fixture
 def stark_contract(networks, project):
```

### Comparing `eth-ape-0.6.8/docs/userguides/transactions.md` & `eth-ape-0.6.9/docs/userguides/transactions.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/pyproject.toml` & `eth-ape-0.6.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/setup.py` & `eth-ape-0.6.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         "pytest-cov>=4.0.0,<5",  # Coverage analyzer plugin
         "pytest-mock",  # For creating mocks
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
         "hypothesis-jsonschema==0.19.0",  # JSON Schema fuzzer extension
     ],
     "lint": [
         "black>=23.3.0,<24",  # Auto-formatter and linter
-        "mypy>=0.991",  # Static type analyzer
+        "mypy>=0.991,<1",  # Static type analyzer
         "types-PyYAML",  # Needed due to mypy typeshed
         "types-requests",  # Needed due to mypy typeshed
         "types-setuptools",  # Needed due to mypy typeshed
         "pandas-stubs==1.2.0.62",  # Needed due to mypy typeshed
         "types-SQLAlchemy>=1.4.49",  # Needed due to mypy typeshed
         "flake8>=6.0.0,<7",  # Style linter
         "flake8-breakpoint>=1.1.0,<2",  # detect breakpoints left in code
@@ -92,40 +92,41 @@
     },
     include_package_data=True,
     install_requires=[
         "click>=8.1.3,<9",
         "ijson>=3.1.4,<4",
         "importlib-metadata",
         "ipython>=8.5.0,<9",
+        "lazyasd>=0.1.4",
         "packaging>=23.0,<24",
         "pandas>=1.3.0,<2",
         "pluggy>=0.12,<2",
         "pydantic>=1.9.2,<2",
         "PyGithub>=1.54,<2",
         "pytest>=6.0,<8.0",
         "python-dateutil>=2.8.2,<3",
-        "pyyaml>=6.0,<7",
+        "PyYAML>=5.0,<7",
         "requests>=2.28.1,<3",
         "rich>=12.5.1,<13",
         "SQLAlchemy>=1.4.35",
         "tqdm>=4.62.3,<5.0",
         "traitlets>=5.3.0",
         "watchdog>=2.1.9,<3.0",
         # ** Dependencies maintained by Ethereum Foundation **
         "eth-abi>=4.0.0,<5",
         "eth-account>=0.8,<0.9",
         "eth-typing>=3.1,<4",
         "eth-utils>=2.0.0,<3",
         "hexbytes>=0.2.3,<1",
         "py-geth>=3.12.0,<4",
-        "web3[tester]>=6.0.0,<7",
+        "web3[tester]>=6.4.0,<7",
         # ** Dependencies maintained by ApeWorX **
         "eip712>=0.2.1,<0.3",
-        "ethpm-types>=0.4.3,<0.5",
-        "evm-trace>=0.1.0a17",
+        "ethpm-types>=0.5.0,<0.6",
+        "evm-trace>=0.1.0a20",
     ],
     entry_points={
         "console_scripts": ["ape=ape._cli:cli"],
         "pytest11": ["ape_test=ape.pytest.plugin"],
         "ape_cli_subcommands": [
             "ape_accounts=ape_accounts._cli:cli",
             "ape_cache=ape_cache._cli:cli",
@@ -134,15 +135,15 @@
             "ape_plugins=ape_plugins._cli:cli",
             "ape_run=ape_run._cli:cli",
             "ape_networks=ape_networks._cli:cli",
             "ape_test=ape_test._cli:cli",
             "ape_init=ape_init._cli:cli",
         ],
     },
-    python_requires=">=3.8,<3.11",
+    python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=packages_data["__modules__"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages("src"),
     package_dir={"": "src"},
@@ -154,9 +155,10 @@
         "Natural Language :: English",
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `eth-ape-0.6.8/src/ape/__init__.py` & `eth-ape-0.6.9/src/ape/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/_cli.py` & `eth-ape-0.6.9/src/ape/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/api/__init__.py` & `eth-ape-0.6.9/src/ape/api/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/api/accounts.py` & `eth-ape-0.6.9/src/ape/api/accounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,14 +172,16 @@
             raise AccountsError("Must provide 'VALUE' or use 'send_everything=True'")
 
         elif value and kwargs.get("send_everything"):
             raise AccountsError("Cannot use 'send_everything=True' with 'VALUE'.")
 
         elif value:
             txn.value = self.conversion_manager.convert(value, int)
+            if txn.value < 0:
+                raise AccountsError("Value cannot be negative.")
 
         return self.call(txn, **kwargs)
 
     def deploy(
         self, contract: "ContractContainer", *args, publish: bool = False, **kwargs
     ) -> "ContractInstance":
         """
@@ -464,8 +466,9 @@
         # Returns input transaction unsigned (since it doesn't have access to the key)
         return txn
 
     def call(self, txn: TransactionAPI, send_everything: bool = False, **kwargs) -> ReceiptAPI:
         txn = self.prepare_transaction(txn)
         if not txn.sender:
             txn.sender = self.raw_address
+
         return self.provider.send_transaction(txn)
```

### Comparing `eth-ape-0.6.8/src/ape/api/address.py` & `eth-ape-0.6.9/src/ape/api/address.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/api/compiler.py` & `eth-ape-0.6.9/src/ape/api/compiler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from pathlib import Path
-from typing import Dict, List, Optional, Set
+from typing import Dict, Iterator, List, Optional, Set, Tuple
 
-from ethpm_types import ContractType
+from ethpm_types import ContractType, HexBytes
+from ethpm_types.source import ContractSource
+from evm_trace.geth import TraceFrame as EvmTraceFrame
+from evm_trace.geth import create_call_node_data
 from semantic_version import Version  # type: ignore
 
 from ape.exceptions import ContractLogicError
+from ape.types.trace import SourceTraceback, TraceFrame
 from ape.utils import BaseInterfaceModel, abstractmethod, raises_not_implemented
 
 
 class CompilerAPI(BaseInterfaceModel):
     """
     Compiler plugins, such as for languages like
     `Solidity <https://docs.soliditylang.org/en/v0.8.11/>`__ or
@@ -121,7 +125,39 @@
               to enrich.
 
         Returns:
             :class:`~ape.exceptions.ContractLogicError`: The enriched exception.
         """
 
         return err
+
+    @raises_not_implemented
+    def trace_source(  # type: ignore[empty-body]
+        self, contract_type: ContractType, trace: Iterator[TraceFrame], calldata: HexBytes
+    ) -> SourceTraceback:
+        """
+        Get a source-traceback for the given contract type.
+        The source traceback object contains all the control paths taken in the transaction.
+        When available, source-code location information is accessible from the object.
+
+        Args:
+            contract_type (``ContractType``): A contract type that was created by this compiler.
+            trace (Iterator[:class:`~ape.types.trace.TraceFrame`]): The resulting frames from
+              executing a function defined in the given contract type.
+            calldata (``HexBytes``): Calldata passed to the top-level call.
+
+        Returns:
+            :class:`~ape.types.trace.SourceTraceback`
+        """
+
+    def _create_contract_from_call(
+        self, frame: TraceFrame
+    ) -> Tuple[Optional[ContractSource], HexBytes]:
+        evm_frame = EvmTraceFrame(**frame.raw)
+        data = create_call_node_data(evm_frame)
+        calldata = data["calldata"]
+        address = self.provider.network.ecosystem.decode_address(data["address"])
+        if address not in self.chain_manager.contracts:
+            return None, calldata
+
+        called_contract = self.chain_manager.contracts[address]
+        return self.project_manager._create_contract_source(called_contract), calldata
```

### Comparing `eth-ape-0.6.8/src/ape/api/config.py` & `eth-ape-0.6.9/src/ape/api/config.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/api/convert.py` & `eth-ape-0.6.9/src/ape/api/convert.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/api/explorers.py` & `eth-ape-0.6.9/src/ape/api/explorers.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/api/networks.py` & `eth-ape-0.6.9/src/ape/api/networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,17 +246,15 @@
         Attach a new network to an ecosystem (e.g. L2 networks like Optimism).
 
         Raises:
             :class:`~ape.exceptions.NetworkError`: When the network already exists.
 
         Args:
             network_name (str): The name of the network to add.
-
-        Returns:
-            :class:`~ape.api.networks.NetworkAPI`
+            network (:class:`~ape.api.networks.NetworkAPI`): The network to add.
         """
         if network_name in self.networks:
             raise NetworkError(f"Unable to overwrite existing network '{network_name}'.")
         else:
             self.networks[network_name] = network
 
     @property
@@ -415,18 +413,19 @@
         Raises:
               :class:`~ape.exceptions.NetworkNotFoundError`: When the network is not present.
 
         Returns:
               :class:`~ape.api.networks.NetworkAPI`
         """
 
-        if network_name in self.networks:
-            return self.networks[network_name]
-        else:
-            raise NetworkNotFoundError(network_name)
+        name = network_name.replace("_", "-")
+        if name in self.networks:
+            return self.networks[name]
+
+        raise NetworkNotFoundError(network_name)
 
     def get_network_data(self, network_name: str) -> Dict:
         """
         Get a dictionary of data about providers in the network.
 
         **NOTE**: The keys are added in an opinionated order for nicely
         translating into ``yaml``.
@@ -672,15 +671,15 @@
         for more information on plugin configurations.
         """
 
         return self.config_manager.get_config(self.ecosystem.name)
 
     @property
     def _network_config(self) -> Dict:
-        return self.config.get(self.name, {})
+        return self.config.get(self.name.replace("-", "_"), {})
 
     @cached_property
     def gas_limit(self) -> GasLimit:
         return self._network_config.get("gas_limit", "auto")
 
     @property
     def chain_id(self) -> int:
```

### Comparing `eth-ape-0.6.8/src/ape/api/projects.py` & `eth-ape-0.6.9/src/ape/api/projects.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os.path
 import tempfile
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 import yaml
 from ethpm_types import Checksum, ContractType, PackageManifest, Source
 from ethpm_types.manifest import PackageName
 from ethpm_types.utils import AnyUrl, compute_checksum
 from packaging.version import InvalidVersion, Version
 from pydantic import ValidationError
@@ -167,25 +167,28 @@
         manifest.version = version or manifest.version
         manifest.sources = cls._create_source_dict(source_paths, contracts_path)
         manifest.contract_types = contract_types
         return manifest
 
     @classmethod
     def _create_source_dict(
-        cls, contract_filepaths: List[Path], base_path: Path
+        cls, contract_filepaths: Union[Path, List[Path]], base_path: Path
     ) -> Dict[str, Source]:
+        filepaths = (
+            [contract_filepaths] if isinstance(contract_filepaths, Path) else contract_filepaths
+        )
         source_imports: Dict[str, List[str]] = cls.compiler_manager.get_imports(
-            contract_filepaths, base_path
+            filepaths, base_path
         )  # {source_id: [import_source_ids, ...], ...}
         source_references: Dict[str, List[str]] = cls.compiler_manager.get_references(
             imports_dict=source_imports
         )  # {source_id: [referring_source_ids, ...], ...}
 
         source_dict: Dict[str, Source] = {}
-        for source_path in contract_filepaths:
+        for source_path in filepaths:
             key = str(get_relative_path(source_path, base_path))
             source_dict[key] = Source(
                 checksum=Checksum(
                     algorithm="md5",
                     hash=compute_checksum(source_path.read_bytes()),
                 ),
                 urls=[],
@@ -350,15 +353,15 @@
                 source_path = contracts_folder / get_relative_path(
                     absolute_path, contracts_folder.absolute()
                 )
 
                 # Create content, including sub-directories.
                 source_path.parent.mkdir(parents=True, exist_ok=True)
                 source_path.touch()
-                source_path.write_text(content)
+                source_path.write_text(str(content))
 
             # Handle import remapping entries indicated in the manifest file
             target_config_file = project.path / project.config_file_name
             packages_used = set()
             config_data: Dict[str, Any] = {}
             for compiler in [x for x in manifest.compilers or [] if x.settings]:
                 name = compiler.name.lower()
@@ -396,14 +399,16 @@
 
                 dependency = {"name": str(package_name)}
                 if uri_str.startswith("https://"):
                     # Assume GitHub dependency
                     version = uri_str.split("/")[-1]
                     dependency["github"] = uri_str.replace(f"/releases/tag/{version}", "")
                     dependency["github"] = dependency["github"].replace("https://github.com/", "")
+
+                    # NOTE: If version fails, the dependency system will automatically try `ref`.
                     dependency["version"] = version
 
                 elif uri_str.startswith("file://"):
                     dependency["local"] = uri_str.replace("file://", "")
 
                 dependencies_config.append(dependency)
```

### Comparing `eth-ape-0.6.8/src/ape/api/providers.py` & `eth-ape-0.6.9/src/ape/api/providers.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import logging
 import platform
 import shutil
 import sys
 import time
 from abc import ABC
 from concurrent.futures import ThreadPoolExecutor
+from copy import copy
 from itertools import tee
 from logging import FileHandler, Formatter, Logger, getLogger
 from pathlib import Path
 from signal import SIGINT, SIGTERM, signal
 from subprocess import DEVNULL, PIPE, Popen
 from typing import Any, Dict, Iterator, List, Optional, Union, cast
 
@@ -20,26 +21,27 @@
 from evm_trace import CallTreeNode as EvmCallTreeNode
 from evm_trace import TraceFrame as EvmTraceFrame
 from hexbytes import HexBytes
 from pydantic import Field, root_validator, validator
 from web3 import Web3
 from web3.exceptions import BlockNotFound
 from web3.exceptions import ContractLogicError as Web3ContractLogicError
-from web3.exceptions import TimeExhausted
+from web3.exceptions import MethodUnavailable, TimeExhausted
 from web3.types import RPCEndpoint, TxParams
 
 from ape.api.config import PluginConfig
 from ape.api.networks import LOCAL_NETWORK_NAME, NetworkAPI
 from ape.api.query import BlockTransactionQuery
 from ape.api.transactions import ReceiptAPI, TransactionAPI
 from ape.exceptions import (
     ApeException,
     APINotImplementedError,
     BlockNotFoundError,
     ContractLogicError,
+    OutOfGasError,
     ProviderError,
     ProviderNotConnectedError,
     RPCTimeoutError,
     SubprocessError,
     SubprocessTimeoutError,
     TransactionError,
     TransactionNotFoundError,
@@ -699,14 +701,18 @@
             provider's network has been configured with a gas limit override, it
             will be returned. If the gas limit configuration is "max" this will
             return the block maximum gas limit.
         """
 
         txn_dict = txn.dict()
 
+        # Force the use of hex values to support a wider range of nodes.
+        if isinstance(txn_dict.get("type"), int):
+            txn_dict["type"] = HexBytes(txn_dict["type"]).hex()
+
         # NOTE: "auto" means to enter this method, so remove it from dict
         if "gas" in txn_dict and txn_dict["gas"] == "auto":
             txn_dict.pop("gas")
             # Also pop these, they are overriden by "auto"
             txn_dict.pop("maxFeePerGas", None)
             txn_dict.pop("maxPriorityFeePerGas", None)
 
@@ -752,15 +758,21 @@
 
     @property
     def gas_price(self) -> int:
         return self._web3.eth.generate_gas_price()  # type: ignore
 
     @property
     def priority_fee(self) -> int:
-        return self.web3.eth.max_priority_fee
+        try:
+            return self.web3.eth.max_priority_fee
+        except MethodUnavailable as err:
+            # The user likely should be using a more-catered plugin.
+            raise APINotImplementedError(
+                "eth_maxPriorityFeePerGas not supported in this RPC. Please specify manually."
+            ) from err
 
     def get_block(self, block_id: BlockID) -> BlockAPI:
         if isinstance(block_id, str) and block_id.isnumeric():
             block_id = int(block_id)
 
         try:
             block_data = dict(self.web3.eth.get_block(block_id))
@@ -843,15 +855,15 @@
         Returns:
             str: The result of the transaction call.
         """
         skip_trace = kwargs.pop("skip_trace", False)
         if skip_trace:
             return self._send_call(txn, **kwargs)
 
-        track_gas = self.chain_manager._reports.track_gas
+        track_gas = self._test_runner is not None and self._test_runner.gas_tracker.enabled
         show_trace = kwargs.pop("show_trace", False)
         show_gas = kwargs.pop("show_gas_report", False)
         needs_trace = track_gas or show_trace or show_gas
         if not needs_trace or not self.provider.supports_tracing or not txn.receiver:
             return self._send_call(txn, **kwargs)
 
         # The user is requesting information related to a call's trace,
@@ -901,14 +913,23 @@
         return HexBytes(returndata)
 
     def _send_call(self, txn: TransactionAPI, **kwargs) -> bytes:
         arguments = self._prepare_call(txn, **kwargs)
         return self._eth_call(arguments)
 
     def _eth_call(self, arguments: List) -> bytes:
+        # Force the usage of hex-type to support a wider-range of nodes.
+        txn_dict = copy(arguments[0])
+        if isinstance(txn_dict.get("type"), int):
+            txn_dict["type"] = HexBytes(txn_dict["type"]).hex()
+
+        # Remove unnecessary values to support a wider-range of nodes.
+        txn_dict.pop("chainId", None)
+
+        arguments[0] = txn_dict
         try:
             result = self._make_request("eth_call", arguments)
         except Exception as err:
             raise self.get_virtual_machine_error(err) from err
 
         if "error" in result:
             raise ProviderError(result["error"]["message"])
@@ -1190,22 +1211,26 @@
             inputs=evm_call.calldata[4:].hex(),
             method_id=evm_call.calldata[:4].hex(),
             outputs=evm_call.returndata.hex(),
             raw=evm_call.dict(),
             txn_hash=txn_hash,
         )
 
-    @classmethod
-    def _create_trace_frame(cls, evm_frame: EvmTraceFrame) -> TraceFrame:
+    def _create_trace_frame(self, evm_frame: EvmTraceFrame) -> TraceFrame:
+        address_bytes = evm_frame.address
+        address = (
+            self.network.ecosystem.decode_address(address_bytes.hex()) if address_bytes else None
+        )
         return TraceFrame(
             pc=evm_frame.pc,
             op=evm_frame.op,
             gas=evm_frame.gas,
             gas_cost=evm_frame.gas_cost,
             depth=evm_frame.depth,
+            contract_address=address,
             raw=evm_frame.dict(),
         )
 
     def _make_request(self, endpoint: str, parameters: List) -> Any:
         coroutine = self.web3.provider.make_request(RPCEndpoint(endpoint), parameters)
         result = run_until_complete(coroutine)
 
@@ -1261,14 +1286,17 @@
         if txn is not None and "nonce too low" in str(err_msg):
             txn = cast(TransactionAPI, txn)
             new_err_msg = f"Nonce '{txn.nonce}' is too low"
             return VirtualMachineError(
                 new_err_msg, base_err=exception, code=err_data.get("code"), **kwargs
             )
 
+        elif "out of gas" in str(err_msg):
+            return OutOfGasError(code=err_data.get("code"), **kwargs)
+
         return VirtualMachineError(str(err_msg), code=err_data.get("code"), **kwargs)
 
     def _handle_execution_reverted(
         self,
         exception: Union[Exception, str],
         txn: Optional[TransactionAPI] = None,
         trace: Optional[Iterator[TraceFrame]] = None,
```

### Comparing `eth-ape-0.6.8/src/ape/api/query.py` & `eth-ape-0.6.9/src/ape/api/query.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/api/transactions.py` & `eth-ape-0.6.9/src/ape/api/transactions.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,21 @@
     NetworkError,
     ProviderNotConnectedError,
     SignatureError,
     TransactionError,
     TransactionNotFoundError,
 )
 from ape.logging import logger
-from ape.types import AddressType, ContractLogContainer, TraceFrame, TransactionSignature
+from ape.types import (
+    AddressType,
+    ContractLogContainer,
+    SourceTraceback,
+    TraceFrame,
+    TransactionSignature,
+)
 from ape.utils import BaseInterfaceModel, abstractmethod, cached_property, raises_not_implemented
 
 if TYPE_CHECKING:
     from ape.api.providers import BlockAPI
     from ape.contracts import ContractEvent
 
 
@@ -125,14 +131,26 @@
             return None
 
         try:
             return self.provider.get_receipt(txn_hash, required_confirmations=0, timeout=0)
         except (TransactionNotFoundError, ProviderNotConnectedError):
             return None
 
+    @property
+    def trace(self) -> Iterator[TraceFrame]:
+        """
+        The transaction trace. Only works if this transaction was published
+        and you are using a provider that support tracing.
+
+        Raises:
+            :class:`~ape.exceptions.APINotImplementedError`: When using a provider
+              that does not support tracing.
+        """
+        return self.provider.get_transaction_trace(self.txn_hash.hex())
+
     @abstractmethod
     def serialize_transaction(self) -> bytes:
         """
         Serialize the transaction
         """
 
     def __repr__(self) -> str:
@@ -424,14 +442,23 @@
             output = call_tree.outputs
 
         if isinstance(output, tuple) and len(output) < 2:
             output = output[0] if len(output) == 1 else None
 
         return output
 
+    @property
+    @raises_not_implemented
+    def source_traceback(self) -> SourceTraceback:  # type: ignore[empty-body]
+        """
+        A pythonic style traceback for both failing and non-failing receipts.
+        Requires a provider that implements
+        :meth:~ape.api.providers.ProviderAPI.get_transaction_trace`.
+        """
+
     @raises_not_implemented
     def show_trace(self, verbose: bool = False, file: IO[str] = sys.stdout):
         """
         Display the complete sequence of contracts and methods called during
         the transaction.
 
         Args:
@@ -441,18 +468,27 @@
 
     @raises_not_implemented
     def show_gas_report(self, file: IO[str] = sys.stdout):
         """
         Display a gas report for the calls made in this transaction.
         """
 
+    @raises_not_implemented
+    def show_source_traceback(self):
+        """
+        Show a receipt traceback mapping to lines in the source code.
+        Only works when the contract type and source code are both available,
+        like in local projects.
+        """
+
     def track_gas(self):
         """
         Track this receipt's gas in the on-going session gas-report.
         Requires using a provider that support transaction traces.
         This gets called when running tests with the ``--gas`` flag.
         """
 
         call_tree = self.call_tree
         receiver = self.receiver
-        if call_tree and receiver is not None:
-            self.chain_manager._reports.append_gas(call_tree.enrich(in_line=False), receiver)
+        if call_tree and receiver is not None and self._test_runner is not None:
+            tracker = self._test_runner.gas_tracker
+            tracker.append_gas(call_tree.enrich(in_line=False), receiver)
```

### Comparing `eth-ape-0.6.8/src/ape/cli/__init__.py` & `eth-ape-0.6.9/src/ape/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/cli/arguments.py` & `eth-ape-0.6.9/src/ape/cli/arguments.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/cli/choices.py` & `eth-ape-0.6.9/src/ape/cli/choices.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/cli/options.py` & `eth-ape-0.6.9/src/ape/cli/options.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/cli/paramtype.py` & `eth-ape-0.6.9/src/ape/cli/paramtype.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/contracts/base.py` & `eth-ape-0.6.9/src/ape/contracts/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,19 @@
 
     def __init__(self, contract: "ContractInstance", abis: List[MethodABI]) -> None:
         super().__init__()
         self.contract = contract
         self.abis = abis
 
     def __repr__(self) -> str:
+        # `<ContractName 0x1234...AbCd>.method_name`
+        return f"{self.contract.__repr__()}.{self.abis[-1].name}"
+
+    def __str__(self) -> str:
+        # `method_name(type1 arg1, ...) -> return_type`
         abis = sorted(self.abis, key=lambda abi: len(abi.inputs or []))
         return abis[-1].signature
 
     def encode_input(self, *args) -> HexBytes:
         selected_abi = _select_method_abi(self.abis, args)
         args = self._convert_tuple(args, selected_abi)
         ecosystem = self.provider.network.ecosystem
@@ -634,14 +639,42 @@
             # Get all events in the new block.
             yield from self.range(new_block.number, stop=new_block.number + 1)
 
 
 class ContractTypeWrapper(ManagerAccessMixin):
     contract_type: ContractType
 
+    @cached_property
+    def source_path(self) -> Optional[Path]:
+        """
+        Returns the path to the local contract if determined that this container
+        belongs to the active project by cross checking source_id.
+
+        WARN: The will return a path if the contract has the same
+        source ID as one in the current project. That does not necessarily mean
+        they are the same contract, however.
+        """
+        contract_name = self.contract_type.name
+        source_id = self.contract_type.source_id
+        if not (contract_name and source_id):
+            return None
+
+        contract_container = self.project_manager._get_contract(contract_name)
+        if not (
+            contract_container
+            and contract_container.contract_type.source_id
+            and self.contract_type.source_id
+        ):
+            return None
+
+        if source_id == contract_container.contract_type.source_id:
+            return self.project_manager.contracts_folder / source_id
+        else:
+            return None
+
     def decode_input(self, calldata: bytes) -> Tuple[str, Dict[str, Any]]:
         """
         Decode the given calldata using this contract.
         If the calldata has a method ID prefix, Ape will detect it and find
         the corresponding method, else it will error.
 
         Args:
@@ -724,15 +757,15 @@
         The receipt associated with deploying the contract instance,
         if it is known and exists.
         """
 
         if not self._cached_receipt and self.txn_hash:
             try:
                 receipt = self.chain_manager.get_receipt(self.txn_hash)
-            except TransactionNotFoundError:
+            except (TransactionNotFoundError, ValueError):
                 return None
 
             self._cached_receipt = receipt
             return receipt
 
         elif self._cached_receipt:
             return self._cached_receipt
@@ -1128,42 +1161,14 @@
         """
 
         return self.chain_manager.contracts.instance_at(
             address, self.contract_type, txn_hash=txn_hash
         )
 
     @cached_property
-    def source_path(self) -> Optional[Path]:
-        """
-        Returns the path to the local contract if determined that this container
-        belongs to the active project by cross checking source_id.
-
-        WARN: The will return a path if the contract has the same
-        source ID as one in the current project. That does not necessarily mean
-        they are the same contract, however.
-        """
-        contract_name = self.contract_type.name
-        source_id = self.contract_type.source_id
-        if not (contract_name and source_id):
-            return None
-
-        contract_container = self.project_manager._get_contract(contract_name)
-        if not (
-            contract_container
-            and contract_container.contract_type.source_id
-            and self.contract_type.source_id
-        ):
-            return None
-
-        if source_id == contract_container.contract_type.source_id:
-            return self.project_manager.contracts_folder / source_id
-        else:
-            return None
-
-    @cached_property
     def constructor(self) -> ContractConstructor:
         return ContractConstructor(
             abi=self.contract_type.constructor,
             deployment_bytecode=self.contract_type.get_deployment_bytecode() or HexBytes(""),
         )
 
     def __call__(self, *args, **kwargs) -> TransactionAPI:
```

### Comparing `eth-ape-0.6.8/src/ape/exceptions.py` & `eth-ape-0.6.9/src/ape/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import sys
+import tempfile
 import time
 import traceback
 from collections import deque
 from functools import cached_property
 from inspect import getframeinfo, stack
-from itertools import tee
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional
+from types import CodeType, TracebackType
+from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional, Union
 
 import click
 from eth_utils import humanize_hash
+from ethpm_types import ContractType
 from ethpm_types.abi import ErrorABI
 from rich import print as rich_print
 
 from ape.logging import LogLevel, logger
 
 if TYPE_CHECKING:
     from ape.api.networks import NetworkAPI
     from ape.api.providers import SubprocessProvider
-    from ape.api.transactions import TransactionAPI
-    from ape.types import AddressType, BlockID, SnapshotID, TraceFrame
-    from ape.utils.basemodel import ManagerAccessMixin
+    from ape.api.transactions import ReceiptAPI, TransactionAPI
+    from ape.types import AddressType, BlockID, SnapshotID, SourceTraceback, TraceFrame
+
+
+FailedTxn = Union["TransactionAPI", "ReceiptAPI"]
 
 
 class ApeException(Exception):
     """
     An exception raised by ape.
     """
 
@@ -98,28 +102,43 @@
     DEFAULT_MESSAGE = "Transaction failed."
 
     def __init__(
         self,
         message: Optional[str] = None,
         base_err: Optional[Exception] = None,
         code: Optional[int] = None,
-        txn: Optional["TransactionAPI"] = None,
+        txn: Optional[FailedTxn] = None,
         trace: Optional[Iterator["TraceFrame"]] = None,
         contract_address: Optional["AddressType"] = None,
     ):
         message = message or (str(base_err) if base_err else self.DEFAULT_MESSAGE)
         self.message = message
         self.base_err = base_err
         self.code = code
         self.txn = txn
         self.trace = trace
         self.contract_address = contract_address
+        self.source_traceback: Optional["SourceTraceback"] = None
         ex_message = f"({code}) {message}" if code else message
+
+        # Finalizes expected revert message.
         super().__init__(ex_message)
 
+        if not txn:
+            return
+
+        ape_tb = _get_ape_traceback(txn)
+        if not ape_tb:
+            return
+
+        self.source_traceback = ape_tb
+        py_tb = _get_custom_python_traceback(self, txn, ape_tb)
+        if py_tb:
+            self.__traceback__ = py_tb
+
 
 class VirtualMachineError(TransactionError):
     """
     Raised when a transaction error occurs in a virtual machine.
     """
 
 
@@ -128,15 +147,15 @@
     Raised when there is a contract-defined revert,
     such as from an assert/require statement.
     """
 
     def __init__(
         self,
         revert_message: Optional[str] = None,
-        txn: Optional["TransactionAPI"] = None,
+        txn: Optional[FailedTxn] = None,
         trace: Optional[Iterator["TraceFrame"]] = None,
         contract_address: Optional["AddressType"] = None,
     ):
         self.txn = txn
         self.trace = trace
         self.contract_address = contract_address
         if revert_message is None:
@@ -159,99 +178,118 @@
         """
         The dev-string message of the exception.
 
         Raises:
             ``ValueError``: When unable to get dev message.
         """
 
-        accessor: Optional["ManagerAccessMixin"] = None
-        if self.txn:
-            accessor = self.txn
-        elif self.trace is not None:
-            self.trace, second_trace = tee(self.trace)
-            if second_trace:
-                accessor = next(second_trace, None)
-
-        if accessor is None:
-            raise ValueError("Missing trace access.")
+        trace = self._get_trace()
+        if len(trace) == 0:
+            raise ValueError("Missing trace.")
 
         contract_address = self.contract_address or getattr(self.txn, "receiver", None)
         if not contract_address:
             raise ValueError("Could not fetch contract information to check dev message.")
 
         try:
-            contract = accessor.chain_manager.contracts.instance_at(contract_address)
+            contract_type = trace[-1].chain_manager.contracts[contract_address]
         except ValueError as err:
             raise ValueError(
                 f"Could not fetch contract at {contract_address} to check dev message."
             ) from err
 
-        if contract.contract_type.pcmap is None:
+        if contract_type.pcmap is None:
             raise ValueError("Compiler does not support source code mapping.")
 
-        if self.trace is None and self.txn is not None:
-            try:
-                trace = deque(accessor.provider.get_transaction_trace(self.txn.txn_hash.hex()))
-
-            except APINotImplementedError as err:
-                raise ValueError(
-                    "Cannot check dev message; " "provider must support transaction tracing."
-                ) from err
-
-            except (ProviderError, SignatureError) as err:
-                raise ValueError("Cannot fetch transaction trace.") from err
-
-        elif self.trace is not None:
-            trace = deque(self.trace)
-
-        else:
-            raise ValueError("Cannot fetch transaction trace.")
-
-        if trace is None:
-            raise ValueError("Cannot fetch transaction trace.")
-
         pc = None
-        pcmap = contract.contract_type.pcmap.parse()
+        pcmap = contract_type.pcmap.parse()
 
         # To find a suitable line for inspecting dev messages, we must start at the revert and work
         # our way backwards. If the last frame's PC is in the PC map, the offending line is very
         # likely a 'raise' statement.
         if trace[-1].pc in pcmap:
             pc = trace[-1].pc
 
         # Otherwise we must traverse the trace backwards until we find our first suitable candidate.
         else:
+            last_depth = 1
             while len(trace) > 0:
                 frame = trace.pop()
+                if frame.depth > last_depth:
+                    # Call was made, get the new PCMap.
+                    contract_type = self._find_next_contract(trace)
+                    if not contract_type.pcmap:
+                        raise ValueError("Compiler does not support source code mapping.")
+
+                    pcmap = contract_type.pcmap.parse()
+                    last_depth += 1
+
                 if frame.pc in pcmap:
                     pc = frame.pc
                     break
 
         # We were unable to find a suitable PC that matched the compiler's map.
         if pc is None:
             return None
 
         offending_source = pcmap[pc]
         if offending_source is None:
             return None
 
-        dev_messages = contract.contract_type.dev_messages or {}
+        dev_messages = contract_type.dev_messages or {}
         if offending_source.line_start is None:
             # Check for a `dev` field in PCMap.
             return None if offending_source.dev is None else offending_source.dev
 
         elif offending_source.line_start in dev_messages:
             return dev_messages[offending_source.line_start]
 
         elif offending_source.dev is not None:
             return offending_source.dev
 
         # Dev message is neither found from the compiler or from a dev-comment.
         return None
 
+    def _get_trace(self) -> deque:
+        trace = None
+        if self.trace is None and self.txn is not None:
+            try:
+                trace = deque(self.txn.trace)
+            except APINotImplementedError as err:
+                raise ValueError(
+                    "Cannot check dev message; provider must support transaction tracing."
+                ) from err
+
+            except (ProviderError, SignatureError) as err:
+                raise ValueError("Cannot fetch transaction trace.") from err
+
+        elif self.trace is not None:
+            trace = deque(self.trace)
+
+        if not trace:
+            raise ValueError("Cannot fetch transaction trace.")
+
+        return trace
+
+    def _find_next_contract(self, trace: deque) -> ContractType:
+        msg = "Could not fetch contract at '{address}' to check dev message."
+        idx = len(trace) - 1
+        while idx >= 0:
+            frame = trace[idx]
+            if frame.contract_address:
+                ct = frame.chain_manager.contracts.get(frame.contract_address)
+                if not ct:
+                    raise ValueError(msg.format(address=frame.contract_address))
+
+                return ct
+
+            idx -= 1
+
+        raise ValueError(msg.format(address=frame.contract_address))
+
     @classmethod
     def from_error(cls, err: Exception):
         """
         Creates this class from the error message of the given
         error.
 
         This should be overridden whenever possible to handle
@@ -262,15 +300,15 @@
 
 class OutOfGasError(VirtualMachineError):
     """
     Raised when detecting a transaction failed because it ran
     out of gas.
     """
 
-    def __init__(self, code: Optional[int] = None, txn: Optional["TransactionAPI"] = None):
+    def __init__(self, code: Optional[int] = None, txn: Optional[FailedTxn] = None):
         super().__init__("The transaction ran out of gas.", code=code, txn=txn)
 
 
 class NetworkError(ApeException):
     """
     Raised when a problem occurs when using blockchain networks.
     """
@@ -510,17 +548,18 @@
     """
     Handle a transaction error by showing relevant stack frames,
     including custom contract frames added to the exception.
     This method must be called within an ``except`` block or with
     an exception on the exc-stack.
 
     Args:
-        err (:class:`~ape.exceptions.ApeException`): The transaction error
+        err (:class:`~ape.exceptions.TransactionError`): The transaction error
           being handled.
-        base_paths (List[Path]): Source base paths for allowed frames.
+        base_paths (Optional[List[Path]]): Optionally include additional
+          source-path prefixes to use when finding relevant frames.
 
     Returns:
         bool: ``True`` if outputted something.
     """
 
     tb = traceback.extract_tb(sys.exc_info()[2])
     relevant_tb = [f for f in tb if any(str(p) in f.filename for p in base_paths)]
@@ -578,15 +617,15 @@
     An error defined in a smart contract.
     """
 
     def __init__(
         self,
         abi: ErrorABI,
         inputs: Dict[str, Any],
-        txn: Optional["TransactionAPI"] = None,
+        txn: Optional[FailedTxn] = None,
         trace: Optional[Iterator["TraceFrame"]] = None,
         contract_address: Optional["AddressType"] = None,
     ):
         self.abi = abi
         self.inputs = inputs
 
         if inputs:
@@ -599,7 +638,92 @@
 
     @property
     def name(self) -> str:
         """
         The name of the error.
         """
         return self.abi.name
+
+
+def _get_ape_traceback(txn: FailedTxn) -> Optional["SourceTraceback"]:
+    is_receipt = "ReceiptAPI" in [t.__name__ for t in txn.__class__.__bases__]
+    receipt: "ReceiptAPI" = txn if is_receipt else txn.receipt  # type: ignore
+    if not receipt:
+        return None
+
+    try:
+        ape_traceback = receipt.source_traceback
+    except (ApeException, NotImplementedError):
+        return None
+
+    if ape_traceback is None or not len(ape_traceback):
+        return None
+
+    return ape_traceback
+
+
+def _get_custom_python_traceback(
+    err: TransactionError, txn: FailedTxn, ape_traceback: "SourceTraceback"
+) -> Optional[TracebackType]:
+    # Manipulate python traceback to show lines from contract.
+    # Help received from Jinja lib:
+    #  https://github.com/pallets/jinja/blob/main/src/jinja2/debug.py#L142
+
+    _, exc_value, tb = sys.exc_info()
+    depth = None
+    idx = len(ape_traceback) - 1
+    frames = []
+    project_path = txn.project_manager.path.as_posix()
+    while tb is not None:
+        if not tb.tb_frame.f_code.co_filename.startswith(project_path):
+            # Ignore frames outside the project.
+            # This allows both contract code an scripts to appear.
+            tb = tb.tb_next
+            continue
+
+        frames.append(tb)
+        tb = tb.tb_next
+
+    while (depth is None or depth > 1) and idx >= 0:
+        exec_item = ape_traceback[idx]
+        if depth is not None and exec_item.depth >= depth:
+            # Wait for decreasing depth.
+            continue
+
+        depth = exec_item.depth
+        lineno = exec_item.begin_lineno
+        if lineno is None:
+            continue
+
+        if exec_item.source_path is None:
+            # File is not local. Create a temporary file in its place.
+            # This is necessary for tracebacks to work in Python.
+            temp_file = tempfile.NamedTemporaryFile(prefix="unknown_contract_")
+            filename = temp_file.name
+        else:
+            filename = exec_item.source_path.as_posix()
+
+        # Raise an exception at the correct line number.
+        py_code: CodeType = compile(
+            "\n" * (lineno - 1) + "raise __ape_exception__", filename, "exec"
+        )
+        py_code = py_code.replace(co_name=exec_item.closure.name)
+
+        # Execute the new code to get a new (fake) tb with contract source info.
+        try:
+            exec(py_code, {"__ape_exception__": err}, {})
+        except BaseException:
+            fake_tb = sys.exc_info()[2].tb_next  # type: ignore
+            if isinstance(fake_tb, TracebackType):
+                frames.append(fake_tb)
+
+        idx -= 1
+
+    if not frames:
+        return None
+
+    tb_next = None
+    for tb in frames:
+        tb.tb_next = tb_next
+        tb_next = tb
+
+    return frames[-1]
```

### Comparing `eth-ape-0.6.8/src/ape/logging.py` & `eth-ape-0.6.9/src/ape/logging.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/managers/__init__.py` & `eth-ape-0.6.9/src/ape/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/managers/accounts.py` & `eth-ape-0.6.9/src/ape/managers/accounts.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     finally:
         _DEFAULT_SENDERS.pop()
 
 
 class TestAccountManager(list, ManagerAccessMixin):
     __test__ = False
 
+    _impersonated_accounts: Dict[AddressType, ImpersonatedAccount] = {}
+
     def __repr__(self) -> str:
         accounts_str = ", ".join([a.address for a in self.accounts])
         return f"[{accounts_str}]"
 
     @cached_property
     def containers(self) -> Dict[str, TestAccountContainerAPI]:
         containers = {}
@@ -104,15 +106,19 @@
             raise IndexError(
                 f"Your provider does not support impersonating accounts:\n{err_message}"
             ) from err
 
         if not can_impersonate:
             raise IndexError(err_message)
 
-        return ImpersonatedAccount(raw_address=account_id)
+        if account_id not in self._impersonated_accounts:
+            acct = ImpersonatedAccount(raw_address=account_id)
+            self._impersonated_accounts[account_id] = acct
+
+        return self._impersonated_accounts[account_id]
 
     def __contains__(self, address: AddressType) -> bool:  # type: ignore
         return any(address in container for container in self.containers.values())
 
     def generate_test_account(self, container_name: str = "test") -> TestAccountAPI:
         return self.containers[container_name].generate_account()
```

### Comparing `eth-ape-0.6.8/src/ape/managers/chain.py` & `eth-ape-0.6.9/src/ape/managers/chain.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import time
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import contextmanager
 from functools import partial
 from pathlib import Path
 from typing import IO, Collection, Dict, Iterator, List, Optional, Set, Type, Union, cast
 
+import click
 import pandas as pd
 from ethpm_types import ContractType
-from evm_trace.gas import merge_reports
 from rich import get_console
 from rich.console import Console as RichConsole
 
 from ape.api import BlockAPI, ReceiptAPI
 from ape.api.address import BaseAddress
 from ape.api.networks import LOCAL_NETWORK_NAME, NetworkAPI, ProxyInfoAPI
 from ape.api.query import (
@@ -24,28 +24,22 @@
 from ape.contracts import ContractContainer, ContractInstance
 from ape.exceptions import (
     APINotImplementedError,
     BlockNotFoundError,
     ChainError,
     ConversionError,
     CustomError,
+    ProviderNotConnectedError,
     QueryEngineError,
     UnknownSnapshotError,
 )
 from ape.logging import logger
 from ape.managers.base import BaseManager
-from ape.types import (
-    AddressType,
-    BlockID,
-    CallTreeNode,
-    ContractFunctionPath,
-    GasReport,
-    SnapshotID,
-)
-from ape.utils import BaseInterfaceModel, TraceStyles, parse_gas_table, singledispatchmethod
+from ape.types import AddressType, BlockID, CallTreeNode, SnapshotID, SourceTraceback
+from ape.utils import BaseInterfaceModel, TraceStyles, singledispatchmethod
 
 
 class BlockContainer(BaseManager):
     """
     A list of blocks on the chain.
 
     Usages example::
@@ -607,34 +601,41 @@
     def __getitem_str(self, account_or_hash: str) -> Union[AccountHistory, ReceiptAPI]:
         """
         Get a receipt from the history by its transaction hash.
         If the receipt is not currently cached, will use the provider
         to retrieve it.
 
         Args:
-            transaction_hash (str): The hash of the transaction.
+            account_or_hash (str): The hash of the transaction.
 
         Returns:
             :class:`~ape.api.transactions.ReceiptAPI`: The receipt.
         """
 
         try:
             address = self.provider.network.ecosystem.decode_address(account_or_hash)
             return self._get_account_history(address)
         except Exception:
             # Use Transaction hash
-            receipt = self._hash_to_receipt_map.get(account_or_hash)
-            if not receipt:
-                # TODO: Replace with query manager once supports receipts
-                #  instead of transactions.
-                # TODO: Add timeout = 0 once in API method to not wait for txns
-                receipt = self.provider.get_receipt(account_or_hash)
-                self.append(receipt)
+            try:
+                return self._get_receipt(account_or_hash)
+            except Exception:
+                pass
+
+            # If we get here, we failed to get an account or receipt.
+            # Raise top-level exception.
+            raise
+
+    def _get_receipt(self, txn_hash: str) -> ReceiptAPI:
+        receipt = self._hash_to_receipt_map.get(txn_hash)
+        if not receipt:
+            receipt = self.provider.get_receipt(txn_hash, timeout=0)
+            self.append(receipt)
 
-            return receipt
+        return receipt
 
     def append(self, txn_receipt: ReceiptAPI):
         """
         Add a transaction to the cache This is useful for sessional-transactions.
 
         Raises:
             :class:`~ape.exceptions.ChainError`: When trying to append a transaction
@@ -1107,15 +1108,25 @@
             if contract_type:
                 # If a default contract type was provided, don't error and use it.
                 logger.error(str(err))
             else:
                 raise  # Current exception
 
         if not contract_type:
-            raise ChainError(f"Failed to get contract type for address '{contract_address}'.")
+            msg = f"Failed to get contract type for address '{contract_address}'."
+            if self.provider.network.explorer is None:
+                msg += (
+                    f" Current provider '{self.provider.name}' has no associated "
+                    "explorer plugin. Try installing an explorer plugin using "
+                    f"{click.style(text='ape plugins install etherscan', fg='green')}, "
+                    "or using a network with explorer support."
+                )
+            else:
+                msg += " Contract may need verification."
+            raise ChainError(msg)
         elif not isinstance(contract_type, ContractType):
             raise TypeError(
                 f"Expected type '{ContractType.__name__}' for argument 'contract_type'."
             )
 
         if not txn_hash:
             # Check for txn_hash in deployments.
@@ -1235,17 +1246,14 @@
     """
     A class representing the active Ape session. Useful for tracking data and
     building reports.
 
     **NOTE**: This class is not part of the public API.
     """
 
-    track_gas: bool = False
-    gas_exclusions: List[ContractFunctionPath] = []
-    session_gas_report: Optional[GasReport] = None
     rich_console_map: Dict[str, RichConsole] = {}
 
     def show_trace(
         self,
         call_tree: CallTreeNode,
         sender: Optional[AddressType] = None,
         transaction_hash: Optional[str] = None,
@@ -1262,43 +1270,37 @@
             console.print(f"[bold red]{revert_message}[/]")
         if sender:
             console.print(f"tx.origin=[{TraceStyles.CONTRACTS}]{sender}[/]")
 
         console.print(root)
 
     def show_gas(self, call_tree: CallTreeNode, file: Optional[IO[str]] = None):
-        console = self._get_console(file)
         tables = call_tree.as_gas_tables()
-        console.print(*tables)
+        self.echo(*tables, file=file)
 
-    def show_session_gas(
-        self,
-        file: Optional[IO[str]] = None,
-    ) -> bool:
-        if not self.session_gas_report:
-            return False
+    def echo(self, *rich_items, file: Optional[IO[str]] = None):
+        console = self._get_console(file=file)
+        console.print(*rich_items)
 
-        tables = parse_gas_table(self.session_gas_report)
-        console = self._get_console(file)
-        console.print(*tables)
-        return True
+    @property
+    def track_gas(self) -> bool:
+        # TODO: Delete in 0.7; call _test_runner directly if needed.
+        return self._test_runner is not None and self._test_runner.gas_tracker.enabled
+
+    def append_gas(self, *args, **kwargs):
+        # TODO: Delete in 0.7 and have all plugins call `_test_runner.gas_tracker.append_gas()`.
+        if self._test_runner:
+            self._test_runner.gas_tracker.append_gas(*args, **kwargs)
 
-    def append_gas(
-        self,
-        call_tree: CallTreeNode,
-        contract_address: AddressType,
+    def show_source_traceback(
+        self, traceback: SourceTraceback, file: Optional[IO[str]] = None, failing: bool = True
     ):
-        contract_type = self.chain_manager.contracts.get(contract_address)
-        if not contract_type:
-            # Skip unknown contracts.
-            return
-
-        gas_report = call_tree.get_gas_report(exclude=self.gas_exclusions)
-        session_report = self.session_gas_report or {}
-        self.session_gas_report = merge_reports(session_report, gas_report)
+        console = self._get_console(file)
+        style = "red" if failing else None
+        console.print(str(traceback), style=style)
 
     def _get_console(self, file: Optional[IO[str]] = None) -> RichConsole:
         if not file:
             return get_console()
 
         # Configure custom file console
         file_id = str(file)
@@ -1338,19 +1340,24 @@
         return self._block_container_map[self.chain_id]
 
     @property
     def history(self) -> TransactionHistory:
         """
         A mapping of transactions from the active session to the account responsible.
         """
-        if self.chain_id not in self._transaction_history_map:
+        try:
+            chain_id = self.chain_id
+        except ProviderNotConnectedError:
+            return TransactionHistory()  # Empty list.
+
+        if chain_id not in self._transaction_history_map:
             history = TransactionHistory()
-            self._transaction_history_map[self.chain_id] = history
+            self._transaction_history_map[chain_id] = history
 
-        return self._transaction_history_map[self.chain_id]
+        return self._transaction_history_map[chain_id]
 
     @property
     def chain_id(self) -> int:
         """
         The blockchain ID.
         See `ChainList <https://chainlist.org/>`__ for a comprehensive list of IDs.
         """
@@ -1467,14 +1474,15 @@
         """
 
         snapshot = None
         try:
             snapshot = self.snapshot()
         except APINotImplementedError:
             logger.warning("Provider does not support snapshotting.")
+        pending = self.pending_timestamp
 
         start_ecosystem_name = self.provider.network.ecosystem.name
         start_network_name = self.provider.network.name
         start_provider_name = self.provider.name
 
         try:
             yield
@@ -1493,14 +1501,20 @@
                 or start_provider_name != end_provider_name
             ):
                 logger.warning("Provider changed before isolation completed.")
                 return
 
             self.chain_manager.restore(snapshot)
 
+            try:
+                self.pending_timestamp = pending
+            except APINotImplementedError:
+                # Provider does not support time travel.
+                pass
+
     def mine(
         self,
         num_blocks: int = 1,
         timestamp: Optional[int] = None,
         deltatime: Optional[int] = None,
     ) -> None:
         """
```

### Comparing `eth-ape-0.6.8/src/ape/managers/compilers.py` & `eth-ape-0.6.9/src/ape/managers/compilers.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/managers/config.py` & `eth-ape-0.6.9/src/ape/managers/config.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/managers/converters.py` & `eth-ape-0.6.9/src/ape/managers/converters.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/managers/networks.py` & `eth-ape-0.6.9/src/ape/managers/networks.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/managers/project/dependency.py` & `eth-ape-0.6.9/src/ape/managers/project/dependency.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,18 +96,19 @@
 
         latest_release = github_client.get_release(self.github, "latest")
         return latest_release.tag_name
 
     @property
     def uri(self) -> AnyUrl:
         _uri = f"https://github.com/{self.github.strip('/')}"
-        if self.version and not self.version.startswith("v"):
-            _uri = f"{_uri}/releases/tag/v{self.version}"
-        elif self.version:
-            _uri = f"{_uri}/releases/tag/{self.version}"
+        if self.version:
+            version = f"v{self.version}" if not self.version.startswith("v") else self.version
+            _uri = f"{_uri}/releases/tag/{version}"
+        elif self._reference:
+            _uri = f"{_uri}/tree/{self._reference}"
 
         return HttpUrl(_uri, scheme="https")
 
     def __repr__(self):
         return f"<{self.__class__.__name__} github={self.github}>"
 
     def extract_manifest(self) -> PackageManifest:
```

### Comparing `eth-ape-0.6.8/src/ape/managers/project/manager.py` & `eth-ape-0.6.9/src/ape/managers/project/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import shutil
 from pathlib import Path
 from typing import Dict, Iterable, List, Optional, Type, Union
 
-from ethpm_types import Compiler
 from ethpm_types import ContractInstance as EthPMContractInstance
 from ethpm_types import ContractType, PackageManifest, PackageMeta, Source
 from ethpm_types.contract_type import BIP122_URI
 from ethpm_types.manifest import PackageName
+from ethpm_types.source import Compiler, ContractSource
 from ethpm_types.utils import AnyUrl
 
 from ape.api import DependencyAPI, ProjectAPI
 from ape.api.networks import LOCAL_NETWORK_NAME
 from ape.contracts import ContractContainer, ContractInstance, ContractNamespace
 from ape.exceptions import APINotImplementedError, ProjectError
 from ape.logging import logger
@@ -576,14 +576,17 @@
             pathlib.Path: The path if it exists, else ``None``.
         """
 
         path = Path(key_contract_path)
         ext = path.suffix or None
 
         def find_in_dir(dir_path: Path) -> Optional[Path]:
+            if not dir_path.is_dir():
+                return None
+
             for file_path in dir_path.iterdir():
                 if file_path.is_dir():
                     result = find_in_dir(file_path)
                     if result:
                         return result
 
                 # If the user provided an extension, it has to match.
@@ -722,14 +725,35 @@
 
         if destination.is_file():
             logger.debug("Deployment already tracked. Re-tracking.")
             destination.unlink()
 
         destination.write_text(artifact.json())
 
+    def _create_contract_source(self, contract_type: ContractType) -> Optional[ContractSource]:
+        if not contract_type.source_id:
+            return None
+
+        src = self._lookup_source(contract_type.source_id)
+        if not src:
+            return None
+
+        try:
+            return ContractSource.create(contract_type, src, self.contracts_folder)
+        except (ValueError, FileNotFoundError):
+            return None
+
+    def _lookup_source(self, source_id: str) -> Optional[Source]:
+        source_path = self.lookup_path(source_id)
+        if source_path and source_path.is_file():
+            result = self.local_project._create_source_dict(source_path, self.contracts_folder)
+            return next(iter(result.values())) if result else None
+
+        return None
+
     def _get_contract(self, name: str) -> Optional[ContractContainer]:
         if name in self.contracts:
             return self.chain_manager.contracts.get_container(self.contracts[name])
 
         return None
 
     # def publish_manifest(self):
```

### Comparing `eth-ape-0.6.8/src/ape/managers/project/types.py` & `eth-ape-0.6.9/src/ape/managers/project/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 import yaml
 from ethpm_types import ContractType, PackageManifest, Source
 from ethpm_types.utils import compute_checksum
@@ -72,20 +73,21 @@
         source_id = str(get_relative_path(source_path, self.contracts_folder))
 
         if source_id not in self.cached_sources:
             return True  # New file added
 
         cached_source = self.cached_sources[source_id]
         cached_checksum = cached_source.calculate_checksum()
-
         source_file = self.contracts_folder / source_path
-        checksum = compute_checksum(
-            source_file.read_text("utf8").encode("utf8"),
-            algorithm=cached_checksum.algorithm,
-        )
+
+        # ethpm_types strips trailing white space and ensures
+        # a newline at the end so content so `splitlines()` works.
+        # We need to do the same here for to prevent the endless recompiling bug.
+        content = f"{source_file.read_text('utf8').rstrip()}\n"
+        checksum = compute_checksum(content.encode("utf8"), algorithm=cached_checksum.algorithm)
 
         # NOTE: Filter by checksum to only update what's needed
         return checksum != cached_checksum.hash  # Contents changed
 
     def get_source_reference_paths(self, source_id: str) -> List[Path]:
         return [s for s in self._source_reference_paths.get(source_id, []) if s.is_file()]
 
@@ -109,14 +111,15 @@
         return True
 
     @property
     def source_paths(self) -> List[Path]:
         """
         All the source files in the project.
         Excludes files with extensions that don't have a registered compiler.
+
         Returns:
             List[pathlib.Path]: A list of a source file paths in the project.
         """
         files: List[Path] = []
 
         if not self.contracts_folder.is_dir():
             return files
@@ -139,15 +142,17 @@
         config_data = {**kwargs}
         if self.name:
             config_data["name"] = self.name
         if self.version:
             config_data["version"] = self.version
 
         contracts_folder = kwargs.get("contracts_folder") or self.contracts_folder
-        contracts_folder_config_item = str(contracts_folder).replace(str(self.path), "").strip("/")
+        contracts_folder_config_item = (
+            str(contracts_folder).replace(str(self.path), "").strip(os.path.sep)
+        )
         config_data["contracts_folder"] = contracts_folder_config_item
         self.config_file.parent.mkdir(parents=True, exist_ok=True)
         self.config_file.touch()
         with open(self.config_file, "w") as f:
             yaml.safe_dump(config_data, f)
 
         return True
```

### Comparing `eth-ape-0.6.8/src/ape/managers/query.py` & `eth-ape-0.6.9/src/ape/managers/query.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/plugins/__init__.py` & `eth-ape-0.6.9/src/ape/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/plugins/account.py` & `eth-ape-0.6.9/src/ape/plugins/account.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/plugins/compiler.py` & `eth-ape-0.6.9/src/ape/plugins/compiler.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/plugins/config.py` & `eth-ape-0.6.9/src/ape/plugins/config.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/plugins/converter.py` & `eth-ape-0.6.9/src/ape/plugins/converter.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/plugins/network.py` & `eth-ape-0.6.9/src/ape/plugins/network.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/plugins/pluggy_patch.py` & `eth-ape-0.6.9/src/ape/plugins/pluggy_patch.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/plugins/project.py` & `eth-ape-0.6.9/src/ape/plugins/project.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/plugins/query.py` & `eth-ape-0.6.9/src/ape/plugins/query.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/pytest/README.md` & `eth-ape-0.6.9/src/ape/pytest/README.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/pytest/config.py` & `eth-ape-0.6.9/src/ape/pytest/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,18 @@
         return self.config_manager.get_config("test")
 
     @cached_property
     def track_gas(self) -> bool:
         return self.pytest_config.getoption("--gas") or self.ape_test_config.gas.show
 
     @cached_property
+    def show_internal(self) -> bool:
+        return self.pytest_config.getoption("showinternal")
+
+    @cached_property
     def gas_exclusions(self) -> List[ContractFunctionPath]:
         """
         The combination of both CLI values and config values.
         """
 
         cli_value = self.pytest_config.getoption("--gas-exclude")
         exclusions: List[ContractFunctionPath] = []
```

### Comparing `eth-ape-0.6.8/src/ape/pytest/contextmanagers.py` & `eth-ape-0.6.9/src/ape/pytest/contextmanagers.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/pytest/fixtures.py` & `eth-ape-0.6.9/src/ape/pytest/fixtures.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,14 +72,22 @@
     def project(self) -> ProjectManager:
         """
         Access contract types and dependencies.
         """
 
         return self.project_manager
 
+    @pytest.fixture(scope="session")
+    def Contract(self):
+        """
+        Instantiate a reference to an on-chain contract
+        using its address (same as ``ape.Contract``).
+        """
+        return self.chain_manager.contracts.instance_at
+
     def _isolation(self) -> Iterator[None]:
         """
         Isolation logic used to implement isolation fixtures for each pytest scope.
         When tracing support is available, will also assist in capturing receipts.
         """
 
         snapshot_id = self._snapshot()
@@ -125,16 +133,14 @@
 class ReceiptCapture(ManagerAccessMixin):
     config_wrapper: ConfigWrapper
     receipt_map: Dict[str, Dict[str, ReceiptAPI]] = {}
     enter_blocks: List[int] = []
 
     def __init__(self, config_wrapper: ConfigWrapper):
         self.config_wrapper = config_wrapper
-        self.chain_manager._reports.track_gas = self.config_wrapper.track_gas
-        self.chain_manager._reports.gas_exclusions = self.config_wrapper.gas_exclusions
 
     def __enter__(self):
         block_number = self._get_block_number()
         if block_number is not None:
             self.enter_blocks.append(block_number)
 
     def __exit__(self, exc_type, exc_val, exc_tb):
```

### Comparing `eth-ape-0.6.8/src/ape/pytest/plugin.py` & `eth-ape-0.6.9/src/ape/pytest/plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 
 import pytest
 
 from ape import networks, project
 from ape.logging import LogLevel, logger
 from ape.pytest.config import ConfigWrapper
 from ape.pytest.fixtures import PytestApeFixtures, ReceiptCapture
+from ape.pytest.gas import GasTracker
 from ape.pytest.runners import PytestApeRunner
+from ape.utils import ManagerAccessMixin
 
 
 def pytest_addoption(parser):
     parser.addoption(
         "--showinternal",
         action="store_true",
     )
@@ -59,26 +61,35 @@
             modules = [v for v in sys.modules.values() if is_module(v)]
             for module in modules:
                 if hasattr(module, "__tracebackhide__"):
                     setattr(module, "__tracebackhide__", True)
 
     config_wrapper = ConfigWrapper(config)
     receipt_capture = ReceiptCapture(config_wrapper)
+    gas_tracker = GasTracker(config_wrapper=config_wrapper)
 
     # Enable verbose output if stdout capture is disabled
     config.option.verbose = config.getoption("capture") == "no"
 
     # Register the custom Ape test runner
-    session = PytestApeRunner(config_wrapper, receipt_capture)
-    config.pluginmanager.register(session, "ape-test")
+    runner = PytestApeRunner(config_wrapper, receipt_capture, gas_tracker)
+    config.pluginmanager.register(runner, "ape-test")
+
+    # Inject runner for access to gas and coverage trackers.
+    ManagerAccessMixin._test_runner = runner
 
     # Include custom fixtures for project, accounts etc.
     fixtures = PytestApeFixtures(config_wrapper, receipt_capture)
     config.pluginmanager.register(fixtures, "ape-fixtures")
 
+    # Add custom markers
+    config.addinivalue_line(
+        "markers", "use_network(choice): Run this test using the given network choice."
+    )
+
 
 def pytest_load_initial_conftests(early_config):
     """
     Compile contracts before loading ``conftest.py``s.
     """
     capture_manager = early_config.pluginmanager.get_plugin("capturemanager")
```

### Comparing `eth-ape-0.6.8/src/ape/pytest/runners.py` & `eth-ape-0.6.9/src/ape/pytest/runners.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,31 +7,35 @@
 
 import ape
 from ape.api import ProviderContextManager
 from ape.logging import LogLevel
 from ape.pytest.config import ConfigWrapper
 from ape.pytest.contextmanagers import RevertsContextManager
 from ape.pytest.fixtures import ReceiptCapture
+from ape.pytest.gas import GasTracker
 from ape.utils import ManagerAccessMixin
 from ape_console._cli import console
 
 
 class PytestApeRunner(ManagerAccessMixin):
     def __init__(
         self,
         config_wrapper: ConfigWrapper,
         receipt_capture: ReceiptCapture,
+        gas_tracker: GasTracker,
     ):
         self.config_wrapper = config_wrapper
         self.receipt_capture = receipt_capture
         self._provider_is_connected = False
-        ape.reverts = RevertsContextManager  # type: ignore
 
         # Ensure the gas report starts off None for this runner.
-        self.chain_manager._reports.session_gas_report = None
+        gas_tracker.session_gas_report = None
+        self.gas_tracker = gas_tracker
+
+        ape.reverts = RevertsContextManager  # type: ignore
 
     @property
     def _provider_context(self) -> ProviderContextManager:
         return self.network_manager.parse_network_choice(self.config_wrapper.network)
 
     def pytest_exception_interact(self, report, call):
         """
@@ -40,32 +44,37 @@
         same console as the ``ape console`` command.
         """
 
         # Find the last traceback frame within the active project
         tb_frames: PytestTraceback = call.excinfo.traceback
         base = self.project_manager.path.as_posix()
 
-        if self.config_wrapper.pytest_config.getoption("showinternal"):
+        if self.config_wrapper.show_internal:
             relevant_tb = list(tb_frames)
         else:
             relevant_tb = [
                 f
                 for f in tb_frames
                 if Path(f.path).as_posix().startswith(base) or Path(f.path).name.startswith("test_")
             ]
 
         if relevant_tb:
             call.excinfo.traceback = PytestTraceback(relevant_tb)
+
+            # Only show locals if not digging into the framework's traceback.
+            # Else, it gets way too noisy.
+            show_locals = not self.config_wrapper.show_internal
+
             report.longrepr = call.excinfo.getrepr(
                 funcargs=True,
                 abspath=Path.cwd(),
-                showlocals=True,
+                showlocals=show_locals,
                 style="short",
                 tbfilter=False,
-                truncate_locals=False,
+                truncate_locals=True,
                 chain=False,
             )
 
         if self.config_wrapper.interactive and report.failed:
             traceback = call.excinfo.traceback[0]
 
             # Suspend capsys to ignore our own output.
@@ -157,14 +166,26 @@
         """
         reporter = self.config_wrapper.get_pytest_plugin("terminalreporter")
         warnings = reporter.stats.pop("warnings", [])
         warnings = [i for i in warnings if "PytestAssertRewriteWarning" not in i.message]
         if warnings and not self.config_wrapper.disable_warnings:
             reporter.stats["warnings"] = warnings
 
+    @pytest.hookimpl(tryfirst=True, hookwrapper=True)
+    def pytest_runtest_call(self, item):
+        if network_marker := item.get_closest_marker("use_network"):
+            if len(getattr(network_marker, "args", []) or []) != 1:
+                raise ValueError("`use_network` marker requires single network choice argument.")
+
+            with self.network_manager.parse_network_choice(network_marker.args[0]):
+                yield
+
+        else:
+            yield
+
     @pytest.hookimpl(trylast=True, hookwrapper=True)
     def pytest_collection_finish(self, session):
         """
         Called after collection has been performed and modified.
         """
         outcome = yield
 
@@ -187,22 +208,22 @@
             terminalreporter.write_line(
                 f"{LogLevel.ERROR.name}: Provider '{self.provider.name}' does not support "
                 f"transaction tracing and is unable to display a gas profile.",
                 red=True,
             )
             return
 
-        if not self.chain_manager._reports.show_session_gas():
+        if not self.gas_tracker.show_session_gas():
             terminalreporter.write_line(
                 f"{LogLevel.WARNING.name}: No gas usage data found.", yellow=True
             )
 
     def pytest_unconfigure(self):
         if self._provider_is_connected and self.config_wrapper.disconnect_providers_after:
             self._provider_context.disconnect_all()
             self._provider_is_connected = False
 
         # NOTE: Clearing the state is helpful for pytester-based tests,
         #  which may run pytest many times in-process.
         self.receipt_capture.clear()
         self.chain_manager.contracts.clear_local_caches()
-        self.chain_manager._reports.session_gas_report = None
+        self.gas_tracker.session_gas_report = None
```

### Comparing `eth-ape-0.6.8/src/ape/types/__init__.py` & `eth-ape-0.6.9/src/ape/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, Dict, List, Literal, Optional, Union
 
 from eth_abi.abi import encode
 from eth_abi.packed import encode_packed
-from eth_typing import ChecksumAddress as AddressType
 from eth_typing import HexStr
 from eth_utils import encode_hex, keccak
 from ethpm_types import (
     ABI,
     Bytecode,
     Checksum,
     Compiler,
     ContractType,
     PackageManifest,
     PackageMeta,
     Source,
 )
 from ethpm_types.abi import EventABI
+from ethpm_types.source import Closure
 from hexbytes import HexBytes
 from pydantic import BaseModel, root_validator, validator
 from web3.types import FilterParams
 
+from ape.types.address import AddressType, RawAddress
 from ape.types.signatures import MessageSignature, SignableMessage, TransactionSignature
-from ape.types.trace import CallTreeNode, GasReport, TraceFrame
+from ape.types.trace import CallTreeNode, ControlFlow, GasReport, SourceTraceback, TraceFrame
 from ape.utils import BaseInterfaceModel, cached_property
 from ape.utils.misc import to_int
 
 if TYPE_CHECKING:
     from ape.api.providers import BlockAPI
     from ape.contracts import ContractEvent
 
@@ -47,19 +48,14 @@
 :meth:`~ape.managers.chain.ChainManager.snapshot` and
 :meth:`~ape.managers.chain.ChainManager.snapshot` methods. Can be a ``str``, ``int``, or ``bytes``.
 Providers will expect and handle snapshot IDs differently. There shouldn't be a need to change
 providers when using this feature, so there should not be confusion over this type in practical use
 cases.
 """
 
-RawAddress = Union[str, int, HexBytes]
-"""
-A raw data-type representation of an address.
-"""
-
 
 GasLimit = Union[Literal["auto", "max"], int, str]
 """
 A value you can give to Ape for handling gas-limit calculations.
 ``"auto"`` refers to automatically figuring out the gas,
 ``"max"`` refers to using the maximum block gas limit,
 and otherwise you can provide a numeric value.
@@ -296,21 +292,25 @@
 __all__ = [
     "ABI",
     "AddressType",
     "BlockID",
     "Bytecode",
     "CallTreeNode",
     "Checksum",
+    "Closure",
     "Compiler",
     "ContractLog",
     "ContractLogContainer",
     "ContractType",
     "GasReport",
     "MessageSignature",
     "PackageManifest",
     "PackageMeta",
+    "RawAddress",
     "SignableMessage",
     "SnapshotID",
     "Source",
+    "SourceTraceback",
+    "ControlFlow",
     "TraceFrame",
     "TransactionSignature",
 ]
```

### Comparing `eth-ape-0.6.8/src/ape/types/signatures.py` & `eth-ape-0.6.9/src/ape/types/signatures.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/utils/__init__.py` & `eth-ape-0.6.9/src/ape/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/utils/abi.py` & `eth-ape-0.6.9/src/ape/utils/abi.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/utils/basemodel.py` & `eth-ape-0.6.9/src/ape/utils/basemodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC
-from typing import TYPE_CHECKING, ClassVar, Dict, List, cast
+from typing import TYPE_CHECKING, ClassVar, Dict, List, Optional, cast
 
 from pydantic import BaseModel
 
 from ape.exceptions import ProviderNotConnectedError
 from ape.utils.misc import cached_property, singledispatchmethod
 
 if TYPE_CHECKING:
@@ -13,14 +13,15 @@
     from ape.managers.compilers import CompilerManager
     from ape.managers.config import ConfigManager
     from ape.managers.converters import ConversionManager
     from ape.managers.networks import NetworkManager
     from ape.managers.project import DependencyManager, ProjectManager
     from ape.managers.query import QueryManager
     from ape.plugins import PluginManager
+    from ape.pytest.runners import PytestApeRunner
 
 
 class injected_before_use(property):
     """
     Injected properties are injected class variables that must be set before use.
 
     **NOTE**: do not appear in a Pydantic model's set of properties.
@@ -52,14 +53,16 @@
 
     plugin_manager: ClassVar["PluginManager"] = cast("PluginManager", injected_before_use())
 
     project_manager: ClassVar["ProjectManager"] = cast("ProjectManager", injected_before_use())
 
     query_manager: ClassVar["QueryManager"] = cast("QueryManager", injected_before_use())
 
+    _test_runner: ClassVar[Optional["PytestApeRunner"]] = None
+
     @property
     def provider(self) -> "ProviderAPI":
         """
         The current active provider if connected to one.
 
         Raises:
             :class:`~ape.exceptions.ProviderNotConnectedError`: When there is
```

### Comparing `eth-ape-0.6.8/src/ape/utils/github.py` & `eth-ape-0.6.9/src/ape/utils/github.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/utils/misc.py` & `eth-ape-0.6.9/src/ape/utils/misc.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/utils/os.py` & `eth-ape-0.6.9/src/ape/utils/os.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/utils/process.py` & `eth-ape-0.6.9/src/ape/utils/process.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/utils/testing.py` & `eth-ape-0.6.9/src/ape/utils/testing.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape/utils/trace.py` & `eth-ape-0.6.9/src/ape/utils/trace.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_accounts/_cli.py` & `eth-ape-0.6.9/src/ape_accounts/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_accounts/accounts.py` & `eth-ape-0.6.9/src/ape_accounts/accounts.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_cache/_cli.py` & `eth-ape-0.6.9/src/ape_cache/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_cache/models.py` & `eth-ape-0.6.9/src/ape_cache/models.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_cache/query.py` & `eth-ape-0.6.9/src/ape_cache/query.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_compile/_cli.py` & `eth-ape-0.6.9/src/ape_compile/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_console/_cli.py` & `eth-ape-0.6.9/src/ape_console/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_console/plugin.py` & `eth-ape-0.6.9/src/ape_console/plugin.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_ethereum/__init__.py` & `eth-ape-0.6.9/src/ape_ethereum/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_ethereum/_converters.py` & `eth-ape-0.6.9/src/ape_ethereum/_converters.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_ethereum/ecosystem.py` & `eth-ape-0.6.9/src/ape_ethereum/ecosystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,14 +163,18 @@
 
     gas_limit: int = Field(alias="gasLimit")
     gas_used: int = Field(alias="gasUsed")
     base_fee: int = Field(0, alias="baseFeePerGas")
     difficulty: int = 0
     total_difficulty: int = Field(0, alias="totalDifficulty")
 
+    @validator("total_difficulty", pre=True)
+    def validate_total_difficulty(cls, value):
+        return value or 0
+
 
 class Ethereum(EcosystemAPI):
     name: str = "ethereum"
 
     """
     Default transaction type should be overidden id chain doesn't support EIP-1559
     """
@@ -184,18 +188,18 @@
     @property
     def default_transaction_type(self) -> TransactionType:
         network = self.default_network.replace("-", "_")
         return self.config[network].default_transaction_type
 
     @classmethod
     def decode_address(cls, raw_address: RawAddress) -> AddressType:
-        if isinstance(raw_address, int):
-            raw_address = HexBytes(raw_address)
-
-        return to_checksum_address(raw_address)
+        raw: Union[str, HexBytes] = (
+            HexBytes(raw_address) if isinstance(raw_address, int) else raw_address
+        )
+        return to_checksum_address(raw)
 
     @classmethod
     def encode_address(cls, address: AddressType) -> RawAddress:
         return str(address)
 
     def get_proxy_info(self, address: AddressType) -> Optional[ProxyInfo]:
         contract_code = self.provider.get_code(address)
```

### Comparing `eth-ape-0.6.8/src/ape_ethereum/multicall/constants.py` & `eth-ape-0.6.9/src/ape_ethereum/multicall/constants.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_ethereum/multicall/exceptions.py` & `eth-ape-0.6.9/src/ape_ethereum/multicall/exceptions.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_ethereum/multicall/handlers.py` & `eth-ape-0.6.9/src/ape_ethereum/multicall/handlers.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_ethereum/transactions.py` & `eth-ape-0.6.9/src/ape_ethereum/transactions.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from eth_abi import decode
 from eth_account import Account as EthAccount
 from eth_account._utils.legacy_transactions import (
     encode_transaction,
     serializable_unsigned_transaction_from_dict,
 )
 from eth_utils import decode_hex, encode_hex, keccak, to_hex, to_int
-from ethpm_types import HexBytes
+from ethpm_types import ContractType, HexBytes
 from ethpm_types.abi import EventABI, MethodABI
 from pydantic import BaseModel, Field, root_validator, validator
 
 from ape.api import ReceiptAPI, TransactionAPI
 from ape.contracts import ContractEvent
 from ape.exceptions import OutOfGasError, SignatureError, TransactionError
-from ape.types import CallTreeNode, ContractLog, ContractLogContainer
+from ape.types import CallTreeNode, ContractLog, ContractLogContainer, SourceTraceback
 from ape.utils import cached_property
 
 
 class TransactionStatusEnum(IntEnum):
     """
     An ``Enum`` class representing the status of a transaction.
     """
@@ -57,15 +57,20 @@
             raise SignatureError("The transaction is not signed.")
 
         txn_data = self.dict(exclude={"sender"})
         unsigned_txn = serializable_unsigned_transaction_from_dict(txn_data)
         signature = (self.signature.v, to_int(self.signature.r), to_int(self.signature.s))
         signed_txn = encode_transaction(unsigned_txn, signature)
 
-        if self.sender and EthAccount.recover_transaction(signed_txn) != self.sender:
+        # If this is a real sender (not impersonated), verify its signature.
+        if (
+            self.sender
+            and self.sender not in self.account_manager.test_accounts._impersonated_accounts
+            and EthAccount.recover_transaction(signed_txn) != self.sender
+        ):
             raise SignatureError("Recovered signer doesn't match sender!")
 
         return signed_txn
 
     @property
     def txn_hash(self) -> HexBytes:
         txn_bytes = self.serialize_transaction()
@@ -145,39 +150,53 @@
 
     @property
     def failed(self) -> bool:
         return self.status != TransactionStatusEnum.NO_ERROR
 
     @cached_property
     def call_tree(self) -> Optional[CallTreeNode]:
+        if self.receiver:
+            return self.provider.get_call_tree(self.txn_hash)
+
+        # Not an function invoke
+        return None
+
+    @cached_property
+    def contract_type(self) -> Optional[ContractType]:
         if not self.receiver:
-            # Not an function invoke
             return None
 
-        return self.provider.get_call_tree(self.txn_hash)
+        return self.chain_manager.contracts.get(self.receiver)
 
     @cached_property
     def method_called(self) -> Optional[MethodABI]:
-        contract_type = self.chain_manager.contracts.get(self.receiver)
-        if not contract_type:
+        if not self.contract_type:
             return None
 
         method_id = self.data[:4]
-        if method_id not in contract_type.methods:
+        if method_id not in self.contract_type.methods:
             return None
 
-        return contract_type.methods[method_id]
+        return self.contract_type.methods[method_id]
+
+    @property
+    def source_traceback(self) -> SourceTraceback:
+        contract_type = self.contract_type
+        if not contract_type:
+            return SourceTraceback.parse_obj([])
+
+        return SourceTraceback.create(contract_type, self.trace, HexBytes(self.data))
 
     def raise_for_status(self):
         if self.gas_limit is not None and self.ran_out_of_gas:
-            raise OutOfGasError(txn=self.transaction)
+            raise OutOfGasError(txn=self)
 
         elif self.status != TransactionStatusEnum.NO_ERROR:
             txn_hash = HexBytes(self.txn_hash).hex()
-            raise TransactionError(f"Transaction '{txn_hash}' failed.")
+            raise TransactionError(f"Transaction '{txn_hash}' failed.", txn=self)
 
     def show_trace(self, verbose: bool = False, file: IO[str] = sys.stdout):
         call_tree = self.call_tree
         if not call_tree:
             return
 
         call_tree.enrich(use_symbol_for_tokens=True)
@@ -223,14 +242,19 @@
             call_tree.method_id = f"to:{receiver_id}"
 
         elif call_tree.contract_id.startswith("Transferring "):
             call_tree.method_id = f"to:{self.receiver}"
 
         self.chain_manager._reports.show_gas(call_tree, file=file)
 
+    def show_source_traceback(self, file: IO[str] = sys.stdout):
+        self.chain_manager._reports.show_source_traceback(
+            self.source_traceback, file=file, failing=self.failed
+        )
+
     def decode_logs(
         self,
         abi: Optional[
             Union[List[Union[EventABI, "ContractEvent"]], Union[EventABI, "ContractEvent"]]
         ] = None,
     ) -> ContractLogContainer:
         if abi is not None:
```

### Comparing `eth-ape-0.6.8/src/ape_geth/__init__.py` & `eth-ape-0.6.9/src/ape_geth/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_geth/provider.py` & `eth-ape-0.6.9/src/ape_geth/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         if self.is_running:
             logger.info("Stopping 'geth' process.")
             self.stop()
 
         self._clean()
 
     def _clean(self):
-        if self.data_dir.exists():
+        if self.data_dir.is_dir():
             shutil.rmtree(self.data_dir)
 
 
 class GethNetworkConfig(PluginConfig):
     # Make sure you are running the right networks when you try for these
     mainnet: dict = DEFAULT_SETTINGS.copy()
     goerli: dict = DEFAULT_SETTINGS.copy()
@@ -477,15 +477,15 @@
         skip_trace = kwargs.pop("skip_trace", False)
         arguments = self._prepare_call(txn, **kwargs)
         if skip_trace:
             return self._eth_call(arguments)
 
         show_gas = kwargs.pop("show_gas_report", False)
         show_trace = kwargs.pop("show_trace", False)
-        track_gas = self.chain_manager._reports.track_gas
+        track_gas = self._test_runner is not None and self._test_runner.gas_tracker.enabled
         needs_trace = show_gas or show_trace or track_gas
         if not needs_trace:
             return self._eth_call(arguments)
 
         # The user is requesting information related to a call's trace,
         # such as gas usage data.
 
@@ -507,20 +507,20 @@
         call_tree = self._create_call_tree_node(evm_call_tree)
 
         receiver = txn.receiver
         if track_gas and show_gas and not show_trace:
             # Optimization to enrich early and in_place=True.
             call_tree.enrich()
 
-        if track_gas and call_tree and receiver is not None:
+        if track_gas and call_tree and receiver is not None and self._test_runner is not None:
             # Gas report being collected, likely for showing a report
             # at the end of a test run.
             # Use `in_place=False` in case also `show_trace=True`
             enriched_call_tree = call_tree.enrich(in_place=False)
-            self.chain_manager._reports.append_gas(enriched_call_tree, receiver)
+            self._test_runner.gas_tracker.append_gas(enriched_call_tree, receiver)
 
         if show_gas:
             enriched_call_tree = call_tree.enrich(in_place=False)
             self.chain_manager._reports.show_gas(enriched_call_tree)
 
         if show_trace:
             call_tree = call_tree.enrich(use_symbol_for_tokens=True)
```

### Comparing `eth-ape-0.6.8/src/ape_init/_cli.py` & `eth-ape-0.6.9/src/ape_init/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_networks/_cli.py` & `eth-ape-0.6.9/src/ape_networks/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_plugins/_cli.py` & `eth-ape-0.6.9/src/ape_plugins/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_plugins/utils.py` & `eth-ape-0.6.9/src/ape_plugins/utils.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_pm/compiler.py` & `eth-ape-0.6.9/src/ape_pm/compiler.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_run/_cli.py` & `eth-ape-0.6.9/src/ape_run/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_test/__init__.py` & `eth-ape-0.6.9/src/ape_test/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_test/_cli.py` & `eth-ape-0.6.9/src/ape_test/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_test/accounts.py` & `eth-ape-0.6.9/src/ape_test/accounts.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/src/ape_test/provider.py` & `eth-ape-0.6.9/src/ape_test/provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,30 +3,32 @@
 from typing import Optional, cast
 
 from eth.exceptions import HeaderNotFound
 from eth_tester.backends import PyEVMBackend  # type: ignore
 from eth_tester.exceptions import TransactionFailed  # type: ignore
 from eth_utils.exceptions import ValidationError
 from ethpm_types import HexBytes
+from lazyasd import LazyObject  # type: ignore
 from web3 import EthereumTesterProvider, Web3
 from web3.providers.eth_tester.defaults import API_ENDPOINTS
 from web3.types import TxParams
 
 from ape.api import ReceiptAPI, TestProviderAPI, TransactionAPI, Web3Provider
 from ape.exceptions import (
     ContractLogicError,
+    ProviderError,
     ProviderNotConnectedError,
     TransactionError,
     UnknownSnapshotError,
     VirtualMachineError,
 )
 from ape.types import SnapshotID
 from ape.utils import gas_estimation_error_message
 
-CHAIN_ID = API_ENDPOINTS["eth"]["chainId"]()
+CHAIN_ID = LazyObject(lambda: API_ENDPOINTS["eth"]["chainId"](), globals(), "CHAIN_ID")
 
 
 class LocalProvider(TestProviderAPI, Web3Provider):
     _evm_backend: Optional[PyEVMBackend] = None
     _CANNOT_AFFORD_GAS_PATTERN = re.compile(
         r"Sender b'[\\*|\w]*' cannot afford txn gas (\d+) with account balance (\d+)"
     )
@@ -96,15 +98,15 @@
     @property
     def chain_id(self) -> int:
         if self.cached_chain_id is not None:
             return self.cached_chain_id
         elif hasattr(self.web3, "eth"):
             chain_id = self.web3.eth.chain_id
         else:
-            chain_id = CHAIN_ID
+            chain_id = CHAIN_ID  # type: ignore
 
         self.cached_chain_id = chain_id
         return chain_id
 
     @property
     def gas_price(self) -> int:
         return self.base_fee  # no miner tip
@@ -152,15 +154,15 @@
             txn_dict["nonce"] += 1
             txn_params = cast(TxParams, txn_dict)
 
             # Replay txn to get revert reason
             try:
                 self.web3.eth.call(txn_params)
             except (ValidationError, TransactionFailed) as err:
-                vm_err = self.get_virtual_machine_error(err, txn=txn)
+                vm_err = self.get_virtual_machine_error(err, txn=receipt)
                 raise vm_err from err
 
         self.chain_manager.history.append(receipt)
         return receipt
 
     def snapshot(self) -> SnapshotID:
         return self.evm_backend.take_snapshot()
@@ -171,15 +173,34 @@
             if current_hash != snapshot_id:
                 try:
                     return self.evm_backend.revert_to_snapshot(snapshot_id)
                 except HeaderNotFound:
                     raise UnknownSnapshotError(snapshot_id)
 
     def set_timestamp(self, new_timestamp: int):
-        self.evm_backend.time_travel(new_timestamp)
+        current = self.get_block("pending").timestamp
+        if new_timestamp == current:
+            # Is the same, treat as a noop.
+            return
+
+        try:
+            self.evm_backend.time_travel(new_timestamp)
+        except ValidationError as err:
+            pattern = re.compile(
+                r"timestamp must be strictly later than parent, "
+                r"but is 0 seconds before\.\n- child\s{2}: (\d*)\n- parent : (\d*)\.\s*"
+            )
+            if match := re.match(pattern, str(err)):
+                if groups := match.groups():
+                    if groups[0].strip() == groups[1].strip():
+                        # Handle race condition when block headers are the same.
+                        # Treat as noop, same as pre-check.
+                        return
+
+            raise ProviderError(f"Failed to time travel: {err}") from err
 
     def mine(self, num_blocks: int = 1):
         self.evm_backend.mine_blocks(num_blocks)
 
     def get_virtual_machine_error(self, exception: Exception, **kwargs) -> VirtualMachineError:
         txn = kwargs.get("txn")
         trace = kwargs.get("trace")
```

### Comparing `eth-ape-0.6.8/src/eth_ape.egg-info/PKG-INFO` & `eth-ape-0.6.9/src/eth_ape.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,223 +1,224 @@
 Metadata-Version: 2.1
 Name: eth-ape
-Version: 0.6.8
+Version: 0.6.9
 Summary: Ape Ethereum Framework
 Home-page: https://apeworx.io
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Project-URL: Documentation, https://docs.apeworx.io/ape/
 Project-URL: Funding, https://gitcoin.co/grants/5958/ape-maintenance-fund
 Project-URL: Source, https://github.com/ApeWorX/ape
 Project-URL: Tracker, https://github.com/ApeWorX/ape/issues
 Project-URL: Twitter, https://twitter.com/ApeFramework
-Description: # Overview
-        
-        **Ape Framework** is an easy-to-use Web3 development tool.
-        Users can compile, test, and interact with smart contracts all in one command line session.
-        With our **modular plugin system**, Ape supports multiple contract languages and chains.
-        
-        Ape is built by [ApeWorX LTD](https://www.apeworx.io/).
-        
-        Join our [ApeWorX Discord server](https://discord.gg/apeworx) to stay up to date on new releases, plugins and tutorials.
-        
-        If you want to just get started, jump down to the [Playing with Ape](#playing-with-ape)
-        
-        ## Documentation
-        
-        Read our [technical documentation](https://docs.apeworx.io/ape/stable/) to get a deeper understanding of our open source Framework.
-        
-        Read our [academic platform](https://academy.apeworx.io/) will help you master Ape Framework with tutorials and challenges.
-        
-        ## Prerequisite
-        
-        In the latest release, Ape requires:
-        
-        - Linux or macOS
-        - Python 3.8 or later
-        - **Windows**: Install Windows Subsystem Linux [(WSL)](https://docs.microsoft.com/en-us/windows/wsl/install) with Python 3.8 or later
-        
-        Check your python version in a terminal with `python3 --version`
-        
-        ## Installation
-        
-        There are three ways to install ape: `pipx`, `pip`, or `Docker`.
-        
-        ### Considerations for Installing:
-        
-        - We advise installing in a [virtualenv](https://pypi.org/project/virtualenv/) or [venv](https://docs.python.org/3/library/venv.html) to avoid interfering with *OS-level site packages*.
-        
-        - We advise installing **`ape`** with recommended plugins `pip install eth-ape'[recommended-plugins]'`
-        
-        - We advise for **macOS** users to install virtual env via [homebrew](https://formulae.brew.sh/formula/virtualenv)
-        
-        ### via `pipx` or `pip`
-        
-        1. Install `pipx` via their [installation instructions](https://pypa.github.io/pipx/) or `pip` via their [installation instructions](https://pip.pypa.io/en/stable/cli/pip_install/)
-        
-        2. Install **`ape`** via `pipx install eth-ape` or `pip install eth-ape`
-        
-        ### via `docker`
-        
-        Ape can also run in a docker container.
-        
-        Please visit our [Dockerhub](https://hub.docker.com/repository/docker/apeworx/ape) for more details on using Ape with Docker.
-        
-        ```bash
-        docker run \
-        --volume $HOME/.ape:/home/harambe/.ape \
-        --volume $HOME/.vvm:/home/harambe/.vvm \
-        --volume $HOME/.solcx:/home/harambe/.solcx \
-        --volume $PWD:/home/harambe/project \
-        --workdir /home/harambe/project \
-        apeworx/ape compile
-        ```
-        
-        ## Playing with Ape
-        
-        After you installed Ape, you can run `ape --version` to make sure it works and is the latest version.
-        
-        There are two ways to interact with Ape:
-        
-        - [CLI Reference](https://docs.apeworx.io/ape/latest/index.html)
-        
-        - [Python Reference](https://docs.apeworx.io/ape/latest/index.html)
-        
-        Ape is both a CLI tool and a Python SDK.
-        
-        The CLI tool contains all the Ape commands and the Python SDK contains the classes and types needed to compose scripts, console actions, and tests.
-        
-        ## **Ape Modular Plugin System:**
-        
-        Our [list of plugins](https://www.apeworx.io/#plugins) is the best way to have the most interoperable experience with Web3.
-        
-        **NOTE**: If a plugin does not originate from the [ApeWorX GitHub Organization](https://github.com/ApeWorX?q=ape&type=all), you will get a warning about installing 3rd-party plugins.
-        
-        Install 3rd party plugins at your own risk.
-        
-        Additionally, plugins that come bundled with **`ape`** in the core installation cannot be removed and are part of the **`ape`** core software.
-        
-        - Learn more about **installing** plugins from following this [installing user guide](https://docs.apeworx.io/ape/stable/userguides/installing_plugins.html).
-        
-        - Learn more about **developing** your own plugins from this [developing user guide](https://docs.apeworx.io/ape/stable/userguides/developing_plugins.html).
-        
-        ### Accounts
-        
-        In Ape, you will need accounts to make transactions.
-        You can import or generate accounts using the core `accounts` plugin:
-        
-        ```bash
-        ape accounts import acc0   # Will prompt for a private key
-        ape accounts generate acc1
-        ```
-        
-        List all your accounts with the `list` command.
-        
-        ```bash
-        ape accounts list
-        ```
-        
-        Learn more about accounts in Ape by following the [accounts guide](https://docs.apeworx.io/ape/stable/userguides/accounts.html).
-        
-        ### Plugins
-        
-        Add any plugins you may need, such as `vyper`.
-        
-        ```bash
-        ape plugins list -a
-        ape plugins install vyper
-        ape plugins list -a
-        ```
-        
-        ## Projects
-        
-        When using Ape, you generally will work with a project.
-        
-        Learn more about smart-contract **projects** from this [projects guide](https://docs.apeworx.io/ape/stable/userguides/projects.html).
-        
-        ### Compiling
-        
-        You can compile contracts within the `contracts/` directory of your project.
-        The `--size` option will display you the size of the contract.
-        
-        ```bash
-        ape compile --size
-        ```
-        
-        Learn more about compiling in Ape by following the [compile guide](https://docs.apeworx.io/ape/stable/userguides/compile.html).
-        
-        ### Testing
-        
-        Use Ape to test your smart-contract projects.
-        Provide the same arguments to `pytest` as you would to the `ape test` command.
-        
-        For example:
-        
-        ```bash
-        ape test -k test_only_one_thing
-        ```
-        
-        Visit the [testing guide](https://docs.apeworx.io/ape/stable/userguides/testing.html) to learn more about testing using Ape.
-        
-        ### Console
-        
-        Ape provides an `IPython` interactive console with useful pre-defined locals to interact with your project.
-        To interact with a deployed contract in a local environment, start by opening the console:
-        
-        ```bash
-        ape console --network ethereum:mainnet:infura
-        ```
-        
-        Visit [Ape Console](https://docs.apeworx.io/ape/stable/commands/console.html) to learn how to use Ape Console.
-        
-        ### Scripts
-        
-        If you want to run specific files in a `scripts/` directory, you can do it using the `ape run` command.
-        
-        ```bash
-        # This command will run a file named deploy in the scripts/ directory
-        $ ape run deploy
-        ```
-        
-        Learn more about scripting using Ape by following the [scripting guide](https://docs.apeworx.io/ape/stable/userguides/scripts.html).
-        
-        ### Logging
-        
-        To enable debug logging, run your command with the `--verbosity` flag using `DEBUG` as the value:
-        
-        ```bash
-        ape --verbosity DEBUG run
-        ```
-        
-        ### Networks
-        
-        You can work with registered networks, providers, and blockchain ecosystems (like Ethereum):
-        
-        ```python
-        from ape import networks
-        with networks.ethereum.mainnet.use_provider("infura"):
-            ...  # Work with the infura provider here
-        ```
-        
-        To learn more about networks in Ape, see [this guide](https://docs.apeworx.io/ape/stable/commands/networks.html).
-        
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8,<3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
 Provides-Extra: recommended-plugins
+License-File: LICENSE
+
+# Overview
+
+**Ape Framework** is an easy-to-use Web3 development tool.
+Users can compile, test, and interact with smart contracts all in one command line session.
+With our **modular plugin system**, Ape supports multiple contract languages and chains.
+
+Ape is built by [ApeWorX LTD](https://www.apeworx.io/).
+
+Join our [ApeWorX Discord server](https://discord.gg/apeworx) to stay up to date on new releases, plugins and tutorials.
+
+If you want to just get started, jump down to the [Playing with Ape](#playing-with-ape).
+
+## Documentation
+
+Read our [technical documentation](https://docs.apeworx.io/ape/stable/) to get a deeper understanding of our open source Framework.
+
+Read our [academic platform](https://academy.apeworx.io/) will help you master Ape Framework with tutorials and challenges.
+
+## Prerequisite
+
+In the latest release, Ape requires:
+
+- Linux or macOS
+- Python 3.8 up to 3.11
+- **Windows**: Install Windows Subsystem Linux [(WSL)](https://docs.microsoft.com/en-us/windows/wsl/install)
+
+Check your python version in a terminal with `python3 --version`.
+
+## Installation
+
+There are three ways to install ape: `pipx`, `pip`, or `Docker`.
+
+### Considerations for Installing:
+
+- We advise installing in a [virtualenv](https://pypi.org/project/virtualenv/) or [venv](https://docs.python.org/3/library/venv.html) to avoid interfering with *OS-level site packages*.
+
+- We advise installing **`ape`** with recommended plugins `pip install eth-ape'[recommended-plugins]'`.
+
+- We advise for **macOS** users to install virtual env via [homebrew](https://formulae.brew.sh/formula/virtualenv).
+
+### via `pipx` or `pip`
+
+1. Install `pipx` via their [installation instructions](https://pypa.github.io/pipx/) or `pip` via their [installation instructions](https://pip.pypa.io/en/stable/cli/pip_install/).
+
+2. Install **`ape`** via `pipx install eth-ape` or `pip install eth-ape`.
+
+### via `docker`
+
+Ape can also run in a docker container.
+
+Please visit our [Dockerhub](https://hub.docker.com/repository/docker/apeworx/ape) for more details on using Ape with Docker.
+
+```bash
+docker run \
+--volume $HOME/.ape:/home/harambe/.ape \
+--volume $HOME/.vvm:/home/harambe/.vvm \
+--volume $HOME/.solcx:/home/harambe/.solcx \
+--volume $PWD:/home/harambe/project \
+--workdir /home/harambe/project \
+apeworx/ape compile
+```
+
+## Playing with Ape
+
+After you installed Ape, you can run `ape --version` to make sure it works and is the latest version.
+
+There are two ways to interact with Ape:
+
+- [CLI Reference](https://docs.apeworx.io/ape/latest/index.html)
+
+- [Python Reference](https://docs.apeworx.io/ape/latest/index.html)
+
+Ape is both a CLI tool and a Python SDK.
+
+The CLI tool contains all the Ape commands and the Python SDK contains the classes and types needed to compose scripts, console actions, and tests.
+
+## **Ape Modular Plugin System:**
+
+Our [list of plugins](https://www.apeworx.io/#plugins) is the best way to have the most interoperable experience with Web3.
+
+**NOTE**: If a plugin does not originate from the [ApeWorX GitHub Organization](https://github.com/ApeWorX?q=ape&type=all), you will get a warning about installing 3rd-party plugins.
+
+Install 3rd party plugins at your own risk.
+
+Additionally, plugins that come bundled with **`ape`** in the core installation cannot be removed and are part of the **`ape`** core software.
+
+- Learn more about **installing** plugins from following this [installing user guide](https://docs.apeworx.io/ape/stable/userguides/installing_plugins.html).
+
+- Learn more about **developing** your own plugins from this [developing user guide](https://docs.apeworx.io/ape/stable/userguides/developing_plugins.html).
+
+### Accounts
+
+In Ape, you will need accounts to make transactions.
+You can import or generate accounts using the core `accounts` plugin:
+
+```bash
+ape accounts import acc0   # Will prompt for a private key
+ape accounts generate acc1
+```
+
+List all your accounts with the `list` command.
+
+```bash
+ape accounts list
+```
+
+Learn more about accounts in Ape by following the [accounts guide](https://docs.apeworx.io/ape/stable/userguides/accounts.html).
+
+### Plugins
+
+Add any plugins you may need, such as `vyper`.
+
+```bash
+ape plugins list -a
+ape plugins install vyper
+ape plugins list -a
+```
+
+## Projects
+
+When using Ape, you generally will work with a project.
+
+Learn more about smart-contract **projects** from this [projects guide](https://docs.apeworx.io/ape/stable/userguides/projects.html).
+
+### Compiling
+
+You can compile contracts within the `contracts/` directory of your project.
+The `--size` option will display you the size of the contract.
+
+```bash
+ape compile --size
+```
+
+Learn more about compiling in Ape by following the [compile guide](https://docs.apeworx.io/ape/stable/userguides/compile.html).
+
+### Testing
+
+Use Ape to test your smart-contract projects.
+Provide the same arguments to `pytest` as you would to the `ape test` command.
+
+For example:
+
+```bash
+ape test -k test_only_one_thing
+```
+
+Visit the [testing guide](https://docs.apeworx.io/ape/stable/userguides/testing.html) to learn more about testing using Ape.
+
+### Console
+
+Ape provides an `IPython` interactive console with useful pre-defined locals to interact with your project.
+To interact with a deployed contract in a local environment, start by opening the console:
+
+```bash
+ape console --network ethereum:mainnet:infura
+```
+
+Visit [Ape Console](https://docs.apeworx.io/ape/stable/commands/console.html) to learn how to use Ape Console.
+
+### Scripts
+
+If you want to run specific files in a `scripts/` directory, you can do it using the `ape run` command.
+
+```bash
+# This command will run a file named deploy in the scripts/ directory
+$ ape run deploy
+```
+
+Learn more about scripting using Ape by following the [scripting guide](https://docs.apeworx.io/ape/stable/userguides/scripts.html).
+
+### Logging
+
+To enable debug logging, run your command with the `--verbosity` flag using `DEBUG` as the value:
+
+```bash
+ape --verbosity DEBUG run
+```
+
+### Networks
+
+You can work with registered networks, providers, and blockchain ecosystems (like Ethereum):
+
+```python
+from ape import networks
+with networks.ethereum.mainnet.use_provider("infura"):
+    ...  # Work with the infura provider here
+```
+
+To learn more about networks in Ape, see [this guide](https://docs.apeworx.io/ape/stable/commands/networks.html).
```

### Comparing `eth-ape-0.6.8/src/eth_ape.egg-info/SOURCES.txt` & `eth-ape-0.6.9/src/eth_ape.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -119,17 +119,19 @@
 src/ape/plugins/project.py
 src/ape/plugins/query.py
 src/ape/pytest/README.md
 src/ape/pytest/__init__.py
 src/ape/pytest/config.py
 src/ape/pytest/contextmanagers.py
 src/ape/pytest/fixtures.py
+src/ape/pytest/gas.py
 src/ape/pytest/plugin.py
 src/ape/pytest/runners.py
 src/ape/types/__init__.py
+src/ape/types/address.py
 src/ape/types/signatures.py
 src/ape/types/trace.py
 src/ape/utils/__init__.py
 src/ape/utils/abi.py
 src/ape/utils/basemodel.py
 src/ape/utils/github.py
 src/ape/utils/misc.py
@@ -228,14 +230,15 @@
 tests/functional/data/contracts/ethereum/local/contract_b.json
 tests/functional/data/contracts/ethereum/local/contract_c.json
 tests/functional/data/contracts/ethereum/local/ds_note_test.json
 tests/functional/data/contracts/ethereum/local/has_error.json
 tests/functional/data/contracts/ethereum/local/proxy.json
 tests/functional/data/contracts/ethereum/local/reverts_contract.json
 tests/functional/data/contracts/ethereum/local/solidity_contract.json
+tests/functional/data/contracts/ethereum/local/sub_reverts_contract.json
 tests/functional/data/contracts/ethereum/local/vyper_contract.json
 tests/functional/data/contracts/ethereum/local/vyper_math_dev_checks.json
 tests/functional/data/manifests/OpenZeppelin/v3.1.0/OpenZeppelin.json
 tests/functional/data/manifests/OpenZeppelin/v4.4.2/OpenZeppelin.json
 tests/functional/data/projects/ApeProject/ape-config.yaml
 tests/functional/data/projects/ApeProject/contracts/ApeContract0.json
 tests/functional/data/projects/ApeProject/contracts/ApeContract1.json
@@ -246,17 +249,19 @@
 tests/functional/data/python/__init__.py
 tests/functional/data/sources/ContractA.sol
 tests/functional/data/sources/ContractB.sol
 tests/functional/data/sources/ContractC.sol
 tests/functional/data/sources/HasError.sol
 tests/functional/data/sources/Proxy.sol
 tests/functional/data/sources/RevertsContractVy.vy
+tests/functional/data/sources/SubRevertsVy.vy
 tests/functional/data/sources/TestContractSol.sol
 tests/functional/data/sources/TestContractVy.vy
 tests/functional/data/sources/VyperMathDevChecks.vy
+tests/functional/data/sources/interfaces/ISubRevertsVy.vy
 tests/functional/utils/__init__.py
 tests/functional/utils/test_github.py
 tests/functional/utils/test_misc.py
 tests/functional/utils/test_os.py
 tests/integration/__init__.py
 tests/integration/cli/__init__.py
 tests/integration/cli/conftest.py
```

### Comparing `eth-ape-0.6.8/src/eth_ape.egg-info/requires.txt` & `eth-ape-0.6.9/src/eth_ape.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 click<9,>=8.1.3
 ijson<4,>=3.1.4
 importlib-metadata
 ipython<9,>=8.5.0
+lazyasd>=0.1.4
 packaging<24,>=23.0
 pandas<2,>=1.3.0
 pluggy<2,>=0.12
 pydantic<2,>=1.9.2
 PyGithub<2,>=1.54
 pytest<8.0,>=6.0
 python-dateutil<3,>=2.8.2
-pyyaml<7,>=6.0
+PyYAML<7,>=5.0
 requests<3,>=2.28.1
 rich<13,>=12.5.1
 SQLAlchemy>=1.4.35
 tqdm<5.0,>=4.62.3
 traitlets>=5.3.0
 watchdog<3.0,>=2.1.9
 eth-abi<5,>=4.0.0
 eth-account<0.9,>=0.8
 eth-typing<4,>=3.1
 eth-utils<3,>=2.0.0
 hexbytes<1,>=0.2.3
 py-geth<4,>=3.12.0
-web3[tester]<7,>=6.0.0
+web3[tester]<7,>=6.4.0
 eip712<0.3,>=0.2.1
-ethpm-types<0.5,>=0.4.3
-evm-trace>=0.1.0a17
+ethpm-types<0.6,>=0.5.0
+evm-trace>=0.1.0a20
 
 [dev]
 pytest-xdist
 pytest-cov<5,>=4.0.0
 pytest-mock
 hypothesis<7.0,>=6.2.0
 hypothesis-jsonschema==0.19.0
 black<24,>=23.3.0
-mypy>=0.991
+mypy<1,>=0.991
 types-PyYAML
 types-requests
 types-setuptools
 pandas-stubs==1.2.0.62
 types-SQLAlchemy>=1.4.49
 flake8<7,>=6.0.0
 flake8-breakpoint<2,>=1.1.0
@@ -67,15 +68,15 @@
 Sphinx<7,>=6.1.3
 sphinx_rtd_theme<2,>=1.2.0
 sphinxcontrib-napoleon>=0.7
 sphinx-plausible<0.2,>=0.1.2
 
 [lint]
 black<24,>=23.3.0
-mypy>=0.991
+mypy<1,>=0.991
 types-PyYAML
 types-requests
 types-setuptools
 pandas-stubs==1.2.0.62
 types-SQLAlchemy>=1.4.49
 flake8<7,>=6.0.0
 flake8-breakpoint<2,>=1.1.0
```

### Comparing `eth-ape-0.6.8/tests/README.md` & `eth-ape-0.6.9/tests/README.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/conftest.py` & `eth-ape-0.6.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/conftest.py` & `eth-ape-0.6.9/tests/functional/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,24 +144,40 @@
 
 @pytest.fixture
 def reverts_contract_type(get_contract_type) -> ContractType:
     return get_contract_type("reverts_contract")
 
 
 @pytest.fixture
+def sub_reverts_contract_type(get_contract_type) -> ContractType:
+    return get_contract_type("sub_reverts_contract")
+
+
+@pytest.fixture
 def reverts_contract_container(reverts_contract_type) -> ContractContainer:
     return ContractContainer(contract_type=reverts_contract_type)
 
 
 @pytest.fixture
+def sub_reverts_contract_container(sub_reverts_contract_type) -> ContractContainer:
+    return ContractContainer(contract_type=sub_reverts_contract_type)
+
+
+@pytest.fixture
 def reverts_contract_instance(
-    owner, reverts_contract_container, networks_connected_to_tester, geth_provider
+    owner, reverts_contract_container, sub_reverts_contract_instance, geth_provider
 ) -> ContractInstance:
-    _ = geth_provider  # Must use geth, as it supports traces
-    return owner.deploy(reverts_contract_container, required_confirmations=0)
+    return owner.deploy(
+        reverts_contract_container, sub_reverts_contract_instance, required_confirmations=0
+    )
+
+
+@pytest.fixture
+def sub_reverts_contract_instance(owner, sub_reverts_contract_container, geth_provider):
+    return owner.deploy(sub_reverts_contract_container, required_confirmations=0)
 
 
 @pytest.fixture(params=("solidity", "vyper"))
 def contract_container(
     request, solidity_contract_container, vyper_contract_container, networks_connected_to_tester
 ):
     return solidity_contract_container if request.param == "solidity" else vyper_contract_container
```

### Comparing `eth-ape-0.6.8/tests/functional/conversion/test_encode_structs.py` & `eth-ape-0.6.9/tests/functional/conversion/test_encode_structs.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/conversion/test_ether.py` & `eth-ape-0.6.9/tests/functional/conversion/test_ether.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/conversion/test_timestamp.py` & `eth-ape-0.6.9/tests/functional/conversion/test_timestamp.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/data/contracts/ethereum/local/InterfaceImplementation.json` & `eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/InterfaceImplementation.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/data/contracts/ethereum/local/contract_a.json` & `eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/contract_a.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/data/contracts/ethereum/local/contract_b.json` & `eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/contract_b.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/data/contracts/ethereum/local/contract_c.json` & `eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/contract_c.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/data/contracts/ethereum/local/ds_note_test.json` & `eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/ds_note_test.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/data/contracts/ethereum/local/has_error.json` & `eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/has_error.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/data/contracts/ethereum/local/proxy.json` & `eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/proxy.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/data/contracts/ethereum/local/solidity_contract.json` & `eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/solidity_contract.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/data/contracts/ethereum/local/vyper_contract.json` & `eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/vyper_contract.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/data/contracts/ethereum/local/vyper_math_dev_checks.json` & `eth-ape-0.6.9/tests/functional/data/contracts/ethereum/local/vyper_math_dev_checks.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/data/manifests/OpenZeppelin/v3.1.0/OpenZeppelin.json` & `eth-ape-0.6.9/tests/functional/data/manifests/OpenZeppelin/v3.1.0/OpenZeppelin.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/data/manifests/OpenZeppelin/v4.4.2/OpenZeppelin.json` & `eth-ape-0.6.9/tests/functional/data/manifests/OpenZeppelin/v4.4.2/OpenZeppelin.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/data/projects/ApeProject/contracts/Contract.json` & `eth-ape-0.6.9/tests/functional/data/projects/ApeProject/contracts/Contract.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/data/python/__init__.py` & `eth-ape-0.6.9/tests/functional/data/python/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/data/sources/ContractA.sol` & `eth-ape-0.6.9/tests/functional/data/sources/ContractA.sol`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/data/sources/ContractB.sol` & `eth-ape-0.6.9/tests/functional/data/sources/ContractB.sol`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/data/sources/ContractC.sol` & `eth-ape-0.6.9/tests/functional/data/sources/ContractC.sol`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/data/sources/TestContractSol.sol` & `eth-ape-0.6.9/tests/functional/data/sources/TestContractSol.sol`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/data/sources/TestContractVy.vy` & `eth-ape-0.6.9/tests/functional/data/sources/TestContractVy.vy`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/test_accounts.py` & `eth-ape-0.6.9/tests/functional/test_accounts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pytest
 from eip712.messages import EIP712Message
 from eth_account.messages import encode_defunct
 
 import ape
 from ape import convert
+from ape.api import ImpersonatedAccount
 from ape.exceptions import AccountsError, NetworkError, ProjectError, SignatureError
 from ape.types.signatures import recover_signer
 from ape.utils.testing import DEFAULT_NUMBER_OF_TEST_ACCOUNTS
 from ape_ethereum.ecosystem import ProxyType
 from ape_test.accounts import TestAccount
 
 MISSING_VALUE_TRANSFER_ERR_MSG = "Must provide 'VALUE' or use 'send_everything=True"
@@ -86,14 +87,19 @@
     expected_sender_balance = initial_sender_balance - expected_sender_loss
     assert receiver.balance == expected_receiver_balance
     assert (
         sender.balance == expected_sender_balance
     ), f"difference: {abs(sender.balance - expected_sender_balance)}"
 
 
+def test_transfer_with_negative_value(sender, receiver):
+    with pytest.raises(AccountsError, match="Value cannot be negative."):
+        sender.transfer(receiver, value=-1)
+
+
 def test_transfer_without_value(sender, receiver):
     with pytest.raises(AccountsError, match=MISSING_VALUE_TRANSFER_ERR_MSG):
         sender.transfer(receiver)
 
 
 def test_transfer_without_value_send_everything_false(sender, receiver):
     with pytest.raises(AccountsError, match=MISSING_VALUE_TRANSFER_ERR_MSG):
@@ -285,14 +291,33 @@
         "Your provider does not support impersonating accounts:\n"
         f"No account with address '{test_address}'."
     )
     with pytest.raises(IndexError, match=expected_err_msg):
         _ = accounts[test_address]
 
 
+def test_impersonated_account_ignores_signature_check_on_txn(accounts):
+    address = "0xd8dA6BF26964aF9D7eEd9e03E53415D37aA96045"
+    account = ImpersonatedAccount(raw_address=address)
+
+    # Impersonate hack, since no providers in core actually support it.
+    accounts.test_accounts._impersonated_accounts[address] = account
+    other_0 = accounts.test_accounts[8]
+    other_1 = accounts.test_accounts[9]
+    txn = other_0.transfer(other_1, "1 gwei").transaction
+
+    # Hack in fake sender.
+    txn.sender = address
+    actual = txn.serialize_transaction()
+
+    # Normally, you'd get a signature error here, but since the account is registered
+    # as impersonated, ape lets it slide because it knows it won't match.
+    assert isinstance(actual, bytes)
+
+
 def test_contract_as_sender_non_fork_network(contract_instance):
     expected_err_msg = (
         "Your provider does not support impersonating accounts:\n"
         f"No account with address '{contract_instance}'."
     )
     with pytest.raises(IndexError, match=expected_err_msg):
         contract_instance.setNumber(5, sender=contract_instance)
```

### Comparing `eth-ape-0.6.8/tests/functional/test_chain.py` & `eth-ape-0.6.9/tests/functional/test_chain.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/test_cli.py` & `eth-ape-0.6.9/tests/functional/test_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/test_compilers.py` & `eth-ape-0.6.9/tests/functional/test_compilers.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/test_config.py` & `eth-ape-0.6.9/tests/functional/test_config.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/test_contract_container.py` & `eth-ape-0.6.9/tests/functional/test_contract_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,17 +68,19 @@
     implementation = chain.contracts.instance_at(proxy.address)
     assert implementation.contract_type == vyper_contract_instance.contract_type
 
 
 def test_source_path_in_project(project_with_contract):
     contracts_folder = project_with_contract.contracts_folder
     contract = project_with_contract.contracts["Contract"]
-    path = contracts_folder / contract.source_id
-    assert path.is_file()
-    assert project_with_contract.get_contract("Contract").source_path == path
+    contract_container = project_with_contract.get_contract("Contract")
+    expected = contracts_folder / contract.source_id
+
+    assert contract_container.source_path.is_file()
+    assert contract_container.source_path == expected
 
 
 def test_source_path_out_of_project(contract_container, project_with_contract):
     assert not contract_container.source_path
 
 
 def test_encode_constructor_input(contract_container, calldata):
```

### Comparing `eth-ape-0.6.8/tests/functional/test_contract_event.py` & `eth-ape-0.6.9/tests/functional/test_contract_event.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/test_contract_instance.py` & `eth-ape-0.6.9/tests/functional/test_contract_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,16 +155,24 @@
 
 
 def test_repr(vyper_contract_instance):
     assert re.match(
         rf"<TestContract((Sol)|(Vy)) {vyper_contract_instance.address}>",
         repr(vyper_contract_instance),
     )
-    assert repr(vyper_contract_instance.setNumber) == "setNumber(uint256 num)"
-    assert repr(vyper_contract_instance.myNumber) == "myNumber() -> uint256"
+    assert (
+        repr(vyper_contract_instance.setNumber)
+        == "<TestContractVy 0xF7F78379391C5dF2Db5B66616d18fF92edB82022>.setNumber"
+    )
+    assert str(vyper_contract_instance.setNumber) == "setNumber(uint256 num)"
+    assert (
+        repr(vyper_contract_instance.myNumber)
+        == "<TestContractVy 0xF7F78379391C5dF2Db5B66616d18fF92edB82022>.myNumber"
+    )
+    assert str(vyper_contract_instance.myNumber) == "myNumber() -> uint256"
     assert (
         repr(vyper_contract_instance.NumberChange) == "NumberChange(bytes32 b, uint256 prevNum, "
         "string dynData, uint256 indexed newNum, string indexed dynIndexed)"
     )
 
 
 def test_structs(contract_instance, sender, chain):
@@ -658,7 +666,17 @@
     Helps in cases where multiple errors have same name.
     Only happens when importing or using types from interfaces.
     """
     signature = error_contract.Unauthorized.abi.signature
     actual = error_contract.get_error_by_signature(signature)
     expected = error_contract.Unauthorized
     assert actual == expected
+
+
+def test_source_path(project_with_contract, owner):
+    contracts_folder = project_with_contract.contracts_folder
+    contract = project_with_contract.contracts["Contract"]
+    contract_instance = owner.deploy(project_with_contract.get_contract("Contract"))
+    expected = contracts_folder / contract.source_id
+
+    assert contract_instance.source_path.is_file()
+    assert contract_instance.source_path == expected
```

### Comparing `eth-ape-0.6.8/tests/functional/test_default_sender_context_manager.py` & `eth-ape-0.6.9/tests/functional/test_default_sender_context_manager.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/test_dependencies.py` & `eth-ape-0.6.9/tests/functional/test_dependencies.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,19 @@
             "github": "OpenZeppelin/openzeppelin-contracts",
         }
 
     return {"dependencies": [_create_oz_dependency("3.1.0"), _create_oz_dependency("4.4.2")]}
 
 
 @pytest.fixture
+def local_dependency(project_with_dependency_config):
+    return project_with_dependency_config.dependencies["testdependency"]["local"]
+
+
+@pytest.fixture
 def project_with_downloaded_dependencies(temp_config, config, oz_dependencies_config):
     manifests_directory = Path(__file__).parent / "data" / "manifests"
     oz_manifests = manifests_directory / "OpenZeppelin"
     oz_manifests_dest = config.packages_folder / "OpenZeppelin"
 
     if oz_manifests_dest.is_dir():
         shutil.rmtree(oz_manifests_dest)
@@ -31,40 +36,57 @@
         yield project
 
 
 def test_two_dependencies_with_same_name(project_with_downloaded_dependencies):
     name = "OpenZeppelin"
     oz_310 = project_with_downloaded_dependencies.dependencies[name]["3.1.0"]
     oz_442 = project_with_downloaded_dependencies.dependencies[name]["4.4.2"]
+    base_uri = "https://github.com/OpenZeppelin/openzeppelin-contracts/releases/tag"
 
     assert oz_310.version == "3.1.0"
     assert oz_310.name == name
+    assert str(oz_310.uri) == f"{base_uri}/v3.1.0"
     assert oz_442.version == "4.4.2"
     assert oz_442.name == name
+    assert str(oz_442.uri) == f"{base_uri}/v4.4.2"
 
 
-def test_dependency_with_longer_contracts_folder(project_with_dependency_config, config):
-    dependency = project_with_dependency_config.dependencies["testdependency"]["local"]
-    expected = "source/v0.1"
-    actual = dependency.contracts_folder
-    assert actual == expected
+def test_dependency_contracts_folder(config, local_dependency):
+    """
+    The local dependency fixture uses a longer contracts folder path.
+    This test ensures that the contracts folder field is honored, specifically
+    In the case when it contains sub-paths.
+    """
+    actual = local_dependency.contracts_folder
+    assert actual == "source/v0.1"
+
+
+def test_local_dependency(local_dependency, config):
+    assert local_dependency.name == "testdependency"
+    assert local_dependency.version_id == "local"
+    expected = config.DATA_FOLDER / "packages" / "testdependency" / "local" / "testdependency.json"
+    assert str(local_dependency.uri) == f"file://{expected}"
 
 
 def test_access_dependency_contracts(project_with_downloaded_dependencies):
     name = "OpenZeppelin"
     oz_442 = project_with_downloaded_dependencies.dependencies[name]["4.4.2"]
     contract = oz_442.AccessControl
     assert contract.contract_type.name == "AccessControl"
 
 
-def test_dependency_with_non_version_version_id(recwarn, dependency_manager):
+@pytest.mark.parametrize("ref", ("main", "v1.0.0", "1.0.0"))
+def test_dependency_using_reference(ref, recwarn, dependency_manager):
     dependency_config = {
         "github": "apeworx/testfoobartest",
         "name": "foobar",
-        "branch": "main",
+        "ref": ref,
     }
     dependency = dependency_manager.decode_dependency(dependency_config)
     _ = dependency.cached_manifest
+    assert dependency.version is None
+    assert dependency.ref == ref
+    assert str(dependency.uri) == f"https://github.com/apeworx/testfoobartest/tree/{ref}"
 
     # Tests against bug where we tried creating version objects out of branch names,
     # thus causing warnings to show in `ape test` runs.
     assert DeprecationWarning not in [w.category for w in recwarn.list]
```

### Comparing `eth-ape-0.6.8/tests/functional/test_ecosystem.py` & `eth-ape-0.6.9/tests/functional/test_ecosystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,7 +223,18 @@
     config_dict = {"ethereum": {"mainnet_fork": {"default_transaction_type": 0}}}
     assert ethereum.default_transaction_type == TransactionType.DYNAMIC
 
     with temp_config(config_dict):
         ethereum._default_network = "mainnet-fork"
         assert ethereum.default_transaction_type == TransactionType.STATIC
         ethereum._default_network = LOCAL_NETWORK_NAME
+
+
+@pytest.mark.parametrize("network_name", (LOCAL_NETWORK_NAME, "mainnet-fork", "mainnet_fork"))
+def test_gas_limit_local_networks(ethereum, network_name):
+    network = ethereum.get_network(network_name)
+    assert network.gas_limit == "max"
+
+
+def test_gas_limit_live_networks(ethereum):
+    network = ethereum.get_network("goerli")
+    assert network.gas_limit == "auto"
```

### Comparing `eth-ape-0.6.8/tests/functional/test_geth.py` & `eth-ape-0.6.9/tests/functional/test_geth.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 import pytest
 from eth_typing import HexStr
 
 from ape.exceptions import (
     BlockNotFoundError,
     ContractLogicError,
     NetworkMismatchError,
+    OutOfGasError,
     TransactionNotFoundError,
 )
+from ape.utils import ZERO_ADDRESS
 from ape_ethereum.ecosystem import Block
 from ape_geth.provider import Geth
 from tests.conftest import GETH_URI, geth_process_test
 from tests.functional.data.python import TRACE_RESPONSE
 
 TRANSACTION_HASH = "0x053cba5c12172654d894f66d5670bab6215517a94189a9ffc09bc40a589ec04d"
 LOCAL_TRACE = r"""
@@ -73,14 +75,24 @@
     │     993453434534534534534977788884443333
     │   \] \[731 gas\]
     └── ContractC\.methodC1\(windows95="simpler", jamaica=111, cardinal=ContractA\) \[44525 gas\]
 """
 
 
 @pytest.fixture
+def geth_account(accounts):
+    return accounts.test_accounts[5]
+
+
+@pytest.fixture
+def geth_contract(geth_account, vyper_contract_container, geth_provider):
+    return geth_account.deploy(vyper_contract_container, 0)
+
+
+@pytest.fixture
 def mock_geth(geth_provider, mock_web3):
     provider = Geth(
         name="geth",
         network=geth_provider.network,
         provider_settings={},
         data_folder=Path("."),
         request_header="",
@@ -97,14 +109,24 @@
 
 
 @pytest.fixture
 def geth_receipt(contract_with_call_depth_geth, owner, geth_provider):
     return contract_with_call_depth_geth.methodWithoutArguments(sender=owner)
 
 
+@pytest.fixture
+def geth_vyper_contract(owner, vyper_contract_container, geth_provider):
+    return owner.deploy(vyper_contract_container, 0)
+
+
+@pytest.fixture
+def geth_vyper_receipt(geth_vyper_contract, owner):
+    return geth_vyper_contract.setNumber(44, sender=owner)
+
+
 @geth_process_test
 def test_uri(geth_provider):
     assert geth_provider.uri == GETH_URI
 
 
 @geth_process_test
 def test_uri_uses_value_from_config(geth_provider, temp_config):
@@ -114,46 +136,39 @@
     try:
         with temp_config(config):
             assert geth_provider.uri == "value/from/config"
     finally:
         geth_provider.provider_settings = settings
 
 
-def test_tx_revert(accounts, sender, vyper_contract_container):
+def test_tx_revert(accounts, sender, geth_vyper_contract, owner):
     # 'sender' is not the owner so it will revert (with a message)
-    contract = accounts.test_accounts[-1].deploy(vyper_contract_container, 0)
     with pytest.raises(ContractLogicError, match="!authorized"):
-        contract.setNumber(5, sender=sender)
+        geth_vyper_contract.setNumber(5, sender=sender)
 
 
-def test_revert_no_message(accounts, vyper_contract_container):
+def test_revert_no_message(accounts, geth_vyper_contract, owner):
     # The Contract raises empty revert when setting number to 5.
     expected = "Transaction failed."  # Default message
-    owner = accounts.test_accounts[-2]
-    contract = owner.deploy(vyper_contract_container, 0)
     with pytest.raises(ContractLogicError, match=expected):
-        contract.setNumber(5, sender=owner)
+        geth_vyper_contract.setNumber(5, sender=owner)
 
 
 @geth_process_test
-def test_contract_interaction(geth_provider, vyper_contract_container, accounts):
-    owner = accounts.test_accounts[-2]
-    contract = owner.deploy(vyper_contract_container, 0)
-    contract.setNumber(102, sender=owner)
-    assert contract.myNumber() == 102
+def test_contract_interaction(owner, geth_vyper_contract):
+    geth_vyper_contract.setNumber(102, sender=owner)
+    assert geth_vyper_contract.myNumber() == 102
 
 
 @geth_process_test
-def test_get_call_tree(geth_provider, vyper_contract_container, accounts):
-    owner = accounts.test_accounts[-3]
-    contract = owner.deploy(vyper_contract_container, 0)
-    receipt = contract.setNumber(10, sender=owner)
+def test_get_call_tree(geth_vyper_contract, owner, geth_provider):
+    receipt = geth_vyper_contract.setNumber(10, sender=owner)
     result = geth_provider.get_call_tree(receipt.txn_hash)
     expected = (
-        rf"{contract.address}.0x3fb5c1cb"
+        rf"{geth_vyper_contract.address}.0x3fb5c1cb"
         r"\(0x000000000000000000000000000000000000000000000000000000000000000a\) \[\d+ gas\]"
     )
     actual = repr(result)
     assert re.match(expected, actual)
 
 
 def test_get_call_tree_erigon(mock_web3, mock_geth, parity_trace_response):
@@ -177,21 +192,19 @@
 
 def test_repr_on_live_network_and_disconnected(networks):
     geth = networks.get_provider_from_choice("ethereum:goerli:geth")
     assert repr(geth) == "<geth chain_id=5>"
 
 
 @geth_process_test
-def test_get_logs(geth_provider, accounts, vyper_contract_container):
-    owner = accounts.test_accounts[-4]
-    contract = owner.deploy(vyper_contract_container, 0)
-    contract.setNumber(101010, sender=owner)
-    actual = contract.NumberChange[-1]
+def test_get_logs(geth_vyper_contract, owner):
+    geth_vyper_contract.setNumber(101010, sender=owner)
+    actual = geth_vyper_contract.NumberChange[-1]
     assert actual.event_name == "NumberChange"
-    assert actual.contract_address == contract.address
+    assert actual.contract_address == geth_vyper_contract.address
     assert actual.event_arguments["newNum"] == 101010
 
 
 @geth_process_test
 def test_chain_id_when_connected(geth_provider):
     assert geth_provider.chain_id == 1337
 
@@ -277,39 +290,36 @@
     actual = geth_provider.get_receipt(receipt.txn_hash)
     assert receipt.txn_hash == actual.txn_hash
     assert actual.receiver == contract.address
     assert actual.sender == receipt.sender
 
 
 @geth_process_test
-def test_snapshot_and_revert(geth_provider, accounts, vyper_contract_container):
-    owner = accounts.test_accounts[-6]
-    contract = owner.deploy(vyper_contract_container, 0)
-
+def test_snapshot_and_revert(geth_provider, geth_account, geth_contract):
     snapshot = geth_provider.snapshot()
-    start_nonce = owner.nonce
-    contract.setNumber(211112, sender=owner)  # Advance a block
+    start_nonce = geth_account.nonce
+    geth_contract.setNumber(211112, sender=geth_account)  # Advance a block
     actual_block_number = geth_provider.get_block("latest").number
     expected_block_number = snapshot + 1
-    actual_nonce = owner.nonce
+    actual_nonce = geth_account.nonce
     expected_nonce = start_nonce + 1
     assert actual_block_number == expected_block_number
     assert actual_nonce == expected_nonce
 
     geth_provider.revert(snapshot)
 
     actual_block_number = geth_provider.get_block("latest").number
     expected_block_number = snapshot
-    actual_nonce = owner.nonce
+    actual_nonce = geth_account.nonce
     expected_nonce = start_nonce
     assert actual_block_number == expected_block_number
     assert actual_nonce == expected_nonce
 
     # Use account after revert
-    receipt = contract.setNumber(311113, sender=owner)  # Advance a block
+    receipt = geth_contract.setNumber(311113, sender=geth_account)  # Advance a block
     assert not receipt.failed
 
 
 @pytest.fixture
 def captrace(capsys):
     class CapTrace:
         def read_trace(self, expected_start: str, file=None):
@@ -380,13 +390,89 @@
     actual_len = len(actual_lines)
     expected_len = len(expected_lines)
     if expected_len > actual_len:
         rest = "\n".join(expected_lines[actual_len:])
         pytest.fail(f"Missing expected lines: {rest}")
 
 
+@geth_process_test
 def test_custom_error(error_contract_geth, not_owner):
     contract = error_contract_geth
     with pytest.raises(contract.Unauthorized) as err:
         contract.withdraw(sender=not_owner)
 
     assert err.value.inputs == {"addr": not_owner.address, "counter": 123}
+
+
+@geth_process_test
+def test_return_value_list(geth_account, geth_contract, geth_provider):
+    receipt = geth_contract.getFilledArray.transact(sender=geth_account)
+    assert receipt.return_value == [1, 2, 3]
+
+
+@geth_process_test
+def test_return_value_nested_address_array(geth_account, geth_contract, geth_provider):
+    receipt = geth_contract.getNestedAddressArray.transact(sender=geth_account)
+    expected = [
+        [geth_account.address, geth_account.address, geth_account.address],
+        [ZERO_ADDRESS, ZERO_ADDRESS, ZERO_ADDRESS],
+    ]
+    assert receipt.return_value == expected
+
+
+@geth_process_test
+def test_return_value_nested_struct_in_tuple(geth_account, geth_contract, geth_provider):
+    receipt = geth_contract.getNestedStructWithTuple1.transact(sender=geth_account)
+    actual = receipt.return_value
+    assert actual[0].t.a == geth_account.address
+    assert actual[0].foo == 1
+    assert actual[1] == 1
+
+
+@geth_process_test
+def test_get_pending_block(geth_provider, geth_account, accounts):
+    """
+    Pending timestamps can be weird.
+    This ensures we can check those are various strange states of geth.
+    """
+    actual = geth_provider.get_block("latest")
+    assert isinstance(actual, Block)
+
+    snap = geth_provider.snapshot()
+
+    # Transact to increase block
+    geth_account.transfer(accounts.test_accounts[0], "1 gwei")
+    actual = geth_provider.get_block("latest")
+    assert isinstance(actual, Block)
+
+    # Restore state before transaction
+    geth_provider.revert(snap)
+    actual = geth_provider.get_block("latest")
+    assert isinstance(actual, Block)
+
+
+@geth_process_test
+def test_isolate(chain, geth_contract, geth_account):
+    number_at_start = 444
+    geth_contract.setNumber(number_at_start, sender=geth_account)
+    start_head = chain.blocks.height
+
+    with chain.isolate():
+        geth_contract.setNumber(333, sender=geth_account)
+        assert geth_contract.myNumber() == 333
+        assert chain.blocks.height == start_head + 1
+
+    assert geth_contract.myNumber() == number_at_start
+    assert chain.blocks.height == start_head
+
+
+@geth_process_test
+def test_out_of_gas_error(geth_contract, geth_account, geth_provider):
+    """
+    Attempt to transact with not quite enough gas. We should get an error saying
+    we ran out of gas.
+    """
+    txn = geth_contract.setNumber.as_transaction(333, sender=geth_account)
+    gas = geth_provider.estimate_gas_cost(txn)
+    txn.gas_limit = gas - 1
+    with pytest.raises(OutOfGasError):
+        geth_account.call(txn)
```

### Comparing `eth-ape-0.6.8/tests/functional/test_logging.py` & `eth-ape-0.6.9/tests/functional/test_logging.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/test_networks.py` & `eth-ape-0.6.9/tests/functional/test_networks.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/test_plugins.py` & `eth-ape-0.6.9/tests/functional/test_plugins.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/test_project.py` & `eth-ape-0.6.9/tests/functional/test_project.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/test_provider.py` & `eth-ape-0.6.9/tests/functional/test_provider.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from unittest import mock
 
 import pytest
 from eth_typing import HexStr
+from eth_utils import ValidationError
 
 from ape.exceptions import BlockNotFoundError, ProviderNotConnectedError, TransactionNotFoundError
 from ape.types import LogFilter
 from ape_test.provider import CHAIN_ID
 
 
 @pytest.mark.parametrize("block_id", (0, "0", "0x0", HexStr("0x0")))
@@ -151,7 +152,47 @@
     """
     Test that the address is an AddressType.
     """
     balance = networks.provider.get_balance(accounts.test_accounts[0].address)
 
     assert type(balance) == int
     assert balance == 1000000000000000000000000
+
+
+def test_set_timestamp(eth_tester_provider):
+    pending_at_start = eth_tester_provider.get_block("pending").timestamp
+    expected = pending_at_start + 100
+    eth_tester_provider.set_timestamp(expected)
+    eth_tester_provider.mine()
+    actual = eth_tester_provider.get_block("pending").timestamp
+    assert actual == expected + 1  # Mining adds another second.
+
+
+def test_set_timestamp_to_same_time(eth_tester_provider):
+    """
+    Eth tester normally fails when setting the timestamp to the same time.
+    However, in Ape, we treat it as a no-op and let it pass.
+    """
+    expected = eth_tester_provider.get_block("pending").timestamp
+    eth_tester_provider.set_timestamp(expected)
+    actual = eth_tester_provider.get_block("pending").timestamp
+    assert actual == expected
+
+
+def test_set_timestamp_handle_same_time_race_condition(mocker, eth_tester_provider):
+    """
+    Ensures that when we get an error saying the timestamps are the same,
+    we ignore it and treat it as a noop. This handles the race condition
+    when the block advances after ``set_timestamp`` has been called but before
+    the operation completes.
+    """
+
+    def side_effect(*args, **kwargs):
+        raise ValidationError(
+            "timestamp must be strictly later than parent, "
+            "but is 0 seconds before.\n"
+            "- child  : 0\n"
+            "- parent : 0."
+        )
+
+    mocker.patch.object(eth_tester_provider.evm_backend, "time_travel", side_effect=side_effect)
+    eth_tester_provider.set_timestamp(123)
```

### Comparing `eth-ape-0.6.8/tests/functional/test_query.py` & `eth-ape-0.6.9/tests/functional/test_query.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/test_receipt.py` & `eth-ape-0.6.9/tests/functional/test_receipt.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,12 +161,12 @@
         gas_price=0,
         block_number=0,
         transaction=txn,
     )
     with pytest.raises(OutOfGasError) as err:
         receipt.raise_for_status()
 
-    assert err.value.txn == receipt.transaction
+    assert err.value.txn == receipt
 
 
 def test_receipt_chain_id(invoke_receipt, eth_tester_provider):
     assert invoke_receipt.chain_id == eth_tester_provider.chain_id
```

### Comparing `eth-ape-0.6.8/tests/functional/test_revert_context_manager.py` & `eth-ape-0.6.9/tests/functional/test_revert_context_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,14 +121,44 @@
         reverts_contract_instance.revertStrings(2, sender=owner)
 
     with reverts(dev_message=re.compile(r"dev: err\w+")):
         reverts_contract_instance.revertStrings2(2, sender=owner)
 
 
 @geth_process_test
+def test_dev_revert_from_sub_contract(owner, reverts_contract_instance, geth_provider):
+    """
+    Test to ensure we can assert on dev messages from inner-contracts.
+    """
+    with reverts(dev_message="dev: sub-zero"):
+        reverts_contract_instance.subRevertStrings(0, sender=owner)
+
+
+@geth_process_test
+def test_dev_revert_deep_in_method(owner, reverts_contract_instance, geth_provider):
+    """
+    Test to ensure we can assert on a dev message that is in the middle of a
+    complicated function implementation.
+    """
+    with reverts(dev_message="dev: foobarbaz"):
+        reverts_contract_instance.revertStrings(13, sender=owner)
+
+    with reverts(dev_message="dev: such modifiable, wow"):
+        reverts_contract_instance.revertStrings(4, sender=owner)
+
+    with reverts(dev_message="dev: great job"):
+        reverts_contract_instance.revertStrings(31337, sender=owner)
+
+
+def test_dev_revert_in_loop(owner, reverts_contract_instance, geth_provider):
+    with reverts(dev_message="dev: loop test"):
+        reverts_contract_instance.revertStrings2(12, sender=owner)
+
+
+@geth_process_test
 def test_dev_revert_nonpayable_check(owner, vyper_contract_container, geth_provider):
     """
     Tests that we can assert on dev messages injected from the compiler.
     """
     contract = owner.deploy(vyper_contract_container, 0)
     with reverts(dev_message="dev: Cannot send ether to non-payable function"):
         contract.setNumber(123, sender=owner, value=1)
```

### Comparing `eth-ape-0.6.8/tests/functional/test_transaction.py` & `eth-ape-0.6.9/tests/functional/test_transaction.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/test_types.py` & `eth-ape-0.6.9/tests/functional/test_types.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/utils/test_github.py` & `eth-ape-0.6.9/tests/functional/utils/test_github.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/utils/test_misc.py` & `eth-ape-0.6.9/tests/functional/utils/test_misc.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/functional/utils/test_os.py` & `eth-ape-0.6.9/tests/functional/utils/test_os.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/integration/cli/conftest.py` & `eth-ape-0.6.9/tests/integration/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/integration/cli/projects/geth/contracts/contract.json` & `eth-ape-0.6.9/tests/integration/cli/projects/geth/contracts/contract.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/integration/cli/projects/geth/contracts/token_a.json` & `eth-ape-0.6.9/tests/integration/cli/projects/geth/contracts/token_a.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/integration/cli/projects/geth/contracts/token_b.json` & `eth-ape-0.6.9/tests/integration/cli/projects/geth/contracts/token_b.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/integration/cli/projects/geth/tests/test_using_local_geth.py` & `eth-ape-0.6.9/tests/integration/cli/projects/geth/tests/test_using_local_geth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import pytest
+
+
 def test_provider(project, networks):
     """
     Tests that the network gets set from ape-config.yaml.
     """
     assert networks.provider.name == "geth"
 
 
@@ -62,7 +65,17 @@
     """
     Call a method excluded in the ``ape-config.yaml`` file
     for asserting it does not show in gas report.
     """
     account = accounts[-4]
     receipt = contract.setAddress(account.address, sender=account)
     assert not receipt.failed
+
+
+@pytest.mark.use_network("ethereum:local:test")
+def test_switch_back_to_eth_tester(chain):
+    """
+    Test to verify the `use_network` marker works.
+    This test is in the geth project because that is the only test project
+    that has multiple providers.
+    """
+    assert chain.provider.name == "test"
```

### Comparing `eth-ape-0.6.8/tests/integration/cli/projects/test/tests/test_fixture_isolation.py` & `eth-ape-0.6.9/tests/integration/cli/projects/test/tests/test_fixture_isolation.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/integration/cli/projects/test/tests/test_networks.py` & `eth-ape-0.6.9/tests/integration/cli/projects/test/tests/test_networks.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/integration/cli/projects/with-contracts/contracts/ContractA.json` & `eth-ape-0.6.9/tests/integration/cli/projects/with-contracts/contracts/ContractA.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/integration/cli/projects/with-contracts/contracts/RawSolidityOutput.json` & `eth-ape-0.6.9/tests/integration/cli/projects/with-contracts/contracts/RawSolidityOutput.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/integration/cli/projects/with-contracts/contracts/RawVyperOutput.json` & `eth-ape-0.6.9/tests/integration/cli/projects/with-contracts/contracts/RawVyperOutput.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/integration/cli/projects/with-contracts/tests/test_contract.py` & `eth-ape-0.6.9/tests/integration/cli/projects/with-contracts/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/integration/cli/test_accounts.py` & `eth-ape-0.6.9/tests/integration/cli/test_accounts.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/integration/cli/test_compile.py` & `eth-ape-0.6.9/tests/integration/cli/test_compile.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,20 +131,21 @@
     finally:
         if temp_dir.is_dir():
             shutil.rmtree(temp_dir)
 
 
 @skip_projects_except("multiple-interfaces")
 def test_compile_when_source_contains_return_characters(ape_cli, runner, project, clean_cache):
-    # NOTE: This tests a bugfix where a source file contained return-characters
-    # and that triggered endless re-compiles because it technically contains extra
-    # bytes than the ones that show up in the text.
-
-    # Change the contents of a file to contain the '\r' character.
+    """
+    This tests a bugfix where a source file contained return-characters
+    and that triggered endless re-compiles because it technically contains extra
+    bytes than the ones that show up in the text.
+    """
     source_path = project.contracts_folder / "Interface.json"
+    # Change the contents of a file to contain the '\r' character.
     modified_source_text = f"{source_path.read_text()}\r"
     source_path.unlink()
     source_path.touch()
     source_path.write_text(modified_source_text)
 
     result = runner.invoke(ape_cli, ["compile"], catch_exceptions=False)
     assert result.exit_code == 0, result.output
```

### Comparing `eth-ape-0.6.8/tests/integration/cli/test_console.py` & `eth-ape-0.6.9/tests/integration/cli/test_console.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/integration/cli/test_init.py` & `eth-ape-0.6.9/tests/integration/cli/test_init.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/integration/cli/test_networks.py` & `eth-ape-0.6.9/tests/integration/cli/test_networks.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/integration/cli/test_plugins.py` & `eth-ape-0.6.9/tests/integration/cli/test_plugins.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/integration/cli/test_run.py` & `eth-ape-0.6.9/tests/integration/cli/test_run.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.6.8/tests/integration/cli/test_test.py` & `eth-ape-0.6.9/tests/integration/cli/test_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,21 +163,22 @@
     assert "F _function_isolation" not in "\n".join(result.outlines)
 
 
 @skip_projects_except("test", "with-contracts")
 def test_fixture_docs(setup_pytester, project, pytester, eth_tester_provider):
     _ = eth_tester_provider  # Ensure using EthTester for this test.
     result = pytester.runpytest("-q", "--fixtures")
+    actual = "\n".join(result.outlines)
 
     # 'accounts', 'networks', 'chain', and 'project' (etc.)
     fixtures = [prop for n, prop in vars(PytestApeFixtures).items() if not n.startswith("_")]
     for fixture in fixtures:
         # The doc str of the fixture shows in the CLI output
-        doc_str = fixture.__doc__.strip()
-        assert doc_str in "\n".join(result.outlines)
+        for doc_str in fixture.__doc__.splitlines():
+            assert doc_str.strip() in actual
 
 
 @skip_projects_except("test")
 def test_gas_flag_when_not_supported(setup_pytester, project, pytester, eth_tester_provider):
     _ = eth_tester_provider  # Ensure using EthTester for this test.
     setup_pytester(project.path.name)
     result = pytester.runpytest("--gas")
```

### Comparing `eth-ape-0.6.8/tests/integration/cli/utils.py` & `eth-ape-0.6.9/tests/integration/cli/utils.py`

 * *Files identical despite different names*

