# Comparing `tmp/c65faucet-1.0.53.tar.gz` & `tmp/c65faucet-1.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c65faucet-1.0.53.tar", last modified: Thu May 11 20:51:18 2023, max compression
+gzip compressed data, was "c65faucet-1.0.54.tar", last modified: Thu May 25 09:31:20 2023, max compression
```

## Comparing `c65faucet-1.0.53.tar` & `c65faucet-1.0.54.tar`

### file list

```diff
@@ -1,374 +1,373 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.352042 c65faucet-1.0.53/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-11 20:51:15.000000 c65faucet-1.0.53/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-11 20:51:15.000000 c65faucet-1.0.53/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-11 20:51:15.000000 c65faucet-1.0.53/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.296041 c65faucet-1.0.53/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-11 20:51:15.000000 c65faucet-1.0.53/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-11 20:51:15.000000 c65faucet-1.0.53/.github/renovate.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.300041 c65faucet-1.0.53/.github/workflows/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.300041 c65faucet-1.0.53/.github/workflows/disabled/
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-11 20:51:15.000000 c65faucet-1.0.53/.github/workflows/disabled/periodic.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-11 20:51:15.000000 c65faucet-1.0.53/.github/workflows/disabled/release-debian.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-11 20:51:15.000000 c65faucet-1.0.53/.github/workflows/release-docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-11 20:51:15.000000 c65faucet-1.0.53/.github/workflows/release-python.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-11 20:51:15.000000 c65faucet-1.0.53/.github/workflows/tests-codecheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-05-11 20:51:15.000000 c65faucet-1.0.53/.github/workflows/tests-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-05-11 20:51:15.000000 c65faucet-1.0.53/.github/workflows/tests-integration.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-11 20:51:15.000000 c65faucet-1.0.53/.github/workflows/tests-unit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-11 20:51:15.000000 c65faucet-1.0.53/.github/workflows/tests-yaml-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-11 20:51:15.000000 c65faucet-1.0.53/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-11 20:51:15.000000 c65faucet-1.0.53/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-11 20:51:15.000000 c65faucet-1.0.53/.renovaterc.json
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-11 20:51:15.000000 c65faucet-1.0.53/.stickler.yml
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-11 20:51:18.000000 c65faucet-1.0.53/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-11 20:51:15.000000 c65faucet-1.0.53/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 20:51:18.000000 c65faucet-1.0.53/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-11 20:51:15.000000 c65faucet-1.0.53/Dockerfile.faucet
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-11 20:51:15.000000 c65faucet-1.0.53/Dockerfile.fuzz-config
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-11 20:51:15.000000 c65faucet-1.0.53/Dockerfile.fuzz-packet
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-11 20:51:15.000000 c65faucet-1.0.53/Dockerfile.gauge
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-11 20:51:15.000000 c65faucet-1.0.53/Dockerfile.tests
--rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-05-11 20:51:15.000000 c65faucet-1.0.53/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-11 20:51:15.000000 c65faucet-1.0.53/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-11 20:51:18.352042 c65faucet-1.0.53/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-11 20:51:15.000000 c65faucet-1.0.53/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.300041 c65faucet-1.0.53/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-11 20:51:15.000000 c65faucet-1.0.53/adapters/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.288041 c65faucet-1.0.53/adapters/vendors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.300041 c65faucet-1.0.53/adapters/vendors/faucetagent/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-11 20:51:15.000000 c65faucet-1.0.53/adapters/vendors/faucetagent/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-11 20:51:15.000000 c65faucet-1.0.53/adapters/vendors/faucetagent/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-11 20:51:15.000000 c65faucet-1.0.53/adapters/vendors/faucetagent/docker-compose.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      694 2023-05-11 20:51:15.000000 c65faucet-1.0.53/adapters/vendors/faucetagent/example_client.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1142 2023-05-11 20:51:15.000000 c65faucet-1.0.53/adapters/vendors/faucetagent/gencerts.sh
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-11 20:51:15.000000 c65faucet-1.0.53/adapters/vendors/faucetagent/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.300041 c65faucet-1.0.53/adapters/vendors/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-11 20:51:15.000000 c65faucet-1.0.53/adapters/vendors/rabbitmq/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-11 20:51:15.000000 c65faucet-1.0.53/adapters/vendors/rabbitmq/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-11 20:51:15.000000 c65faucet-1.0.53/adapters/vendors/rabbitmq/docker-compose-rabbitmq.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-11 20:51:15.000000 c65faucet-1.0.53/adapters/vendors/rabbitmq/docker-compose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-11 20:51:15.000000 c65faucet-1.0.53/adapters/vendors/rabbitmq/example_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.300041 c65faucet-1.0.53/adapters/vendors/rabbitmq/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-11 20:51:15.000000 c65faucet-1.0.53/adapters/vendors/rabbitmq/hooks/pre_build
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-05-11 20:51:15.000000 c65faucet-1.0.53/adapters/vendors/rabbitmq/rabbit.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 20:51:15.000000 c65faucet-1.0.53/adapters/vendors/rabbitmq/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-11 20:51:15.000000 c65faucet-1.0.53/adapters/vendors/rabbitmq/test_rabbit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.304041 c65faucet-1.0.53/c65faucet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-11 20:51:18.000000 c65faucet-1.0.53/c65faucet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-05-11 20:51:18.000000 c65faucet-1.0.53/c65faucet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:51:18.000000 c65faucet-1.0.53/c65faucet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-11 20:51:18.000000 c65faucet-1.0.53/c65faucet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 20:51:18.000000 c65faucet-1.0.53/c65faucet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 20:51:18.000000 c65faucet-1.0.53/c65faucet.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-11 20:51:18.000000 c65faucet-1.0.53/c65faucet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 20:51:18.000000 c65faucet-1.0.53/c65faucet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.304041 c65faucet-1.0.53/clib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:15.000000 c65faucet-1.0.53/clib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      540 2023-05-11 20:51:15.000000 c65faucet-1.0.53/clib/clib_mininet_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34289 2023-05-11 20:51:15.000000 c65faucet-1.0.53/clib/clib_mininet_test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-05-11 20:51:15.000000 c65faucet-1.0.53/clib/clib_mininet_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    25032 2023-05-11 20:51:15.000000 c65faucet-1.0.53/clib/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-05-11 20:51:15.000000 c65faucet-1.0.53/clib/docker_host.py
--rw-r--r--   0 runner    (1001) docker     (123)    51086 2023-05-11 20:51:15.000000 c65faucet-1.0.53/clib/fakeoftable.py
--rw-r--r--   0 runner    (1001) docker     (123)   143546 2023-05-11 20:51:15.000000 c65faucet-1.0.53/clib/mininet_test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    35487 2023-05-11 20:51:15.000000 c65faucet-1.0.53/clib/mininet_test_base_topo.py
--rw-r--r--   0 runner    (1001) docker     (123)    28930 2023-05-11 20:51:15.000000 c65faucet-1.0.53/clib/mininet_test_topo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-05-11 20:51:15.000000 c65faucet-1.0.53/clib/mininet_test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-05-11 20:51:15.000000 c65faucet-1.0.53/clib/mininet_test_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-05-11 20:51:15.000000 c65faucet-1.0.53/clib/tcpdump_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)   118212 2023-05-11 20:51:15.000000 c65faucet-1.0.53/clib/valve_test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-11 20:51:15.000000 c65faucet-1.0.53/codecheck-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.308041 c65faucet-1.0.53/debian/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-11 20:51:15.000000 c65faucet-1.0.53/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-11 20:51:15.000000 c65faucet-1.0.53/debian/compat
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-11 20:51:15.000000 c65faucet-1.0.53/debian/control
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-11 20:51:15.000000 c65faucet-1.0.53/debian/copyright
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-11 20:51:15.000000 c65faucet-1.0.53/debian/faucet-all-in-one.install
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-11 20:51:15.000000 c65faucet-1.0.53/debian/faucet-docs.docs
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-11 20:51:15.000000 c65faucet-1.0.53/debian/faucet.default
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-11 20:51:15.000000 c65faucet-1.0.53/debian/faucet.install
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-11 20:51:15.000000 c65faucet-1.0.53/debian/faucet.postinst
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-11 20:51:15.000000 c65faucet-1.0.53/debian/faucet.service
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-11 20:51:15.000000 c65faucet-1.0.53/debian/gauge.default
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-11 20:51:15.000000 c65faucet-1.0.53/debian/gauge.install
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-11 20:51:15.000000 c65faucet-1.0.53/debian/gauge.postinst
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-11 20:51:15.000000 c65faucet-1.0.53/debian/gauge.service
--rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-05-11 20:51:15.000000 c65faucet-1.0.53/debian/rules
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.308041 c65faucet-1.0.53/debian/source/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 20:51:15.000000 c65faucet-1.0.53/debian/source/format
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-11 20:51:15.000000 c65faucet-1.0.53/debian/watch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.308041 c65faucet-1.0.53/docker/
--rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docker/fuzz_config.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docker/fuzz_packet.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1176 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docker/install-faucet.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1232 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docker/localtest.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      797 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docker/pip_deps.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docker/retrycmd.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     7205 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docker/runtests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      697 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docker/shard_tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docker-compose.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.312041 c65faucet-1.0.53/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.292041 c65faucet-1.0.53/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.312041 c65faucet-1.0.53/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/css/responsive-tables.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.312041 c65faucet-1.0.53/docs/_static/deployments/
--rw-r--r--   0 runner    (1001) docker     (123)    89120 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/deployments/ONF_Faucet_deploy1.png
--rw-r--r--   0 runner    (1001) docker     (123)   984943 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/deployments/nznog17-physical-network.jpg
--rw-r--r--   0 runner    (1001) docker     (123)  1106115 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/deployments/nznog17-virtual-network.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.316042 c65faucet-1.0.53/docs/_static/grafana-dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)    23629 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/grafana-dashboards/faucet_instrumentation.json
--rw-r--r--   0 runner    (1001) docker     (123)    22310 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/grafana-dashboards/faucet_inventory.json
--rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/grafana-dashboards/faucet_port_statistics.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.320042 c65faucet-1.0.53/docs/_static/images/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8466 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/images/8021X-conf-diagram.svg
--rw-r--r--   0 runner    (1001) docker     (123)    97737 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/images/faucet-architecture.svg
--rw-r--r--   0 runner    (1001) docker     (123)    23716 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/images/faucet-pipeline.png
--rw-r--r--   0 runner    (1001) docker     (123)    58351 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/images/faucet-pipeline.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/images/faucet-pipeline.txt
--rw-r--r--   0 runner    (1001) docker     (123)   136689 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/images/gauge-nznog17.png
--rw-r--r--   0 runner    (1001) docker     (123)   285918 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/images/gauge-snapshot1.png
--rw-r--r--   0 runner    (1001) docker     (123)   452164 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/images/gauge-snapshot2.png
--rw-r--r--   0 runner    (1001) docker     (123)   467326 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/images/gauge-snapshot3.png
--rw-r--r--   0 runner    (1001) docker     (123)    51732 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/images/tutorial-acls.svg
--rw-r--r--   0 runner    (1001) docker     (123)    77255 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/images/tutorial-bgp-routing.svg
--rw-r--r--   0 runner    (1001) docker     (123)    47652 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/images/tutorial-ivr.svg
--rw-r--r--   0 runner    (1001) docker     (123)   120062 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/images/tutorial-multi-root-stack.svg
--rw-r--r--   0 runner    (1001) docker     (123)    87114 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/images/tutorial-nfv-services.svg
--rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/images/tutorial-stack-loop.svg
--rw-r--r--   0 runner    (1001) docker     (123)    78230 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/images/tutorial-stack-tunnel.svg
--rw-r--r--   0 runner    (1001) docker     (123)    53594 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/images/tutorial-stack.svg
--rw-r--r--   0 runner    (1001) docker     (123)   109550 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/images/tutorial-stackwithivr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    59007 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/images/tutorial-static-routing.svg
--rw-r--r--   0 runner    (1001) docker     (123)   172474 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/images/tutorial-vlans.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.324041 c65faucet-1.0.53/docs/_static/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/tutorial/add_tagged_interface
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/tutorial/as_ns
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/tutorial/cleanup
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/tutorial/create_ns
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/tutorial/destroy_ns
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/_static/tutorial/inter_switch_link
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/architecture.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.324041 c65faucet-1.0.53/docs/autogen/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/autogen/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    40109 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14496 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/developer_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/external_resources.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/fuzzing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/monitoring.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.324041 c65faucet-1.0.53/docs/recipe_book/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/recipe_book/forwarding.rst
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/recipe_book/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/recipe_book/policy.rst
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/recipe_book/routing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.324041 c65faucet-1.0.53/docs/release_notes/
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/release_notes/1.7.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/release_notes/1.9.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.324041 c65faucet-1.0.53/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.324041 c65faucet-1.0.53/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/tutorials/acls.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/tutorials/conntrack.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18441 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/tutorials/first_time.rst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17927 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/tutorials/nfv_services.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15268 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/tutorials/routing.rst
--rw-r--r--   0 runner    (1001) docker     (123)    30053 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/tutorials/stacking.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/tutorials/vlans.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.324041 c65faucet-1.0.53/docs/vendors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.324041 c65faucet-1.0.53/docs/vendors/allied-telesis/
--rw-r--r--   0 runner    (1001) docker     (123)    14233 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/vendors/allied-telesis/README_Allied_Telesis.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.324041 c65faucet-1.0.53/docs/vendors/cisco/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9404 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/vendors/cisco/README_Cisco.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.324041 c65faucet-1.0.53/docs/vendors/hpe/
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/vendors/hpe/README_Aruba.rst
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/vendors/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.324041 c65faucet-1.0.53/docs/vendors/lagopus/
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/vendors/lagopus/README_Lagopus.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.328042 c65faucet-1.0.53/docs/vendors/northboundnetworks/
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/vendors/northboundnetworks/README_ZodiacFX.rst
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/vendors/northboundnetworks/README_ZodiacGX.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1292 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/vendors/northboundnetworks/conf-zodiac.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.328042 c65faucet-1.0.53/docs/vendors/noviflow/
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/vendors/noviflow/README_noviflow.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.328042 c65faucet-1.0.53/docs/vendors/ovs/
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/vendors/ovs/README_OVS-DPDK.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18223 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/vendors/ovs/faucet_ovs_test.png
--rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-05-11 20:51:15.000000 c65faucet-1.0.53/docs/vendors/ovs/faucet_testing_with_OVS_on_hardware.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.292041 c65faucet-1.0.53/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.328042 c65faucet-1.0.53/etc/default/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-11 20:51:15.000000 c65faucet-1.0.53/etc/default/faucet
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-11 20:51:15.000000 c65faucet-1.0.53/etc/default/gauge
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.328042 c65faucet-1.0.53/etc/faucet/
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-11 20:51:15.000000 c65faucet-1.0.53/etc/faucet/acls.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-11 20:51:15.000000 c65faucet-1.0.53/etc/faucet/faucet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-11 20:51:15.000000 c65faucet-1.0.53/etc/faucet/gauge.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-11 20:51:15.000000 c65faucet-1.0.53/etc/faucet/os_ken.conf
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-11 20:51:15.000000 c65faucet-1.0.53/etc/faucet/ryu.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.328042 c65faucet-1.0.53/etc/logrotate.d/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-11 20:51:15.000000 c65faucet-1.0.53/etc/logrotate.d/faucet
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-11 20:51:15.000000 c65faucet-1.0.53/etc/logrotate.d/gauge
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.328042 c65faucet-1.0.53/etc/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-11 20:51:15.000000 c65faucet-1.0.53/etc/prometheus/faucet.rules.yml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-11 20:51:15.000000 c65faucet-1.0.53/etc/prometheus/prometheus-docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-11 20:51:15.000000 c65faucet-1.0.53/etc/prometheus/prometheus.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.292041 c65faucet-1.0.53/etc/systemd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.328042 c65faucet-1.0.53/etc/systemd/system/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-11 20:51:15.000000 c65faucet-1.0.53/etc/systemd/system/faucet.service
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-11 20:51:15.000000 c65faucet-1.0.53/etc/systemd/system/gauge.service
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-11 20:51:15.000000 c65faucet-1.0.53/etc/systemd/system/prometheus.service
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.340042 c65faucet-1.0.53/faucet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5773 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35363 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/acl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2276 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/check_faucet_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    14246 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/config_parser_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    71188 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/dp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/faucet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/faucet_bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/faucet_dot1x.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/faucet_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/faucet_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11424 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/faucet_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/faucet_pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7755 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/fctl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/gauge.py
--rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/gauge_influx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/gauge_pollers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/gauge_prom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    31120 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/port.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/prom_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/router.py
--rw-r--r--   0 runner    (1001) docker     (123)    19588 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/tfm_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    73345 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/valve.py
--rw-r--r--   0 runner    (1001) docker     (123)    30131 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/valve_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/valve_coprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/valve_lldp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/valve_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    42091 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/valve_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/valve_of_old.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/valve_outonly.py
--rw-r--r--   0 runner    (1001) docker     (123)    28984 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/valve_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/valve_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    49835 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/valve_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/valve_ryuapp.py
--rw-r--r--   0 runner    (1001) docker     (123)    18431 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/valve_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/valve_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    30701 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/valve_switch_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)    52744 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/valve_switch_standalone.py
--rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/valve_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/valve_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18634 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/valves_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    26043 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/vlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-11 20:51:15.000000 c65faucet-1.0.53/faucet/watcher_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-11 20:51:15.000000 c65faucet-1.0.53/fuzz-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.340042 c65faucet-1.0.53/git-hook/
--rwxr-xr-x   0 runner    (1001) docker     (123)      456 2023-05-11 20:51:15.000000 c65faucet-1.0.53/git-hook/pre-commit
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-11 20:51:15.000000 c65faucet-1.0.53/helper-funcs
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-11 20:51:15.000000 c65faucet-1.0.53/hw_switch_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.344042 c65faucet-1.0.53/ofctl_rest/
--rw-r--r--   0 runner    (1001) docker     (123)    27150 2023-05-11 20:51:15.000000 c65faucet-1.0.53/ofctl_rest/ofctl_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-05-11 20:51:15.000000 c65faucet-1.0.53/ofctl_rest/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-11 20:51:15.000000 c65faucet-1.0.53/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-11 20:51:18.356042 c65faucet-1.0.53/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3802 2023-05-11 20:51:15.000000 c65faucet-1.0.53/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-11 20:51:15.000000 c65faucet-1.0.53/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.344042 c65faucet-1.0.53/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.344042 c65faucet-1.0.53/tests/codecheck/
--rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/codecheck/flake8.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/codecheck/min_pylint.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/codecheck/pylint.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      342 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/codecheck/pytype.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      701 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/codecheck/src_files.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.292041 c65faucet-1.0.53/tests/generative/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.292041 c65faucet-1.0.53/tests/generative/fuzzer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.344042 c65faucet-1.0.53/tests/generative/fuzzer/config/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/config/config.dict
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.344042 c65faucet-1.0.53/tests/generative/fuzzer/config/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/config/examples/ex0
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/config/fuzz_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/config/generate_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.344042 c65faucet-1.0.53/tests/generative/fuzzer/packet/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/display_packet_crash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.348042 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/aoe.ex1
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/arp.ex1
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/arp.ex2
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/asap.ex1
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/asap.ex2
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/diameter.ex1
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/dns.ex1
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/dns.ex2
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/http.ex1
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/http.ex2
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/icmp.ex1
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/icmp.ex2
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/icmp.ex3
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/icmp.ex4
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/igmpv2.ex1
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/ipv4.ex1
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/ipv6.ex1
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/irc.ex1
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/irc.ex2
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/irc.ex3
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/lacp.ex1
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/msger.ex1
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/packet.dict
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/tcp.ex1
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/tcp.ex2
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/tcp.ex3
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/tcp.ex4
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/tcp.ex5
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/udp.ex1
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/udp.ex2
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/udp.ex3
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/udp.ex4
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/fake_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/fuzzer/packet/fuzz_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.348042 c65faucet-1.0.53/tests/generative/integration/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2304 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/integration/fault_tolerance_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    18304 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/integration/fault_tolerance_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.348042 c65faucet-1.0.53/tests/generative/unit/
--rwxr-xr-x   0 runner    (1001) docker     (123)    12779 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/generative/unit/test_topology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.352042 c65faucet-1.0.53/tests/integration/
--rwxr-xr-x   0 runner    (1001) docker     (123)      565 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/integration/mininet_main.py
--rw-r--r--   0 runner    (1001) docker     (123)   157767 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/integration/mininet_multidp_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)   308688 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/integration/mininet_tests.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      574 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/run_unit_tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      244 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/sysctls_for_tests.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.292041 c65faucet-1.0.53/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.352042 c65faucet-1.0.53/tests/unit/clib/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8815 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/unit/clib/test_topo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.352042 c65faucet-1.0.53/tests/unit/faucet/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10401 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/unit/faucet/test_check_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   134114 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/unit/faucet/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6666 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/unit/faucet/test_fctl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1519 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/unit/faucet/test_main.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5773 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/unit/faucet/test_port.py
--rw-r--r--   0 runner    (1001) docker     (123)    31562 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/unit/faucet/test_valve.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    39651 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/unit/faucet/test_valve_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4960 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/unit/faucet/test_valve_dot1x.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5875 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/unit/faucet/test_valve_egress.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2968 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/unit/faucet/test_valve_of.py
--rw-r--r--   0 runner    (1001) docker     (123)   154810 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/unit/faucet/test_valve_stack.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2770 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/unit/faucet/test_valveapp_smoke.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9217 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/unit/faucet/test_vlan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.352042 c65faucet-1.0.53/tests/unit/gauge/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5590 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/unit/gauge/test_config_gauge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36917 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/unit/gauge/test_gauge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1516 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/unit/gauge/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 20:51:18.352042 c65faucet-1.0.53/tests/unit/packaging/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5501 2023-05-11 20:51:15.000000 c65faucet-1.0.53/tests/unit/packaging/test_packaging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.624098 c65faucet-1.0.54/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-25 09:30:45.000000 c65faucet-1.0.54/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-25 09:30:45.000000 c65faucet-1.0.54/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 09:30:45.000000 c65faucet-1.0.54/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.588097 c65faucet-1.0.54/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-25 09:30:45.000000 c65faucet-1.0.54/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-25 09:30:45.000000 c65faucet-1.0.54/.github/renovate.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.588097 c65faucet-1.0.54/.github/workflows/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.588097 c65faucet-1.0.54/.github/workflows/disabled/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-25 09:30:45.000000 c65faucet-1.0.54/.github/workflows/disabled/periodic.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-25 09:30:45.000000 c65faucet-1.0.54/.github/workflows/disabled/release-debian.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-25 09:30:45.000000 c65faucet-1.0.54/.github/workflows/release-docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-25 09:30:45.000000 c65faucet-1.0.54/.github/workflows/release-python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-25 09:30:45.000000 c65faucet-1.0.54/.github/workflows/tests-codecheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-05-25 09:30:45.000000 c65faucet-1.0.54/.github/workflows/tests-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-05-25 09:30:45.000000 c65faucet-1.0.54/.github/workflows/tests-integration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-25 09:30:45.000000 c65faucet-1.0.54/.github/workflows/tests-unit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-25 09:30:45.000000 c65faucet-1.0.54/.github/workflows/tests-yaml-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-25 09:30:45.000000 c65faucet-1.0.54/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-25 09:30:45.000000 c65faucet-1.0.54/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-25 09:30:45.000000 c65faucet-1.0.54/.renovaterc.json
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-25 09:31:20.000000 c65faucet-1.0.54/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-25 09:30:45.000000 c65faucet-1.0.54/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-25 09:31:20.000000 c65faucet-1.0.54/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-25 09:30:45.000000 c65faucet-1.0.54/Dockerfile.faucet
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-25 09:30:45.000000 c65faucet-1.0.54/Dockerfile.fuzz-config
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-25 09:30:45.000000 c65faucet-1.0.54/Dockerfile.fuzz-packet
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-25 09:30:45.000000 c65faucet-1.0.54/Dockerfile.gauge
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-25 09:30:45.000000 c65faucet-1.0.54/Dockerfile.tests
+-rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-05-25 09:30:45.000000 c65faucet-1.0.54/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-25 09:30:45.000000 c65faucet-1.0.54/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-25 09:31:20.624098 c65faucet-1.0.54/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-25 09:30:45.000000 c65faucet-1.0.54/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.588097 c65faucet-1.0.54/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-25 09:30:45.000000 c65faucet-1.0.54/adapters/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.580097 c65faucet-1.0.54/adapters/vendors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.588097 c65faucet-1.0.54/adapters/vendors/faucetagent/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-25 09:30:45.000000 c65faucet-1.0.54/adapters/vendors/faucetagent/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-25 09:30:45.000000 c65faucet-1.0.54/adapters/vendors/faucetagent/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-25 09:30:45.000000 c65faucet-1.0.54/adapters/vendors/faucetagent/docker-compose.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      694 2023-05-25 09:30:45.000000 c65faucet-1.0.54/adapters/vendors/faucetagent/example_client.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1142 2023-05-25 09:30:45.000000 c65faucet-1.0.54/adapters/vendors/faucetagent/gencerts.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-25 09:30:45.000000 c65faucet-1.0.54/adapters/vendors/faucetagent/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.588097 c65faucet-1.0.54/adapters/vendors/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-25 09:30:45.000000 c65faucet-1.0.54/adapters/vendors/rabbitmq/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-25 09:30:45.000000 c65faucet-1.0.54/adapters/vendors/rabbitmq/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-25 09:30:45.000000 c65faucet-1.0.54/adapters/vendors/rabbitmq/docker-compose-rabbitmq.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-25 09:30:45.000000 c65faucet-1.0.54/adapters/vendors/rabbitmq/docker-compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-25 09:30:45.000000 c65faucet-1.0.54/adapters/vendors/rabbitmq/example_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.588097 c65faucet-1.0.54/adapters/vendors/rabbitmq/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-25 09:30:45.000000 c65faucet-1.0.54/adapters/vendors/rabbitmq/hooks/pre_build
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-05-25 09:30:45.000000 c65faucet-1.0.54/adapters/vendors/rabbitmq/rabbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 09:30:45.000000 c65faucet-1.0.54/adapters/vendors/rabbitmq/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-25 09:30:45.000000 c65faucet-1.0.54/adapters/vendors/rabbitmq/test_rabbit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.592097 c65faucet-1.0.54/c65faucet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-25 09:31:20.000000 c65faucet-1.0.54/c65faucet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-05-25 09:31:20.000000 c65faucet-1.0.54/c65faucet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:31:20.000000 c65faucet-1.0.54/c65faucet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-25 09:31:20.000000 c65faucet-1.0.54/c65faucet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:31:20.000000 c65faucet-1.0.54/c65faucet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 09:31:20.000000 c65faucet-1.0.54/c65faucet.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-25 09:31:20.000000 c65faucet-1.0.54/c65faucet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 09:31:20.000000 c65faucet-1.0.54/c65faucet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.592097 c65faucet-1.0.54/clib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:30:45.000000 c65faucet-1.0.54/clib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      540 2023-05-25 09:30:45.000000 c65faucet-1.0.54/clib/clib_mininet_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35493 2023-05-25 09:30:45.000000 c65faucet-1.0.54/clib/clib_mininet_test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-05-25 09:30:45.000000 c65faucet-1.0.54/clib/clib_mininet_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25032 2023-05-25 09:30:45.000000 c65faucet-1.0.54/clib/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-05-25 09:30:45.000000 c65faucet-1.0.54/clib/docker_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51086 2023-05-25 09:30:45.000000 c65faucet-1.0.54/clib/fakeoftable.py
+-rw-r--r--   0 runner    (1001) docker     (123)   143186 2023-05-25 09:30:45.000000 c65faucet-1.0.54/clib/mininet_test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34950 2023-05-25 09:30:45.000000 c65faucet-1.0.54/clib/mininet_test_base_topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30928 2023-05-25 09:30:45.000000 c65faucet-1.0.54/clib/mininet_test_topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-05-25 09:30:45.000000 c65faucet-1.0.54/clib/mininet_test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-05-25 09:30:45.000000 c65faucet-1.0.54/clib/mininet_test_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-05-25 09:30:45.000000 c65faucet-1.0.54/clib/tcpdump_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118212 2023-05-25 09:30:45.000000 c65faucet-1.0.54/clib/valve_test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 09:30:45.000000 c65faucet-1.0.54/codecheck-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.596097 c65faucet-1.0.54/debian/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-25 09:30:45.000000 c65faucet-1.0.54/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-25 09:30:45.000000 c65faucet-1.0.54/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-25 09:30:45.000000 c65faucet-1.0.54/debian/control
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-25 09:30:45.000000 c65faucet-1.0.54/debian/copyright
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-25 09:30:45.000000 c65faucet-1.0.54/debian/faucet-all-in-one.install
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 09:30:45.000000 c65faucet-1.0.54/debian/faucet-docs.docs
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-25 09:30:45.000000 c65faucet-1.0.54/debian/faucet.default
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-25 09:30:45.000000 c65faucet-1.0.54/debian/faucet.install
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-25 09:30:45.000000 c65faucet-1.0.54/debian/faucet.postinst
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-25 09:30:45.000000 c65faucet-1.0.54/debian/faucet.service
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-25 09:30:45.000000 c65faucet-1.0.54/debian/gauge.default
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-25 09:30:45.000000 c65faucet-1.0.54/debian/gauge.install
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-25 09:30:45.000000 c65faucet-1.0.54/debian/gauge.postinst
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-25 09:30:45.000000 c65faucet-1.0.54/debian/gauge.service
+-rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-05-25 09:30:45.000000 c65faucet-1.0.54/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.596097 c65faucet-1.0.54/debian/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 09:30:45.000000 c65faucet-1.0.54/debian/source/format
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-25 09:30:45.000000 c65faucet-1.0.54/debian/watch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.596097 c65faucet-1.0.54/docker/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docker/fuzz_config.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docker/fuzz_packet.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1176 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docker/install-faucet.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1232 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docker/localtest.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      797 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docker/pip_deps.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docker/retrycmd.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7205 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docker/runtests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      697 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docker/shard_tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docker-compose.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.596097 c65faucet-1.0.54/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.580097 c65faucet-1.0.54/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.596097 c65faucet-1.0.54/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/css/responsive-tables.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.600097 c65faucet-1.0.54/docs/_static/deployments/
+-rw-r--r--   0 runner    (1001) docker     (123)    89120 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/deployments/ONF_Faucet_deploy1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   984943 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/deployments/nznog17-physical-network.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)  1106115 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/deployments/nznog17-virtual-network.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.600097 c65faucet-1.0.54/docs/_static/grafana-dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)    23629 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/grafana-dashboards/faucet_instrumentation.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22310 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/grafana-dashboards/faucet_inventory.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/grafana-dashboards/faucet_port_statistics.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.604097 c65faucet-1.0.54/docs/_static/images/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8466 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/images/8021X-conf-diagram.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    97737 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/images/faucet-architecture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23716 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/images/faucet-pipeline.png
+-rw-r--r--   0 runner    (1001) docker     (123)    58351 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/images/faucet-pipeline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/images/faucet-pipeline.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   136689 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/images/gauge-nznog17.png
+-rw-r--r--   0 runner    (1001) docker     (123)   285918 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/images/gauge-snapshot1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   452164 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/images/gauge-snapshot2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   467326 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/images/gauge-snapshot3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    51732 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/images/tutorial-acls.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    77255 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/images/tutorial-bgp-routing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    47652 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/images/tutorial-ivr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   120062 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/images/tutorial-multi-root-stack.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    87114 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/images/tutorial-nfv-services.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/images/tutorial-stack-loop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    78230 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/images/tutorial-stack-tunnel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    53594 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/images/tutorial-stack.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   109550 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/images/tutorial-stackwithivr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    59007 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/images/tutorial-static-routing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   172474 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/images/tutorial-vlans.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.604097 c65faucet-1.0.54/docs/_static/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/tutorial/add_tagged_interface
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/tutorial/as_ns
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/tutorial/cleanup
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/tutorial/create_ns
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/tutorial/destroy_ns
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/_static/tutorial/inter_switch_link
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/architecture.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.604097 c65faucet-1.0.54/docs/autogen/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/autogen/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40109 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14496 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/developer_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/external_resources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/fuzzing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/monitoring.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.604097 c65faucet-1.0.54/docs/recipe_book/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/recipe_book/forwarding.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/recipe_book/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/recipe_book/policy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/recipe_book/routing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.608097 c65faucet-1.0.54/docs/release_notes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/release_notes/1.7.0.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/release_notes/1.9.0.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.608097 c65faucet-1.0.54/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.608097 c65faucet-1.0.54/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/tutorials/acls.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/tutorials/conntrack.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18441 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/tutorials/first_time.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17927 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/tutorials/nfv_services.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15268 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/tutorials/routing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    30053 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/tutorials/stacking.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/tutorials/vlans.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.608097 c65faucet-1.0.54/docs/vendors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.608097 c65faucet-1.0.54/docs/vendors/allied-telesis/
+-rw-r--r--   0 runner    (1001) docker     (123)    14233 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/vendors/allied-telesis/README_Allied_Telesis.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.608097 c65faucet-1.0.54/docs/vendors/cisco/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9404 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/vendors/cisco/README_Cisco.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.608097 c65faucet-1.0.54/docs/vendors/hpe/
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/vendors/hpe/README_Aruba.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/vendors/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.608097 c65faucet-1.0.54/docs/vendors/lagopus/
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/vendors/lagopus/README_Lagopus.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.608097 c65faucet-1.0.54/docs/vendors/northboundnetworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/vendors/northboundnetworks/README_ZodiacFX.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/vendors/northboundnetworks/README_ZodiacGX.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1292 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/vendors/northboundnetworks/conf-zodiac.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.608097 c65faucet-1.0.54/docs/vendors/noviflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/vendors/noviflow/README_noviflow.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.608097 c65faucet-1.0.54/docs/vendors/ovs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/vendors/ovs/README_OVS-DPDK.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18223 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/vendors/ovs/faucet_ovs_test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-05-25 09:30:45.000000 c65faucet-1.0.54/docs/vendors/ovs/faucet_testing_with_OVS_on_hardware.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.584097 c65faucet-1.0.54/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.608097 c65faucet-1.0.54/etc/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-25 09:30:45.000000 c65faucet-1.0.54/etc/default/faucet
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-25 09:30:45.000000 c65faucet-1.0.54/etc/default/gauge
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.608097 c65faucet-1.0.54/etc/faucet/
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-25 09:30:45.000000 c65faucet-1.0.54/etc/faucet/acls.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-25 09:30:45.000000 c65faucet-1.0.54/etc/faucet/faucet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-25 09:30:45.000000 c65faucet-1.0.54/etc/faucet/gauge.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-25 09:30:45.000000 c65faucet-1.0.54/etc/faucet/os_ken.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-25 09:30:45.000000 c65faucet-1.0.54/etc/faucet/ryu.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.608097 c65faucet-1.0.54/etc/logrotate.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-25 09:30:45.000000 c65faucet-1.0.54/etc/logrotate.d/faucet
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-25 09:30:45.000000 c65faucet-1.0.54/etc/logrotate.d/gauge
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.612098 c65faucet-1.0.54/etc/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-25 09:30:45.000000 c65faucet-1.0.54/etc/prometheus/faucet.rules.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-25 09:30:45.000000 c65faucet-1.0.54/etc/prometheus/prometheus-docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-25 09:30:45.000000 c65faucet-1.0.54/etc/prometheus/prometheus.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.584097 c65faucet-1.0.54/etc/systemd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.612098 c65faucet-1.0.54/etc/systemd/system/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-25 09:30:45.000000 c65faucet-1.0.54/etc/systemd/system/faucet.service
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-25 09:30:45.000000 c65faucet-1.0.54/etc/systemd/system/gauge.service
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-25 09:30:45.000000 c65faucet-1.0.54/etc/systemd/system/prometheus.service
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.616098 c65faucet-1.0.54/faucet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5773 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35363 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/acl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2276 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/check_faucet_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14246 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/config_parser_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71188 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/dp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/faucet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/faucet_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/faucet_dot1x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/faucet_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/faucet_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11424 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/faucet_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/faucet_pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7755 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/fctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/gauge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/gauge_influx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/gauge_pollers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/gauge_prom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31120 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/prom_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19588 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/tfm_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73345 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/valve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30131 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/valve_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/valve_coprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/valve_lldp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/valve_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42091 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/valve_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/valve_of_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/valve_outonly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28984 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/valve_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/valve_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49835 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/valve_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/valve_ryuapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18431 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/valve_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/valve_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30701 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/valve_switch_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52744 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/valve_switch_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/valve_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/valve_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18634 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/valves_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26043 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/vlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-25 09:30:45.000000 c65faucet-1.0.54/faucet/watcher_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-25 09:30:45.000000 c65faucet-1.0.54/fuzz-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.616098 c65faucet-1.0.54/git-hook/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      456 2023-05-25 09:30:45.000000 c65faucet-1.0.54/git-hook/pre-commit
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-25 09:30:45.000000 c65faucet-1.0.54/helper-funcs
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-25 09:30:45.000000 c65faucet-1.0.54/hw_switch_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.616098 c65faucet-1.0.54/ofctl_rest/
+-rw-r--r--   0 runner    (1001) docker     (123)    27150 2023-05-25 09:30:45.000000 c65faucet-1.0.54/ofctl_rest/ofctl_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-05-25 09:30:45.000000 c65faucet-1.0.54/ofctl_rest/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-25 09:30:45.000000 c65faucet-1.0.54/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-25 09:31:20.624098 c65faucet-1.0.54/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3802 2023-05-25 09:30:45.000000 c65faucet-1.0.54/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-25 09:30:45.000000 c65faucet-1.0.54/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.616098 c65faucet-1.0.54/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.616098 c65faucet-1.0.54/tests/codecheck/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/codecheck/flake8.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/codecheck/min_pylint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/codecheck/pylint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      342 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/codecheck/pytype.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      701 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/codecheck/src_files.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.584097 c65faucet-1.0.54/tests/generative/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.584097 c65faucet-1.0.54/tests/generative/fuzzer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.620098 c65faucet-1.0.54/tests/generative/fuzzer/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/config/config.dict
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.620098 c65faucet-1.0.54/tests/generative/fuzzer/config/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/config/examples/ex0
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/config/fuzz_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/config/generate_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.620098 c65faucet-1.0.54/tests/generative/fuzzer/packet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/display_packet_crash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.620098 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/aoe.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/arp.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/arp.ex2
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/asap.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/asap.ex2
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/diameter.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/dns.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/dns.ex2
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/http.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/http.ex2
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/icmp.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/icmp.ex2
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/icmp.ex3
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/icmp.ex4
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/igmpv2.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/ipv4.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/ipv6.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/irc.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/irc.ex2
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/irc.ex3
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/lacp.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/msger.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/packet.dict
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/tcp.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/tcp.ex2
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/tcp.ex3
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/tcp.ex4
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/tcp.ex5
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/udp.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/udp.ex2
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/udp.ex3
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/udp.ex4
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/fake_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/fuzzer/packet/fuzz_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.620098 c65faucet-1.0.54/tests/generative/integration/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2304 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/integration/fault_tolerance_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18304 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/integration/fault_tolerance_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.620098 c65faucet-1.0.54/tests/generative/unit/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12779 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/generative/unit/test_topology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.624098 c65faucet-1.0.54/tests/integration/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      565 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/integration/mininet_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)   157767 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/integration/mininet_multidp_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)   308768 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/integration/mininet_tests.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      574 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/run_unit_tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      244 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/sysctls_for_tests.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.584097 c65faucet-1.0.54/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.624098 c65faucet-1.0.54/tests/unit/clib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8815 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/unit/clib/test_topo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.624098 c65faucet-1.0.54/tests/unit/faucet/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10401 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/unit/faucet/test_check_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   134114 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/unit/faucet/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6666 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/unit/faucet/test_fctl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1519 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/unit/faucet/test_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5773 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/unit/faucet/test_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31562 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/unit/faucet/test_valve.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39651 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/unit/faucet/test_valve_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4960 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/unit/faucet/test_valve_dot1x.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5875 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/unit/faucet/test_valve_egress.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2968 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/unit/faucet/test_valve_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154810 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/unit/faucet/test_valve_stack.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2770 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/unit/faucet/test_valveapp_smoke.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9217 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/unit/faucet/test_vlan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.624098 c65faucet-1.0.54/tests/unit/gauge/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5590 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/unit/gauge/test_config_gauge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36917 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/unit/gauge/test_gauge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1516 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/unit/gauge/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:31:20.624098 c65faucet-1.0.54/tests/unit/packaging/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5501 2023-05-25 09:30:45.000000 c65faucet-1.0.54/tests/unit/packaging/test_packaging.py
```

### Comparing `c65faucet-1.0.53/.github/workflows/disabled/periodic.yml` & `c65faucet-1.0.54/.github/workflows/disabled/periodic.yml`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 env:
   FAUCET_TEST_IMG: "c65sdn/tests"
   SHARDARGS: "--privileged --sysctl net.ipv6.conf.all.disable_ipv6=0 --ulimit core=99999999999:99999999999 -v /var/local/lib/docker:/var/lib/docker -v /var/tmp:/var/tmp"
 
 jobs:
   generative-testing:
     name: Generative tests
-    runs-on: ubuntu-latest
+    runs-on: ubuntu-22.04
     strategy:
       matrix:
         MATRIX_SHARD: [--generative_unit, --generative_tolerance]
     steps:
       - name: Checkout repo
         uses: actions/checkout@v3
       - name: Setup docker test requirements
```

