# Comparing `tmp/gadapt-0.2.12.tar.gz` & `tmp/gadapt-0.2.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gadapt-0.2.12.tar", last modified: Wed May 24 07:02:18 2023, max compression
+gzip compressed data, was "dist\gadapt-0.2.13.tar", last modified: Thu May 25 20:01:16 2023, max compression
```

## Comparing `gadapt-0.2.12.tar` & `gadapt-0.2.13.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.198118 gadapt-0.2.12/
--rw-rw-rw-   0        0        0      340 2023-05-24 07:02:18.198617 gadapt-0.2.12/PKG-INFO
--rw-rw-rw-   0        0        0       43 2023-05-20 09:05:31.000000 gadapt-0.2.12/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:17.992616 gadapt-0.2.12/gadapt/
--rw-rw-rw-   0        0        0        2 2023-05-24 06:11:19.000000 gadapt-0.2.12/gadapt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.011116 gadapt-0.2.12/gadapt/cost_finding/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:46.000000 gadapt-0.2.12/gadapt/cost_finding/__init__.py
--rw-rw-rw-   0        0        0      728 2023-05-24 06:38:53.000000 gadapt-0.2.12/gadapt/cost_finding/base_cost_finder.py
--rw-rw-rw-   0        0        0     2112 2023-05-24 06:54:25.000000 gadapt-0.2.12/gadapt/cost_finding/common_cost_finder.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.018118 gadapt-0.2.12/gadapt/crossover/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:39.000000 gadapt-0.2.12/gadapt/crossover/__init__.py
--rw-rw-rw-   0        0        0     7036 2023-05-24 06:54:25.000000 gadapt-0.2.12/gadapt/crossover/base_crossover.py
--rw-rw-rw-   0        0        0     1257 2023-05-23 23:45:14.000000 gadapt-0.2.12/gadapt/crossover/uniform_crossover.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.022117 gadapt-0.2.12/gadapt/execution/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:34.000000 gadapt-0.2.12/gadapt/execution/__init__.py
--rw-rw-rw-   0        0        0     3343 2023-05-24 06:48:25.000000 gadapt-0.2.12/gadapt/execution/ga_executor.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.028617 gadapt-0.2.12/gadapt/exit_check/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:29.000000 gadapt-0.2.12/gadapt/exit_check/__init__.py
--rw-rw-rw-   0        0        0      315 2023-05-23 23:28:45.000000 gadapt-0.2.12/gadapt/exit_check/avg_cost_exit_checker.py
--rw-rw-rw-   0        0        0     1060 2023-05-24 06:38:53.000000 gadapt-0.2.12/gadapt/exit_check/base_exit_checker.py
--rw-rw-rw-   0        0        0      305 2023-05-23 23:28:54.000000 gadapt-0.2.12/gadapt/exit_check/min_cost_exit_checker.py
--rw-rw-rw-   0        0        0      387 2023-05-23 23:29:00.000000 gadapt-0.2.12/gadapt/exit_check/requested_cost_exit_checker.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.031618 gadapt-0.2.12/gadapt/factory/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:24.000000 gadapt-0.2.12/gadapt/factory/__init__.py
--rw-rw-rw-   0        0        0    10088 2023-05-24 06:38:53.000000 gadapt-0.2.12/gadapt/factory/ga_factory.py
--rw-rw-rw-   0        0        0     7812 2023-05-24 06:54:24.000000 gadapt-0.2.12/gadapt/ga.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.034617 gadapt-0.2.12/gadapt/ga_logging/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:17.000000 gadapt-0.2.12/gadapt/ga_logging/__init__.py
--rw-rw-rw-   0        0        0     2123 2023-05-23 23:47:24.000000 gadapt-0.2.12/gadapt/ga_logging/logging_settings.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.054617 gadapt-0.2.12/gadapt/ga_model/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:07.000000 gadapt-0.2.12/gadapt/ga_model/__init__.py
--rw-rw-rw-   0        0        0     6676 2023-05-24 06:43:20.000000 gadapt-0.2.12/gadapt/ga_model/chromosome.py
--rw-rw-rw-   0        0        0      683 2023-05-21 10:44:03.000000 gadapt-0.2.12/gadapt/ga_model/definitions.py
--rw-rw-rw-   0        0        0     3718 2023-05-23 23:14:52.000000 gadapt-0.2.12/gadapt/ga_model/ga_options.py
--rw-rw-rw-   0        0        0     1423 2023-05-23 23:26:32.000000 gadapt-0.2.12/gadapt/ga_model/ga_results.py
--rw-rw-rw-   0        0        0     1339 2023-05-24 06:38:53.000000 gadapt-0.2.12/gadapt/ga_model/gene.py
--rw-rw-rw-   0        0        0     2546 2023-05-24 06:38:53.000000 gadapt-0.2.12/gadapt/ga_model/genetic_variable.py
--rw-rw-rw-   0        0        0       53 2023-05-17 16:44:58.000000 gadapt-0.2.12/gadapt/ga_model/message_levels.py
--rw-rw-rw-   0        0        0    10337 2023-05-24 06:38:53.000000 gadapt-0.2.12/gadapt/ga_model/population.py
--rw-rw-rw-   0        0        0      785 2023-05-24 06:38:53.000000 gadapt-0.2.12/gadapt/ga_model/ranking_model.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.059117 gadapt-0.2.12/gadapt/gene_combination/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:01.000000 gadapt-0.2.12/gadapt/gene_combination/__init__.py
--rw-rw-rw-   0        0        0      308 2023-05-24 06:38:53.000000 gadapt-0.2.12/gadapt/gene_combination/base_gene_combination.py
--rw-rw-rw-   0        0        0      837 2023-05-23 23:22:44.000000 gadapt-0.2.12/gadapt/gene_combination/blending_gene_combination.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.060617 gadapt-0.2.12/gadapt/immigration/
--rw-rw-rw-   0        0        0        0 2023-05-24 00:04:24.000000 gadapt-0.2.12/gadapt/immigration/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.066616 gadapt-0.2.12/gadapt/immigration/chromosome_immigration/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:55.000000 gadapt-0.2.12/gadapt/immigration/chromosome_immigration/__init__.py
--rw-rw-rw-   0        0        0      611 2023-05-24 06:38:53.000000 gadapt-0.2.12/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py
--rw-rw-rw-   0        0        0      336 2023-05-23 23:22:33.000000 gadapt-0.2.12/gadapt/immigration/chromosome_immigration/random_chromosome_immigrator.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.070616 gadapt-0.2.12/gadapt/immigration/population_immigration/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:43.000000 gadapt-0.2.12/gadapt/immigration/population_immigration/__init__.py
--rw-rw-rw-   0        0        0      174 2023-05-24 06:38:53.000000 gadapt-0.2.12/gadapt/immigration/population_immigration/base_population_immigrator.py
--rw-rw-rw-   0        0        0      831 2023-05-23 23:22:20.000000 gadapt-0.2.12/gadapt/immigration/population_immigration/common_population_immigrator.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.071617 gadapt-0.2.12/gadapt/mutation/
--rw-rw-rw-   0        0        0        0 2023-05-24 00:04:04.000000 gadapt-0.2.12/gadapt/mutation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.076617 gadapt-0.2.12/gadapt/mutation/chromosome_mutation/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:32.000000 gadapt-0.2.12/gadapt/mutation/chromosome_mutation/__init__.py
--rw-rw-rw-   0        0        0      841 2023-05-24 06:38:53.000000 gadapt-0.2.12/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py
--rw-rw-rw-   0        0        0     2938 2023-05-24 06:54:25.000000 gadapt-0.2.12/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py
--rw-rw-rw-   0        0        0      936 2023-05-23 23:45:26.000000 gadapt-0.2.12/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.093616 gadapt-0.2.12/gadapt/mutation/population_mutation/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:12.000000 gadapt-0.2.12/gadapt/mutation/population_mutation/__init__.py
--rw-rw-rw-   0        0        0     1402 2023-05-24 06:38:53.000000 gadapt-0.2.12/gadapt/mutation/population_mutation/base_population_mutator.py
--rw-rw-rw-   0        0        0     1269 2023-05-23 23:43:50.000000 gadapt-0.2.12/gadapt/mutation/population_mutation/composed_population_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.096618 gadapt-0.2.12/gadapt/mutation/population_mutation/cost_diversity/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:26.000000 gadapt-0.2.12/gadapt/mutation/population_mutation/cost_diversity/__init__.py
--rw-rw-rw-   0        0        0     2899 2023-05-24 06:54:25.000000 gadapt-0.2.12/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py
--rw-rw-rw-   0        0        0     1982 2023-05-23 23:45:44.000000 gadapt-0.2.12/gadapt/mutation/population_mutation/parents_diversity_population_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.120617 gadapt-0.2.12/gadapt/mutation/population_mutation/previous_cost_diversity/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:19.000000 gadapt-0.2.12/gadapt/mutation/population_mutation/previous_cost_diversity/__init__.py
--rw-rw-rw-   0        0        0     3769 2023-05-24 06:54:24.000000 gadapt-0.2.12/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_population_mutator.py
--rw-rw-rw-   0        0        0      469 2023-05-24 06:38:53.000000 gadapt-0.2.12/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_property_taker.py
--rw-rw-rw-   0        0        0     1069 2023-05-23 23:46:12.000000 gadapt-0.2.12/gadapt/mutation/population_mutation/random_population_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.123617 gadapt-0.2.12/gadapt/parent_selection/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:56.000000 gadapt-0.2.12/gadapt/parent_selection/__init__.py
--rw-rw-rw-   0        0        0      299 2023-05-24 06:38:53.000000 gadapt-0.2.12/gadapt/parent_selection/base_parent_selector.py
--rw-rw-rw-   0        0        0      883 2023-05-23 23:20:13.000000 gadapt-0.2.12/gadapt/parent_selection/sampling_parent_selector.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.134116 gadapt-0.2.12/gadapt/sampling/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:48.000000 gadapt-0.2.12/gadapt/sampling/__init__.py
--rw-rw-rw-   0        0        0      707 2023-05-24 06:38:53.000000 gadapt-0.2.12/gadapt/sampling/base_sampling.py
--rw-rw-rw-   0        0        0      433 2023-05-23 23:19:58.000000 gadapt-0.2.12/gadapt/sampling/from_top_to_bottom_sampling.py
--rw-rw-rw-   0        0        0      425 2023-05-23 23:46:22.000000 gadapt-0.2.12/gadapt/sampling/random_sampling.py
--rw-rw-rw-   0        0        0     1812 2023-05-23 23:46:32.000000 gadapt-0.2.12/gadapt/sampling/roulette_wheel_sampling.py
--rw-rw-rw-   0        0        0     2622 2023-05-23 23:46:42.000000 gadapt-0.2.12/gadapt/sampling/tournament_sampling.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.163619 gadapt-0.2.12/gadapt/string_operation/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:11:28.000000 gadapt-0.2.12/gadapt/string_operation/__init__.py
--rw-rw-rw-   0        0        0     3219 2023-05-24 06:41:20.000000 gadapt-0.2.12/gadapt/string_operation/ga_strings.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.168619 gadapt-0.2.12/gadapt/utils/
--rw-rw-rw-   0        0        0      229 2023-05-04 17:34:59.000000 gadapt-0.2.12/gadapt/utils/TimeStampFormatter.py
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:32.000000 gadapt-0.2.12/gadapt/utils/__init__.py
--rw-rw-rw-   0        0        0     1228 2023-05-24 06:38:53.000000 gadapt-0.2.12/gadapt/utils/ga_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.172118 gadapt-0.2.12/gadapt/validation/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:26.000000 gadapt-0.2.12/gadapt/validation/__init__.py
--rw-rw-rw-   0        0        0      787 2023-05-24 06:45:03.000000 gadapt-0.2.12/gadapt/validation/base_options_validator.py
--rw-rw-rw-   0        0        0    15281 2023-05-24 06:38:52.000000 gadapt-0.2.12/gadapt/validation/common_options_validator.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.196118 gadapt-0.2.12/gadapt/variable_update/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:11.000000 gadapt-0.2.12/gadapt/variable_update/__init__.py
--rw-rw-rw-   0        0        0      176 2023-05-24 06:38:52.000000 gadapt-0.2.12/gadapt/variable_update/base_variable_updater.py
--rw-rw-rw-   0        0        0     2001 2023-05-24 06:54:25.000000 gadapt-0.2.12/gadapt/variable_update/common_variable_updater.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:02:18.006617 gadapt-0.2.12/gadapt.egg-info/
--rw-rw-rw-   0        0        0      340 2023-05-24 07:02:17.000000 gadapt-0.2.12/gadapt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3461 2023-05-24 07:02:17.000000 gadapt-0.2.12/gadapt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 07:02:17.000000 gadapt-0.2.12/gadapt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-24 07:02:17.000000 gadapt-0.2.12/gadapt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-05-24 07:02:18.200619 gadapt-0.2.12/setup.cfg
--rw-rw-rw-   0        0        0      434 2023-05-24 07:02:04.000000 gadapt-0.2.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.872894 gadapt-0.2.13/
+-rw-rw-rw-   0        0        0      320 2023-05-25 20:01:16.873893 gadapt-0.2.13/PKG-INFO
+-rw-rw-rw-   0        0        0     3623 2023-05-25 15:08:36.000000 gadapt-0.2.13/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.658891 gadapt-0.2.13/gadapt/
+-rw-rw-rw-   0        0        0        2 2023-05-24 06:11:19.000000 gadapt-0.2.13/gadapt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.683891 gadapt-0.2.13/gadapt/cost_finding/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:46.000000 gadapt-0.2.13/gadapt/cost_finding/__init__.py
+-rw-rw-rw-   0        0        0      728 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/cost_finding/base_cost_finder.py
+-rw-rw-rw-   0        0        0     2112 2023-05-24 06:54:25.000000 gadapt-0.2.13/gadapt/cost_finding/common_cost_finder.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.696392 gadapt-0.2.13/gadapt/crossover/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:39.000000 gadapt-0.2.13/gadapt/crossover/__init__.py
+-rw-rw-rw-   0        0        0     7036 2023-05-24 06:54:25.000000 gadapt-0.2.13/gadapt/crossover/base_crossover.py
+-rw-rw-rw-   0        0        0     1257 2023-05-23 23:45:14.000000 gadapt-0.2.13/gadapt/crossover/uniform_crossover.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.698892 gadapt-0.2.13/gadapt/execution/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:34.000000 gadapt-0.2.13/gadapt/execution/__init__.py
+-rw-rw-rw-   0        0        0     3101 2023-05-25 16:03:23.000000 gadapt-0.2.13/gadapt/execution/ga_executor.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.705893 gadapt-0.2.13/gadapt/exit_check/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:29.000000 gadapt-0.2.13/gadapt/exit_check/__init__.py
+-rw-rw-rw-   0        0        0      315 2023-05-23 23:28:45.000000 gadapt-0.2.13/gadapt/exit_check/avg_cost_exit_checker.py
+-rw-rw-rw-   0        0        0     1060 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/exit_check/base_exit_checker.py
+-rw-rw-rw-   0        0        0      305 2023-05-23 23:28:54.000000 gadapt-0.2.13/gadapt/exit_check/min_cost_exit_checker.py
+-rw-rw-rw-   0        0        0      387 2023-05-23 23:29:00.000000 gadapt-0.2.13/gadapt/exit_check/requested_cost_exit_checker.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.709391 gadapt-0.2.13/gadapt/factory/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:24.000000 gadapt-0.2.13/gadapt/factory/__init__.py
+-rw-rw-rw-   0        0        0     9957 2023-05-25 16:26:07.000000 gadapt-0.2.13/gadapt/factory/ga_factory.py
+-rw-rw-rw-   0        0        0     8842 2023-05-25 16:17:40.000000 gadapt-0.2.13/gadapt/ga.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.712393 gadapt-0.2.13/gadapt/ga_logging/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:17.000000 gadapt-0.2.13/gadapt/ga_logging/__init__.py
+-rw-rw-rw-   0        0        0     2123 2023-05-24 07:42:21.000000 gadapt-0.2.13/gadapt/ga_logging/logging_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.742393 gadapt-0.2.13/gadapt/ga_model/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:07.000000 gadapt-0.2.13/gadapt/ga_model/__init__.py
+-rw-rw-rw-   0        0        0     6676 2023-05-24 06:43:20.000000 gadapt-0.2.13/gadapt/ga_model/chromosome.py
+-rw-rw-rw-   0        0        0      683 2023-05-21 10:44:03.000000 gadapt-0.2.13/gadapt/ga_model/definitions.py
+-rw-rw-rw-   0        0        0     5248 2023-05-25 16:08:26.000000 gadapt-0.2.13/gadapt/ga_model/ga_options.py
+-rw-rw-rw-   0        0        0     1398 2023-05-24 16:01:11.000000 gadapt-0.2.13/gadapt/ga_model/ga_results.py
+-rw-rw-rw-   0        0        0     1339 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/ga_model/gene.py
+-rw-rw-rw-   0        0        0     2546 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/ga_model/genetic_variable.py
+-rw-rw-rw-   0        0        0       53 2023-05-17 16:44:58.000000 gadapt-0.2.13/gadapt/ga_model/message_levels.py
+-rw-rw-rw-   0        0        0    10169 2023-05-24 16:00:25.000000 gadapt-0.2.13/gadapt/ga_model/population.py
+-rw-rw-rw-   0        0        0      785 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/ga_model/ranking_model.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.754891 gadapt-0.2.13/gadapt/gene_combination/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:01.000000 gadapt-0.2.13/gadapt/gene_combination/__init__.py
+-rw-rw-rw-   0        0        0      308 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/gene_combination/base_gene_combination.py
+-rw-rw-rw-   0        0        0      837 2023-05-23 23:22:44.000000 gadapt-0.2.13/gadapt/gene_combination/blending_gene_combination.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.756391 gadapt-0.2.13/gadapt/immigration/
+-rw-rw-rw-   0        0        0        0 2023-05-24 00:04:24.000000 gadapt-0.2.13/gadapt/immigration/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.765894 gadapt-0.2.13/gadapt/immigration/chromosome_immigration/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:55.000000 gadapt-0.2.13/gadapt/immigration/chromosome_immigration/__init__.py
+-rw-rw-rw-   0        0        0      611 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py
+-rw-rw-rw-   0        0        0      336 2023-05-23 23:22:33.000000 gadapt-0.2.13/gadapt/immigration/chromosome_immigration/random_chromosome_immigrator.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.775392 gadapt-0.2.13/gadapt/immigration/population_immigration/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:43.000000 gadapt-0.2.13/gadapt/immigration/population_immigration/__init__.py
+-rw-rw-rw-   0        0        0      174 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/immigration/population_immigration/base_population_immigrator.py
+-rw-rw-rw-   0        0        0      831 2023-05-23 23:22:20.000000 gadapt-0.2.13/gadapt/immigration/population_immigration/common_population_immigrator.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.777393 gadapt-0.2.13/gadapt/mutation/
+-rw-rw-rw-   0        0        0        0 2023-05-24 00:04:04.000000 gadapt-0.2.13/gadapt/mutation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.789893 gadapt-0.2.13/gadapt/mutation/chromosome_mutation/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:32.000000 gadapt-0.2.13/gadapt/mutation/chromosome_mutation/__init__.py
+-rw-rw-rw-   0        0        0      841 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py
+-rw-rw-rw-   0        0        0     2938 2023-05-24 06:54:25.000000 gadapt-0.2.13/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py
+-rw-rw-rw-   0        0        0      936 2023-05-23 23:45:26.000000 gadapt-0.2.13/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.797892 gadapt-0.2.13/gadapt/mutation/population_mutation/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:12.000000 gadapt-0.2.13/gadapt/mutation/population_mutation/__init__.py
+-rw-rw-rw-   0        0        0     1402 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/mutation/population_mutation/base_population_mutator.py
+-rw-rw-rw-   0        0        0     1269 2023-05-23 23:43:50.000000 gadapt-0.2.13/gadapt/mutation/population_mutation/composed_population_mutator.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.800393 gadapt-0.2.13/gadapt/mutation/population_mutation/cost_diversity/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:26.000000 gadapt-0.2.13/gadapt/mutation/population_mutation/cost_diversity/__init__.py
+-rw-rw-rw-   0        0        0     2899 2023-05-24 06:54:25.000000 gadapt-0.2.13/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py
+-rw-rw-rw-   0        0        0     1982 2023-05-23 23:45:44.000000 gadapt-0.2.13/gadapt/mutation/population_mutation/parents_diversity_population_mutator.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.803894 gadapt-0.2.13/gadapt/mutation/population_mutation/previous_cost_diversity/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:19.000000 gadapt-0.2.13/gadapt/mutation/population_mutation/previous_cost_diversity/__init__.py
+-rw-rw-rw-   0        0        0     3769 2023-05-24 06:54:24.000000 gadapt-0.2.13/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_population_mutator.py
+-rw-rw-rw-   0        0        0      469 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_property_taker.py
+-rw-rw-rw-   0        0        0     1069 2023-05-23 23:46:12.000000 gadapt-0.2.13/gadapt/mutation/population_mutation/random_population_mutator.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.807392 gadapt-0.2.13/gadapt/parent_selection/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:12:56.000000 gadapt-0.2.13/gadapt/parent_selection/__init__.py
+-rw-rw-rw-   0        0        0      299 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/parent_selection/base_parent_selector.py
+-rw-rw-rw-   0        0        0      883 2023-05-23 23:20:13.000000 gadapt-0.2.13/gadapt/parent_selection/sampling_parent_selector.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.826392 gadapt-0.2.13/gadapt/sampling/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:12:48.000000 gadapt-0.2.13/gadapt/sampling/__init__.py
+-rw-rw-rw-   0        0        0      707 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/sampling/base_sampling.py
+-rw-rw-rw-   0        0        0      433 2023-05-23 23:19:58.000000 gadapt-0.2.13/gadapt/sampling/from_top_to_bottom_sampling.py
+-rw-rw-rw-   0        0        0      425 2023-05-23 23:46:22.000000 gadapt-0.2.13/gadapt/sampling/random_sampling.py
+-rw-rw-rw-   0        0        0     1812 2023-05-23 23:46:32.000000 gadapt-0.2.13/gadapt/sampling/roulette_wheel_sampling.py
+-rw-rw-rw-   0        0        0     2622 2023-05-23 23:46:42.000000 gadapt-0.2.13/gadapt/sampling/tournament_sampling.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.828393 gadapt-0.2.13/gadapt/string_operation/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:11:28.000000 gadapt-0.2.13/gadapt/string_operation/__init__.py
+-rw-rw-rw-   0        0        0     3219 2023-05-24 06:41:20.000000 gadapt-0.2.13/gadapt/string_operation/ga_strings.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.831893 gadapt-0.2.13/gadapt/utils/
+-rw-rw-rw-   0        0        0      229 2023-05-04 17:34:59.000000 gadapt-0.2.13/gadapt/utils/TimeStampFormatter.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:12:32.000000 gadapt-0.2.13/gadapt/utils/__init__.py
+-rw-rw-rw-   0        0        0     1272 2023-05-25 15:37:31.000000 gadapt-0.2.13/gadapt/utils/ga_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.835892 gadapt-0.2.13/gadapt/validation/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:12:26.000000 gadapt-0.2.13/gadapt/validation/__init__.py
+-rw-rw-rw-   0        0        0      787 2023-05-24 06:45:03.000000 gadapt-0.2.13/gadapt/validation/base_options_validator.py
+-rw-rw-rw-   0        0        0    17426 2023-05-25 15:43:59.000000 gadapt-0.2.13/gadapt/validation/common_options_validator.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.869892 gadapt-0.2.13/gadapt/variable_update/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:12:11.000000 gadapt-0.2.13/gadapt/variable_update/__init__.py
+-rw-rw-rw-   0        0        0      176 2023-05-24 06:38:52.000000 gadapt-0.2.13/gadapt/variable_update/base_variable_updater.py
+-rw-rw-rw-   0        0        0     2001 2023-05-24 06:54:25.000000 gadapt-0.2.13/gadapt/variable_update/common_variable_updater.py
+drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.679391 gadapt-0.2.13/gadapt.egg-info/
+-rw-rw-rw-   0        0        0      320 2023-05-25 20:01:03.000000 gadapt-0.2.13/gadapt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3461 2023-05-25 20:01:03.000000 gadapt-0.2.13/gadapt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 20:01:03.000000 gadapt-0.2.13/gadapt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-25 20:01:03.000000 gadapt-0.2.13/gadapt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-05-25 20:01:16.877393 gadapt-0.2.13/setup.cfg
+-rw-rw-rw-   0        0        0      389 2023-05-25 20:00:39.000000 gadapt-0.2.13/setup.py
```

### Comparing `gadapt-0.2.12/gadapt/cost_finding/base_cost_finder.py` & `gadapt-0.2.13/gadapt/cost_finding/base_cost_finder.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/cost_finding/common_cost_finder.py` & `gadapt-0.2.13/gadapt/cost_finding/common_cost_finder.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/crossover/base_crossover.py` & `gadapt-0.2.13/gadapt/crossover/base_crossover.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/crossover/uniform_crossover.py` & `gadapt-0.2.13/gadapt/crossover/uniform_crossover.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/execution/ga_executor.py` & `gadapt-0.2.13/gadapt/execution/ga_executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,21 +14,15 @@
 
     def execute(self) -> GAResults:
         results = GAResults()
         try: 
             init_logging(self.ga_options.logging)                           
         except Exception as ex:
             results.messages.append((message_levels.WARNING, "Logging failed. Error message: {exc}".format(exc=str(ex))))
