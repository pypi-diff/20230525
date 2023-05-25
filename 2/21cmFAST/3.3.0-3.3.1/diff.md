# Comparing `tmp/21cmFAST-3.3.0.tar.gz` & `tmp/21cmFAST-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "21cmFAST-3.3.0.tar", last modified: Thu May 18 15:40:54 2023, max compression
+gzip compressed data, was "21cmFAST-3.3.1.tar", last modified: Thu May 25 00:22:44 2023, max compression
```

## Comparing `21cmFAST-3.3.0.tar` & `21cmFAST-3.3.1.tar`

### file list

```diff
@@ -1,211 +1,211 @@
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2023-05-18 15:40:54.226727 21cmFAST-3.3.0/
--rw-r--r--   0 steven    (1000) steven    (1000)       93 2023-05-17 19:39:49.000000 21cmFAST-3.3.0/.bumpversion.cfg
--rw-r--r--   0 steven    (1000) steven    (1000)      761 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/.flake8
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2023-05-18 15:40:53.976727 21cmFAST-3.3.0/.github/
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2023-05-18 15:40:53.986727 21cmFAST-3.3.0/.github/workflows/
--rw-r--r--   0 steven    (1000) steven    (1000)      637 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/.github/workflows/merge-me.yaml
--rw-r--r--   0 steven    (1000) steven    (1000)      727 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/.github/workflows/merge-to-dev.yaml
--rw-r--r--   0 steven    (1000) steven    (1000)     2131 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 steven    (1000) steven    (1000)      365 2022-09-15 19:17:42.000000 21cmFAST-3.3.0/.github/workflows/tag-release.yaml
--rw-r--r--   0 steven    (1000) steven    (1000)     3299 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/.github/workflows/test_suite.yaml
--rw-r--r--   0 steven    (1000) steven    (1000)      593 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/.gitignore
--rw-r--r--   0 steven    (1000) steven    (1000)      243 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/.isort.cfg
--rw-r--r--   0 steven    (1000) steven    (1000)     1647 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/.pre-commit-config.yaml
--rw-r--r--   0 steven    (1000) steven    (1000)      380 2022-09-15 19:17:42.000000 21cmFAST-3.3.0/.readthedocs.yml
--rw-r--r--   0 steven    (1000) steven    (1000)      577 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/.travis.yml
--rw-r--r--   0 steven    (1000) steven    (1000)      178 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/AUTHORS.rst
--rw-r--r--   0 steven    (1000) steven    (1000)    13854 2023-05-18 15:40:02.000000 21cmFAST-3.3.0/CHANGELOG.rst
--rw-r--r--   0 steven    (1000) steven    (1000)     4263 2022-09-15 19:17:42.000000 21cmFAST-3.3.0/CONTRIBUTING.rst
--rw-r--r--   0 steven    (1000) steven    (1000)     9701 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/INSTALLATION.rst
--rw-r--r--   0 steven    (1000) steven    (1000)     1080 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/LICENSE
--rw-r--r--   0 steven    (1000) steven    (1000)    22239 2023-05-18 15:40:54.226727 21cmFAST-3.3.0/PKG-INFO
--rw-r--r--   0 steven    (1000) steven    (1000)     8189 2022-09-15 19:17:42.000000 21cmFAST-3.3.0/README.rst
--rw-r--r--   0 steven    (1000) steven    (1000)        6 2023-05-17 19:39:49.000000 21cmFAST-3.3.0/VERSION
--rwxr-xr-x   0 steven    (1000) steven    (1000)     2181 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/build_cffi.py
--rwxr-xr-x   0 steven    (1000) steven    (1000)      389 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/bump
--rw-r--r--   0 steven    (1000) steven    (1000)      590 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/changethelog.py
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2023-05-18 15:40:53.986727 21cmFAST-3.3.0/ci/
--rw-r--r--   0 steven    (1000) steven    (1000)      392 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/ci/macos-latest-env.yml
--rw-r--r--   0 steven    (1000) steven    (1000)      339 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/ci/ubuntu-latest-env.yml
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2023-05-18 15:40:53.996727 21cmFAST-3.3.0/devel/
--rw-r--r--   0 steven    (1000) steven    (1000)     1871 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/devel/TestFindHalos.py
--rw-r--r--   0 steven    (1000) steven    (1000)     3215 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/devel/estimated_mem_usage_plot.py
--rw-r--r--   0 steven    (1000) steven    (1000)      949 2022-09-15 19:17:42.000000 21cmFAST-3.3.0/devel/filter_valgrind.py
--rw-r--r--   0 steven    (1000) steven    (1000)    53949 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/devel/peak_memory_usage.png
--rw-r--r--   0 steven    (1000) steven    (1000)     1504 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/devel/prepare_gh_logs_for_diff.py
--rw-r--r--   0 steven    (1000) steven    (1000)      851 2022-09-15 19:17:42.000000 21cmFAST-3.3.0/devel/prepare_log_for_diff.py
--rw-r--r--   0 steven    (1000) steven    (1000)     1858 2022-09-15 19:17:42.000000 21cmFAST-3.3.0/devel/simulate_mcmc_memory_leak.py
--rw-r--r--   0 steven    (1000) steven    (1000)     1725 2022-09-15 19:17:42.000000 21cmFAST-3.3.0/devel/simulate_mcmc_memory_leak_lightcone.py
--rw-r--r--   0 steven    (1000) steven    (1000)     8186 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/devel/valgrind-python.supp
--rw-r--r--   0 steven    (1000) steven    (1000)     7183 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/devel/valgrind-suppress-all-but-c.supp
--rw-r--r--   0 steven    (1000) steven    (1000)   116373 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/devel/visualise_boxes_and_power.ipynb
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2023-05-18 15:40:54.006727 21cmFAST-3.3.0/docs/
--rw-r--r--   0 steven    (1000) steven    (1000)     5586 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/docs/Makefile
--rw-r--r--   0 steven    (1000) steven    (1000)       28 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/docs/authors.rst
--rw-r--r--   0 steven    (1000) steven    (1000)       30 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/docs/changelog.rst
--rw-r--r--   0 steven    (1000) steven    (1000)     2876 2023-04-12 17:40:59.000000 21cmFAST-3.3.0/docs/conf.py
--rw-r--r--   0 steven    (1000) steven    (1000)       71 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/docs/contributing.rst
--rw-r--r--   0 steven    (1000) steven    (1000)     6370 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/docs/design.rst
--rw-r--r--   0 steven    (1000) steven    (1000)      313 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/docs/environment.yaml
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2023-05-18 15:40:54.006727 21cmFAST-3.3.0/docs/faqs/
--rw-r--r--   0 steven    (1000) steven    (1000)      249 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/docs/faqs/installation_faq.rst
--rw-r--r--   0 steven    (1000) steven    (1000)     5163 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/docs/faqs/misc.rst
--rw-r--r--   0 steven    (1000) steven    (1000)      263 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/docs/index.rst
--rw-r--r--   0 steven    (1000) steven    (1000)       33 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/docs/installation.rst
--rw-r--r--   0 steven    (1000) steven    (1000)    22414 2022-09-15 19:17:42.000000 21cmFAST-3.3.0/docs/notes_for_developers.rst
--rw-r--r--   0 steven    (1000) steven    (1000)       27 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/docs/readme.rst
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2023-05-18 15:40:54.016727 21cmFAST-3.3.0/docs/reference/
--rw-r--r--   0 steven    (1000) steven    (1000)       87 2022-09-15 19:17:42.000000 21cmFAST-3.3.0/docs/reference/index.rst
--rw-r--r--   0 steven    (1000) steven    (1000)      259 2022-10-31 20:47:57.000000 21cmFAST-3.3.0/docs/reference/py21cmfast.rst
--rw-r--r--   0 steven    (1000) steven    (1000)      109 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/docs/spelling_wordlist.txt
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2023-05-18 15:40:54.016727 21cmFAST-3.3.0/docs/templates/
--rw-r--r--   0 steven    (1000) steven    (1000)      564 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/docs/templates/class.rst
--rw-r--r--   0 steven    (1000) steven    (1000)      727 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/docs/templates/module.rst
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2023-05-18 15:40:54.046727 21cmFAST-3.3.0/docs/tutorials/
--rw-r--r--   0 steven    (1000) steven    (1000)   758159 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/docs/tutorials/coeval_cubes.ipynb
--rw-r--r--   0 steven    (1000) steven    (1000)   297781 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/docs/tutorials/gather_data.ipynb
--rw-r--r--   0 steven    (1000) steven    (1000)   223452 2023-04-12 17:40:59.000000 21cmFAST-3.3.0/docs/tutorials/lightcones.ipynb
--rw-r--r--   0 steven    (1000) steven    (1000)  1977676 2023-04-12 17:40:59.000000 21cmFAST-3.3.0/docs/tutorials/mini-halos.ipynb
--rw-r--r--   0 steven    (1000) steven    (1000)   108656 2023-04-12 17:40:59.000000 21cmFAST-3.3.0/docs/tutorials/relative_velocities.ipynb
--rw-r--r--   0 steven    (1000) steven    (1000)      470 2022-09-15 19:17:42.000000 21cmFAST-3.3.0/docs/tutorials.rst
--rw-r--r--   0 steven    (1000) steven    (1000)     1593 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/environment_dev.yml
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2023-05-18 15:40:54.046727 21cmFAST-3.3.0/examples/
--rw-r--r--   0 steven    (1000) steven    (1000)      478 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/examples/runconfig_example.yml
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2023-05-18 15:40:54.066727 21cmFAST-3.3.0/joss-paper/
--rw-r--r--   0 steven    (1000) steven    (1000)       52 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/joss-paper/.gitignore
--rw-r--r--   0 steven    (1000) steven    (1000)     2104 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/joss-paper/Makefile
--rw-r--r--   0 steven    (1000) steven    (1000)    15040 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/joss-paper/apa.csl
--rw-r--r--   0 steven    (1000) steven    (1000)    98285 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/joss-paper/joss-logo.png
--rw-r--r--   0 steven    (1000) steven    (1000)    10730 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/joss-paper/latex.template
--rw-r--r--   0 steven    (1000) steven    (1000)   437687 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/joss-paper/lightcone.pdf
--rw-r--r--   0 steven    (1000) steven    (1000)     1427 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/joss-paper/make-example-plots.py
--rw-r--r--   0 steven    (1000) steven    (1000)     9102 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/joss-paper/paper.bib
--rw-r--r--   0 steven    (1000) steven    (1000)    14600 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/joss-paper/paper.md
--rw-r--r--   0 steven    (1000) steven    (1000)    10181 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/joss-paper/xH_history.pdf
--rw-r--r--   0 steven    (1000) steven    (1000)  1033531 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/joss-paper/yuxiangs-plot-small.png
--rw-r--r--   0 steven    (1000) steven    (1000)      308 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/pyproject.toml
--rw-r--r--   0 steven    (1000) steven    (1000)      448 2023-05-18 15:40:54.226727 21cmFAST-3.3.0/setup.cfg
--rw-r--r--   0 steven    (1000) steven    (1000)     3053 2023-04-12 17:40:59.000000 21cmFAST-3.3.0/setup.py
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2023-05-18 15:40:53.976727 21cmFAST-3.3.0/src/
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2023-05-18 15:40:54.076727 21cmFAST-3.3.0/src/21cmFAST.egg-info/
--rw-r--r--   0 steven    (1000) steven    (1000)    22239 2023-05-18 15:40:53.000000 21cmFAST-3.3.0/src/21cmFAST.egg-info/PKG-INFO
--rw-r--r--   0 steven    (1000) steven    (1000)     6154 2023-05-18 15:40:53.000000 21cmFAST-3.3.0/src/21cmFAST.egg-info/SOURCES.txt
--rw-r--r--   0 steven    (1000) steven    (1000)        1 2023-05-18 15:40:53.000000 21cmFAST-3.3.0/src/21cmFAST.egg-info/dependency_links.txt
--rw-r--r--   0 steven    (1000) steven    (1000)       49 2023-05-18 15:40:53.000000 21cmFAST-3.3.0/src/21cmFAST.egg-info/entry_points.txt
--rw-r--r--   0 steven    (1000) steven    (1000)        1 2022-09-15 20:29:07.000000 21cmFAST-3.3.0/src/21cmFAST.egg-info/not-zip-safe
--rw-r--r--   0 steven    (1000) steven    (1000)      402 2023-05-18 15:40:53.000000 21cmFAST-3.3.0/src/21cmFAST.egg-info/requires.txt
--rw-r--r--   0 steven    (1000) steven    (1000)       11 2023-05-18 15:40:53.000000 21cmFAST-3.3.0/src/21cmFAST.egg-info/top_level.txt
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2023-05-18 15:40:54.086727 21cmFAST-3.3.0/src/py21cmfast/
--rw-r--r--   0 steven    (1000) steven    (1000)     1414 2023-04-12 17:40:59.000000 21cmFAST-3.3.0/src/py21cmfast/__init__.py
--rw-r--r--   0 steven    (1000) steven    (1000)     3698 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/src/py21cmfast/_cfg.py
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2023-05-18 15:40:54.156727 21cmFAST-3.3.0/src/py21cmfast/_data/
--rw-r--r--   0 steven    (1000) steven    (1000) 13955167 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/src/py21cmfast/_data/Lyman_alpha_heating_table.dat
--rw-r--r--   0 steven    (1000) steven    (1000)     5998 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/_data/Transfers_z0.dat
--rw-r--r--   0 steven    (1000) steven    (1000)       60 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/_data/__init__.py
--rwxr-xr-x   0 steven    (1000) steven    (1000)      385 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/_data/kappa_eH_table.dat
--rwxr-xr-x   0 steven    (1000) steven    (1000)      284 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/_data/kappa_pH_table.dat
--rwxr-xr-x   0 steven    (1000) steven    (1000)    23554 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/_data/recfast_LCDM.dat
--rwxr-xr-x   0 steven    (1000) steven    (1000)     1162 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/_data/stellar_spectra.dat
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2023-05-18 15:40:54.166727 21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/
--rwxr-xr-x   0 steven    (1000) steven    (1000)    19811 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/log_xi_-1.0.dat
--rwxr-xr-x   0 steven    (1000) steven    (1000)    19641 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/log_xi_-1.3.dat
--rwxr-xr-x   0 steven    (1000) steven    (1000)    19444 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/log_xi_-1.6.dat
--rwxr-xr-x   0 steven    (1000) steven    (1000)    19318 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/log_xi_-2.0.dat
--rwxr-xr-x   0 steven    (1000) steven    (1000)    19181 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/log_xi_-2.3.dat
--rwxr-xr-x   0 steven    (1000) steven    (1000)    19021 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/log_xi_-2.6.dat
--rwxr-xr-x   0 steven    (1000) steven    (1000)    18794 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/log_xi_-3.0.dat
--rwxr-xr-x   0 steven    (1000) steven    (1000)    18612 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/log_xi_-3.3.dat
--rwxr-xr-x   0 steven    (1000) steven    (1000)    18522 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/log_xi_-3.6.dat
--rwxr-xr-x   0 steven    (1000) steven    (1000)    18812 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/log_xi_-4.0.dat
--rwxr-xr-x   0 steven    (1000) steven    (1000)    20412 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/xi_0.500.dat
--rwxr-xr-x   0 steven    (1000) steven    (1000)    20860 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/xi_0.900.dat
--rwxr-xr-x   0 steven    (1000) steven    (1000)    20267 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/xi_0.990.dat
--rwxr-xr-x   0 steven    (1000) steven    (1000)    18893 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/xi_0.999.dat
--rw-r--r--   0 steven    (1000) steven    (1000)     1129 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/_logging.py
--rw-r--r--   0 steven    (1000) steven    (1000)    57874 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/src/py21cmfast/_utils.py
--rw-r--r--   0 steven    (1000) steven    (1000)      160 2023-05-18 15:40:53.000000 21cmFAST-3.3.0/src/py21cmfast/_version.py
--rw-r--r--   0 steven    (1000) steven    (1000)     6528 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/src/py21cmfast/cache_tools.py
--rw-r--r--   0 steven    (1000) steven    (1000)    26037 2023-04-12 17:40:59.000000 21cmFAST-3.3.0/src/py21cmfast/cli.py
--rw-r--r--   0 steven    (1000) steven    (1000)    42820 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/src/py21cmfast/inputs.py
--rw-r--r--   0 steven    (1000) steven    (1000)    41737 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/src/py21cmfast/outputs.py
--rw-r--r--   0 steven    (1000) steven    (1000)    13303 2023-04-12 17:40:59.000000 21cmFAST-3.3.0/src/py21cmfast/plotting.py
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2023-05-18 15:40:54.186727 21cmFAST-3.3.0/src/py21cmfast/src/
--rw-r--r--   0 steven    (1000) steven    (1000)     7117 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/src/py21cmfast/src/21cmFAST.h
--rw-r--r--   0 steven    (1000) steven    (1000)    28640 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/src/py21cmfast/src/BrightnessTemperatureBox.c
--rw-r--r--   0 steven    (1000) steven    (1000)    10077 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/src/py21cmfast/src/Constants.h
--rw-r--r--   0 steven    (1000) steven    (1000)    19966 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/src/py21cmfast/src/FindHaloes.c
--rw-r--r--   0 steven    (1000) steven    (1000)    39664 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/src/py21cmfast/src/GenerateICs.c
--rw-r--r--   0 steven    (1000) steven    (1000)     3554 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/src/py21cmfast/src/Globals.h
--rw-r--r--   0 steven    (1000) steven    (1000)   102235 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/src/py21cmfast/src/IonisationBox.c
--rw-r--r--   0 steven    (1000) steven    (1000)    35206 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/src/py21cmfast/src/PerturbField.c
--rw-r--r--   0 steven    (1000) steven    (1000)    12437 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/src/py21cmfast/src/PerturbHaloField.c
--rw-r--r--   0 steven    (1000) steven    (1000)   152572 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/src/py21cmfast/src/SpinTemperatureBox.c
--rw-r--r--   0 steven    (1000) steven    (1000)    34665 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/src/py21cmfast/src/UsefulFunctions.c
--rwxr-xr-x   0 steven    (1000) steven    (1000)    13658 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/src/py21cmfast/src/bubble_helper_progs.c
--rw-r--r--   0 steven    (1000) steven    (1000)    10244 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/src/cexcept.h
--rw-r--r--   0 steven    (1000) steven    (1000)     5033 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/src/py21cmfast/src/dft.c
--rwxr-xr-x   0 steven    (1000) steven    (1000)    16857 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/src/elec_interp.c
--rw-r--r--   0 steven    (1000) steven    (1000)      571 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/src/exceptions.h
--rwxr-xr-x   0 steven    (1000) steven    (1000)    53301 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/src/py21cmfast/src/heating_helper_progs.c
--rw-r--r--   0 steven    (1000) steven    (1000)     4151 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/src/py21cmfast/src/indexing.c
--rw-r--r--   0 steven    (1000) steven    (1000)     4036 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/src/logger.h
--rw-r--r--   0 steven    (1000) steven    (1000)   170742 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/src/py21cmfast/src/ps.c
--rwxr-xr-x   0 steven    (1000) steven    (1000)    11214 2022-09-15 19:17:42.000000 21cmFAST-3.3.0/src/py21cmfast/src/recombinations.c
--rw-r--r--   0 steven    (1000) steven    (1000)   120866 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/src/py21cmfast/wrapper.py
--rw-r--r--   0 steven    (1000) steven    (1000)     1444 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/src/py21cmfast/yaml.py
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2023-05-18 15:40:54.196727 21cmFAST-3.3.0/tests/
--rw-r--r--   0 steven    (1000) steven    (1000)        0 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/tests/__init__.py
--rw-r--r--   0 steven    (1000) steven    (1000)     3689 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/conftest.py
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2023-05-18 15:40:54.196727 21cmFAST-3.3.0/tests/plots/
--rw-r--r--   0 steven    (1000) steven    (1000)    35933 2022-09-15 19:17:42.000000 21cmFAST-3.3.0/tests/plots/tests.test_integration_features.py--test_power_spectra_coeval[18-kwargs12].pdf
--rw-r--r--   0 steven    (1000) steven    (1000)    20090 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/produce_integration_test_data.py
--rw-r--r--   0 steven    (1000) steven    (1000)     1222 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/tests/test_cache_tools.py
--rw-r--r--   0 steven    (1000) steven    (1000)     4243 2022-09-15 19:17:42.000000 21cmFAST-3.3.0/tests/test_cli.py
--rw-r--r--   0 steven    (1000) steven    (1000)     1279 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/tests/test_config.py
-drwxr-xr-x   0 steven    (1000) steven    (1000)        0 2023-05-18 15:40:54.226727 21cmFAST-3.3.0/tests/test_data/
--rw-r--r--   0 steven    (1000) steven    (1000)     6160 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/tests/test_data/halo_field_data_halo_field.h5
--rw-r--r--   0 steven    (1000) steven    (1000)     8496 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/tests/test_data/perturb_field_data_highres.h5
--rw-r--r--   0 steven    (1000) steven    (1000)     8496 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/tests/test_data/perturb_field_data_linear.h5
--rw-r--r--   0 steven    (1000) steven    (1000)     8496 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/tests/test_data/perturb_field_data_no2lpt.h5
--rw-r--r--   0 steven    (1000) steven    (1000)     8496 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/tests/test_data/perturb_field_data_simple.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    18944 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_change_step_factor.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    18928 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_change_z_heat_max.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    21152 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_cmb_heating.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    19128 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_fast_fcoll_hiz.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    21264 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_fast_fcoll_lowz.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    18952 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_fftw_wisdom.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    21120 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_halo_field.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    27200 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_halo_field_mdz.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    21608 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_halo_field_mdz_highres.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    21896 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_inhomo.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    18960 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_interp_perturb_field.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    19064 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_larger_step_factor.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    21152 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_lyman_alpha_heating.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    21328 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_mdz_and_photoncons.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    27144 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_mdz_and_ts_fluct.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    27408 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_mdz_and_tsfluct_nthreads.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    27248 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_mdz_tsfluct_nthreads.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    18960 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_mdzeta.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    26520 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_mini_halos.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    27240 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_minihalos_no_tables.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    27232 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_minimize_mem.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    19072 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_mmin_in_mass.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    21064 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_nthreads.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    18960 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_perturb_high_res.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    21000 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_photoncons.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    22992 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_relvel.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    21088 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_rsd.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    14744 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_simple.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    27056 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_ts_fluct_no_tables.h5
--rw-r--r--   0 steven    (1000) steven    (1000)    26720 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_data/power_spectra_tsfluct.h5
--rw-r--r--   0 steven    (1000) steven    (1000)      458 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/tests/test_data_exists.py
--rw-r--r--   0 steven    (1000) steven    (1000)      615 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/tests/test_exceptions.py
--rw-r--r--   0 steven    (1000) steven    (1000)     3772 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_high_level_io.py
--rw-r--r--   0 steven    (1000) steven    (1000)     2818 2022-09-15 19:17:42.000000 21cmFAST-3.3.0/tests/test_initial_conditions.py
--rw-r--r--   0 steven    (1000) steven    (1000)     5179 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/tests/test_input_structs.py
--rw-r--r--   0 steven    (1000) steven    (1000)     7948 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_integration_features.py
--rw-r--r--   0 steven    (1000) steven    (1000)     4620 2022-09-15 19:17:42.000000 21cmFAST-3.3.0/tests/test_output_structs.py
--rw-r--r--   0 steven    (1000) steven    (1000)     2362 2023-05-05 17:15:48.000000 21cmFAST-3.3.0/tests/test_plotting.py
--rw-r--r--   0 steven    (1000) steven    (1000)      660 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/tests/test_spin_temp.py
--rw-r--r--   0 steven    (1000) steven    (1000)      108 2022-06-03 07:11:37.000000 21cmFAST-3.3.0/tests/test_tables.py
--rw-r--r--   0 steven    (1000) steven    (1000)    14710 2023-05-17 19:36:59.000000 21cmFAST-3.3.0/tests/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:22:44.292467 21cmFAST-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:22:44.252467 21cmFAST-3.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:22:44.256467 21cmFAST-3.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/.github/workflows/merge-me.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/.github/workflows/merge-to-dev.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/.github/workflows/tag-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/.github/workflows/test_suite.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13963 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/INSTALLATION.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22348 2023-05-25 00:22:44.292467 21cmFAST-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2181 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/build_cffi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      389 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/bump
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/changethelog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:22:44.256467 21cmFAST-3.3.1/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/ci/macos-latest-env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/ci/ubuntu-latest-env.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:22:44.256467 21cmFAST-3.3.1/devel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/devel/TestFindHalos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/devel/estimated_mem_usage_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/devel/filter_valgrind.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53949 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/devel/peak_memory_usage.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/devel/prepare_gh_logs_for_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/devel/prepare_log_for_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/devel/simulate_mcmc_memory_leak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/devel/simulate_mcmc_memory_leak_lightcone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/devel/valgrind-python.supp
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/devel/valgrind-suppress-all-but-c.supp
+-rw-r--r--   0 runner    (1001) docker     (123)   116373 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/devel/visualise_boxes_and_power.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:22:44.256467 21cmFAST-3.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/design.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:22:44.260467 21cmFAST-3.3.1/docs/faqs/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/faqs/installation_faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/faqs/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    22414 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/notes_for_developers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:22:44.260467 21cmFAST-3.3.1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/reference/py21cmfast.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/spelling_wordlist.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:22:44.260467 21cmFAST-3.3.1/docs/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/templates/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:22:44.264467 21cmFAST-3.3.1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)   758159 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/tutorials/coeval_cubes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   297781 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/tutorials/gather_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   223452 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/tutorials/lightcones.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1977676 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/tutorials/mini-halos.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   108656 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/tutorials/relative_velocities.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/docs/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/environment_dev.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:22:44.264467 21cmFAST-3.3.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/examples/runconfig_example.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:22:44.264467 21cmFAST-3.3.1/joss-paper/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/joss-paper/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/joss-paper/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    15040 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/joss-paper/apa.csl
+-rw-r--r--   0 runner    (1001) docker     (123)    98285 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/joss-paper/joss-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/joss-paper/latex.template
+-rw-r--r--   0 runner    (1001) docker     (123)   437687 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/joss-paper/lightcone.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/joss-paper/make-example-plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/joss-paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/joss-paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/joss-paper/xH_history.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)  1033531 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/joss-paper/yuxiangs-plot-small.png
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-25 00:22:44.292467 21cmFAST-3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:22:44.252467 21cmFAST-3.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:22:44.268467 21cmFAST-3.3.1/src/21cmFAST.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22348 2023-05-25 00:22:44.000000 21cmFAST-3.3.1/src/21cmFAST.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-05-25 00:22:44.000000 21cmFAST-3.3.1/src/21cmFAST.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 00:22:44.000000 21cmFAST-3.3.1/src/21cmFAST.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-25 00:22:44.000000 21cmFAST-3.3.1/src/21cmFAST.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 00:22:44.000000 21cmFAST-3.3.1/src/21cmFAST.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-25 00:22:44.000000 21cmFAST-3.3.1/src/21cmFAST.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 00:22:44.000000 21cmFAST-3.3.1/src/21cmFAST.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:22:44.268467 21cmFAST-3.3.1/src/py21cmfast/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:22:44.280467 21cmFAST-3.3.1/src/py21cmfast/_data/
+-rw-r--r--   0 runner    (1001) docker     (123) 13955167 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_data/Lyman_alpha_heating_table.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_data/Transfers_z0.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_data/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      385 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_data/kappa_eH_table.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      284 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_data/kappa_pH_table.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23554 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_data/recfast_LCDM.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1162 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_data/stellar_spectra.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:22:44.284467 21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19811 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/log_xi_-1.0.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19641 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/log_xi_-1.3.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19444 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/log_xi_-1.6.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19318 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/log_xi_-2.0.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19181 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/log_xi_-2.3.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19021 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/log_xi_-2.6.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18794 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/log_xi_-3.0.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18612 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/log_xi_-3.3.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18522 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/log_xi_-3.6.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18812 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/log_xi_-4.0.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20412 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/xi_0.500.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20860 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/xi_0.900.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20267 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/xi_0.990.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18893 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/xi_0.999.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57874 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-25 00:22:44.000000 21cmFAST-3.3.1/src/py21cmfast/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/cache_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26037 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42820 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41737 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13303 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:22:44.288467 21cmFAST-3.3.1/src/py21cmfast/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/src/21cmFAST.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28640 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/src/BrightnessTemperatureBox.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/src/Constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/src/FindHaloes.c
+-rw-r--r--   0 runner    (1001) docker     (123)    39664 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/src/GenerateICs.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/src/Globals.h
+-rw-r--r--   0 runner    (1001) docker     (123)   102235 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/src/IonisationBox.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35206 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/src/PerturbField.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/src/PerturbHaloField.c
+-rw-r--r--   0 runner    (1001) docker     (123)   152572 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/src/SpinTemperatureBox.c
+-rw-r--r--   0 runner    (1001) docker     (123)    34665 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/src/UsefulFunctions.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13658 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/src/bubble_helper_progs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/src/cexcept.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/src/dft.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16857 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/src/elec_interp.c
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/src/exceptions.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    53477 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/src/heating_helper_progs.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/src/indexing.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/src/logger.h
+-rw-r--r--   0 runner    (1001) docker     (123)   170742 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/src/ps.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11214 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/src/recombinations.c
+-rw-r--r--   0 runner    (1001) docker     (123)   120866 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/src/py21cmfast/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:22:44.288467 21cmFAST-3.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:22:44.288467 21cmFAST-3.3.1/tests/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)    35933 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/plots/tests.test_integration_features.py--test_power_spectra_coeval[18-kwargs12].pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    20090 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/produce_integration_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_cache_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 00:22:44.292467 21cmFAST-3.3.1/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/halo_field_data_halo_field.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/perturb_field_data_highres.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/perturb_field_data_linear.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/perturb_field_data_no2lpt.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/perturb_field_data_simple.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    18944 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_change_step_factor.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    18928 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_change_z_heat_max.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    21152 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_cmb_heating.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    19128 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_fast_fcoll_hiz.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    21264 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_fast_fcoll_lowz.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_fftw_wisdom.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    21120 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_halo_field.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    27200 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_halo_field_mdz.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    21608 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_halo_field_mdz_highres.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    21896 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_inhomo.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    18960 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_interp_perturb_field.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    19064 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_larger_step_factor.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    21152 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_lyman_alpha_heating.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    21328 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_mdz_and_photoncons.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    27144 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_mdz_and_ts_fluct.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    27408 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_mdz_and_tsfluct_nthreads.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    27248 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_mdz_tsfluct_nthreads.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    18960 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_mdzeta.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_mini_halos.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    27240 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_minihalos_no_tables.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    27232 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_minimize_mem.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    19072 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_mmin_in_mass.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    21064 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_nthreads.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    18960 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_perturb_high_res.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    21000 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_photoncons.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    22992 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_relvel.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    21088 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_rsd.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_simple.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    27056 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_ts_fluct_no_tables.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    26720 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data/power_spectra_tsfluct.h5
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_data_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_high_level_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_initial_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_input_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7948 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_integration_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_output_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_spin_temp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14710 2023-05-25 00:22:23.000000 21cmFAST-3.3.1/tests/test_wrapper.py
```

### Comparing `21cmFAST-3.3.0/.flake8` & `21cmFAST-3.3.1/.flake8`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/.github/workflows/merge-me.yaml` & `21cmFAST-3.3.1/.github/workflows/merge-me.yaml`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/.github/workflows/merge-to-dev.yaml` & `21cmFAST-3.3.1/.github/workflows/merge-to-dev.yaml`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/.github/workflows/publish-to-pypi.yaml` & `21cmFAST-3.3.1/.github/workflows/publish-to-pypi.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 name: Deploy to PyPI
 
 on: push
 
 jobs:
   build-n-publish:
     name: Deploy
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-latest
     if: "!contains(github.event.pull_request.labels.*.name, 'auto-pr')"
     steps:
       - uses: actions/checkout@master
       # https://github.com/ansible/pylibssh/blob/1e7b17f/.github/workflows/build-test-n-publish.yml#L146-L151
       - name: Get history and tags for SCM versioning to work
         run: |
           git fetch --prune --unshallow
           git fetch --depth=1 origin +refs/tags/*:refs/tags/*
           git describe --tags
           git describe --tags $(git rev-list --tags --max-count=1)
-      - name: Set up Python 3.7
+      - name: Set up Python 3.10
         uses: actions/setup-python@v1
         with:
-          python-version: 3.7
-      - name: Install pep517
+          python-version: "3.10"
+      - name: Install build
         run: |
-          python -m pip install pep517 --user
+          python -m pip install build
           python -m pip install setuptools_scm
           python setup.py --version
       - name: Create setuptools_scm env variable
         if: startsWith(github.ref, 'refs/tags/') != true
         shell: bash
         run: |
           wget https://gist.github.com/plaplant/0902f09e59166bac742bbd554f3cd2f9/raw/make_dev_version.sh -O ../make_dev_version.sh
           version=$(bash ../make_dev_version.sh)
           echo "SETUPTOOLS_SCM_PRETEND_VERSION=$version" >> $GITHUB_ENV
       - name: Build a source tarball
-        run: python -m pep517.build --source --out-dir dist .
+        run: python -m build --sdist .
+
       # deploy to Test PyPI on any push except when merging to production, since that will
       # already exist, and thus fail.
       - name: Publish distribution 📦 to Test PyPI
         if: ${{ !contains(github.ref, 'production') }}
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.test_pypi_password }}
```