### Comparing `c65faucet-1.0.53/.github/workflows/disabled/release-debian.yml` & `c65faucet-1.0.54/.github/workflows/disabled/release-debian.yml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/.github/workflows/release-docker.yml` & `c65faucet-1.0.54/.github/workflows/release-docker.yml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/.github/workflows/release-python.yml` & `c65faucet-1.0.54/.github/workflows/release-python.yml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/.github/workflows/tests-codecheck.yml` & `c65faucet-1.0.54/.github/workflows/tests-codecheck.yml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/.github/workflows/tests-docs.yml` & `c65faucet-1.0.54/.github/workflows/tests-docs.yml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/.github/workflows/tests-integration.yml` & `c65faucet-1.0.54/.github/workflows/tests-integration.yml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 env:
   FILES_CHANGED: "all"
   MATRIX_SHARDS: 10
 
 jobs:
   sanity-tests:
     name: Sanity tests
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
     container:
       image: c65sdn/test-base:latest
       options: --privileged --cap-add=ALL -v /lib/modules:/lib/modules -v /var/local/lib/docker:/var/lib/docker --sysctl net.ipv6.conf.all.disable_ipv6=0 --ulimit core=-1
     steps:
       - name: Checkout repo
         uses: actions/checkout@v3
       - if: ${{ github.event_name == 'pull_request' }}