-            self.ga_options.logging = False
-        validator = self.factory.get_options_validator()
-        validator.validate()
-        if not validator.success:
-            results.success = False
-            results.messages = validator.validation_messages
-            return results
+            self.ga_options.logging = False        
         #try:
         chromosome_mutator = self.factory.get_chromosome_mutator()
         population_mutator = self.factory.get_population_mutator()
         exit_checker = self.factory.get_exit_checker()
         cost_finder = self.factory.get_cost_finder()
         population_immigrator = self.factory.get_population_immigrator()
         chromosome_immigrator = self.factory.get_chromosome_immigrator()
```

### Comparing `gadapt-0.2.12/gadapt/exit_check/base_exit_checker.py` & `gadapt-0.2.13/gadapt/exit_check/base_exit_checker.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/factory/ga_factory.py` & `gadapt-0.2.13/gadapt/factory/ga_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,80 +33,89 @@
 from gadapt.gene_combination.base_gene_combination import BaseGeneCombination
 from gadapt.gene_combination.blending_gene_combination import BlendingGeneCombination
 from gadapt.variable_update.common_variable_updater import CommonVariableUpdater
 import gadapt.ga_model.definitions as definitions
 
 
 class GAFactory:
-    def __init__(self, ga) -> None:
-        self.ga_options = ga
+    def __init__(self, ga, options: GAOptions) -> None:
+        self.ga = ga
+        self.options = options
 
     @property
