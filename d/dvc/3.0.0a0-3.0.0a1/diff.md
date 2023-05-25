# Comparing `tmp/dvc-3.0.0a0.tar.gz` & `tmp/dvc-3.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-3.0.0a0.tar", last modified: Tue May 23 04:11:21 2023, max compression
+gzip compressed data, was "dvc-3.0.0a1.tar", last modified: Thu May 25 10:51:41 2023, max compression
```

## Comparing `dvc-3.0.0a0.tar` & `dvc-3.0.0a1.tar`

### file list

```diff
@@ -1,690 +1,687 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.601779 dvc-3.0.0a0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.525778 dvc-3.0.0a0/.dvc/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.dvc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.dvc/config
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.dvcignore
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.525778 dvc-3.0.0a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.525778 dvc-3.0.0a0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.github/ISSUE_TEMPLATE/epic_story.md
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (122)      395 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.github/mergify.yml
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.525778 dvc-3.0.0a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.github/workflows/benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      701 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3272 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.github/workflows/packages.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.github/workflows/plugin_tests.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      238 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.mailmap
--rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      631 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-23 04:11:03.000000 dvc-3.0.0a0/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (122)     3347 2023-05-23 04:11:03.000000 dvc-3.0.0a0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-05-23 04:11:03.000000 dvc-3.0.0a0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-05-23 04:11:03.000000 dvc-3.0.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    14468 2023-05-23 04:11:21.601779 dvc-3.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13193 2023-05-23 04:11:03.000000 dvc-3.0.0a0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.533778 dvc-3.0.0a0/dvc/
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6574 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/_debug.py
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-05-23 04:11:21.000000 dvc-3.0.0a0/dvc/_dvc_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     4115 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/analytics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.533778 dvc-3.0.0a0/dvc/api/
--rw-r--r--   0 runner    (1001) docker     (122)      530 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9452 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/api/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4974 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/api/experiments.py
--rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/api/scm.py
--rw-r--r--   0 runner    (1001) docker     (122)    11606 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/api/show.py
--rw-r--r--   0 runner    (1001) docker     (122)     2089 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/cachemgr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.533778 dvc-3.0.0a0/dvc/cli/
--rw-r--r--   0 runner    (1001) docker     (122)     7647 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      811 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/cli/completion.py
--rw-r--r--   0 runner    (1001) docker     (122)     4639 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.537778 dvc-3.0.0a0/dvc/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3394 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/add.py
--rw-r--r--   0 runner    (1001) docker     (122)     2876 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3707 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/check_ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)     3062 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/commit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/completion.py
--rw-r--r--   0 runner    (1001) docker     (122)     6939 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/daemon.py
--rw-r--r--   0 runner    (1001) docker     (122)     5427 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/dag.py
--rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    11868 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/data_sync.py
--rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/destroy.py
--rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/diff.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.541778 dvc-3.0.0a0/dvc/commands/experiments/
--rw-r--r--   0 runner    (1001) docker     (122)     2391 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/experiments/apply.py
--rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/experiments/branch.py
--rw-r--r--   0 runner    (1001) docker     (122)      757 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/experiments/clean.py
--rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/experiments/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/experiments/exec_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     1859 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/experiments/ls.py
--rw-r--r--   0 runner    (1001) docker     (122)     3481 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/experiments/pull.py
--rw-r--r--   0 runner    (1001) docker     (122)     5138 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/experiments/push.py
--rw-r--r--   0 runner    (1001) docker     (122)      851 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/experiments/queue_worker.py
--rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/experiments/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     4560 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/experiments/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/experiments/save.py
--rw-r--r--   0 runner    (1001) docker     (122)     9597 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/experiments/show.py
--rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/freeze.py
--rw-r--r--   0 runner    (1001) docker     (122)     6423 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/gc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2911 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/get.py
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     4514 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/git_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     3025 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/imp.py
--rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/imp_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     2926 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/init.py
--rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/install.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.541778 dvc-3.0.0a0/dvc/commands/ls/
--rw-r--r--   0 runner    (1001) docker     (122)     2464 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/ls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1362 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/ls/ls_colors.py
--rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/ls_url.py
--rw-r--r--   0 runner    (1001) docker     (122)    16883 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/machine.py
--rw-r--r--   0 runner    (1001) docker     (122)     7415 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/move.py
--rw-r--r--   0 runner    (1001) docker     (122)     3616 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/params.py
--rw-r--r--   0 runner    (1001) docker     (122)    14462 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.541778 dvc-3.0.0a0/dvc/commands/queue/
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/queue/kill.py
--rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/queue/logs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2793 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/queue/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     1157 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/queue/start.py
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/queue/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/queue/stop.py
--rw-r--r--   0 runner    (1001) docker     (122)     9506 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     5245 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/repro.py
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/root.py
--rw-r--r--   0 runner    (1001) docker     (122)     2973 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (122)    10561 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/stage.py
--rw-r--r--   0 runner    (1001) docker     (122)     2749 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/unprotect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2533 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/update.py
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/commands/version.py
--rw-r--r--   0 runner    (1001) docker     (122)    13223 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/compare.py
--rw-r--r--   0 runner    (1001) docker     (122)    10154 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    10948 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/daemon.py
--rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/dagascii.py
--rw-r--r--   0 runner    (1001) docker     (122)     7287 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/data_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.541778 dvc-3.0.0a0/dvc/dependency/
--rw-r--r--   0 runner    (1001) docker     (122)     2962 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/dependency/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5184 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/dependency/param.py
--rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/dependency/repo.py
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/dirs.py
--rw-r--r--   0 runner    (1001) docker     (122)    12574 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/dvcfile.py
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/env.py
--rw-r--r--   0 runner    (1001) docker     (122)    10279 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.541778 dvc-3.0.0a0/dvc/fs/
--rw-r--r--   0 runner    (1001) docker     (122)     4472 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/fs/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)      899 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/fs/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    13720 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/fs/dvc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/fs/git.py
--rw-r--r--   0 runner    (1001) docker     (122)    14832 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)     4990 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/info.py
--rw-r--r--   0 runner    (1001) docker     (122)     5489 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/lock.py
--rw-r--r--   0 runner    (1001) docker     (122)     7867 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.541778 dvc-3.0.0a0/dvc/machine/
--rw-r--r--   0 runner    (1001) docker     (122)     6843 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.545778 dvc-3.0.0a0/dvc/machine/backend/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/machine/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/machine/backend/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3230 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/machine/backend/terraform.py
--rw-r--r--   0 runner    (1001) docker     (122)    44839 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/output.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.545778 dvc-3.0.0a0/dvc/parsing/
--rw-r--r--   0 runner    (1001) docker     (122)    15488 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16536 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/parsing/context.py
--rw-r--r--   0 runner    (1001) docker     (122)     5953 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/parsing/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (122)     2581 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/pathspec_math.py
--rw-r--r--   0 runner    (1001) docker     (122)     4938 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/progress.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.545778 dvc-3.0.0a0/dvc/render/
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/render/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.545778 dvc-3.0.0a0/dvc/render/converter/
--rw-r--r--   0 runner    (1001) docker     (122)      536 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/render/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/render/converter/image.py
--rw-r--r--   0 runner    (1001) docker     (122)    11094 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/render/converter/vega.py
--rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/render/match.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.549779 dvc-3.0.0a0/dvc/repo/
--rw-r--r--   0 runner    (1001) docker     (122)    18486 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9293 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/add.py
--rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (122)     4620 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/brancher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)     2069 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/collect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/commit.py
--rw-r--r--   0 runner    (1001) docker     (122)     6613 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/data.py
--rw-r--r--   0 runner    (1001) docker     (122)      519 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/destroy.py
--rw-r--r--   0 runner    (1001) docker     (122)     4468 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/diff.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.553779 dvc-3.0.0a0/dvc/repo/experiments/
--rw-r--r--   0 runner    (1001) docker     (122)    16678 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/apply.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/branch.py
--rw-r--r--   0 runner    (1001) docker     (122)     2197 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/clean.py
--rw-r--r--   0 runner    (1001) docker     (122)    11268 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/collect.py
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     3568 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.553779 dvc-3.0.0a0/dvc/repo/experiments/executor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28015 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/executor/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     8313 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/executor/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     9800 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/executor/ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/ls.py
--rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/pull.py
--rw-r--r--   0 runner    (1001) docker     (122)     5404 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/push.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.553779 dvc-3.0.0a0/dvc/repo/experiments/queue/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    27803 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/queue/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    23538 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/queue/celery.py
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/queue/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/queue/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/queue/tasks.py
--rw-r--r--   0 runner    (1001) docker     (122)     7393 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/queue/tempdir.py
--rw-r--r--   0 runner    (1001) docker     (122)     2804 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/queue/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     9540 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/queue/workspace.py
--rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/refs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3899 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     3412 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     1055 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/save.py
--rw-r--r--   0 runner    (1001) docker     (122)     6579 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/serialize.py
--rw-r--r--   0 runner    (1001) docker     (122)    11978 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/show.py
--rw-r--r--   0 runner    (1001) docker     (122)     6776 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/stash.py
--rw-r--r--   0 runner    (1001) docker     (122)    25084 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/experiments/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5357 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/fetch.py
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/freeze.py
--rw-r--r--   0 runner    (1001) docker     (122)     4672 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/gc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/get.py
--rw-r--r--   0 runner    (1001) docker     (122)      546 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     4352 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/graph.py
--rw-r--r--   0 runner    (1001) docker     (122)      233 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/imp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2369 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/imp_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     4121 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/imports.py
--rw-r--r--   0 runner    (1001) docker     (122)    20412 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/index.py
--rw-r--r--   0 runner    (1001) docker     (122)     2826 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/init.py
--rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/install.py
--rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/ls.py
--rw-r--r--   0 runner    (1001) docker     (122)      818 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/ls_url.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.553779 dvc-3.0.0a0/dvc/repo/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/metrics/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     4339 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/metrics/show.py
--rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/move.py
--rw-r--r--   0 runner    (1001) docker     (122)     8225 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/open_repo.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.553779 dvc-3.0.0a0/dvc/repo/params/
--rw-r--r--   0 runner    (1001) docker     (122)      305 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/params/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/params/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     5827 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/params/show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.553779 dvc-3.0.0a0/dvc/repo/plots/
--rw-r--r--   0 runner    (1001) docker     (122)    16703 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      633 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/plots/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1218 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/pull.py
--rw-r--r--   0 runner    (1001) docker     (122)     3514 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/push.py
--rw-r--r--   0 runner    (1001) docker     (122)      913 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     8706 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/reproduce.py
--rw-r--r--   0 runner    (1001) docker     (122)      744 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     4711 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/scm_context.py
--rw-r--r--   0 runner    (1001) docker     (122)    14437 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/stage.py
--rw-r--r--   0 runner    (1001) docker     (122)     3575 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/trie.py
--rw-r--r--   0 runner    (1001) docker     (122)     1847 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/update.py
--rw-r--r--   0 runner    (1001) docker     (122)    14157 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/repo/worktree.py
--rw-r--r--   0 runner    (1001) docker     (122)     6577 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/rwlock.py
--rw-r--r--   0 runner    (1001) docker     (122)     4342 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     7178 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/scm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.557779 dvc-3.0.0a0/dvc/stage/
--rw-r--r--   0 runner    (1001) docker     (122)    25959 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/stage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9042 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/stage/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1641 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/stage/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     2951 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/stage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/stage/imports.py
--rw-r--r--   0 runner    (1001) docker     (122)     7439 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/stage/loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     3489 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/stage/monitor.py
--rw-r--r--   0 runner    (1001) docker     (122)      393 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/stage/params.py
--rw-r--r--   0 runner    (1001) docker     (122)     5034 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/stage/run.py
--rw-r--r--   0 runner    (1001) docker     (122)     7010 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/stage/serialize.py
--rw-r--r--   0 runner    (1001) docker     (122)     8752 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/stage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.557779 dvc-3.0.0a0/dvc/testing/
--rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4088 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/api_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.557779 dvc-3.0.0a0/dvc/testing/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.557779 dvc-3.0.0a0/dvc/testing/benchmarks/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.557779 dvc-3.0.0a0/dvc/testing/benchmarks/cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.561779 dvc-3.0.0a0/dvc/testing/benchmarks/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/commands/test_add.py
--rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/commands/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)     1235 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/commands/test_data_status.py
--rw-r--r--   0 runner    (1001) docker     (122)      350 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/commands/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/commands/test_exp_show.py
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/commands/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/commands/test_get.py
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/commands/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/commands/test_help.py
--rw-r--r--   0 runner    (1001) docker     (122)      270 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/commands/test_import.py
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/commands/test_import_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      383 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/commands/test_init.py
--rw-r--r--   0 runner    (1001) docker     (122)      399 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/commands/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (122)      675 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/commands/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)      188 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/commands/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/commands/test_push.py
--rw-r--r--   0 runner    (1001) docker     (122)      342 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/commands/test_status.py
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/commands/test_update.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.561779 dvc-3.0.0a0/dvc/testing/benchmarks/cli/stories/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/stories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/stories/test_modify_data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.561779 dvc-3.0.0a0/dvc/testing/benchmarks/cli/stories/use_cases/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/stories/use_cases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/cli/stories/use_cases/test_sharing.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     6571 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     2957 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/benchmarks/plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     7316 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)    10376 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/path_info.py
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)    12035 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/remote_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     8948 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/tmp_dir.py
--rw-r--r--   0 runner    (1001) docker     (122)    13091 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/testing/workspace_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.561779 dvc-3.0.0a0/dvc/ui/
--rw-r--r--   0 runner    (1001) docker     (122)    10748 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/ui/_rich_progress.py
--rw-r--r--   0 runner    (1001) docker     (122)     2381 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/ui/pager.py
--rw-r--r--   0 runner    (1001) docker     (122)     3228 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/ui/table.py
--rw-r--r--   0 runner    (1001) docker     (122)     5385 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.565779 dvc-3.0.0a0/dvc/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/utils/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)    12261 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-23 04:11:06.000000 dvc-3.0.0a0/dvc/utils/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/utils/cli_parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     5226 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/utils/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/utils/flatten.py
--rw-r--r--   0 runner    (1001) docker     (122)     2079 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (122)      743 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/utils/humanize.py
--rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/utils/hydra.py
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/utils/objects.py
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/utils/pkg.py
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.565779 dvc-3.0.0a0/dvc/utils/serialize/
--rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/utils/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/utils/serialize/_common.py
--rw-r--r--   0 runner    (1001) docker     (122)      984 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/utils/serialize/_json.py
--rw-r--r--   0 runner    (1001) docker     (122)     5163 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/utils/serialize/_py.py
--rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/utils/serialize/_toml.py
--rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/utils/serialize/_yaml.py
--rw-r--r--   0 runner    (1001) docker     (122)     9779 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/utils/strictyaml.py
--rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/utils/studio.py
--rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/utils/table.py
--rw-r--r--   0 runner    (1001) docker     (122)     2647 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/utils/threadpool.py
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-05-23 04:11:03.000000 dvc-3.0.0a0/dvc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.533778 dvc-3.0.0a0/dvc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14468 2023-05-23 04:11:21.000000 dvc-3.0.0a0/dvc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    17231 2023-05-23 04:11:21.000000 dvc-3.0.0a0/dvc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 04:11:21.000000 dvc-3.0.0a0/dvc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-05-23 04:11:21.000000 dvc-3.0.0a0/dvc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-05-23 04:11:21.000000 dvc-3.0.0a0/dvc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-05-23 04:11:21.000000 dvc-3.0.0a0/dvc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     9367 2023-05-23 04:11:03.000000 dvc-3.0.0a0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.565779 dvc-3.0.0a0/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/build-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2503 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/build.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      231 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/build_package.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.565779 dvc-3.0.0a0/scripts/fpm/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/fpm/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/fpm/after-install.sh
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/fpm/after-remove.sh
--rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/fpm/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/fpm/notarize.py
--rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/fpm/sign.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.565779 dvc-3.0.0a0/scripts/innosetup/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/innosetup/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     2674 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/innosetup/addSymLinkPermissions.ps1
--rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/innosetup/addsymlink.iss
--rw-r--r--   0 runner    (1001) docker     (122)      934 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/innosetup/build.py
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/innosetup/dvc.ico.dvc
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/innosetup/dvc_left.bmp.dvc
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/innosetup/dvc_up.bmp.dvc
--rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/innosetup/modpath.iss
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/innosetup/setup.iss
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.569779 dvc-3.0.0a0/scripts/pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/pyinstaller/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      789 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/pyinstaller/build.py
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/pyinstaller/entitlements.plist
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.569779 dvc-3.0.0a0/scripts/pyinstaller/hooks/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/pyinstaller/hooks/hook-asyncssh.py
--rw-r--r--   0 runner    (1001) docker     (122)      482 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/pyinstaller/hooks/hook-celery.py
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/pyinstaller/hooks/hook-dvc.py
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/pyinstaller/hooks/hook-dvc.system.py
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/pyinstaller/hooks/hook-dvc.tree.gs.py
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/pyinstaller/hooks/hook-dvc.utils.flatten.py
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/pyinstaller/hooks/hook-dvc_task.py
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/pyinstaller/hooks/hook-fsspec.py
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/pyinstaller/hooks/hook-google_compute_engine.logger.py
--rw-r--r--   0 runner    (1001) docker     (122)      116 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/pyinstaller/hooks/hook-pydrive2.py
--rw-r--r--   0 runner    (1001) docker     (122)      958 2023-05-23 04:11:03.000000 dvc-3.0.0a0/scripts/pyinstaller/sign.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 04:11:21.601779 dvc-3.0.0a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.569779 dvc-3.0.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7176 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     3748 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/dir_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.577779 dvc-3.0.0a0/tests/func/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.577779 dvc-3.0.0a0/tests/func/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6885 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/api/test_data.py
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/api/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (122)      719 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/api/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (122)    10796 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/api/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.577779 dvc-3.0.0a0/tests/func/artifacts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/artifacts/test_artifacts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.577779 dvc-3.0.0a0/tests/func/data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.577779 dvc-3.0.0a0/tests/func/data/db/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/data/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3820 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/data/db/test_index.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.581779 dvc-3.0.0a0/tests/func/experiments/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/experiments/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.581779 dvc-3.0.0a0/tests/func/experiments/executor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/experiments/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5129 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/experiments/executor/test_ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     3819 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/experiments/test_apply.py
--rw-r--r--   0 runner    (1001) docker     (122)     8946 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/experiments/test_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (122)      999 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/experiments/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)    26141 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/experiments/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/experiments/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (122)    15984 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/experiments/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     6753 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/experiments/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     4924 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/experiments/test_save.py
--rw-r--r--   0 runner    (1001) docker     (122)     3994 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/experiments/test_set_params.py
--rw-r--r--   0 runner    (1001) docker     (122)    23537 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/experiments/test_show.py
--rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/experiments/test_stash_exp.py
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/experiments/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.581779 dvc-3.0.0a0/tests/func/machine/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/machine/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     5344 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/machine/test_machine_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/machine/test_machine_status.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.581779 dvc-3.0.0a0/tests/func/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7112 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/metrics/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     9489 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/metrics/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.581779 dvc-3.0.0a0/tests/func/params/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/params/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8152 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/params/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     6928 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/params/test_show.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.581779 dvc-3.0.0a0/tests/func/parsing/
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10114 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/parsing/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (122)    15835 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/parsing/test_foreach.py
--rw-r--r--   0 runner    (1001) docker     (122)     9670 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/parsing/test_interpolated_entry.py
--rw-r--r--   0 runner    (1001) docker     (122)     6091 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/parsing/test_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.581779 dvc-3.0.0a0/tests/func/plots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1896 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/plots/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/plots/test_modify.py
--rw-r--r--   0 runner    (1001) docker     (122)    12871 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/plots/test_show.py
--rw-r--r--   0 runner    (1001) docker     (122)    35506 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_add.py
--rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (122)     4281 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_check_ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)    26547 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)     4928 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     8797 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_commit.py
--rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    16832 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_data_cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)    16348 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_data_status.py
--rw-r--r--   0 runner    (1001) docker     (122)    18824 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)    12248 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_dvcfile.py
--rw-r--r--   0 runner    (1001) docker     (122)     7554 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_external_repo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1412 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (122)    14728 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (122)    11136 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_get.py
--rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)    14876 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)    20849 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_import.py
--rw-r--r--   0 runner    (1001) docker     (122)     7625 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_import_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     3215 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_init.py
--rw-r--r--   0 runner    (1001) docker     (122)     5558 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_install.py
--rw-r--r--   0 runner    (1001) docker     (122)     1740 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (122)     5057 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_lockfile.py
--rw-r--r--   0 runner    (1001) docker     (122)    17854 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_ls_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     5573 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_merge_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)     5734 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_move.py
--rw-r--r--   0 runner    (1001) docker     (122)     5936 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_odb.py
--rw-r--r--   0 runner    (1001) docker     (122)    15547 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     3465 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_repo.py
--rw-r--r--   0 runner    (1001) docker     (122)    10062 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_repo_index.py
--rw-r--r--   0 runner    (1001) docker     (122)    34572 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_repro.py
--rw-r--r--   0 runner    (1001) docker     (122)    13663 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_repro_multistage.py
--rw-r--r--   0 runner    (1001) docker     (122)      340 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_root.py
--rw-r--r--   0 runner    (1001) docker     (122)     6037 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_run_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)    11484 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_run_multistage.py
--rw-r--r--   0 runner    (1001) docker     (122)    24708 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_run_single_stage.py
--rw-r--r--   0 runner    (1001) docker     (122)      639 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (122)     1839 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_scm_context.py
--rw-r--r--   0 runner    (1001) docker     (122)    10257 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_stage.py
--rw-r--r--   0 runner    (1001) docker     (122)    14749 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_stage_load.py
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     5156 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_status.py
--rw-r--r--   0 runner    (1001) docker     (122)      830 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_unprotect.py
--rw-r--r--   0 runner    (1001) docker     (122)    14335 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_update.py
--rw-r--r--   0 runner    (1001) docker     (122)     1951 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_used_objs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     5562 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/test_virtual_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.581779 dvc-3.0.0a0/tests/func/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8318 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/utils/test_hydra.py
--rw-r--r--   0 runner    (1001) docker     (122)     9702 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/func/utils/test_strict_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.581779 dvc-3.0.0a0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      118 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/integration/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.585779 dvc-3.0.0a0/tests/integration/plots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/integration/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5922 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/integration/plots/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    13779 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/integration/plots/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)     3978 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/integration/plots/test_repo_plots_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     3253 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/integration/test_studio_live_experiments.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.585779 dvc-3.0.0a0/tests/remotes/
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/remotes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.585779 dvc-3.0.0a0/tests/remotes/git-init/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/remotes/git-init/git.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/remotes/git_server.py
--rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/remotes/user.key
--rw-r--r--   0 runner    (1001) docker     (122)      394 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/remotes/user.key.pub
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/remotes_env.sample
--rw-r--r--   0 runner    (1001) docker     (122)      118 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.585779 dvc-3.0.0a0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.589779 dvc-3.0.0a0/tests/unit/cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/cli/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.589779 dvc-3.0.0a0/tests/unit/command/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.593779 dvc-3.0.0a0/tests/unit/command/ls/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/ls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3087 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/ls/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/ls/test_ls_colors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2687 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_add.py
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (122)      610 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_compat_flag.py
--rw-r--r--   0 runner    (1001) docker     (122)      883 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     7404 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_data_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     2800 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_data_sync.py
--rw-r--r--   0 runner    (1001) docker     (122)    11210 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)    10398 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_experiments.py
--rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_get.py
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_get_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      563 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_git_hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     2028 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_imp.py
--rw-r--r--   0 runner    (1001) docker     (122)     4010 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_imp_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      656 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_ls_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     4858 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_machine.py
--rw-r--r--   0 runner    (1001) docker     (122)     4212 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_params.py
--rw-r--r--   0 runner    (1001) docker     (122)    11193 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)     6178 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_repro.py
--rw-r--r--   0 runner    (1001) docker     (122)     3738 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     2800 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_stage.py
--rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/command/test_update.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.593779 dvc-3.0.0a0/tests/unit/data/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.593779 dvc-3.0.0a0/tests/unit/data/db/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/data/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3994 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/data/db/test_local.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.593779 dvc-3.0.0a0/tests/unit/dependency/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/dependency/test_dependency.py
--rw-r--r--   0 runner    (1001) docker     (122)     8862 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/dependency/test_params.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.593779 dvc-3.0.0a0/tests/unit/fs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2482 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/fs/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/fs/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7529 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/fs/test_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    19085 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/fs/test_dvc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3638 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/fs/test_dvc_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     2108 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/fs/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/fs/test_path.py
--rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/fs/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1373 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/fs/test_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.593779 dvc-3.0.0a0/tests/unit/machine/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/machine/test_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.593779 dvc-3.0.0a0/tests/unit/output/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      360 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/output/test_annotations.py
--rw-r--r--   0 runner    (1001) docker     (122)     4098 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/output/test_load.py
--rw-r--r--   0 runner    (1001) docker     (122)     1903 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/output/test_local.py
--rw-r--r--   0 runner    (1001) docker     (122)     6664 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/output/test_output.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.593779 dvc-3.0.0a0/tests/unit/remote/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      573 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/remote/test_oss.py
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/remote/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     4407 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/remote/test_webdav.py
--rw-r--r--   0 runner    (1001) docker     (122)     1587 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/remote/test_webhdfs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.597779 dvc-3.0.0a0/tests/unit/render/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3196 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/render/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/render/test_image_converter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4240 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/render/test_match.py
--rw-r--r--   0 runner    (1001) docker     (122)    14720 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/render/test_vega_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.597779 dvc-3.0.0a0/tests/unit/repo/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/repo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.597779 dvc-3.0.0a0/tests/unit/repo/experiments/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/repo/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6140 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/repo/experiments/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.597779 dvc-3.0.0a0/tests/unit/repo/experiments/queue/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/repo/experiments/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/repo/experiments/queue/test_celery.py
--rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/repo/experiments/queue/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     4239 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/repo/experiments/test_executor_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     1563 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/repo/experiments/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/repo/experiments/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.597779 dvc-3.0.0a0/tests/unit/repo/plots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/repo/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1450 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/repo/plots/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     2957 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/repo/test_open_repo.py
--rw-r--r--   0 runner    (1001) docker     (122)     3661 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/repo/test_repo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1749 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/repo/test_reproduce.py
--rw-r--r--   0 runner    (1001) docker     (122)      335 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/repo/test_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/repo/test_scm_context.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.597779 dvc-3.0.0a0/tests/unit/scm/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/scm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/scm/test_scm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.597779 dvc-3.0.0a0/tests/unit/stage/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/stage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5924 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/stage/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     8626 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/stage/test_loader_pipeline_file.py
--rw-r--r--   0 runner    (1001) docker     (122)      578 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/stage/test_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     6087 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/stage/test_serialize_pipeline_file.py
--rw-r--r--   0 runner    (1001) docker     (122)     8394 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/stage/test_serialize_pipeline_lock.py
--rw-r--r--   0 runner    (1001) docker     (122)     4318 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/stage/test_stage.py
--rw-r--r--   0 runner    (1001) docker     (122)      687 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/stage/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4263 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_analytics.py
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (122)    13495 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (122)     3118 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    12356 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_context.py
--rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_daemon.py
--rw-r--r--   0 runner    (1001) docker     (122)     3971 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_dvcfile.py
--rw-r--r--   0 runner    (1001) docker     (122)      457 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_hashinfo.py
--rw-r--r--   0 runner    (1001) docker     (122)     8869 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_ignore.py
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (122)     4352 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     3045 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (122)     3447 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_lockfile.py
--rw-r--r--   0 runner    (1001) docker     (122)     8687 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1240 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     3747 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_pathspec_math.py
--rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     4282 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_rwlock.py
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (122)     9682 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_tabular_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     5357 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/test_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.597779 dvc-3.0.0a0/tests/unit/ui/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1558 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/ui/test_console.py
--rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/ui/test_pager.py
--rw-r--r--   0 runner    (1001) docker     (122)     4393 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/ui/test_table.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.601779 dvc-3.0.0a0/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.601779 dvc-3.0.0a0/tests/unit/utils/serialize/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/utils/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/utils/serialize/test_python.py
--rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/utils/serialize/test_toml.py
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/utils/serialize/test_yaml.py
--rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/utils/test_cli_parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     5635 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/utils/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (122)     2546 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/utils/test_executors.py
--rw-r--r--   0 runner    (1001) docker     (122)     4640 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/utils/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2050 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/utils/test_humanize.py
--rw-r--r--   0 runner    (1001) docker     (122)     1758 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/utils/test_studio.py
--rw-r--r--   0 runner    (1001) docker     (122)     5103 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/unit/utils/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 04:11:21.601779 dvc-3.0.0a0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     1633 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      593 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/utils/asserts.py
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-23 04:11:03.000000 dvc-3.0.0a0/tests/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.021571 dvc-3.0.0a1/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.877570 dvc-3.0.0a1/.dvc/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.dvc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.dvc/config
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.dvcignore
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.881569 dvc-3.0.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.881569 dvc-3.0.0a1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/ISSUE_TEMPLATE/epic_story.md
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (122)      395 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/mergify.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.881569 dvc-3.0.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/workflows/benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3272 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/workflows/packages.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/workflows/plugin_tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      238 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      631 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-25 10:51:20.000000 dvc-3.0.0a1/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3347 2023-05-25 10:51:20.000000 dvc-3.0.0a1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-05-25 10:51:20.000000 dvc-3.0.0a1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-05-25 10:51:20.000000 dvc-3.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    14468 2023-05-25 10:51:41.021571 dvc-3.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13193 2023-05-25 10:51:20.000000 dvc-3.0.0a1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.889570 dvc-3.0.0a1/dvc/
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6574 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-05-25 10:51:40.000000 dvc-3.0.0a1/dvc/_dvc_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4115 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.889570 dvc-3.0.0a1/dvc/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      490 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9452 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/api/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3994 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/api/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/api/scm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11606 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/api/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2089 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/cachemgr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.889570 dvc-3.0.0a1/dvc/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     7647 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      811 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/cli/completion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.897570 dvc-3.0.0a1/dvc/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3394 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/add.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2876 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3707 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/check_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3062 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/commit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/completion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6939 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2070 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5427 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/dag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6292 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11868 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/data_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1514 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/diff.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.901570 dvc-3.0.0a1/dvc/commands/experiments/
+-rw-r--r--   0 runner    (1001) docker     (122)     2391 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/clean.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/exec_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2578 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3481 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5138 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/push.py
+-rw-r--r--   0 runner    (1001) docker     (122)      851 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/queue_worker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2365 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3373 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/save.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9492 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/experiments/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1778 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/freeze.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6423 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2911 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/get.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4514 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/git_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3025 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/imp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/imp_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2926 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/install.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.901570 dvc-3.0.0a1/dvc/commands/ls/
+-rw-r--r--   0 runner    (1001) docker     (122)     2464 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/ls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1362 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/ls/ls_colors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/ls_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16883 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/machine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7415 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/move.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3616 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14462 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.901570 dvc-3.0.0a1/dvc/commands/queue/
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/queue/kill.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/queue/logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2793 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/queue/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1157 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/queue/start.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/queue/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/queue/stop.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9506 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5245 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/repro.py
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/root.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10238 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2749 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/unprotect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2533 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/commands/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13223 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/compare.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10154 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10948 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/dagascii.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7287 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/data_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.905570 dvc-3.0.0a1/dvc/dependency/
+-rw-r--r--   0 runner    (1001) docker     (122)     2962 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/dependency/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5184 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/dependency/param.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/dependency/repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/dirs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12574 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/dvcfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)      673 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/env.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10279 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.905570 dvc-3.0.0a1/dvc/fs/
+-rw-r--r--   0 runner    (1001) docker     (122)     4472 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/fs/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)      899 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/fs/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13720 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/fs/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/fs/git.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14832 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4990 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5489 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7867 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.905570 dvc-3.0.0a1/dvc/machine/
+-rw-r--r--   0 runner    (1001) docker     (122)     6843 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.905570 dvc-3.0.0a1/dvc/machine/backend/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/machine/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/machine/backend/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3230 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/machine/backend/terraform.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44224 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/output.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.905570 dvc-3.0.0a1/dvc/parsing/
+-rw-r--r--   0 runner    (1001) docker     (122)    15488 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16536 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/parsing/context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5953 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/parsing/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2581 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/pathspec_math.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4938 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.905570 dvc-3.0.0a1/dvc/render/
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/render/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.909570 dvc-3.0.0a1/dvc/render/converter/
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/render/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/render/converter/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11094 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/render/converter/vega.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/render/match.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.913570 dvc-3.0.0a1/dvc/repo/
+-rw-r--r--   0 runner    (1001) docker     (122)    18486 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9293 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/add.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4620 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/brancher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2069 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/collect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/commit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6613 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4468 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/diff.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.917570 dvc-3.0.0a1/dvc/repo/experiments/
+-rw-r--r--   0 runner    (1001) docker     (122)    13047 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1329 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/brancher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2197 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/clean.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11268 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/collect.py
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.921570 dvc-3.0.0a1/dvc/repo/experiments/executor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25405 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/executor/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7923 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/executor/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9696 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/executor/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5404 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/push.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.921570 dvc-3.0.0a1/dvc/repo/experiments/queue/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24548 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/queue/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23073 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/queue/celery.py
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/queue/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/queue/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/queue/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6834 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/queue/tempdir.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/queue/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8879 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/queue/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/refs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3899 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3330 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1055 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/save.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6331 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11978 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6759 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/stash.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24913 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/experiments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5357 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/freeze.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4672 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/get.py
+-rw-r--r--   0 runner    (1001) docker     (122)      546 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4352 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)      233 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/imp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2369 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/imp_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4121 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20412 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/index.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2826 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2559 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/install.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2285 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      818 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/ls_url.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.921570 dvc-3.0.0a1/dvc/repo/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/metrics/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4339 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/metrics/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/move.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8225 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/open_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.921570 dvc-3.0.0a1/dvc/repo/params/
+-rw-r--r--   0 runner    (1001) docker     (122)      305 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/params/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5827 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/params/show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.921570 dvc-3.0.0a1/dvc/repo/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)    17028 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      633 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/plots/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1218 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3514 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/push.py
+-rw-r--r--   0 runner    (1001) docker     (122)      913 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7288 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/reproduce.py
+-rw-r--r--   0 runner    (1001) docker     (122)      744 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4711 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/scm_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14437 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3575 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/trie.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1847 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14157 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/repo/worktree.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6577 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/rwlock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4303 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7178 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/scm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.925570 dvc-3.0.0a1/dvc/stage/
+-rw-r--r--   0 runner    (1001) docker     (122)    24877 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/stage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9042 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/stage/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1641 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/stage/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/stage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/stage/imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7439 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/stage/loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      393 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/stage/params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4096 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/stage/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6907 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/stage/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8604 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/stage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.925570 dvc-3.0.0a1/dvc/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4088 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/api_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.929570 dvc-3.0.0a1/dvc/testing/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.929570 dvc-3.0.0a1/dvc/testing/benchmarks/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.929570 dvc-3.0.0a1/dvc/testing/benchmarks/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.933570 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1235 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_data_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      350 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_exp_show.py
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (122)      270 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_import_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      675 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)      188 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_push.py
+-rw-r--r--   0 runner    (1001) docker     (122)      342 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.933570 dvc-3.0.0a1/dvc/testing/benchmarks/cli/stories/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/stories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/stories/test_modify_data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.933570 dvc-3.0.0a1/dvc/testing/benchmarks/cli/stories/use_cases/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/stories/use_cases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/cli/stories/use_cases/test_sharing.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6571 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2957 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/benchmarks/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7316 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10376 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/path_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12035 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/remote_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8948 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/tmp_dir.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13091 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/testing/workspace_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.933570 dvc-3.0.0a1/dvc/ui/
+-rw-r--r--   0 runner    (1001) docker     (122)    10748 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/ui/_rich_progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2381 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/ui/pager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3228 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/ui/table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5385 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.937570 dvc-3.0.0a1/dvc/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)    12261 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-25 10:51:24.000000 dvc-3.0.0a1/dvc/utils/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1295 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/cli_parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5226 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2079 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      743 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/humanize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/hydra.py
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/pkg.py
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.937570 dvc-3.0.0a1/dvc/utils/serialize/
+-rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/serialize/_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      984 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/serialize/_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5163 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/serialize/_py.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/serialize/_toml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/serialize/_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9779 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/strictyaml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/studio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2647 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/utils/threadpool.py
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2023-05-25 10:51:20.000000 dvc-3.0.0a1/dvc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.889570 dvc-3.0.0a1/dvc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14468 2023-05-25 10:51:40.000000 dvc-3.0.0a1/dvc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    17149 2023-05-25 10:51:40.000000 dvc-3.0.0a1/dvc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 10:51:40.000000 dvc-3.0.0a1/dvc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-05-25 10:51:40.000000 dvc-3.0.0a1/dvc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-05-25 10:51:40.000000 dvc-3.0.0a1/dvc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-05-25 10:51:40.000000 dvc-3.0.0a1/dvc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     9367 2023-05-25 10:51:20.000000 dvc-3.0.0a1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.937570 dvc-3.0.0a1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/build-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2503 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/build.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      231 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/build_package.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.941570 dvc-3.0.0a1/scripts/fpm/
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/fpm/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/fpm/after-install.sh
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/fpm/after-remove.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/fpm/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/fpm/notarize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/fpm/sign.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.941570 dvc-3.0.0a1/scripts/innosetup/
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/innosetup/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     2674 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/innosetup/addSymLinkPermissions.ps1
+-rw-r--r--   0 runner    (1001) docker     (122)     1153 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/innosetup/addsymlink.iss
+-rw-r--r--   0 runner    (1001) docker     (122)      934 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/innosetup/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/innosetup/dvc.ico.dvc
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/innosetup/dvc_left.bmp.dvc
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/innosetup/dvc_up.bmp.dvc
+-rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/innosetup/modpath.iss
+-rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/innosetup/setup.iss
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.941570 dvc-3.0.0a1/scripts/pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      789 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/entitlements.plist
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.945570 dvc-3.0.0a1/scripts/pyinstaller/hooks/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/hooks/hook-asyncssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)      482 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/hooks/hook-celery.py
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/hooks/hook-dvc.py
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/hooks/hook-dvc.system.py
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/hooks/hook-dvc.tree.gs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/hooks/hook-dvc.utils.flatten.py
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/hooks/hook-dvc_task.py
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/hooks/hook-fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/hooks/hook-google_compute_engine.logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/hooks/hook-pydrive2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      958 2023-05-25 10:51:20.000000 dvc-3.0.0a1/scripts/pyinstaller/sign.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-25 10:51:41.021571 dvc-3.0.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.945570 dvc-3.0.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7176 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3748 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/dir_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.957570 dvc-3.0.0a1/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.957570 dvc-3.0.0a1/tests/func/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6885 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/api/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/api/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/api/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10796 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/api/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.957570 dvc-3.0.0a1/tests/func/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/artifacts/test_artifacts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.957570 dvc-3.0.0a1/tests/func/data/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.957570 dvc-3.0.0a1/tests/func/data/db/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/data/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3820 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/data/db/test_index.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.961570 dvc-3.0.0a1/tests/func/experiments/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.961570 dvc-3.0.0a1/tests/func/experiments/executor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5129 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/executor/test_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3819 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/test_apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)      999 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26233 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13387 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6753 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4928 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3970 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/test_set_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22437 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/test_show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/test_stash_exp.py
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/experiments/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.961570 dvc-3.0.0a1/tests/func/machine/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/machine/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5344 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/machine/test_machine_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/machine/test_machine_status.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.961570 dvc-3.0.0a1/tests/func/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7112 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/metrics/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9489 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/metrics/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.965570 dvc-3.0.0a1/tests/func/params/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8152 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/params/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6928 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/params/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.965570 dvc-3.0.0a1/tests/func/parsing/
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10114 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/parsing/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15835 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/parsing/test_foreach.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9670 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/parsing/test_interpolated_entry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6091 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/parsing/test_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.965570 dvc-3.0.0a1/tests/func/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1896 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/plots/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/plots/test_modify.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12871 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/plots/test_show.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35171 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4281 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_check_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26547 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3924 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8797 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_commit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16745 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_data_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16348 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_data_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18824 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12248 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_dvcfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7554 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_external_repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1412 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14728 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11136 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14876 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20849 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7625 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_import_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3215 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5558 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_install.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1740 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5057 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_lockfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17854 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_ls_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5573 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_merge_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5734 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_move.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5936 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_odb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15547 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3465 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10062 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_repo_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34947 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_repro.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13819 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_repro_multistage.py
+-rw-r--r--   0 runner    (1001) docker     (122)      340 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_root.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6037 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_run_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11484 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_run_multistage.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16626 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_run_single_stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)      639 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1839 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_scm_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9662 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14749 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_stage_load.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5156 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_unprotect.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14335 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1951 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_used_objs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5562 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/test_virtual_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.965570 dvc-3.0.0a1/tests/func/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8318 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/utils/test_hydra.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9702 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/func/utils/test_strict_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.965570 dvc-3.0.0a1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/integration/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.969570 dvc-3.0.0a1/tests/integration/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/integration/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5922 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/integration/plots/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13779 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/integration/plots/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3978 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/integration/plots/test_repo_plots_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3253 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/integration/test_studio_live_experiments.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.969570 dvc-3.0.0a1/tests/remotes/
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/remotes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.969570 dvc-3.0.0a1/tests/remotes/git-init/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/remotes/git-init/git.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/remotes/git_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1679 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/remotes/user.key
+-rw-r--r--   0 runner    (1001) docker     (122)      394 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/remotes/user.key.pub
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/remotes_env.sample
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.977570 dvc-3.0.0a1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.981570 dvc-3.0.0a1/tests/unit/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/cli/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.985571 dvc-3.0.0a1/tests/unit/command/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.985571 dvc-3.0.0a1/tests/unit/command/ls/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/ls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3087 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/ls/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/ls/test_ls_colors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2687 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_compat_flag.py
+-rw-r--r--   0 runner    (1001) docker     (122)      883 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7404 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_data_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2800 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_data_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11210 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11627 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_get_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      563 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_git_hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2028 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_imp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4010 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_imp_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      656 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_ls_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4858 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_machine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4212 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11193 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6178 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_repro.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2707 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/command/test_update.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.985571 dvc-3.0.0a1/tests/unit/data/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.989570 dvc-3.0.0a1/tests/unit/data/db/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/data/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3994 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/data/db/test_local.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.989570 dvc-3.0.0a1/tests/unit/dependency/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/dependency/test_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8862 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/dependency/test_params.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.993570 dvc-3.0.0a1/tests/unit/fs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2482 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/fs/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/fs/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7529 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/fs/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19085 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/fs/test_dvc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3638 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/fs/test_dvc_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2108 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/fs/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/fs/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/fs/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1373 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/fs/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.997571 dvc-3.0.0a1/tests/unit/machine/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/machine/test_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:40.997571 dvc-3.0.0a1/tests/unit/output/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/output/test_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4098 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/output/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1903 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/output/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6664 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/output/test_output.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.001571 dvc-3.0.0a1/tests/unit/remote/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/remote/test_oss.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/remote/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4407 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/remote/test_webdav.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1587 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/remote/test_webhdfs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.001571 dvc-3.0.0a1/tests/unit/render/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3196 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/render/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/render/test_image_converter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4240 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/render/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14720 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/render/test_vega_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.005571 dvc-3.0.0a1/tests/unit/repo/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.005571 dvc-3.0.0a1/tests/unit/repo/experiments/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3673 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/experiments/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.005571 dvc-3.0.0a1/tests/unit/repo/experiments/queue/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/experiments/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/experiments/queue/test_celery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3951 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/experiments/queue/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4239 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/experiments/test_executor_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1563 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/experiments/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/experiments/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.005571 dvc-3.0.0a1/tests/unit/repo/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1450 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/plots/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2957 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/test_open_repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3661 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/test_repo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1749 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/test_reproduce.py
+-rw-r--r--   0 runner    (1001) docker     (122)      335 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4396 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/repo/test_scm_context.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.009571 dvc-3.0.0a1/tests/unit/scm/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/scm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/scm/test_scm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.009571 dvc-3.0.0a1/tests/unit/stage/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/stage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5924 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/stage/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8626 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/stage/test_loader_pipeline_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      578 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/stage/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6087 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/stage/test_serialize_pipeline_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8394 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/stage/test_serialize_pipeline_lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3710 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/stage/test_stage.py
+-rw-r--r--   0 runner    (1001) docker     (122)      687 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/stage/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4263 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13495 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3118 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12356 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3971 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_dvcfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)      457 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_hashinfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8869 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4352 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3045 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3447 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_lockfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8687 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1240 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3747 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_pathspec_math.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4282 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_rwlock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9682 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_tabular_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5357 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.013571 dvc-3.0.0a1/tests/unit/ui/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1558 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/ui/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2697 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/ui/test_pager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4393 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/ui/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.017571 dvc-3.0.0a1/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.021571 dvc-3.0.0a1/tests/unit/utils/serialize/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/serialize/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/serialize/test_toml.py
+-rw-r--r--   0 runner    (1001) docker     (122)      629 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/serialize/test_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/test_cli_parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5635 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2546 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/test_executors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4640 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2050 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/test_humanize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1758 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/test_studio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5103 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/unit/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:51:41.021571 dvc-3.0.0a1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     1633 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      593 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/utils/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-25 10:51:20.000000 dvc-3.0.0a1/tests/utils/plots.py
```

### Comparing `dvc-3.0.0a0/.git-blame-ignore-revs` & `dvc-3.0.0a1/.git-blame-ignore-revs`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/.github/ISSUE_TEMPLATE/bug_report.md` & `dvc-3.0.0a1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/.github/ISSUE_TEMPLATE/epic_story.md` & `dvc-3.0.0a1/.github/ISSUE_TEMPLATE/epic_story.md`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/.github/workflows/codeql.yml` & `dvc-3.0.0a1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/.github/workflows/packages.yaml` & `dvc-3.0.0a1/.github/workflows/packages.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/.github/workflows/plugin_tests.yaml` & `dvc-3.0.0a1/.github/workflows/plugin_tests.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/.github/workflows/tests.yaml` & `dvc-3.0.0a1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/.pre-commit-config.yaml` & `dvc-3.0.0a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/.pre-commit-hooks.yaml` & `dvc-3.0.0a1/.pre-commit-hooks.yaml`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/CODE_OF_CONDUCT.md` & `dvc-3.0.0a1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/LICENSE` & `dvc-3.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/PKG-INFO` & `dvc-3.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc
-Version: 3.0.0a0
+Version: 3.0.0a1
 Summary: Git for data scientists - manage your code and data together
 Author-email: Dmitry Petrov <dmitry@dvc.org>
 Maintainer-email: Iterative <support@dvc.org>
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Issues, https://github.com/iterative/dvc/issues
 Project-URL: Source, https://github.com/iterative/dvc
```