@@ -71,15 +71,15 @@
         run: |
           if [ ls -1 /var/tmp/core* > /dev/null 2>&1 ]; then
             exit 1
           fi
 
   integration-tests:
     name: Integration tests
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-22.04
     needs: sanity-tests
     container:
       image: c65sdn/test-base:latest
       options: --privileged --cap-add=ALL -v /lib/modules:/lib/modules -v /var/local/lib/docker:/var/lib/docker --sysctl net.ipv6.conf.all.disable_ipv6=0 --ulimit core=-1
     strategy:
       matrix:
         MATRIX_SHARD: [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
```

### Comparing `c65faucet-1.0.53/.github/workflows/tests-unit.yml` & `c65faucet-1.0.54/.github/workflows/tests-unit.yml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/.pylintrc` & `c65faucet-1.0.54/.pylintrc`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/CONTRIBUTING.rst` & `c65faucet-1.0.54/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/LICENSE` & `c65faucet-1.0.54/LICENSE`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/Makefile` & `c65faucet-1.0.54/Makefile`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/PKG-INFO` & `c65faucet-1.0.54/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c65faucet
-Version: 1.0.53
+Version: 1.0.54
 Summary: Faucet is an OpenFlow controller that implements a layer 2 and layer 3 switch.
 Home-page: https://faucet.nz
 Author: Faucet development team
 Author-email: faucetsdn@googlegroups.com
 License: Apache-2
 Keywords: openflow,openvswitch,ryu
 Platform: any
```

### Comparing `c65faucet-1.0.53/README.rst` & `c65faucet-1.0.54/README.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/adapters/vendors/faucetagent/Dockerfile` & `c65faucet-1.0.54/adapters/vendors/faucetagent/Dockerfile`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/adapters/vendors/faucetagent/README.rst` & `c65faucet-1.0.54/adapters/vendors/faucetagent/README.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/adapters/vendors/faucetagent/example_client.sh` & `c65faucet-1.0.54/adapters/vendors/faucetagent/example_client.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/adapters/vendors/faucetagent/gencerts.sh` & `c65faucet-1.0.54/adapters/vendors/faucetagent/gencerts.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/adapters/vendors/rabbitmq/Dockerfile` & `c65faucet-1.0.54/adapters/vendors/rabbitmq/Dockerfile`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/adapters/vendors/rabbitmq/README.rst` & `c65faucet-1.0.54/adapters/vendors/rabbitmq/README.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/adapters/vendors/rabbitmq/docker-compose.yaml` & `c65faucet-1.0.54/adapters/vendors/rabbitmq/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/adapters/vendors/rabbitmq/example_consumer.py` & `c65faucet-1.0.54/adapters/vendors/rabbitmq/example_consumer.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/adapters/vendors/rabbitmq/rabbit.py` & `c65faucet-1.0.54/adapters/vendors/rabbitmq/rabbit.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/adapters/vendors/rabbitmq/test_rabbit.py` & `c65faucet-1.0.54/adapters/vendors/rabbitmq/test_rabbit.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/c65faucet.egg-info/PKG-INFO` & `c65faucet-1.0.54/c65faucet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c65faucet
-Version: 1.0.53
+Version: 1.0.54
 Summary: Faucet is an OpenFlow controller that implements a layer 2 and layer 3 switch.
 Home-page: https://faucet.nz
 Author: Faucet development team
 Author-email: faucetsdn@googlegroups.com
 License: Apache-2
 Keywords: openflow,openvswitch,ryu
 Platform: any
```

### Comparing `c65faucet-1.0.53/c65faucet.egg-info/SOURCES.txt` & `c65faucet-1.0.54/c65faucet.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 .codecov.yml
 .dockerignore
 .flake8
 .pylintrc
 .readthedocs.yml
 .renovaterc.json
-.stickler.yml
 AUTHORS
 CONTRIBUTING.rst
 ChangeLog
 Dockerfile.faucet
 Dockerfile.fuzz-config
 Dockerfile.fuzz-packet
 Dockerfile.gauge
```

### Comparing `c65faucet-1.0.53/clib/clib_mininet_test.py` & `c65faucet-1.0.54/clib/clib_mininet_test.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/clib/clib_mininet_test_main.py` & `c65faucet-1.0.54/clib/clib_mininet_test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,14 @@
         ["--version"],
         "Open vSwitch",
         r"ovs-vsctl\s+\(Open vSwitch\)\s+(\d+\.\d+)\.\d+\n",
         "2.3",
     ),
     ("tcpdump", ["-h"], "tcpdump", r"tcpdump\s+version\s+(\d+\.\d+)\.\d+\n", "4.5"),
     ("nc", ["-h"], "OpenBSD netcat", "", 0),