-    def ga_options(self):
-        return self._ga_options
+    def ga(self):
+        return self._ga
 
-    @ga_options.setter
-    def ga_options(self, value):
-        self._ga_options = value
+    @ga.setter
+    def ga(self, value):
+        self._ga = value
+
+    @property
+    def options(self):
+        return self._options
+
+    @options.setter
+    def options(self, value):
+        self._options = value
 
     def get_cost_finder(self) -> BaseCostFinder:
         return CommonCostFinder()
 
     def get_population_immigrator(self) -> BasePopulationImmigrator:
         return CommonPopulationImmigrator()
 
     def get_chromosome_immigrator(self) -> BaseChromosomeImmigrator:
         return RandomChromosomeImmigrator()
 
     def get_chromosome_mutator(self) -> BaseChromosomeMutator:
-        if self.ga_options.chromosome_mutation.strip() == definitions.CROSS_DIVERSITY:
-            return CrossDiversityChromosomeMutator(self.get_sampling_method(self.ga_options.cross_diversity_mutation_gene_selection))
-        elif self.ga_options.chromosome_mutation.strip() == definitions.RANDOM:
+        if self.ga.chromosome_mutation.strip() == definitions.CROSS_DIVERSITY:
+            return CrossDiversityChromosomeMutator(self.get_sampling_method(self.ga.cross_diversity_mutation_gene_selection))
+        elif self.ga.chromosome_mutation.strip() == definitions.RANDOM:
             return RandomChromosomeMutator()
         else:
             raise Exception("unknown chromosome mutation")
 
     def population_mutator_options_validation(self):