### Comparing `21cmFAST-3.3.0/.github/workflows/test_suite.yaml` & `21cmFAST-3.3.1/.github/workflows/test_suite.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         run: |
           LOG_LEVEL=${{ env.log_level }} CFLAGS="-isysroot /Library/Developer/CommandLineTools/SDKs/MacOSX.sdk" pip install .
 
       - name: Run Tests
         run: |
           python -m pytest -n 2 -l --cov=py21cmfast --cov-config=.coveragerc -vv --cov-report xml:./coverage.xml --durations=25 ${{ env.extra_pytest_args }}
 
-      - uses: codecov/codecov-action@v2
+      - uses: codecov/codecov-action@v3
         if: matrix.os == 'ubuntu-latest' && success() && !contains(github.event.pull_request.labels.*.name, 'auto-pr')
         with:
           fail_ci_if_error: true
           verbose: true
           token: ${{ secrets.CODECOV_TOKEN }}
 
 # CC=$HOME/miniconda/envs/$ENV_NAME/bin/gcc
```

### Comparing `21cmFAST-3.3.0/.gitignore` & `21cmFAST-3.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/.pre-commit-config.yaml` & `21cmFAST-3.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/.travis.yml` & `21cmFAST-3.3.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/CHANGELOG.rst` & `21cmFAST-3.3.1/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 Changelog
 =========
 
 dev-version
 -----------
 