-    ("vconfig", [], "the VLAN you are talking about", "", 0),
     (
         "fuser",
         ["-V"],
         r"fuser \(PSmisc\)",
         r"fuser \(PSmisc\) (\d+\.\d+|UNKNOWN)\n",
         "22.0",
     ),
@@ -805,17 +804,48 @@
             report_results([sanity_result], hw_config, report_json_filename)
 
     if no_tests:
         print("no tests selected")
         shutil.rmtree(root_tmpdir)
         sys.exit(0)
     else:
-        decoded_pcap_logs = glob.glob(
-            os.path.join(os.path.join(root_tmpdir, "*"), "*of.cap.txt")
-        )
+        decoded_pcap_logs = []
+        port_match_re = re.compile(".+\-([0-9]+)-of.cap")
+        of_pcaps = glob.glob(os.path.join(os.path.join(root_tmpdir, "*"), "*of.cap"))
+        for of_pcap in of_pcaps:
+            port_match = port_match_re.match(of_pcap)
+            if not port_match:
+                print("ignoring unexpected OpenFlow pcap %s" % of_pcap)
+                continue
+            text_ofcap_log = of_pcap.replace(".cap", ".txt")
+            decoded_pcap_logs.append(text_ofcap_log)
+            of_port = int(port_match.group(1))
+            with open(text_ofcap_log, "w", encoding="utf-8") as text_ofcap:
+                subprocess.call(
+                    [
+                        "timeout",
+                        str(60),
+                        "tshark",
+                        "-l",
+                        "-n",
+                        "-Q",
+                        "-d",
+                        "tcp.port==%u,openflow" % of_port,
+                        "-O",
+                        "openflow_v4",
+                        "-Y",
+                        "openflow_v4",
+                        "-r",
+                        of_pcap,
+                    ],
+                    stdout=text_ofcap,
+                    stdin=mininet_test_util.DEVNULL,
+                    stderr=mininet_test_util.DEVNULL,
+                    close_fds=True,
+                )
         pipeline_superset_report(decoded_pcap_logs)
         clean_test_dirs(
             root_tmpdir,
             all_successful,
             sanity_result.wasSuccessful(),
             keep_logs,
             dumpfail,
```

### Comparing `c65faucet-1.0.53/clib/clib_mininet_tests.py` & `c65faucet-1.0.54/clib/clib_mininet_tests.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/clib/config_generator.py` & `c65faucet-1.0.54/clib/config_generator.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/clib/docker_host.py` & `c65faucet-1.0.54/clib/docker_host.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/clib/fakeoftable.py` & `c65faucet-1.0.54/clib/fakeoftable.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/clib/mininet_test_base.py` & `c65faucet-1.0.54/clib/mininet_test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -610,16 +610,15 @@
                 self.assertFalse(stderr, msg="%s: %s" % (stderr, cmd))
 
         _cmd("ebtables --f OUTPUT")
         for phys_port in self.switch_map.values():
             phys_mac = self.get_mac_of_intf(phys_port)
             for cmd in (
                 "ip link set dev %s up" % phys_port,
-                "ip -4 addr flush dev %s" % phys_port,
-                "ip -6 addr flush dev %s" % phys_port,
+                "ip addr flush dev %s" % phys_port,
                 "ebtables -A OUTPUT -s %s -o %s -j DROP" % (phys_mac, phys_port),
             ):
                 _cmd(cmd)
 
     def _attach_physical_switch(self):
         """Bridge a physical switch into test topology.
 
@@ -701,23 +700,20 @@
         return self.net.controllers[0]
 
     @staticmethod
     def _start_gauge_check():
         return None
 
     def _start_check(self):
-        # '_wait_controllers_connected' also checks the 'healthy' state
         if not self._wait_controllers_connected():
             return "not all controllers connected to switch"
         if not self._wait_ofctl_up():
             return "ofctl not up"
         if not self.wait_dp_status(1):
             return "prometheus port not up"
-        if not self._wait_controllers_healthy():
-            return "not all controllers healthy after initial switch connection"
         if self.config_ports:
             for port_name, port in self.config_ports.items():
                 if port is not None and not port_name.startswith("gauge"):
                     if not self._get_controller().listen_port(port):
                         return "faucet not listening on %u (%s)" % (port, port_name)
         return self._start_gauge_check()
 
@@ -999,18 +995,18 @@
             )
 
     @staticmethod
     def tcpdump_helper(*args, **kwargs):
         return TcpdumpHelper(*args, **kwargs).execute()
 
     @staticmethod
-    def scapy_template(packet, iface, count=1):
+    def scapy_template(packet, iface, count=1, inter=0.5):
         return (
-            "python3 -c \"from scapy.all import * ; sendp(%s, iface='%s', count=%u)\""
-            % (packet, iface, count)
+            "python3 -c \"from scapy.all import * ; pkt = %s ; sendp(pkt, iface='%s', count=%u, inter=%u)\""
+            % (packet, iface, count, inter)
         )
 
     def scapy_base_udp(
         self, mac, iface, src_ip, dst_ip, dport, sport, count=1, dst=None
     ):
         if dst is None:
             dst = "ff:ff:ff:ff:ff:ff"
@@ -2120,36 +2116,34 @@
             self.assertNotEqual(locations, new_locations)
             locations = new_locations
 
     def _verify_xcast(
         self, received_expected, packets, tcpdump_filter, scapy_cmd, host_a, host_b
     ):
         received_packets = False
-        for _ in range(packets):
-            tcpdump_txt = self.tcpdump_helper(
-                host_b,
-                tcpdump_filter,
-                [partial(host_a.cmd, scapy_cmd)],
-                packets=1,
-                timeout=2,
-            )
-            msg = "%s (%s) -> %s (%s): %s" % (
-                host_a,
-                host_a.MAC(),
-                host_b,
-                host_b.MAC(),
-                tcpdump_txt,
-            )
-            received_no_packets = self.tcpdump_rx_packets(tcpdump_txt, packets=0)
-            received_packets = received_packets or not received_no_packets
-            if received_packets:
-                if received_expected is not False:
-                    return True
-                self.assertTrue(received_expected, msg=msg)
-            time.sleep(1)
+        tcpdump_txt = self.tcpdump_helper(
+            host_b,
+            tcpdump_filter,
+            [partial(host_a.cmd, scapy_cmd)],
+            packets=packets,
+            timeout=packets,
+        )
+        msg = "%s (%s) -> %s (%s): %s" % (
+            host_a,
+            host_a.MAC(),
+            host_b,
+            host_b.MAC(),
+            tcpdump_txt,
+        )
+        received_no_packets = self.tcpdump_rx_packets(tcpdump_txt, packets=0)
+        received_packets = received_packets or not received_no_packets
+        if received_packets:
+            if received_expected is not False:
+                return True
+            self.assertTrue(received_expected, msg=msg)
 
         if received_expected is None:
             return received_packets
         self.assertEqual(received_expected, received_packets, msg=msg)
         return None
 
     def verify_broadcast(self, hosts=None, broadcast_expected=True, packets=3):
@@ -2936,15 +2930,18 @@
             retries=retries,
             default=default,
         )
 
     def quiet_commands(self, host, commands):
         for command in commands:
             result = host.cmd(command)
-            self.assertEqual("", result, msg="%s: %s" % (command, result))
+            self.assertTrue(
+                result == "" or result.startswith("Killed"),
+                msg="%s: %s" % (command, result),
+            )
 
     def _config_tableids(self):
         # Wait for VLAN table to appear, rapidly scrape the rest.
         self._VLAN_TABLE = self._get_tableid("vlan", 1, self._VLAN_TABLE)
         self._COPRO_TABLE = self._get_tableid("vlan", 1, self._COPRO_TABLE)
         self._PORT_ACL_TABLE = self._get_tableid("port_acl", 1, self._PORT_ACL_TABLE)
         self._VLAN_ACL_TABLE = self._get_tableid("vlan_acl", 1, self._VLAN_ACL_TABLE)
@@ -2984,23 +2981,21 @@
 
     def add_macvlan(self, host, macvlan_intf, ipa=None, ipm=24, mac=None, mode="vepa"):
         if mac is None:
             mac = ""
         else:
             mac = "address %s" % mac
         add_cmds = [
-            "ip link add %s link %s %s type macvlan mode %s"
+            "link add %s link %s %s type macvlan mode %s"
             % (macvlan_intf, host.defaultIntf(), mac, mode),
-            "ip link set dev %s up" % macvlan_intf,
+            "link set dev %s up" % macvlan_intf,
         ]
         if ipa:
-            add_cmds.append(
-                "ip address add %s/%s brd + dev %s" % (ipa, ipm, macvlan_intf)
-            )
-        self.quiet_commands(host, add_cmds)
+            add_cmds.append("addr add %s/%s brd + dev %s" % (ipa, ipm, macvlan_intf))
+        host.run_ip_batch(add_cmds)
 
     def del_macvlan(self, host, macvlan_intf):
         self.quiet_commands(
             host,
             [host.cmd("ip link del link %s %s" % (host.defaultIntf(), macvlan_intf))],
         )
 
@@ -3656,16 +3651,15 @@
         )
         self.verify_ipv4_routing(
             first_host, first_host_routed_ip, second_host, second_host_routed_ip2
         )
 
     @staticmethod
     def host_drop_all_ips(host):
-        for ipv in (4, 6):
-            host.cmd("ip -%u addr flush dev %s" % (ipv, host.defaultIntf()))
+        host.cmd("ip addr flush dev %s" % host.defaultIntf())
 
     def setup_ipv6_hosts_addresses(
         self,
         first_host,
         first_host_ip,
         first_host_routed_ip,
         second_host,
```

### Comparing `c65faucet-1.0.53/clib/mininet_test_base_topo.py` & `c65faucet-1.0.54/clib/mininet_test_base_topo.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,44 +284,44 @@
                 bond_members = [
                     pair[0].name
                     for switch in lacp_switches
                     for pair in host.connectionsTo(switch)
                 ]
                 bond_name = "bond%u" % (bond_index)
                 self.host_information[host_id]["bond"] = bond_name
+                bond_cmds = []
                 for bond_member in bond_members:
                     # Deconfigure bond members
-                    self.quiet_commands(
-                        host,
-                        (
-                            "ip link set %s down" % bond_member,
-                            "ip address flush dev %s" % bond_member,
-                        ),
+                    bond_cmds.extend(
+                        [
+                            "link set %s down" % bond_member,
+                            "address flush dev %s" % bond_member,
+                        ]
                     )
                 # Configure bond interface
-                self.quiet_commands(
-                    host,
-                    (
+                bond_cmds.extend(
+                    [
                         (
-                            "ip link add %s address 0e:00:00:00:00:99 "
+                            "link add %s address 0e:00:00:00:00:99 "
                             "type bond mode 802.3ad lacp_rate fast miimon 100 "
                             "xmit_hash_policy layer2+3"
                         )
                         % (bond_name),
-                        "ip add add %s/%s dev %s"
-                        % (orig_ip, self.NETPREFIX, bond_name),
-                        "ip link set %s up" % bond_name,
-                    ),
+                        "addr add %s/%s dev %s" % (orig_ip, self.NETPREFIX, bond_name),
+                        "link set %s up" % bond_name,
+                    ]
                 )
                 # Add bond members
                 for bond_member in bond_members:
-                    self.quiet_commands(
-                        host,
-                        ("ip link set dev %s master %s" % (bond_member, bond_name),),
+                    bond_cmds.extend(
+                        [
+                            "link set dev %s master %s" % (bond_member, bond_name),
+                        ]
                     )
+                host.run_ip_batch(bond_cmds)
                 bond_index += 1
                 # Return the ports to UP
                 for dp_i, ports in self.host_port_maps[host_id].items():
                     for port in ports:
                         self.set_port_up(port, self.topo.dpids_by_id[dp_i])
 
     def setup_intervlan_host_routes(self):
@@ -437,40 +437,27 @@
         """Verify all stack ports are up"""
         for _ in range(timeout):
             links = 0
             links_up = 0
             for link, ports in self.link_port_maps.items():
                 if link[0] in self.IGNORED_SWITCHES or link[1] in self.IGNORED_SWITCHES:
                     continue
+                dpid = self.topo.dpids_by_id[link[0]]
+                name = self.topo.switches_by_id[link[0]]
                 for port in ports:
-                    dpid = self.topo.dpids_by_id[link[0]]
-                    name = self.topo.switches_by_id[link[0]]
                     status = self.stack_port_status(dpid, name, port)
                     links += 1
                     if status == 3:  # STACK_STATE_UP
                         links_up += 1
             prop_up = links_up / links
             if prop_up >= prop:
                 return
+            time.sleep(1)
         self.fail("not enough links up: %f / %f" % (links_up, links))
 
-    def verify_stack_down(self):
-        """Verify all stack ports are down"""
-        links = 0
-        links_down = 0
-        for link, ports in self.link_port_maps.items():
-            for port in ports:
-                dpid = self.topo.dpids_by_id[link[0]]
-                name = self.topo.switches_by_id[link[0]]
-                status = self.stack_port_status(dpid, name, port)
-                links += 1
-                if status != 3:
-                    links_down += 1
-        self.assertEqual(links, links_down, "Not all links DOWN")
-
     def verify_one_stack_down(self, stack_offset_port, coldstart=False):
         """Test conditions when one stack port is down"""
         self.retry_net_ping()
         stack_link = None
         count = 0
         for sport, link in self.topo.ports[self.topo.switches_by_id[0]].items():
             if self.topo.isSwitch(link[0]):
```

### Comparing `c65faucet-1.0.53/clib/mininet_test_topo.py` & `c65faucet-1.0.54/clib/mininet_test_topo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 #!/usr/bin/env python3
 """Topology components for FAUCET Mininet unit tests."""
 
 from collections import namedtuple
 import os
+import pty
+import select
 import socket
 import string
 import shutil
 import subprocess
+import tempfile
 import time
 
 import netifaces
 
 # pylint: disable=too-many-arguments
 
-from mininet.log import output, warn
+from mininet.log import output, warn, error
 from mininet.topo import Topo
 from mininet.node import Controller
-from mininet.node import CPULimitedHost
+from mininet.node import Host
 from mininet.node import OVSSwitch
 from mininet.link import TCIntf, Link
 
 from clib import mininet_test_util
 
 
 SWITCH_START_PORT = 5
@@ -66,21 +69,77 @@
             addr1=addr1,
             addr2=addr2,
             params1=params,
             params2=params,
         )
 
 
-class FaucetHost(CPULimitedHost):
+class FaucetHost(Host):
     """Base Mininet Host class, for Mininet-based tests."""
 
     def __init__(self, *args, **kwargs):
         self.pid_files = []
         super().__init__(*args, **kwargs)
 
+    def startShell(self, mnopts=None):
+        "Start a shell process for running commands"
+        if self.shell:
+            error("%s: shell is already running\n" % self.name)
+            return
+        # mnexec: (c)lose descriptors, (d)etach from tty,
+        # (p)rint pid, and run in (n)amespace
+        opts = "-cd" if mnopts is None else mnopts
+        if self.inNamespace:
+            opts += "n"
+        # bash -i: force interactive
+        # -s: pass $* to shell, and make process easy to find in ps
+        # prompt is set to sentinel chr( 127 )
+        cmd = [
+            "mnexec",
+            opts,
+            "env",
+            "PS1=" + chr(127),
+            "dash",
+            "-is",
+            "mininet:" + self.name,
+        ]
+
+        # Spawn a shell subprocess in a pseudo-tty, to disable buffering
+        # in the subprocess and insulate it from signals (e.g. SIGINT)
+        # received by the parent
+        self.master, self.slave = pty.openpty()
+        self.shell = self._popen(
+            cmd, stdin=self.slave, stdout=self.slave, stderr=self.slave, close_fds=False
+        )
+        # XXX BL: This doesn't seem right, and we should also probably
+        # close our files when we exit...
+        self.stdin = os.fdopen(self.master, "r")
+        self.stdout = self.stdin
+        self.pid = self.shell.pid
+        self.pollOut = select.poll()
+        self.pollOut.register(self.stdout)
+        # Maintain mapping between file descriptors and nodes
+        # This is useful for monitoring multiple nodes
+        # using select.poll()
+        self.outToNode[self.stdout.fileno()] = self
+        self.inToNode[self.stdin.fileno()] = self
+        self.execed = False
+        self.lastCmd = None
+        self.lastPid = None
+        self.readbuf = ""
+        # Wait for prompt
+        while True:
+            data = self.read(1024)
+            if data[-1] == chr(127):
+                break
+            self.pollOut.poll()
+        self.waiting = False
+        # +m: disable job control notification
+        self.cmd("unset HISTFILE; stty -echo; set +m")
+
     def terminate(self):
         # If any 'dnsmasq' processes were started, terminate them now
         for pid_file in self.pid_files:
             with open(pid_file, "r", encoding="utf-8") as pf:
                 for _, pid in enumerate(pf):
                     os.kill(int(pid), 15)
         super().terminate()
@@ -130,14 +189,22 @@
             mininet_test_util.timeout_cmd(dhclient_cmd, timeout), verbose=True
         )
 
     def return_ip(self):
         """Return host IP as a string"""
         return self.cmd("hostname -I")
 
+    def run_ip_batch(self, cmds):
+        with tempfile.TemporaryDirectory() as tmpdir:
+            cmd_filename = os.path.join(tmpdir, "ipcmds.txt")
+            with open(cmd_filename, "w") as cmd_file:
+                cmd_file.write("\n".join(cmds))
+            result = self.cmd("ip -b %s" % cmd_filename)
+            assert result == "", (cmds, result)
+
 
 class VLANHost(FaucetHost):
     """Implementation of a Mininet host on a tagged VLAN."""
 
     intf_root_name = None
 
     vlans = None
@@ -151,66 +218,66 @@
         vlan_intfs (dict): Dictionary of interface IP addresses keyed by VLAN indices
         """
         super_config = super().config(**params)
         if vlans is None:
             vlans = [100]
         self.vlans = vlans
         self.vlan_intfs = {}
-        cmds = []
+        batch_cmds = []
         intf = self.defaultIntf()
         self.intf_root_name = intf.name
+        unique_intfs = set()
+
+        def _config_vlan(root_name, full_name, vlan_id):
+            batch_cmds.extend(
+                [
+                    "link add link %s name %s type vlan id %s"
+                    % (root_name, full_name, vlan_id),
+                    "link set dev %s up" % full_name,
+                ]
+            )
+
+        def _config_ip(config_full_name, config_ip):
+            batch_cmds.extend(["addr add %s dev %s" % (config_ip, config_full_name)])
+
         if "vlan_intfs" in params:
             vlan_intfs = params.get("vlan_intfs", {})
             for vlan_id, ip_addr in vlan_intfs.items():
                 if isinstance(vlan_id, tuple):
                     # Interface will take multiply VLAN tagged packets
                     intf_name = "%s" % intf.name
                     for vlan_i in vlan_id:
                         prev_name = intf_name
                         # Cannot have intf name tu0xy-eth0.VID1.VID2 as that takes up too many bytes
                         intf_name += ".%s" % vlan_i
-                        cmds.extend(
-                            [
-                                "ip link add link %s name %s type vlan id %s"
-                                % (prev_name, intf_name, vlans[vlan_i]),
-                                "ip link set dev %s up" % (intf_name),
-                            ]
-                        )
+                        if intf_name not in unique_intfs:
+                            _config_vlan(prev_name, intf_name, vlans[vlan_i])
+                            unique_intfs.add(intf_name)
                         self.nameToIntf[intf_name] = intf
                         self.vlan_intfs.setdefault(vlan_id, [])
                         self.vlan_intfs[vlan_id].append(intf_name)
-                    cmds.append("ip -4 addr add %s dev %s" % (ip_addr, intf_name))
+                    _config_ip(intf_name, ip_addr)
                 else:
                     intf_name = "%s.%s" % (intf, vlans[vlan_id])
-                    cmds.extend(
-                        [
-                            "vconfig add %s %d" % (intf.name, vlans[vlan_id]),
-                            "ip -4 addr add %s dev %s" % (ip_addr, intf_name),
-                            "ip link set dev %s up" % intf_name,
-                        ]
-                    )
+                    _config_vlan(intf, intf_name, vlans[vlan_id])
+                    _config_ip(intf_name, ip_addr)
                     self.nameToIntf[intf_name] = intf
                     self.vlan_intfs[vlan_id] = intf_name
         else:
-            vlan_intf_name = "%s.%s" % (intf, ".".join(str(v) for v in vlans))
-            cmds.extend(
-                [
-                    "ip link set dev %s up" % vlan_intf_name,
-                    "ip -4 addr add %s dev %s" % (params["ip"], vlan_intf_name),
-                ]
-            )
-            for vlan in vlans:
-                cmds.append("vconfig add %s %d" % (intf, vlan))
-            intf.name = vlan_intf_name
-            self.nameToIntf[vlan_intf_name] = intf
-        cmds.extend(
-            ["ip -4 addr flush dev %s" % intf, "ip -6 addr flush dev %s" % intf]
-        )
-        for cmd in cmds:
-            self.cmd(cmd)
+            for vlan_id in vlans:
+                intf_name = "%s.%s" % (intf, vlan_id)
+                _config_vlan(intf, intf_name, vlan_id)
+                _config_ip(intf_name, params["ip"])
+                self.nameToIntf[intf_name] = intf
+                self.vlan_intfs.setdefault(vlan_id, [])
+                self.vlan_intfs[vlan_id].append(intf_name)
+            intf.name = intf_name
+
+        batch_cmds.extend(["addr flush dev %s" % self.intf_root_name])
+        self.run_ip_batch(batch_cmds)
         return super_config
 
 
 class FaucetSwitch(OVSSwitch):
     """Switch that will be used by all tests (netdev based OVS)."""
 
     clist = None
@@ -316,21 +383,29 @@
             cargs
             + " -- add-br %s" % self
             + " -- set bridge %s controller=[%s]" % (self, cids)
             + self.bridgeOpts()
             + intfs
         )
         # switch interfaces on mininet host, must have no IP config.