-        mutator_strings = self.ga_options.population_mutation.split(definitions.PARAM_SEPARATOR)
+        mutator_strings = self.ga.population_mutation.split(definitions.PARAM_SEPARATOR)
         for s in mutator_strings:
             if not s.strip() in definitions.POPULATION_MUTATOR_STRINGS:
                 raise Exception(s + " is not defined as option for population mutation")
 
     def get_population_mutator(self, population_mutator_string=None) -> BasePopulationMutator:
         self.population_mutator_options_validation()
         if population_mutator_string is None:
-            population_mutator_string = self.ga_options.population_mutation.strip()
+            population_mutator_string = self.ga.population_mutation.strip()
         if population_mutator_string.find(definitions.PARAM_SEPARATOR) > -1:
             return self.get_population_mutator_combined()
         elif population_mutator_string == definitions.COST_DIVERSITY:
-            return CostDiversityPopulationMutator(self.ga_options, ParentsDiversityPopulationMutator(self.get_sampling_method(self.ga_options.parent_diversity_mutation_chromosome_selection), self.ga_options))
+            return CostDiversityPopulationMutator(self.options, ParentsDiversityPopulationMutator(self.get_sampling_method(self.ga.parent_diversity_mutation_chromosome_selection), self.options))
         elif population_mutator_string == definitions.PARENTS_DIVERSITY:
-            return ParentsDiversityPopulationMutator(self.get_sampling_method(self.ga_options.parent_diversity_mutation_chromosome_selection), self.ga_options)
+            return ParentsDiversityPopulationMutator(self.get_sampling_method(self.ga.parent_diversity_mutation_chromosome_selection), self.options)
         elif population_mutator_string == definitions.RANDOM:
-            return RandomPopulationMutator(self.ga_options)
+            return RandomPopulationMutator(self.options)
         else:
             raise Exception("unknown population mutation")
 
     def get_previous_cost_diversity_property_taker(self) -> BasePreviousCostDiversityPropertyTaker:
         return AvgPreviousCostCostDiversityPropertyTaker()
 
     def get_population_mutator_combined(self) -> ComposedPopulationMutator:
-        mutator_strings = [ms.strip() for ms in self.ga_options.population_mutation.split(definitions.PARAM_SEPARATOR)]
+        mutator_strings = [ms.strip() for ms in self.ga.population_mutation.split(definitions.PARAM_SEPARATOR)]
         if (self.is_cost_diversity_random(mutator_strings)):
-            return CostDiversityPopulationMutator(self.ga_options, RandomPopulationMutator(self.ga_options))
+            return CostDiversityPopulationMutator(self.options, RandomPopulationMutator(self.options))
         if (self.is_cost_diversity_parents_diversity(mutator_strings)):
-            return CostDiversityPopulationMutator(self.ga_options, ParentsDiversityPopulationMutator(self.get_sampling_method(self.ga_options.parent_diversity_mutation_chromosome_selection), self.ga_options))
+            return CostDiversityPopulationMutator(self.options, ParentsDiversityPopulationMutator(self.get_sampling_method(self.ga.parent_diversity_mutation_chromosome_selection), self.options))
         if self.is_cost_diversity_parents_diversity_random(mutator_strings):
-            composedPopulationMutator = ComposedPopulationMutator(self.ga_options)
+            composedPopulationMutator = ComposedPopulationMutator(self.options)
             composedPopulationMutator.append(ParentsDiversityPopulationMutator(self.get_sampling_method(
-                self.ga_options.parent_diversity_mutation_chromosome_selection), self.ga_options))
+                self.ga.parent_diversity_mutation_chromosome_selection), self.options))
             composedPopulationMutator.append(
-                RandomPopulationMutator(self.ga_options))
-            return PreviousCostDiversityPopulationMutator(self.ga_options, composedPopulationMutator)
-        composedPopulationMutator = ComposedPopulationMutator(self.ga_options)
+                RandomPopulationMutator(self.options))
+            return PreviousCostDiversityPopulationMutator(self.options, composedPopulationMutator)
+        composedPopulationMutator = ComposedPopulationMutator(self.options)
         for ms in mutator_strings:
             composedPopulationMutator.append(self.get_population_mutator(ms))
         return composedPopulationMutator
 
     def is_cost_diversity_random(self, mutator_strings: list):
         if len(mutator_strings) == 2 and definitions.COST_DIVERSITY in mutator_strings and definitions.RANDOM in mutator_strings:
             return True
