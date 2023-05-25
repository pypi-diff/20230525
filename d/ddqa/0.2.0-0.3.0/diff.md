# Comparing `tmp/ddqa-0.2.0.tar.gz` & `tmp/ddqa-0.3.0.tar.gz`

## Comparing `ddqa-0.2.0.tar` & `ddqa-0.3.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ddqa-0.2.0/.gitattributes
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ddqa-0.2.0/.linkcheckerrc
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ddqa-0.2.0/HISTORY.md
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 ddqa-0.2.0/mkdocs.yml
--rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 ddqa-0.2.0/pyoxidizer.bzl
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 ddqa-0.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0    12674 2020-02-02 00:00:00.000000 ddqa-0.2.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 ddqa-0.2.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 ddqa-0.2.0/.github/workflows/publish-docs.yml
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ddqa-0.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 ddqa-0.2.0/docs/index.md
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 ddqa-0.2.0/docs/install.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ddqa-0.2.0/docs/.snippets/abbrs.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ddqa-0.2.0/docs/.snippets/links.txt
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 ddqa-0.2.0/docs/assets/css/custom.css
--rw-r--r--   0        0        0    40436 2020-02-02 00:00:00.000000 ddqa-0.2.0/docs/assets/images/favicon.ico
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 ddqa-0.2.0/docs/assets/images/logo.svg
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 ddqa-0.2.0/docs/config/repo.md
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 ddqa-0.2.0/docs/config/user.md
--rw-r--r--   0        0        0   193753 2020-02-02 00:00:00.000000 ddqa-0.2.0/screenshots/config.PNG
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/__init__.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/py.typed
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/app/__init__.py
--rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/app/core.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/app/style.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/cli/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/cli/config/__init__.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/cli/config/edit.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/cli/config/explore.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/cli/config/find.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/cli/config/restore.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/cli/config/show.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/cli/create/__init__.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/cli/status/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/cli/sync/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/config/__init__.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/config/constants.py
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/config/core.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/config/file.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/config/utils.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/data/__init__.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/data/logo.png
--rw-r--r--   0        0        0   345099 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/data/shame.png
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/models/__init__.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/models/github.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/models/jira.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/models/config/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/models/config/app.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/models/config/auth.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/models/config/repo.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/models/config/team.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/screens/__init__.py
--rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/screens/configure.py
--rw-r--r--   0        0        0    15706 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/screens/create.py
--rw-r--r--   0        0        0    17067 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/screens/status.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/screens/sync.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/utils/__init__.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/utils/ci.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/utils/errors.py
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/utils/fs.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/utils/git.py
--rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/utils/github.py
--rw-r--r--   0        0        0    11019 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/utils/jira.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/utils/network.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/utils/structures.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/utils/time.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/utils/widgets.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/widgets/__init__.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/widgets/input.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/widgets/layout.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ddqa-0.2.0/src/ddqa/widgets/static.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/config/__init__.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/config/test_edit.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/config/test_explore.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/config/test_find.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/config/test_restore.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/config/test_show.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/create/__init__.py
--rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/create/test_create.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/status/__init__.py
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/status/test_status.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/sync/__init__.py
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/cli/sync/test_sync.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/helpers/__init__.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/helpers/api.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/screens/__init__.py
--rw-r--r--   0        0        0    23170 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/screens/test_configure.py
--rw-r--r--   0        0        0    34995 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/screens/test_create.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/screens/test_status.py
--rw-r--r--   0        0        0     7905 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/screens/test_sync.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/utils/test_fs.py
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/utils/test_git.py
--rw-r--r--   0        0        0    22924 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/utils/test_github.py
--rw-r--r--   0        0        0    28668 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/utils/test_jira.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/utils/test_structures.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 ddqa-0.2.0/tests/utils/test_time.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 ddqa-0.2.0/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ddqa-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 ddqa-0.2.0/README.md
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 ddqa-0.2.0/hatch.toml
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 ddqa-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 ddqa-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ddqa-0.3.0/.gitattributes
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ddqa-0.3.0/.linkcheckerrc
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 ddqa-0.3.0/HISTORY.md
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 ddqa-0.3.0/mkdocs.yml
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 ddqa-0.3.0/pyoxidizer.bzl
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 ddqa-0.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0    12900 2020-02-02 00:00:00.000000 ddqa-0.3.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 ddqa-0.3.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 ddqa-0.3.0/.github/workflows/publish-docs.yml
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ddqa-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 ddqa-0.3.0/docs/index.md
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 ddqa-0.3.0/docs/install.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ddqa-0.3.0/docs/.snippets/abbrs.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ddqa-0.3.0/docs/.snippets/links.txt
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 ddqa-0.3.0/docs/assets/css/custom.css
+-rw-r--r--   0        0        0    40436 2020-02-02 00:00:00.000000 ddqa-0.3.0/docs/assets/images/favicon.ico
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 ddqa-0.3.0/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 ddqa-0.3.0/docs/config/repo.md
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 ddqa-0.3.0/docs/config/user.md
+-rw-r--r--   0        0        0   193753 2020-02-02 00:00:00.000000 ddqa-0.3.0/screenshots/config.PNG
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/py.typed
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/app/__init__.py
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/app/core.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/app/style.py
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/cli/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/cli/config/__init__.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/cli/config/edit.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/cli/config/explore.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/cli/config/find.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/cli/config/restore.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/cli/config/show.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/cli/create/__init__.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/cli/status/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/cli/sync/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/config/__init__.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/config/constants.py
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/config/core.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/config/file.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/config/utils.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/data/__init__.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/data/logo.png
+-rw-r--r--   0        0        0   345099 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/data/shame.png
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/models/__init__.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/models/github.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/models/jira.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/models/config/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/models/config/app.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/models/config/auth.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/models/config/repo.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/models/config/team.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/screens/__init__.py
+-rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/screens/configure.py
+-rw-r--r--   0        0        0    15706 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/screens/create.py
+-rw-r--r--   0        0        0    17067 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/screens/status.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/screens/sync.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/utils/__init__.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/utils/ci.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/utils/errors.py
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/utils/fs.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/utils/git.py
+-rw-r--r--   0        0        0     9133 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/utils/github.py
+-rw-r--r--   0        0        0    11019 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/utils/jira.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/utils/network.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/utils/structures.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/utils/time.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/utils/widgets.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/widgets/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/widgets/input.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/widgets/layout.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ddqa-0.3.0/src/ddqa/widgets/static.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/config/__init__.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/config/test_edit.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/config/test_explore.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/config/test_find.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/config/test_restore.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/config/test_show.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/create/__init__.py
+-rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/create/test_create.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/status/__init__.py
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/status/test_status.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/sync/__init__.py
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/cli/sync/test_sync.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/helpers/api.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/screens/__init__.py
+-rw-r--r--   0        0        0    23170 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/screens/test_configure.py
+-rw-r--r--   0        0        0    34995 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/screens/test_create.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/screens/test_status.py
+-rw-r--r--   0        0        0     7905 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/screens/test_sync.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/utils/test_fs.py
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/utils/test_git.py
+-rw-r--r--   0        0        0    22924 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/utils/test_github.py
+-rw-r--r--   0        0        0    28668 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/utils/test_jira.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/utils/test_structures.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 ddqa-0.3.0/tests/utils/test_time.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 ddqa-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ddqa-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 ddqa-0.3.0/README.md
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 ddqa-0.3.0/hatch.toml
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 ddqa-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 ddqa-0.3.0/PKG-INFO
```

### Comparing `ddqa-0.2.0/HISTORY.md` & `ddqa-0.3.0/HISTORY.md`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
+## 0.3.0 - 2023-05-24
+
+***Added:***
+
+- Upgrade Textual to 0.20.1
+- Upgrade PyApp to 0.7.0
+
 ## 0.2.0 - 2023-05-17
 
 ***Changed:***
 
 - Remove vendored `pyperclip` dependency and the `--copy` flag of the `config find` command
 
 ***Fixed:***
```