+        sysctls = []
+        ipcmds = []
         for intf in switch_intfs:
-            for ipv in (4, 6):
-                self.cmd("ip -%u addr flush dev %s" % (ipv, intf))
-            assert (
-                self.cmd("echo 1 > /proc/sys/net/ipv6/conf/%s/disable_ipv6" % intf)
-                == ""
-            )
+            ipcmds.append("addr flush dev %s" % intf)
+            sysctls.append("net.ipv6.conf.%s.disable_ipv6=1" % intf)
+        with tempfile.TemporaryDirectory() as tmpdir:
+            sysctl_filename = os.path.join(tmpdir, "sysctl.txt")
+            ip_batch_filename = os.path.join(tmpdir, "ipbatch.txt")
+            with open(sysctl_filename, "w") as sysctl_file:
+                sysctl_file.write("\n".join(sysctls))
+            with open(ip_batch_filename, "w") as ip_batch_file:
+                ip_batch_file.write("\n".join(ipcmds))
+            self.cmd("sysctl -p %s" % sysctl_filename)
+            result = self.cmd("ip -b %s" % ip_batch_filename)
+            assert result == "", (result, ipcmds)
         # If necessary, restore TC config overwritten by OVS
         if not self.batch:
             for intf in self.intfList():
                 self.TCReapply(intf)
 
 
 class NoControllerFaucetSwitch(FaucetSwitch):