@@ -119,15 +128,15 @@
 
     def is_cost_diversity_parents_diversity_random(self, mutator_strings: list):
         if len(mutator_strings) == 3 and definitions.COST_DIVERSITY in mutator_strings and definitions.PARENTS_DIVERSITY in mutator_strings and definitions.RANDOM in mutator_strings:
             return True
         return False
 
     def get_parent_selector(self) -> BaseParentSelector:
-        return SamplingParentSelector(self.get_sampling_method(self.ga_options.parent_selection))
+        return SamplingParentSelector(self.get_sampling_method(self.ga.parent_selection))
 
     def get_sampling_method(self, str) -> BaseSampling:
         str_value = str
         sampling_method_strings = str.split(definitions.PARAM_SEPARATOR)
         other_value = None
         if len(sampling_method_strings) > 1:
             str_value = sampling_method_strings[0]
@@ -143,21 +152,18 @@
             return RandomSampling()
         return RouletteWheelSampling()
 
     def get_gene_combination(self) -> BaseGeneCombination:
         return BlendingGeneCombination()
 
     def get_exit_checker(self) -> BaseExitChecker:
-        if self.ga_options.exit_check == definitions.AVG_COST:
-            return AvgCostExitChecker(self.ga_options.max_attempt_no)
-        if self.ga_options.exit_check == definitions.MIN_COST:
-            return MinCostExitChecker(self.ga_options.max_attempt_no)
-        return RequestedCostExitChecker(self.ga_options.requested_cost)
+        if self.ga.exit_check == definitions.AVG_COST:
+            return AvgCostExitChecker(self.ga.max_attempt_no)
+        if self.ga.exit_check == definitions.MIN_COST:
+            return MinCostExitChecker(self.ga.max_attempt_no)
+        return RequestedCostExitChecker(self.ga.requested_cost)
 
     def get_crossover(self, gene_combination: BaseGeneCombination, mutator: BaseChromosomeMutator, immigrator: BaseChromosomeImmigrator) -> BaseCrossover:
         return UniformCrossover(gene_combination, mutator, immigrator)
 
     def get_variable_updater(self):
         return CommonVariableUpdater()
-    
-    def get_options_validator(self) -> BaseOptionsValidator:
-        return CommonOptionsValidator(self.ga_options)
```

### Comparing `gadapt-0.2.12/gadapt/ga.py` & `gadapt-0.2.13/gadapt/ga.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,57 +3,68 @@
 from gadapt.factory.ga_factory import GAFactory
 from gadapt.ga_model.genetic_variable import GeneticVariable
 from gadapt.ga_model.ga_options import GAOptions
 from gadapt.ga_model.ga_results import GAResults
 from gadapt.ga_model.population import Population
 import gadapt.utils.ga_utils as ga_utils
 import gadapt.ga_model.definitions as definitions
+from gadapt.validation.common_options_validator import CommonOptionsValidator
 
 class GA:
     def __init__(self,
                  cost_function = None,
                  population_size = 64, 
                  exit_check = definitions.AVG_COST,
                  requested_cost = sys.float_info.max,
                  max_attempt_no = 10,
                  parent_selection = definitions.ROULETTE_WHEEL,
                  population_mutation = definitions.COST_DIVERSITY, 
-                 number_of_mutation_chromosomes = 1,    
+                 number_of_mutation_chromosomes = -1,    
+                 percentage_of_mutation_chromosomes = 10.0,
                  parent_diversity_mutation_chromosome_selection = definitions.ROULETTE_WHEEL, 
                  must_mutate_for_same_parents = True,
                  chromosome_mutation = definitions.CROSS_DIVERSITY,                                        
-                 number_of_mutation_genes = 1,                     
+                 number_of_mutation_genes = -1,   
+                 percentage_of_mutations_genes = 10.0,           
                  cross_diversity_mutation_gene_selection = definitions.ROULETTE_WHEEL,
                  immigration_number = 0,                                                                                   
                  logging = False,                                                              
                  timeout = 120
                  ) -> None:                     
         self.cost_function = cost_function
         self.population_size = population_size
         self.exit_check = exit_check 
         self.requested_cost = requested_cost 
         self.max_attempt_no = max_attempt_no
         self.parent_selection = parent_selection
         self.population_mutation = population_mutation
         self.must_mutate_for_same_parents = must_mutate_for_same_parents
-        self._number_of_mutation_chromosomes = -1
         self.number_of_mutation_chromosomes = number_of_mutation_chromosomes
-        self._number_of_mutation_chromosomes_changed = False
+        self.percentage_of_mutation_chromosomes = percentage_of_mutation_chromosomes
         self.number_of_mutation_genes = number_of_mutation_genes
+        self.percentage_of_mutation_genes = percentage_of_mutations_genes
         self.chromosome_mutation = chromosome_mutation        
         self.immigration_number = immigration_number                                              
         self.logging = logging
         self._genetic_variables = []        
         self.cross_diversity_mutation_gene_selection = cross_diversity_mutation_gene_selection
         self.parent_diversity_mutation_chromosome_selection = parent_diversity_mutation_chromosome_selection        
         self.timeout = timeout 
         self._current_gv_id = 0               
 
-    def execute(self) -> GAResults:        
-        return GAExecutor(GAOptions(self) , GAFactory(self)).execute()
+    def execute(self) -> GAResults:  
+        validator = CommonOptionsValidator(self)
+        validator.validate()
+        if not validator.success:
+            results = GAResults()
+            results.success = False
+            results.messages = validator.validation_messages
+            return results
+        ga_options = GAOptions(self)  
+        return GAExecutor(ga_options, GAFactory(self, ga_options)).execute()
         
     @property
     def population_size(self) -> int:
         return self._population_size
     
     @population_size.setter
     def population_size(self, value: int):
@@ -82,23 +93,36 @@
         return self._number_of_mutation_genes
     
     @number_of_mutation_genes.setter
     def number_of_mutation_genes(self, value: int):
         self._number_of_mutation_genes = ga_utils.try_get_int(value)
 
     @property
+    def percentage_of_mutation_genes(self) -> float:
+        return self._percentage_of_mutation_genes
+
+    @percentage_of_mutation_genes.setter
+    def percentage_of_mutation_genes(self, value: float):
+        self._percentage_of_mutation_genes = ga_utils.try_get_float(value)
+
+    @property
     def number_of_mutation_chromosomes(self) -> int:
         return self._number_of_mutation_chromosomes
     
     @number_of_mutation_chromosomes.setter
     def number_of_mutation_chromosomes(self, value: int):