### Comparing `dvc-3.0.0a0/README.rst` & `dvc-3.0.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/_debug.py` & `dvc-3.0.0a1/dvc/_debug.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/analytics.py` & `dvc-3.0.0a1/dvc/analytics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/annotations.py` & `dvc-3.0.0a1/dvc/annotations.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/api/data.py` & `dvc-3.0.0a1/dvc/api/data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/api/experiments.py` & `dvc-3.0.0a1/dvc/api/experiments.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,13 @@
-import builtins
-import os
-from time import sleep
 from typing import Dict, List, Optional, Union
 
 from rich.text import Text
 
-from dvc.env import DVC_CHECKPOINT, DVC_ROOT
 from dvc.repo import Repo
 from dvc.repo.experiments.show import tabulate
-from dvc.stage.monitor import CheckpointTask
-
-
-def make_checkpoint():
-    """
-    Signal DVC to create a checkpoint experiment.
-
-    If the current process is being run from DVC, this function will block
-    until DVC has finished creating the checkpoint. Otherwise, this function
-    will return immediately.
-    """
-    if os.getenv(DVC_CHECKPOINT) is None:
-        return
-
-    root_dir = os.getenv(DVC_ROOT, Repo.find_root())
-    signal_file = os.path.join(
-        root_dir, Repo.DVC_DIR, "tmp", CheckpointTask.SIGNAL_FILE
-    )
-
-    with builtins.open(signal_file, "w", encoding="utf-8") as fobj:
-        # NOTE: force flushing/writing empty file to disk, otherwise when
-        # run in certain contexts (pytest) file may not actually be written
-        fobj.write("")
-        fobj.flush()
-        os.fsync(fobj.fileno())
-    while os.path.exists(signal_file):
-        sleep(0.1)
 
 
 def exp_save(
     name: Optional[str] = None,
     force: bool = False,
     include_untracked: Optional[List[str]] = None,
 ):
```

### Comparing `dvc-3.0.0a0/dvc/api/scm.py` & `dvc-3.0.0a1/dvc/api/scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/api/show.py` & `dvc-3.0.0a1/dvc/api/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/cachemgr.py` & `dvc-3.0.0a1/dvc/cachemgr.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/cli/__init__.py` & `dvc-3.0.0a1/dvc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/cli/command.py` & `dvc-3.0.0a1/dvc/cli/command.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/cli/completion.py` & `dvc-3.0.0a1/dvc/cli/completion.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/cli/parser.py` & `dvc-3.0.0a1/dvc/cli/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     params,
     plots,
     queue,
     remote,
     remove,
     repro,
     root,
-    run,
     stage,
     unprotect,
     update,
     version,
 )
 
 from . import DvcParserError
@@ -58,15 +57,14 @@
     get,
     get_url,
     destroy,
     add,
     remove,
     move,
     unprotect,
-    run,
     repro,
     data_sync,
     gc,
     imp,
     imp_url,
     config,
     checkout,
```

### Comparing `dvc-3.0.0a0/dvc/cli/utils.py` & `dvc-3.0.0a1/dvc/cli/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/add.py` & `dvc-3.0.0a1/dvc/commands/add.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/cache.py` & `dvc-3.0.0a1/dvc/commands/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/check_ignore.py` & `dvc-3.0.0a1/dvc/commands/check_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/checkout.py` & `dvc-3.0.0a1/dvc/commands/checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/commit.py` & `dvc-3.0.0a1/dvc/commands/commit.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/completion.py` & `dvc-3.0.0a1/dvc/commands/completion.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/config.py` & `dvc-3.0.0a1/dvc/commands/config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/daemon.py` & `dvc-3.0.0a1/dvc/commands/daemon.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/dag.py` & `dvc-3.0.0a1/dvc/commands/dag.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/data.py` & `dvc-3.0.0a1/dvc/commands/data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/data_sync.py` & `dvc-3.0.0a1/dvc/commands/data_sync.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/destroy.py` & `dvc-3.0.0a1/dvc/commands/destroy.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/diff.py` & `dvc-3.0.0a1/dvc/commands/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/experiments/__init__.py` & `dvc-3.0.0a1/dvc/commands/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/experiments/apply.py` & `dvc-3.0.0a1/dvc/commands/experiments/apply.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/experiments/branch.py` & `dvc-3.0.0a1/dvc/commands/experiments/branch.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/experiments/clean.py` & `dvc-3.0.0a1/dvc/commands/experiments/clean.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/experiments/diff.py` & `dvc-3.0.0a1/dvc/commands/experiments/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/experiments/exec_run.py` & `dvc-3.0.0a1/dvc/commands/experiments/exec_run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/experiments/ls.py` & `dvc-3.0.0a1/dvc/commands/experiments/remove.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,75 @@
 import argparse
 import logging
 
 from dvc.cli.command import CmdBase
 from dvc.cli.utils import append_doc_link
+from dvc.exceptions import InvalidArgumentError
 from dvc.ui import ui
 
 logger = logging.getLogger(__name__)
 
 
-class CmdExperimentsList(CmdBase):
+class CmdExperimentsRemove(CmdBase):
+    def check_arguments(self):
+        if not any(
+            [
+                self.args.all_commits,
+                self.args.rev,
+                self.args.queue,
+            ]
+        ) ^ bool(self.args.experiment):
+            raise InvalidArgumentError(
+                "Either provide an `experiment` argument, or use the "
+                "`--rev` or `--all-commits` or `--queue` flag."
+            )
+
     def run(self):
