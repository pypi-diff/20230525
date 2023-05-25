# Comparing `tmp/orchestrator-core-1.0.2rc3.tar.gz` & `tmp/orchestrator_core-1.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchestrator-core-1.0.2rc3.tar", last modified: Fri May  5 08:14:09 2023, max compression
+gzip compressed data, was "orchestrator_core-1.1.0rc1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `orchestrator-core-1.0.2rc3.tar` & `orchestrator_core-1.1.0rc1.tar`

### file list

```diff
@@ -1,316 +1,330 @@
--rw-r--r--   0        0        0      346 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.bumpversion.cfg
--rw-r--r--   0        0        0       33 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.coveragerc
--rw-r--r--   0        0        0     2620 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.github/workflows/README.md
--rw-r--r--   0        0        0     1851 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.github/workflows/build-push-container.yml
--rw-r--r--   0        0        0      291 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.github/workflows/changelog.yml
--rw-r--r--   0        0        0     2341 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      371 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.github/workflows/gh-pages.yml
--rw-r--r--   0        0        0      550 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.github/workflows/publish-package.yml
--rw-r--r--   0        0        0     1163 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.github/workflows/run-linting-tests.yml
--rw-r--r--   0        0        0     2106 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.github/workflows/run-unit-tests.yml
--rw-r--r--   0        0        0     1985 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.github/workflows/scheduled-build.yml
--rw-r--r--   0        0        0     1782 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.gitignore
--rw-r--r--   0        0        0     2074 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1150 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.stignore
--rw-r--r--   0        0        0    29713 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/CHANGELOG.md
--rw-r--r--   0        0        0      333 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/Dockerfile
--rw-r--r--   0        0        0    11409 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/LICENSE
--rw-r--r--   0        0        0      150 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/NOTICE
--rw-r--r--   0        0        0     4965 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/README.md
--rw-r--r--   0        0        0       76 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/codecov.yml
--rw-r--r--   0        0        0       45 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/application/api.md
--rw-r--r--   0        0        0    16572 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/application/cli.md
--rw-r--r--   0        0        0    10741 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/application/domainmodels.md
--rw-r--r--   0        0        0     4347 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/application/forms.md
--rw-r--r--   0        0        0    48867 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/application/openapi.json
--rw-r--r--   0        0        0     1565 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/application/python.md
--rw-r--r--   0        0        0     5641 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/application/scaling.md
--rw-r--r--   0        0        0     5514 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/application/tasks.md
--rw-r--r--   0        0        0     2371 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/application/websockets.md
--rw-r--r--   0        0        0    11465 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/application/workflow.md
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/orchestration/philosophy.md
--rw-r--r--   0        0        0     2080 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/tldr.md
--rw-r--r--   0        0        0     1694 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/contributing/guidelines.md
--rw-r--r--   0        0        0    10000 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/contributing/testing.md
--rw-r--r--   0        0        0      452 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/css/custom.css
--rw-r--r--   0        0        0     2165 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/css/termynal.css
--rw-r--r--   0        0        0     2135 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/getting-started/base.md
--rw-r--r--   0        0        0      928 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/getting-started/development.md
--rw-r--r--   0        0        0     2367 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/index.md
--rw-r--r--   0        0        0     3897 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/js/termynal.js
--rw-r--r--   0        0        0     5605 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/create-user-group.md
--rw-r--r--   0        0        0     4438 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/create-user.md
--rw-r--r--   0        0        0     7471 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/database-migration.md
--rw-r--r--   0        0        0     3700 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/debian.md
--rw-r--r--   0        0        0     3063 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/docker.md
--rw-r--r--   0        0        0     6106 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/domain-models.md
--rw-r--r--   0        0        0     1952 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/explore.md
--rw-r--r--   0        0        0     3996 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/input-forms.md
--rw-r--r--   0        0        0     3595 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/macos.md
--rw-r--r--   0        0        0     3411 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/modify-user-group.md
--rw-r--r--   0        0        0     2143 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/modify-user.md
--rw-r--r--   0        0        0     2885 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/overview.md
--rw-r--r--   0        0        0     4547 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/register-workflows.md
--rw-r--r--   0        0        0      786 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/scenario.md
--rw-r--r--   0        0        0     1013 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/start-applications.md
--rw-r--r--   0        0        0     2988 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/terminate-user-group.md
--rw-r--r--   0        0        0     1332 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/terminate-user.md
--rw-r--r--   0        0        0     3637 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/workflow-introduction.md
--rw-r--r--   0        0        0    46296 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/docs/workshops/images/metadata_products.png
--rw-r--r--   0        0        0      771 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/examples/basic/basic_orchestrator.py
--rw-r--r--   0        0        0     3601 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/mkdocs.yml
--rw-r--r--   0        0        0     1267 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/mutmut_config.py
--rw-r--r--   0        0        0     1098 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/__init__.py
--rw-r--r--   0        0        0      571 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/__init__.py
--rw-r--r--   0        0        0      571 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/__init__.py
--rw-r--r--   0        0        0     2871 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/api.py
--rw-r--r--   0        0        0      571 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/__init__.py
--rw-r--r--   0        0        0     2841 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/fixed_input.py
--rw-r--r--   0        0        0     1236 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/health.py
--rw-r--r--   0        0        0    12955 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/processes.py
--rw-r--r--   0        0        0     2703 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/product_blocks.py
--rw-r--r--   0        0        0     3331 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/products.py
--rw-r--r--   0        0        0     2552 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/resource_types.py
--rw-r--r--   0        0        0     5848 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/settings.py
--rw-r--r--   0        0        0     2866 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
--rw-r--r--   0        0        0    11510 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/subscriptions.py
--rw-r--r--   0        0        0      996 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/translations.py
--rw-r--r--   0        0        0     1833 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/user.py
--rw-r--r--   0        0        0     1961 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/workflows.py
--rw-r--r--   0        0        0     1543 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/error_handling.py
--rw-r--r--   0        0        0    11705 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/helpers.py
--rw-r--r--   0        0        0     5636 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/models.py
--rw-r--r--   0        0        0     7395 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/app.py
--rw-r--r--   0        0        0      571 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/__init__.py
--rw-r--r--   0        0        0    13831 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/database.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/__init__.py
--rw-r--r--   0        0        0     6853 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
--rw-r--r--   0        0        0     1953 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/helpers.py
--rw-r--r--   0        0        0    10653 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
--rw-r--r--   0        0        0     9423 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/product_helpers.py
--rw-r--r--   0        0        0    24095 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
--rw-r--r--   0        0        0     1439 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/types.py
--rw-r--r--   0        0        0      571 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/helpers/__init__.py
--rw-r--r--   0        0        0     1165 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/helpers/input_helpers.py
--rw-r--r--   0        0        0      830 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/helpers/print_helpers.py
--rw-r--r--   0        0        0      871 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/main.py
--rwxr-xr-x   0        0        0    20183 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/migrate_domain_models.py
--rwxr-xr-x   0        0        0     8943 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/migrate_workflows.py
--rw-r--r--   0        0        0     4113 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/migration_helpers.py
--rw-r--r--   0        0        0     1896 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/scheduler.py
--rw-r--r--   0        0        0      571 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/config/__init__.py
--rw-r--r--   0        0        0      770 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/config/assignee.py
--rw-r--r--   0        0        0     2920 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/db/__init__.py
--rw-r--r--   0        0        0    10288 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/db/database.py
--rw-r--r--   0        0        0      301 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/db/filters/__init__.py
--rw-r--r--   0        0        0     3415 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/db/filters/filters.py
--rw-r--r--   0        0        0     4507 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/db/filters/process.py
--rw-r--r--   0        0        0    23116 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/db/models.py
--rw-r--r--   0        0        0      104 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/db/range/__init__.py
--rw-r--r--   0        0        0     1439 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/db/range/range.py
--rw-r--r--   0        0        0      240 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/db/sorting/__init__.py
--rw-r--r--   0        0        0      368 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/db/sorting/process.py
--rw-r--r--   0        0        0     3413 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/db/sorting/sorting.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/devtools/__init__.py
--rw-r--r--   0        0        0    16866 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/devtools/populator.py
--rw-r--r--   0        0        0     2554 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/distlock/__init__.py
--rw-r--r--   0        0        0     2528 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/distlock/distlock_manager.py
--rw-r--r--   0        0        0      571 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/distlock/managers/__init__.py
--rw-r--r--   0        0        0     3062 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/distlock/managers/memory_distlock_manager.py
--rw-r--r--   0        0        0     3315 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/distlock/managers/redis_distlock_manager.py
--rw-r--r--   0        0        0      924 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/domain/__init__.py
--rw-r--r--   0        0        0    62844 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/domain/base.py
--rw-r--r--   0        0        0     2694 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/domain/lifecycle.py
--rw-r--r--   0        0        0     2977 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/exception_handlers.py
--rw-r--r--   0        0        0     5434 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/forms/__init__.py
--rw-r--r--   0        0        0     2145 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/forms/network_type_validators.py
--rw-r--r--   0        0        0    11483 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/forms/validators.py
--rw-r--r--   0        0        0     4481 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/graphql/__init__.py
--rw-r--r--   0        0        0     4265 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/graphql/authentication.py
--rw-r--r--   0        0        0     1350 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/graphql/extensions/ErrorCollectorExtension.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/graphql/extensions/__init__.py
--rw-r--r--   0        0        0     4325 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/graphql/extensions/deprecation_checker_extension.py
--rw-r--r--   0        0        0     2105 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/graphql/pagination.py
--rw-r--r--   0        0        0     4097 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/graphql/resolvers/process.py
--rw-r--r--   0        0        0     2259 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/graphql/schemas/process.py
--rw-r--r--   0        0        0     2056 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/graphql/types.py
--rw-r--r--   0        0        0      992 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/graphql/utils/get_selected_fields.py
--rw-r--r--   0        0        0       39 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/README
--rw-r--r--   0        0        0      873 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/alembic.ini
--rwxr-xr-x   0        0        0     3365 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/env.py
--rw-r--r--   0        0        0    40397 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/helpers.py
--rw-r--r--   0        0        0      510 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/script.py.mako
--rw-r--r--   0        0        0      905 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/templates/alembic.ini.j2
--rwxr-xr-x   0        0        0     2821 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/templates/env.py.j2
--rw-r--r--   0        0        0       98 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/templates/helpers.py.j2
--rw-r--r--   0        0        0     2641 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
--rw-r--r--   0        0        0     1266 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
--rw-r--r--   0        0        0    38591 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
--rw-r--r--   0        0        0      951 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
--rw-r--r--   0        0        0     1213 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
--rw-r--r--   0        0        0     1556 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
--rw-r--r--   0        0        0     5105 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
--rw-r--r--   0        0        0     7723 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/py.typed
--rw-r--r--   0        0        0     1090 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schedules/__init__.py
--rw-r--r--   0        0        0      832 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schedules/resume_workflows.py
--rw-r--r--   0        0        0     1535 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schedules/scheduling.py
--rw-r--r--   0        0        0      821 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schedules/task_vacuum.py
--rw-r--r--   0        0        0     1053 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schedules/validate_products.py
--rw-r--r--   0        0        0     2131 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schedules/validate_subscriptions.py
--rw-r--r--   0        0        0     2631 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/__init__.py
--rw-r--r--   0        0        0      886 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/base.py
--rw-r--r--   0        0        0     1275 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/engine_settings.py
--rw-r--r--   0        0        0     1346 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/fixed_input.py
--rw-r--r--   0        0        0      842 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/problem_detail.py
--rw-r--r--   0        0        0     3390 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/process.py
--rw-r--r--   0        0        0     1670 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/product.py
--rw-r--r--   0        0        0     1735 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/product_block.py
--rw-r--r--   0        0        0      951 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/resource_type.py
--rw-r--r--   0        0        0     3180 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/subscription.py
--rw-r--r--   0        0        0     1013 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/subscription_descriptions.py
--rw-r--r--   0        0        0     1803 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/workflow.py
--rw-r--r--   0        0        0     1797 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/security.py
--rw-r--r--   0        0        0      571 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/services/__init__.py
--rw-r--r--   0        0        0     3586 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/services/celery.py
--rw-r--r--   0        0        0    22351 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/services/processes.py
--rw-r--r--   0        0        0     1530 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/services/products.py
--rw-r--r--   0        0        0     3879 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/services/settings.py
--rw-r--r--   0        0        0    24204 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/services/subscriptions.py
--rw-r--r--   0        0        0     5695 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/services/tasks.py
--rw-r--r--   0        0        0     1719 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/services/translations.py
--rw-r--r--   0        0        0     3741 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/settings.py
--rw-r--r--   0        0        0      731 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/targets.py
--rw-r--r--   0        0        0     9397 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/types.py
--rw-r--r--   0        0        0      571 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/__init__.py
--rw-r--r--   0        0        0     5593 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/crypt.py
--rw-r--r--   0        0        0     1477 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/datetime.py
--rw-r--r--   0        0        0     6207 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/docs.py
--rw-r--r--   0        0        0     3839 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/errors.py
--rw-r--r--   0        0        0     8079 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/functional.py
--rw-r--r--   0        0        0     2817 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/helpers.py
--rw-r--r--   0        0        0     8512 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/json.py
--rw-r--r--   0        0        0     3403 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/redis.py
--rw-r--r--   0        0        0     2972 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/show_process.py
--rw-r--r--   0        0        0     2395 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/speed.py
--rw-r--r--   0        0        0    13148 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/state.py
--rw-r--r--   0        0        0     1077 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/strings.py
--rw-r--r--   0        0        0     7231 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/vlans.py
--rw-r--r--   0        0        0     1323 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/version.py
--rw-r--r--   0        0        0     4476 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/websocket/__init__.py
--rw-r--r--   0        0        0     3535 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/websocket/managers/broadcast_websocket_manager.py
--rw-r--r--   0        0        0     3194 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/websocket/managers/memory_websocket_manager.py
--rw-r--r--   0        0        0     2900 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/websocket/websocket_manager.py
--rw-r--r--   0        0        0    33615 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/workflow.py
--rw-r--r--   0        0        0     4085 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2135 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/workflows/modify_note.py
--rw-r--r--   0        0        0      909 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/workflows/removed_workflow.py
--rw-r--r--   0        0        0     9204 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/workflows/steps.py
--rw-r--r--   0        0        0      571 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     1510 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/workflows/tasks/cleanup_tasks_log.py
--rw-r--r--   0        0        0     2120 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/workflows/tasks/resume_workflows.py
--rw-r--r--   0        0        0     8335 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/workflows/tasks/validate_products.py
--rw-r--r--   0        0        0      684 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/workflows/translations/en-GB.json
--rw-r--r--   0        0        0     8839 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/orchestrator/workflows/utils.py
--rw-r--r--   0        0        0     4574 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/pyproject.toml
--rw-r--r--   0        0        0     2413 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/setup.cfg
--rw-r--r--   0        0        0      665 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/setup.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/__init__.py
--rw-r--r--   0        0        0     3199 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
--rw-r--r--   0        0        0     1855 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
--rw-r--r--   0        0        0     1544 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/main.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
--rw-r--r--   0        0        0     1608 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
--rw-r--r--   0        0        0     1211 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2828 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
--rw-r--r--   0        0        0      588 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/test_test_product.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/__init__.py
--rw-r--r--   0        0        0     5786 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_caching.py
--rw-r--r--   0        0        0     1578 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_fixed_inputs.py
--rw-r--r--   0        0        0     1192 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_health.py
--rw-r--r--   0        0        0     3049 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_helpers.py
--rw-r--r--   0        0        0     1747 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_models.py
--rw-r--r--   0        0        0    20143 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_processes.py
--rw-r--r--   0        0        0    16019 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_processes_ws.py
--rw-r--r--   0        0        0     3742 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_product_blocks.py
--rw-r--r--   0        0        0     7942 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_products.py
--rw-r--r--   0        0        0     2486 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_resource_types.py
--rw-r--r--   0        0        0     1772 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_settings.py
--rw-r--r--   0        0        0     2985 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_subscription_customer_descriptions.py
--rw-r--r--   0        0        0    37733 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_subscriptions.py
--rw-r--r--   0        0        0     2394 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_workflows.py
--rw-r--r--   0        0        0    25724 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
--rw-r--r--   0        0        0    27170 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
--rw-r--r--   0        0        0      422 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/config.py
--rw-r--r--   0        0        0    20845 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/domain/__init__.py
--rw-r--r--   0        0        0    50537 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/domain/test_base.py
--rw-r--r--   0        0        0     8092 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/domain/test_base_with_list_union.py
--rw-r--r--   0        0        0     4493 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/domain/test_base_with_union.py
--rw-r--r--   0        0        0     2824 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/__init__.py
--rw-r--r--   0        0        0     7530 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/processes.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/__init__.py
--rw-r--r--   0        0        0     1683 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
--rw-r--r--   0        0        0     2569 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
--rw-r--r--   0        0        0     1609 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
--rw-r--r--   0        0        0     2642 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
--rw-r--r--   0        0        0     2590 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
--rw-r--r--   0        0        0     1232 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
--rw-r--r--   0        0        0     1055 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/__init__.py
--rw-r--r--   0        0        0     2372 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
--rw-r--r--   0        0        0     2262 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
--rw-r--r--   0        0        0     4191 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
--rw-r--r--   0        0        0     3240 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_one.py
--rw-r--r--   0        0        0     2341 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
--rw-r--r--   0        0        0     2977 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
--rw-r--r--   0        0        0     2298 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
--rw-r--r--   0        0        0     2282 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
--rw-r--r--   0        0        0     1671 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
--rw-r--r--   0        0        0     1898 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_union.py
--rw-r--r--   0        0        0      527 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/resource_types.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/forms/__init__.py
--rw-r--r--   0        0        0     1462 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/forms/shared.py
--rw-r--r--   0        0        0    25426 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/forms/test_generic_validators.py
--rw-r--r--   0        0        0     7644 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/forms/test_network_validators.py
--rw-r--r--   0        0        0     6626 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/forms/test_post_process.py
--rw-r--r--   0        0        0    10081 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/graphql/test_processes.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/schedules/__init__.py
--rw-r--r--   0        0        0      807 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/schedules/test_scheduling.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/services/__init__.py
--rw-r--r--   0        0        0    26695 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/services/test_processes.py
--rw-r--r--   0        0        0     1083 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/services/test_products.py
--rw-r--r--   0        0        0     5830 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/services/test_subscriptions.py
--rw-r--r--   0        0        0     2100 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/services/test_translations.py
--rw-r--r--   0        0        0     7353 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/test_db.py
--rw-r--r--   0        0        0      385 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/test_types.py
--rw-r--r--   0        0        0    12048 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/test_workflow.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/utils/__init__.py
--rw-r--r--   0        0        0      163 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_datetime.py
--rw-r--r--   0        0        0     1871 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_errors.py
--rw-r--r--   0        0        0     3517 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_functional.py
--rw-r--r--   0        0        0     3052 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_json.py
--rw-r--r--   0        0        0     1144 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_speed.py
--rw-r--r--   0        0        0    11501 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_state.py
--rw-r--r--   0        0        0      192 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_strings.py
--rw-r--r--   0        0        0     8339 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_vlans.py
--rw-r--r--   0        0        0    12492 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/workflows/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/workflows/conftest.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/workflows/shared/__init__.py
--rw-r--r--   0        0        0     2091 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/workflows/shared/test_validate_subscriptions.py
--rw-r--r--   0        0        0        0 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     2039 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
--rw-r--r--   0        0        0     2584 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/workflows/tasks/test_resume_workflows.py
--rw-r--r--   0        0        0      288 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/workflows/tasks/test_validate_products.py
--rw-r--r--   0        0        0     3390 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/workflows/test_config_db_code.py
--rw-r--r--   0        0        0     1877 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/workflows/test_generic_workflow_steps.py
--rw-r--r--   0        0        0      987 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/workflows/test_modify_note.py
--rw-r--r--   0        0        0     5285 1970-01-01 00:00:00.000000 orchestrator-core-1.0.2rc3/PKG-INFO
+-rw-r--r--   0        0        0      346 2023-05-24 07:44:35.502022 orchestrator_core-1.1.0rc1/.bumpversion.cfg
+-rw-r--r--   0        0        0       33 2023-05-24 07:44:35.502022 orchestrator_core-1.1.0rc1/.coveragerc
+-rw-r--r--   0        0        0     2620 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.github/workflows/README.md
+-rw-r--r--   0        0        0     1851 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.github/workflows/build-push-container.yml
+-rw-r--r--   0        0        0      291 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0     2341 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      371 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.github/workflows/gh-pages.yml
+-rw-r--r--   0        0        0      550 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.github/workflows/publish-package.yml
+-rw-r--r--   0        0        0     1163 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.github/workflows/run-linting-tests.yml
+-rw-r--r--   0        0        0     2113 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0        0        0     1985 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.github/workflows/scheduled-build.yml
+-rw-r--r--   0        0        0     1782 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.gitignore
+-rw-r--r--   0        0        0     2074 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1150 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/.stignore
+-rw-r--r--   0        0        0    29835 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0      333 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/Dockerfile
+-rw-r--r--   0        0        0    11409 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/LICENSE
+-rw-r--r--   0        0        0      150 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/NOTICE
+-rw-r--r--   0        0        0     4965 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/README.md
+-rw-r--r--   0        0        0       76 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/codecov.yml
+-rw-r--r--   0        0        0       45 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/application/api.md
+-rw-r--r--   0        0        0    16572 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/application/cli.md
+-rw-r--r--   0        0        0    10741 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/application/domainmodels.md
+-rw-r--r--   0        0        0    13931 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/application/forms.md
+-rw-r--r--   0        0        0    48867 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/application/openapi.json
+-rw-r--r--   0        0        0     1565 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/application/python.md
+-rw-r--r--   0        0        0     5641 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/application/scaling.md
+-rw-r--r--   0        0        0     5514 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/application/tasks.md
+-rw-r--r--   0        0        0     2371 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/application/websockets.md
+-rw-r--r--   0        0        0    11465 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/application/workflow.md
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/orchestration/philosophy.md
+-rw-r--r--   0        0        0     2080 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/architecture/tldr.md
+-rw-r--r--   0        0        0     1694 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/contributing/guidelines.md
+-rw-r--r--   0        0        0    10000 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/contributing/testing.md
+-rw-r--r--   0        0        0      452 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/css/custom.css
+-rw-r--r--   0        0        0     2165 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/css/termynal.css
+-rw-r--r--   0        0        0     2135 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/getting-started/base.md
+-rw-r--r--   0        0        0      928 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/getting-started/development.md
+-rw-r--r--   0        0        0     2367 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/index.md
+-rw-r--r--   0        0        0     3897 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/js/termynal.js
+-rw-r--r--   0        0        0     5605 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/create-user-group.md
+-rw-r--r--   0        0        0     4438 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/create-user.md
+-rw-r--r--   0        0        0     7471 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/database-migration.md
+-rw-r--r--   0        0        0     3700 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/debian.md
+-rw-r--r--   0        0        0     3063 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/docker.md
+-rw-r--r--   0        0        0     6106 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/domain-models.md
+-rw-r--r--   0        0        0     1952 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/explore.md
+-rw-r--r--   0        0        0     3996 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/input-forms.md
+-rw-r--r--   0        0        0     3595 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/macos.md
+-rw-r--r--   0        0        0     3411 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/modify-user-group.md
+-rw-r--r--   0        0        0     2143 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/modify-user.md
+-rw-r--r--   0        0        0     2885 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/overview.md
+-rw-r--r--   0        0        0     4547 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/register-workflows.md
+-rw-r--r--   0        0        0      786 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/scenario.md
+-rw-r--r--   0        0        0     1013 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/start-applications.md
+-rw-r--r--   0        0        0     2988 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/terminate-user-group.md
+-rw-r--r--   0        0        0     1332 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/terminate-user.md
+-rw-r--r--   0        0        0     3637 2023-05-24 07:44:35.506023 orchestrator_core-1.1.0rc1/docs/workshops/beginner/workflow-introduction.md
+-rw-r--r--   0        0        0    46296 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/docs/workshops/images/metadata_products.png
+-rw-r--r--   0        0        0      771 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/examples/basic/basic_orchestrator.py
+-rw-r--r--   0        0        0     3601 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/mkdocs.yml
+-rw-r--r--   0        0        0     1267 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/mutmut_config.py
+-rw-r--r--   0        0        0     1098 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/__init__.py
+-rw-r--r--   0        0        0      571 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/__init__.py
+-rw-r--r--   0        0        0      571 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/__init__.py
+-rw-r--r--   0        0        0     2871 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/api.py
+-rw-r--r--   0        0        0      571 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/__init__.py
+-rw-r--r--   0        0        0     2841 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/fixed_input.py
+-rw-r--r--   0        0        0     1236 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/health.py
+-rw-r--r--   0        0        0    12955 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/processes.py
+-rw-r--r--   0        0        0     2703 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/product_blocks.py
+-rw-r--r--   0        0        0     3331 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/products.py
+-rw-r--r--   0        0        0     2552 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/resource_types.py
+-rw-r--r--   0        0        0     5803 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/settings.py
+-rw-r--r--   0        0        0     2866 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    11510 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/subscriptions.py
+-rw-r--r--   0        0        0      996 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/translations.py
+-rw-r--r--   0        0        0     1833 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/user.py
+-rw-r--r--   0        0        0     1961 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/workflows.py
+-rw-r--r--   0        0        0     1543 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/error_handling.py
+-rw-r--r--   0        0        0    11705 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/helpers.py
+-rw-r--r--   0        0        0     5636 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/api/models.py
+-rw-r--r--   0        0        0     7395 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/app.py
+-rw-r--r--   0        0        0      571 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/__init__.py
+-rw-r--r--   0        0        0    13831 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/database.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/__init__.py
+-rw-r--r--   0        0        0     6853 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
+-rw-r--r--   0        0        0     1953 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/helpers.py
+-rw-r--r--   0        0        0    10653 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
+-rw-r--r--   0        0        0     9423 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/product_helpers.py
+-rw-r--r--   0        0        0    24095 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
+-rw-r--r--   0        0        0     1439 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/types.py
+-rw-r--r--   0        0        0      571 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/helpers/__init__.py
+-rw-r--r--   0        0        0     1165 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/helpers/input_helpers.py
+-rw-r--r--   0        0        0      830 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/helpers/print_helpers.py
+-rw-r--r--   0        0        0      871 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/main.py
+-rwxr-xr-x   0        0        0    20183 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/migrate_domain_models.py
+-rwxr-xr-x   0        0        0     8943 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/migrate_workflows.py
+-rw-r--r--   0        0        0     4113 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/migration_helpers.py
+-rw-r--r--   0        0        0     1896 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/cli/scheduler.py
+-rw-r--r--   0        0        0      571 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/config/__init__.py
+-rw-r--r--   0        0        0      770 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/config/assignee.py
+-rw-r--r--   0        0        0     2920 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/__init__.py
+-rw-r--r--   0        0        0    10288 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/database.py
+-rw-r--r--   0        0        0      301 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/filters/__init__.py
+-rw-r--r--   0        0        0     3415 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/filters/filters.py
+-rw-r--r--   0        0        0     4507 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/filters/process.py
+-rw-r--r--   0        0        0     1924 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/filters/product.py
+-rw-r--r--   0        0        0    23116 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/models.py
+-rw-r--r--   0        0        0      104 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/range/__init__.py
+-rw-r--r--   0        0        0     1439 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/range/range.py
+-rw-r--r--   0        0        0      240 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/sorting/__init__.py
+-rw-r--r--   0        0        0      368 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/sorting/process.py
+-rw-r--r--   0        0        0      346 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/sorting/product.py
+-rw-r--r--   0        0        0     3413 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/db/sorting/sorting.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/devtools/__init__.py
+-rw-r--r--   0        0        0    16866 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/devtools/populator.py
+-rw-r--r--   0        0        0     2508 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/distlock/__init__.py
+-rw-r--r--   0        0        0     2533 2023-05-24 07:44:35.510022 orchestrator_core-1.1.0rc1/orchestrator/distlock/distlock_manager.py
+-rw-r--r--   0        0        0      571 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/distlock/managers/__init__.py
+-rw-r--r--   0        0        0     3062 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/distlock/managers/memory_distlock_manager.py
+-rw-r--r--   0        0        0     3329 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/distlock/managers/redis_distlock_manager.py
+-rw-r--r--   0        0        0      924 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/domain/__init__.py
+-rw-r--r--   0        0        0    62844 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/domain/base.py
+-rw-r--r--   0        0        0     2694 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/domain/lifecycle.py
+-rw-r--r--   0        0        0     2977 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/exception_handlers.py
+-rw-r--r--   0        0        0     5434 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/forms/__init__.py
+-rw-r--r--   0        0        0     2145 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/forms/network_type_validators.py
+-rw-r--r--   0        0        0    11483 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/forms/validators.py
+-rw-r--r--   0        0        0     5091 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/__init__.py
+-rw-r--r--   0        0        0     1350 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/extensions/ErrorCollectorExtension.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/extensions/__init__.py
+-rw-r--r--   0        0        0     4325 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/extensions/deprecation_checker_extension.py
+-rw-r--r--   0        0        0     2105 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/pagination.py
+-rw-r--r--   0        0        0      317 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/resolvers/__init__.py
+-rw-r--r--   0        0        0     4097 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/resolvers/process.py
+-rw-r--r--   0        0        0     2576 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/resolvers/product.py
+-rw-r--r--   0        0        0     3727 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/resolvers/settings.py
+-rw-r--r--   0        0        0      203 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/schemas/errors.py
+-rw-r--r--   0        0        0      513 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/schemas/fixed_input.py
+-rw-r--r--   0        0        0     2259 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/schemas/process.py
+-rw-r--r--   0        0        0      690 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/schemas/product.py
+-rw-r--r--   0        0        0      530 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/schemas/product_block.py
+-rw-r--r--   0        0        0      305 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/schemas/resource_type.py
+-rw-r--r--   0        0        0      980 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/schemas/settings.py
+-rw-r--r--   0        0        0      172 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/schemas/workflow.py
+-rw-r--r--   0        0        0     2056 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/types.py
+-rw-r--r--   0        0        0      114 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/utils/__init__.py
+-rw-r--r--   0        0        0      992 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/graphql/utils/get_selected_fields.py
+-rw-r--r--   0        0        0       39 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/README
+-rw-r--r--   0        0        0      873 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/alembic.ini
+-rwxr-xr-x   0        0        0     3365 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/env.py
+-rw-r--r--   0        0        0    40397 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/helpers.py
+-rw-r--r--   0        0        0      510 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/script.py.mako
+-rw-r--r--   0        0        0      905 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/templates/alembic.ini.j2
+-rwxr-xr-x   0        0        0     2821 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/templates/env.py.j2
+-rw-r--r--   0        0        0       98 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/templates/helpers.py.j2
+-rw-r--r--   0        0        0     2641 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
+-rw-r--r--   0        0        0     1266 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
+-rw-r--r--   0        0        0    38591 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
+-rw-r--r--   0        0        0      951 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
+-rw-r--r--   0        0        0     1213 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
+-rw-r--r--   0        0        0     1556 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
+-rw-r--r--   0        0        0     5105 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
+-rw-r--r--   0        0        0     7723 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/py.typed
+-rw-r--r--   0        0        0     1090 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schedules/__init__.py
+-rw-r--r--   0        0        0      832 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schedules/resume_workflows.py
+-rw-r--r--   0        0        0     1535 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schedules/scheduling.py
+-rw-r--r--   0        0        0      821 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schedules/task_vacuum.py
+-rw-r--r--   0        0        0     1053 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schedules/validate_products.py
+-rw-r--r--   0        0        0     2131 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schedules/validate_subscriptions.py
+-rw-r--r--   0        0        0     2631 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/__init__.py
+-rw-r--r--   0        0        0      886 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/base.py
+-rw-r--r--   0        0        0     1293 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/engine_settings.py
+-rw-r--r--   0        0        0     1346 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/fixed_input.py
+-rw-r--r--   0        0        0      842 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/problem_detail.py
+-rw-r--r--   0        0        0     3390 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/process.py
+-rw-r--r--   0        0        0     1670 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/product.py
+-rw-r--r--   0        0        0     1735 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/product_block.py
+-rw-r--r--   0        0        0      951 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/resource_type.py
+-rw-r--r--   0        0        0     3180 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/subscription.py
+-rw-r--r--   0        0        0     1013 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/subscription_descriptions.py
+-rw-r--r--   0        0        0     1803 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/schemas/workflow.py
+-rw-r--r--   0        0        0     1797 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/security.py
+-rw-r--r--   0        0        0      571 2023-05-24 07:44:35.514022 orchestrator_core-1.1.0rc1/orchestrator/services/__init__.py
+-rw-r--r--   0        0        0     3586 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/services/celery.py
+-rw-r--r--   0        0        0    22351 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/services/processes.py
+-rw-r--r--   0        0        0     1530 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/services/products.py
+-rw-r--r--   0        0        0     3879 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/services/settings.py
+-rw-r--r--   0        0        0    24204 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/services/subscriptions.py
+-rw-r--r--   0        0        0     5707 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/services/tasks.py
+-rw-r--r--   0        0        0     1719 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/services/translations.py
+-rw-r--r--   0        0        0     3708 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/settings.py
+-rw-r--r--   0        0        0      766 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/targets.py
+-rw-r--r--   0        0        0     9397 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/types.py
+-rw-r--r--   0        0        0      571 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/__init__.py
+-rw-r--r--   0        0        0     5593 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/crypt.py
+-rw-r--r--   0        0        0     1477 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/datetime.py
+-rw-r--r--   0        0        0     6207 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/docs.py
+-rw-r--r--   0        0        0     3839 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/errors.py
+-rw-r--r--   0        0        0     8079 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/functional.py
+-rw-r--r--   0        0        0     2785 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/helpers.py
+-rw-r--r--   0        0        0     8512 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/json.py
+-rw-r--r--   0        0        0     3376 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/redis.py
+-rw-r--r--   0        0        0     2972 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/show_process.py
+-rw-r--r--   0        0        0     2395 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/speed.py
+-rw-r--r--   0        0        0    13148 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/state.py
+-rw-r--r--   0        0        0     1077 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/strings.py
+-rw-r--r--   0        0        0     7231 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/utils/vlans.py
+-rw-r--r--   0        0        0     1323 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/version.py
+-rw-r--r--   0        0        0     4476 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/websocket/__init__.py
+-rw-r--r--   0        0        0     3535 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/websocket/managers/broadcast_websocket_manager.py
+-rw-r--r--   0        0        0     3312 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/websocket/managers/memory_websocket_manager.py
+-rw-r--r--   0        0        0     2900 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/websocket/websocket_manager.py
+-rw-r--r--   0        0        0    33615 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/workflow.py
+-rw-r--r--   0        0        0     4085 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2135 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/workflows/modify_note.py
+-rw-r--r--   0        0        0      909 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/workflows/removed_workflow.py
+-rw-r--r--   0        0        0     9204 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/workflows/steps.py
+-rw-r--r--   0        0        0      571 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     1510 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/workflows/tasks/cleanup_tasks_log.py
+-rw-r--r--   0        0        0     2120 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/workflows/tasks/resume_workflows.py
+-rw-r--r--   0        0        0     8335 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/workflows/tasks/validate_products.py
+-rw-r--r--   0        0        0      684 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/workflows/translations/en-GB.json
+-rw-r--r--   0        0        0     8839 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/orchestrator/workflows/utils.py
+-rw-r--r--   0        0        0     4574 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     2413 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/setup.cfg
+-rw-r--r--   0        0        0      665 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/setup.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/__init__.py
+-rw-r--r--   0        0        0     3199 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
+-rw-r--r--   0        0        0     1855 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
+-rw-r--r--   0        0        0     1544 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/main.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1608 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
+-rw-r--r--   0        0        0     1211 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2828 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
+-rw-r--r--   0        0        0      588 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/acceptance_tests/test_test_product.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/unit_tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/unit_tests/api/__init__.py
+-rw-r--r--   0        0        0     5159 2023-05-24 07:44:35.518023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_caching.py
+-rw-r--r--   0        0        0     1578 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_fixed_inputs.py
+-rw-r--r--   0        0        0     1192 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_health.py
+-rw-r--r--   0        0        0     3049 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_helpers.py
+-rw-r--r--   0        0        0     1747 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_models.py
+-rw-r--r--   0        0        0    20143 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_processes.py
+-rw-r--r--   0        0        0    16019 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_processes_ws.py
+-rw-r--r--   0        0        0     3742 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_product_blocks.py
+-rw-r--r--   0        0        0     7942 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_products.py
+-rw-r--r--   0        0        0     2486 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_resource_types.py
+-rw-r--r--   0        0        0     1772 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_settings.py
+-rw-r--r--   0        0        0     2985 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    37706 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_subscriptions.py
+-rw-r--r--   0        0        0     2367 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/api/test_workflows.py
+-rw-r--r--   0        0        0    25724 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
+-rw-r--r--   0        0        0    27170 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
+-rw-r--r--   0        0        0      511 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/config.py
+-rw-r--r--   0        0        0    21642 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/domain/__init__.py
+-rw-r--r--   0        0        0    50537 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/domain/test_base.py
+-rw-r--r--   0        0        0     8092 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/domain/test_base_with_list_union.py
+-rw-r--r--   0        0        0     4493 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/domain/test_base_with_union.py
+-rw-r--r--   0        0        0     2824 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     7530 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/processes.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1683 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
+-rw-r--r--   0        0        0     2569 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
+-rw-r--r--   0        0        0     1609 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
+-rw-r--r--   0        0        0     2642 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
+-rw-r--r--   0        0        0     2590 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
+-rw-r--r--   0        0        0     1232 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
+-rw-r--r--   0        0        0     1055 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/__init__.py
+-rw-r--r--   0        0        0     2372 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
+-rw-r--r--   0        0        0     2262 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
+-rw-r--r--   0        0        0     4191 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
+-rw-r--r--   0        0        0     3240 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_one.py
+-rw-r--r--   0        0        0     2341 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
+-rw-r--r--   0        0        0     2977 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
+-rw-r--r--   0        0        0     2298 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
+-rw-r--r--   0        0        0     2282 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
+-rw-r--r--   0        0        0     1671 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
+-rw-r--r--   0        0        0     1898 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_union.py
+-rw-r--r--   0        0        0      527 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/resource_types.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/forms/__init__.py
+-rw-r--r--   0        0        0     1462 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/forms/shared.py
+-rw-r--r--   0        0        0    25426 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/forms/test_generic_validators.py
+-rw-r--r--   0        0        0     7644 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/forms/test_network_validators.py
+-rw-r--r--   0        0        0     6626 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/forms/test_post_process.py
+-rw-r--r--   0        0        0    10123 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/graphql/test_processes.py
+-rw-r--r--   0        0        0     4594 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/graphql/test_product.py
+-rw-r--r--   0        0        0     5174 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/graphql/test_settings.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/schedules/__init__.py
+-rw-r--r--   0        0        0      807 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/schedules/test_scheduling.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/services/__init__.py
+-rw-r--r--   0        0        0    26695 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/services/test_processes.py
+-rw-r--r--   0        0        0     1083 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/services/test_products.py
+-rw-r--r--   0        0        0     5830 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/services/test_subscriptions.py
+-rw-r--r--   0        0        0     2100 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/services/test_translations.py
+-rw-r--r--   0        0        0     7353 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/test_db.py
+-rw-r--r--   0        0        0      385 2023-05-24 07:44:35.522023 orchestrator_core-1.1.0rc1/test/unit_tests/test_types.py
+-rw-r--r--   0        0        0    12048 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/test_workflow.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/utils/__init__.py
+-rw-r--r--   0        0        0      163 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_datetime.py
+-rw-r--r--   0        0        0     1871 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_errors.py
+-rw-r--r--   0        0        0     3517 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_functional.py
+-rw-r--r--   0        0        0     3052 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_json.py
+-rw-r--r--   0        0        0     1144 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_speed.py
+-rw-r--r--   0        0        0    11501 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_state.py
+-rw-r--r--   0        0        0      192 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_strings.py
+-rw-r--r--   0        0        0     8339 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_vlans.py
+-rw-r--r--   0        0        0    12492 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/workflows/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/workflows/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/workflows/shared/__init__.py
+-rw-r--r--   0        0        0     2091 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/workflows/shared/test_validate_subscriptions.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     2039 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
+-rw-r--r--   0        0        0     2584 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/workflows/tasks/test_resume_workflows.py
+-rw-r--r--   0        0        0      288 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/workflows/tasks/test_validate_products.py
+-rw-r--r--   0        0        0     3390 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/workflows/test_config_db_code.py
+-rw-r--r--   0        0        0     1877 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/workflows/test_generic_workflow_steps.py
+-rw-r--r--   0        0        0      987 2023-05-24 07:44:35.526023 orchestrator_core-1.1.0rc1/test/unit_tests/workflows/test_modify_note.py
+-rw-r--r--   0        0        0     5285 1970-01-01 00:00:00.000000 orchestrator_core-1.1.0rc1/PKG-INFO
```