### Comparing `ddqa-0.2.0/mkdocs.yml` & `ddqa-0.3.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/pyoxidizer.bzl` & `ddqa-0.3.0/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/.github/workflows/build.yml` & `ddqa-0.3.0/.github/workflows/build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -83,24 +83,28 @@
     outputs:
       version: ${{ steps.version.outputs.version }}
 
     env:
       CARGO: cargo
       CARGO_BUILD_TARGET: ${{ matrix.job.target }}
       PYAPP_REPO: pyapp
-      PYAPP_VERSION: v0.6.0
+      PYAPP_VERSION: "0.7.0"
 
     steps:
     - name: Checkout code
       uses: actions/checkout@v3
       with:
         fetch-depth: 0
 
-    - name: Clone PyApp
-      run: git clone --depth 1 --branch $PYAPP_VERSION https://github.com/ofek/pyapp $PYAPP_REPO
+    - name: Fetch PyApp
+      run: >-
+        mkdir $PYAPP_REPO && curl -L
+        https://github.com/ofek/pyapp/releases/download/v$PYAPP_VERSION/source.tar.gz
+        |
+        tar --strip-components=1 -xzf - -C $PYAPP_REPO
 
     - name: Set up Python ${{ env.PYTHON_VERSION }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ env.PYTHON_VERSION }}
 
     - name: Install Hatch