+v3.3.1 [24 May 2023]
+----------------------
+
+Fixed
+~~~~~
+
+* Compilation of C code for some compilers (#330)
+
 v3.3.0 [17 May 2023]
 ----------------------
 
 Internals
----------
+~~~~~~~~~
 
 * Refactored setting up of inputs to high-level functions so that there is less code
   repetition.
 
 Fixed
------
+~~~~~
 
 * Running with ``R_BUBBLE_MAX`` too large auto-fixes it to be ``BOX_LEN`` (#112)
 * Bug in calling ``clear_cache``.
 * Inconsistency in the way that the very highest redshift of an evolution is handled
   between low-level code (eg. ``spin_temperature()``) and high-level code (eg. ``run_coeval()``).
 
 
 Added
------
+~~~~~
 
 * New ``validate_all_inputs`` function that cross-references the four main input structs
   and ensures all the parameters make sense together. Mostly for internal use.
 * Ability to save/read directly from an open HDF5 File (#170)
 * An implementation of cloud-in-cell to more accurately redistribute the perturbed mass
   across all neighbouring cells instead of the previous nearest cell approach
 * Changed PhotonConsEndCalibz from z = 5 -> z = 3.5 to handle later reionisation
```

### Comparing `21cmFAST-3.3.0/CONTRIBUTING.rst` & `21cmFAST-3.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/INSTALLATION.rst` & `21cmFAST-3.3.1/INSTALLATION.rst`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/LICENSE` & `21cmFAST-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/PKG-INFO` & `21cmFAST-3.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 21cmFAST
-Version: 3.3.0
+Version: 3.3.1
 Summary: A semi-numerical cosmological simulation code for the 21cm signal
 Home-page: https://github.com/21cmFAST/21cmFAST
 Author: The 21cmFAST coredev team
 Author-email: 21cmfast.coredev@gmail.com
 License: MIT license
 Keywords: Epoch of Reionization,Cosmology
 Classifier: Development Status :: 5 - Production/Stable
@@ -192,34 +192,42 @@
 
 Changelog
 =========
 
 dev-version
 -----------
 
+v3.3.1 [24 May 2023]
+----------------------
+
+Fixed
+~~~~~
+
+* Compilation of C code for some compilers (#330)
+
 v3.3.0 [17 May 2023]
 ----------------------
 
 Internals
----------
+~~~~~~~~~
 
 * Refactored setting up of inputs to high-level functions so that there is less code
   repetition.
 
 Fixed
------
+~~~~~
 
 * Running with ``R_BUBBLE_MAX`` too large auto-fixes it to be ``BOX_LEN`` (#112)
 * Bug in calling ``clear_cache``.
 * Inconsistency in the way that the very highest redshift of an evolution is handled
   between low-level code (eg. ``spin_temperature()``) and high-level code (eg. ``run_coeval()``).
 
 
 Added
------
+~~~~~
 
 * New ``validate_all_inputs`` function that cross-references the four main input structs
   and ensures all the parameters make sense together. Mostly for internal use.
 * Ability to save/read directly from an open HDF5 File (#170)
 * An implementation of cloud-in-cell to more accurately redistribute the perturbed mass
   across all neighbouring cells instead of the previous nearest cell approach
 * Changed PhotonConsEndCalibz from z = 5 -> z = 3.5 to handle later reionisation
```

### Comparing `21cmFAST-3.3.0/README.rst` & `21cmFAST-3.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/build_cffi.py` & `21cmFAST-3.3.1/build_cffi.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/changethelog.py` & `21cmFAST-3.3.1/changethelog.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/devel/TestFindHalos.py` & `21cmFAST-3.3.1/devel/TestFindHalos.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/devel/estimated_mem_usage_plot.py` & `21cmFAST-3.3.1/devel/estimated_mem_usage_plot.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/devel/filter_valgrind.py` & `21cmFAST-3.3.1/devel/filter_valgrind.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/devel/peak_memory_usage.png` & `21cmFAST-3.3.1/devel/peak_memory_usage.png`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/devel/prepare_gh_logs_for_diff.py` & `21cmFAST-3.3.1/devel/prepare_gh_logs_for_diff.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/devel/prepare_log_for_diff.py` & `21cmFAST-3.3.1/devel/prepare_log_for_diff.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/devel/simulate_mcmc_memory_leak.py` & `21cmFAST-3.3.1/devel/simulate_mcmc_memory_leak.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/devel/simulate_mcmc_memory_leak_lightcone.py` & `21cmFAST-3.3.1/devel/simulate_mcmc_memory_leak_lightcone.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/devel/valgrind-python.supp` & `21cmFAST-3.3.1/devel/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/devel/valgrind-suppress-all-but-c.supp` & `21cmFAST-3.3.1/devel/valgrind-suppress-all-but-c.supp`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/devel/visualise_boxes_and_power.ipynb` & `21cmFAST-3.3.1/devel/visualise_boxes_and_power.ipynb`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/docs/Makefile` & `21cmFAST-3.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/docs/conf.py` & `21cmFAST-3.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/docs/design.rst` & `21cmFAST-3.3.1/docs/design.rst`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/docs/faqs/misc.rst` & `21cmFAST-3.3.1/docs/faqs/misc.rst`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/docs/notes_for_developers.rst` & `21cmFAST-3.3.1/docs/notes_for_developers.rst`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/docs/templates/class.rst` & `21cmFAST-3.3.1/docs/templates/class.rst`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/docs/templates/module.rst` & `21cmFAST-3.3.1/docs/templates/module.rst`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/docs/tutorials/coeval_cubes.ipynb` & `21cmFAST-3.3.1/docs/tutorials/coeval_cubes.ipynb`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/docs/tutorials/gather_data.ipynb` & `21cmFAST-3.3.1/docs/tutorials/gather_data.ipynb`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/docs/tutorials/lightcones.ipynb` & `21cmFAST-3.3.1/docs/tutorials/lightcones.ipynb`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/docs/tutorials/mini-halos.ipynb` & `21cmFAST-3.3.1/docs/tutorials/mini-halos.ipynb`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/docs/tutorials/relative_velocities.ipynb` & `21cmFAST-3.3.1/docs/tutorials/relative_velocities.ipynb`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/environment_dev.yml` & `21cmFAST-3.3.1/environment_dev.yml`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/joss-paper/Makefile` & `21cmFAST-3.3.1/joss-paper/Makefile`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/joss-paper/apa.csl` & `21cmFAST-3.3.1/joss-paper/apa.csl`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/joss-paper/joss-logo.png` & `21cmFAST-3.3.1/joss-paper/joss-logo.png`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/joss-paper/latex.template` & `21cmFAST-3.3.1/joss-paper/latex.template`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/joss-paper/lightcone.pdf` & `21cmFAST-3.3.1/joss-paper/lightcone.pdf`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/joss-paper/make-example-plots.py` & `21cmFAST-3.3.1/joss-paper/make-example-plots.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/joss-paper/paper.bib` & `21cmFAST-3.3.1/joss-paper/paper.bib`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/joss-paper/paper.md` & `21cmFAST-3.3.1/joss-paper/paper.md`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/joss-paper/xH_history.pdf` & `21cmFAST-3.3.1/joss-paper/xH_history.pdf`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/joss-paper/yuxiangs-plot-small.png` & `21cmFAST-3.3.1/joss-paper/yuxiangs-plot-small.png`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/setup.py` & `21cmFAST-3.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/21cmFAST.egg-info/PKG-INFO` & `21cmFAST-3.3.1/src/21cmFAST.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 21cmFAST
-Version: 3.3.0
+Version: 3.3.1
 Summary: A semi-numerical cosmological simulation code for the 21cm signal
 Home-page: https://github.com/21cmFAST/21cmFAST
 Author: The 21cmFAST coredev team
 Author-email: 21cmfast.coredev@gmail.com
 License: MIT license
 Keywords: Epoch of Reionization,Cosmology
 Classifier: Development Status :: 5 - Production/Stable
@@ -192,34 +192,42 @@
 
 Changelog
 =========
 
 dev-version
 -----------
 
+v3.3.1 [24 May 2023]
+----------------------
+
+Fixed
+~~~~~
+
+* Compilation of C code for some compilers (#330)
+
 v3.3.0 [17 May 2023]
 ----------------------
 
 Internals
----------
+~~~~~~~~~
 
 * Refactored setting up of inputs to high-level functions so that there is less code
   repetition.
 
 Fixed
------
+~~~~~
 
 * Running with ``R_BUBBLE_MAX`` too large auto-fixes it to be ``BOX_LEN`` (#112)
 * Bug in calling ``clear_cache``.
 * Inconsistency in the way that the very highest redshift of an evolution is handled
   between low-level code (eg. ``spin_temperature()``) and high-level code (eg. ``run_coeval()``).
 
 
 Added
------
+~~~~~
 
 * New ``validate_all_inputs`` function that cross-references the four main input structs
   and ensures all the parameters make sense together. Mostly for internal use.
 * Ability to save/read directly from an open HDF5 File (#170)
 * An implementation of cloud-in-cell to more accurately redistribute the perturbed mass
   across all neighbouring cells instead of the previous nearest cell approach
 * Changed PhotonConsEndCalibz from z = 5 -> z = 3.5 to handle later reionisation
```

### Comparing `21cmFAST-3.3.0/src/21cmFAST.egg-info/SOURCES.txt` & `21cmFAST-3.3.1/src/21cmFAST.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/__init__.py` & `21cmFAST-3.3.1/src/py21cmfast/__init__.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/_cfg.py` & `21cmFAST-3.3.1/src/py21cmfast/_cfg.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/_data/Lyman_alpha_heating_table.dat` & `21cmFAST-3.3.1/src/py21cmfast/_data/Lyman_alpha_heating_table.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/_data/Transfers_z0.dat` & `21cmFAST-3.3.1/src/py21cmfast/_data/Transfers_z0.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/_data/recfast_LCDM.dat` & `21cmFAST-3.3.1/src/py21cmfast/_data/recfast_LCDM.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/_data/stellar_spectra.dat` & `21cmFAST-3.3.1/src/py21cmfast/_data/stellar_spectra.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/log_xi_-1.0.dat` & `21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/log_xi_-1.0.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/log_xi_-1.3.dat` & `21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/log_xi_-1.3.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/log_xi_-1.6.dat` & `21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/log_xi_-1.6.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/log_xi_-2.0.dat` & `21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/log_xi_-2.0.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/log_xi_-2.3.dat` & `21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/log_xi_-2.3.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/log_xi_-2.6.dat` & `21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/log_xi_-2.6.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/log_xi_-3.0.dat` & `21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/log_xi_-3.0.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/log_xi_-3.3.dat` & `21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/log_xi_-3.3.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/log_xi_-3.6.dat` & `21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/log_xi_-3.6.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/log_xi_-4.0.dat` & `21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/log_xi_-4.0.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/xi_0.500.dat` & `21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/xi_0.500.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/xi_0.900.dat` & `21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/xi_0.900.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/xi_0.990.dat` & `21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/xi_0.990.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/_data/x_int_tables/xi_0.999.dat` & `21cmFAST-3.3.1/src/py21cmfast/_data/x_int_tables/xi_0.999.dat`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/_logging.py` & `21cmFAST-3.3.1/src/py21cmfast/_logging.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/_utils.py` & `21cmFAST-3.3.1/src/py21cmfast/_utils.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/cache_tools.py` & `21cmFAST-3.3.1/src/py21cmfast/cache_tools.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/cli.py` & `21cmFAST-3.3.1/src/py21cmfast/cli.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/inputs.py` & `21cmFAST-3.3.1/src/py21cmfast/inputs.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/outputs.py` & `21cmFAST-3.3.1/src/py21cmfast/outputs.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/plotting.py` & `21cmFAST-3.3.1/src/py21cmfast/plotting.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/src/21cmFAST.h` & `21cmFAST-3.3.1/src/py21cmfast/src/21cmFAST.h`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/src/BrightnessTemperatureBox.c` & `21cmFAST-3.3.1/src/py21cmfast/src/BrightnessTemperatureBox.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/src/Constants.h` & `21cmFAST-3.3.1/src/py21cmfast/src/Constants.h`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/src/FindHaloes.c` & `21cmFAST-3.3.1/src/py21cmfast/src/FindHaloes.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/src/GenerateICs.c` & `21cmFAST-3.3.1/src/py21cmfast/src/GenerateICs.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/src/Globals.h` & `21cmFAST-3.3.1/src/py21cmfast/src/Globals.h`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/src/IonisationBox.c` & `21cmFAST-3.3.1/src/py21cmfast/src/IonisationBox.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/src/PerturbField.c` & `21cmFAST-3.3.1/src/py21cmfast/src/PerturbField.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/src/PerturbHaloField.c` & `21cmFAST-3.3.1/src/py21cmfast/src/PerturbHaloField.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/src/SpinTemperatureBox.c` & `21cmFAST-3.3.1/src/py21cmfast/src/SpinTemperatureBox.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/src/UsefulFunctions.c` & `21cmFAST-3.3.1/src/py21cmfast/src/UsefulFunctions.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/src/bubble_helper_progs.c` & `21cmFAST-3.3.1/src/py21cmfast/src/bubble_helper_progs.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/src/cexcept.h` & `21cmFAST-3.3.1/src/py21cmfast/src/cexcept.h`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/src/dft.c` & `21cmFAST-3.3.1/src/py21cmfast/src/dft.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/src/elec_interp.c` & `21cmFAST-3.3.1/src/py21cmfast/src/elec_interp.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/src/exceptions.h` & `21cmFAST-3.3.1/src/py21cmfast/src/exceptions.h`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/src/heating_helper_progs.c` & `21cmFAST-3.3.1/src/py21cmfast/src/heating_helper_progs.c`

 * *Files 0% similar despite different names*

```diff
@@ -82,14 +82,16 @@
 
 double species_weighted_x_ray_cross_section(double nu, double x_e);
 
 // * Returns the maximum redshift at which a Lyn transition contributes to Lya flux at z * //
 float zmax(float z, int n);
 
 //Lyman-Alpha heating functions
+int find_nearest_point(double min, double max, int n, double value);
+int find_xyz_pos(int xpos, int ypos, int zpos, int len_yarr, int len_zarr);
 double interpolate_heating_efficiencies(double tk, double ts, double taugp, double *arrE);
 double Energy_Lya_heating(double Tk, double Ts, double tau_gp, int flag);
 
 int init_heat()
 {
     kappa_10(1.0,1);
     kappa_10_elec(1.0,1);
@@ -1373,14 +1375,32 @@
     }
     if (flag == 3) {
       ans = interpolate_heating_efficiencies(Tk, Ts, tau_gp, dEI); //For Injected Flux
     }
     return ans;
 }
 
+// Useful functions for effeciently navigating through the heating interpolation tables
+//find the nearest value
+int find_nearest_point(double min, double max, int n, double value){
+    int pos=0;
+    double dn = (max - min)/(n-1);
+    if (value<=(min+dn)) pos=0;              // ensures we are in the first point
+    else if (value>=max) pos = n-2;          // ensures we cannot exceed the maximum point
+    else pos = (int)floor((value - min)/dn); // round it down to ensure we are always either side of the cell boundary
+    return pos;
+}
+
+//find x-y-z position in an 1D array
+//x=Tk, y=Ts, z=Tau_GP
+int find_xyz_pos(int xpos, int ypos, int zpos, int len_yarr, int len_zarr){
+    int pxyz = xpos*len_yarr*len_zarr + ypos*len_zarr + zpos;
+    return pxyz;
+}
+
 
 //Tri-linear interpolation function for Lyman-alpha heating efficiencies
 double interpolate_heating_efficiencies(double tk, double ts, double taugp, double *arrE) {
     tk = log10(tk);
     // Check that the value doesn't exceed the bound of the table. If it does, set it to the edge value (do not interpolate)
     if(tk < Tk_min) {
         tk = Tk_min;
@@ -1401,31 +1421,14 @@
     if(taugp < taugp_min) {
         taugp = taugp_min;
     }
     if(taugp > taugp_max) {
         taugp = taugp_max;
     }
 
-    //find the nearest value
-    int find_nearest_point(double min, double max, int n, double value){
-        int pos=0;
-        double dn = (max - min)/(n-1);
-        if (value<=(min+dn)) pos=0;              // ensures we are in the first point
-        else if (value>=max) pos = n-2;          // ensures we cannot exceed the maximum point
-        else pos = (int)floor((value - min)/dn); // round it down to ensure we are always either side of the cell boundary
-        return pos;
-	}
-
-    //find x-y-z position in an 1D array
-    //x=Tk, y=Ts, z=Tau_GP
-    int find_xyz_pos(int xpos, int ypos, int zpos, int len_yarr, int len_zarr){
-        int pxyz = xpos*len_yarr*len_zarr + ypos*len_zarr + zpos;
-        return pxyz;
-    }
-
     int itk, its, itaugp, idec;
     itk = find_nearest_point(Tk_min, Tk_max, nT, tk);
     its = find_nearest_point(Ts_min, Ts_max, nT, ts);
     itaugp = find_nearest_point(taugp_min, taugp_max, ngp, taugp);
 
     idec = find_xyz_pos(itk, its, itaugp, nT, ngp);
```

### Comparing `21cmFAST-3.3.0/src/py21cmfast/src/indexing.c` & `21cmFAST-3.3.1/src/py21cmfast/src/indexing.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/src/logger.h` & `21cmFAST-3.3.1/src/py21cmfast/src/logger.h`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/src/ps.c` & `21cmFAST-3.3.1/src/py21cmfast/src/ps.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/src/recombinations.c` & `21cmFAST-3.3.1/src/py21cmfast/src/recombinations.c`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/wrapper.py` & `21cmFAST-3.3.1/src/py21cmfast/wrapper.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/src/py21cmfast/yaml.py` & `21cmFAST-3.3.1/src/py21cmfast/yaml.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/conftest.py` & `21cmFAST-3.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/plots/tests.test_integration_features.py--test_power_spectra_coeval[18-kwargs12].pdf` & `21cmFAST-3.3.1/tests/plots/tests.test_integration_features.py--test_power_spectra_coeval[18-kwargs12].pdf`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/produce_integration_test_data.py` & `21cmFAST-3.3.1/tests/produce_integration_test_data.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_cache_tools.py` & `21cmFAST-3.3.1/tests/test_cache_tools.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_cli.py` & `21cmFAST-3.3.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_config.py` & `21cmFAST-3.3.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/halo_field_data_halo_field.h5` & `21cmFAST-3.3.1/tests/test_data/halo_field_data_halo_field.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/perturb_field_data_highres.h5` & `21cmFAST-3.3.1/tests/test_data/perturb_field_data_highres.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/perturb_field_data_linear.h5` & `21cmFAST-3.3.1/tests/test_data/perturb_field_data_linear.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/perturb_field_data_no2lpt.h5` & `21cmFAST-3.3.1/tests/test_data/perturb_field_data_no2lpt.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/perturb_field_data_simple.h5` & `21cmFAST-3.3.1/tests/test_data/perturb_field_data_simple.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_change_step_factor.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_change_step_factor.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_change_z_heat_max.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_change_z_heat_max.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_cmb_heating.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_cmb_heating.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_fast_fcoll_hiz.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_fast_fcoll_hiz.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_fast_fcoll_lowz.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_fast_fcoll_lowz.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_fftw_wisdom.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_fftw_wisdom.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_halo_field.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_halo_field.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_halo_field_mdz.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_halo_field_mdz.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_halo_field_mdz_highres.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_halo_field_mdz_highres.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_inhomo.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_inhomo.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_interp_perturb_field.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_interp_perturb_field.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_larger_step_factor.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_larger_step_factor.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_lyman_alpha_heating.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_lyman_alpha_heating.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_mdz_and_photoncons.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_mdz_and_photoncons.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_mdz_and_ts_fluct.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_mdz_and_ts_fluct.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_mdz_and_tsfluct_nthreads.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_mdz_and_tsfluct_nthreads.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_mdz_tsfluct_nthreads.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_mdz_tsfluct_nthreads.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_mdzeta.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_mdzeta.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_mini_halos.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_mini_halos.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_minihalos_no_tables.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_minihalos_no_tables.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_minimize_mem.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_minimize_mem.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_mmin_in_mass.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_mmin_in_mass.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_nthreads.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_nthreads.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_perturb_high_res.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_perturb_high_res.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_photoncons.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_photoncons.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_relvel.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_relvel.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_rsd.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_rsd.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_simple.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_simple.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_ts_fluct_no_tables.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_ts_fluct_no_tables.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_data/power_spectra_tsfluct.h5` & `21cmFAST-3.3.1/tests/test_data/power_spectra_tsfluct.h5`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_exceptions.py` & `21cmFAST-3.3.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_high_level_io.py` & `21cmFAST-3.3.1/tests/test_high_level_io.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_initial_conditions.py` & `21cmFAST-3.3.1/tests/test_initial_conditions.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_input_structs.py` & `21cmFAST-3.3.1/tests/test_input_structs.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_integration_features.py` & `21cmFAST-3.3.1/tests/test_integration_features.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_output_structs.py` & `21cmFAST-3.3.1/tests/test_output_structs.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_plotting.py` & `21cmFAST-3.3.1/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_spin_temp.py` & `21cmFAST-3.3.1/tests/test_spin_temp.py`

 * *Files identical despite different names*

### Comparing `21cmFAST-3.3.0/tests/test_wrapper.py` & `21cmFAST-3.3.1/tests/test_wrapper.py`

 * *Files identical despite different names*