### Comparing `orchestrator-core-1.0.2rc3/.github/workflows/README.md` & `orchestrator_core-1.1.0rc1/.github/workflows/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/.github/workflows/build-push-container.yml` & `orchestrator_core-1.1.0rc1/.github/workflows/build-push-container.yml`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/.github/workflows/codeql-analysis.yml` & `orchestrator_core-1.1.0rc1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/.github/workflows/publish-package.yml` & `orchestrator_core-1.1.0rc1/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/.github/workflows/run-linting-tests.yml` & `orchestrator_core-1.1.0rc1/.github/workflows/run-linting-tests.yml`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/.github/workflows/run-unit-tests.yml` & `orchestrator_core-1.1.0rc1/.github/workflows/run-unit-tests.yml`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
           python -m pip install --upgrade pip
           pip install flit
           flit install --deps develop --symlink
           echo "GIT_COMMIT_HASH=\"test\"" > orchestrator/version.py
         env:
           FLIT_ROOT_INSTALL: 1
       - name: Run Unit tests
-        run: CACHE_HOST=redis DATABASE_URI=postgresql://$POSTGRES_USER:$POSTGRES_PASSWORD@$POSTGRES_HOST/$POSTGRES_DB  pytest --cov-branch --cov=orchestrator --cov-report=xml --ignore=test --ignore=orchestrator/devtools --ignore=examples --ignore=docs
+        run: CACHE_URI=redis://redis DATABASE_URI=postgresql://$POSTGRES_USER:$POSTGRES_PASSWORD@$POSTGRES_HOST/$POSTGRES_DB  pytest --cov-branch --cov=orchestrator --cov-report=xml --ignore=test --ignore=orchestrator/devtools --ignore=examples --ignore=docs
         env:
           POSTGRES_DB: orchestrator-core-test
           POSTGRES_USER: nwa
           POSTGRES_PASSWORD: nwa
           POSTGRES_HOST: postgres
           ENVIRONMENT: TESTING
       - name: "Upload coverage to Codecov"