-        first_time = self._number_of_mutation_chromosomes == -1
         self._number_of_mutation_chromosomes = ga_utils.try_get_int(value)
-        if not first_time:
-            self._number_of_mutation_chromosomes_changed = True
+
+    @property
+    def percentage_of_mutation_chromosomes(self) -> float:
+        return self._percentage_of_mutation_chromosomes
+
+    @percentage_of_mutation_chromosomes.setter
+    def percentage_of_mutation_chromosomes(self, value: float):
+        self._percentage_of_mutation_chromosomes = ga_utils.try_get_float(value)
 
     @property
     def immigration_number(self) -> int:
         return self._immigration_number
     
     @immigration_number.setter
     def immigration_number(self, value: int):
```

### Comparing `gadapt-0.2.12/gadapt/ga_logging/logging_settings.py` & `gadapt-0.2.13/gadapt/ga_logging/logging_settings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/ga_model/chromosome.py` & `gadapt-0.2.13/gadapt/ga_model/chromosome.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/ga_model/definitions.py` & `gadapt-0.2.13/gadapt/ga_model/definitions.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/ga_model/ga_results.py` & `gadapt-0.2.13/gadapt/ga_model/ga_results.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import List
 import gadapt.string_operation.ga_strings as ga_strings
 
 class GAResults:
     def __init__(self) -> None:
         self._success = True
         self.result_values = {}
         self._messages = []
```

### Comparing `gadapt-0.2.12/gadapt/ga_model/gene.py` & `gadapt-0.2.13/gadapt/ga_model/gene.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/ga_model/genetic_variable.py` & `gadapt-0.2.13/gadapt/ga_model/genetic_variable.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/ga_model/population.py` & `gadapt-0.2.13/gadapt/ga_model/population.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from typing import List, Tuple
 from gadapt.exit_check.base_exit_checker import BaseExitChecker
 from gadapt.cost_finding.base_cost_finder import BaseCostFinder
 from gadapt.crossover.base_crossover import BaseCrossover
 from gadapt.ga_model.chromosome import Chromosome
 from gadapt.ga_model.ga_options import GAOptions
 from gadapt.ga_model.gene import Gene
-from gadapt.ga_model.genetic_variable import GeneticVariable
 from gadapt.immigration.chromosome_immigration.base_chromosome_immigrator import BaseChromosomeImmigrator
 from gadapt.immigration.population_immigration.base_population_immigrator import BasePopulationImmigrator
 from gadapt.mutation.chromosome_mutation.base_chromosome_mutator import BaseChromosomeMutator
 from gadapt.mutation.population_mutation.base_population_mutator import BasePopulationMutator
 from gadapt.mutation.population_mutation.composed_population_mutator import ComposedPopulationMutator
-from sklearn.preprocessing import MinMaxScaler
 from gadapt.variable_update.base_variable_updater import BaseVariableUpdater
 import gadapt.string_operation.ga_strings as ga_strings
 from datetime import datetime
 import gadapt.ga_model.definitions as definitions
 
 class Population:
 
@@ -27,15 +25,14 @@
                  population_immigrator: BasePopulationImmigrator,
                  chromosome_immigrator: BaseChromosomeImmigrator,
                  selector,
                  crossover: BaseCrossover,
                  variable_updater: BaseVariableUpdater):
         if options.population_size < 4:
             raise Exception("Population size 4 must be higher than 3")        
-        self.scaler = MinMaxScaler(feature_range=(1, 2))
         self.options = options
         self.chromosome_mutator = chromosome_mutator
         self.population_mutator = population_mutator
         self.exit_checker = exit_checker
         self.cost_finder = cost_finder
         self.population_immigrator = population_immigrator
         self.chromosome_immigrator = chromosome_immigrator
```

### Comparing `gadapt-0.2.12/gadapt/ga_model/ranking_model.py` & `gadapt-0.2.13/gadapt/ga_model/ranking_model.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/gene_combination/blending_gene_combination.py` & `gadapt-0.2.13/gadapt/gene_combination/blending_gene_combination.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py` & `gadapt-0.2.13/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/immigration/population_immigration/common_population_immigrator.py` & `gadapt-0.2.13/gadapt/immigration/population_immigration/common_population_immigrator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py` & `gadapt-0.2.13/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py` & `gadapt-0.2.13/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py` & `gadapt-0.2.13/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/mutation/population_mutation/base_population_mutator.py` & `gadapt-0.2.13/gadapt/mutation/population_mutation/base_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/mutation/population_mutation/composed_population_mutator.py` & `gadapt-0.2.13/gadapt/mutation/population_mutation/composed_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py` & `gadapt-0.2.13/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/mutation/population_mutation/parents_diversity_population_mutator.py` & `gadapt-0.2.13/gadapt/mutation/population_mutation/parents_diversity_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_population_mutator.py` & `gadapt-0.2.13/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/mutation/population_mutation/random_population_mutator.py` & `gadapt-0.2.13/gadapt/mutation/population_mutation/random_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/parent_selection/sampling_parent_selector.py` & `gadapt-0.2.13/gadapt/parent_selection/sampling_parent_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/sampling/base_sampling.py` & `gadapt-0.2.13/gadapt/sampling/base_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/sampling/roulette_wheel_sampling.py` & `gadapt-0.2.13/gadapt/sampling/roulette_wheel_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/sampling/tournament_sampling.py` & `gadapt-0.2.13/gadapt/sampling/tournament_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/string_operation/ga_strings.py` & `gadapt-0.2.13/gadapt/string_operation/ga_strings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/utils/ga_utils.py` & `gadapt-0.2.13/gadapt/utils/ga_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,26 +27,26 @@
         except:
             return s
     return s
 
 def try_get_float(s):
     if isinstance(s, float):
         return s
-    if isinstance(s, str):
+    if isinstance(s, str) or isinstance(s, int):
         try:
             n = float(s)
             return n
         except:
             return s
     return s
 
 def try_get_bool(s):
     if isinstance(s, bool):
         return s
-    if isinstance(s, str):
+    if isinstance(s, str) or isinstance(s, int):
         try:
             n = bool(s)
             return n
         except:
             return s
     return s
```

### Comparing `gadapt-0.2.12/gadapt/validation/base_options_validator.py` & `gadapt-0.2.13/gadapt/validation/base_options_validator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt/validation/common_options_validator.py` & `gadapt-0.2.13/gadapt/validation/common_options_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,39 +89,54 @@
             self.add_message("Immigration Number must not be type same or greater than population size!")
             rslt &= False        
         elif self.options.immigration_number < 0:
             self.add_message("Immigration Number must ne eqals or greather than 0!")
             rslt &= False
         else:
             immigration_number = self.options.immigration_number