@@ -185,15 +189,18 @@
       with:
         name: standalone
         path: packaging/*
         if-no-files-found: error
 
   windows-packaging:
     name: Build Windows installers
-    if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
+    if: >-
+      github.event_name == 'push'
+      &&
+      (github.ref == 'refs/heads/master' || startsWith(github.event.ref, 'refs/tags'))
     needs: binaries
     runs-on: windows-2022
 
     env:
       VERSION: ${{ needs.binaries.outputs.version }}
 
     steps:
@@ -255,15 +262,18 @@
       uses: actions/upload-artifact@v3
       with:
         name: installers
         path: installers/*
 
   macos-packaging:
     name: Build macOS installer and sign/notarize artifacts
-    if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
+    if: >-
+      github.event_name == 'push'
+      &&
+      (github.ref == 'refs/heads/master' || startsWith(github.event.ref, 'refs/tags'))
     needs: binaries
     runs-on: macos-12
 
     env:
       VERSION: ${{ needs.binaries.outputs.version }}
 
     steps:
```

### Comparing `ddqa-0.2.0/.github/workflows/docs.yml` & `ddqa-0.3.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/.github/workflows/publish-docs.yml` & `ddqa-0.3.0/.github/workflows/publish-docs.yml`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/.github/workflows/test.yml` & `ddqa-0.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/docs/index.md` & `ddqa-0.3.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/docs/install.md` & `ddqa-0.3.0/docs/install.md`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/docs/assets/css/custom.css` & `ddqa-0.3.0/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/docs/assets/images/favicon.ico` & `ddqa-0.3.0/docs/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/docs/assets/images/logo.svg` & `ddqa-0.3.0/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/docs/config/repo.md` & `ddqa-0.3.0/docs/config/repo.md`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/docs/config/user.md` & `ddqa-0.3.0/docs/config/user.md`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/screenshots/config.PNG` & `ddqa-0.3.0/screenshots/config.PNG`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/app/core.py` & `ddqa-0.3.0/src/ddqa/app/core.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/cli/__init__.py` & `ddqa-0.3.0/src/ddqa/cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,14 +85,18 @@
 
 
 ddqa.add_command(config)
 ddqa.add_command(create)
 ddqa.add_command(status)
 ddqa.add_command(sync)
 
+__management_command = os.environ.get('PYAPP_COMMAND_NAME', '')
+if __management_command:
+    ddqa.add_command(click.Command(name=__management_command, help='Manage this application'))
+
 
 def main():  # no cov
     try:
         return ddqa(prog_name='ddqa', windows_expand_args=False)
     except Exception:
         from rich.console import Console
```

### Comparing `ddqa-0.2.0/src/ddqa/cli/config/__init__.py` & `ddqa-0.3.0/src/ddqa/cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/cli/config/show.py` & `ddqa-0.3.0/src/ddqa/cli/config/show.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/cli/create/__init__.py` & `ddqa-0.3.0/src/ddqa/cli/create/__init__.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/cli/status/__init__.py` & `ddqa-0.3.0/src/ddqa/cli/status/__init__.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/config/core.py` & `ddqa-0.3.0/src/ddqa/config/core.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/config/file.py` & `ddqa-0.3.0/src/ddqa/config/file.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/data/logo.png` & `ddqa-0.3.0/src/ddqa/data/logo.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/data/shame.png` & `ddqa-0.3.0/src/ddqa/data/shame.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/models/github.py` & `ddqa-0.3.0/src/ddqa/models/github.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/models/jira.py` & `ddqa-0.3.0/src/ddqa/models/jira.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/models/config/repo.py` & `ddqa-0.3.0/src/ddqa/models/config/repo.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/screens/configure.py` & `ddqa-0.3.0/src/ddqa/screens/configure.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/screens/create.py` & `ddqa-0.3.0/src/ddqa/screens/create.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/screens/status.py` & `ddqa-0.3.0/src/ddqa/screens/status.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/screens/sync.py` & `ddqa-0.3.0/src/ddqa/screens/sync.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/utils/fs.py` & `ddqa-0.3.0/src/ddqa/utils/fs.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/utils/git.py` & `ddqa-0.3.0/src/ddqa/utils/git.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/utils/github.py` & `ddqa-0.3.0/src/ddqa/utils/github.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/utils/jira.py` & `ddqa-0.3.0/src/ddqa/utils/jira.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/utils/network.py` & `ddqa-0.3.0/src/ddqa/utils/network.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/utils/structures.py` & `ddqa-0.3.0/src/ddqa/utils/structures.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/utils/time.py` & `ddqa-0.3.0/src/ddqa/utils/time.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/widgets/input.py` & `ddqa-0.3.0/src/ddqa/widgets/input.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/widgets/layout.py` & `ddqa-0.3.0/src/ddqa/widgets/layout.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/src/ddqa/widgets/static.py` & `ddqa-0.3.0/src/ddqa/widgets/static.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/tests/conftest.py` & `ddqa-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/tests/cli/config/test_restore.py` & `ddqa-0.3.0/tests/cli/config/test_restore.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/tests/cli/config/test_show.py` & `ddqa-0.3.0/tests/cli/config/test_show.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/tests/cli/create/test_create.py` & `ddqa-0.3.0/tests/cli/create/test_create.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/tests/cli/status/test_status.py` & `ddqa-0.3.0/tests/cli/status/test_status.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/tests/cli/sync/test_sync.py` & `ddqa-0.3.0/tests/cli/sync/test_sync.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/tests/helpers/api.py` & `ddqa-0.3.0/tests/helpers/api.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/tests/screens/test_configure.py` & `ddqa-0.3.0/tests/screens/test_configure.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/tests/screens/test_create.py` & `ddqa-0.3.0/tests/screens/test_create.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/tests/screens/test_sync.py` & `ddqa-0.3.0/tests/screens/test_sync.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/tests/utils/test_fs.py` & `ddqa-0.3.0/tests/utils/test_fs.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/tests/utils/test_git.py` & `ddqa-0.3.0/tests/utils/test_git.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/tests/utils/test_github.py` & `ddqa-0.3.0/tests/utils/test_github.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/tests/utils/test_jira.py` & `ddqa-0.3.0/tests/utils/test_jira.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/tests/utils/test_structures.py` & `ddqa-0.3.0/tests/utils/test_structures.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/tests/utils/test_time.py` & `ddqa-0.3.0/tests/utils/test_time.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/LICENSE.txt` & `ddqa-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/README.md` & `ddqa-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/hatch.toml` & `ddqa-0.3.0/hatch.toml`

 * *Files identical despite different names*

### Comparing `ddqa-0.2.0/pyproject.toml` & `ddqa-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 dependencies = [
   "click>=8.1.3",
   "httpx",
   "pillow",
   "platformdirs",
   "pydantic<2",
   "rich",
-  "textual~=0.19.0",
+  "textual~=0.20.1",
   "textual-autocomplete>=2.1.0b0",
   "tomli-w",
 ]
 
 [project.urls]
 Source = "https://github.com/DataDog/ddqa"
```

### Comparing `ddqa-0.2.0/PKG-INFO` & `ddqa-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddqa
-Version: 0.2.0
+Version: 0.3.0
 Summary: Datadog's QA manager for releases of GitHub repositories
 Project-URL: Source, https://github.com/DataDog/ddqa
 Author-email: "Datadog, Inc." <dev@datadoghq.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: datadog,qa,testing,tooling
 Classifier: Development Status :: 4 - Beta
@@ -16,15 +16,15 @@
 Requires-Dist: click>=8.1.3
 Requires-Dist: httpx
 Requires-Dist: pillow
 Requires-Dist: platformdirs
 Requires-Dist: pydantic<2
 Requires-Dist: rich
 Requires-Dist: textual-autocomplete>=2.1.0b0
-Requires-Dist: textual~=0.19.0
+Requires-Dist: textual~=0.20.1
 Requires-Dist: tomli-w
 Description-Content-Type: text/markdown
 
 # Datadog QA
 
 | | |
 | --- | --- |
```