```

### Comparing `orchestrator-core-1.0.2rc3/.github/workflows/scheduled-build.yml` & `orchestrator_core-1.1.0rc1/.github/workflows/scheduled-build.yml`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/.gitignore` & `orchestrator_core-1.1.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/.pre-commit-config.yaml` & `orchestrator_core-1.1.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/.stignore` & `orchestrator_core-1.1.0rc1/.stignore`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/CHANGELOG.md` & `orchestrator_core-1.1.0rc1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # Changelog
 
-## [Unreleased]
+## [1.1.0rc1]
+
+### Breaking change
+ - Changed `settings.CACHE_HOST` and `settings.CACHE_PORT` to `settings.CACHE_URI` 
+
+## [1.0.2]
 
 - Allow user to extend the default translation set, instead of overwriting everything
-- Return worker status information in the `/api/settings/status` endpoint
+- Return worker status information in the `/api/settings/worker-status` endpoint
 
 ## [0.4.0-rc1](https://github.com/workfloworchestrator/orchestrator-core/tree/0.4.0-rc1) (2022-03-08)
 
 [Full Changelog](https://github.com/workfloworchestrator/orchestrator-core/compare/0.3.8...0.4.0-rc1)
 
 **Merged pull requests:**
```

### Comparing `orchestrator-core-1.0.2rc3/LICENSE` & `orchestrator_core-1.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/README.md` & `orchestrator_core-1.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/architecture/application/cli.md` & `orchestrator_core-1.1.0rc1/docs/architecture/application/cli.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/architecture/application/domainmodels.md` & `orchestrator_core-1.1.0rc1/docs/architecture/application/domainmodels.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/architecture/application/openapi.json` & `orchestrator_core-1.1.0rc1/docs/architecture/application/openapi.json`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/architecture/application/python.md` & `orchestrator_core-1.1.0rc1/docs/architecture/application/python.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/architecture/application/scaling.md` & `orchestrator_core-1.1.0rc1/docs/architecture/application/scaling.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/architecture/application/tasks.md` & `orchestrator_core-1.1.0rc1/docs/architecture/application/tasks.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/architecture/application/websockets.md` & `orchestrator_core-1.1.0rc1/docs/architecture/application/websockets.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/architecture/application/workflow.md` & `orchestrator_core-1.1.0rc1/docs/architecture/application/workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/architecture/tldr.md` & `orchestrator_core-1.1.0rc1/docs/architecture/tldr.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/contributing/guidelines.md` & `orchestrator_core-1.1.0rc1/docs/contributing/guidelines.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/contributing/testing.md` & `orchestrator_core-1.1.0rc1/docs/contributing/testing.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/css/termynal.css` & `orchestrator_core-1.1.0rc1/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/getting-started/base.md` & `orchestrator_core-1.1.0rc1/docs/getting-started/base.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/getting-started/development.md` & `orchestrator_core-1.1.0rc1/docs/getting-started/development.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/index.md` & `orchestrator_core-1.1.0rc1/docs/index.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/js/custom.js` & `orchestrator_core-1.1.0rc1/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/js/termynal.js` & `orchestrator_core-1.1.0rc1/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/workshops/beginner/create-user-group.md` & `orchestrator_core-1.1.0rc1/docs/workshops/beginner/create-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/workshops/beginner/create-user.md` & `orchestrator_core-1.1.0rc1/docs/workshops/beginner/create-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/workshops/beginner/database-migration.md` & `orchestrator_core-1.1.0rc1/docs/workshops/beginner/database-migration.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/workshops/beginner/debian.md` & `orchestrator_core-1.1.0rc1/docs/workshops/beginner/debian.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/workshops/beginner/docker.md` & `orchestrator_core-1.1.0rc1/docs/workshops/beginner/docker.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/workshops/beginner/domain-models.md` & `orchestrator_core-1.1.0rc1/docs/workshops/beginner/domain-models.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/workshops/beginner/explore.md` & `orchestrator_core-1.1.0rc1/docs/workshops/beginner/explore.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/workshops/beginner/input-forms.md` & `orchestrator_core-1.1.0rc1/docs/workshops/beginner/input-forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/workshops/beginner/macos.md` & `orchestrator_core-1.1.0rc1/docs/workshops/beginner/macos.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/workshops/beginner/modify-user-group.md` & `orchestrator_core-1.1.0rc1/docs/workshops/beginner/modify-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/workshops/beginner/modify-user.md` & `orchestrator_core-1.1.0rc1/docs/workshops/beginner/modify-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/workshops/beginner/overview.md` & `orchestrator_core-1.1.0rc1/docs/workshops/beginner/overview.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/workshops/beginner/register-workflows.md` & `orchestrator_core-1.1.0rc1/docs/workshops/beginner/register-workflows.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/workshops/beginner/scenario.md` & `orchestrator_core-1.1.0rc1/docs/workshops/beginner/scenario.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/workshops/beginner/start-applications.md` & `orchestrator_core-1.1.0rc1/docs/workshops/beginner/start-applications.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/workshops/beginner/terminate-user-group.md` & `orchestrator_core-1.1.0rc1/docs/workshops/beginner/terminate-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/workshops/beginner/terminate-user.md` & `orchestrator_core-1.1.0rc1/docs/workshops/beginner/terminate-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/workshops/beginner/workflow-introduction.md` & `orchestrator_core-1.1.0rc1/docs/workshops/beginner/workflow-introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/docs/workshops/images/metadata_products.png` & `orchestrator_core-1.1.0rc1/docs/workshops/images/metadata_products.png`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/examples/basic/basic_orchestrator.py` & `orchestrator_core-1.1.0rc1/examples/basic/basic_orchestrator.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/mkdocs.yml` & `orchestrator_core-1.1.0rc1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/mutmut_config.py` & `orchestrator_core-1.1.0rc1/mutmut_config.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/__init__.py` & `orchestrator_core-1.1.0rc1/orchestrator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This is the orchestrator workflow engine."""
 
-__version__ = "1.0.2rc3"
+__version__ = "1.1.0rc1"
 
 from orchestrator.app import OrchestratorCore
 from orchestrator.settings import app_settings, oauth2_settings
 from orchestrator.workflow import begin, conditional, done, focussteps, inputstep, retrystep, step, steplens, workflow
 
 __all__ = [
     "OrchestratorCore",
```

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/api/__init__.py` & `orchestrator_core-1.1.0rc1/orchestrator/api/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/__init__.py` & `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/api.py` & `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/api.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/__init__.py` & `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/fixed_input.py` & `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/health.py` & `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/processes.py` & `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/product_blocks.py` & `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/products.py` & `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/products.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/resource_types.py` & `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/settings.py` & `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 CACHE_FLUSH_OPTIONS: dict[str, str] = {
     "all": "All caches",
 }
 
 
 @router.delete("/cache/{name}")
 async def clear_cache(name: str) -> Union[int, None]:
-    cache: AIORedis = AIORedis(host=app_settings.CACHE_HOST, port=app_settings.CACHE_PORT)
+    cache: AIORedis = AIORedis.from_url(app_settings.CACHE_URI)
     if name not in CACHE_FLUSH_OPTIONS:
         raise_status(HTTPStatus.BAD_REQUEST, "Invalid cache name")
 
     key_name = "orchestrator:*" if name == "all" else f"orchestrator:{name}:*"
     return await delete_keys_matching_pattern(cache, key_name)
 
 
@@ -88,17 +88,18 @@
             [WS_CHANNELS.ENGINE_SETTINGS],
             {"engine-status": generate_engine_status_response(result)},
         )
 
     return status_response
 
 
+@router.get("/worker-status", response_model=WorkerStatus)
 def get_worker_status() -> WorkerStatus:
     """
-    Return information job workers and queues.
+    Return data on job workers and queues.
 
     Returns:
     - The number of queued jobs
     - The number of workers
     - The number of running jobs
     - The number of successful and unsuccessful jobs
     """
@@ -117,17 +118,15 @@
     Retrieve the global status object.
 
     Returns:
         The global status of the engine
 
     """
     engine_settings = EngineSettingsTable.query.one()
-    response = generate_engine_status_response(engine_settings)
-    response.worker_status = get_worker_status()
-    return response
+    return generate_engine_status_response(engine_settings)
 
 
 if app_settings.ENABLE_WEBSOCKETS:
 
     @router.websocket("/ws-status/")
     async def websocket_get_global_status(websocket: WebSocket, token: str = Query(...)) -> None:
         error = await websocket_manager.authorize(websocket, token)
```

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py` & `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/subscriptions.py` & `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/translations.py` & `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/user.py` & `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/workflows.py` & `orchestrator_core-1.1.0rc1/orchestrator/api/api_v1/endpoints/workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/api/error_handling.py` & `orchestrator_core-1.1.0rc1/orchestrator/api/error_handling.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/api/helpers.py` & `orchestrator_core-1.1.0rc1/orchestrator/api/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/api/models.py` & `orchestrator_core-1.1.0rc1/orchestrator/api/models.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/app.py` & `orchestrator_core-1.1.0rc1/orchestrator/app.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/cli/__init__.py` & `orchestrator_core-1.1.0rc1/orchestrator/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/cli/database.py` & `orchestrator_core-1.1.0rc1/orchestrator/cli/database.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py` & `orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/helpers.py` & `orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/product_block_helpers.py` & `orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/product_block_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/product_helpers.py` & `orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/product_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py` & `orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/types.py` & `orchestrator_core-1.1.0rc1/orchestrator/cli/domain_gen_helpers/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/cli/helpers/__init__.py` & `orchestrator_core-1.1.0rc1/orchestrator/cli/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/cli/helpers/input_helpers.py` & `orchestrator_core-1.1.0rc1/orchestrator/cli/helpers/input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/cli/helpers/print_helpers.py` & `orchestrator_core-1.1.0rc1/orchestrator/cli/helpers/print_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/cli/main.py` & `orchestrator_core-1.1.0rc1/orchestrator/cli/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/cli/migrate_domain_models.py` & `orchestrator_core-1.1.0rc1/orchestrator/cli/migrate_domain_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/cli/migrate_workflows.py` & `orchestrator_core-1.1.0rc1/orchestrator/cli/migrate_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/cli/migration_helpers.py` & `orchestrator_core-1.1.0rc1/orchestrator/cli/migration_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/cli/scheduler.py` & `orchestrator_core-1.1.0rc1/orchestrator/cli/scheduler.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/config/__init__.py` & `orchestrator_core-1.1.0rc1/orchestrator/config/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/config/assignee.py` & `orchestrator_core-1.1.0rc1/orchestrator/config/assignee.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/db/__init__.py` & `orchestrator_core-1.1.0rc1/orchestrator/db/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/db/database.py` & `orchestrator_core-1.1.0rc1/orchestrator/db/database.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/db/filters/filters.py` & `orchestrator_core-1.1.0rc1/orchestrator/db/filters/filters.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/db/filters/process.py` & `orchestrator_core-1.1.0rc1/orchestrator/db/filters/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/db/models.py` & `orchestrator_core-1.1.0rc1/orchestrator/db/models.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/db/range/range.py` & `orchestrator_core-1.1.0rc1/orchestrator/db/range/range.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/db/sorting/sorting.py` & `orchestrator_core-1.1.0rc1/orchestrator/db/sorting/sorting.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/devtools/populator.py` & `orchestrator_core-1.1.0rc1/orchestrator/devtools/populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/distlock/__init__.py` & `orchestrator_core-1.1.0rc1/orchestrator/distlock/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,17 +51,15 @@
 wrapped_distlock_manager = WrappedDistLockManager()
 distlock_manager = cast(DistLockManager, wrapped_distlock_manager)
 
 
 # The Global DistLockManager is set after calling this function
 def init_distlock_manager(settings: AppSettings) -> DistLockManager:
     wrapped_distlock_manager.update(
-        DistLockManager(
-            settings.ENABLE_DISTLOCK_MANAGER, settings.DISTLOCK_BACKEND, (settings.CACHE_HOST, settings.CACHE_PORT)
-        )
+        DistLockManager(settings.ENABLE_DISTLOCK_MANAGER, settings.DISTLOCK_BACKEND, settings.CACHE_URI)
     )
     return distlock_manager
 
 
 __all__ = [
     "distlock_manager",
     "init_distlock_manager",
```

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/distlock/distlock_manager.py` & `orchestrator_core-1.1.0rc1/orchestrator/distlock/distlock_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Optional, Tuple, Union
+from typing import Optional, Union
+
+from pydantic import RedisDsn
 
 from orchestrator.distlock.managers.memory_distlock_manager import Lock as MemoryLock
 from orchestrator.distlock.managers.memory_distlock_manager import MemoryDistLockManager
 from orchestrator.distlock.managers.redis_distlock_manager import Lock as RedisLock
 from orchestrator.distlock.managers.redis_distlock_manager import RedisDistLockManager
 
 DistLock = Union[MemoryLock, RedisLock]
@@ -29,19 +31,19 @@
 
     Locks are to be created with an expiration period after which the backend
     implementation must release it.
     """
 
     _backend: Union[MemoryDistLockManager, RedisDistLockManager]
 
-    def __init__(self, enabled: bool, backend: Optional[str] = None, redis_address: Optional[Tuple[str, int]] = None):
+    def __init__(self, enabled: bool, backend: Optional[str] = None, redis_dsn: Optional[RedisDsn] = None):
         self.enabled = enabled
         self.connected = False
-        if backend == "redis" and redis_address:
-            self._backend = RedisDistLockManager(redis_address)
+        if backend == "redis" and redis_dsn:
+            self._backend = RedisDistLockManager(redis_dsn)
         else:
             self._backend = MemoryDistLockManager()
 
     async def connect_redis(self) -> None:
         if not self.connected:
             await self._backend.connect_redis()
             self.connected = True
```

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/distlock/managers/__init__.py` & `orchestrator_core-1.1.0rc1/orchestrator/distlock/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/distlock/managers/memory_distlock_manager.py` & `orchestrator_core-1.1.0rc1/orchestrator/distlock/managers/memory_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/distlock/managers/redis_distlock_manager.py` & `orchestrator_core-1.1.0rc1/orchestrator/distlock/managers/redis_distlock_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,40 +6,43 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Optional, Tuple
+from typing import Optional
 
+from pydantic import RedisDsn
 from redis import Redis
 from redis.asyncio import Redis as AIORedis
 from redis.asyncio.lock import Lock
 from redis.exceptions import LockError
 from redis.lock import Lock as SyncLock
 from structlog import get_logger
 
+from orchestrator.settings import app_settings
+
 logger = get_logger(__name__)
 
 
 class RedisDistLockManager:
     """Create Distributed Locks in Redis.
 
     https://redis.io/topics/distlock
     """
 
     namespace = "orchestrator:distlock"
 
-    def __init__(self, redis_address: Tuple[str, int]):
+    def __init__(self, redis_address: RedisDsn):
         self.redis_conn: Optional[AIORedis] = None
         self.redis_address = redis_address
 
     async def connect_redis(self) -> None:
-        self.redis_conn = AIORedis(host=self.redis_address[0], port=self.redis_address[1])
+        self.redis_conn = AIORedis.from_url(self.redis_address)
 
     async def disconnect_redis(self) -> None:
         if self.redis_conn:
             await self.redis_conn.close()
 
     async def get_lock(self, resource: str, expiration_seconds: int) -> Optional[Lock]:
         if not self.redis_conn:
@@ -73,15 +76,15 @@
         except LockError:
             logger.Exception("Could not release lock for resource", resource=lock.name)
 
     # https://github.com/aio-libs/aioredis-py/issues/1273
     def release_sync(self, lock: Lock) -> None:
         redis_conn: Optional[Redis] = None
         try:
-            redis_conn = Redis(host=self.redis_address[0], port=self.redis_address[1])
+            redis_conn = Redis.from_url(app_settings.CACHE_URI)
             sync_lock: SyncLock = SyncLock(
                 redis=redis_conn,
                 name=lock.name,  # type: ignore
                 timeout=lock.timeout,
                 blocking=False,
                 thread_local=False,
             )
```

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/domain/__init__.py` & `orchestrator_core-1.1.0rc1/orchestrator/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/domain/base.py` & `orchestrator_core-1.1.0rc1/orchestrator/domain/base.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/domain/lifecycle.py` & `orchestrator_core-1.1.0rc1/orchestrator/domain/lifecycle.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/exception_handlers.py` & `orchestrator_core-1.1.0rc1/orchestrator/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/forms/__init__.py` & `orchestrator_core-1.1.0rc1/orchestrator/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/forms/network_type_validators.py` & `orchestrator_core-1.1.0rc1/orchestrator/forms/network_type_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/forms/validators.py` & `orchestrator_core-1.1.0rc1/orchestrator/forms/validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/graphql/__init__.py` & `orchestrator_core-1.1.0rc1/orchestrator/graphql/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,40 +16,53 @@
 import strawberry
 import structlog
 from fastapi import Depends
 from fastapi.routing import APIRouter
 from graphql import GraphQLError, GraphQLFormattedError
 from graphql.error.graphql_error import format_error
 from httpx import HTTPStatusError
+from oauth2_lib.graphql_authentication import authenticated_field
 from starlette.requests import Request
 from strawberry.fastapi import GraphQLRouter
 from strawberry.http import GraphQLHTTPResponse
+from strawberry.tools import merge_types
 from strawberry.types import ExecutionContext, ExecutionResult
 from strawberry.utils.logging import StrawberryLogger
 
-from orchestrator.graphql.authentication import authenticated_field
 from orchestrator.graphql.extensions.deprecation_checker_extension import make_deprecation_checker_extension
 from orchestrator.graphql.extensions.ErrorCollectorExtension import ErrorCollectorExtension
 from orchestrator.graphql.pagination import Connection
-from orchestrator.graphql.resolvers.process import resolve_processes
+from orchestrator.graphql.resolvers import SettingsMutation, resolve_processes, resolve_products, resolve_settings
 from orchestrator.graphql.schemas.process import ProcessType
+from orchestrator.graphql.schemas.product import ProductType
+from orchestrator.graphql.schemas.settings import StatusType
 from orchestrator.graphql.types import CustomContext
 from orchestrator.security import get_oidc_user, get_opa_security_graphql
 from orchestrator.settings import app_settings
 
 api_router = APIRouter()
 
 logger = structlog.get_logger(__name__)
 
 
 @strawberry.type(description="Orchestrator queries")
 class Query:
     processes: Connection[ProcessType] = authenticated_field(
         resolver=resolve_processes, description="Returns list of processes"
     )
+    products: Connection[ProductType] = authenticated_field(
+        resolver=resolve_products, description="Returns list of products"
+    )
+    settings: StatusType = authenticated_field(
+        resolver=resolve_settings,
+        description="Returns information about cache, workers, and global engine settings",
+    )
+
+
+Mutation = merge_types("Mutation", (SettingsMutation,))
 
 
 class OrchestratorGraphqlRouter(GraphQLRouter):
     def __init__(self, schema: strawberry.federation.Schema, **kwargs: Any) -> None:
         super().__init__(schema, **kwargs)
 
     @staticmethod
@@ -88,14 +101,15 @@
                 StrawberryLogger.logger.debug(message)
             else:
                 StrawberryLogger.error(error, execution_context)
 
 
 schema = OrchestratorSchema(
     query=Query,
+    mutation=Mutation,
     enable_federation_2=app_settings.FEDEREATION_ENABLED,
     extensions=[ErrorCollectorExtension, make_deprecation_checker_extension(query=Query)],
 )
 
 
 def custom_context_dependency(
     get_current_user: Callable = Depends(get_oidc_user),  # noqa: B008
```

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/graphql/extensions/ErrorCollectorExtension.py` & `orchestrator_core-1.1.0rc1/orchestrator/graphql/extensions/ErrorCollectorExtension.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/graphql/extensions/deprecation_checker_extension.py` & `orchestrator_core-1.1.0rc1/orchestrator/graphql/extensions/deprecation_checker_extension.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/graphql/pagination.py` & `orchestrator_core-1.1.0rc1/orchestrator/graphql/pagination.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/graphql/resolvers/process.py` & `orchestrator_core-1.1.0rc1/orchestrator/graphql/resolvers/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/graphql/schemas/process.py` & `orchestrator_core-1.1.0rc1/orchestrator/graphql/schemas/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/graphql/types.py` & `orchestrator_core-1.1.0rc1/orchestrator/graphql/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/graphql/utils/get_selected_fields.py` & `orchestrator_core-1.1.0rc1/orchestrator/graphql/utils/get_selected_fields.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/migrations/alembic.ini` & `orchestrator_core-1.1.0rc1/orchestrator/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/migrations/env.py` & `orchestrator_core-1.1.0rc1/orchestrator/migrations/env.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/migrations/helpers.py` & `orchestrator_core-1.1.0rc1/orchestrator/migrations/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/migrations/templates/alembic.ini.j2` & `orchestrator_core-1.1.0rc1/orchestrator/migrations/templates/alembic.ini.j2`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/migrations/templates/env.py.j2` & `orchestrator_core-1.1.0rc1/orchestrator/migrations/templates/env.py.j2`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py` & `orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py` & `orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py` & `orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py` & `orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py` & `orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py` & `orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py` & `orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py` & `orchestrator_core-1.1.0rc1/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/schedules/__init__.py` & `orchestrator_core-1.1.0rc1/orchestrator/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/schedules/resume_workflows.py` & `orchestrator_core-1.1.0rc1/orchestrator/schedules/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/schedules/scheduling.py` & `orchestrator_core-1.1.0rc1/orchestrator/schedules/scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/schedules/task_vacuum.py` & `orchestrator_core-1.1.0rc1/orchestrator/schedules/task_vacuum.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/schedules/validate_products.py` & `orchestrator_core-1.1.0rc1/orchestrator/schedules/validate_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/schedules/validate_subscriptions.py` & `orchestrator_core-1.1.0rc1/orchestrator/schedules/validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/schemas/__init__.py` & `orchestrator_core-1.1.0rc1/orchestrator/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/schemas/base.py` & `orchestrator_core-1.1.0rc1/orchestrator/schemas/base.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/schemas/engine_settings.py` & `orchestrator_core-1.1.0rc1/orchestrator/schemas/engine_settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,18 +9,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Optional
 
+import strawberry
+
 from orchestrator.schemas.base import OrchestratorBaseModel
 from orchestrator.types import strEnum
 
 
+@strawberry.enum
 class GlobalStatusEnum(strEnum):
     RUNNING = "RUNNING"
     PAUSED = "PAUSED"
     PAUSING = "PAUSING"
 
 
 class EngineSettingsBaseSchema(OrchestratorBaseModel):
@@ -33,11 +36,11 @@
     number_of_queued_jobs: int = 0
     number_of_running_jobs: int = 0
 
 
 class EngineSettingsSchema(EngineSettingsBaseSchema):
     global_status: Optional[GlobalStatusEnum]
     running_processes: int
-    worker_status: Optional[WorkerStatus]
 
     class Config:
         orm_mode = True
+        orm_mode = True
```

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/schemas/fixed_input.py` & `orchestrator_core-1.1.0rc1/orchestrator/schemas/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/schemas/problem_detail.py` & `orchestrator_core-1.1.0rc1/orchestrator/schemas/problem_detail.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/schemas/process.py` & `orchestrator_core-1.1.0rc1/orchestrator/schemas/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/schemas/product.py` & `orchestrator_core-1.1.0rc1/orchestrator/schemas/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/schemas/product_block.py` & `orchestrator_core-1.1.0rc1/orchestrator/schemas/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/schemas/resource_type.py` & `orchestrator_core-1.1.0rc1/orchestrator/schemas/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/schemas/subscription.py` & `orchestrator_core-1.1.0rc1/orchestrator/schemas/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/schemas/subscription_descriptions.py` & `orchestrator_core-1.1.0rc1/orchestrator/schemas/subscription_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/schemas/workflow.py` & `orchestrator_core-1.1.0rc1/orchestrator/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/security.py` & `orchestrator_core-1.1.0rc1/orchestrator/security.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/services/__init__.py` & `orchestrator_core-1.1.0rc1/orchestrator/services/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/services/celery.py` & `orchestrator_core-1.1.0rc1/orchestrator/services/celery.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/services/processes.py` & `orchestrator_core-1.1.0rc1/orchestrator/services/processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/services/products.py` & `orchestrator_core-1.1.0rc1/orchestrator/services/products.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/services/settings.py` & `orchestrator_core-1.1.0rc1/orchestrator/services/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/services/subscriptions.py` & `orchestrator_core-1.1.0rc1/orchestrator/services/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/services/tasks.py` & `orchestrator_core-1.1.0rc1/orchestrator/services/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,11 +132,11 @@
             return
 
         inspection: Inspect = _celery.control.inspect()
         stats = inspection.stats()
         self.number_of_workers_online = len(stats)
 
         def sum_items(d: dict) -> int:
-            return sum(len(l) for _, l in d.items())
+            return sum(len(l) for _, l in d.items()) if d else 0
 
         self.number_of_queued_jobs = sum_items(inspection.scheduled()) + sum_items(inspection.reserved())
         self.number_of_running_jobs = sum(len(tasks) for w, tasks in inspection.active().items())
```

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/services/translations.py` & `orchestrator_core-1.1.0rc1/orchestrator/services/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/settings.py` & `orchestrator_core-1.1.0rc1/orchestrator/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from pathlib import Path
 from typing import List, Optional
 
 from opentelemetry.exporter.otlp.proto.grpc.trace_exporter import OTLPSpanExporter
 from opentelemetry.sdk.resources import SERVICE_NAME, Resource
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
-from pydantic import BaseSettings
+from pydantic import BaseSettings, PostgresDsn, RedisDsn
 
 from orchestrator.types import strEnum
 
 
 class ExecutorType(strEnum):
     WORKER = "celery"
     THREADPOOL = "threadpool"
@@ -47,21 +47,20 @@
         "Content-Range",
         "ETag",
     ]
     ENVIRONMENT: str = "local"
     EXECUTOR: str = ExecutorType.THREADPOOL
     WORKFLOWS_SWAGGER_HOST: str = "localhost"
     WORKFLOWS_GUI_URI: str = "http://localhost:3000"
-    DATABASE_URI: str = "postgresql://nwa:nwa@localhost/orchestrator-core"
+    DATABASE_URI: PostgresDsn = "postgresql://nwa:nwa@localhost/orchestrator-core"  # type: ignore
     MAX_WORKERS: int = 5
     MAIL_SERVER: str = "localhost"
     MAIL_PORT: int = 25
     MAIL_STARTTLS: bool = False
-    CACHE_HOST: str = "127.0.0.1"
-    CACHE_PORT: int = 6379
+    CACHE_URI: RedisDsn = "redis://localhost:6379/0"  # type: ignore
     CACHE_DOMAIN_MODELS: bool = False
     CACHE_HMAC_SECRET: Optional[str] = None  # HMAC signing key, used when pickling results in the cache
     ENABLE_DISTLOCK_MANAGER: bool = True
     DISTLOCK_BACKEND: str = "memory"
     CC_NOC: int = 0
     SERVICE_NAME: str = "orchestrator-core"
     LOGGING_HOST: str = "localhost"
@@ -73,17 +72,15 @@
     TRANSLATIONS_DIR: Optional[Path] = None
     WEBSOCKET_BROADCASTER_URL: str = "memory://"
     ENABLE_WEBSOCKETS: bool = True
     DISABLE_INSYNC_CHECK: bool = False
     DEFAULT_PRODUCT_WORKFLOWS: List[str] = ["modify_note"]
     SKIP_MODEL_FOR_MIGRATION_DB_DIFF: List[str] = []
     SERVE_GRAPHQL_UI: bool = True
-    MUTATIONS_ENABLED: bool = False
     FEDEREATION_ENABLED: bool = False
-    ENVIRONMENT_IGNORE_MUTATION_DISABLED: list = []
 
 
 class Oauth2Settings(BaseSettings):
     OAUTH2_ACTIVE: bool = False
     OAUTH2_RESOURCE_SERVER_ID: str = ""
     OAUTH2_RESOURCE_SERVER_SECRET: str = ""
     OAUTH2_TOKEN_URL: str = ""
```

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/targets.py` & `orchestrator_core-1.1.0rc1/orchestrator/targets.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import strawberry
 
 from orchestrator.types import strEnum
 
 
+@strawberry.enum
 class Target(strEnum):
     CREATE = "CREATE"
     MODIFY = "MODIFY"
     TERMINATE = "TERMINATE"
     SYSTEM = "SYSTEM"
```

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/types.py` & `orchestrator_core-1.1.0rc1/orchestrator/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/utils/__init__.py` & `orchestrator_core-1.1.0rc1/orchestrator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/utils/crypt.py` & `orchestrator_core-1.1.0rc1/orchestrator/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/utils/datetime.py` & `orchestrator_core-1.1.0rc1/orchestrator/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/utils/docs.py` & `orchestrator_core-1.1.0rc1/orchestrator/utils/docs.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/utils/errors.py` & `orchestrator_core-1.1.0rc1/orchestrator/utils/errors.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/utils/functional.py` & `orchestrator_core-1.1.0rc1/orchestrator/utils/functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/utils/helpers.py` & `orchestrator_core-1.1.0rc1/orchestrator/utils/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,22 +67,22 @@
 
 def warn_if_unmapped_fields(source: dict, used: dict) -> None:
     if unmapped_fields := [key for key in source.keys() if key not in used.keys()]:
         keys = ",".join(unmapped_fields)
         logger.warning("Found unused keys", keys=keys)
 
 
-def map_value(mapping: dict[str, Callable], k: str, v: Any) -> tuple[str, Any]:
+def map_value(mapping: dict[str, Callable], k: str, v: Any) -> tuple[Any, ...]:
     if f := mapping.get(k):
         if v is None:
             return k, None
         elif type(v) == dict:
-            return result if type(result := f(**v)) is tuple else (k, result)  # type: ignore
+            return result if type(result := f(**v)) is tuple else (k, result)
         else:
-            return result if type(result := f(v)) is tuple else (k, result)  # type: ignore
+            return result if type(result := f(v)) is tuple else (k, result)
     else:
         return k, v
 
 
 def to_camel(s: str) -> str:
     first, *rest = s.split("_")
     return first + "".join(word.title() for word in rest)
```

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/utils/json.py` & `orchestrator_core-1.1.0rc1/orchestrator/utils/json.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/utils/redis.py` & `orchestrator_core-1.1.0rc1/orchestrator/utils/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from orchestrator.services.subscriptions import _generate_etag
 from orchestrator.settings import app_settings
 from orchestrator.utils.json import json_dumps, json_loads
 
 logger = get_logger(__name__)
 
-cache = Redis(host=app_settings.CACHE_HOST, port=app_settings.CACHE_PORT)
+cache = Redis.from_url(app_settings.CACHE_URI)
 
 ONE_WEEK = 3600 * 24 * 7
 
 
 def caching_models_enabled() -> bool:
     return getenv("AIOCACHE_DISABLE", "0") == "0" and app_settings.CACHE_DOMAIN_MODELS
```

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/utils/show_process.py` & `orchestrator_core-1.1.0rc1/orchestrator/utils/show_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/utils/speed.py` & `orchestrator_core-1.1.0rc1/orchestrator/utils/speed.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/utils/state.py` & `orchestrator_core-1.1.0rc1/orchestrator/utils/state.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/utils/strings.py` & `orchestrator_core-1.1.0rc1/orchestrator/utils/strings.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/utils/vlans.py` & `orchestrator_core-1.1.0rc1/orchestrator/utils/vlans.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/version.py` & `orchestrator_core-1.1.0rc1/orchestrator/version.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/websocket/__init__.py` & `orchestrator_core-1.1.0rc1/orchestrator/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/websocket/managers/broadcast_websocket_manager.py` & `orchestrator_core-1.1.0rc1/orchestrator/websocket/managers/broadcast_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/websocket/managers/memory_websocket_manager.py` & `orchestrator_core-1.1.0rc1/orchestrator/websocket/managers/memory_websocket_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Dict, List, Union
 
 from fastapi import WebSocket, WebSocketDisconnect, status
+from starlette.websockets import WebSocketState
 from structlog import get_logger
 
 from orchestrator.utils.json import json_dumps
 
 logger = get_logger(__name__)
 
 
@@ -61,15 +62,16 @@
                         await websocket.send_text(json_dumps(data))
                         if "close" in data and data["close"]:
                             await self.remove_ws(websocket, channel)
         except (RuntimeError, ValueError):
             pass
 
     async def remove_ws(self, websocket: WebSocket, channel: str) -> None:
-        await self.disconnect(websocket)
+        if websocket.client_state != WebSocketState.DISCONNECTED:
+            await self.disconnect(websocket)
         if channel in self.connections_by_pid:
             self.connections_by_pid[channel].remove(websocket)
             if len(self.connections_by_pid[channel]):
                 del self.connections_by_pid[channel]
         self.log_amount_of_connections()
 
     def log_amount_of_connections(self) -> None:
```

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/websocket/websocket_manager.py` & `orchestrator_core-1.1.0rc1/orchestrator/websocket/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/workflow.py` & `orchestrator_core-1.1.0rc1/orchestrator/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/workflows/__init__.py` & `orchestrator_core-1.1.0rc1/orchestrator/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/workflows/modify_note.py` & `orchestrator_core-1.1.0rc1/orchestrator/workflows/modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/workflows/removed_workflow.py` & `orchestrator_core-1.1.0rc1/orchestrator/workflows/removed_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/workflows/steps.py` & `orchestrator_core-1.1.0rc1/orchestrator/workflows/steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/workflows/tasks/__init__.py` & `orchestrator_core-1.1.0rc1/orchestrator/workflows/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/workflows/tasks/cleanup_tasks_log.py` & `orchestrator_core-1.1.0rc1/orchestrator/workflows/tasks/cleanup_tasks_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/workflows/tasks/resume_workflows.py` & `orchestrator_core-1.1.0rc1/orchestrator/workflows/tasks/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/workflows/tasks/validate_products.py` & `orchestrator_core-1.1.0rc1/orchestrator/workflows/tasks/validate_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/workflows/translations/en-GB.json` & `orchestrator_core-1.1.0rc1/orchestrator/workflows/translations/en-GB.json`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/orchestrator/workflows/utils.py` & `orchestrator_core-1.1.0rc1/orchestrator/workflows/utils.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/pyproject.toml` & `orchestrator_core-1.1.0rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     "schedule==1.1.0",
     "sentry-sdk[fastapi]==1.15.0",
     "SQLAlchemy==1.4.28",
     "SQLAlchemy-Utils==0.40.0",
     "typer==0.7.0",
     "uvicorn[standard]~=0.20.0",
     "nwa-stdlib~=1.4.7",
-    "oauth2-lib~=1.2.8",
+    "oauth2-lib~=1.2.9",
     "markupsafe==2.0.1",
     "bandit==1.7.2",
     "tabulate==0.9.0",
     "strawberry-graphql==0.171.1"
 ]
 description-file = "README.md"
 requires-python = ">=3.9,<3.12"
```

### Comparing `orchestrator-core-1.0.2rc3/setup.cfg` & `orchestrator_core-1.1.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/setup.py` & `orchestrator_core-1.1.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/acceptance_tests/conftest.py` & `orchestrator_core-1.1.0rc1/test/acceptance_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py` & `orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/main.py` & `orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py` & `orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py` & `orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py` & `orchestrator_core-1.1.0rc1/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/acceptance_tests/test_test_product.py` & `orchestrator_core-1.1.0rc1/test/acceptance_tests/test_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_caching.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_caching.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,19 @@
 """(regression)tests in relation to domain model caching."""
 from http import HTTPStatus
 from os import getenv
-from unittest.mock import patch
 
 import pytest
 from nwastdlib.url import URL
-from redis import Redis
 
 from orchestrator.domain.base import SubscriptionModel
 from orchestrator.services.subscriptions import build_extended_domain_model
-from orchestrator.settings import app_settings
 from orchestrator.utils.redis import to_redis
 
 
-@pytest.fixture
-def cache_fixture():
-    # Fixture to enable domain model caching and cleanup keys added to the list
-    with patch.object(app_settings, "CACHE_DOMAIN_MODELS", True):
-        cache = Redis(host=app_settings.CACHE_HOST, port=app_settings.CACHE_PORT)
-        to_cleanup = []
-
-        yield to_cleanup
-
-        for key in to_cleanup:
-            try:
-                cache.delete(key)
-            except Exception as exc:
-                print("failed to delete cache key", key, str(exc))  # noqa: T001, T201
-
-
 @pytest.mark.skipif(
     not getenv("AIOCACHE_DISABLE", "0") == "0", reason="AIOCACHE must be enabled for this test to do anything"
 )
 def test_cache_update_customer_description(
     test_client, generic_subscription_1, make_customer_description, cache_fixture
 ):
     """Check that updating subscription customer description is reflected in the cache."""
```

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_fixed_inputs.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_health.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_health.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_helpers.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_models.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_processes.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_processes_ws.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_processes_ws.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_product_blocks.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_products.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_resource_types.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_settings.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_subscription_customer_descriptions.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_subscriptions.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_subscriptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -916,15 +916,15 @@
 
     app_settings.CACHE_DOMAIN_MODELS = True
 
     to_redis(extended_model)
 
     response = test_client.get(URL("api/subscriptions/domain-model") / generic_subscription_1)
 
-    cache = Redis(host=app_settings.CACHE_HOST, port=app_settings.CACHE_PORT)
+    cache = Redis.from_url(app_settings.CACHE_URI)
     result = cache.get(f"domain:{generic_subscription_1}")
     cached_model = json_dumps(json_loads(result))
     cached_etag = cache.get(f"domain:etag:{generic_subscription_1}")
     assert cached_model == json_dumps(extended_model)
     assert cached_etag.decode("utf-8") == etag
 
     assert response.status_code == HTTPStatus.OK
```

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_workflows.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/api/test_workflows.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 @pytest.mark.skipif(
     not getenv("AIOCACHE_DISABLE", "0") == "0", reason="AIOCACHE must be enabled for this test to do anything"
 )
 def test_push_subscriptions_to_cache_step(generic_subscription_1):
     push_subscription = orig(cache_domain_models)
     push_subscription("Aribtrary_name", SubscriptionModel.from_subscription(generic_subscription_1))
 
-    cache = Redis(host=app_settings.CACHE_HOST, port=app_settings.CACHE_PORT)
+    cache = Redis.from_url(app_settings.CACHE_URI)
     assert cache.get(f"domain:{generic_subscription_1}") is None
 
     app_settings.CACHE_DOMAIN_MODELS = True
     push_subscription("Aribtrary_name", SubscriptionModel.from_subscription(generic_subscription_1))
     result = cache.get(f"domain:{generic_subscription_1}")
     assert result is not None
     app_settings.CACHE_DOMAIN_MODELS = False
```

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/cli/test_migrate_domain_models_with_instances.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/cli/test_migrate_domain_models_with_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/cli/test_migrate_domain_models_without_instances.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/cli/test_migrate_domain_models_without_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/conftest.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Any, Optional, cast
 
 import pytest
 import requests
 import structlog
 from alembic import command
 from alembic.config import Config
+from redis import Redis
 from sqlalchemy import create_engine
 from sqlalchemy.engine.url import make_url
 from sqlalchemy.orm.scoping import scoped_session
 from sqlalchemy.orm.session import sessionmaker
 from starlette.testclient import TestClient
 from urllib3_mock import Responses
 
@@ -135,15 +136,15 @@
 
     Returns:
         None
 
     """
     path = os.path.join(os.path.dirname(os.path.realpath(__file__)))
     os.environ["DATABASE_URI"] = db_uri
-    app_settings.DATABASE_URI = db_uri
+    app_settings.DATABASE_URI = db_uri  # type: ignore
     alembic_cfg = Config(file_=os.path.join(path, "../../orchestrator/migrations/alembic.ini"))
     alembic_cfg.set_main_option("script_location", os.path.join(path, "../../orchestrator/migrations"))
     alembic_cfg.set_main_option(
         "version_locations",
         f"{os.path.join(path, '../../orchestrator/migrations/versions/schema')}",
     )
     alembic_cfg.set_main_option("sqlalchemy.url", db_uri)
@@ -239,14 +240,17 @@
         finally:
             if not trans._deactivated_from_connection:
                 trans.rollback()
 
 
 @pytest.fixture(scope="session", autouse=True)
 def fastapi_app(database, db_uri):
+    from oauth2_lib.settings import oauth2lib_settings
+
+    oauth2lib_settings.ENVIRONMENT_IGNORE_MUTATION_DISABLED = ["local", "TESTING"]
     app_settings.DATABASE_URI = db_uri
     app = OrchestratorCore(base_settings=app_settings)
     # Start ProcessDataBroadcastThread to test websocket_manager with memory backend
     app.broadcast_thread.start()
     yield app
     app.broadcast_thread.stop()
 
@@ -580,7 +584,27 @@
             subscription_id=subscription_id, customer_id=customer_id, description=description
         )
         db.session.add(model)
         db.session.commit()
         return model
 
     return customer_description