-        name_only = self.args.name_only
-        exps = self.repo.experiments.ls(
+        from dvc.utils import humanize
+
+        self.check_arguments()
+
+        removed = self.repo.experiments.remove(
+            exp_names=self.args.experiment,
             all_commits=self.args.all_commits,
             rev=self.args.rev,
             num=self.args.num,
+            queue=self.args.queue,
             git_remote=self.args.git_remote,
         )
-
-        for baseline in exps:
-            if not name_only:
-                ui.write(f"{baseline}:")
-            for exp_name in exps[baseline]:
-                indent = "" if name_only else "\t"
-                ui.write(f"{indent}{exp_name}")
+        if removed:
+            ui.write(f"Removed experiments: {humanize.join(map(repr, removed))}")
+        else:
+            ui.write("No experiments to remove.")
 
         return 0
 
 
 def add_parser(experiments_subparsers, parent_parser):
     from . import add_rev_selection_flags
 
-    EXPERIMENTS_LIST_HELP = "List local and remote experiments."
-    experiments_list_parser = experiments_subparsers.add_parser(
-        "list",
+    EXPERIMENTS_REMOVE_HELP = "Remove experiments."
+    experiments_remove_parser = experiments_subparsers.add_parser(
+        "remove",
         parents=[parent_parser],
-        description=append_doc_link(EXPERIMENTS_LIST_HELP, "exp/list"),
-        help=EXPERIMENTS_LIST_HELP,
+        description=append_doc_link(EXPERIMENTS_REMOVE_HELP, "exp/remove"),
+        help=EXPERIMENTS_REMOVE_HELP,
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
-    add_rev_selection_flags(experiments_list_parser, "List")
-    experiments_list_parser.add_argument(
-        "--name-only",
-        "--names-only",
-        action="store_true",
-        help="Only output experiment names (without parent commits).",
+    remove_group = experiments_remove_parser.add_mutually_exclusive_group()
+    add_rev_selection_flags(experiments_remove_parser, "Remove", False)
+    remove_group.add_argument(
+        "--queue", action="store_true", help="Remove all queued experiments."
     )
-    experiments_list_parser.add_argument(
-        "git_remote",
-        nargs="?",
-        default=None,
-        help=(
-            "Optional Git remote name or Git URL. "
-            "If provided, experiments from the specified Git repository "
-            " will be listed instead of local ones."
-        ),
+    remove_group.add_argument(
+        "-g",
+        "--git-remote",
         metavar="<git_remote>",
+        help="Name or URL of the Git remote to remove the experiment from",
+    )
+    experiments_remove_parser.add_argument(
+        "experiment",
+        nargs="*",
+        help="Experiments to remove.",
+        metavar="<experiment>",
     )
-    experiments_list_parser.set_defaults(func=CmdExperimentsList)
+    experiments_remove_parser.set_defaults(func=CmdExperimentsRemove)
```

### Comparing `dvc-3.0.0a0/dvc/commands/experiments/pull.py` & `dvc-3.0.0a1/dvc/commands/experiments/pull.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/experiments/push.py` & `dvc-3.0.0a1/dvc/commands/experiments/push.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/experiments/queue_worker.py` & `dvc-3.0.0a1/dvc/commands/experiments/queue_worker.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/experiments/run.py` & `dvc-3.0.0a1/dvc/commands/experiments/run.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,25 @@
 import argparse
 import logging
 
-from dvc.cli import completion
 from dvc.cli.utils import append_doc_link
 from dvc.commands.repro import CmdRepro
 from dvc.commands.repro import add_arguments as add_repro_arguments
-from dvc.exceptions import InvalidArgumentError
-from dvc.ui import ui
 
 logger = logging.getLogger(__name__)
 
 
 class CmdExperimentsRun(CmdRepro):
     def run(self):
-        if self.args.checkpoint_resume:
-            if self.args.reset:
-                raise InvalidArgumentError("--reset and --rev are mutually exclusive.")
-            if not (self.args.queue or self.args.tmp_dir):
-                raise InvalidArgumentError(
-                    "--rev can only be used in conjunction with --queue or --temp."
-                )
-
-        if self.args.reset:
-            ui.write("Any existing checkpoints will be reset and re-run.")
-
         self.repo.experiments.run(
             name=self.args.name,
             queue=self.args.queue,
             run_all=self.args.run_all,
             jobs=self.args.jobs,
             params=self.args.set_param,
-            checkpoint_resume=self.args.checkpoint_resume,
-            reset=self.args.reset,
             tmp_dir=self.args.tmp_dir,
             machine=self.args.machine,
             copy_paths=self.args.copy_paths,
             message=self.args.message,
             **self._common_kwargs,
         )
 
@@ -48,30 +32,14 @@
         "run",
         parents=[parent_parser],
         description=append_doc_link(EXPERIMENTS_RUN_HELP, "exp/run"),
         help=EXPERIMENTS_RUN_HELP,
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     _add_run_common(experiments_run_parser)
-    experiments_run_parser.add_argument(
-        "-r",
-        "--rev",
-        type=str,
-        dest="checkpoint_resume",
-        help=(
-            "Continue the specified checkpoint experiment. Can only be used "
-            "in conjunction with --queue or --temp."
-        ),
-        metavar="<experiment_rev>",
-    ).complete = completion.EXPERIMENT
-    experiments_run_parser.add_argument(
-        "--reset",
-        action="store_true",
-        help="Reset existing checkpoints and restart the experiment.",
-    )
     experiments_run_parser.set_defaults(func=CmdExperimentsRun)
 
 
 def _add_run_common(parser):
     """Add common args for 'exp run'."""
     # inherit arguments from `dvc repro`
     add_repro_arguments(parser)
```

### Comparing `dvc-3.0.0a0/dvc/commands/experiments/save.py` & `dvc-3.0.0a1/dvc/commands/experiments/save.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/experiments/show.py` & `dvc-3.0.0a1/dvc/commands/experiments/show.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,14 @@
 FILL_VALUE_ERRORED = "!"
 
 
 logger = logging.getLogger(__name__)
 
 
 experiment_types = {
-    "checkpoint_tip": "│ ╓",
-    "checkpoint_commit": "│ ╟",
-    "checkpoint_base": "├─╨",
     "branch_commit": "├──",
     "branch_base": "└──",
     "baseline": "",
 }
 
 
 def prepare_exp_id(kwargs) -> "RichText":
```

### Comparing `dvc-3.0.0a0/dvc/commands/freeze.py` & `dvc-3.0.0a1/dvc/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/gc.py` & `dvc-3.0.0a1/dvc/commands/gc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/get.py` & `dvc-3.0.0a1/dvc/commands/get.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/get_url.py` & `dvc-3.0.0a1/dvc/commands/get_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/git_hook.py` & `dvc-3.0.0a1/dvc/commands/git_hook.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/imp.py` & `dvc-3.0.0a1/dvc/commands/imp.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/imp_url.py` & `dvc-3.0.0a1/dvc/commands/imp_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/init.py` & `dvc-3.0.0a1/dvc/commands/init.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/install.py` & `dvc-3.0.0a1/dvc/commands/install.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/ls/__init__.py` & `dvc-3.0.0a1/dvc/commands/ls/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/ls/ls_colors.py` & `dvc-3.0.0a1/dvc/commands/ls/ls_colors.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/ls_url.py` & `dvc-3.0.0a1/dvc/commands/ls_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/machine.py` & `dvc-3.0.0a1/dvc/commands/machine.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/metrics.py` & `dvc-3.0.0a1/dvc/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/move.py` & `dvc-3.0.0a1/dvc/commands/move.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/params.py` & `dvc-3.0.0a1/dvc/commands/params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/plots.py` & `dvc-3.0.0a1/dvc/commands/plots.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/queue/__init__.py` & `dvc-3.0.0a1/dvc/commands/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/queue/kill.py` & `dvc-3.0.0a1/dvc/commands/queue/kill.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/queue/logs.py` & `dvc-3.0.0a1/dvc/commands/queue/logs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/queue/remove.py` & `dvc-3.0.0a1/dvc/commands/queue/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/queue/start.py` & `dvc-3.0.0a1/dvc/commands/queue/start.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/queue/status.py` & `dvc-3.0.0a1/dvc/commands/queue/status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/queue/stop.py` & `dvc-3.0.0a1/dvc/commands/queue/stop.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/remote.py` & `dvc-3.0.0a1/dvc/commands/remote.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/remove.py` & `dvc-3.0.0a1/dvc/commands/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/repro.py` & `dvc-3.0.0a1/dvc/commands/repro.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/root.py` & `dvc-3.0.0a1/dvc/commands/root.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/stage.py` & `dvc-3.0.0a1/dvc/commands/stage.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,25 +192,14 @@
         "--outs-no-cache",
         action="append",
         default=[],
         help="Declare output file or directory (do not put into DVC cache).",
         metavar="<filename>",
     ).complete = completion.FILE
     parser.add_argument(
-        "-c",
-        "--checkpoints",
-        action="append",
-        default=[],
-        help=(
-            "Declare checkpoint output file or directory for 'dvc exp run'. "
-            "Not compatible with 'dvc repro'."
-        ),
-        metavar="<filename>",
-    ).complete = completion.FILE
-    parser.add_argument(
         "--external",
         action="store_true",
         default=False,
         help="Allow outputs that are outside of the DVC repository.",
     )
     parser.add_argument(
         "--outs-persist",
```

### Comparing `dvc-3.0.0a0/dvc/commands/status.py` & `dvc-3.0.0a1/dvc/commands/status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/unprotect.py` & `dvc-3.0.0a1/dvc/commands/unprotect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/update.py` & `dvc-3.0.0a1/dvc/commands/update.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/commands/version.py` & `dvc-3.0.0a1/dvc/commands/version.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/compare.py` & `dvc-3.0.0a1/dvc/compare.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/config.py` & `dvc-3.0.0a1/dvc/config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/config_schema.py` & `dvc-3.0.0a1/dvc/config_schema.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/daemon.py` & `dvc-3.0.0a1/dvc/daemon.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/dagascii.py` & `dvc-3.0.0a1/dvc/dagascii.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/data_cloud.py` & `dvc-3.0.0a1/dvc/data_cloud.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/dependency/__init__.py` & `dvc-3.0.0a1/dvc/dependency/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/dependency/base.py` & `dvc-3.0.0a1/dvc/dependency/base.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/dependency/param.py` & `dvc-3.0.0a1/dvc/dependency/param.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/dependency/repo.py` & `dvc-3.0.0a1/dvc/dependency/repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/dirs.py` & `dvc-3.0.0a1/dvc/dirs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/dvcfile.py` & `dvc-3.0.0a1/dvc/dvcfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/env.py` & `dvc-3.0.0a1/dvc/env.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-DVCLIVE_RESUME = "DVCLIVE_RESUME"
-DVC_CHECKPOINT = "DVC_CHECKPOINT"
 DVC_DAEMON = "DVC_DAEMON"
 DVC_EXP_AUTO_PUSH = "DVC_EXP_AUTO_PUSH"
 DVC_EXP_BASELINE_REV = "DVC_EXP_BASELINE_REV"
 DVC_EXP_GIT_REMOTE = "DVC_EXP_GIT_REMOTE"
 DVC_EXP_NAME = "DVC_EXP_NAME"
 DVC_GLOBAL_CONFIG_DIR = "DVC_GLOBAL_CONFIG_DIR"
 DVC_IGNORE_ISATTY = "DVC_IGNORE_ISATTY"
```

### Comparing `dvc-3.0.0a0/dvc/exceptions.py` & `dvc-3.0.0a1/dvc/exceptions.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/fs/__init__.py` & `dvc-3.0.0a1/dvc/fs/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/fs/callbacks.py` & `dvc-3.0.0a1/dvc/fs/callbacks.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/fs/data.py` & `dvc-3.0.0a1/dvc/fs/data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/fs/dvc.py` & `dvc-3.0.0a1/dvc/fs/dvc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/fs/git.py` & `dvc-3.0.0a1/dvc/fs/git.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/ignore.py` & `dvc-3.0.0a1/dvc/ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/info.py` & `dvc-3.0.0a1/dvc/info.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/lock.py` & `dvc-3.0.0a1/dvc/lock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/logger.py` & `dvc-3.0.0a1/dvc/logger.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/machine/__init__.py` & `dvc-3.0.0a1/dvc/machine/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/machine/backend/base.py` & `dvc-3.0.0a1/dvc/machine/backend/base.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/machine/backend/terraform.py` & `dvc-3.0.0a1/dvc/machine/backend/terraform.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/output.py` & `dvc-3.0.0a1/dvc/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,29 +87,27 @@
     ret = []
     for d in d_list:
         p = d.pop(Output.PARAM_PATH)
         cache = d.pop(Output.PARAM_CACHE, True)
         metric = d.pop(Output.PARAM_METRIC, False)
         plot = d.pop(Output.PARAM_PLOT, False)
         persist = d.pop(Output.PARAM_PERSIST, False)
-        checkpoint = d.pop(Output.PARAM_CHECKPOINT, False)
         remote = d.pop(Output.PARAM_REMOTE, None)
         annot = {field: d.pop(field, None) for field in ANNOTATION_FIELDS}
         files = d.pop(Output.PARAM_FILES, None)
         push = d.pop(Output.PARAM_PUSH, True)
         ret.append(
             _get(
                 stage,
                 p,
                 info=d,
                 cache=cache,
                 metric=metric,
                 plot=plot,
                 persist=persist,
-                checkpoint=checkpoint,
                 remote=remote,
                 **annot,
                 files=files,
                 push=push,
             )
         )
     return ret
@@ -118,28 +116,26 @@
 def loads_from(
     stage,
     s_list,
     use_cache=True,
     metric=False,
     plot=False,
     persist=False,
-    checkpoint=False,
     remote=None,
     push=True,
 ):
     return [
         _get(
             stage,
             s,
             info={},
             cache=use_cache,
             metric=metric,
             plot=plot,
             persist=persist,
-            checkpoint=checkpoint,
             remote=remote,
             push=push,
         )
         for s in s_list
     ]
 
 
@@ -187,15 +183,14 @@
             plt_d, flags = _split_dict(flags, keys=PLOT_PROPS.keys())
 
         extra = project(
             flags,
             [
                 Output.PARAM_CACHE,
                 Output.PARAM_PERSIST,
-                Output.PARAM_CHECKPOINT,
                 Output.PARAM_REMOTE,
                 Output.PARAM_PUSH,
                 *ANNOTATION_FIELDS,
             ],
         )
 
         yield _get(
@@ -282,15 +277,14 @@
 
 
 class Output:
     IS_DEPENDENCY = False
 
     PARAM_PATH = "path"
     PARAM_CACHE = "cache"
-    PARAM_CHECKPOINT = "checkpoint"
     PARAM_FILES = "files"
     PARAM_METRIC = "metric"
     PARAM_METRIC_TYPE = "type"
     PARAM_METRIC_XPATH = "xpath"
     PARAM_PLOT = "plot"
     PARAM_PLOT_TEMPLATE = "template"
     PARAM_PLOT_X = "x"
@@ -323,15 +317,14 @@
         stage,
         path,
         info=None,
         cache=True,
         metric=False,
         plot=False,
         persist=False,
-        checkpoint=False,
         desc=None,
         type=None,  # noqa: A002, pylint: disable=redefined-builtin
         labels=None,
         meta=None,
         remote=None,
         repo=None,
         fs_config=None,
@@ -390,15 +383,14 @@
         if files is not None:
             files = [merge_file_meta_from_cloud(f) for f in files]
         self.files = files
         self.use_cache = False if self.IS_DEPENDENCY else cache
         self.metric = False if self.IS_DEPENDENCY else metric
         self.plot = False if self.IS_DEPENDENCY else plot
         self.persist = persist
-        self.checkpoint = checkpoint
         self.can_push = push
 
         self.fs_path = self._parse_path(self.fs, fs_path)
         self.obj: Optional["HashFile"] = None
 
         self.odb: Optional["HashFileDB"] = None
         self.remote = remote
@@ -818,17 +810,14 @@
 
             if self.plot:
                 ret[self.PARAM_PLOT] = self.plot
 
             if self.persist:
                 ret[self.PARAM_PERSIST] = self.persist
 
-            if self.checkpoint:
-                ret[self.PARAM_CHECKPOINT] = self.checkpoint
-
             if self.remote:
                 ret[self.PARAM_REMOTE] = self.remote
 
             if not self.can_push:
                 ret[self.PARAM_PUSH] = self.can_push
 
         if with_files:
@@ -890,15 +879,14 @@
     def checkout(
         self,
         force: bool = False,
         progress_callback: "Callback" = DEFAULT_CALLBACK,
         relink: bool = False,
         filter_info: Optional[str] = None,
         allow_missing: bool = False,
-        checkpoint_reset: bool = False,
         **kwargs,
     ) -> Optional[Tuple[bool, Optional[bool]]]:
         # callback passed act as a aggregate callback.
         # do not let checkout to call set_size and change progressbar.
         class CallbackProxy(Callback):
             def relative_update(self, inc: int = 1) -> None:
                 progress_callback.relative_update(inc)
@@ -910,19 +898,14 @@
             return None
 
         obj = self.get_obj(filter_info=filter_info)
         if not obj and (filter_info and filter_info != self.fs_path):
             # backward compatibility
             return None
 
-        if self.checkpoint and checkpoint_reset:
-            if self.exists:
-                self.remove()
-            return None
-
         added = not self.exists
 
         try:
             modified = self._checkout(
                 filter_info or self.fs_path,
                 self.fs,
                 obj,
@@ -931,15 +914,15 @@
                 progress_callback=callback,
                 relink=relink,
                 state=self.repo.state,
                 prompt=prompt.confirm,
                 **kwargs,
             )
         except CheckoutError:
-            if allow_missing or self.checkpoint:
+            if allow_missing:
                 return None
             raise
         self.set_exec()
         return added, False if added else modified
 
     def remove(self, ignore_remove=False):
         self.fs.remove(self.fs_path, recursive=True)
@@ -1432,15 +1415,14 @@
 
 ARTIFACT_SCHEMA = {
     **CHECKSUMS_SCHEMA,
     **META_SCHEMA,
     Required(Output.PARAM_PATH): str,
     Output.PARAM_PLOT: bool,
     Output.PARAM_PERSIST: bool,
-    Output.PARAM_CHECKPOINT: bool,
     Output.PARAM_CLOUD: CLOUD_SCHEMA,
 }
 
 DIR_FILES_SCHEMA: Dict[str, Any] = {
     **CHECKSUMS_SCHEMA,
     **META_SCHEMA,
     Required(Tree.PARAM_RELPATH): str,
```

### Comparing `dvc-3.0.0a0/dvc/parsing/__init__.py` & `dvc-3.0.0a1/dvc/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/parsing/context.py` & `dvc-3.0.0a1/dvc/parsing/context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/parsing/interpolate.py` & `dvc-3.0.0a1/dvc/parsing/interpolate.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/pathspec_math.py` & `dvc-3.0.0a1/dvc/pathspec_math.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/progress.py` & `dvc-3.0.0a1/dvc/progress.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/prompt.py` & `dvc-3.0.0a1/dvc/prompt.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/render/convert.py` & `dvc-3.0.0a1/dvc/render/convert.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/render/converter/__init__.py` & `dvc-3.0.0a1/dvc/render/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/render/converter/image.py` & `dvc-3.0.0a1/dvc/render/converter/image.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/render/converter/vega.py` & `dvc-3.0.0a1/dvc/render/converter/vega.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/render/match.py` & `dvc-3.0.0a1/dvc/render/match.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/__init__.py` & `dvc-3.0.0a1/dvc/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/add.py` & `dvc-3.0.0a1/dvc/repo/add.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/artifacts.py` & `dvc-3.0.0a1/dvc/repo/artifacts.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/brancher.py` & `dvc-3.0.0a1/dvc/repo/brancher.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/checkout.py` & `dvc-3.0.0a1/dvc/repo/checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/collect.py` & `dvc-3.0.0a1/dvc/repo/collect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/commit.py` & `dvc-3.0.0a1/dvc/repo/commit.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/data.py` & `dvc-3.0.0a1/dvc/repo/data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/destroy.py` & `dvc-3.0.0a1/dvc/repo/destroy.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/diff.py` & `dvc-3.0.0a1/dvc/repo/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/__init__.py` & `dvc-3.0.0a1/dvc/repo/experiments/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 import os
 import re
 from typing import TYPE_CHECKING, Dict, Iterable, List, Optional
 
 from funcy import chain, first
 
-from dvc.exceptions import DvcException
 from dvc.ui import ui
 from dvc.utils import relpath
 from dvc.utils.objects import cached_property
 
 from .cache import ExpCache
 from .exceptions import (
     BaselineMismatchError,
@@ -18,15 +17,14 @@
     MultipleBranchError,
 )
 from .refs import (
     APPLY_STASH,
     CELERY_FAILED_STASH,
     CELERY_STASH,
     EXEC_APPLY,
-    EXEC_CHECKPOINT,
     EXEC_NAMESPACE,
     EXPS_NAMESPACE,
     WORKSPACE_STASH,
     ExpRefInfo,
 )
 from .stash import ApplyStash
 from .utils import check_ref_format, exp_refs_by_rev, unlocked_repo
@@ -44,18 +42,15 @@
 class Experiments:
     """Class that manages experiments in a DVC repo.
 
     Args:
         repo (dvc.repo.Repo): repo instance that these experiments belong to.
     """
 
-    BRANCH_RE = re.compile(
-        r"^(?P<baseline_rev>[a-f0-9]{7})-(?P<exp_sha>[a-f0-9]+)"
-        r"(?P<checkpoint>-checkpoint)?$"
-    )
+    BRANCH_RE = re.compile(r"^(?P<baseline_rev>[a-f0-9]{7})-(?P<exp_sha>[a-f0-9]+)")
 
     def __init__(self, repo):
         from dvc.scm import NoSCMError
 
         if repo.config["core"].get("no_scm", False):
             raise NoSCMError
 
@@ -134,55 +129,26 @@
         if exp_rev is not None:
             self._log_reproduced(results, tmp_dir=tmp_dir)
         return results
 
     def queue_one(
         self,
         queue: "BaseStashQueue",
-        checkpoint_resume: Optional[str] = None,
-        reset: bool = False,
         **kwargs,
     ) -> "QueueEntry":
         """Queue a single experiment."""
-        if reset:
-            self.reset_checkpoints()
-
         if kwargs.pop("machine", None) is not None:
             # TODO: decide how to handle queued remote execution
             raise NotImplementedError
 
-        if checkpoint_resume:
-            from dvc.scm import resolve_rev
-
-            resume_rev = resolve_rev(self.scm, checkpoint_resume)
-            try:
-                self.check_baseline(resume_rev)
-                checkpoint_resume = resume_rev
-            except BaselineMismatchError as exc:
-                raise DvcException(
-                    f"Cannot resume from '{checkpoint_resume}' as it is not "
-                    "derived from your current workspace."
-                ) from exc
-        else:
-            checkpoint_resume = self._workspace_resume_rev()
-
         return self.new(
             queue,
-            checkpoint_resume=checkpoint_resume,
-            reset=reset,
             **kwargs,
         )
 
-    def _workspace_resume_rev(self) -> Optional[str]:
-        last_checkpoint = self._get_last_checkpoint()
-        last_applied = self._get_last_applied()
-        if last_checkpoint and last_applied:
-            return last_applied
-        return None
-
     def reproduce_celery(  # noqa: C901
         self, entries: Optional[Iterable["QueueEntry"]] = None, **kwargs
     ) -> Dict[str, str]:
         results: Dict[str, str] = {}
         if entries is None:
             entries = list(
                 chain(
@@ -253,107 +219,45 @@
             "\tdvc exp branch <exp> <branch>\n"
         )
 
     def new(
         self,
         queue: "BaseStashQueue",
         *args,
-        checkpoint_resume: Optional[str] = None,
         **kwargs,
     ) -> "QueueEntry":
         """Create and enqueue a new experiment.
 
         Experiment will be derived from the current workspace.
         """
-        if checkpoint_resume is not None:
-            return self._resume_checkpoint(
-                queue, *args, resume_rev=checkpoint_resume, **kwargs
-            )
 
         name = kwargs.get("name", None)
         baseline_sha = kwargs.get("baseline_rev") or self.repo.scm.get_rev()
 
         if name:
             exp_ref = ExpRefInfo(baseline_sha=baseline_sha, name=name)
             check_ref_format(self.scm, exp_ref)
             force = kwargs.get("force", False)
             if self.scm.get_ref(str(exp_ref)) and not force:
                 raise ExperimentExistsError(exp_ref.name)
 
         return queue.put(*args, **kwargs)
 
-    def _resume_checkpoint(
-        self,
-        queue: "BaseStashQueue",
-        *args,
-        resume_rev: Optional[str] = None,
-        **kwargs,
-    ) -> "QueueEntry":
-        """Create and queue a resumed checkpoint experiment."""
-        assert resume_rev
-
-        branch: Optional[str] = None
-        try:
-            allow_multiple = bool(kwargs.get("params", None))
-            branch = self.get_branch_by_rev(resume_rev, allow_multiple=allow_multiple)
-            if not branch:
-                raise DvcException(
-                    f"Could not find checkpoint experiment '{resume_rev[:7]}'"
-                )
-            baseline_rev = self._get_baseline(branch)
-        except MultipleBranchError as exc:
-            baselines = {
-                info.baseline_sha for info in exc.ref_infos if info.baseline_sha
-            }
-            if len(baselines) == 1:
-                baseline_rev = baselines.pop()
-            else:
-                raise
-
-        logger.debug(
-            "Checkpoint run from '%s' with baseline '%s'",
-            resume_rev[:7],
-            baseline_rev,
-        )
-        return queue.put(
-            *args,
-            resume_rev=resume_rev,
-            baseline_rev=baseline_rev,
-            branch=branch,
-            **kwargs,
-        )
-
-    def _get_last_checkpoint(self) -> Optional[str]:
-        try:
-            last_checkpoint = self.scm.get_ref(EXEC_CHECKPOINT)
-            if last_checkpoint:
-                self.check_baseline(last_checkpoint)
-            return last_checkpoint
-        except BaselineMismatchError:
-            # If HEAD has moved since the the last checkpoint run,
-            # the specified checkpoint is no longer relevant
-            self.scm.remove_ref(EXEC_CHECKPOINT)
-        return None
-
     def _get_last_applied(self) -> Optional[str]:
         try:
             last_applied = self.scm.get_ref(EXEC_APPLY)
             if last_applied:
                 self.check_baseline(last_applied)
             return last_applied
         except BaselineMismatchError:
             # If HEAD has moved since the the last applied experiment,
             # the applied experiment is no longer relevant
             self.scm.remove_ref(EXEC_APPLY)
         return None
 
-    def reset_checkpoints(self):
-        self.scm.remove_ref(EXEC_CHECKPOINT)
-        self.scm.remove_ref(EXEC_APPLY)
-
     @unlocked_repo
     def _reproduce_queue(
         self,
         queue: "BaseStashQueue",
         copy_paths: Optional[List[str]] = None,
         message: Optional[str] = None,
         **kwargs,
@@ -445,25 +349,14 @@
                 else:
                     failed_stash = self.celery_queue.failed_stash
                     if failed_stash and rev in failed_stash.stash_revs:
                         name = failed_stash.stash_revs[rev].name
             result[rev] = name
         return result
 
-    def get_running_exps(self, fetch_refs: bool = True) -> Dict[str, Dict]:
-        """Return info for running experiments."""
-        result = {}
-        for queue in (
-            self.workspace_queue,
-            self.tempdir_queue,
-            self.celery_queue,
-        ):
-            result.update(queue.get_running_exps(fetch_refs))
-        return result
-
     def apply(self, *args, **kwargs):
         from dvc.repo.experiments.apply import apply
 
         return apply(self.repo, *args, **kwargs)
 
     def branch(self, *args, **kwargs):
         from dvc.repo.experiments.branch import branch
```

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/apply.py` & `dvc-3.0.0a1/dvc/repo/experiments/apply.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/branch.py` & `dvc-3.0.0a1/dvc/repo/experiments/branch.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/cache.py` & `dvc-3.0.0a1/dvc/repo/experiments/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/collect.py` & `dvc-3.0.0a1/dvc/repo/experiments/collect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/diff.py` & `dvc-3.0.0a1/dvc/repo/experiments/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/exceptions.py` & `dvc-3.0.0a1/dvc/repo/experiments/exceptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,29 +27,14 @@
             f"To {command} this experiment with a different name run:\n\n"
             f"\tdvc exp {command} -n <new_name> ...\n"
         )
         super().__init__(msg)
         self.name = name
 
 
-class CheckpointExistsError(DvcException):
-    def __init__(self, name: str):
-        msg = (
-            "Reproduced checkpoint experiment conflicts with existing "
-            f"experiment '{name}'. To restart (and overwrite) the existing "
-            "experiment run:\n\n"
-            "\tdvc exp run -f ...\n\n"
-            "To resume the existing experiment, run:\n\n"
-            f"\tdvc exp apply {name}\n"
-            "\tdvc exp run\n"
-        )
-        super().__init__(msg)
-        self.name = name
-
-
 class InvalidExpRefError(DvcException):
     def __init__(self, ref):
         super().__init__(f"'{ref}' is not a valid experiment refname.")
         self.ref = ref
 
 
 class InvalidExpRevError(InvalidArgumentError):
@@ -110,7 +95,14 @@
 
 class UnresolvedRunningExpNamesError(UnresolvedExpNamesError):
     NAME = "running experiment name"
 
 
 class ExpQueueEmptyError(DvcException):
     pass
+
+
+class ExpNotStartedError(DvcException):
+    def __init__(self, name: str):
+        super().__init__(
+            f"Queued experiment '{name}' exists but has not started running yet"
+        )
```

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/executor/base.py` & `dvc-3.0.0a1/dvc/repo/experiments/executor/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import os
 import pickle  # nosec B403
 import shutil
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from dataclasses import asdict, dataclass
 from enum import IntEnum
-from functools import partial
 from itertools import chain
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
@@ -25,26 +24,20 @@
 )
 
 from funcy import get_in
 from scmrepo.exceptions import SCMError
 
 from dvc.env import DVC_EXP_AUTO_PUSH, DVC_EXP_GIT_REMOTE
 from dvc.exceptions import DvcException
-from dvc.repo.experiments.exceptions import CheckpointExistsError, ExperimentExistsError
-from dvc.repo.experiments.refs import (
-    EXEC_BASELINE,
-    EXEC_BRANCH,
-    EXEC_CHECKPOINT,
-    ExpRefInfo,
-)
+from dvc.repo.experiments.exceptions import ExperimentExistsError
+from dvc.repo.experiments.refs import EXEC_BASELINE, EXEC_BRANCH, ExpRefInfo
 from dvc.repo.experiments.utils import to_studio_params
 from dvc.repo.metrics.show import _collect_top_level_metrics
 from dvc.repo.params.show import _collect_top_level_params
 from dvc.stage.serialize import to_lockfile
-from dvc.ui import ui
 from dvc.utils import dict_sha256, env2bool, relpath
 from dvc.utils.fs import remove
 from dvc.utils.studio import env_to_config
 
 if TYPE_CHECKING:
     from queue import Queue
 
@@ -377,58 +370,49 @@
         return data["args"], data["kwargs"]
 
     def fetch_exps(
         self,
         dest_scm: "Git",
         refs: List[str],
         force: bool = False,
-        on_diverged: Optional[Callable[[str, bool], None]] = None,
+        on_diverged: Optional[Callable[[str], None]] = None,
         **kwargs,
     ) -> Iterable[str]:
         """Fetch reproduced experiment refs into the specified SCM.
 
         Args:
             dest_scm: Destination Git instance.
             refs: reference names to be fetched from the remotes.
             force: If True, diverged refs will be overwritten
-            on_diverged: Callback in the form on_diverged(ref, is_checkpoint)
+            on_diverged: Callback in the form on_diverged(ref)
                 to be called when an experiment ref has diverged.
 
         Extra kwargs will be passed into the remote git client.
         """
 
-        if EXEC_CHECKPOINT in refs:
-            refs.remove(EXEC_CHECKPOINT)
-            has_checkpoint = True
-        else:
-            has_checkpoint = False
-
         def on_diverged_ref(orig_ref: str, new_rev: str):
             if force:
                 logger.debug("Replacing existing experiment '%s'", orig_ref)
                 return True
 
             if on_diverged:
-                return on_diverged(orig_ref, has_checkpoint)
+                return on_diverged(orig_ref)
 
-            self._raise_ref_conflict(dest_scm, orig_ref, new_rev, has_checkpoint)
+            self._raise_ref_conflict(dest_scm, orig_ref, new_rev)
             logger.debug("Reproduced existing experiment '%s'", orig_ref)
             return False
 
         # fetch experiments
         try:
             refspecs = [f"{ref}:{ref}" for ref in refs]
-            # update last run checkpoint (if it exists)
-            if has_checkpoint:
-                refspecs.append(f"{EXEC_CHECKPOINT}:{EXEC_CHECKPOINT}")
             dest_scm.fetch_refspecs(
                 self.git_url,
                 refspecs,
                 on_diverged=on_diverged_ref,
-                force=force or has_checkpoint,
+                force=force,
                 **kwargs,
             )
         except SCMError:
             pass
 
         return refs
 
@@ -473,14 +457,15 @@
             experiment hash (or None on error), exp_ref is the experiment ref,
             and force is a bool specifying whether or not this experiment
             should force overwrite any existing duplicates.
         """
         from dvc.repo.checkout import checkout as dvc_checkout
         from dvc.repo.reproduce import reproduce as dvc_reproduce
         from dvc.stage import PipelineStage
+        from dvc.ui import ui
 
         auto_push = env2bool(DVC_EXP_AUTO_PUSH)
         git_remote = os.getenv(DVC_EXP_GIT_REMOTE, None)
 
         unchanged = []
 
         if queue is not None:
@@ -493,14 +478,17 @@
                 [stage for stage in stages if isinstance(stage, PipelineStage)]
             )
 
         exp_hash: Optional[str] = None
         exp_ref: Optional["ExpRefInfo"] = None
         repro_force: bool = False
 
+        if info.name:
+            ui.write(f"Reproducing experiment '{info.name}'")
+
         with cls._repro_dvc(
             info,
             infofile,
             log_errors=log_errors,
             copy_paths=copy_paths,
             message=message,
             **kwargs,
@@ -517,64 +505,40 @@
             repro_force = kwargs.get("force", False)
             logger.trace(  # type: ignore[attr-defined]
                 "Executor repro with force = '%s'", str(repro_force)
             )
 
             repro_dry = kwargs.get("dry")
 
-            # NOTE: checkpoint outs are handled as a special type of persist
-            # out:
-            #
-            # - checkpoint out may not yet exist if this is the first time this
-            #   experiment has been run, this is not an error condition for
-            #   experiments
-            # - if experiment was run with --reset, the checkpoint out will be
-            #   removed at the start of the experiment (regardless of any
-            #   dvc.lock entry for the checkpoint out)
-            # - if run without --reset, the checkpoint out will be checked out
-            #   using any hash present in dvc.lock (or removed if no entry
-            #   exists in dvc.lock)
-            checkpoint_reset: bool = kwargs.pop("reset", False)
             if not repro_dry:
                 dvc_checkout(
                     dvc,
                     targets=targets,
                     with_deps=targets is not None,
                     force=True,
                     quiet=True,
                     allow_missing=True,
-                    checkpoint_reset=checkpoint_reset,
                     recursive=kwargs.get("recursive", False),
                 )
 
-            checkpoint_func = partial(
-                cls.checkpoint_callback,
-                dvc,
-                dvc.scm,
-                info.name,
-                repro_force or checkpoint_reset,
-            )
-
             stages = dvc_reproduce(
                 dvc,
                 *args,
                 on_unchanged=filter_pipeline,
-                checkpoint_func=checkpoint_func,
                 **kwargs,
             )
             if paths := cls._get_top_level_paths(dvc):
                 logger.debug("Staging top-level files: %s", paths)
                 dvc.scm_context.add(paths)
 
             exp_hash = cls.hash_exp(stages)
             if not repro_dry:
                 ref, exp_ref, repro_force = cls._repro_commit(
                     dvc,
                     info,
-                    stages,
                     exp_hash,
                     auto_push,
                     git_remote,
                     repro_force,
                     message=message,
                 )
                 info.result_hash = exp_hash
@@ -587,28 +551,25 @@
         return ExecutorResult(exp_hash, exp_ref, repro_force)
 
     @classmethod
     def _repro_commit(
         cls,
         dvc,
         info,
-        stages,
         exp_hash,
         auto_push,
         git_remote,
         repro_force,
         message: Optional[str] = None,
     ) -> Tuple[Optional[str], Optional["ExpRefInfo"], bool]:
-        is_checkpoint = any(stage.is_checkpoint for stage in stages)
         cls.commit(
             dvc.scm,
             exp_hash,
             exp_name=info.name,
             force=repro_force,
-            checkpoint=is_checkpoint,
             message=message,
         )
         if auto_push:
             cls._auto_push(dvc, dvc.scm, git_remote)
         ref: Optional[str] = dvc.scm.get_ref(EXEC_BRANCH, follow=False)
         exp_ref: Optional["ExpRefInfo"] = ExpRefInfo.from_ref(ref) if ref else None
         if cls.WARN_UNTRACKED:
@@ -635,15 +596,14 @@
         copy_paths: Optional[List[str]] = None,
         message: Optional[str] = None,
         **kwargs,
     ) -> Iterator["Repo"]:
         from dvc_studio_client.post_live_metrics import post_live_metrics
 
         from dvc.repo import Repo
-        from dvc.stage.monitor import CheckpointKilledError
 
         with Repo(os.path.join(info.root_dir, info.dvc_dir)) as dvc:
             info.status = TaskStatus.RUNNING
             if infofile is not None:
                 info.dump_json(infofile)
             if cls.QUIET:
                 dvc.scm_context.quiet = cls.QUIET
@@ -674,17 +634,14 @@
                     params=to_studio_params(dvc.params.show()),
                     dvc_studio_config=dvc_studio_config,
                     message=message,
                 )
                 logger.debug("Running repro in '%s'", os.getcwd())
                 yield dvc
                 info.status = TaskStatus.SUCCESS
-            except CheckpointKilledError:
-                info.status = TaskStatus.FAILED
-                raise
             except DvcException:
                 if log_errors:
                     logger.exception("")
                 info.status = TaskStatus.FAILED
                 raise
             except Exception:
                 if log_errors:
@@ -742,39 +699,20 @@
                     "to the remote '%s': %s"
                 ),
                 git_remote,
                 exc,
             )
 
     @classmethod
-    def checkpoint_callback(
-        cls,
-        dvc: "Repo",
-        scm: "Git",
-        name: Optional[str],
-        force: bool,
-        unchanged: Iterable["PipelineStage"],
-        stages: Iterable["PipelineStage"],
-    ):
-        exp_hash = cls.hash_exp(list(stages) + list(unchanged))
-        exp_rev = cls.commit(scm, exp_hash, exp_name=name, force=force, checkpoint=True)
-
-        if env2bool(DVC_EXP_AUTO_PUSH):
-            git_remote = os.getenv(DVC_EXP_GIT_REMOTE)
-            cls._auto_push(dvc, scm, git_remote)
-        ui.write(f"Checkpoint experiment iteration '{exp_rev[:7]}'.")
-
-    @classmethod
     def commit(
         cls,
         scm: "Git",
         exp_hash: str,
         exp_name: Optional[str] = None,
         force: bool = False,
-        checkpoint: bool = False,
         message: Optional[str] = None,
     ):
         """Commit stages as an experiment and return the commit SHA."""
         rev = scm.get_rev()
         if not scm.is_dirty(untracked_files=False):
             logger.debug("No changes to commit")
 
@@ -801,31 +739,28 @@
                 logger.debug("Commit to new experiment branch '%s'", branch)
 
         scm.add([], update=True)
         message = message or f"dvc: commit experiment {exp_hash}"
         scm.commit(message, no_verify=True)
         new_rev = scm.get_rev()
         if check_conflict:
-            new_rev = cls._raise_ref_conflict(scm, branch, new_rev, checkpoint)
+            new_rev = cls._raise_ref_conflict(scm, branch, new_rev)
         else:
             scm.set_ref(branch, new_rev, old_ref=old_ref)
         scm.set_ref(EXEC_BRANCH, branch, symbolic=True)
-        if checkpoint:
-            scm.set_ref(EXEC_CHECKPOINT, new_rev)
+
         return new_rev
 
     @staticmethod
-    def _raise_ref_conflict(scm, ref, new_rev, checkpoint):
+    def _raise_ref_conflict(scm, ref, new_rev):
         # If this commit is a duplicate of the existing commit at 'ref', return
         # the existing commit. Otherwise, error out and require user to re-run
         # with --force as needed
         orig_rev = scm.get_ref(ref)
         if scm.diff(orig_rev, new_rev):
-            if checkpoint:
-                raise CheckpointExistsError(ref)
             raise ExperimentExistsError(ref)
         return orig_rev
 
     @staticmethod
     def _set_log_level(level):
         # When executor.reproduce is run in a multiprocessing child process,
         # dvc.cli.main will not be called for that child process so we need to
```

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/executor/local.py` & `dvc-3.0.0a1/dvc/repo/experiments/executor/local.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,18 +6,16 @@
 
 from configobj import ConfigObj
 from funcy import retry
 from shortuuid import uuid
 
 from dvc.lock import LockError
 from dvc.repo.experiments.refs import (
-    EXEC_APPLY,
     EXEC_BASELINE,
     EXEC_BRANCH,
-    EXEC_CHECKPOINT,
     EXEC_HEAD,
     EXEC_MERGE,
     EXEC_NAMESPACE,
     TEMP_NAMESPACE,
 )
 from dvc.repo.experiments.utils import EXEC_TMP_DIR, get_exp_rwlock
 from dvc.scm import SCM, Git
@@ -120,17 +118,14 @@
                     push_refspec(scm, self.git_url, refspec)
                 self.scm.set_ref(EXEC_BRANCH, branch, symbolic=True)
             else:
                 push_refspec(scm, self.git_url, refspec)
                 if self.scm.get_ref(EXEC_BRANCH):
                     self.scm.remove_ref(EXEC_BRANCH)
 
-            if self.scm.get_ref(EXEC_CHECKPOINT):
-                self.scm.remove_ref(EXEC_CHECKPOINT)
-
         # checkout EXEC_HEAD and apply EXEC_MERGE on top of it without
         # committing
         assert isinstance(self.scm, Git)
         head = EXEC_BRANCH if branch else EXEC_HEAD
         self.scm.checkout(head, detach=True)
         merge_rev = self.scm.get_ref(EXEC_MERGE)
 
@@ -185,15 +180,14 @@
             raise
 
 
 class WorkspaceExecutor(BaseLocalExecutor):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._detach_stack = ExitStack()
-        self._orig_checkpoint = self.scm.get_ref(EXEC_CHECKPOINT)
 
     @classmethod
     def from_stash_entry(
         cls,
         repo: "Repo",
         entry: "ExpStashEntry",
         **kwargs,
@@ -247,10 +241,7 @@
         if infofile:
             remove(os.path.dirname(infofile))
         with self._detach_stack:
             self.scm.remove_ref(EXEC_BASELINE)
             self.scm.remove_ref(EXEC_MERGE)
             if self.scm.get_ref(EXEC_BRANCH):
                 self.scm.remove_ref(EXEC_BRANCH)
-            checkpoint = self.scm.get_ref(EXEC_CHECKPOINT)
-            if checkpoint and checkpoint != self._orig_checkpoint:
-                self.scm.set_ref(EXEC_APPLY, checkpoint)
```

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/executor/ssh.py` & `dvc-3.0.0a1/dvc/repo/experiments/executor/ssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 from dvc_ssh import SSHFileSystem
 from funcy import first
 
 from dvc.repo.experiments.refs import (
     EXEC_BASELINE,
     EXEC_BRANCH,
-    EXEC_CHECKPOINT,
     EXEC_HEAD,
     EXEC_MERGE,
     EXEC_NAMESPACE,
 )
 
 from .base import BaseExecutor, ExecutorInfo, ExecutorResult, TaskStatus
 
@@ -158,15 +157,14 @@
                 push_refspec(scm, self.git_url, refspec, **kwargs)
 
             if branch:
                 push_refspec(scm, self.git_url, [(branch, branch)], **kwargs)
                 self._ssh_cmd(fs, f"git symbolic-ref {EXEC_BRANCH} {branch}")
             else:
                 self._ssh_cmd(fs, f"git symbolic-ref -d {EXEC_BRANCH}", check=False)
-            self._ssh_cmd(fs, f"git update-ref -d {EXEC_CHECKPOINT}", check=False)
 
             # checkout EXEC_HEAD and apply EXEC_MERGE on top of it without
             # committing
             head = EXEC_BRANCH if branch else EXEC_HEAD
             self._ssh_cmd(fs, f"git checkout {head}")
             merge_rev = scm.get_ref(EXEC_MERGE)
             self._ssh_cmd(fs, f"git stash apply {merge_rev}")
```

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/ls.py` & `dvc-3.0.0a1/dvc/repo/experiments/ls.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from collections import defaultdict
-from typing import List, Optional, Union
+from typing import Dict, List, Optional, Tuple, Union
 
 from dvc.repo import locked
 from dvc.repo.scm_context import scm_context
 from dvc.scm import iter_revs
 
 from .utils import exp_refs_by_baseline
 
@@ -15,15 +15,19 @@
 @scm_context
 def ls(
     repo,
     rev: Optional[Union[List[str], str]] = None,
     all_commits: bool = False,
     num: int = 1,
     git_remote: Optional[str] = None,
-):
+) -> Dict[str, List[Tuple[str, Optional[str]]]]:
+    """List experiments.
+
+    Returns a dict mapping baseline revs to a list of (exp_name, exp_sha) tuples.
+    """
     rev_set = None
     if not all_commits:
         rev = rev or "HEAD"
         if isinstance(rev, str):
             rev = [rev]
         revs = iter_revs(repo.scm, rev, num)
         rev_set = set(revs.keys())
@@ -32,13 +36,18 @@
     tags = repo.scm.describe(ref_info_dict.keys())
     remained = {baseline for baseline, tag in tags.items() if tag is None}
     base = "refs/heads"
     ref_heads = repo.scm.describe(remained, base=base)
 
     results = defaultdict(list)
     for baseline in ref_info_dict:
-        name = baseline[:7]
+        name = baseline
         if tags[baseline] or ref_heads[baseline]:
             name = tags[baseline] or ref_heads[baseline][len(base) + 1 :]
-        results[name] = [info.name for info in ref_info_dict[baseline]]
+        for info in ref_info_dict[baseline]:
+            if git_remote:
+                exp_rev = None
+            else:
+                exp_rev = repo.scm.get_ref(str(info))
+            results[name].append((info.name, exp_rev))
 
     return results
```

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/pull.py` & `dvc-3.0.0a1/dvc/repo/experiments/pull.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/push.py` & `dvc-3.0.0a1/dvc/repo/experiments/push.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/queue/base.py` & `dvc-3.0.0a1/dvc/repo/experiments/queue/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,30 +17,27 @@
     Union,
 )
 
 from dvc_studio_client.post_live_metrics import get_studio_config
 from funcy import retry
 
 from dvc.dependency import ParamsDependency
-from dvc.env import DVC_EXP_BASELINE_REV, DVC_EXP_NAME, DVCLIVE_RESUME
-from dvc.exceptions import DvcException
+from dvc.env import DVC_EXP_BASELINE_REV, DVC_EXP_NAME
 from dvc.lock import LockError
-from dvc.repo.experiments.exceptions import CheckpointExistsError, ExperimentExistsError
+from dvc.repo.experiments.exceptions import ExperimentExistsError
 from dvc.repo.experiments.executor.base import BaseExecutor
 from dvc.repo.experiments.executor.local import WorkspaceExecutor
 from dvc.repo.experiments.refs import ExpRefInfo
 from dvc.repo.experiments.stash import ExpStash, ExpStashEntry
 from dvc.repo.experiments.utils import (
     EXEC_PID_DIR,
     EXEC_TMP_DIR,
-    exp_refs_by_rev,
     get_exp_rwlock,
     get_random_exp_name,
 )
-from dvc.ui import ui
 from dvc.utils.objects import cached_property
 from dvc.utils.studio import config_to_env
 
 from .utils import get_remote_executor_refs
 
 if TYPE_CHECKING:
     from dvc.repo import Repo
@@ -296,30 +293,28 @@
             rev: Stash rev or exp name.
             encoding: Text encoding for redirected output. Defaults to
                 `locale.getpreferredencoding()`.
             follow: Attach to running exp process and follow additional
                 output.
         """
 
-    def _stash_exp(  # noqa: PLR0915, C901
+    def _stash_exp(  # noqa: C901
         self,
         *args,
         params: Optional[Dict[str, List[str]]] = None,
-        resume_rev: Optional[str] = None,
         baseline_rev: Optional[str] = None,
         branch: Optional[str] = None,
         name: Optional[str] = None,
         **kwargs,
     ) -> QueueEntry:
         """Stash changes from the workspace as an experiment.
 
         Args:
             params: Dict mapping paths to `Hydra Override`_ patterns,
                 provided via `exp run --set-param`.
-            resume_rev: Optional checkpoint resume rev.
             baseline_rev: Optional baseline rev for this experiment, defaults
                 to the current SCM rev.
             branch: Optional experiment branch name. If specified, the
                 experiment will be added to `branch` instead of creating
                 a new branch.
             name: Optional experiment name. If specified this will be used as
                 the human-readable name in the experiment branch ref. Has no
@@ -334,96 +329,29 @@
                 if baseline_rev is None:
                     baseline_rev = orig_head
 
                 try:
                     if workspace:
                         self.stash.apply(workspace)
 
-                    if resume_rev:
-                        # move HEAD to the resume rev so that the stashed diff
-                        # only contains changes relative to resume rev
-                        stash_head = resume_rev
-                        self.scm.set_ref(
-                            "HEAD",
-                            resume_rev,
-                            message=f"dvc: resume from HEAD {resume_rev[:7]}",
-                        )
-                        self.scm.reset()
-
                     # update experiment params from command line
                     if params:
                         self._update_params(params)
 
                     # DVC commit data deps to preserve state across workspace
                     # & tempdir runs
                     self._stash_commit_deps(*args, **kwargs)
 
-                    if resume_rev:
-                        if branch:
-                            branch_name = ExpRefInfo.from_ref(branch).name
-                        else:
-                            branch_name = f"{resume_rev[:7]}"
-                        if self.scm.is_dirty(untracked_files=False):
-                            ui.write(
-                                (
-                                    "Modified checkpoint experiment based on "
-                                    f"'{branch_name}' will be created"
-                                ),
-                            )
-                            branch = None
-                        elif not branch or self.scm.get_ref(branch) != resume_rev:
-                            err_msg = [
-                                "Nothing to do for unchanged checkpoint "
-                                f"'{resume_rev[:7]}'. "
-                            ]
-                            if branch:
-                                err_msg.append(
-                                    "To resume from the head of this "
-                                    "experiment, use "
-                                    f"'dvc exp apply {branch_name}'."
-                                )
-                            else:
-                                names = [
-                                    ref_info.name
-                                    for ref_info in exp_refs_by_rev(
-                                        self.scm, resume_rev
-                                    )
-                                ]
-                                if len(names) > 3:
-                                    names[3:] = [f"... ({len(names) - 3} more)"]
-                                err_msg.append(
-                                    "To resume an experiment containing this "
-                                    "checkpoint, apply one of these heads:\n"
-                                    "\t{}".format(", ".join(names))
-                                )
-                            raise DvcException("".join(err_msg))
-                        else:
-                            ui.write(
-                                "Existing checkpoint experiment "
-                                f"'{branch_name}' will be resumed"
-                            )
-                        if name:
-                            logger.warning(
-                                (
-                                    "Ignoring option '--name %s' for resumed "
-                                    "experiment. Existing experiment name will"
-                                    "be preserved instead."
-                                ),
-                                name,
-                            )
-
                     # save additional repro command line arguments
                     run_env = {
                         DVC_EXP_BASELINE_REV: baseline_rev,
                     }
                     if not name:
                         name = get_random_exp_name(self.scm, baseline_rev)
                     run_env[DVC_EXP_NAME] = name
-                    if resume_rev:
-                        run_env[DVCLIVE_RESUME] = "1"
 
                     # save studio config to read later by dvc and dvclive
                     studio_config = get_studio_config(
                         dvc_studio_config=self.repo.config.get("studio")
                     )
                     run_env = {**config_to_env(studio_config), **run_env}
                     self._pack_args(*args, run_env=run_env, **kwargs)
@@ -441,20 +369,14 @@
                             "Stashed experiment '%s' with baseline '%s' "
                             "for future execution."
                         ),
                         stash_rev[:7],
                         baseline_rev[:7],
                     )
                 finally:
-                    if resume_rev:
-                        # NOTE: this set_ref + reset() is equivalent to
-                        # `git reset orig_head` (our SCM reset() only operates
-                        # on HEAD rather than any arbitrary commit)
-                        self.scm.set_ref("HEAD", orig_head, message="dvc: restore HEAD")
-                        self.scm.reset()
                     # Revert any of our changes before prior unstashing
                     self.scm.reset(hard=True)
 
         return QueueEntry(
             self.repo.root_dir,
             self.scm.root_dir,
             self.ref,
@@ -629,18 +551,16 @@
     def collect_git(
         exp: "Experiments",
         executor: BaseExecutor,
         exec_result: "ExecutorResult",
     ) -> Dict[str, str]:
         results = {}
 
-        def on_diverged(ref: str, checkpoint: bool):
+        def on_diverged(ref: str):
             ref_info = ExpRefInfo.from_ref(ref)
-            if checkpoint:
-                raise CheckpointExistsError(ref_info.name)
             raise ExperimentExistsError(ref_info.name)
 
         refs = get_remote_executor_refs(exp.scm, executor.git_url)
 
         with get_exp_rwlock(exp.repo, writes=refs):
             for ref in executor.fetch_exps(
                 exp.scm,
@@ -726,22 +646,14 @@
             self.scm.set_ref(
                 self.failed_stash.ref,
                 entry.stash_rev,
                 message=f"commit: {msg}",
             )
 
     @abstractmethod
-    def get_running_exps(self, fetch_refs: bool = True) -> Dict[str, Dict]:
-        """Get the execution info of the currently running experiments
-
-        Args:
-            fetch_ref (bool): fetch completed checkpoints or not.
-        """
-
-    @abstractmethod
     def collect_active_data(
         self,
         baseline_revs: Optional[Collection[str]],
         fetch_refs: bool = False,
         **kwargs,
     ) -> Dict[str, List["ExpRange"]]:
         """Collect data for active (running) experiments.
@@ -786,7 +698,31 @@
             baseline_revs: Optional resolved baseline Git SHAs. If set, only experiments
                 derived from the specified revisions will be collected. Defaults to
                 collecting all experiments.
 
         Returns:
             Dict mapping baseline revision to list of queued experiments.
         """
+
+    def active_repo(self, name: str) -> "Repo":
+        """Return a Repo for the specified active experiment if it exists."""
+        from dvc.exceptions import DvcException
+        from dvc.repo import Repo
+        from dvc.repo.experiments.exceptions import (
+            ExpNotStartedError,
+            InvalidExpRevError,
+        )
+        from dvc.repo.experiments.executor.base import ExecutorInfo, TaskStatus
+
+        for entry in self.iter_active():
+            if entry.name != name:
+                continue
+            infofile = self.get_infofile_path(entry.stash_rev)
+            executor_info = ExecutorInfo.load_json(infofile)
+            if executor_info.status < TaskStatus.RUNNING:
+                raise ExpNotStartedError(name)
+            dvc_root = os.path.join(executor_info.root_dir, executor_info.dvc_dir)
+            try:
+                return Repo(dvc_root)
+            except (FileNotFoundError, DvcException) as exc:
+                raise InvalidExpRevError(name) from exc
+        raise InvalidExpRevError(name)
```

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/queue/celery.py` & `dvc-3.0.0a1/dvc/repo/experiments/queue/celery.py`

 * *Files 2% similar despite different names*

```diff
@@ -485,27 +485,14 @@
         return celery_clear(self, *args, **kwargs)
 
     def remove(self, *args, **kwargs):
         from .remove import celery_remove
 
         return celery_remove(self, *args, **kwargs)
 
-    def get_running_exps(self, fetch_refs: bool = True) -> Dict[str, Dict]:
-        """Get the execution info of the currently running experiments
-
-        Args:
-            fetch_ref (bool): fetch completed checkpoints or not.
-        """
-        result: Dict[str, Dict] = {}
-        for entry in self.iter_active():
-            result.update(
-                fetch_running_exp_from_temp_dir(self, entry.stash_rev, fetch_refs)
-            )
-        return result
-
     def get_ref_and_entry_by_names(
         self,
         exp_names: Union[str, List[str]],
         git_remote: Optional[str] = None,
     ) -> Dict[str, ExpRefAndQueueEntry]:
         """Find finished ExpRefInfo or queued or failed QueueEntry by name"""
         from dvc.repo.experiments.utils import resolve_name
```

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/queue/remove.py` & `dvc-3.0.0a1/dvc/repo/experiments/queue/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/queue/tasks.py` & `dvc-3.0.0a1/dvc/repo/experiments/queue/tasks.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/queue/tempdir.py` & `dvc-3.0.0a1/dvc/repo/experiments/queue/tempdir.py`

 * *Files 10% similar despite different names*

```diff
@@ -96,16 +96,14 @@
         self,
         entry: QueueEntry,
         executor: "BaseExecutor",
         copy_paths: Optional[List[str]] = None,
         message: Optional[str] = None,
         **kwargs,
     ) -> Dict[str, Dict[str, str]]:
-        from dvc.stage.monitor import CheckpointKilledError
-
         results: Dict[str, Dict[str, str]] = defaultdict(dict)
         exec_name = self._EXEC_NAME or entry.stash_rev
         infofile = self.get_infofile_path(exec_name)
         try:
             rev = entry.stash_rev
             exec_result = executor.reproduce(
                 info=executor.info,
@@ -118,20 +116,14 @@
             )
             if not exec_result.exp_hash:
                 raise DvcException(f"Failed to reproduce experiment '{rev[:7]}'")
             if exec_result.ref_info:
                 results[rev].update(
                     self.collect_executor(self.repo.experiments, executor, exec_result)
                 )
-        except CheckpointKilledError:
-            results[rev].update(
-                self.collect_executor(self.repo.experiments, executor, exec_result)
-            )
-
-            return results
         except DvcException:
             raise
         except Exception as exc:  # noqa: BLE001
             raise DvcException(f"Failed to reproduce experiment '{rev[:7]}'") from exc
         finally:
             executor.cleanup(infofile)
         return results
@@ -140,22 +132,14 @@
     def collect_executor(
         exp: "Experiments",
         executor: "BaseExecutor",
         exec_result: "ExecutorResult",
     ) -> Dict[str, str]:
         return BaseStashQueue.collect_executor(exp, executor, exec_result)
 
-    def get_running_exps(self, fetch_refs: bool = True) -> Dict[str, Dict]:
-        result: Dict[str, Dict] = {}
-        for entry in self.iter_active():
-            result.update(
-                fetch_running_exp_from_temp_dir(self, entry.stash_rev, fetch_refs)
-            )
-        return result
-
     def collect_active_data(
         self,
         baseline_revs: Optional[Collection[str]],
         fetch_refs: bool = False,
         **kwargs,
     ) -> Dict[str, List["ExpRange"]]:
         from dvc.repo import Repo
```

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/queue/utils.py` & `dvc-3.0.0a1/dvc/repo/experiments/queue/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 import logging
 from typing import TYPE_CHECKING, Dict, List
 
 from scmrepo.exceptions import SCMError
 
 from dvc.repo.experiments.executor.base import ExecutorInfo, TaskStatus
-from dvc.repo.experiments.refs import (
-    EXEC_CHECKPOINT,
-    EXEC_NAMESPACE,
-    EXPS_NAMESPACE,
-    EXPS_STASH,
-)
+from dvc.repo.experiments.refs import EXEC_NAMESPACE, EXPS_NAMESPACE, EXPS_STASH
 from dvc.repo.experiments.utils import get_exp_rwlock, iter_remote_refs
 
 logger = logging.getLogger(__name__)
 
 
 if TYPE_CHECKING:
     from dvc.scm import Git
@@ -29,17 +24,15 @@
     """
     refs = []
     for ref in iter_remote_refs(
         scm,
         remote_url,
         base=EXPS_NAMESPACE,
     ):
-        if ref == EXEC_CHECKPOINT or (
-            not ref.startswith(EXEC_NAMESPACE) and ref != EXPS_STASH
-        ):
+        if not ref.startswith(EXEC_NAMESPACE) and ref != EXPS_STASH:
             refs.append(ref)
     return refs
 
 
 def fetch_running_exp_from_temp_dir(
     queue: "BaseStashQueue", rev: str, fetch_refs: bool
 ) -> Dict[str, Dict]:
@@ -63,15 +56,15 @@
         info = ExecutorInfo.from_dict(load_json(infofile))
     except OSError:
         return result
     if info.status <= TaskStatus.RUNNING:
         result[rev] = info.asdict()
         if info.git_url and fetch_refs and info.status > TaskStatus.PREPARING:
 
-            def on_diverged(_ref: str, _checkpoint: bool):
+            def on_diverged(_ref: str):
                 return True
 
             executor = TempDirExecutor.from_info(info)
             try:
                 refs = get_remote_executor_refs(queue.scm, executor.git_url)
                 with get_exp_rwlock(queue.repo, writes=refs):
                     for ref in executor.fetch_exps(
```

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/queue/workspace.py` & `dvc-3.0.0a1/dvc/repo/experiments/queue/workspace.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,15 +97,14 @@
             pass
         return results
 
     def _reproduce_entry(
         self, entry: QueueEntry, executor: "BaseExecutor", **kwargs
     ) -> Dict[str, Dict[str, str]]:
         kwargs.pop("copy_paths", None)
-        from dvc.stage.monitor import CheckpointKilledError
         from dvc_task.proc.process import ProcessInfo
 
         results: Dict[str, Dict[str, str]] = defaultdict(dict)
         exec_name = self._EXEC_NAME or entry.stash_rev
         proc_info = ProcessInfo(os.getpid(), None, None, None, None)
         proc_info_path = self._proc_info_path(exec_name)
         os.makedirs(os.path.dirname(proc_info_path), exist_ok=True)
@@ -123,17 +122,14 @@
             )
             if not exec_result.exp_hash:
                 raise DvcException(f"Failed to reproduce experiment '{rev[:7]}'")
             if exec_result.ref_info:
                 results[rev].update(
                     self.collect_executor(self.repo.experiments, executor, exec_result)
                 )
-        except CheckpointKilledError:
-            # Checkpoint errors have already been logged
-            return {}
         except DvcException:
             raise
         except Exception as exc:  # noqa: BLE001
             raise DvcException(f"Failed to reproduce experiment '{rev[:7]}'") from exc
         finally:
             executor.cleanup(infofile)
             remove(self._proc_info_path(exec_name))
@@ -187,41 +183,26 @@
         self,
         rev: str,
         encoding: Optional[str] = None,
         follow: bool = False,
     ):
         raise NotImplementedError
 
-    def get_running_exps(
-        self,
-        fetch_refs: bool = True,  # noqa: ARG002
-    ) -> Dict[str, Dict]:
+    def get_running_exp(self) -> Optional[str]:
+        """Return the name of the exp running in workspace (if it exists)."""
         assert self._EXEC_NAME
-        result: Dict[str, Dict] = {}
         if self._active_pid is None:
-            return result
+            return None
 
         infofile = self.get_infofile_path(self._EXEC_NAME)
-
         try:
             info = ExecutorInfo.from_dict(load_json(infofile))
         except OSError:
-            return result
-
-        if info.status < TaskStatus.FAILED:
-            # If we are appending to a checkpoint branch in a workspace
-            # run, show the latest checkpoint as running.
-            if info.status == TaskStatus.SUCCESS:
-                return result
-            last_rev = self.scm.get_ref(EXEC_BRANCH)
-            if last_rev:
-                result[last_rev] = info.asdict()
-            else:
-                result[self._EXEC_NAME] = info.asdict()
-        return result
+            return None
+        return info.name
 
     def collect_active_data(
         self,
         baseline_revs: Optional[Collection[str]],
         fetch_refs: bool = False,  # noqa: ARG002
         **kwargs,
     ) -> Dict[str, List["ExpRange"]]:
```

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/refs.py` & `dvc-3.0.0a1/dvc/repo/experiments/refs.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 APPLY_HEAD = f"{APPLY_NAMESPACE}/ORIG_HEAD"
 APPLY_STASH = f"{APPLY_NAMESPACE}/stash"
 CELERY_NAMESPACE = f"{EXPS_NAMESPACE}/celery"
 CELERY_STASH = f"{CELERY_NAMESPACE}/stash"
 CELERY_FAILED_STASH = f"{CELERY_NAMESPACE}/failed"
 EXEC_NAMESPACE = f"{EXPS_NAMESPACE}/exec"
 EXEC_APPLY = f"{EXEC_NAMESPACE}/EXEC_APPLY"
-EXEC_CHECKPOINT = f"{EXEC_NAMESPACE}/EXEC_CHECKPOINT"
 EXEC_BRANCH = f"{EXEC_NAMESPACE}/EXEC_BRANCH"
 EXEC_BASELINE = f"{EXEC_NAMESPACE}/EXEC_BASELINE"
 EXEC_HEAD = f"{EXEC_NAMESPACE}/EXEC_HEAD"
 EXEC_MERGE = f"{EXEC_NAMESPACE}/EXEC_MERGE"
 TEMP_NAMESPACE = f"{EXPS_NAMESPACE}/temp"
 STASHES = {WORKSPACE_STASH, CELERY_STASH}
 ITER_SKIP_NAMESPACES = {
```

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/remove.py` & `dvc-3.0.0a1/dvc/repo/experiments/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/run.py` & `dvc-3.0.0a1/dvc/repo/experiments/run.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,17 +83,14 @@
         from dvc.utils.hydra import get_hydra_sweeps
 
         sweeps = get_hydra_sweeps(path_overrides)
         name_prefix = kwargs.get("name")
     else:
         sweeps = [path_overrides]
 
-    if not kwargs.get("checkpoint_resume", None):
-        kwargs["reset"] = True
-
     for idx, sweep_overrides in enumerate(sweeps):
         if hydra_sweep and name_prefix is not None:
             kwargs["name"] = f"{name_prefix}-{idx+1}"
         queue_entry = repo.experiments.queue_one(
             repo.experiments.celery_queue,
             targets=targets,
             params=sweep_overrides,
```

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/save.py` & `dvc-3.0.0a1/dvc/repo/experiments/save.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/serialize.py` & `dvc-3.0.0a1/dvc/repo/experiments/serialize.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,15 +65,14 @@
                 repo,
                 targets=None,
                 rev=rev[:7],
                 recursive=False,
                 onerror=onerror_collect,
             )
         )
-        meta = cls._gather_meta(repo)
         return cls(
             rev=rev,
             params=params,
             metrics=metrics,
             deps={
                 relpath(dep.fs_path, repo.root_dir): ExpDep(
                     hash=dep.hash_info.value if dep.hash_info else None,
@@ -90,24 +89,17 @@
                     nfiles=out.meta.nfiles if out.meta else None,
                     use_cache=out.use_cache,
                     is_data_source=out.stage.is_data_source,
                 )
                 for out in repo.index.outs
                 if not (out.is_metric or out.is_plot)
             },
-            meta=meta,
             **kwargs,
         )
 
-    @staticmethod
-    def _gather_meta(repo: "Repo") -> Dict[str, Any]:
-        return {
-            "has_checkpoints": any(stage.is_checkpoint for stage in repo.index.stages)
-        }
-
     def dumpd(self) -> Dict[str, Any]:
         return asdict(self)
 
     def as_bytes(self) -> bytes:
         return _ISOEncoder().encode(self.dumpd()).encode("utf-8")
 
     @classmethod
```

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/show.py` & `dvc-3.0.0a1/dvc/repo/experiments/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/stash.py` & `dvc-3.0.0a1/dvc/repo/experiments/stash.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 class ExpStashEntry(NamedTuple):
     """Experiment stash entry.
 
     stash_index: Stash index for this entry. Can be None if this commit
         is not pushed onto the stash ref.
     head_rev: HEAD Git commit to be checked out for this experiment.
     baseline_rev: Experiment baseline commit.
-    branch: Optional exp (checkpoint) branch name for this experiment.
+    branch: Optional branch name for this experiment.
     name: Optional exp name.
     """
 
     stash_index: Optional[int]
     head_rev: str
     baseline_rev: str
     branch: Optional[str]
```

### Comparing `dvc-3.0.0a0/dvc/repo/experiments/utils.py` & `dvc-3.0.0a1/dvc/repo/experiments/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from dvc.rwlock import rwlock
 from dvc.scm import Git
 
 from .refs import (
     EXEC_APPLY,
     EXEC_BASELINE,
     EXEC_BRANCH,
-    EXEC_CHECKPOINT,
     EXPS_NAMESPACE,
     ITER_SKIP_NAMESPACES,
     STASHES,
     ExpRefInfo,
 )
 
 if TYPE_CHECKING:
@@ -217,24 +216,21 @@
         shas.update(scm.branch_revs(str(ref_info), ref_info.baseline_sha))
     yield from shas
 
 
 def remove_exp_refs(scm: "Git", ref_infos: Iterable[ExpRefInfo]):
     exec_branch = scm.get_ref(EXEC_BRANCH, follow=False)
     exec_apply = scm.get_ref(EXEC_APPLY)
-    exec_checkpoint = scm.get_ref(EXEC_CHECKPOINT)
 
     for ref_info in ref_infos:
         ref = scm.get_ref(str(ref_info))
         if exec_branch and str(ref_info):
             scm.remove_ref(EXEC_BRANCH)
         if exec_apply and exec_apply == ref:
             scm.remove_ref(EXEC_APPLY)
-        if exec_checkpoint and exec_checkpoint == ref:
-            scm.remove_ref(EXEC_CHECKPOINT)
         scm.remove_ref(str(ref_info))
 
 
 def fix_exp_head(scm: Union["Git", "NoSCM"], ref: Optional[str]) -> Optional[str]:
     if ref:
         name, tail = Git.split_ref_pattern(ref)
         if name == "HEAD" and scm.get_ref(EXEC_BASELINE):
```

### Comparing `dvc-3.0.0a0/dvc/repo/fetch.py` & `dvc-3.0.0a1/dvc/repo/fetch.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/gc.py` & `dvc-3.0.0a1/dvc/repo/gc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/get.py` & `dvc-3.0.0a1/dvc/repo/get.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/get_url.py` & `dvc-3.0.0a1/dvc/repo/get_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/graph.py` & `dvc-3.0.0a1/dvc/repo/graph.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/imp_url.py` & `dvc-3.0.0a1/dvc/repo/imp_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/imports.py` & `dvc-3.0.0a1/dvc/repo/imports.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/index.py` & `dvc-3.0.0a1/dvc/repo/index.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/init.py` & `dvc-3.0.0a1/dvc/repo/init.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/install.py` & `dvc-3.0.0a1/dvc/repo/install.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/ls.py` & `dvc-3.0.0a1/dvc/repo/ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/ls_url.py` & `dvc-3.0.0a1/dvc/repo/ls_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/metrics/diff.py` & `dvc-3.0.0a1/dvc/repo/metrics/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/metrics/show.py` & `dvc-3.0.0a1/dvc/repo/metrics/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/move.py` & `dvc-3.0.0a1/dvc/repo/move.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/open_repo.py` & `dvc-3.0.0a1/dvc/repo/open_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/params/diff.py` & `dvc-3.0.0a1/dvc/repo/params/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/params/show.py` & `dvc-3.0.0a1/dvc/repo/params/show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/plots/__init__.py` & `dvc-3.0.0a1/dvc/repo/plots/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,59 +117,66 @@
                             }
                         }
                     }
                 }
 
             }
         """
+        from dvc.repo.experiments.brancher import switch_repo
         from dvc.utils.collections import ensure_list
 
         targets = ensure_list(targets)
         targets = [self.repo.dvcfs.from_os_path(target) for target in targets]
 
-        for rev in self.repo.brancher(revs=revs):
-            # .brancher() adds unwanted workspace
-            if revs is not None and rev not in revs:
-                continue
-            rev = rev or "workspace"
-
-            res: Dict = {}
-            definitions = _collect_definitions(
-                self.repo,
-                targets=targets,
-                revision=rev,
-                onerror=onerror,
-                props=props,
-            )
-            if definitions:
-                res[rev] = {"definitions": definitions}
-
-                data_targets = _get_data_targets(definitions)
-
-                res[rev]["sources"] = self._collect_data_sources(
-                    targets=data_targets,
-                    recursive=recursive,
-                    props=props,
+        if revs is None:
+            revs = ["workspace"]
+        else:
+            revs = list(revs)
+            if "workspace" in revs:
+                # reorder revs to match repo.brancher ordering
+                revs.remove("workspace")
+                revs = ["workspace"] + revs
+        for rev in revs:
+            with switch_repo(self.repo, rev) as (repo, _):
+                res: Dict = {}
+                definitions = _collect_definitions(
+                    repo,
+                    targets=targets,
+                    revision=rev,
                     onerror=onerror,
+                    props=props,
                 )
-            yield res
+                if definitions:
+                    res[rev] = {"definitions": definitions}
+
+                    data_targets = _get_data_targets(definitions)
+
+                    res[rev]["sources"] = self._collect_data_sources(
+                        repo,
+                        targets=data_targets,
+                        recursive=recursive,
+                        props=props,
+                        onerror=onerror,
+                    )
+                yield res
 
     @error_handler
     def _collect_data_sources(
         self,
+        repo: "Repo",
         targets: Optional[List[str]] = None,
         recursive: bool = False,
         props: Optional[Dict] = None,
         onerror: Optional[Callable] = None,
     ):
-        fs = self.repo.dvcfs
+        fs = repo.dvcfs
 
         props = props or {}
 
-        plots = _collect_plots(self.repo, targets, recursive)
+        plots = _collect_plots(repo, targets, recursive)
         res: Dict[str, Any] = {}
         for fs_path, rev_props in plots.items():
             joined_props = {**rev_props, **props}
             res[fs_path] = {"props": joined_props}
             res[fs_path].update(
                 {
                     "data_source": partial(
```

### Comparing `dvc-3.0.0a0/dvc/repo/plots/diff.py` & `dvc-3.0.0a1/dvc/repo/plots/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/pull.py` & `dvc-3.0.0a1/dvc/repo/pull.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/push.py` & `dvc-3.0.0a1/dvc/repo/push.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/remove.py` & `dvc-3.0.0a1/dvc/repo/remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/reproduce.py` & `dvc-3.0.0a1/dvc/repo/reproduce.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,37 @@
 import logging
-from functools import partial
 from typing import TYPE_CHECKING, Iterator, List
 
-from dvc.exceptions import DvcException, ReproductionError
+from dvc.exceptions import ReproductionError
 from dvc.repo.scm_context import scm_context
-from dvc.stage.exceptions import CheckpointKilledError
 
 from . import locked
 
 if TYPE_CHECKING:
     from dvc.stage import Stage
 
     from . import Repo
 
 logger = logging.getLogger(__name__)
 
 
 def _reproduce_stage(stage: "Stage", **kwargs) -> List["Stage"]:
-    def _run_callback(repro_callback):
-        stage.dump(update_pipeline=False)
-        _track_stage(stage)
-        repro_callback([stage])
-
-    checkpoint_func = kwargs.pop("checkpoint_func", None)
-    if stage.is_checkpoint:
-        if checkpoint_func:
-            kwargs["checkpoint_func"] = partial(_run_callback, checkpoint_func)
-        else:
-            raise DvcException(
-                "Checkpoint stages are not supported in 'dvc repro'. "
-                "Checkpoint stages must be reproduced with 'dvc exp run'. "
-            )
-
     if stage.frozen and not stage.is_import:
         logger.warning(
             "%s is frozen. Its dependencies are not going to be reproduced.",
             stage,
         )
 
     stage = stage.reproduce(**kwargs)
     if not stage:
         return []
 
     if not kwargs.get("dry", False):
-        track = checkpoint_func is not None
         stage.dump(update_pipeline=False)
-        if track:
-            _track_stage(stage)
+        _track_stage(stage)
 
     return [stage]
 
 
 def _get_stage_files(stage: "Stage") -> Iterator[str]:
     yield stage.dvcfile.relpath
     for dep in stage.deps:
@@ -178,25 +159,19 @@
     steps = _get_steps(graph, stages, downstream, single_item)
 
     force_downstream = kwargs.pop("force_downstream", False)
     result = []
     unchanged: List["Stage"] = []
     # `ret` is used to add a cosmetic newline.
     ret: List["Stage"] = []
-    checkpoint_func = kwargs.pop("checkpoint_func", None)
 
-    for i, stage in enumerate(steps):
+    for stage in steps:
         if ret:
             logger.info("")
 
-        if checkpoint_func:
-            kwargs["checkpoint_func"] = partial(
-                _repro_callback, checkpoint_func, unchanged
-            )
-
         try:
             ret = _reproduce_stage(stage, **kwargs)
 
             if len(ret) == 0:
                 unchanged.extend([stage])
             elif force_downstream:
                 # NOTE: we are walking our pipeline from the top to the
@@ -204,29 +179,14 @@
                 # which tells us that we should force reproducing all of
                 # the other stages down below, even if their direct
                 # dependencies didn't change.
                 kwargs["force"] = True
 
             if ret:
                 result.extend(ret)
-        except CheckpointKilledError:
-            result.append(stage)
-            logger.warning(
-                (
-                    "Checkpoint stage '%s' was interrupted remaining stages in"
-                    " pipeline will not be reproduced."
-                ),
-                stage.addressing,
-            )
-            logger.warning(
-                "skipped stages '%s'",
-                ", ".join(s.addressing for s in steps[i + 1 :]),
-            )
-
-            break
         except Exception as exc:  # noqa: BLE001
             raise ReproductionError(stage.addressing) from exc
 
     if on_unchanged is not None:
         on_unchanged(unchanged)
     return result
```

### Comparing `dvc-3.0.0a0/dvc/repo/run.py` & `dvc-3.0.0a1/dvc/repo/run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/scm_context.py` & `dvc-3.0.0a1/dvc/repo/scm_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/stage.py` & `dvc-3.0.0a1/dvc/repo/stage.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/status.py` & `dvc-3.0.0a1/dvc/repo/status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/trie.py` & `dvc-3.0.0a1/dvc/repo/trie.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/update.py` & `dvc-3.0.0a1/dvc/repo/update.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/repo/worktree.py` & `dvc-3.0.0a1/dvc/repo/worktree.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/rwlock.py` & `dvc-3.0.0a1/dvc/rwlock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/schema.py` & `dvc-3.0.0a1/dvc/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 }
 
 OUT_PSTAGE_DETAILED_SCHEMA = {
     str: {
         **ANNOTATION_SCHEMA,  # type: ignore[arg-type]
         Output.PARAM_CACHE: bool,
         Output.PARAM_PERSIST: bool,
-        Output.PARAM_CHECKPOINT: bool,
         Output.PARAM_REMOTE: str,
         Output.PARAM_PUSH: bool,
     }
 }
 
 PLOTS = "plots"
 PLOT_PROPS = {
```

### Comparing `dvc-3.0.0a0/dvc/scm.py` & `dvc-3.0.0a1/dvc/scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/stage/__init__.py` & `dvc-3.0.0a1/dvc/stage/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -273,61 +273,37 @@
 
         return isinstance(self.deps[0], RepoDependency)
 
     @property
     def is_versioned_import(self) -> bool:
         return self.is_import and self.deps[0].fs.version_aware
 
-    @property
-    def is_checkpoint(self) -> bool:
-        """
-        A stage containing checkpoint outs is always considered as changed
-        since the checkpoint out is a circular dependency.
-        """
-        return any(out.checkpoint for out in self.outs)
-
     def short_description(self) -> Optional["str"]:
         desc: Optional["str"] = None
         if self.desc:
             with suppress(ValueError):
                 # try to use first non-empty line as a description
                 line = next(filter(None, self.desc.splitlines()))
                 return line.strip()
         return desc
 
-    def _read_env(self, out, checkpoint_func=None) -> Env:
-        env: Env = {}
-        if out.checkpoint and checkpoint_func:
-            from dvc.env import DVC_CHECKPOINT
-
-            env.update({DVC_CHECKPOINT: "1"})
-        return env
-
-    def env(self, checkpoint_func=None) -> Env:
+    def env(self) -> Env:
         from dvc.env import DVC_ROOT
 
         env: Env = {}
         if self.repo:
             env.update({DVC_ROOT: self.repo.root_dir})
 
-        for out in self.outs:
-            current = self._read_env(out, checkpoint_func=checkpoint_func)
-            if any(
-                env.get(key) != current.get(key)
-                for key in set(env.keys()).intersection(current.keys())
-            ):
-                raise DvcException("Conflicting values for env variable")
-            env.update(current)
         return env
 
     def changed_deps(self, allow_missing: bool = False) -> bool:
         if self.frozen:
             return False
 
-        if self.is_callback or self.always_changed or self.is_checkpoint:
+        if self.is_callback or self.always_changed:
             return True
 
         return self._changed_deps(allow_missing=allow_missing)
 
     @rwlocked(read=["deps"])
     def _changed_deps(self, allow_missing: bool = False) -> bool:
         for dep in self.deps:
@@ -380,15 +356,15 @@
             logger.debug("%s changed.", self)
         return is_changed
 
     @rwlocked(write=["outs"])
     def remove_outs(self, ignore_remove=False, force=False) -> None:
         """Used mainly for `dvc remove --outs` and :func:`Stage.reproduce`."""
         for out in self.outs:
-            if (out.persist or out.checkpoint) and not force:
+            if out.persist and not force:
                 out.unprotect()
                 continue
 
             logger.debug("Removing output '%s' of %s.", out, self)
             out.remove(ignore_remove=ignore_remove)
 
     def unprotect_outs(self) -> None:
@@ -521,15 +497,15 @@
         from dvc.output import OutputDoesNotExistError
 
         old_versioned_outs = self.get_versioned_outs()
         for out in self.outs:
             try:
                 out.save()
             except OutputDoesNotExistError:
-                if not (allow_missing or out.checkpoint):
+                if not allow_missing:
                     raise
 
             if old_out := old_versioned_outs.get(out.def_path):
                 out.merge_version_meta(old_out)
 
     def ignore_outs(self) -> None:
         for out in self.outs:
@@ -556,15 +532,15 @@
         from dvc.output import OutputDoesNotExistError
 
         link_failures = []
         for out in self.filter_outs(filter_info):
             try:
                 out.commit(filter_info=filter_info, **kwargs)
             except OutputDoesNotExistError:
-                if not (allow_missing or out.checkpoint):
+                if not allow_missing:
                     raise
             except CacheLinkError:
                 link_failures.append(out.fs_path)
         if link_failures:
             raise CacheLinkError(link_failures)
 
     @rwlocked(write=["outs"])
@@ -575,15 +551,15 @@
 
         link_failures = []
         old_versioned_outs = self.get_versioned_outs()
         for out in self.filter_outs(filter_info):
             try:
                 out.add(filter_info, **kwargs)
             except (FileNotFoundError, OutputDoesNotExistError):
-                if not (allow_missing or out.checkpoint):
+                if not allow_missing:
                     raise
             except CacheLinkError:
                 link_failures.append(filter_info or out.fs_path)
 
             if old_out := old_versioned_outs.get(out.def_path):
                 out.merge_version_meta(old_out)
 
@@ -615,15 +591,15 @@
             self.checkout()
         elif not dry:
             args = ("outputs", "frozen ") if self.frozen else ("data sources", "")
             logger.info("Verifying %s in %s%s", *args, self)
             self._check_missing_outputs()
 
         if not dry:
-            if kwargs.get("checkpoint_func", None) or no_download:
+            if no_download:
                 allow_missing = True
 
             no_cache_outs = any(
                 not out.use_cache
                 for out in self.outs
                 if not (out.is_metric or out.is_plot)
             )
@@ -662,15 +638,15 @@
         stats: Dict[str, List["StrPath"]] = defaultdict(list)
         if self.is_partial_import:
             return stats
 
         for out in self.filter_outs(kwargs.get("filter_info")):
             key, outs = self._checkout(
                 out,
-                allow_missing=allow_missing or self.is_checkpoint,
+                allow_missing=allow_missing,
                 **kwargs,
             )
             if key:
                 stats[key].extend(outs)
         return stats
 
     @staticmethod
@@ -717,15 +693,15 @@
     def _status_outs(self, ret, filter_info) -> None:
         filter_outs = self.filter_outs(filter_info)
         outs_status = self._status(filter_outs)
         if outs_status:
             ret.append({"changed outs": outs_status})
 
     def _status_always_changed(self, ret) -> None:
-        if self.is_callback or self.always_changed or self.is_checkpoint:
+        if self.is_callback or self.always_changed:
             ret.append("always changed")
 
     def _status_stage(self, ret) -> None:
         if self.changed_stage():
             ret.append("changed checksum")
 
     def already_cached(self) -> bool:
```

### Comparing `dvc-3.0.0a0/dvc/stage/cache.py` & `dvc-3.0.0a1/dvc/stage/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/stage/decorators.py` & `dvc-3.0.0a1/dvc/stage/decorators.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/stage/exceptions.py` & `dvc-3.0.0a1/dvc/stage/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,22 +5,14 @@
     def __init__(self, cmd, status=None):
         msg = f"failed to run: {cmd}"
         if status is not None:
             msg += f", exited with {status}"
         super().__init__(msg)
 
 
-class CheckpointKilledError(DvcException):
-    def __init__(self, cmd, status=None):
-        msg = f"failed to finish: {cmd}"
-        if status is not None:
-            msg += f", exited with {status}"
-        super().__init__(msg)
-
-
 class StageFileDoesNotExistError(DvcException):
     DVC_IGNORED = "is dvc-ignored"
     DOES_NOT_EXIST = "does not exist"
 
     def __init__(self, fname, dvc_ignored=False):
         self.file = fname
         message = self.DVC_IGNORED if dvc_ignored else self.DOES_NOT_EXIST
```

### Comparing `dvc-3.0.0a0/dvc/stage/imports.py` & `dvc-3.0.0a1/dvc/stage/imports.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/stage/loader.py` & `dvc-3.0.0a1/dvc/stage/loader.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/stage/run.py` & `dvc-3.0.0a1/dvc/stage/run.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 import logging
 import os
 import signal
 import subprocess  # nosec B404
 import threading
-from typing import TYPE_CHECKING, List
 
-from dvc.stage.monitor import CheckpointTask, Monitor
 from dvc.utils import fix_env
 
 from .decorators import unlocked_repo
 from .exceptions import StageCmdFailedError
 
-if TYPE_CHECKING:
-    from dvc.stage import Stage
-
 logger = logging.getLogger(__name__)
 
 
 def _make_cmd(executable, cmd):
     if executable is None:
         return cmd
     opts = {"zsh": ["--no-rcs"], "bash": ["--noprofile", "--norc"]}
@@ -39,18 +34,17 @@
 
 
 def _enforce_cmd_list(cmd):
     assert cmd
     return cmd if isinstance(cmd, list) else cmd.splitlines()
 
 
-def prepare_kwargs(stage, checkpoint_func=None, run_env=None):
+def prepare_kwargs(stage, run_env=None):
     kwargs = {"cwd": stage.wdir, "env": fix_env(None), "close_fds": True}
 
-    kwargs["env"].update(stage.env(checkpoint_func=checkpoint_func))
     if run_env:
         kwargs["env"].update(run_env)
 
     # NOTE: when you specify `shell=True`, `Popen` [1] will default to
     # `/bin/sh` on *nix and will add ["/bin/sh", "-c"] to your command.
     # But we actually want to run the same shell that we are running
     # from right now, which is usually determined by the `SHELL` env
@@ -71,96 +65,78 @@
     logger.info("%s %s", ">", cmd)
 
 
 def get_executable():
     return (os.getenv("SHELL") or "/bin/sh") if os.name != "nt" else None
 
 
-def _run(stage: "Stage", executable, cmd, checkpoint_func, **kwargs):
+def _run(executable, cmd, **kwargs):
     # pylint: disable=protected-access
     main_thread = isinstance(
         threading.current_thread(),
         threading._MainThread,  # type: ignore[attr-defined]
     )
     old_handler = None
 
     exec_cmd = _make_cmd(executable, cmd)
 
     try:
         p = subprocess.Popen(exec_cmd, **kwargs)  # nosec B603
         if main_thread:
             old_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
 
-        tasks = _get_monitor_tasks(stage, checkpoint_func, p)
-
-        if tasks:
-            with Monitor(tasks):
-                p.communicate()
-        else:
-            p.communicate()
+        p.communicate()
 
         if p.returncode != 0:
-            for t in tasks:
-                if t.updated.is_set():
-                    raise t.error_cls(cmd, p.returncode)
             raise StageCmdFailedError(cmd, p.returncode)
     finally:
         if old_handler:
             signal.signal(signal.SIGINT, old_handler)
 
 
-def _get_monitor_tasks(stage, checkpoint_func, proc) -> List[CheckpointTask]:
-    result = []
-    if checkpoint_func:
-        result.append(CheckpointTask(stage, checkpoint_func, proc))
-
-    return result
-
-
-def cmd_run(stage, dry=False, checkpoint_func=None, run_env=None):
+def cmd_run(stage, dry=False, run_env=None):
     logger.info("Running stage '%s':", stage.addressing)
     commands = _enforce_cmd_list(stage.cmd)
-    kwargs = prepare_kwargs(stage, checkpoint_func=checkpoint_func, run_env=run_env)
+    kwargs = prepare_kwargs(stage, run_env=run_env)
     executable = get_executable()
 
     if not dry:
         warn_if_fish(executable)
 
     for cmd in commands:
         display_command(cmd)
         if dry:
             continue
 
-        _run(stage, executable, cmd, checkpoint_func=checkpoint_func, **kwargs)
+        _run(executable, cmd, **kwargs)
 
 
 def _pull_missing_deps(stage):
     for dep in stage.deps:
         if not dep.exists:
             stage.repo.pull(dep.def_path)
 
 
 def run_stage(
     stage,
     dry=False,
     force=False,
-    checkpoint_func=None,
     run_env=None,
     allow_missing: bool = False,
     **kwargs,
 ):
-    if not (force or checkpoint_func):
+    if not force:
         if allow_missing and kwargs.get("pull") and not dry:
             _pull_missing_deps(stage)
 
         from .cache import RunCacheNotFoundError
 
         try:
             stage.repo.stage_cache.restore(stage, dry=dry, **kwargs)
             if not dry:
                 return
         except RunCacheNotFoundError:
             if not dry:
                 stage.save_deps()
 
     run = cmd_run if dry else unlocked_repo(cmd_run)
-    run(stage, dry=dry, checkpoint_func=checkpoint_func, run_env=run_env)
+    run(stage, dry=dry, run_env=run_env)
```

### Comparing `dvc-3.0.0a0/dvc/stage/serialize.py` & `dvc-3.0.0a1/dvc/stage/serialize.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,31 +30,28 @@
 PARAM_DEPS = StageParams.PARAM_DEPS
 PARAM_OUTS = StageParams.PARAM_OUTS
 
 PARAM_CACHE = Output.PARAM_CACHE
 PARAM_METRIC = Output.PARAM_METRIC
 PARAM_PLOT = Output.PARAM_PLOT
 PARAM_PERSIST = Output.PARAM_PERSIST
-PARAM_CHECKPOINT = Output.PARAM_CHECKPOINT
 PARAM_DESC = Annotation.PARAM_DESC
 PARAM_REMOTE = Output.PARAM_REMOTE
 PARAM_PUSH = Output.PARAM_PUSH
 
 DEFAULT_PARAMS_FILE = ParamsDependency.DEFAULT_PARAMS_FILE
 
 
 @post_processing(OrderedDict)
 def _get_flags(out):
     annot = out.annot.to_dict()
     yield from annot.items()
 
     if not out.use_cache:
         yield PARAM_CACHE, False
-    if out.checkpoint:
-        yield PARAM_CHECKPOINT, True
     if out.persist:
         yield PARAM_PERSIST, True
     if out.plot and isinstance(out.plot, dict):
         # notice `out.plot` is not sorted
         # `out.plot` is in the same order as is in the file when read
         # and, should be dumped as-is without any sorting
         yield from out.plot.items()
```

### Comparing `dvc-3.0.0a0/dvc/stage/utils.py` & `dvc-3.0.0a1/dvc/stage/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,28 +58,26 @@
         "metrics_persist_no_cache",
         "plots",
         "plots_persist",
         "plots_no_cache",
         "plots_persist_no_cache",
         "outs_no_cache",
         "outs",
-        "checkpoints",
     ]
 
     stage.outs = []
 
     for key in keys:
         stage.outs += loads_from(
             stage,
             kwargs.get(key, []),
             use_cache="no_cache" not in key,
             persist="persist" in key,
             metric="metrics" in key,
             plot="plots" in key,
-            checkpoint="checkpoints" in key,
         )
 
 
 def fill_stage_dependencies(stage, deps=None, erepo=None, params=None, fs_config=None):
     from dvc.dependency import loads_from, loads_params
 
     assert not stage.deps
@@ -165,15 +163,14 @@
         d,
         exclude=[
             *ANNOTATION_FIELDS,
             stage.PARAM_LOCKED,  # backward compatibility
             stage.PARAM_FROZEN,
             Output.PARAM_METRIC,
             Output.PARAM_PERSIST,
-            Output.PARAM_CHECKPOINT,
             Meta.PARAM_ISEXEC,
             Meta.PARAM_SIZE,
             Meta.PARAM_NFILES,
         ],
     )
 
 
@@ -236,15 +233,14 @@
             kwargs.get("outs_no_cache", []),
             kwargs.get("metrics", []),
             kwargs.get("metrics_no_cache", []),
             kwargs.get("plots", []),
             kwargs.get("plots_no_cache", []),
             kwargs.get("outs_persist", []),
             kwargs.get("outs_persist_no_cache", []),
-            kwargs.get("checkpoints", []),
         )
     )
 
     return (
         os.path.basename(os.path.normpath(out)) + DVC_FILE_SUFFIX if out else DVC_FILE
     )
```

### Comparing `dvc-3.0.0a0/dvc/testing/README.rst` & `dvc-3.0.0a1/dvc/testing/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/testing/api_tests.py` & `dvc-3.0.0a1/dvc/testing/api_tests.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/testing/benchmarks/cli/commands/test_checkout.py` & `dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/testing/benchmarks/cli/commands/test_data_status.py` & `dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_data_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/testing/benchmarks/cli/commands/test_plots.py` & `dvc-3.0.0a1/dvc/testing/benchmarks/cli/commands/test_plots.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/testing/benchmarks/cli/stories/test_modify_data.py` & `dvc-3.0.0a1/dvc/testing/benchmarks/cli/stories/test_modify_data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/testing/benchmarks/fixtures.py` & `dvc-3.0.0a1/dvc/testing/benchmarks/fixtures.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/testing/benchmarks/plugin.py` & `dvc-3.0.0a1/dvc/testing/benchmarks/plugin.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/testing/cloud.py` & `dvc-3.0.0a1/dvc/testing/cloud.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/testing/fixtures.py` & `dvc-3.0.0a1/dvc/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/testing/path_info.py` & `dvc-3.0.0a1/dvc/testing/path_info.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/testing/plugin.py` & `dvc-3.0.0a1/dvc/testing/plugin.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/testing/remote_tests.py` & `dvc-3.0.0a1/dvc/testing/remote_tests.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/testing/tmp_dir.py` & `dvc-3.0.0a1/dvc/testing/tmp_dir.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/testing/workspace_tests.py` & `dvc-3.0.0a1/dvc/testing/workspace_tests.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/ui/__init__.py` & `dvc-3.0.0a1/dvc/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/ui/_rich_progress.py` & `dvc-3.0.0a1/dvc/ui/_rich_progress.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/ui/pager.py` & `dvc-3.0.0a1/dvc/ui/pager.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/ui/table.py` & `dvc-3.0.0a1/dvc/ui/table.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/updater.py` & `dvc-3.0.0a1/dvc/updater.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/utils/__init__.py` & `dvc-3.0.0a1/dvc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/utils/cli_parse.py` & `dvc-3.0.0a1/dvc/utils/cli_parse.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/utils/collections.py` & `dvc-3.0.0a1/dvc/utils/collections.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/utils/diff.py` & `dvc-3.0.0a1/dvc/utils/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/utils/fs.py` & `dvc-3.0.0a1/dvc/utils/fs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/utils/humanize.py` & `dvc-3.0.0a1/dvc/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/utils/hydra.py` & `dvc-3.0.0a1/dvc/utils/hydra.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/utils/serialize/__init__.py` & `dvc-3.0.0a1/dvc/utils/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/utils/serialize/_common.py` & `dvc-3.0.0a1/dvc/utils/serialize/_common.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/utils/serialize/_json.py` & `dvc-3.0.0a1/dvc/utils/serialize/_json.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/utils/serialize/_py.py` & `dvc-3.0.0a1/dvc/utils/serialize/_py.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/utils/serialize/_toml.py` & `dvc-3.0.0a1/dvc/utils/serialize/_toml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/utils/serialize/_yaml.py` & `dvc-3.0.0a1/dvc/utils/serialize/_yaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/utils/strictyaml.py` & `dvc-3.0.0a1/dvc/utils/strictyaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/utils/studio.py` & `dvc-3.0.0a1/dvc/utils/studio.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/utils/table.py` & `dvc-3.0.0a1/dvc/utils/table.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc/utils/threadpool.py` & `dvc-3.0.0a1/dvc/utils/threadpool.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/dvc.egg-info/PKG-INFO` & `dvc-3.0.0a1/dvc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc
-Version: 3.0.0a0
+Version: 3.0.0a1
 Summary: Git for data scientists - manage your code and data together
 Author-email: Dmitry Petrov <dmitry@dvc.org>
 Maintainer-email: Iterative <support@dvc.org>
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Issues, https://github.com/iterative/dvc/issues
 Project-URL: Source, https://github.com/iterative/dvc
```

### Comparing `dvc-3.0.0a0/dvc.egg-info/SOURCES.txt` & `dvc-3.0.0a1/dvc.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,14 @@
 dvc/commands/move.py
 dvc/commands/params.py
 dvc/commands/plots.py
 dvc/commands/remote.py
 dvc/commands/remove.py
 dvc/commands/repro.py
 dvc/commands/root.py
-dvc/commands/run.py
 dvc/commands/stage.py
 dvc/commands/status.py
 dvc/commands/unprotect.py
 dvc/commands/update.py
 dvc/commands/version.py
 dvc/commands/experiments/__init__.py
 dvc/commands/experiments/apply.py
@@ -196,14 +195,15 @@
 dvc/repo/status.py
 dvc/repo/trie.py
 dvc/repo/update.py
 dvc/repo/worktree.py
 dvc/repo/experiments/__init__.py
 dvc/repo/experiments/apply.py
 dvc/repo/experiments/branch.py
+dvc/repo/experiments/brancher.py
 dvc/repo/experiments/cache.py
 dvc/repo/experiments/clean.py
 dvc/repo/experiments/collect.py
 dvc/repo/experiments/diff.py
 dvc/repo/experiments/exceptions.py
 dvc/repo/experiments/ls.py
 dvc/repo/experiments/pull.py
@@ -239,15 +239,14 @@
 dvc/repo/plots/diff.py
 dvc/stage/__init__.py
 dvc/stage/cache.py
 dvc/stage/decorators.py
 dvc/stage/exceptions.py
 dvc/stage/imports.py
 dvc/stage/loader.py
-dvc/stage/monitor.py
 dvc/stage/params.py
 dvc/stage/run.py
 dvc/stage/serialize.py
 dvc/stage/utils.py
 dvc/testing/README.rst
 dvc/testing/__init__.py
 dvc/testing/api_tests.py
@@ -415,15 +414,14 @@
 tests/func/artifacts/test_artifacts.py
 tests/func/data/__init__.py
 tests/func/data/db/__init__.py
 tests/func/data/db/test_index.py
 tests/func/experiments/__init__.py
 tests/func/experiments/conftest.py
 tests/func/experiments/test_apply.py
-tests/func/experiments/test_checkpoints.py
 tests/func/experiments/test_diff.py
 tests/func/experiments/test_experiments.py
 tests/func/experiments/test_queue.py
 tests/func/experiments/test_remote.py
 tests/func/experiments/test_remove.py
 tests/func/experiments/test_save.py
 tests/func/experiments/test_set_params.py
@@ -514,15 +512,14 @@
 tests/unit/command/test_ls_url.py
 tests/unit/command/test_machine.py
 tests/unit/command/test_metrics.py
 tests/unit/command/test_params.py
 tests/unit/command/test_plots.py
 tests/unit/command/test_queue.py
 tests/unit/command/test_repro.py
-tests/unit/command/test_run.py
 tests/unit/command/test_stage.py
 tests/unit/command/test_status.py
 tests/unit/command/test_update.py
 tests/unit/command/ls/__init__.py
 tests/unit/command/ls/test_ls.py
 tests/unit/command/ls/test_ls_colors.py
 tests/unit/data/__init__.py
```

### Comparing `dvc-3.0.0a0/dvc.egg-info/requires.txt` & `dvc-3.0.0a1/dvc.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 [dev]
 dvc[azure,gdrive,gs,hdfs,lint,oss,s3,ssh,terraform,tests,webdav,webhdfs]
 
 [gdrive]
 dvc-gdrive==2.19.2
 
 [gs]
-dvc-gs==2.22.0
+dvc-gs==2.22.1
 
 [hdfs]
 dvc-hdfs==2.19
 
 [lint]
 mypy==1.3.0
 pylint==2.17.4
```

### Comparing `dvc-3.0.0a0/pyproject.toml` & `dvc-3.0.0a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     "zc.lockfile>=1.2.1",
 ]
 [project.optional-dependencies]
 all = ["dvc[azure,gdrive,gs,hdfs,oss,s3,ssh,webdav,webhdfs]"]
 azure = ["dvc-azure==2.21.1"]
 dev = ["dvc[azure,gdrive,gs,hdfs,lint,oss,s3,ssh,terraform,tests,webdav,webhdfs]"]
 gdrive = ["dvc-gdrive==2.19.2"]
-gs = ["dvc-gs==2.22.0"]
+gs = ["dvc-gs==2.22.1"]
 hdfs = ["dvc-hdfs==2.19"]
 lint = [
     "mypy==1.3.0",
     "pylint==2.17.4",
     "types-colorama",
     "types-psutil",
     "types-requests",
```

### Comparing `dvc-3.0.0a0/scripts/build.py` & `dvc-3.0.0a1/scripts/build.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/scripts/fpm/build.py` & `dvc-3.0.0a1/scripts/fpm/build.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/scripts/fpm/notarize.py` & `dvc-3.0.0a1/scripts/fpm/notarize.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/scripts/fpm/sign.py` & `dvc-3.0.0a1/scripts/fpm/sign.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/scripts/innosetup/addSymLinkPermissions.ps1` & `dvc-3.0.0a1/scripts/innosetup/addSymLinkPermissions.ps1`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/scripts/innosetup/addsymlink.iss` & `dvc-3.0.0a1/scripts/innosetup/addsymlink.iss`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/scripts/innosetup/build.py` & `dvc-3.0.0a1/scripts/innosetup/build.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/scripts/innosetup/modpath.iss` & `dvc-3.0.0a1/scripts/innosetup/modpath.iss`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/scripts/innosetup/setup.iss` & `dvc-3.0.0a1/scripts/innosetup/setup.iss`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/scripts/pyinstaller/build.py` & `dvc-3.0.0a1/scripts/pyinstaller/build.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/scripts/pyinstaller/hooks/hook-dvc.py` & `dvc-3.0.0a1/scripts/pyinstaller/hooks/hook-dvc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/scripts/pyinstaller/sign.py` & `dvc-3.0.0a1/scripts/pyinstaller/sign.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/conftest.py` & `dvc-3.0.0a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/dir_helpers.py` & `dvc-3.0.0a1/tests/dir_helpers.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/api/test_data.py` & `dvc-3.0.0a1/tests/func/api/test_data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/api/test_experiments.py` & `dvc-3.0.0a1/tests/func/api/test_experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/api/test_scm.py` & `dvc-3.0.0a1/tests/func/api/test_scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/api/test_show.py` & `dvc-3.0.0a1/tests/func/api/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/artifacts/test_artifacts.py` & `dvc-3.0.0a1/tests/func/artifacts/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/data/db/test_index.py` & `dvc-3.0.0a1/tests/func/data/db/test_index.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/experiments/conftest.py` & `dvc-3.0.0a1/tests/func/experiments/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import pytest
 
 from tests.unit.repo.experiments.conftest import (  # noqa, pylint disable=unused-argument
-    checkpoint_stage,
     exp_stage,
-    failed_checkpoint_stage,
     failed_exp_stage,
     session_app,
     session_queue,
     session_worker,
     test_queue,
 )
```

### Comparing `dvc-3.0.0a0/tests/func/experiments/executor/test_ssh.py` & `dvc-3.0.0a1/tests/func/experiments/executor/test_ssh.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/experiments/test_apply.py` & `dvc-3.0.0a1/tests/func/experiments/test_apply.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/experiments/test_diff.py` & `dvc-3.0.0a1/tests/func/experiments/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/experiments/test_experiments.py` & `dvc-3.0.0a1/tests/func/experiments/test_experiments.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,38 +358,38 @@
     ref_info_b = first(exp_refs_by_rev(scm, exp_b))
 
     tmp_dir.scm_gen("new", "new", commit="new")
     results = dvc.experiments.run(exp_stage.addressing, params=["foo=4"])
     exp_c = first(results)
     ref_info_c = first(exp_refs_by_rev(scm, exp_c))
 
-    assert dvc.experiments.ls() == {"master": [ref_info_c.name]}
+    assert dvc.experiments.ls() == {"master": [(ref_info_c.name, exp_c)]}
 
     exp_list = dvc.experiments.ls(rev=ref_info_a.baseline_sha)
     assert {key: set(val) for key, val in exp_list.items()} == {
-        baseline_a[:7]: {ref_info_a.name, ref_info_b.name}
+        baseline_a: {(ref_info_a.name, exp_a), (ref_info_b.name, exp_b)}
     }
 
     exp_list = dvc.experiments.ls(rev=[baseline_a, scm.get_rev()])
     assert {key: set(val) for key, val in exp_list.items()} == {
-        baseline_a[:7]: {ref_info_a.name, ref_info_b.name},
-        "master": {ref_info_c.name},
+        baseline_a: {(ref_info_a.name, exp_a), (ref_info_b.name, exp_b)},
+        "master": {(ref_info_c.name, exp_c)},
     }
 
     exp_list = dvc.experiments.ls(all_commits=True)
     assert {key: set(val) for key, val in exp_list.items()} == {
-        baseline_a[:7]: {ref_info_a.name, ref_info_b.name},
-        "master": {ref_info_c.name},
+        baseline_a: {(ref_info_a.name, exp_a), (ref_info_b.name, exp_b)},
+        "master": {(ref_info_c.name, exp_c)},
     }
 
     scm.checkout("branch", True)
     exp_list = dvc.experiments.ls(all_commits=True)
     assert {key: set(val) for key, val in exp_list.items()} == {
-        baseline_a[:7]: {ref_info_a.name, ref_info_b.name},
-        "branch": {ref_info_c.name},
+        baseline_a: {(ref_info_a.name, exp_a), (ref_info_b.name, exp_b)},
+        "branch": {(ref_info_c.name, exp_c)},
     }
 
 
 def test_subdir(tmp_dir, scm, dvc, workspace):
     subdir = tmp_dir / "dir"
     subdir.gen("copy.py", COPY_SCRIPT)
     subdir.gen("params.yaml", "foo: 1")
```

### Comparing `dvc-3.0.0a0/tests/func/experiments/test_queue.py` & `dvc-3.0.0a1/tests/func/experiments/test_queue.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/experiments/test_remote.py` & `dvc-3.0.0a1/tests/func/experiments/test_remote.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import os
-
 import pytest
 from funcy import first
 
 from dvc.repo.experiments.utils import exp_refs_by_rev
 
 
 @pytest.mark.parametrize("use_url", [True, False])
@@ -106,32 +104,14 @@
     }
     assert git_upstream.tmp_dir.scm.get_ref(str(ref_info)) == remote_rev
 
     dvc.experiments.push(git_upstream.remote, [ref_info.name], force=True)
     assert git_upstream.tmp_dir.scm.get_ref(str(ref_info)) == exp
 
 
-def test_push_checkpoint(tmp_dir, scm, dvc, git_upstream, checkpoint_stage):
-    results = dvc.experiments.run(checkpoint_stage.addressing, params=["foo=2"])
-    exp_a = first(results)
-    ref_info_a = first(exp_refs_by_rev(scm, exp_a))
-
-    dvc.experiments.push(git_upstream.remote, [ref_info_a.name], force=True)
-    assert git_upstream.tmp_dir.scm.get_ref(str(ref_info_a)) == exp_a
-
-    results = dvc.experiments.run(checkpoint_stage.addressing, checkpoint_resume=exp_a)
-    exp_b = first(results)
-    ref_info_b = first(exp_refs_by_rev(scm, exp_b))
-
-    tmp_dir.scm_gen("new", "new", commit="new")
-
-    dvc.experiments.push(git_upstream.remote, [ref_info_b.name], force=True)
-    assert git_upstream.tmp_dir.scm.get_ref(str(ref_info_b)) == exp_b
-
-
 def test_push_ambiguous_name(tmp_dir, scm, dvc, git_upstream, exp_stage):
     from dvc.exceptions import InvalidArgumentError
 
     remote = git_upstream.remote
 
     results = dvc.experiments.run(exp_stage.addressing, params=["foo=2"], name="foo")
     exp_a = first(results)
@@ -175,21 +155,21 @@
     assert git_downstream.tmp_dir.scm.get_ref("HEAD") != scm.get_ref("HEAD")
     downstream_exp = git_downstream.tmp_dir.dvc.experiments
     assert downstream_exp.ls(git_remote=remote) == {}
 
     git_downstream.tmp_dir.scm.fetch_refspecs(remote, ["master:master"])
     exp_list = downstream_exp.ls(rev=baseline_a, git_remote=remote)
     assert {key: set(val) for key, val in exp_list.items()} == {
-        baseline_a[:7]: {ref_info_a.name, ref_info_b.name}
+        baseline_a: {(ref_info_a.name, None), (ref_info_b.name, None)}
     }
 
     exp_list = downstream_exp.ls(all_commits=True, git_remote=remote)
     assert {key: set(val) for key, val in exp_list.items()} == {
-        baseline_a[:7]: {ref_info_a.name, ref_info_b.name},
-        "master": {ref_info_c.name},
+        baseline_a: {(ref_info_a.name, None), (ref_info_b.name, None)},
+        "master": {(ref_info_c.name, None)},
     }
 
 
 @pytest.mark.parametrize("use_url", [True, False])
 def test_pull(tmp_dir, scm, dvc, git_downstream, exp_stage, use_url):
     from dvc.exceptions import InvalidArgumentError
 
@@ -289,31 +269,14 @@
     assert downstream_exp.pull(git_downstream.remote, ref_info.name) == []
     assert git_downstream.tmp_dir.scm.get_ref(str(ref_info)) == remote_rev
 
     downstream_exp.pull(git_downstream.remote, ref_info.name, force=True)
     assert git_downstream.tmp_dir.scm.get_ref(str(ref_info)) == exp
 
 
-def test_pull_checkpoint(tmp_dir, scm, dvc, git_downstream, checkpoint_stage):
-    results = dvc.experiments.run(checkpoint_stage.addressing, params=["foo=2"])
-    exp_a = first(results)
-    ref_info_a = first(exp_refs_by_rev(scm, exp_a))
-
-    downstream_exp = git_downstream.tmp_dir.dvc.experiments
-    downstream_exp.pull(git_downstream.remote, [ref_info_a.name], force=True)
-    assert git_downstream.tmp_dir.scm.get_ref(str(ref_info_a)) == exp_a
-
-    results = dvc.experiments.run(checkpoint_stage.addressing, checkpoint_resume=exp_a)
-    exp_b = first(results)
-    ref_info_b = first(exp_refs_by_rev(scm, exp_b))
-
-    downstream_exp.pull(git_downstream.remote, [ref_info_b.name], force=True)
-    assert git_downstream.tmp_dir.scm.get_ref(str(ref_info_b)) == exp_b
-
-
 def test_pull_ambiguous_name(tmp_dir, scm, dvc, git_downstream, exp_stage):
     from dvc.exceptions import InvalidArgumentError
 
     results = dvc.experiments.run(exp_stage.addressing, params=["foo=2"], name="foo")
     exp_a = first(results)
     ref_info_a = first(exp_refs_by_rev(scm, exp_a))
 
@@ -331,44 +294,14 @@
     assert git_downstream.tmp_dir.scm.get_ref(str(ref_info_b)) == exp_b
 
     with git_downstream.tmp_dir.scm.detach_head(ref_info_a.baseline_sha):
         downstream_exp.pull(remote, ["foo"])
     assert git_downstream.tmp_dir.scm.get_ref(str(ref_info_a)) == exp_a
 
 
-def test_push_pull_cache(
-    tmp_dir, scm, dvc, git_upstream, checkpoint_stage, local_remote
-):
-    from dvc.utils.fs import remove
-    from tests.func.test_diff import digest
-
-    remote = git_upstream.remote
-    results = dvc.experiments.run(checkpoint_stage.addressing, params=["foo=2"])
-    exp = first(results)
-    ref_info = first(exp_refs_by_rev(scm, exp))
-
-    dvc.experiments.push(remote, [ref_info.name], push_cache=True)
-    for x in range(2, checkpoint_stage.iterations + 1):
-        hash_ = digest(str(x))
-        path = os.path.join(local_remote.url, hash_[:2], hash_[2:])
-        assert os.path.exists(path)
-        with open(path, encoding="utf-8") as f:
-            assert f.read() == str(x)
-
-    remove(dvc.cache.local.path)
-
-    dvc.experiments.pull(remote, [ref_info.name], pull_cache=True)
-    for x in range(2, checkpoint_stage.iterations + 1):
-        hash_ = digest(str(x))
-        path = os.path.join(dvc.cache.local.path, hash_[:2], hash_[2:])
-        assert os.path.exists(path)
-        with open(path, encoding="utf-8") as f:
-            assert f.read() == str(x)
-
-
 def test_auth_error_list(tmp_dir, scm, dvc, http_auth_patch):
     from dvc.scm import GitAuthError
 
     with pytest.raises(
         GitAuthError,
         match=f"Authentication failed for: '{http_auth_patch}'",
     ):
```

### Comparing `dvc-3.0.0a0/tests/func/experiments/test_remove.py` & `dvc-3.0.0a1/tests/func/experiments/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/experiments/test_save.py` & `dvc-3.0.0a1/tests/func/experiments/test_save.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,16 @@
     baseline = scm.get_rev()
     dvc.experiments.save(name="exp-1", force=True)
 
     tmp_dir.scm_gen({"new_file": "new_file"}, commit="new baseline")
     dvc.experiments.save(name="exp-2", force=True)
 
     all_exps = dvc.experiments.ls(all_commits=True)
-    assert all_exps[baseline[:7]] == ["exp-1"]
-    assert all_exps["master"] == ["exp-2"]
+    assert all_exps[baseline][0][0] == "exp-1"
+    assert all_exps["master"][0][0] == "exp-2"
 
 
 def test_exp_save_with_staged_changes(tmp_dir, dvc, scm):
     setup_stage(tmp_dir, dvc, scm)
     tmp_dir.gen({"deleted": "deleted", "modified": "modified"})
     scm.add_commit(["deleted", "modified"], "init")
```

### Comparing `dvc-3.0.0a0/tests/func/experiments/test_set_params.py` & `dvc-3.0.0a1/tests/func/experiments/test_set_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,14 @@
     dvc.experiments.run(params=overrides, queue=True)
 
     assert patched.call_count == len(expected)
     for e in expected:
         patched.assert_any_call(
             mocker.ANY,
             params=e,
-            reset=True,
             targets=None,
             copy_paths=None,
             message=None,
         )
 
 
 def test_hydra_sweep_requires_queue(params_repo, dvc):
```

### Comparing `dvc-3.0.0a0/tests/func/experiments/test_show.py` & `dvc-3.0.0a1/tests/func/experiments/test_show.py`

 * *Files 3% similar despite different names*

```diff
@@ -239,48 +239,14 @@
                 ),
                 "name": ANY,
             }
         ],
     }
 
 
-@pytest.mark.vscode
-@pytest.mark.parametrize("workspace", [True, False])
-def test_show_checkpoint(tmp_dir, scm, dvc, checkpoint_stage, capsys, workspace):
-    results = dvc.experiments.run(
-        checkpoint_stage.addressing, params=["foo=2"], tmp_dir=not workspace
-    )
-    exp_rev = first(results)
-
-    baseline = dvc.experiments.show()[1]
-    assert baseline.data.meta.get("has_checkpoints")
-    checkpoints = first(baseline.experiments)
-    # 2 checkpoints + final commit
-    assert len(checkpoints) == checkpoint_stage.iterations + 1
-    assert first(checkpoints).rev == exp_rev
-
-    capsys.readouterr()
-    assert main(["exp", "show", "--no-pager"]) == 0
-    cap = capsys.readouterr()
-
-    for i, exp in enumerate(checkpoints):
-        rev = exp.rev
-        if i == 0:
-            name = dvc.experiments.get_exact_name([rev])[rev]
-            name = f"{rev[:7]} [{name}]"
-            fs = "╓"
-        elif i == len(checkpoints) - 1:
-            name = rev[:7]
-            fs = "╨"
-        else:
-            name = rev[:7]
-            fs = "╟"
-        assert f"{fs} {name}" in cap.out
-
-
 def test_show_filter(
     tmp_dir,
     scm,
     dvc,
     capsys,
     copy_script,
 ):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dvc-3.0.0a0/tests/func/experiments/test_stash_exp.py` & `dvc-3.0.0a1/tests/func/experiments/test_stash_exp.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/experiments/test_utils.py` & `dvc-3.0.0a1/tests/func/experiments/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/machine/conftest.py` & `dvc-3.0.0a1/tests/func/machine/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/machine/test_machine_config.py` & `dvc-3.0.0a1/tests/func/machine/test_machine_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/machine/test_machine_status.py` & `dvc-3.0.0a1/tests/func/machine/test_machine_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/metrics/test_diff.py` & `dvc-3.0.0a1/tests/func/metrics/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/metrics/test_show.py` & `dvc-3.0.0a1/tests/func/metrics/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/params/test_diff.py` & `dvc-3.0.0a1/tests/func/params/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/params/test_show.py` & `dvc-3.0.0a1/tests/func/params/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/parsing/__init__.py` & `dvc-3.0.0a1/tests/func/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/parsing/test_errors.py` & `dvc-3.0.0a1/tests/func/parsing/test_errors.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/parsing/test_foreach.py` & `dvc-3.0.0a1/tests/func/parsing/test_foreach.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/parsing/test_interpolated_entry.py` & `dvc-3.0.0a1/tests/func/parsing/test_interpolated_entry.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/parsing/test_resolver.py` & `dvc-3.0.0a1/tests/func/parsing/test_resolver.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/plots/test_diff.py` & `dvc-3.0.0a1/tests/func/plots/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/plots/test_modify.py` & `dvc-3.0.0a1/tests/func/plots/test_modify.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/plots/test_show.py` & `dvc-3.0.0a1/tests/func/plots/test_show.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_add.py` & `dvc-3.0.0a1/tests/func/test_add.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,18 +358,14 @@
     assert ret == 0
     assert file_md5_counter.mock.call_count == 1
 
     ret = main(["status"])
     assert ret == 0
     assert file_md5_counter.mock.call_count == 1
 
-    ret = main(["run", "--single-stage", "-d", "foo", "echo foo"])
-    assert ret == 0
-    assert file_md5_counter.mock.call_count == 1
-
     os.rename("foo", "foo.back")
     ret = main(["checkout"])
     assert ret == 0
     assert file_md5_counter.mock.call_count == 1
 
     ret = main(["status"])
     assert ret == 0
@@ -388,27 +384,22 @@
     assert ret == 0
     assert file_md5_counter.mock.call_count == 4
 
     ret = main(["status"])
     assert ret == 0
     assert file_md5_counter.mock.call_count == 5
 
-    ls = "dir" if os.name == "nt" else "ls"
-    ret = main(["run", "--single-stage", "-d", "data", "{} {}".format(ls, "data")])
-    assert ret == 0
-    assert file_md5_counter.mock.call_count == 7
-
     os.rename("data", "data.back")
     ret = main(["checkout"])
     assert ret == 0
-    assert file_md5_counter.mock.call_count == 7
+    assert file_md5_counter.mock.call_count == 5
 
     ret = main(["status"])
     assert ret == 0
-    assert file_md5_counter.mock.call_count == 9
+    assert file_md5_counter.mock.call_count == 6
 
 
 def test_add_commit(tmp_dir, dvc):
     tmp_dir.gen("foo", "foo")
     ret = main(["add", "foo", "--no-commit"])
     assert ret == 0
     assert os.path.isfile("foo")
```

### Comparing `dvc-3.0.0a0/tests/func/test_analytics.py` & `dvc-3.0.0a1/tests/func/test_analytics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_check_ignore.py` & `dvc-3.0.0a1/tests/func/test_check_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_checkout.py` & `dvc-3.0.0a1/tests/func/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_cli.py` & `dvc-3.0.0a1/tests/func/test_cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,72 +7,23 @@
 from dvc.commands.add import CmdAdd
 from dvc.commands.checkout import CmdCheckout
 from dvc.commands.config import CmdConfig
 from dvc.commands.data_sync import CmdDataPull, CmdDataPush
 from dvc.commands.init import CmdInit
 from dvc.commands.remove import CmdRemove
 from dvc.commands.repro import CmdRepro
-from dvc.commands.run import CmdRun
 from dvc.commands.status import CmdDataStatus
 from dvc.exceptions import NotDvcRepoError
 
 
 def test_argparse(dvc):
     args = parse_args(["init"])
     assert isinstance(args.func(args), CmdInit)
 
 
-def test_run(dvc):
-    dep1 = "dep1"
-    dep2 = "dep2"
-
-    out1 = "out1"
-    out2 = "out2"
-
-    out_no_cache1 = "out_no_cache1"
-    out_no_cache2 = "out_no_cache2"
-
-    fname = "dvc.dvc"
-    cmd = "cmd"
-    arg1 = "arg1"
-    arg2 = "arg2"
-
-    args = parse_args(
-        [
-            "run",
-            "-d",
-            dep1,
-            "--deps",
-            dep2,
-            "-o",
-            out1,
-            "--outs",
-            out2,
-            "-O",
-            out_no_cache1,
-            "--outs-no-cache",
-            out_no_cache2,
-            "--file",
-            fname,
-            cmd,
-            arg1,
-            arg2,
-        ]
-    )
-    cmd_cls = args.func(args)
-    assert isinstance(cmd_cls, CmdRun)
-    assert args.deps == [dep1, dep2]
-    assert args.outs == [out1, out2]
-    assert args.outs_no_cache == [out_no_cache1, out_no_cache2]
-    assert args.file == fname
-    assert args.command == [cmd, arg1, arg2]
-
-    cmd_cls.repo.close()
-
-
 def test_pull(dvc):
     args = parse_args(["pull"])
     cmd = args.func(args)
     assert isinstance(cmd, CmdDataPull)
 
     cmd.repo.close()
```

### Comparing `dvc-3.0.0a0/tests/func/test_commit.py` & `dvc-3.0.0a1/tests/func/test_commit.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_config.py` & `dvc-3.0.0a1/tests/func/test_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_data_cloud.py` & `dvc-3.0.0a1/tests/func/test_data_cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,16 +143,14 @@
     test_file_md5 = mocker.spy(dvc_data.hashfile.hash, "file_md5")
     ret = main(["config", "cache.type", "hardlink"])
     assert ret == 0
     ret = main(["add", "foo"])
     assert ret == 0
     ret = main(["push"])
     assert ret == 0
-    ret = main(["run", "--single-stage", "-d", "foo", "echo foo"])
-    assert ret == 0
     assert test_file_md5.mock.call_count == 1
 
 
 def test_missing_cache(tmp_dir, dvc, local_remote, caplog):
     tmp_dir.dvc_gen({"foo": "foo", "bar": "bar"})
 
     # purge cache
```

### Comparing `dvc-3.0.0a0/tests/func/test_data_status.py` & `dvc-3.0.0a1/tests/func/test_data_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_diff.py` & `dvc-3.0.0a1/tests/func/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_dvcfile.py` & `dvc-3.0.0a1/tests/func/test_dvcfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_external_repo.py` & `dvc-3.0.0a1/tests/func/test_external_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_fs.py` & `dvc-3.0.0a1/tests/func/test_fs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_gc.py` & `dvc-3.0.0a1/tests/func/test_gc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_get.py` & `dvc-3.0.0a1/tests/func/test_get.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_get_url.py` & `dvc-3.0.0a1/tests/func/test_get_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_ignore.py` & `dvc-3.0.0a1/tests/func/test_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_import.py` & `dvc-3.0.0a1/tests/func/test_import.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_import_url.py` & `dvc-3.0.0a1/tests/func/test_import_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_init.py` & `dvc-3.0.0a1/tests/func/test_init.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_install.py` & `dvc-3.0.0a1/tests/func/test_install.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_lock.py` & `dvc-3.0.0a1/tests/func/test_lock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_lockfile.py` & `dvc-3.0.0a1/tests/func/test_lockfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_ls.py` & `dvc-3.0.0a1/tests/func/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_merge_driver.py` & `dvc-3.0.0a1/tests/func/test_merge_driver.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_move.py` & `dvc-3.0.0a1/tests/func/test_move.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_odb.py` & `dvc-3.0.0a1/tests/func/test_odb.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_remote.py` & `dvc-3.0.0a1/tests/func/test_remote.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_remove.py` & `dvc-3.0.0a1/tests/func/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_repo.py` & `dvc-3.0.0a1/tests/func/test_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_repo_index.py` & `dvc-3.0.0a1/tests/func/test_repo_index.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_repro.py` & `dvc-3.0.0a1/tests/func/test_repro.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,42 +331,42 @@
 
         f = os.path.join(idir, "file")
         with open(f, "w+", encoding="utf-8") as fobj:
             fobj.write(str(d))
 
         ret = main(
             [
-                "run",
-                "--no-exec",
-                "--single-stage",
+                "stage",
+                "add",
+                "-n",
+                f"copy-{idir}-{odir}",
                 "-d",
                 idir,
                 "-o",
                 odir,
                 'python -c \'import shutil; shutil.copytree("{}", "{}")\''.format(
                     idir, odir
                 ),
             ]
         )
         assert ret == 0
 
     ret = main(
         [
-            "run",
-            "--no-exec",
-            "--single-stage",
-            "--file",
-            DVC_FILE,
+            "stage",
+            "add",
+            "-n",
+            "ls",
             *deps,
             "ls {}".format(" ".join(dep for i, dep in enumerate(deps) if i % 2)),
         ]
     )
     assert ret == 0
 
-    ret = main(["repro", "--dry", DVC_FILE])
+    ret = main(["repro", "--dry", "ls"])
     assert ret == 0
 
 
 def test_repro_changed_deep_data(tmp_dir, dvc, copy_script, run_stage):
     tmp_dir.gen("bar", "bar")
     tmp_dir.dvc_gen("foo", "foo")
     run_stage(
@@ -1110,40 +1110,61 @@
     #      / \
     #     D   F
     #    / \   \
     #   B   C   G
     #    \ /
     #     A
     #
-    assert main(["run", "--single-stage", "-o", "A", "echo A>A"]) == 0
-    assert main(["run", "--single-stage", "-d", "A", "-o", "B", "echo B>B"]) == 0
-    assert main(["run", "--single-stage", "-d", "A", "-o", "C", "echo C>C"]) == 0
+    assert main(["stage", "add", "-n", "stage-A", "--run", "-o", "A", "echo A>A"]) == 0
+    assert (
+        main(
+            ["stage", "add", "-n", "stage-B", "--run", "-d", "A", "-o", "B", "echo B>B"]
+        )
+        == 0
+    )
+    assert (
+        main(
+            ["stage", "add", "-n", "stage-C", "--run", "-d", "A", "-o", "C", "echo C>C"]
+        )
+        == 0
+    )
     assert (
         main(
             [
-                "run",
-                "--single-stage",
+                "stage",
+                "add",
+                "-n",
+                "stage-D",
+                "--run",
                 "-d",
                 "B",
                 "-d",
                 "C",
                 "-o",
                 "D",
                 "echo D>D",
             ]
         )
         == 0
     )
-    assert main(["run", "--single-stage", "-o", "G", "echo G>G"]) == 0
-    assert main(["run", "--single-stage", "-d", "G", "-o", "F", "echo F>F"]) == 0
+    assert main(["stage", "add", "-n", "stage-G", "--run", "-o", "G", "echo G>G"]) == 0
+    assert (
+        main(
+            ["stage", "add", "-n", "stage-F", "--run", "-d", "G", "-o", "F", "echo F>F"]
+        )
+        == 0
+    )
     assert (
         main(
             [
-                "run",
-                "--single-stage",
+                "stage",
+                "add",
+                "-n",
+                "stage-E",
+                "--run",
                 "-d",
                 "D",
                 "-d",
                 "F",
                 "-o",
                 "E",
                 "echo E>E",
@@ -1156,30 +1177,33 @@
     #
     #       E
     #      /
     #     D
     #    /
     #   B
     #
-    evaluation = dvc.reproduce("B.dvc", downstream=True, force=True)
+    evaluation = dvc.reproduce("stage-B", downstream=True, force=True)
 
     assert len(evaluation) == 3
-    assert evaluation[0].relpath == "B.dvc"
-    assert evaluation[1].relpath == "D.dvc"
-    assert evaluation[2].relpath == "E.dvc"
+    assert evaluation[0].addressing == "stage-B"
+    assert evaluation[1].addressing == "stage-D"
+    assert evaluation[2].addressing == "stage-E"
 
     # B, C should be run (in any order) before D
     # See https://github.com/iterative/dvc/issues/3602
-    evaluation = dvc.reproduce("A.dvc", downstream=True, force=True)
+    evaluation = dvc.reproduce("stage-A", downstream=True, force=True)
 
     assert len(evaluation) == 5
-    assert evaluation[0].relpath == "A.dvc"
-    assert {evaluation[1].relpath, evaluation[2].relpath} == {"B.dvc", "C.dvc"}
-    assert evaluation[3].relpath == "D.dvc"
-    assert evaluation[4].relpath == "E.dvc"
+    assert evaluation[0].addressing == "stage-A"
+    assert {evaluation[1].addressing, evaluation[2].addressing} == {
+        "stage-B",
+        "stage-C",
+    }
+    assert evaluation[3].addressing == "stage-D"
+    assert evaluation[4].addressing == "stage-E"
 
 
 def test_repro_when_cmd_changes(tmp_dir, dvc, run_copy, mocker):
     from dvc.dvcfile import SingleStageFile
 
     tmp_dir.gen("foo", "foo")
     stage = run_copy("foo", "bar", single_stage=True)
@@ -1191,8 +1215,8 @@
 
     data = SingleStageFile(dvc, stage.path)._load()[0]
     data["cmd"] = "  ".join(stage.cmd.split())  # change cmd spacing by two
     (tmp_dir / stage.path).dump(data)
 
     assert dvc.status([stage.addressing]) == {stage.addressing: ["changed checksum"]}
     assert dvc.reproduce(stage.addressing)[0] == stage
-    m.assert_called_once_with(stage, checkpoint_func=None, dry=False, run_env=None)
+    m.assert_called_once_with(stage, dry=False, run_env=None)
```

### Comparing `dvc-3.0.0a0/tests/func/test_repro_multistage.py` & `dvc-3.0.0a1/tests/func/test_repro_multistage.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,38 +32,79 @@
     dvc.freeze("copy-data-stage1")
 
     tmp_dir.gen("data", "bar")
     stages = dvc.reproduce()
     assert stages == [data_stage, stage0]
 
 
-def test_downstream(tmp_dir, dvc):
+def test_downstream(M, tmp_dir, dvc):
     # The dependency graph should look like this:
     #
     #       E
     #      / \
     #     D   F
     #    / \   \
     #   B   C   G
     #    \ /
     #     A
     #
-    assert main(["run", "-n", "A-gen", "-o", "A", "echo A>A"]) == 0
-    assert main(["run", "-n", "B-gen", "-d", "A", "-o", "B", "echo B>B"]) == 0
-    assert main(["run", "--single-stage", "-d", "A", "-o", "C", "echo C>C"]) == 0
+    assert main(["stage", "add", "--run", "-n", "A-gen", "-o", "A", "echo A>A"]) == 0
     assert (
-        main(["run", "-n", "D-gen", "-d", "B", "-d", "C", "-o", "D", "echo D>D"]) == 0
+        main(["stage", "add", "--run", "-n", "B-gen", "-d", "A", "-o", "B", "echo B>B"])
+        == 0
+    )
+    assert (
+        main(
+            [
+                "stage",
+                "add",
+                "--run",
+                "-n",
+                "C-gen",
+                "-d",
+                "A",
+                "-o",
+                "C",
+                "echo C>C",
+            ]
+        )
+        == 0
+    )
+    assert (
+        main(
+            [
+                "stage",
+                "add",
+                "--run",
+                "-n",
+                "D-gen",
+                "-d",
+                "B",
+                "-d",
+                "C",
+                "-o",
+                "D",
+                "echo D>D",
+            ]
+        )
+        == 0
+    )
+    assert main(["stage", "add", "--run", "-n", "G-gen", "-o", "G", "echo G>G"]) == 0
+    assert (
+        main(["stage", "add", "--run", "-n", "F-gen", "-d", "G", "-o", "F", "echo F>F"])
+        == 0
     )
-    assert main(["run", "--single-stage", "-o", "G", "echo G>G"]) == 0
-    assert main(["run", "-n", "F-gen", "-d", "G", "-o", "F", "echo F>F"]) == 0
     assert (
         main(
             [
-                "run",
-                "--single-stage",
+                "stage",
+                "add",
+                "--run",
+                "-n",
+                "E-gen",
                 "-d",
                 "D",
                 "-d",
                 "F",
                 "-o",
                 "E",
                 "echo E>E",
@@ -79,49 +120,32 @@
     #     D
     #    /
     #   B
     #
     evaluation = dvc.reproduce(PROJECT_FILE + ":B-gen", downstream=True, force=True)
 
     assert len(evaluation) == 3
-    assert isinstance(evaluation[0], PipelineStage)
-    assert evaluation[0].relpath == PROJECT_FILE
-    assert evaluation[0].name == "B-gen"
-
-    assert isinstance(evaluation[1], PipelineStage)
-    assert evaluation[1].relpath == PROJECT_FILE
-    assert evaluation[1].name == "D-gen"
-
-    assert not isinstance(evaluation[2], PipelineStage)
-    assert evaluation[2].relpath == "E.dvc"
+    assert all(isinstance(stage, PipelineStage) for stage in evaluation)
+    assert all(stage.relpath == PROJECT_FILE for stage in evaluation)
+    assert [stage.name for stage in evaluation] == ["B-gen", "D-gen", "E-gen"]
 
     # B, C should be run (in any order) before D
     # See https://github.com/iterative/dvc/issues/3602
     evaluation = dvc.reproduce(PROJECT_FILE + ":A-gen", downstream=True, force=True)
 
     assert len(evaluation) == 5
-    assert isinstance(evaluation[0], PipelineStage)
-    assert evaluation[0].relpath == PROJECT_FILE
-    assert evaluation[0].name == "A-gen"
-
-    names = set()
-    for stage in evaluation[1:3]:
-        if isinstance(stage, PipelineStage):
-            assert stage.relpath == PROJECT_FILE
-            names.add(stage.name)
-        else:
-            names.add(stage.relpath)
-    assert names == {"B-gen", "C.dvc"}
-
-    assert isinstance(evaluation[3], PipelineStage)
-    assert evaluation[3].relpath == PROJECT_FILE
-    assert evaluation[3].name == "D-gen"
-
-    assert not isinstance(evaluation[4], PipelineStage)
-    assert evaluation[4].relpath == "E.dvc"
+    assert all(isinstance(stage, PipelineStage) for stage in evaluation)
+    assert all(stage.relpath == PROJECT_FILE for stage in evaluation)
+    assert [stage.name for stage in evaluation] == [
+        "A-gen",
+        M.any_of("B-gen", "C-gen"),
+        M.any_of("B-gen", "C-gen"),
+        "D-gen",
+        "E-gen",
+    ]
 
 
 def test_repro_when_cmd_changes(tmp_dir, dvc, run_copy, mocker):
     from dvc.dvcfile import ProjectFile
 
     tmp_dir.gen("foo", "foo")
     stage = run_copy("foo", "bar", name="copy-file")
@@ -132,15 +156,15 @@
 
     m = mocker.patch("dvc.stage.run.cmd_run", wraps=cmd_run)
     stage.cmd = "  ".join(stage.cmd.split())  # change cmd spacing by two
     ProjectFile(dvc, PROJECT_FILE)._dump_pipeline_file(stage)
 
     assert dvc.status([target]) == {target: ["changed command"]}
     assert dvc.reproduce(target)[0] == stage
-    m.assert_called_once_with(stage, checkpoint_func=None, dry=False, run_env=None)
+    m.assert_called_once_with(stage, dry=False, run_env=None)
 
 
 def test_repro_when_new_deps_is_added_in_dvcfile(tmp_dir, dvc, run_copy, copy_script):
     from dvc.dvcfile import load_file
 
     tmp_dir.gen({"foo": "foo", "bar": "bar"})
     stage = dvc.run(
```

### Comparing `dvc-3.0.0a0/tests/func/test_run_cache.py` & `dvc-3.0.0a1/tests/func/test_run_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_run_multistage.py` & `dvc-3.0.0a1/tests/func/test_run_multistage.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_run_single_stage.py` & `dvc-3.0.0a1/tests/func/test_run_single_stage.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,16 +14,15 @@
     ArgumentDuplicationError,
     CircularDependencyError,
     CyclicGraphError,
     OutputDuplicationError,
     OverlappingOutputPathsError,
     StagePathAsOutputError,
 )
-from dvc.fs import system
-from dvc.output import Output, OutputIsStageFileError
+from dvc.output import OutputIsStageFileError
 from dvc.stage import Stage
 from dvc.stage.exceptions import (
     StageFileAlreadyExistsError,
     StageFileBadNameError,
     StagePathNotDirectoryError,
     StagePathNotFoundError,
     StagePathOutsideError,
@@ -303,270 +302,14 @@
         deps=["append_foo.py"],
         outs=["foo"],
         cmd="python append_foo.py foo",
         single_stage=True,
     )
 
 
-def test_run_unprotect_outs_copy(tmp_dir, dvc, append_foo_script):
-    ret = main(["config", "cache.type", "copy"])
-    assert ret == 0
-
-    ret = main(
-        [
-            "run",
-            "-d",
-            "append_foo.py",
-            "-o",
-            "foo",
-            "--single-stage",
-            "python",
-            "append_foo.py",
-            "foo",
-        ]
-    )
-    assert ret == 0
-    assert os.access("foo", os.W_OK)
-    with open("foo", encoding="utf-8") as fd:
-        assert fd.read() == "foo"
-
-    ret = main(
-        [
-            "run",
-            "--force",
-            "--no-run-cache",
-            "--single-stage",
-            "-d",
-            "append_foo.py",
-            "-o",
-            "foo",
-            "python",
-            "append_foo.py",
-            "foo",
-        ]
-    )
-    assert ret == 0
-    assert os.access("foo", os.W_OK)
-    with open("foo", encoding="utf-8") as fd:
-        assert fd.read() == "foo"
-
-
-def test_run_unprotect_outs_symlink(tmp_dir, dvc, append_foo_script):
-    ret = main(["config", "cache.type", "symlink"])
-    assert ret == 0
-
-    assert ret == 0
-    ret = main(
-        [
-            "run",
-            "-d",
-            "append_foo.py",
-            "-o",
-            "foo",
-            "--single-stage",
-            "python",
-            "append_foo.py",
-            "foo",
-        ]
-    )
-    assert ret == 0
-
-    if os.name == "nt":
-        # NOTE: Windows symlink perms don't propagate to the target
-        assert os.access("foo", os.W_OK)
-    else:
-        assert not os.access("foo", os.W_OK)
-
-    assert system.is_symlink("foo")
-    with open("foo", encoding="utf-8") as fd:
-        assert fd.read() == "foo"
-
-    ret = main(
-        [
-            "run",
-            "--force",
-            "--no-run-cache",
-            "--single-stage",
-            "-d",
-            "append_foo.py",
-            "-o",
-            "foo",
-            "python",
-            "append_foo.py",
-            "foo",
-        ]
-    )
-    assert ret == 0
-
-    if os.name == "nt":
-        # NOTE: Windows symlink perms don't propagate to the target
-        assert os.access("foo", os.W_OK)
-    else:
-        assert not os.access("foo", os.W_OK)
-
-    assert system.is_symlink("foo")
-    with open("foo", encoding="utf-8") as fd:
-        assert fd.read() == "foo"
-
-
-def test_run_unprotect_outs_hardlink(tmp_dir, dvc, append_foo_script):
-    ret = main(["config", "cache.type", "hardlink"])
-    assert ret == 0
-
-    assert ret == 0
-    ret = main(
-        [
-            "run",
-            "-d",
-            "append_foo.py",
-            "-o",
-            "foo",
-            "--single-stage",
-            "python",
-            "append_foo.py",
-            "foo",
-        ]
-    )
-    assert ret == 0
-    assert not os.access("foo", os.W_OK)
-    assert system.is_hardlink("foo")
-    with open("foo", encoding="utf-8") as fd:
-        assert fd.read() == "foo"
-
-    ret = main(
-        [
-            "run",
-            "--force",
-            "--no-run-cache",
-            "--single-stage",
-            "-d",
-            "append_foo.py",
-            "-o",
-            "foo",
-            "python",
-            "append_foo.py",
-            "foo",
-        ]
-    )
-    assert ret == 0
-    assert not os.access("foo", os.W_OK)
-    assert system.is_hardlink("foo")
-    with open("foo", encoding="utf-8") as fd:
-        assert fd.read() == "foo"
-
-
-def test_cmd_run_overwrite(tmp_dir, dvc, copy_script):
-    # NOTE: using sleep() is a workaround  for filesystems
-    # with low mtime resolution. We have to use mtime since
-    # comparing mtime's is the only way to check that the stage
-    # file didn't change(size and inode in the first test down
-    # below don't change).
-    tmp_dir.gen({"foo": "foo", "bar": "bar"})
-    import time
-
-    ret = main(
-        [
-            "run",
-            "-d",
-            "foo",
-            "-d",
-            "copy.py",
-            "-o",
-            "out",
-            "--file",
-            "out.dvc",
-            "--single-stage",
-            "python",
-            "copy.py",
-            "foo",
-            "out",
-        ]
-    )
-    assert ret == 0
-
-    stage_mtime = os.path.getmtime("out.dvc")
-
-    time.sleep(1)
-
-    ret = main(
-        [
-            "run",
-            "-d",
-            "foo",
-            "-d",
-            "copy.py",
-            "--force",
-            "--no-run-cache",
-            "--single-stage",
-            "-o",
-            "out",
-            "--file",
-            "out.dvc",
-            "python",
-            "copy.py",
-            "foo",
-            "out",
-        ]
-    )
-    assert ret == 0
-
-    # NOTE: check that dvcfile was overwritten
-    assert stage_mtime != os.path.getmtime("out.dvc")
-    stage_mtime = os.path.getmtime("out.dvc")
-
-    time.sleep(1)
-
-    ret = main(
-        [
-            "run",
-            "--force",
-            "--single-stage",
-            "--file",
-            "out.dvc",
-            "-d",
-            "bar",
-            "cat bar",
-        ]
-    )
-    assert ret == 0
-
-    # NOTE: check that dvcfile was overwritten
-    assert stage_mtime != os.path.getmtime("out.dvc")
-
-
-class TestCmdRunCliMetrics:
-    def test_cached(self, dvc):
-        ret = main(
-            [
-                "run",
-                "-m",
-                "metrics.txt",
-                "--single-stage",
-                "echo test > metrics.txt",
-            ]
-        )
-        assert ret == 0
-        with open("metrics.txt", encoding="utf-8") as fd:
-            assert fd.read().rstrip() == "test"
-
-    def test_not_cached(self, dvc):
-        ret = main(
-            [
-                "run",
-                "-M",
-                "metrics.txt",
-                "--single-stage",
-                "echo test > metrics.txt",
-            ]
-        )
-        assert ret == 0
-        with open("metrics.txt", encoding="utf-8") as fd:
-            assert fd.read().rstrip() == "test"
-
-
 class TestCmdRunWorkingDirectory:
     def test_default_wdir_is_not_written(self, tmp_dir, dvc):
         stage = dvc.run(
             cmd="echo test > foo",
             outs=["foo"],
             wdir=".",
             single_stage=True,
@@ -661,70 +404,14 @@
     assert run_copy("foo", "out", single_stage=True) is not None
 
     Path("out").write_text("modification", encoding="utf-8")
     with pytest.raises(StageFileAlreadyExistsError):
         run_copy("foo", "out", force=False, single_stage=True)
 
 
-def test_run_commit(dvc):
-    fname = "test"
-    ret = main(
-        [
-            "run",
-            "-o",
-            fname,
-            "--no-commit",
-            "--single-stage",
-            "echo",
-            "test",
-            ">",
-            fname,
-        ]
-    )
-    assert ret == 0
-    assert os.path.isfile(fname)
-    assert not os.path.exists(dvc.cache.local.path)
-
-    ret = main(["commit", fname + ".dvc"])
-    assert ret == 0
-    assert os.path.isfile(fname)
-    assert len(list(dvc.cache.local.all())) == 1
-
-
-@pytest.mark.parametrize(
-    "outs_command",
-    [
-        "--outs-persist",
-        "--outs-persist-no-cache",
-    ],
-)
-def test_run_persist(tmp_dir, dvc, outs_command):
-    assert (
-        main(
-            [
-                "run",
-                "--single-stage",
-                "--always-changed",
-                outs_command,
-                "file",
-                "echo content>>file",
-            ]
-        )
-        == 0
-    )
-    d = (tmp_dir / "file.dvc").load_yaml()
-    assert d["outs"][0][Output.PARAM_PERSIST]
-
-    assert main(["repro", "file.dvc"]) == 0
-    assert (tmp_dir / "file").read_text() == "content\ncontent\n"
-
-    assert main(["remove", "file.dvc", "--outs"]) == 0
-    assert not (tmp_dir / "file").exists()
-
-
 def test_should_raise_on_overlapping_output_paths(tmp_dir, dvc, append_foo_script):
     tmp_dir.gen("data", {"foo": "foo", "bar": "bar"})
     ret = main(["add", "data"])
     assert ret == 0
 
     foo_file = os.path.join("data", "foo")
     with pytest.raises(OverlappingOutputPathsError) as err:
@@ -742,53 +429,14 @@
     assert (
         "overlap and are thus in the same tracked directory.\n"
         "To keep reproducibility, outputs should be in separate "
         "tracked directories or tracked individually." in error_output
     )
 
 
-@pytest.mark.parametrize(
-    "outs_command, first_expected, second_expected",
-    [
-        ("--outs", "foo\n", "bar\n"),
-        ("--outs-persist", "foo\n", "foo\nbar\n"),
-    ],
-)
-def test_rerun_with_same_outputs(
-    tmp_dir, dvc, outs_command, first_expected, second_expected
-):
-    assert (
-        main(
-            [
-                "run",
-                "--single-stage",
-                "--outs",
-                "foo",
-                "echo foo>foo",
-            ]
-        )
-        == 0
-    )
-    assert (tmp_dir / "foo").read_text() == first_expected
-    assert (
-        main(
-            [
-                "run",
-                outs_command,
-                "foo",
-                "--force",
-                "--single-stage",
-                "echo bar>>foo",
-            ]
-        )
-        == 0
-    )
-    assert (tmp_dir / "foo").read_text() == second_expected
-
-
 def test_should_not_checkout_upon_corrupted_local_hardlink_cache(
     mocker, tmp_dir, dvc, copy_script
 ):
     tmp_dir.gen("foo", "foo")
     dvc.cache.local.cache_types = ["hardlink"]
 
     stage = dvc.run(
```

### Comparing `dvc-3.0.0a0/tests/func/test_scm.py` & `dvc-3.0.0a1/tests/func/test_scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_scm_context.py` & `dvc-3.0.0a1/tests/func/test_scm_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_stage.py` & `dvc-3.0.0a1/tests/func/test_stage.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 import pytest
 
 from dvc.annotations import Annotation
 from dvc.dvcfile import SingleStageFile
 from dvc.exceptions import OutputDuplicationError
 from dvc.fs import LocalFileSystem
 from dvc.output import Output
-from dvc.repo import Repo, lock_repo
+from dvc.repo import Repo
 from dvc.stage import PipelineStage, Stage
-from dvc.stage.run import run_stage
 from dvc.stage.utils import compute_md5
 from dvc.utils import dict_md5
 from dvc.utils.serialize import dump_yaml, load_yaml
 from dvc.utils.strictyaml import YAMLValidationError
 
 
 def test_cmd_obj():
@@ -314,32 +313,14 @@
     assert (tmp_dir / stage.relpath).exists()
 
     with dvc.lock:
         stage.remove()
     assert not (tmp_dir / stage.relpath).exists()
 
 
-@pytest.mark.parametrize("checkpoint", [True, False])
-def test_stage_run_checkpoint(tmp_dir, dvc, mocker, checkpoint):
-    stage = Stage(dvc, "stage.dvc", cmd="mycmd arg1 arg2")
-    mocker.patch.object(stage, "save")
-
-    mock_cmd_run = mocker.patch("dvc.stage.run.cmd_run")
-    if checkpoint:
-        callback = mocker.Mock()
-    else:
-        callback = None
-
-    with lock_repo(dvc):
-        run_stage(stage, checkpoint_func=callback)
-    mock_cmd_run.assert_called_with(
-        stage, checkpoint_func=callback, dry=False, run_env=None
-    )
-
-
 def test_stage_add_duplicated_output(tmp_dir, dvc):
     tmp_dir.dvc_gen("foo", "foo")
     dvc.add("foo")
 
     with pytest.raises(
         OutputDuplicationError,
         match="Use `dvc remove foo.dvc` to stop tracking the overlapping output.",
```

### Comparing `dvc-3.0.0a0/tests/func/test_stage_load.py` & `dvc-3.0.0a1/tests/func/test_stage_load.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_state.py` & `dvc-3.0.0a1/tests/func/test_state.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_status.py` & `dvc-3.0.0a1/tests/func/test_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_unprotect.py` & `dvc-3.0.0a1/tests/func/test_unprotect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_update.py` & `dvc-3.0.0a1/tests/func/test_update.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_used_objs.py` & `dvc-3.0.0a1/tests/func/test_used_objs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_utils.py` & `dvc-3.0.0a1/tests/func/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_version.py` & `dvc-3.0.0a1/tests/func/test_version.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/test_virtual_directory.py` & `dvc-3.0.0a1/tests/func/test_virtual_directory.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/utils/test_hydra.py` & `dvc-3.0.0a1/tests/func/utils/test_hydra.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/func/utils/test_strict_yaml.py` & `dvc-3.0.0a1/tests/func/utils/test_strict_yaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/integration/plots/conftest.py` & `dvc-3.0.0a1/tests/integration/plots/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/integration/plots/test_plots.py` & `dvc-3.0.0a1/tests/integration/plots/test_plots.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/integration/plots/test_repo_plots_api.py` & `dvc-3.0.0a1/tests/integration/plots/test_repo_plots_api.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/integration/test_studio_live_experiments.py` & `dvc-3.0.0a1/tests/integration/test_studio_live_experiments.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/remotes/git_server.py` & `dvc-3.0.0a1/tests/remotes/git_server.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/remotes/user.key` & `dvc-3.0.0a1/tests/remotes/user.key`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/remotes_env.sample` & `dvc-3.0.0a1/tests/remotes_env.sample`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/scripts.py` & `dvc-3.0.0a1/tests/scripts.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/cli/test_main.py` & `dvc-3.0.0a1/tests/unit/cli/test_main.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/ls/test_ls.py` & `dvc-3.0.0a1/tests/unit/command/ls/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/ls/test_ls_colors.py` & `dvc-3.0.0a1/tests/unit/command/ls/test_ls_colors.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/test_add.py` & `dvc-3.0.0a1/tests/unit/command/test_add.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/test_cache.py` & `dvc-3.0.0a1/tests/unit/command/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/test_checkout.py` & `dvc-3.0.0a1/tests/unit/command/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/test_compat_flag.py` & `dvc-3.0.0a1/tests/unit/command/test_compat_flag.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/test_config.py` & `dvc-3.0.0a1/tests/unit/command/test_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/test_dag.py` & `dvc-3.0.0a1/tests/unit/command/test_dag.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/test_data_status.py` & `dvc-3.0.0a1/tests/unit/command/test_data_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/test_data_sync.py` & `dvc-3.0.0a1/tests/unit/command/test_data_sync.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/test_diff.py` & `dvc-3.0.0a1/tests/unit/command/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/test_experiments.py` & `dvc-3.0.0a1/tests/unit/command/test_experiments.py`

 * *Files 6% similar despite different names*

```diff
@@ -121,16 +121,14 @@
     default_arguments = {
         "params": [],
         "name": None,
         "queue": False,
         "run_all": False,
         "jobs": 1,
         "tmp_dir": False,
-        "checkpoint_resume": None,
-        "reset": False,
         "machine": None,
         "copy_paths": [],
         "message": None,
     }
     default_arguments.update(repro_arguments)
 
     cmd = CmdExperimentsRun(parse_args(["exp", "run"]))
@@ -184,14 +182,70 @@
         git_remote="origin",
         rev=["foo"],
         all_commits=True,
         num=-1,
     )
 
 
+@pytest.mark.parametrize(
+    "args,expected",
+    [
+        ([], "main:\n\tsha-a [exp-a]\n"),
+        (["--name-only"], "exp-a\n"),
+        (["--sha-only"], "sha-a\n"),
+    ],
+)
+def test_experiments_list_format(mocker, capsys, args, expected):
+    mocker.patch(
+        "dvc.repo.experiments.ls.ls",
+        return_value={
+            "main": [
+                ("exp-a", "sha-a"),
+            ]
+        },
+    )
+    raw_args = ["experiments", "list", *args]
+    cli_args = parse_args(raw_args)
+
+    cmd = cli_args.func(cli_args)
+
+    capsys.readouterr()
+    assert cmd.run() == 0
+    cap = capsys.readouterr()
+    assert cap.out == expected
+
+
+def test_experiments_list_remote(mocker, capsys):
+    mocker.patch(
+        "dvc.repo.experiments.ls.ls",
+        return_value={
+            "main": [
+                ("exp-a", None),
+            ]
+        },
+    )
+    cli_args = parse_args(["experiments", "list", "git_remote"])
+
+    cmd = cli_args.func(cli_args)
+
+    capsys.readouterr()
+    assert cmd.run() == 0
+    cap = capsys.readouterr()
+    assert cap.out == "main:\n\texp-a\n"
+
+    cli_args = parse_args(["experiments", "list", "git_remote", "--sha-only"])
+
+    cmd = cli_args.func(cli_args)
+
+    capsys.readouterr()
+
+    with pytest.raises(InvalidArgumentError):
+        cmd.run()
+
+
 def test_experiments_push(dvc, scm, mocker):
     cli_args = parse_args(
         [
             "experiments",
             "push",
             "origin",
             "experiment1",
```

### Comparing `dvc-3.0.0a0/tests/unit/command/test_gc.py` & `dvc-3.0.0a1/tests/unit/command/test_gc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/test_get.py` & `dvc-3.0.0a1/tests/unit/command/test_get.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/test_git_hook.py` & `dvc-3.0.0a1/tests/unit/command/test_git_hook.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/test_imp.py` & `dvc-3.0.0a1/tests/unit/command/test_imp.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/test_imp_url.py` & `dvc-3.0.0a1/tests/unit/command/test_imp_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/test_ls_url.py` & `dvc-3.0.0a1/tests/unit/command/test_ls_url.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/test_machine.py` & `dvc-3.0.0a1/tests/unit/command/test_machine.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/test_metrics.py` & `dvc-3.0.0a1/tests/unit/command/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/test_params.py` & `dvc-3.0.0a1/tests/unit/command/test_params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/test_plots.py` & `dvc-3.0.0a1/tests/unit/command/test_plots.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/test_queue.py` & `dvc-3.0.0a1/tests/unit/command/test_queue.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/test_repro.py` & `dvc-3.0.0a1/tests/unit/command/test_repro.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/test_stage.py` & `dvc-3.0.0a1/tests/unit/command/test_stage.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,16 +38,14 @@
             "--wdir",
             "wdir",
             "--force",
             "--outs-persist",
             "outs-persist",
             "--outs-persist-no-cache",
             "outs-persist-no-cache",
-            "--checkpoints",
-            "checkpoints",
             "--always-changed",
             "--params",
             "file:param1,param2",
             "--params",
             "param3",
             "--external",
             "--desc",
@@ -75,15 +73,14 @@
         metrics=["metrics"],
         metrics_no_cache=["metrics-no-cache"],
         plots=["plots"],
         plots_no_cache=["plots-no-cache"],
         wdir="wdir",
         outs_persist=["outs-persist"],
         outs_persist_no_cache=["outs-persist-no-cache"],
-        checkpoints=["checkpoints"],
         always_changed=True,
         external=True,
         desc="description",
         cmd=parsed_command,
         force=True,
     )
```

### Comparing `dvc-3.0.0a0/tests/unit/command/test_status.py` & `dvc-3.0.0a1/tests/unit/command/test_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/command/test_update.py` & `dvc-3.0.0a1/tests/unit/command/test_update.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/data/db/test_local.py` & `dvc-3.0.0a1/tests/unit/data/db/test_local.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/dependency/test_params.py` & `dvc-3.0.0a1/tests/unit/dependency/test_params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/fs/test_azure.py` & `dvc-3.0.0a1/tests/unit/fs/test_azure.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/fs/test_data.py` & `dvc-3.0.0a1/tests/unit/fs/test_data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/fs/test_dvc.py` & `dvc-3.0.0a1/tests/unit/fs/test_dvc.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/fs/test_dvc_info.py` & `dvc-3.0.0a1/tests/unit/fs/test_dvc_info.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/fs/test_fs.py` & `dvc-3.0.0a1/tests/unit/fs/test_fs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/fs/test_path.py` & `dvc-3.0.0a1/tests/unit/fs/test_path.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/fs/test_s3.py` & `dvc-3.0.0a1/tests/unit/fs/test_s3.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/fs/test_tree.py` & `dvc-3.0.0a1/tests/unit/fs/test_tree.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/machine/test_machine.py` & `dvc-3.0.0a1/tests/unit/machine/test_machine.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/output/test_load.py` & `dvc-3.0.0a1/tests/unit/output/test_load.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/output/test_local.py` & `dvc-3.0.0a1/tests/unit/output/test_local.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/output/test_output.py` & `dvc-3.0.0a1/tests/unit/output/test_output.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/remote/test_oss.py` & `dvc-3.0.0a1/tests/unit/remote/test_oss.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/remote/test_remote.py` & `dvc-3.0.0a1/tests/unit/remote/test_remote.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/remote/test_webdav.py` & `dvc-3.0.0a1/tests/unit/remote/test_webdav.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/remote/test_webhdfs.py` & `dvc-3.0.0a1/tests/unit/remote/test_webhdfs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/render/test_convert.py` & `dvc-3.0.0a1/tests/unit/render/test_convert.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/render/test_image_converter.py` & `dvc-3.0.0a1/tests/unit/render/test_image_converter.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/render/test_match.py` & `dvc-3.0.0a1/tests/unit/render/test_match.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/render/test_vega_converter.py` & `dvc-3.0.0a1/tests/unit/render/test_vega_converter.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/repo/experiments/queue/test_celery.py` & `dvc-3.0.0a1/tests/unit/repo/experiments/queue/test_celery.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/repo/experiments/queue/test_remove.py` & `dvc-3.0.0a1/tests/unit/repo/experiments/queue/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/repo/experiments/test_executor_status.py` & `dvc-3.0.0a1/tests/unit/repo/experiments/test_executor_status.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/repo/experiments/test_remove.py` & `dvc-3.0.0a1/tests/unit/repo/experiments/test_remove.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/repo/experiments/test_utils.py` & `dvc-3.0.0a1/tests/unit/repo/experiments/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/repo/plots/test_diff.py` & `dvc-3.0.0a1/tests/unit/repo/plots/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/repo/test_open_repo.py` & `dvc-3.0.0a1/tests/unit/repo/test_open_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/repo/test_repo.py` & `dvc-3.0.0a1/tests/unit/repo/test_repo.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/repo/test_reproduce.py` & `dvc-3.0.0a1/tests/unit/repo/test_reproduce.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/repo/test_scm_context.py` & `dvc-3.0.0a1/tests/unit/repo/test_scm_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/scm/test_scm.py` & `dvc-3.0.0a1/tests/unit/scm/test_scm.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/stage/test_cache.py` & `dvc-3.0.0a1/tests/unit/stage/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/stage/test_loader_pipeline_file.py` & `dvc-3.0.0a1/tests/unit/stage/test_loader_pipeline_file.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/stage/test_run.py` & `dvc-3.0.0a1/tests/unit/stage/test_run.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/stage/test_serialize_pipeline_file.py` & `dvc-3.0.0a1/tests/unit/stage/test_serialize_pipeline_file.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/stage/test_serialize_pipeline_lock.py` & `dvc-3.0.0a1/tests/unit/stage/test_serialize_pipeline_lock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/stage/test_utils.py` & `dvc-3.0.0a1/tests/unit/stage/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/test_analytics.py` & `dvc-3.0.0a1/tests/unit/test_analytics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/test_collect.py` & `dvc-3.0.0a1/tests/unit/test_collect.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/test_compare.py` & `dvc-3.0.0a1/tests/unit/test_compare.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/test_config.py` & `dvc-3.0.0a1/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/test_context.py` & `dvc-3.0.0a1/tests/unit/test_context.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/test_daemon.py` & `dvc-3.0.0a1/tests/unit/test_daemon.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/test_dvcfile.py` & `dvc-3.0.0a1/tests/unit/test_dvcfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/test_ignore.py` & `dvc-3.0.0a1/tests/unit/test_ignore.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/test_imports.py` & `dvc-3.0.0a1/tests/unit/test_imports.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/test_info.py` & `dvc-3.0.0a1/tests/unit/test_info.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/test_interpolate.py` & `dvc-3.0.0a1/tests/unit/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/test_lockfile.py` & `dvc-3.0.0a1/tests/unit/test_lockfile.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/test_logger.py` & `dvc-3.0.0a1/tests/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/test_metrics.py` & `dvc-3.0.0a1/tests/unit/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/test_params.py` & `dvc-3.0.0a1/tests/unit/test_params.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/test_pathspec_math.py` & `dvc-3.0.0a1/tests/unit/test_pathspec_math.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/test_progress.py` & `dvc-3.0.0a1/tests/unit/test_progress.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/test_rwlock.py` & `dvc-3.0.0a1/tests/unit/test_rwlock.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/test_tabular_data.py` & `dvc-3.0.0a1/tests/unit/test_tabular_data.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/test_updater.py` & `dvc-3.0.0a1/tests/unit/test_updater.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/ui/test_console.py` & `dvc-3.0.0a1/tests/unit/ui/test_console.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/ui/test_pager.py` & `dvc-3.0.0a1/tests/unit/ui/test_pager.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/ui/test_table.py` & `dvc-3.0.0a1/tests/unit/ui/test_table.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/utils/serialize/test_python.py` & `dvc-3.0.0a1/tests/unit/utils/serialize/test_python.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/utils/serialize/test_toml.py` & `dvc-3.0.0a1/tests/unit/utils/serialize/test_toml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/utils/serialize/test_yaml.py` & `dvc-3.0.0a1/tests/unit/utils/serialize/test_yaml.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/utils/test_cli_parse.py` & `dvc-3.0.0a1/tests/unit/utils/test_cli_parse.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/utils/test_collections.py` & `dvc-3.0.0a1/tests/unit/utils/test_collections.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/utils/test_executors.py` & `dvc-3.0.0a1/tests/unit/utils/test_executors.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/utils/test_fs.py` & `dvc-3.0.0a1/tests/unit/utils/test_fs.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/utils/test_humanize.py` & `dvc-3.0.0a1/tests/unit/utils/test_humanize.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/utils/test_studio.py` & `dvc-3.0.0a1/tests/unit/utils/test_studio.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/unit/utils/test_utils.py` & `dvc-3.0.0a1/tests/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/utils/__init__.py` & `dvc-3.0.0a1/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-3.0.0a0/tests/utils/asserts.py` & `dvc-3.0.0a1/tests/utils/asserts.py`

 * *Files identical despite different names*