@@ -537,14 +612,15 @@
         **kwargs
     ):
         self.name_no_pid = name
         name_with_pid = "%s-%u" % (name, os.getpid())
         self.tmpdir = tmpdir
         self.controller_intf = controller_intf
         self.controller_ipv6 = controller_ipv6
+        self.cached_ryu_pid = None
         super().__init__(
             name_with_pid, cargs=self._add_cargs(cargs, name_with_pid), **kwargs
         )
 
     def _add_cargs(self, cargs, name):
         ofp_listen_host_arg = ""
         if self.controller_intf is not None:
@@ -570,15 +646,17 @@
     def IP(self):  # pylint: disable=invalid-name,arguments-differ
         if self.controller_intf is not None:
             return self.controller_ip
         return super().IP()
 
     def _start_tcpdump(self):
         """Start a tcpdump for OF port."""
-        self.ofcap = os.path.join(self.tmpdir, "-".join((self.name, "of.cap")))
+        self.ofcap = os.path.join(
+            self.tmpdir, "-".join((self.name, "%u-of.cap" % self.port))
+        )
         tcpdump_args = " ".join(
             (
                 "-s 0",
                 "-e",
                 "-n",
                 "-U",
                 "-q",
@@ -610,53 +688,55 @@
         ):
             if carg_val:
                 tls_cargs.append(("--%s=%s" % (carg_key, carg_val)))
         if tls_cargs:
             tls_cargs.append(("--ryu-ofp-ssl-listen-port=%u" % ofctl_port))
         return " ".join(tls_cargs)
 
-    def _command(self, env, tmpdir, name, args):
+    def _command(self, env, name, args):
         """Wrap controller startup command in shell script with environment."""
         env_vars = []
         for var, val in sorted(env.items()):
             env_vars.append("=".join((var, val)))
-        script_wrapper_name = os.path.join(tmpdir, "start-%s.sh" % name)
         cprofile_args = ""
         if self.CPROFILE:
             cprofile_args = "python3 -m cProfile -s time"
         full_faucet_dir = os.path.abspath(mininet_test_util.FAUCET_DIR)
-        with open(script_wrapper_name, "w", encoding="utf-8") as script_wrapper:
-            faucet_cli = "PYTHONPATH=%s %s exec timeout %u %s %s %s $*\n" % (
-                os.path.dirname(full_faucet_dir),
-                " ".join(env_vars),
-                self.MAX_CTL_TIME,
-                os.path.join(full_faucet_dir, "__main__.py"),
-                cprofile_args,
-                args,
-            )
-            script_wrapper.write(faucet_cli)
-        return "/bin/sh %s" % script_wrapper_name
+        faucet_cli = "PYTHONPATH=%s %s timeout %u %s %s %s" % (
+            os.path.dirname(full_faucet_dir),
+            " ".join(env_vars),
+            self.MAX_CTL_TIME,
+            os.path.join(full_faucet_dir, "__main__.py"),
+            cprofile_args,
+            args,
+        )
+        return faucet_cli
 
     def ryu_pid(self):
         """Return PID of ryu-manager process."""
-        if os.path.exists(self.pid_file) and os.path.getsize(self.pid_file) > 0:
-            pid = None
-            with open(self.pid_file, encoding="utf-8") as pid_file:
-                pid = int(pid_file.read())
-            return pid
-        return None
+        if self.cached_ryu_pid is None:
+            if os.path.exists(self.pid_file) and os.path.getsize(self.pid_file) > 0:
+                with open(self.pid_file, encoding="utf-8") as pid_file:
+                    self.cached_ryu_pid = int(pid_file.read())
+        return self.cached_ryu_pid
 
     def listen_port(self, port, state="LISTEN"):
         """Return True if port in specified TCP state."""
-        for ipv in (4, 6):
-            listening_out = self.cmd(
-                mininet_test_util.tcp_listening_cmd(port, ipv=ipv, state=state)
-            ).split()
-            for pid in listening_out:
-                if int(pid) == self.ryu_pid():
+        ryu_pid = self.ryu_pid()
+        if ryu_pid is not None:
+            for ipv in (4, 6):
+                listening_pids = [
+                    int(pid)
+                    for pid in self.cmd(
+                        mininet_test_util.tcp_listening_cmd(
+                            port, ipv=ipv, state=state, pid=ryu_pid
+                        )
+                    ).split()
+                ]
+                if listening_pids:
                     return True
         return False
 
     # pylint: disable=invalid-name
     @staticmethod
     def checkListening():
         """Mininet's checkListening() causes occasional false positives (with
@@ -665,15 +745,15 @@
 
     def listening(self):
         """Return True if controller listening on required ports."""
         return self.listen_port(self.port)
 
     def connected(self):
         """Return True if at least one switch connected and controller healthy."""
-        return self.healthy() and self.listen_port(self.port, state="ESTABLISHED")
+        return self.listen_port(self.port, state="ESTABLISHED") and self.healthy()
 
     def logname(self):
         """Return log file for controller."""
         return os.path.join("/tmp", self.name + ".log")
 
     def healthy(self):
         """Return True if controller logging and listening on required ports."""
@@ -687,41 +767,17 @@
 
     def start(self):
         """Start tcpdump for OF port and then start controller."""
         self._start_tcpdump()
         super().start()
 
     def _stop_cap(self):
-        """Stop tcpdump for OF port and run tshark to decode it."""
+        """Stop tcpdump for OF port."""
         if os.path.exists(self.ofcap):
             self.cmd(" ".join(["fuser", "-15", "-k", self.ofcap]))
-            text_ofcap_log = "%s.txt" % self.ofcap
-            with open(text_ofcap_log, "w", encoding="utf-8") as text_ofcap:
-                subprocess.call(
-                    [
-                        "timeout",
-                        str(self.MAX_CTL_TIME),
-                        "tshark",
-                        "-l",
-                        "-n",
-                        "-Q",
-                        "-d",
-                        "tcp.port==%u,openflow" % self.port,
-                        "-O",
-                        "openflow_v4",
-                        "-Y",
-                        "openflow_v4",
-                        "-r",
-                        self.ofcap,
-                    ],
-                    stdout=text_ofcap,
-                    stdin=mininet_test_util.DEVNULL,
-                    stderr=mininet_test_util.DEVNULL,
-                    close_fds=True,
-                )
 
     def stop(self):  # pylint: disable=arguments-differ
         """Stop controller."""
         try:
             if self.CPROFILE:
                 os.kill(self.ryu_pid(), 2)
             else:
@@ -768,15 +824,15 @@
         cargs = " ".join(self._tls_cargs(port, ctl_privkey, ctl_cert, ca_certs))
         super().__init__(
             name,
             tmpdir,
             controller_intf,
             controller_ipv6,
             cargs=cargs,
-            command=self._command(env, tmpdir, name, " ".join(self.START_ARGS)),
+            command=self._command(env, name, " ".join(self.START_ARGS)),
             port=port,
             **kwargs
         )
 
     def listening(self):
         return (
             self.listen_port(self.ofctl_port)
@@ -803,11 +859,11 @@
     ):
         super().__init__(
             name,
             tmpdir,
             controller_intf,
             controller_ipv6,
             cargs=self._tls_cargs(port, ctl_privkey, ctl_cert, ca_certs),
-            command=self._command(env, tmpdir, name, "--gauge"),
+            command=self._command(env, name, "--gauge"),
             port=port,
             **kwargs
         )
```

### Comparing `c65faucet-1.0.53/clib/mininet_test_util.py` & `c65faucet-1.0.54/clib/mininet_test_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,20 +28,24 @@
 
 
 def flat_test_name(_id):
     """Return short form test name from TestCase ID."""
     return "-".join(_id.split(".")[1:])
 
 
-def lsof_tcp_listening_cmd(port, ipv, state, terse):
+def lsof_tcp_listening_cmd(port, ipv, state, terse, pid):
     """Return a command line for lsof for processes with specified TCP state."""
     terse_arg = ""
     if terse:
         terse_arg = "-t"
-    return "lsof -b -P -n %s -sTCP:%s -i %u -a -i tcp:%u" % (
+    pid_arg = ""
+    if pid:
+        pid_arg = "-p %u" % pid
+    return "lsof -b -P -n %s %s -sTCP:%s -i %u -a -i tcp:%u" % (
+        pid_arg,
         terse_arg,
         state,
         ipv,
         port,
     )
 
 
@@ -49,17 +53,17 @@
     """Return a command line for lsof for processes with specified TCP state."""
     terse_arg = ""
     if terse:
         terse_arg = "-t"
     return "lsof -b -P -n %s -i udp:%u -a" % (terse_arg, port)
 
 
-def tcp_listening_cmd(port, ipv=4, state="LISTEN", terse=True):
+def tcp_listening_cmd(port, ipv=4, state="LISTEN", terse=True, pid=None):
     """Call lsof_tcp_listening_cmd() with default args."""
-    return lsof_tcp_listening_cmd(port, ipv, state, terse)
+    return lsof_tcp_listening_cmd(port, ipv, state, terse, pid)
 
 
 def udp_listening_cmd(port, terse=True):
     """Call lsof_tcp_listening_cmd() with default args."""
     return lsof_udp_listening_cmd(port, terse)
```

### Comparing `c65faucet-1.0.53/clib/mininet_test_watcher.py` & `c65faucet-1.0.54/clib/mininet_test_watcher.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/clib/tcpdump_helper.py` & `c65faucet-1.0.54/clib/tcpdump_helper.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/clib/valve_test_lib.py` & `c65faucet-1.0.54/clib/valve_test_lib.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/debian/control` & `c65faucet-1.0.54/debian/control`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 Package: python3-faucet
 Architecture: all
 Depends: python3-influxdb (>= 2.12.0),
          python3-networkx (>= 1.9),
          python3-pbr (>= 1.9),
          python3-prometheus-client (>= 0.16.0), python3-prometheus-client (<< 0.16.1),
-         python3-ruamel.yaml (>= 0.17.21), python3-ruamel.yaml (<< 0.17.22),
+         python3-ruamel.yaml (>= 0.17.26), python3-ruamel.yaml (<< 0.17.27),
          python3-os-ken (>= 2.6.0), python3-os-ken (<< 2.6.1),
          python3-beka (>= 0.4.2), python3-beka (<< 0.4.3),
          python3-chewie (>= 0.0.25), python3-chewie (<< 0.0.26),
          python3-pytricia (>= 1.0.0),
          python3:any (>= 3.8~),
          ${misc:Depends},
 Suggests: python-faucet-doc, faucet, gauge
```

### Comparing `c65faucet-1.0.53/debian/copyright` & `c65faucet-1.0.54/debian/copyright`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/debian/faucet.postinst` & `c65faucet-1.0.54/debian/faucet.postinst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/debian/gauge.postinst` & `c65faucet-1.0.54/debian/gauge.postinst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/debian/rules` & `c65faucet-1.0.54/debian/rules`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docker/fuzz_config.sh` & `c65faucet-1.0.54/docker/fuzz_config.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docker/fuzz_packet.sh` & `c65faucet-1.0.54/docker/fuzz_packet.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docker/install-faucet.sh` & `c65faucet-1.0.54/docker/install-faucet.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docker/localtest.sh` & `c65faucet-1.0.54/docker/localtest.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docker/pip_deps.sh` & `c65faucet-1.0.54/docker/pip_deps.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docker/runtests.sh` & `c65faucet-1.0.54/docker/runtests.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docker/shard_tests.sh` & `c65faucet-1.0.54/docker/shard_tests.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docker-compose.yaml` & `c65faucet-1.0.54/docker-compose.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -13,29 +13,29 @@
             INFLUXDB_DB: 'faucet'
             INFLUXDB_HTTP_AUTH_ENABLED: 'true'
             INFLUXDB_ADMIN_USER: 'faucet'
             INFLUXDB_ADMIN_PASSWORD: 'faucet'
 
     prometheus:
         restart: always
-        image: 'prom/prometheus:v2.43.1'
+        image: 'prom/prometheus:v2.44.0'
         user: 'root'
         ports:
             - '9090:9090'
         volumes:
             - '${FAUCET_PREFIX}/opt/prometheus/:/prometheus'
             - './etc/prometheus/prometheus-docker-compose.yml:/etc/prometheus/prometheus.yml'
             - './etc/prometheus/faucet.rules.yml:/etc/prometheus/faucet.rules.yml'
         links:
             - faucet
             - gauge
 
     grafana:
         restart: always
-        image: 'grafana/grafana:9.5.1'
+        image: 'grafana/grafana:9.5.2'
         user: 'root'
         ports:
             - '3000:3000'
         volumes:
             - '${FAUCET_PREFIX}/opt/grafana:/var/lib/grafana'
         links:
             - influxdb
```

### Comparing `c65faucet-1.0.53/docs/Makefile` & `c65faucet-1.0.54/docs/Makefile`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/deployments/ONF_Faucet_deploy1.png` & `c65faucet-1.0.54/docs/_static/deployments/ONF_Faucet_deploy1.png`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/deployments/nznog17-physical-network.jpg` & `c65faucet-1.0.54/docs/_static/deployments/nznog17-physical-network.jpg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/deployments/nznog17-virtual-network.jpg` & `c65faucet-1.0.54/docs/_static/deployments/nznog17-virtual-network.jpg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/grafana-dashboards/faucet_instrumentation.json` & `c65faucet-1.0.54/docs/_static/grafana-dashboards/faucet_instrumentation.json`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/grafana-dashboards/faucet_inventory.json` & `c65faucet-1.0.54/docs/_static/grafana-dashboards/faucet_inventory.json`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/grafana-dashboards/faucet_port_statistics.json` & `c65faucet-1.0.54/docs/_static/grafana-dashboards/faucet_port_statistics.json`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/images/8021X-conf-diagram.svg` & `c65faucet-1.0.54/docs/_static/images/8021X-conf-diagram.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/images/faucet-architecture.svg` & `c65faucet-1.0.54/docs/_static/images/faucet-architecture.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/images/faucet-pipeline.png` & `c65faucet-1.0.54/docs/_static/images/faucet-pipeline.png`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/images/faucet-pipeline.svg` & `c65faucet-1.0.54/docs/_static/images/faucet-pipeline.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/images/faucet-pipeline.txt` & `c65faucet-1.0.54/docs/_static/images/faucet-pipeline.txt`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/images/gauge-nznog17.png` & `c65faucet-1.0.54/docs/_static/images/gauge-nznog17.png`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/images/gauge-snapshot1.png` & `c65faucet-1.0.54/docs/_static/images/gauge-snapshot1.png`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/images/gauge-snapshot2.png` & `c65faucet-1.0.54/docs/_static/images/gauge-snapshot2.png`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/images/gauge-snapshot3.png` & `c65faucet-1.0.54/docs/_static/images/gauge-snapshot3.png`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/images/tutorial-acls.svg` & `c65faucet-1.0.54/docs/_static/images/tutorial-acls.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/images/tutorial-bgp-routing.svg` & `c65faucet-1.0.54/docs/_static/images/tutorial-bgp-routing.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/images/tutorial-ivr.svg` & `c65faucet-1.0.54/docs/_static/images/tutorial-ivr.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/images/tutorial-multi-root-stack.svg` & `c65faucet-1.0.54/docs/_static/images/tutorial-multi-root-stack.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/images/tutorial-nfv-services.svg` & `c65faucet-1.0.54/docs/_static/images/tutorial-nfv-services.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/images/tutorial-stack-loop.svg` & `c65faucet-1.0.54/docs/_static/images/tutorial-stack-loop.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/images/tutorial-stack-tunnel.svg` & `c65faucet-1.0.54/docs/_static/images/tutorial-stack-tunnel.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/images/tutorial-stack.svg` & `c65faucet-1.0.54/docs/_static/images/tutorial-stack.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/images/tutorial-stackwithivr.svg` & `c65faucet-1.0.54/docs/_static/images/tutorial-stackwithivr.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/images/tutorial-static-routing.svg` & `c65faucet-1.0.54/docs/_static/images/tutorial-static-routing.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/images/tutorial-vlans.svg` & `c65faucet-1.0.54/docs/_static/images/tutorial-vlans.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/tutorial/cleanup` & `c65faucet-1.0.54/docs/_static/tutorial/cleanup`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/_static/tutorial/inter_switch_link` & `c65faucet-1.0.54/docs/_static/tutorial/inter_switch_link`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/architecture.rst` & `c65faucet-1.0.54/docs/architecture.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/conf.py` & `c65faucet-1.0.54/docs/conf.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/configuration.rst` & `c65faucet-1.0.54/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/developer_guide.rst` & `c65faucet-1.0.54/docs/developer_guide.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/external_resources.rst` & `c65faucet-1.0.54/docs/external_resources.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/fuzzing.rst` & `c65faucet-1.0.54/docs/fuzzing.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/installation.rst` & `c65faucet-1.0.54/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/intro.rst` & `c65faucet-1.0.54/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/monitoring.rst` & `c65faucet-1.0.54/docs/monitoring.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/release_notes/1.7.0.rst` & `c65faucet-1.0.54/docs/release_notes/1.7.0.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/release_notes/1.9.0.rst` & `c65faucet-1.0.54/docs/release_notes/1.9.0.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/testing.rst` & `c65faucet-1.0.54/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/tutorials/acls.rst` & `c65faucet-1.0.54/docs/tutorials/acls.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/tutorials/conntrack.rst` & `c65faucet-1.0.54/docs/tutorials/conntrack.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/tutorials/first_time.rst` & `c65faucet-1.0.54/docs/tutorials/first_time.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/tutorials/nfv_services.rst` & `c65faucet-1.0.54/docs/tutorials/nfv_services.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/tutorials/routing.rst` & `c65faucet-1.0.54/docs/tutorials/routing.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/tutorials/stacking.rst` & `c65faucet-1.0.54/docs/tutorials/stacking.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/tutorials/vlans.rst` & `c65faucet-1.0.54/docs/tutorials/vlans.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/vendors/allied-telesis/README_Allied_Telesis.rst` & `c65faucet-1.0.54/docs/vendors/allied-telesis/README_Allied_Telesis.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/vendors/cisco/README_Cisco.rst` & `c65faucet-1.0.54/docs/vendors/cisco/README_Cisco.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/vendors/hpe/README_Aruba.rst` & `c65faucet-1.0.54/docs/vendors/hpe/README_Aruba.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/vendors/lagopus/README_Lagopus.rst` & `c65faucet-1.0.54/docs/vendors/lagopus/README_Lagopus.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/vendors/northboundnetworks/README_ZodiacFX.rst` & `c65faucet-1.0.54/docs/vendors/northboundnetworks/README_ZodiacFX.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/vendors/northboundnetworks/README_ZodiacGX.rst` & `c65faucet-1.0.54/docs/vendors/northboundnetworks/README_ZodiacGX.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/vendors/northboundnetworks/conf-zodiac.sh` & `c65faucet-1.0.54/docs/vendors/northboundnetworks/conf-zodiac.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/vendors/noviflow/README_noviflow.rst` & `c65faucet-1.0.54/docs/vendors/noviflow/README_noviflow.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/vendors/ovs/README_OVS-DPDK.rst` & `c65faucet-1.0.54/docs/vendors/ovs/README_OVS-DPDK.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/vendors/ovs/faucet_ovs_test.png` & `c65faucet-1.0.54/docs/vendors/ovs/faucet_ovs_test.png`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/docs/vendors/ovs/faucet_testing_with_OVS_on_hardware.rst` & `c65faucet-1.0.54/docs/vendors/ovs/faucet_testing_with_OVS_on_hardware.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/etc/faucet/acls.yaml` & `c65faucet-1.0.54/etc/faucet/acls.yaml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/etc/faucet/faucet.yaml` & `c65faucet-1.0.54/etc/faucet/faucet.yaml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/etc/faucet/gauge.yaml` & `c65faucet-1.0.54/etc/faucet/gauge.yaml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/etc/prometheus/faucet.rules.yml` & `c65faucet-1.0.54/etc/prometheus/faucet.rules.yml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/etc/prometheus/prometheus.yml` & `c65faucet-1.0.54/etc/prometheus/prometheus.yml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/__main__.py` & `c65faucet-1.0.54/faucet/__main__.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/acl.py` & `c65faucet-1.0.54/faucet/acl.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/check_faucet_config.py` & `c65faucet-1.0.54/faucet/check_faucet_config.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/conf.py` & `c65faucet-1.0.54/faucet/conf.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/config_parser.py` & `c65faucet-1.0.54/faucet/config_parser.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/config_parser_util.py` & `c65faucet-1.0.54/faucet/config_parser_util.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/dp.py` & `c65faucet-1.0.54/faucet/dp.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/faucet.py` & `c65faucet-1.0.54/faucet/faucet.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/faucet_bgp.py` & `c65faucet-1.0.54/faucet/faucet_bgp.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/faucet_dot1x.py` & `c65faucet-1.0.54/faucet/faucet_dot1x.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/faucet_event.py` & `c65faucet-1.0.54/faucet/faucet_event.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/faucet_metrics.py` & `c65faucet-1.0.54/faucet/faucet_metrics.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/faucet_pipeline.py` & `c65faucet-1.0.54/faucet/faucet_pipeline.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/fctl.py` & `c65faucet-1.0.54/faucet/fctl.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/gauge.py` & `c65faucet-1.0.54/faucet/gauge.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/gauge_influx.py` & `c65faucet-1.0.54/faucet/gauge_influx.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/gauge_pollers.py` & `c65faucet-1.0.54/faucet/gauge_pollers.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/gauge_prom.py` & `c65faucet-1.0.54/faucet/gauge_prom.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/meter.py` & `c65faucet-1.0.54/faucet/meter.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/port.py` & `c65faucet-1.0.54/faucet/port.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/prom_client.py` & `c65faucet-1.0.54/faucet/prom_client.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/router.py` & `c65faucet-1.0.54/faucet/router.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/stack.py` & `c65faucet-1.0.54/faucet/stack.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/tfm_pipeline.py` & `c65faucet-1.0.54/faucet/tfm_pipeline.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/valve.py` & `c65faucet-1.0.54/faucet/valve.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/valve_acl.py` & `c65faucet-1.0.54/faucet/valve_acl.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/valve_coprocessor.py` & `c65faucet-1.0.54/faucet/valve_coprocessor.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/valve_lldp.py` & `c65faucet-1.0.54/faucet/valve_lldp.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/valve_manager_base.py` & `c65faucet-1.0.54/faucet/valve_manager_base.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/valve_of.py` & `c65faucet-1.0.54/faucet/valve_of.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/valve_of_old.py` & `c65faucet-1.0.54/faucet/valve_of_old.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/valve_outonly.py` & `c65faucet-1.0.54/faucet/valve_outonly.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/valve_packet.py` & `c65faucet-1.0.54/faucet/valve_packet.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/valve_pipeline.py` & `c65faucet-1.0.54/faucet/valve_pipeline.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/valve_route.py` & `c65faucet-1.0.54/faucet/valve_route.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/valve_ryuapp.py` & `c65faucet-1.0.54/faucet/valve_ryuapp.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/valve_stack.py` & `c65faucet-1.0.54/faucet/valve_stack.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/valve_switch.py` & `c65faucet-1.0.54/faucet/valve_switch.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/valve_switch_stack.py` & `c65faucet-1.0.54/faucet/valve_switch_stack.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/valve_switch_standalone.py` & `c65faucet-1.0.54/faucet/valve_switch_standalone.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/valve_table.py` & `c65faucet-1.0.54/faucet/valve_table.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/valve_util.py` & `c65faucet-1.0.54/faucet/valve_util.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/valves_manager.py` & `c65faucet-1.0.54/faucet/valves_manager.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/vlan.py` & `c65faucet-1.0.54/faucet/vlan.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/watcher.py` & `c65faucet-1.0.54/faucet/watcher.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/faucet/watcher_conf.py` & `c65faucet-1.0.54/faucet/watcher_conf.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/hw_switch_config.yaml` & `c65faucet-1.0.54/hw_switch_config.yaml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/ofctl_rest/ofctl_rest.py` & `c65faucet-1.0.54/ofctl_rest/ofctl_rest.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/ofctl_rest/wsgi.py` & `c65faucet-1.0.54/ofctl_rest/wsgi.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/setup.cfg` & `c65faucet-1.0.54/setup.cfg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/setup.py` & `c65faucet-1.0.54/setup.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/codecheck/src_files.sh` & `c65faucet-1.0.54/tests/codecheck/src_files.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/generative/fuzzer/config/fuzz_config.py` & `c65faucet-1.0.54/tests/generative/fuzzer/config/fuzz_config.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/generative/fuzzer/config/generate_dict.py` & `c65faucet-1.0.54/tests/generative/fuzzer/config/generate_dict.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/generative/fuzzer/packet/display_packet_crash.py` & `c65faucet-1.0.54/tests/generative/fuzzer/packet/display_packet_crash.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/http.ex2` & `c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/http.ex2`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/icmp.ex1` & `c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/icmp.ex1`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/icmp.ex2` & `c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/icmp.ex2`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/ipv4.ex1` & `c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/ipv4.ex1`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/generative/fuzzer/packet/examples/msger.ex1` & `c65faucet-1.0.54/tests/generative/fuzzer/packet/examples/msger.ex1`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/generative/fuzzer/packet/fake_packet.py` & `c65faucet-1.0.54/tests/generative/fuzzer/packet/fake_packet.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/generative/fuzzer/packet/fuzz_packet.py` & `c65faucet-1.0.54/tests/generative/fuzzer/packet/fuzz_packet.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/generative/integration/fault_tolerance_main.py` & `c65faucet-1.0.54/tests/generative/integration/fault_tolerance_main.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/generative/integration/fault_tolerance_tests.py` & `c65faucet-1.0.54/tests/generative/integration/fault_tolerance_tests.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/generative/unit/test_topology.py` & `c65faucet-1.0.54/tests/generative/unit/test_topology.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/integration/mininet_main.py` & `c65faucet-1.0.54/tests/integration/mininet_main.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/integration/mininet_multidp_tests.py` & `c65faucet-1.0.54/tests/integration/mininet_multidp_tests.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/integration/mininet_tests.py` & `c65faucet-1.0.54/tests/integration/mininet_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -2220,21 +2220,21 @@
         macvlan2_intf = "macvlan2"
         macvlan2_ipv4 = "10.0.0.101"
         self.add_macvlan(first_host, macvlan1_intf, ipa=macvlan1_ipv4, mode="vepa")
         self.add_macvlan(first_host, macvlan2_intf, mode="vepa")
         macvlan2_mac = self.get_host_intf_mac(first_host, macvlan2_intf)
         netns = self.hostns(first_host)
         setup_cmds = []
-        setup_cmds.extend(["ip link set %s netns %s" % (macvlan2_intf, netns)])
+        setup_cmds.extend(["link set %s netns %s" % (macvlan2_intf, netns)])
         for exec_cmd in (
             "ip address add %s/24 brd + dev %s" % (macvlan2_ipv4, macvlan2_intf),
             "ip link set %s up" % macvlan2_intf,
         ):
-            setup_cmds.append("ip netns exec %s %s" % (netns, exec_cmd))
-        self.quiet_commands(first_host, setup_cmds)
+            setup_cmds.append("netns exec %s %s" % (netns, exec_cmd))
+        first_host.run_ip_batch(setup_cmds)
         self.one_ipv4_ping(first_host, macvlan2_ipv4, intf=macvlan1_intf)
         self.one_ipv4_ping(first_host, second_host.IP())
         # Verify OUTPUT:IN_PORT flood rules are exercised.
         self.wait_nonzero_packet_count_flow(
             {"in_port": self.port_map["port_1"], "dl_dst": "ff:ff:ff:ff:ff:ff"},
             table_id=self._FLOOD_TABLE,
             actions=["OUTPUT:IN_PORT"],
@@ -3309,16 +3309,16 @@
                     self.add_macvlan(second_host, mac_intf, ipa=mac_ipv4)
                     macvlan_mac = self.get_mac_of_intf(mac_intf, second_host)
                     learned_mac_ports[macvlan_mac] = self.port_map["port_2"]
                     mac_ips.append((mac_ipv4, macvlan_mac))
                 return (mac_intfs, mac_ips, learned_mac_ports)
 
             def down_macvlans(macvlans):
-                for macvlan in macvlans:
-                    second_host.cmd("ip link set dev %s down" % macvlan)
+                down_cmds = ["link set dev %s down" % macvlan for macvlan in macvlans]
+                second_host.run_ip_batch(down_cmds)
 
             def learn_then_down_hosts(base, count):
                 mac_intfs, mac_ips, learned_mac_ports = add_macvlans(base, count)
                 self.verify_hosts_learned(
                     first_host, second_host, mac_ips, learned_mac_ports
                 )
                 down_macvlans(mac_intfs)
@@ -4826,44 +4826,43 @@
                 "ip link add name veth-loop1 type veth peer name veth-loop2",
                 "ip link set veth-loop1 up",
                 "ip link set veth-loop2 up",
                 # TODO: tune for loop mitigation performance.
                 "tc qdisc add dev veth-loop1 root tbf rate 1000kbps latency 10ms burst 1000",
                 "tc qdisc add dev veth-loop2 root tbf rate 1000kbps latency 10ms burst 1000",
                 # Connect one leg of veth pair to first host interface.
-                "brctl addbr br-loop1",
-                "brctl setfd br-loop1 0",
+                "ip link add dev br-loop1 type bridge",
+                "ip link set br-loop1 type bridge forward_delay 0",
                 "ip link set br-loop1 up",
-                "brctl addif br-loop1 veth-loop1",
-                "brctl addif br-loop1 %s-eth0" % second_host.name,
+                "ip link set dev veth-loop1 master br-loop1",
+                "ip link set dev %s-eth0 master br-loop1" % second_host.name,
                 # Connect other leg of veth pair.
-                "brctl addbr br-loop2",
-                "brctl setfd br-loop2 0",
+                "ip link add dev br-loop2 type bridge",
+                "ip link set br-loop2 type bridge forward_delay 0",
                 "ip link set br-loop2 up",
-                "brctl addif br-loop2 veth-loop2",
-                "brctl addif br-loop2 %s-eth1" % second_host.name,
+                "ip link set dev veth-loop2 master br-loop2",
+                "ip link set dev %s-eth1 master br-loop2" % second_host.name,
             ),
         )
 
         # Flood some traffic into the loop
         for _ in range(3):
             first_host.cmd("fping %s -c3 10.0.0.254" % self.FPING_ARGS_SHORT)
             end_bans = self.total_port_bans()
             if end_bans > start_bans:
                 return
             time.sleep(1)
         self.assertGreater(end_bans, start_bans)
 
         # Break the loop, and learning should work again
-        self.quiet_commands(
-            second_host,
-            (
-                "ip link set veth-loop1 down",
-                "ip link set veth-loop2 down",
-            ),
+        second_host.run_ip_batch(
+            [
+                "link set veth-loop1 down",
+                "link set veth-loop2 down",
+            ]
         )
         self.one_ipv4_ping(first_host, second_host.IP())
 
 
 class FaucetUntaggedIPv4LACPTest(FaucetTest):
     NUM_DPS = 1
     N_TAGGED = 0
@@ -5048,41 +5047,43 @@
         # Start with ports down.
         for port in lag_ports:
             self.set_port_down(self.port_map["port_%u" % port])
         require_lag_up_ports(0)
         orig_ip = first_host.IP()
         switch = self.first_switch()
         bond_members = [pair[0].name for pair in first_host.connectionsTo(switch)]
+        bond_cmds = []
         # Deconfigure bond members
         for bond_member in bond_members:
-            self.quiet_commands(
-                first_host,
-                (
-                    "ip link set %s down" % bond_member,
-                    "ip address flush dev %s" % bond_member,
-                ),
+            bond_cmds.extend(
+                [
+                    "link set %s down" % bond_member,
+                    "address flush dev %s" % bond_member,
+                ]
             )
         # Configure bond interface
-        self.quiet_commands(
-            first_host,
-            (
+        bond_cmds.extend(
+            [
                 (
-                    "ip link add %s address 0e:00:00:00:00:99 "
+                    "link add %s address 0e:00:00:00:00:99 "
                     "type bond mode 802.3ad lacp_rate fast miimon 100"
                 )
                 % bond,
-                "ip add add %s/24 dev %s" % (orig_ip, bond),
-                "ip link set %s up" % bond,
-            ),
+                "addr add %s/24 dev %s" % (orig_ip, bond),
+                "link set %s up" % bond,
+            ]
         )
         # Add bond members
         for bond_member in bond_members:
-            self.quiet_commands(
-                first_host, ("ip link set dev %s master %s" % (bond_member, bond),)
+            bond_cmds.extend(
+                [
+                    "link set dev %s master %s" % (bond_member, bond),
+                ]
             )
+        first_host.run_ip_batch(bond_cmds)
 
         for _flaps in range(2):
             # All ports down.
             for port in lag_ports:
                 self.set_port_down(self.port_map["port_%u" % port])
             require_lag_up_ports(0)
             # Pick a random port to come up.
@@ -5127,31 +5128,32 @@
     """Ensure remote LACP system ID mismatch is logged."""
 
     def test_untagged(self):
         first_host = self.hosts_name_ordered()[0]
         orig_ip = first_host.IP()
         switch = self.first_switch()
         bond_members = [pair[0].name for pair in first_host.connectionsTo(switch)]
+        bond_cmds = []
         for i, bond_member in enumerate(bond_members):
             bond = "bond%u" % i
-            self.quiet_commands(
-                first_host,
-                (
-                    "ip link set %s down" % bond_member,
-                    "ip address flush dev %s" % bond_member,
+            bond_cmds.extend(
+                [
+                    "link set %s down" % bond_member,
+                    "address flush dev %s" % bond_member,
                     (
-                        "ip link add %s address 0e:00:00:00:00:%2.2x "
+                        "link add %s address 0e:00:00:00:00:%2.2x "
                         "type bond mode 802.3ad lacp_rate fast miimon 100"
                     )
                     % (bond, i * 2 + i),
-                    "ip add add %s/24 dev %s" % (orig_ip, bond),
-                    "ip link set %s up" % bond,
-                    "ip link set dev %s master %s" % (bond_member, bond),
-                ),
+                    "addr add %s/24 dev %s" % (orig_ip, bond),
+                    "link set %s up" % bond,
+                    "link set dev %s master %s" % (bond_member, bond),
+                ]
             )
+        first_host.run_ip_batch(bond_cmds)
         self.wait_until_matching_lines_from_faucet_log_files(
             r".+actor system mismatch.+"
         )
 
 
 class FaucetUntaggedIPv4ControlPlaneFuzzTest(FaucetUntaggedTest):
     CONFIG_GLOBAL = """
@@ -6666,20 +6668,19 @@
                 tagged_vlans: [100]
             %(port_4)d:
                 tagged_vlans: [100]
 """
 
     def test_tagged(self):
         first_host, second_host = self.hosts_name_ordered()[:2]
-        self.quiet_commands(
-            first_host,
+        first_host.run_ip_batch(
             [
-                "ip link set %s type vlan egress %u:1" % (first_host.defaultIntf(), i)
+                "link set %s type vlan egress %u:1" % (first_host.defaultIntf(), i)
                 for i in range(0, 8)
-            ],
+            ]
         )
         self.one_ipv4_ping(first_host, second_host.IP())
         self.wait_nonzero_packet_count_flow(
             {"vlan_vid": 100, "vlan_pcp": 1}, table_id=self._PORT_ACL_TABLE
         )
         tcpdump_filter = "ether dst %s" % second_host.MAC()
         tcpdump_txt = self.tcpdump_helper(
@@ -6722,18 +6723,17 @@
                 tagged_vlans: [100]
             %(port_4)d:
                 tagged_vlans: [100]
 """
 
     def test_tagged(self):
         first_host, second_host = self.hosts_name_ordered()[:2]
-        self.quiet_commands(
-            first_host,
+        first_host.run_ip_batch(
             [
-                "ip link set %s type vlan egress %u:1" % (first_host.defaultIntf(), i)
+                "link set %s type vlan egress %u:1" % (first_host.defaultIntf(), i)
                 for i in range(0, 8)
             ],
         )
         self.one_ipv4_ping(first_host, second_host.IP())
         self.wait_nonzero_packet_count_flow(
             {"vlan_vid": 100, "vlan_pcp": 1}, table_id=self._PORT_ACL_TABLE
         )
@@ -7108,20 +7108,20 @@
         self.ping_all_when_learned()
         for host in self.hosts_name_ordered():
             setup_commands = []
             for vid in self.NEW_VIDS:
                 vlan_int = "%s.%u" % (host.intf_root_name, vid)
                 setup_commands.extend(
                     [
-                        "ip link add link %s name %s type vlan id %u"
+                        "link add link %s name %s type vlan id %u"
                         % (host.intf_root_name, vlan_int, vid),
-                        "ip link set dev %s up" % vlan_int,
+                        "link set dev %s up" % vlan_int,
                     ]
                 )
-            self.quiet_commands(host, setup_commands)
+            host.run_ip_batch(setup_commands)
         for host in self.hosts_name_ordered():
             rdisc6_commands = []
             for vid in self.NEW_VIDS:
                 vlan_int = "%s.%u" % (host.intf_root_name, vid)
                 rdisc6_commands.append("rdisc6 -r2 -w1 -q %s 2> /dev/null" % vlan_int)
             self.quiet_commands(host, rdisc6_commands)
         for vlan in self.NEW_VIDS:
```

### Comparing `c65faucet-1.0.53/tests/run_unit_tests.sh` & `c65faucet-1.0.54/tests/run_unit_tests.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/unit/clib/test_topo.py` & `c65faucet-1.0.54/tests/unit/clib/test_topo.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/unit/faucet/test_check_config.py` & `c65faucet-1.0.54/tests/unit/faucet/test_check_config.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/unit/faucet/test_config.py` & `c65faucet-1.0.54/tests/unit/faucet/test_config.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/unit/faucet/test_fctl.py` & `c65faucet-1.0.54/tests/unit/faucet/test_fctl.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/unit/faucet/test_main.py` & `c65faucet-1.0.54/tests/unit/faucet/test_main.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/unit/faucet/test_port.py` & `c65faucet-1.0.54/tests/unit/faucet/test_port.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/unit/faucet/test_valve.py` & `c65faucet-1.0.54/tests/unit/faucet/test_valve.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/unit/faucet/test_valve_config.py` & `c65faucet-1.0.54/tests/unit/faucet/test_valve_config.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/unit/faucet/test_valve_dot1x.py` & `c65faucet-1.0.54/tests/unit/faucet/test_valve_dot1x.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/unit/faucet/test_valve_egress.py` & `c65faucet-1.0.54/tests/unit/faucet/test_valve_egress.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/unit/faucet/test_valve_of.py` & `c65faucet-1.0.54/tests/unit/faucet/test_valve_of.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/unit/faucet/test_valve_stack.py` & `c65faucet-1.0.54/tests/unit/faucet/test_valve_stack.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/unit/faucet/test_valveapp_smoke.py` & `c65faucet-1.0.54/tests/unit/faucet/test_valveapp_smoke.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/unit/faucet/test_vlan.py` & `c65faucet-1.0.54/tests/unit/faucet/test_vlan.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/unit/gauge/test_config_gauge.py` & `c65faucet-1.0.54/tests/unit/gauge/test_config_gauge.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/unit/gauge/test_gauge.py` & `c65faucet-1.0.54/tests/unit/gauge/test_gauge.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/unit/gauge/test_main.py` & `c65faucet-1.0.54/tests/unit/gauge/test_main.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.53/tests/unit/packaging/test_packaging.py` & `c65faucet-1.0.54/tests/unit/packaging/test_packaging.py`

 * *Files identical despite different names*