+
+
+@pytest.fixture
+def cache_fixture(monkeypatch):
+    """Fixture to enable domain model caching and cleanup keys added to the list."""
+    with monkeypatch.context() as m:
+        m.setattr(app_settings, "CACHE_DOMAIN_MODELS", True)
+        cache = Redis.from_url(app_settings.CACHE_URI)
+        # Clear cache before using this fixture
+        cache.flushdb()
+
+        to_cleanup = []
+
+        yield to_cleanup
+
+        for key in to_cleanup:
+            try:
+                cache.delete(key)
+            except Exception as exc:
+                print("failed to delete cache key", key, str(exc))  # noqa: T001, T201
```

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/domain/test_base.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/domain/test_base.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/domain/test_base_with_list_union.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/domain/test_base_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/domain/test_base_with_union.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/domain/test_base_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/__init__.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/processes.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_one.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_list_union.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_one.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_union.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/product_types/product_type_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/resource_types.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/fixtures/products/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/forms/shared.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/forms/shared.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/forms/test_generic_validators.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/forms/test_generic_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/forms/test_network_validators.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/forms/test_network_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/forms/test_post_process.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/forms/test_post_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/graphql/test_processes.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/graphql/test_processes.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 
 def get_processes_query(
     first: int = 10,
     after: int = 0,
     filter_by: Union[list[str], None] = None,
     sort_by: Union[list[dict[str, str]], None] = None,
-) -> str:
+) -> bytes:
     query = """
 query ProcessQuery($first: Int!, $after: Int!, $sortBy: [GraphqlSort!], $filterBy: [GraphqlFilter!]) {
   processes(first: $first, after: $after, sortBy: $sortBy, filterBy: $filterBy) {
     page {
       assignee
       createdBy
       failedReason
@@ -74,22 +74,22 @@
             "variables": {
                 "first": first,
                 "after": after,
                 "sortBy": sort_by if sort_by else [],
                 "filterBy": filter_by if filter_by else [],
             },
         }
-    )
+    ).encode("utf-8")
 
 
 def test_processes_has_next_page(
     test_client, mocked_processes, mocked_processes_resumeall, generic_subscription_2, generic_subscription_1
 ):
     data = get_processes_query()
-    response = test_client.post("/api/graphql", data=data, headers={"Content-Type": "application/json"})
+    response = test_client.post("/api/graphql", content=data, headers={"Content-Type": "application/json"})
     assert HTTPStatus.OK == response.status_code
     result = response.json()
     processes_data = result["data"]["processes"]
     processes = processes_data["page"]
     pageinfo = processes_data["pageInfo"]
 
     assert len(processes) == 10
@@ -107,15 +107,15 @@
             assert field in process
 
 
 def test_process_has_previous_page(
     test_client, mocked_processes, mocked_processes_resumeall, generic_subscription_2, generic_subscription_1
 ):
     data = get_processes_query(after=1)
-    response = test_client.post("/api/graphql", data=data, headers={"Content-Type": "application/json"})
+    response = test_client.post("/api/graphql", content=data, headers={"Content-Type": "application/json"})
 
     assert HTTPStatus.OK == response.status_code
     result = response.json()
     processes_data = result["data"]["processes"]
     processes = processes_data["page"]
     pageinfo = processes_data["pageInfo"]
 
@@ -132,15 +132,15 @@
 
 def test_processes_sorting_asc(
     test_client, mocked_processes, mocked_processes_resumeall, generic_subscription_2, generic_subscription_1
 ):
     # when
 
     data = get_processes_query(sort_by=[{"field": "started", "order": "ASC"}])
-    response = test_client.post("/api/graphql", data=data, headers={"Content-Type": "application/json"})
+    response = test_client.post("/api/graphql", content=data, headers={"Content-Type": "application/json"})
 
     # then
 
     assert HTTPStatus.OK == response.status_code
     result = response.json()
     processes_data = result["data"]["processes"]
     processes = processes_data["page"]
@@ -161,15 +161,15 @@
 
 def test_processes_sorting_desc(
     test_client, mocked_processes, mocked_processes_resumeall, generic_subscription_2, generic_subscription_1
 ):
     # when
 
     data = get_processes_query(sort_by=[{"field": "started", "order": "DESC"}])
-    response = test_client.post("/api/graphql", data=data, headers={"Content-Type": "application/json"})
+    response = test_client.post("/api/graphql", content=data, headers={"Content-Type": "application/json"})
 
     # then
 
     assert HTTPStatus.OK == response.status_code
     result = response.json()
     processes_data = result["data"]["processes"]
     processes = processes_data["page"]
@@ -192,15 +192,15 @@
 
 def test_processes_has_filtering(
     test_client, mocked_processes, mocked_processes_resumeall, generic_subscription_2, generic_subscription_1
 ):
     # when
 
     data = get_processes_query(filter_by=[{"field": "status", "value": "completed"}])
-    response = test_client.post("/api/graphql", data=data, headers={"Content-Type": "application/json"})
+    response = test_client.post("/api/graphql", content=data, headers={"Content-Type": "application/json"})
 
     # then
 
     assert HTTPStatus.OK == response.status_code
     result = response.json()
     processes_data = result["data"]["processes"]
     processes = processes_data["page"]
@@ -226,15 +226,15 @@
     test_client, mocked_processes, mocked_processes_resumeall, generic_subscription_2, generic_subscription_1
 ):
     # when
 
     data = get_processes_query(
         filter_by=[{"field": "status", "value": "completed"}, {"field": "test", "value": "invalid"}]
     )
-    response = test_client.post("/api/graphql", data=data, headers={"Content-Type": "application/json"})
+    response = test_client.post("/api/graphql", content=data, headers={"Content-Type": "application/json"})
 
     # then
 
     assert HTTPStatus.OK == response.status_code
     result = response.json()
     processes_data = result["data"]["processes"]
     errors = result["errors"]
@@ -282,15 +282,15 @@
 
     data = get_processes_query(
         filter_by=[
             {"field": "status", "value": "completed"},
             {"field": "organisation", "value": "54321447"},
         ]
     )
-    response = test_client.post("/api/graphql", data=data, headers={"Content-Type": "application/json"})
+    response = test_client.post("/api/graphql", content=data, headers={"Content-Type": "application/json"})
 
     # then
 
     assert HTTPStatus.OK == response.status_code
     result = response.json()
     processes_data = result["data"]["processes"]
     errors = result["errors"]
@@ -322,15 +322,15 @@
 def test_single_subscription(
     test_client, mocked_processes, mocked_processes_resumeall, generic_subscription_2, generic_subscription_1
 ):
     process_pid = str(mocked_processes[0])
     # when
 
     data = get_processes_query(filter_by=[{"field": "pid", "value": process_pid}])
-    response = test_client.post("/api/graphql", data=data, headers={"Content-Type": "application/json"})
+    response = test_client.post("/api/graphql", content=data, headers={"Content-Type": "application/json"})
 
     # then
 
     assert HTTPStatus.OK == response.status_code
     result = response.json()
     processes_data = result["data"]["processes"]
     processes = processes_data["page"]
```

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/schedules/test_scheduling.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/schedules/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/services/test_processes.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/services/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/services/test_products.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/services/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/services/test_subscriptions.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/services/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/services/test_translations.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/services/test_translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/test_db.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/test_db.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/test_workflow.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_errors.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_errors.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_functional.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_json.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_speed.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_speed.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_state.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_state.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_vlans.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/utils/test_vlans.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/workflows/__init__.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/workflows/shared/test_validate_subscriptions.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/workflows/shared/test_validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/workflows/tasks/test_clean_up_task_log.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/workflows/tasks/test_clean_up_task_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/workflows/tasks/test_resume_workflows.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/workflows/tasks/test_resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/workflows/test_config_db_code.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/workflows/test_config_db_code.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/workflows/test_generic_workflow_steps.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/workflows/test_generic_workflow_steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/test/unit_tests/workflows/test_modify_note.py` & `orchestrator_core-1.1.0rc1/test/unit_tests/workflows/test_modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc3/PKG-INFO` & `orchestrator_core-1.1.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestrator-core
-Version: 1.0.2rc3
+Version: 1.1.0rc1
 Summary: Open source orchestration software for NREN's
 Requires-Python: >=3.9,<3.12
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
@@ -53,15 +53,15 @@
 Requires-Dist: schedule==1.1.0
 Requires-Dist: sentry-sdk[fastapi]==1.15.0
 Requires-Dist: SQLAlchemy==1.4.28
 Requires-Dist: SQLAlchemy-Utils==0.40.0
 Requires-Dist: typer==0.7.0
 Requires-Dist: uvicorn[standard]~=0.20.0
 Requires-Dist: nwa-stdlib~=1.4.7
-Requires-Dist: oauth2-lib~=1.2.8
+Requires-Dist: oauth2-lib~=1.2.9
 Requires-Dist: markupsafe==2.0.1
 Requires-Dist: bandit==1.7.2
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: strawberry-graphql==0.171.1
 Requires-Dist: celery~=5.2.7 ; extra == "celery"
 Requires-Dist: toml ; extra == "dev"
 Requires-Dist: bumpversion ; extra == "dev"
```