-        if self.options.number_of_mutation_chromosomes is None:
-            self.add_message("Number of Mutation Chromosomes must not be None!")
+        if self.options.number_of_mutation_chromosomes is None and self.options.percentage_of_mutation_chromosomes is None:
+            self.add_message("Number of Mutation Chromosomes or Percentage of Mutation Chromosomes must not be None!")
             rslt &= False
-        elif not isinstance(self.options.number_of_mutation_chromosomes, int):
-            self.add_message("Number of Mutation Chromosomes must be type int!")
+        elif not isinstance(self.options.number_of_mutation_chromosomes, int) and not isinstance(self.options.percentage_of_mutation_chromosomes, float):
+            self.add_message("Number of Mutation Chromosomes must be type int or Percentage of Mutation Chromosomes must be float!")
             rslt &= False
         else:
-            if (self.options.number_of_mutation_chromosomes < 0) or (population_size > 0 and self.options.number_of_mutation_chromosomes > (population_size // 2) - immigration_number):
-                self.add_message("Invalid number of mutation chromosomes: {0}".format(str(self.options.number_of_mutation_chromosomes)))
+            if (not self.options.number_of_mutation_chromosomes is None) and (isinstance(self.options.number_of_mutation_chromosomes, int)) and (self.options.number_of_mutation_chromosomes > 0):
+                if population_size > 0 and self.options.number_of_mutation_chromosomes > (population_size // 2) - immigration_number:
+                    self.add_message("Invalid number of mutation chromosomes: {0}".format(str(self.options.number_of_mutation_chromosomes)))
+                    rslt &= False
+            elif (self.options.percentage_of_mutation_chromosomes is None) or (not isinstance(self.options.percentage_of_mutation_chromosomes, float)):
+                self.add_message("Number of Mutation Chromosomes must have int value >=0 or Percentage of Mutation Chromosomes must have float (0.0-100.0) value! ")
+                rslt &= False
+            elif self.options.percentage_of_mutation_chromosomes < 0.0 or self.options.percentage_of_mutation_chromosomes > 100.0:
+                self.add_message("Invalid percentage of mutation chromosomes: {0} and number of mutation chromosomes: {1}".format(str(self.options.percentage_of_mutation_chromosomes, self.options.number_of_mutation_chromosomes)))
                 rslt &= False
         if self.options._genetic_variables is None:
             self.add_message("Genetic variables must not be None!")
             rslt &= False
         number_of_genetic_variables = len(self.options._genetic_variables) 
         if number_of_genetic_variables < 1:
             self.add_message("At least one genetic variable must be added!")
             rslt &= False
-        if self.options.number_of_mutation_genes is None:
-            self.add_message("Number Of Mutation Variables must not be None!")
+        if self.options.number_of_mutation_genes is None and self.options.percentage_of_mutation_genes is None:
+            self.add_message("Number Of Mutation Genes or Percentage Of Mutation Genes must not be None!")
             rslt &= False
-        elif not isinstance(self.options.number_of_mutation_genes, int):
-            self.add_message("Number Of Mutation Variables must be type int!")
+        elif not isinstance(self.options.number_of_mutation_genes, int) and not isinstance(self.options.percentage_of_mutation_genes, float):
+            self.add_message("Number Of Mutation Genes must have int value >=0 or Percentage Of Mutation Genes must have float (0.0-100.0) value!")
+            rslt &= False        
+        elif (not self.options.number_of_mutation_genes is None) and isinstance(self.options.number_of_mutation_genes, int) and (self.options.number_of_mutation_genes > 0):
+            if (number_of_genetic_variables > 0 and self.options.number_of_mutation_genes > number_of_genetic_variables):
+                self.add_message("Invalid number of mutation genes: {0}".format(
+                    str(self.options.number_of_mutation_genes)))
+                rslt &= False
+        elif (self.options.percentage_of_mutation_genes is None) or (not isinstance(self.options.percentage_of_mutation_genes, float)):
+            self.add_message("Number of Mutation Genes must have int value or Percentage of Mutation Genes must have float value! ")
             rslt &= False
-        elif (self.options.number_of_mutation_genes < 0) or (number_of_genetic_variables > 0 and self.options.number_of_mutation_genes > number_of_genetic_variables):
-            self.add_message("Invalid number of mutation variables: {0}".format(str(self.options.number_of_mutation_genes)))
+        elif self.options.percentage_of_mutation_genes < 0.0 or self.options.percentage_of_mutation_genes > 100.0:
+            self.add_message("Invalid percentage of mutation genes: {0} and number of mutation genes: {1}".format(str(self.options.percentage_of_mutation_genes, self.options.number_of_mutation_genes)))
             rslt &= False
         if self.options.max_attempt_no is None:
             self.add_message("Max Attempt No must not be None!")
             rslt &= False
         elif not isinstance(self.options.max_attempt_no, int):
             self.add_message("Max Attempt No must be type int!")
             rslt &= False
@@ -149,15 +164,15 @@
         if self.options.chromosome_mutation == definitions.CROSS_DIVERSITY:
             if self.options.cross_diversity_mutation_gene_selection is None:
                 self.add_message("Cross Diversity Mutation Gene Selection must not be None!")
                 rslt &= False
             elif not isinstance(self.options.cross_diversity_mutation_gene_selection, str):
                 self.add_message("Cross Diversity Mutation Gene Selection must be type str!")
                 rslt &= False
-            elif not self.validate_selection(self.options.cross_diversity_mutation_gene_selection, "Cross Diversity Mutation Gene Selection", self.options.number_of_mutation_genes, "Group Size for Cross Diversity Mutation Gene Selection must be below or equal than the number of mutation variables!"):
+            elif not self.validate_selection(self.options.cross_diversity_mutation_gene_selection, "Cross Diversity Mutation Gene Selection", self.options.number_of_mutation_genes, "Group Size for Cross Diversity Mutation Gene Selection must be below or equal than the number of mutation genes!"):
                 rslt &= False           
         if self.options.logging is None:
             self.add_message("Logging must not be None!")
             rslt &= False
         elif not isinstance(self.options.logging, bool):
             self.add_message("Logging must be type bool!")
             rslt &= False
```

### Comparing `gadapt-0.2.12/gadapt/variable_update/common_variable_updater.py` & `gadapt-0.2.13/gadapt/variable_update/common_variable_updater.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.12/gadapt.egg-info/SOURCES.txt` & `gadapt-0.2.13/gadapt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

