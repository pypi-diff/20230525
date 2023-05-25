# Comparing `tmp/immuneML-2.2.4.tar.gz` & `tmp/immuneML-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/immuneML-2.2.4.tar", last modified: Thu Mar 30 09:32:45 2023, max compression
+gzip compressed data, was "dist/immuneML-2.2.5.tar", last modified: Thu May 25 12:56:47 2023, max compression
```

## Comparing `immuneML-2.2.4.tar` & `immuneML-2.2.5.tar`

### file list

```diff
@@ -1,588 +1,596 @@
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.216868 immuneML-2.2.4/
--rw-r--r--   0 milenpa    (501) staff       (20)    34523 2020-11-01 17:12:10.000000 immuneML-2.2.4/LICENSE.md
--rw-r--r--   0 milenpa    (501) staff       (20)    11216 2023-03-30 09:32:45.216577 immuneML-2.2.4/PKG-INFO
--rw-r--r--   0 milenpa    (501) staff       (20)    10674 2023-03-30 09:17:22.000000 immuneML-2.2.4/README.md
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.913748 immuneML-2.2.4/immuneML/
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.917390 immuneML-2.2.4/immuneML/IO/
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/IO/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.921062 immuneML-2.2.4/immuneML/IO/dataset_export/
--rw-r--r--   0 milenpa    (501) staff       (20)     9778 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/IO/dataset_export/AIRRExporter.py
--rw-r--r--   0 milenpa    (501) staff       (20)      350 2022-02-11 22:47:04.000000 immuneML-2.2.4/immuneML/IO/dataset_export/DataExporter.py
--rw-r--r--   0 milenpa    (501) staff       (20)     5680 2022-02-11 22:47:04.000000 immuneML-2.2.4/immuneML/IO/dataset_export/ImmuneMLExporter.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/IO/dataset_export/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.936543 immuneML-2.2.4/immuneML/IO/dataset_import/
--rw-r--r--   0 milenpa    (501) staff       (20)    12857 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/IO/dataset_import/AIRRImport.py
--rw-r--r--   0 milenpa    (501) staff       (20)      247 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/IO/dataset_import/DataImport.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1688 2021-03-04 13:59:32.000000 immuneML-2.2.4/immuneML/IO/dataset_import/DatasetImportParams.py
--rw-r--r--   0 milenpa    (501) staff       (20)    10354 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/IO/dataset_import/GenericImport.py
--rw-r--r--   0 milenpa    (501) staff       (20)    10336 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/IO/dataset_import/IGoRImport.py
--rw-r--r--   0 milenpa    (501) staff       (20)    20610 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/IO/dataset_import/IReceptorImport.py
--rw-r--r--   0 milenpa    (501) staff       (20)     6620 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/IO/dataset_import/ImmuneMLImport.py
--rw-r--r--   0 milenpa    (501) staff       (20)    10716 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/IO/dataset_import/ImmunoSEQRearrangementImport.py
--rw-r--r--   0 milenpa    (501) staff       (20)    10246 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/IO/dataset_import/ImmunoSEQSampleImport.py
--rw-r--r--   0 milenpa    (501) staff       (20)    10565 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/IO/dataset_import/MiXCRImport.py
--rw-r--r--   0 milenpa    (501) staff       (20)     6456 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/IO/dataset_import/OLGAImport.py
--rw-r--r--   0 milenpa    (501) staff       (20)     5467 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/IO/dataset_import/RandomReceptorDatasetImport.py
--rw-r--r--   0 milenpa    (501) staff       (20)     4180 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/IO/dataset_import/RandomRepertoireDatasetImport.py
--rw-r--r--   0 milenpa    (501) staff       (20)     4542 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/IO/dataset_import/RandomSequenceDatasetImport.py
--rw-r--r--   0 milenpa    (501) staff       (20)    11644 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/IO/dataset_import/SingleLineReceptorImport.py
--rw-r--r--   0 milenpa    (501) staff       (20)    10653 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/IO/dataset_import/TenxGenomicsImport.py
--rw-r--r--   0 milenpa    (501) staff       (20)    12356 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/IO/dataset_import/VDJdbImport.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/IO/dataset_import/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.936898 immuneML-2.2.4/immuneML/IO/dataset_import/conversion/
--rw-r--r--   0 milenpa    (501) staff       (20)    14265 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/IO/dataset_import/conversion/imgt_adaptive_conversion.csv
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.941357 immuneML-2.2.4/immuneML/IO/ml_method/
--rw-r--r--   0 milenpa    (501) staff       (20)     3131 2023-03-30 09:08:07.000000 immuneML-2.2.4/immuneML/IO/ml_method/MLExporter.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2156 2023-03-30 09:08:07.000000 immuneML-2.2.4/immuneML/IO/ml_method/MLImport.py
--rw-r--r--   0 milenpa    (501) staff       (20)      959 2023-03-30 09:08:07.000000 immuneML-2.2.4/immuneML/IO/ml_method/MLMethodConfiguration.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1868 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/IO/ml_method/UtilIO.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/IO/ml_method/__init__.py
--rw-r--r--   0 milenpa    (501) staff       (20)       86 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.943699 immuneML-2.2.4/immuneML/analysis/
--rw-r--r--   0 milenpa    (501) staff       (20)       84 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/analysis/AxisType.py
--rw-r--r--   0 milenpa    (501) staff       (20)     5129 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/analysis/SequenceMatcher.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/analysis/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.947486 immuneML-2.2.4/immuneML/analysis/criteria_matches/
--rw-r--r--   0 milenpa    (501) staff       (20)       73 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/analysis/criteria_matches/BooleanType.py
--rw-r--r--   0 milenpa    (501) staff       (20)     5413 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/analysis/criteria_matches/CriteriaMatcher.py
--rw-r--r--   0 milenpa    (501) staff       (20)      977 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/analysis/criteria_matches/CriteriaTypeInstantiator.py
--rw-r--r--   0 milenpa    (501) staff       (20)       62 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/analysis/criteria_matches/DataType.py
--rw-r--r--   0 milenpa    (501) staff       (20)      163 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/analysis/criteria_matches/OperationType.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/analysis/criteria_matches/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.949912 immuneML-2.2.4/immuneML/analysis/data_manipulation/
--rw-r--r--   0 milenpa    (501) staff       (20)     1717 2023-03-27 12:19:55.000000 immuneML-2.2.4/immuneML/analysis/data_manipulation/DataReshaper.py
--rw-r--r--   0 milenpa    (501) staff       (20)      156 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/analysis/data_manipulation/NormalizationType.py
--rwxr-xr-x   0 milenpa    (501) staff       (20)       78 2021-01-29 20:00:50.000000 immuneML-2.2.4/immuneML/analysis/data_manipulation/ReductionMethod.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/analysis/data_manipulation/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.950878 immuneML-2.2.4/immuneML/analysis/entropy_calculations/
--rw-r--r--   0 milenpa    (501) staff       (20)      977 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/analysis/entropy_calculations/EntropyCalculator.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/analysis/entropy_calculations/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.952531 immuneML-2.2.4/immuneML/analysis/similarities/
--rw-r--r--   0 milenpa    (501) staff       (20)     1840 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/analysis/similarities/RepertoireSimilarityComputer.py
--rw-r--r--   0 milenpa    (501) staff       (20)      109 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/analysis/similarities/SimilarityMeasureType.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/analysis/similarities/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.953272 immuneML-2.2.4/immuneML/api/
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/api/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.954781 immuneML-2.2.4/immuneML/api/aggregated_runs/
--rw-r--r--   0 milenpa    (501) staff       (20)     9965 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/api/aggregated_runs/MultiDatasetBenchmarkTool.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/api/aggregated_runs/__init__.py
--rw-r--r--   0 milenpa    (501) staff       (20)     4069 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/api/api_encoding.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.962999 immuneML-2.2.4/immuneML/api/galaxy/
--rw-r--r--   0 milenpa    (501) staff       (20)     2107 2022-01-19 10:07:52.000000 immuneML-2.2.4/immuneML/api/galaxy/DataSimulationTool.py
--rw-r--r--   0 milenpa    (501) staff       (20)     4156 2022-11-28 13:16:24.000000 immuneML-2.2.4/immuneML/api/galaxy/DatasetGenerationTool.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2076 2022-11-28 13:16:24.000000 immuneML-2.2.4/immuneML/api/galaxy/GalaxyMLApplicationTool.py
--rw-r--r--   0 milenpa    (501) staff       (20)     5079 2022-01-19 10:07:52.000000 immuneML-2.2.4/immuneML/api/galaxy/GalaxySimulationTool.py
--rw-r--r--   0 milenpa    (501) staff       (20)      653 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/api/galaxy/GalaxyTool.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3494 2021-01-29 10:55:23.000000 immuneML-2.2.4/immuneML/api/galaxy/GalaxyTrainMLModel.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1058 2022-01-19 10:07:52.000000 immuneML-2.2.4/immuneML/api/galaxy/GalaxyYamlTool.py
--rw-r--r--   0 milenpa    (501) staff       (20)      638 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/api/galaxy/RepertoireClassificationTool.py
--rw-r--r--   0 milenpa    (501) staff       (20)     5259 2022-01-19 10:07:52.000000 immuneML-2.2.4/immuneML/api/galaxy/Util.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/api/galaxy/__init__.py
--rw-r--r--   0 milenpa    (501) staff       (20)     4140 2021-06-24 13:55:25.000000 immuneML-2.2.4/immuneML/api/galaxy/build_dataset_yaml.py
--rw-r--r--   0 milenpa    (501) staff       (20)    11894 2022-02-11 22:47:04.000000 immuneML-2.2.4/immuneML/api/galaxy/build_yaml_from_arguments.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.964748 immuneML-2.2.4/immuneML/app/
--rw-r--r--   0 milenpa    (501) staff       (20)     3698 2023-03-27 12:15:28.000000 immuneML-2.2.4/immuneML/app/ImmuneMLApp.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/app/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.967091 immuneML-2.2.4/immuneML/caching/
--rw-r--r--   0 milenpa    (501) staff       (20)     3765 2021-10-21 14:19:15.000000 immuneML-2.2.4/immuneML/caching/CacheHandler.py
--rw-r--r--   0 milenpa    (501) staff       (20)      107 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/caching/CacheObjectType.py
--rw-r--r--   0 milenpa    (501) staff       (20)       96 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/caching/CacheType.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/caching/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.892559 immuneML-2.2.4/immuneML/config/
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.894683 immuneML-2.2.4/immuneML/config/default_params/
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.976936 immuneML-2.2.4/immuneML/config/default_params/datasets/
--rw-r--r--   0 milenpa    (501) staff       (20)      739 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/config/default_params/datasets/airr_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      424 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/config/default_params/datasets/generic_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      739 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/config/default_params/datasets/i_receptor_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      608 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/config/default_params/datasets/igor_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)     1258 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/config/default_params/datasets/immuno_seq_rearrangement_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)     1150 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/config/default_params/datasets/immuno_seq_sample_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      743 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/config/default_params/datasets/mixcr_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      608 2023-03-27 12:15:28.000000 immuneML-2.2.4/immuneML/config/default_params/datasets/olga_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      170 2023-03-07 21:32:01.000000 immuneML-2.2.4/immuneML/config/default_params/datasets/random_receptor_dataset_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      723 2023-03-07 21:31:54.000000 immuneML-2.2.4/immuneML/config/default_params/datasets/random_repertoire_dataset_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)       93 2023-03-07 21:31:47.000000 immuneML-2.2.4/immuneML/config/default_params/datasets/random_sequence_dataset_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      824 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/config/default_params/datasets/tenx_genomics_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      636 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/config/default_params/datasets/vdjdb_params.yaml
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.986227 immuneML-2.2.4/immuneML/config/default_params/encodings/
--rw-r--r--   0 milenpa    (501) staff       (20)      101 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/config/default_params/encodings/atchley_kmer_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      128 2022-01-11 11:48:50.000000 immuneML-2.2.4/immuneML/config/default_params/encodings/comp_airr_distance_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      131 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/config/default_params/encodings/comp_airr_sequence_abundance_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)       90 2021-05-14 20:04:47.000000 immuneML-2.2.4/immuneML/config/default_params/encodings/distance_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      387 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/config/default_params/encodings/kmer_abundance_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      762 2021-02-25 10:05:14.000000 immuneML-2.2.4/immuneML/config/default_params/encodings/kmer_frequency_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      188 2022-02-11 22:47:04.000000 immuneML-2.2.4/immuneML/config/default_params/encodings/matched_receptors_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)       31 2022-02-11 22:47:04.000000 immuneML-2.2.4/immuneML/config/default_params/encodings/matched_regex_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)       95 2023-03-27 12:19:55.000000 immuneML-2.2.4/immuneML/config/default_params/encodings/matched_sequences_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      269 2021-03-04 22:07:02.000000 immuneML-2.2.4/immuneML/config/default_params/encodings/one_hot_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      119 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/config/default_params/encodings/sequence_abundance_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      258 2022-02-11 22:47:04.000000 immuneML-2.2.4/immuneML/config/default_params/encodings/word2_vec_params.yaml
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.992529 immuneML-2.2.4/immuneML/config/default_params/instructions/
--rw-r--r--   0 milenpa    (501) staff       (20)       22 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/config/default_params/instructions/exploratory_analysis_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)       64 2021-02-18 19:16:00.000000 immuneML-2.2.4/immuneML/config/default_params/instructions/export_parser_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)       23 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/config/default_params/instructions/ml_application_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)       22 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/config/default_params/instructions/simulation_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)       62 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/config/default_params/instructions/split_config_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)       30 2021-02-18 19:16:00.000000 immuneML-2.2.4/immuneML/config/default_params/instructions/subsampling_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      905 2021-06-24 13:55:25.000000 immuneML-2.2.4/immuneML/config/default_params/instructions/train_ml_model_params.yaml
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.996672 immuneML-2.2.4/immuneML/config/default_params/ml_methods/
--rw-r--r--   0 milenpa    (501) staff       (20)      196 2022-09-05 11:06:49.000000 immuneML-2.2.4/immuneML/config/default_params/ml_methods/atchley_kmer_mil_classifier_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      654 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/config/default_params/ml_methods/deep_rc_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      268 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/config/default_params/ml_methods/ml_method_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      307 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/config/default_params/ml_methods/receptor_cnn_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)       15 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/config/default_params/ml_methods/tcrdist_classifier_params.yaml
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.997450 immuneML-2.2.4/immuneML/config/default_params/motif_instantiation_strategy/
--rw-r--r--   0 milenpa    (501) staff       (20)      105 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/config/default_params/motif_instantiation_strategy/gapped_kmer_params.yaml
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.998230 immuneML-2.2.4/immuneML/config/default_params/preprocessing/
--rw-r--r--   0 milenpa    (501) staff       (20)       82 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/config/default_params/preprocessing/duplicate_sequence_filter_params.yaml
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.009448 immuneML-2.2.4/immuneML/config/default_params/reports/
--rw-r--r--   0 milenpa    (501) staff       (20)      131 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/config/default_params/reports/coefficients_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      125 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/config/default_params/reports/cv_feature_performance_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      340 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/config/default_params/reports/cytoscape_network_exporter_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)       26 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/config/default_params/reports/deep_rc_motif_discovery_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)       17 2021-01-29 10:55:23.000000 immuneML-2.2.4/immuneML/config/default_params/reports/design_matrix_exporter_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)       69 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/config/default_params/reports/feature_comparison_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      101 2021-03-12 15:52:25.000000 immuneML-2.2.4/immuneML/config/default_params/reports/feature_value_barplot_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)       73 2022-01-11 11:48:50.000000 immuneML-2.2.4/immuneML/config/default_params/reports/ml_settings_performance_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)       38 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/config/default_params/reports/motif_seed_recovery_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)       17 2021-02-18 19:16:00.000000 immuneML-2.2.4/immuneML/config/default_params/reports/receptor_dataset_overview_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)       28 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/config/default_params/reports/recovered_significant_features_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)       51 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/config/default_params/reports/reference_sequence_overlap_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)       16 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/config/default_params/reports/significant_features_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)       60 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/config/default_params/reports/tcrdist_motif_discovery_params.yaml
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.010720 immuneML-2.2.4/immuneML/config/default_params/signal_implanting_strategy/
--rw-r--r--   0 milenpa    (501) staff       (20)       97 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/config/default_params/signal_implanting_strategy/full_sequence_implanting_params.yaml
--rw-r--r--   0 milenpa    (501) staff       (20)      213 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/config/default_params/signal_implanting_strategy/healthy_sequence_implanting_params.yaml
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.012915 immuneML-2.2.4/immuneML/data_model/
--rw-r--r--   0 milenpa    (501) staff       (20)      133 2021-06-13 10:10:40.000000 immuneML-2.2.4/immuneML/data_model/DatasetItem.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/data_model/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.015035 immuneML-2.2.4/immuneML/data_model/cell/
--rw-r--r--   0 milenpa    (501) staff       (20)      400 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/data_model/cell/Cell.py
--rw-r--r--   0 milenpa    (501) staff       (20)      711 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/data_model/cell/CellList.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/data_model/cell/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.018458 immuneML-2.2.4/immuneML/data_model/dataset/
--rw-r--r--   0 milenpa    (501) staff       (20)     1191 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/data_model/dataset/Dataset.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3792 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/data_model/dataset/ElementDataset.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2813 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/data_model/dataset/ReceptorDataset.py
--rw-r--r--   0 milenpa    (501) staff       (20)     8180 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/data_model/dataset/RepertoireDataset.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2870 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/data_model/dataset/SequenceDataset.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/data_model/dataset/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.019847 immuneML-2.2.4/immuneML/data_model/encoded_data/
--rw-r--r--   0 milenpa    (501) staff       (20)     2372 2023-03-27 12:15:28.000000 immuneML-2.2.4/immuneML/data_model/encoded_data/EncodedData.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/data_model/encoded_data/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.026194 immuneML-2.2.4/immuneML/data_model/receptor/
--rw-r--r--   0 milenpa    (501) staff       (20)     1946 2023-03-30 09:08:07.000000 immuneML-2.2.4/immuneML/data_model/receptor/BCKReceptor.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1956 2023-03-30 09:08:07.000000 immuneML-2.2.4/immuneML/data_model/receptor/BCReceptor.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1249 2021-03-07 11:32:41.000000 immuneML-2.2.4/immuneML/data_model/receptor/ChainPair.py
--rw-r--r--   0 milenpa    (501) staff       (20)     5316 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/data_model/receptor/ElementGenerator.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1461 2023-03-30 09:08:07.000000 immuneML-2.2.4/immuneML/data_model/receptor/Receptor.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2605 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/data_model/receptor/ReceptorBuilder.py
--rw-r--r--   0 milenpa    (501) staff       (20)      309 2021-01-25 16:31:21.000000 immuneML-2.2.4/immuneML/data_model/receptor/RegionType.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1969 2023-03-30 09:08:07.000000 immuneML-2.2.4/immuneML/data_model/receptor/TCABReceptor.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1980 2023-03-30 09:08:07.000000 immuneML-2.2.4/immuneML/data_model/receptor/TCGDReceptor.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/data_model/receptor/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.029456 immuneML-2.2.4/immuneML/data_model/receptor/receptor_sequence/
--rw-r--r--   0 milenpa    (501) staff       (20)      957 2022-02-02 10:06:22.000000 immuneML-2.2.4/immuneML/data_model/receptor/receptor_sequence/Chain.py
--rw-r--r--   0 milenpa    (501) staff       (20)     4091 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/data_model/receptor/receptor_sequence/ReceptorSequence.py
--rw-r--r--   0 milenpa    (501) staff       (20)      793 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/data_model/receptor/receptor_sequence/ReceptorSequenceList.py
--rw-r--r--   0 milenpa    (501) staff       (20)      548 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/data_model/receptor/receptor_sequence/SequenceAnnotation.py
--rw-r--r--   0 milenpa    (501) staff       (20)      153 2021-06-24 13:55:25.000000 immuneML-2.2.4/immuneML/data_model/receptor/receptor_sequence/SequenceFrameType.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2605 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/data_model/receptor/receptor_sequence/SequenceMetadata.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/data_model/receptor/receptor_sequence/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.030383 immuneML-2.2.4/immuneML/data_model/repertoire/
--rw-r--r--   0 milenpa    (501) staff       (20)    19042 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/data_model/repertoire/Repertoire.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/data_model/repertoire/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.030828 immuneML-2.2.4/immuneML/dev_util/
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/dev_util/__init__.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1778 2021-02-18 19:16:00.000000 immuneML-2.2.4/immuneML/dev_util/util.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.035027 immuneML-2.2.4/immuneML/dsl/
--rw-r--r--   0 milenpa    (501) staff       (20)     1892 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/dsl/DefaultParamsLoader.py
--rw-r--r--   0 milenpa    (501) staff       (20)     7460 2022-11-28 13:16:24.000000 immuneML-2.2.4/immuneML/dsl/ImmuneMLParser.py
--rw-r--r--   0 milenpa    (501) staff       (20)     6393 2021-02-18 19:16:00.000000 immuneML-2.2.4/immuneML/dsl/InstructionParser.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3883 2021-02-18 19:16:00.000000 immuneML-2.2.4/immuneML/dsl/ObjectParser.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1093 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/dsl/OutputParser.py
--rw-r--r--   0 milenpa    (501) staff       (20)      139 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/dsl/Parser.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/dsl/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.041416 immuneML-2.2.4/immuneML/dsl/definition_parsers/
--rw-r--r--   0 milenpa    (501) staff       (20)     7909 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/dsl/definition_parsers/DefinitionParser.py
--rw-r--r--   0 milenpa    (501) staff       (20)      523 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/dsl/definition_parsers/DefinitionParserOutput.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1852 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/dsl/definition_parsers/EncodingParser.py
--rw-r--r--   0 milenpa    (501) staff       (20)     4497 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/dsl/definition_parsers/MLParser.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2469 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/dsl/definition_parsers/MotifParser.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1377 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/dsl/definition_parsers/PreprocessingParser.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1202 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/dsl/definition_parsers/ReportParser.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3180 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/dsl/definition_parsers/SignalParser.py
--rw-r--r--   0 milenpa    (501) staff       (20)     4429 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/dsl/definition_parsers/SimulationParser.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/dsl/definition_parsers/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.043138 immuneML-2.2.4/immuneML/dsl/import_parsers/
--rw-r--r--   0 milenpa    (501) staff       (20)     4589 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/dsl/import_parsers/ImportParser.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/dsl/import_parsers/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.048701 immuneML-2.2.4/immuneML/dsl/instruction_parsers/
--rw-r--r--   0 milenpa    (501) staff       (20)     3560 2022-02-11 22:47:04.000000 immuneML-2.2.4/immuneML/dsl/instruction_parsers/DatasetExportParser.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3829 2023-03-27 12:15:28.000000 immuneML-2.2.4/immuneML/dsl/instruction_parsers/ExploratoryAnalysisParser.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2825 2022-02-11 22:47:04.000000 immuneML-2.2.4/immuneML/dsl/instruction_parsers/LabelHelper.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2703 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/dsl/instruction_parsers/MLApplicationParser.py
--rw-r--r--   0 milenpa    (501) staff       (20)     4484 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/dsl/instruction_parsers/SimulationParser.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2323 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/dsl/instruction_parsers/SubsamplingParser.py
--rw-r--r--   0 milenpa    (501) staff       (20)    13497 2023-03-27 12:19:55.000000 immuneML-2.2.4/immuneML/dsl/instruction_parsers/TrainMLModelParser.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/dsl/instruction_parsers/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.050312 immuneML-2.2.4/immuneML/dsl/semantic_model/
--rw-r--r--   0 milenpa    (501) staff       (20)       72 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/dsl/semantic_model/MLResult.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1882 2022-11-28 13:16:24.000000 immuneML-2.2.4/immuneML/dsl/semantic_model/SemanticModel.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/dsl/semantic_model/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.052897 immuneML-2.2.4/immuneML/dsl/symbol_table/
--rw-r--r--   0 milenpa    (501) staff       (20)     2448 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/dsl/symbol_table/SymbolTable.py
--rw-r--r--   0 milenpa    (501) staff       (20)      298 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/dsl/symbol_table/SymbolTableEntry.py
--rw-r--r--   0 milenpa    (501) staff       (20)      220 2023-03-27 12:15:28.000000 immuneML-2.2.4/immuneML/dsl/symbol_table/SymbolType.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/dsl/symbol_table/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.054649 immuneML-2.2.4/immuneML/encodings/
--rw-r--r--   0 milenpa    (501) staff       (20)     2006 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/encodings/DatasetEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)      353 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/encodings/EncoderParams.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/encodings/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.058314 immuneML-2.2.4/immuneML/encodings/abundance_encoding/
--rw-r--r--   0 milenpa    (501) staff       (20)     6212 2023-03-27 12:15:28.000000 immuneML-2.2.4/immuneML/encodings/abundance_encoding/AbundanceEncoderHelper.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1763 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/encodings/abundance_encoding/CompAIRRBatchIterator.py
--rw-r--r--   0 milenpa    (501) staff       (20)    19371 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/encodings/abundance_encoding/CompAIRRSequenceAbundanceEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)    13959 2023-03-27 12:15:28.000000 immuneML-2.2.4/immuneML/encodings/abundance_encoding/KmerAbundanceEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)    11123 2023-03-27 12:15:28.000000 immuneML-2.2.4/immuneML/encodings/abundance_encoding/SequenceAbundanceEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/encodings/abundance_encoding/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.060379 immuneML-2.2.4/immuneML/encodings/atchley_kmer_encoding/
--rw-r--r--   0 milenpa    (501) staff       (20)    10094 2021-06-05 21:38:55.000000 immuneML-2.2.4/immuneML/encodings/atchley_kmer_encoding/AtchleyKmerEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)      162 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/encodings/atchley_kmer_encoding/RelativeAbundanceType.py
--rw-r--r--   0 milenpa    (501) staff       (20)     5766 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/encodings/atchley_kmer_encoding/Util.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/encodings/atchley_kmer_encoding/__init__.py
--rw-r--r--   0 milenpa    (501) staff       (20)      751 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/encodings/atchley_kmer_encoding/atchley_factors.csv
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.061486 immuneML-2.2.4/immuneML/encodings/deeprc/
--rw-r--r--   0 milenpa    (501) staff       (20)     4269 2021-03-04 20:37:49.000000 immuneML-2.2.4/immuneML/encodings/deeprc/DeepRCEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/encodings/deeprc/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.063930 immuneML-2.2.4/immuneML/encodings/distance_encoding/
--rw-r--r--   0 milenpa    (501) staff       (20)    12084 2022-01-11 11:48:50.000000 immuneML-2.2.4/immuneML/encodings/distance_encoding/CompAIRRDistanceEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     7335 2021-08-03 14:43:33.000000 immuneML-2.2.4/immuneML/encodings/distance_encoding/DistanceEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)      116 2022-01-11 11:48:50.000000 immuneML-2.2.4/immuneML/encodings/distance_encoding/DistanceMetricType.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3614 2023-02-07 13:47:33.000000 immuneML-2.2.4/immuneML/encodings/distance_encoding/TCRdistEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/encodings/distance_encoding/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.065428 immuneML-2.2.4/immuneML/encodings/evenness_profile/
--rw-r--r--   0 milenpa    (501) staff       (20)     5330 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/encodings/evenness_profile/EvennessProfileEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3398 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/encodings/evenness_profile/EvennessProfileRepertoireEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/encodings/evenness_profile/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.068964 immuneML-2.2.4/immuneML/encodings/kmer_frequency/
--rw-r--r--   0 milenpa    (501) staff       (20)     2222 2021-06-24 13:55:25.000000 immuneML-2.2.4/immuneML/encodings/kmer_frequency/KmerFreqReceptorEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2994 2023-03-23 12:33:14.000000 immuneML-2.2.4/immuneML/encodings/kmer_frequency/KmerFreqRepertoireEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1633 2021-01-29 10:55:23.000000 immuneML-2.2.4/immuneML/encodings/kmer_frequency/KmerFreqSequenceEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)    15879 2023-03-27 12:19:55.000000 immuneML-2.2.4/immuneML/encodings/kmer_frequency/KmerFrequencyEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/encodings/kmer_frequency/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.073542 immuneML-2.2.4/immuneML/encodings/kmer_frequency/sequence_encoding/
--rw-r--r--   0 milenpa    (501) staff       (20)     2015 2022-02-11 22:47:04.000000 immuneML-2.2.4/immuneML/encodings/kmer_frequency/sequence_encoding/GappedKmerSequenceEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2227 2022-02-11 22:47:04.000000 immuneML-2.2.4/immuneML/encodings/kmer_frequency/sequence_encoding/IMGTGappedKmerEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1693 2022-02-11 22:47:04.000000 immuneML-2.2.4/immuneML/encodings/kmer_frequency/sequence_encoding/IMGTKmerSequenceEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1864 2022-02-11 22:47:04.000000 immuneML-2.2.4/immuneML/encodings/kmer_frequency/sequence_encoding/IdentitySequenceEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1367 2022-11-08 20:23:03.000000 immuneML-2.2.4/immuneML/encodings/kmer_frequency/sequence_encoding/KmerSequenceEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)      459 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/encodings/kmer_frequency/sequence_encoding/SequenceEncodingStrategy.py
--rw-r--r--   0 milenpa    (501) staff       (20)      289 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/encodings/kmer_frequency/sequence_encoding/SequenceEncodingType.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/encodings/kmer_frequency/sequence_encoding/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.076009 immuneML-2.2.4/immuneML/encodings/onehot/
--rw-r--r--   0 milenpa    (501) staff       (20)    11023 2023-03-27 12:14:54.000000 immuneML-2.2.4/immuneML/encodings/onehot/OneHotEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3948 2021-06-24 13:55:25.000000 immuneML-2.2.4/immuneML/encodings/onehot/OneHotReceptorEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     5208 2021-03-04 22:07:02.000000 immuneML-2.2.4/immuneML/encodings/onehot/OneHotRepertoireEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3256 2021-03-04 22:07:02.000000 immuneML-2.2.4/immuneML/encodings/onehot/OneHotSequenceEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/encodings/onehot/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.076682 immuneML-2.2.4/immuneML/encodings/preprocessing/
--rw-r--r--   0 milenpa    (501) staff       (20)     2922 2023-03-27 12:19:55.000000 immuneML-2.2.4/immuneML/encodings/preprocessing/FeatureScaler.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/encodings/preprocessing/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.080145 immuneML-2.2.4/immuneML/encodings/reference_encoding/
--rw-r--r--   0 milenpa    (501) staff       (20)    15402 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/encodings/reference_encoding/MatchedReceptorsEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2985 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/encodings/reference_encoding/MatchedReferenceUtil.py
--rw-r--r--   0 milenpa    (501) staff       (20)     8410 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/encodings/reference_encoding/MatchedRegexEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     5366 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/encodings/reference_encoding/MatchedRegexRepertoireEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)    10906 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/encodings/reference_encoding/MatchedSequencesEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)      124 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/encodings/reference_encoding/SequenceMatchingSummaryType.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/encodings/reference_encoding/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.081988 immuneML-2.2.4/immuneML/encodings/word2vec/
--rw-r--r--   0 milenpa    (501) staff       (20)     1492 2022-02-11 22:47:04.000000 immuneML-2.2.4/immuneML/encodings/word2vec/W2VRepertoireEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1228 2022-02-11 22:47:04.000000 immuneML-2.2.4/immuneML/encodings/word2vec/W2VSequenceEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)    11780 2023-03-27 12:14:54.000000 immuneML-2.2.4/immuneML/encodings/word2vec/Word2VecEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/encodings/word2vec/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.084439 immuneML-2.2.4/immuneML/encodings/word2vec/model_creator/
--rw-r--r--   0 milenpa    (501) staff       (20)     1367 2022-02-11 22:47:04.000000 immuneML-2.2.4/immuneML/encodings/word2vec/model_creator/KmerPairModelCreator.py
--rw-r--r--   0 milenpa    (501) staff       (20)      622 2022-02-11 22:47:04.000000 immuneML-2.2.4/immuneML/encodings/word2vec/model_creator/ModelCreatorStrategy.py
--rw-r--r--   0 milenpa    (501) staff       (20)       83 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/encodings/word2vec/model_creator/ModelType.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2212 2022-02-11 22:47:04.000000 immuneML-2.2.4/immuneML/encodings/word2vec/model_creator/SequenceModelCreator.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/encodings/word2vec/model_creator/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.089036 immuneML-2.2.4/immuneML/environment/
--rw-r--r--   0 milenpa    (501) staff       (20)      385 2023-03-30 09:18:47.000000 immuneML-2.2.4/immuneML/environment/Constants.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3330 2022-11-28 13:16:24.000000 immuneML-2.2.4/immuneML/environment/EnvironmentSettings.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1907 2023-03-27 12:19:55.000000 immuneML-2.2.4/immuneML/environment/Label.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3344 2023-03-27 12:19:55.000000 immuneML-2.2.4/immuneML/environment/LabelConfiguration.py
--rw-r--r--   0 milenpa    (501) staff       (20)       89 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/environment/LabelType.py
--rw-r--r--   0 milenpa    (501) staff       (20)      111 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/environment/SequenceType.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/environment/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.090489 immuneML-2.2.4/immuneML/hyperparameter_optimization/
--rw-r--r--   0 milenpa    (501) staff       (20)     1042 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/hyperparameter_optimization/HPSetting.py
--rw-r--r--   0 milenpa    (501) staff       (20)      688 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/hyperparameter_optimization/HPSettingResult.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/hyperparameter_optimization/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.093514 immuneML-2.2.4/immuneML/hyperparameter_optimization/config/
--rw-r--r--   0 milenpa    (501) staff       (20)      125 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/hyperparameter_optimization/config/LeaveOneOutConfig.py
--rw-r--r--   0 milenpa    (501) staff       (20)      171 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/hyperparameter_optimization/config/ManualSplitConfig.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3527 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/hyperparameter_optimization/config/ReportConfig.py
--rw-r--r--   0 milenpa    (501) staff       (20)     7724 2023-03-27 12:15:28.000000 immuneML-2.2.4/immuneML/hyperparameter_optimization/config/SplitConfig.py
--rw-r--r--   0 milenpa    (501) staff       (20)      170 2021-03-04 13:59:32.000000 immuneML-2.2.4/immuneML/hyperparameter_optimization/config/SplitType.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/hyperparameter_optimization/config/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.095889 immuneML-2.2.4/immuneML/hyperparameter_optimization/core/
--rw-r--r--   0 milenpa    (501) staff       (20)     5957 2022-11-28 13:16:24.000000 immuneML-2.2.4/immuneML/hyperparameter_optimization/core/HPAssessment.py
--rw-r--r--   0 milenpa    (501) staff       (20)     4756 2022-11-28 13:16:24.000000 immuneML-2.2.4/immuneML/hyperparameter_optimization/core/HPSelection.py
--rw-r--r--   0 milenpa    (501) staff       (20)     7882 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/hyperparameter_optimization/core/HPUtil.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/hyperparameter_optimization/core/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.099612 immuneML-2.2.4/immuneML/hyperparameter_optimization/states/
--rw-r--r--   0 milenpa    (501) staff       (20)      797 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/hyperparameter_optimization/states/HPAssessmentState.py
--rw-r--r--   0 milenpa    (501) staff       (20)      970 2021-11-07 11:51:14.000000 immuneML-2.2.4/immuneML/hyperparameter_optimization/states/HPItem.py
--rw-r--r--   0 milenpa    (501) staff       (20)      478 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/hyperparameter_optimization/states/HPLabelState.py
--rw-r--r--   0 milenpa    (501) staff       (20)      713 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/hyperparameter_optimization/states/HPSelectionState.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1507 2022-01-11 11:48:50.000000 immuneML-2.2.4/immuneML/hyperparameter_optimization/states/TrainMLModelState.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/hyperparameter_optimization/states/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.101403 immuneML-2.2.4/immuneML/hyperparameter_optimization/strategy/
--rw-r--r--   0 milenpa    (501) staff       (20)     2328 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/hyperparameter_optimization/strategy/GridSearch.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1598 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/hyperparameter_optimization/strategy/HPOptimizationStrategy.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/hyperparameter_optimization/strategy/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.110475 immuneML-2.2.4/immuneML/ml_methods/
--rw-r--r--   0 milenpa    (501) staff       (20)    10971 2023-03-27 12:19:55.000000 immuneML-2.2.4/immuneML/ml_methods/AtchleyKmerMILClassifier.py
--rw-r--r--   0 milenpa    (501) staff       (20)    21752 2023-03-30 09:17:22.000000 immuneML-2.2.4/immuneML/ml_methods/DeepRC.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3753 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/ml_methods/KNN.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3143 2021-10-22 09:13:56.000000 immuneML-2.2.4/immuneML/ml_methods/LogisticRegression.py
--rw-r--r--   0 milenpa    (501) staff       (20)    15572 2023-03-30 09:08:07.000000 immuneML-2.2.4/immuneML/ml_methods/MLMethod.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3105 2023-03-30 09:17:22.000000 immuneML-2.2.4/immuneML/ml_methods/PrecomputedKNN.py
--rw-r--r--   0 milenpa    (501) staff       (20)    20861 2023-03-27 12:19:55.000000 immuneML-2.2.4/immuneML/ml_methods/ProbabilisticBinaryClassifier.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3046 2021-02-18 19:16:00.000000 immuneML-2.2.4/immuneML/ml_methods/RandomForestClassifier.py
--rw-r--r--   0 milenpa    (501) staff       (20)    17041 2023-03-27 12:19:55.000000 immuneML-2.2.4/immuneML/ml_methods/ReceptorCNN.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2593 2022-01-11 11:48:50.000000 immuneML-2.2.4/immuneML/ml_methods/SVC.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2745 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/ml_methods/SVM.py
--rw-r--r--   0 milenpa    (501) staff       (20)    13708 2023-03-27 12:19:55.000000 immuneML-2.2.4/immuneML/ml_methods/SklearnMethod.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2896 2022-01-11 11:48:50.000000 immuneML-2.2.4/immuneML/ml_methods/TCRdistClassifier.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/ml_methods/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.112035 immuneML-2.2.4/immuneML/ml_methods/pytorch_implementations/
--rw-r--r--   0 milenpa    (501) staff       (20)      531 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/ml_methods/pytorch_implementations/PyTorchLogisticRegression.py
--rw-r--r--   0 milenpa    (501) staff       (20)     6046 2021-03-04 13:59:32.000000 immuneML-2.2.4/immuneML/ml_methods/pytorch_implementations/PyTorchReceptorCNN.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/ml_methods/pytorch_implementations/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.113088 immuneML-2.2.4/immuneML/ml_methods/util/
--rw-r--r--   0 milenpa    (501) staff       (20)     4543 2023-03-30 09:07:22.000000 immuneML-2.2.4/immuneML/ml_methods/util/Util.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/ml_methods/util/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.114034 immuneML-2.2.4/immuneML/ml_metrics/
--rw-r--r--   0 milenpa    (501) staff       (20)     1132 2023-03-27 12:19:55.000000 immuneML-2.2.4/immuneML/ml_metrics/Metric.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/ml_metrics/__init__.py
--rw-r--r--   0 milenpa    (501) staff       (20)      925 2022-11-28 13:16:24.000000 immuneML-2.2.4/immuneML/ml_metrics/ml_metrics.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.116423 immuneML-2.2.4/immuneML/pairwise_repertoire_comparison/
--rw-r--r--   0 milenpa    (501) staff       (20)     8646 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/pairwise_repertoire_comparison/ComparisonData.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2509 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/pairwise_repertoire_comparison/ComparisonDataBatch.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3436 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/pairwise_repertoire_comparison/PairwiseRepertoireComparison.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/pairwise_repertoire_comparison/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.117772 immuneML-2.2.4/immuneML/preprocessing/
--rw-r--r--   0 milenpa    (501) staff       (20)     1252 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/preprocessing/Preprocessor.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3256 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/preprocessing/SubjectRepertoireCollector.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/preprocessing/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.121651 immuneML-2.2.4/immuneML/preprocessing/filters/
--rw-r--r--   0 milenpa    (501) staff       (20)     2304 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/preprocessing/filters/ChainRepertoireFilter.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2695 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/preprocessing/filters/ClonesPerRepertoireFilter.py
--rw-r--r--   0 milenpa    (501) staff       (20)      166 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/preprocessing/filters/CountAggregationFunction.py
--rw-r--r--   0 milenpa    (501) staff       (20)     4005 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/preprocessing/filters/CountPerSequenceFilter.py
--rw-r--r--   0 milenpa    (501) staff       (20)     8626 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/preprocessing/filters/DuplicateSequenceFilter.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1430 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/preprocessing/filters/Filter.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2992 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/preprocessing/filters/MetadataRepertoireFilter.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/preprocessing/filters/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.123660 immuneML-2.2.4/immuneML/presentation/
--rw-r--r--   0 milenpa    (501) staff       (20)      170 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/presentation/InstructionPresentation.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2353 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/presentation/PresentationFactory.py
--rw-r--r--   0 milenpa    (501) staff       (20)       74 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/presentation/PresentationFormat.py
--rw-r--r--   0 milenpa    (501) staff       (20)      456 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/presentation/TemplateParser.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/presentation/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.128627 immuneML-2.2.4/immuneML/presentation/html/
--rw-r--r--   0 milenpa    (501) staff       (20)     3281 2021-05-14 20:04:47.000000 immuneML-2.2.4/immuneML/presentation/html/DatasetExportHTMLBuilder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     4562 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/presentation/html/ExploratoryAnalysisHTMLBuilder.py
--rw-r--r--   0 milenpa    (501) staff       (20)    21349 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/presentation/html/HPHTMLBuilder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3418 2021-06-23 22:15:10.000000 immuneML-2.2.4/immuneML/presentation/html/HTMLBuilder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2192 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/presentation/html/MLApplicationHTMLBuilder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1651 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/presentation/html/MultiDatasetBenchmarkHTMLBuilder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2985 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/presentation/html/SimulationHTMLBuilder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2879 2021-01-29 10:55:23.000000 immuneML-2.2.4/immuneML/presentation/html/SubsamplingHTMLBuilder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     4783 2021-02-18 19:16:00.000000 immuneML-2.2.4/immuneML/presentation/html/Util.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/presentation/html/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.134411 immuneML-2.2.4/immuneML/presentation/html/templates/
--rw-r--r--   0 milenpa    (501) staff       (20)     7651 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/presentation/html/templates/AssessmentSplitDetails.html
--rw-r--r--   0 milenpa    (501) staff       (20)     2940 2021-05-14 20:04:47.000000 immuneML-2.2.4/immuneML/presentation/html/templates/DatasetExport.html
--rw-r--r--   0 milenpa    (501) staff       (20)     6023 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/presentation/html/templates/ExploratoryAnalysis.html
--rw-r--r--   0 milenpa    (501) staff       (20)     6961 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/presentation/html/templates/HPOptimization.html
--rw-r--r--   0 milenpa    (501) staff       (20)     2222 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/presentation/html/templates/MLApplication.html
--rw-r--r--   0 milenpa    (501) staff       (20)     2614 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/presentation/html/templates/MLTraining.html
--rw-r--r--   0 milenpa    (501) staff       (20)     1799 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/presentation/html/templates/MultiDatasetBenchmark.html
--rw-r--r--   0 milenpa    (501) staff       (20)     2889 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/presentation/html/templates/Reports.html
--rw-r--r--   0 milenpa    (501) staff       (20)     9566 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/presentation/html/templates/SelectionDetails.html
--rw-r--r--   0 milenpa    (501) staff       (20)     4760 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/presentation/html/templates/Simulation.html
--rw-r--r--   0 milenpa    (501) staff       (20)     3078 2021-01-29 10:55:23.000000 immuneML-2.2.4/immuneML/presentation/html/templates/Subsampling.html
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.134988 immuneML-2.2.4/immuneML/presentation/html/templates/css/
--rw-r--r--   0 milenpa    (501) staff       (20)     2465 2021-02-18 19:16:00.000000 immuneML-2.2.4/immuneML/presentation/html/templates/css/custom.css
--rw-r--r--   0 milenpa    (501) staff       (20)      705 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/presentation/html/templates/index.html
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.138625 immuneML-2.2.4/immuneML/reports/
--rw-r--r--   0 milenpa    (501) staff       (20)     1824 2021-03-07 11:32:41.000000 immuneML-2.2.4/immuneML/reports/PlotlyUtil.py
--rw-r--r--   0 milenpa    (501) staff       (20)     6989 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/reports/Report.py
--rw-r--r--   0 milenpa    (501) staff       (20)      201 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/reports/ReportOutput.py
--rw-r--r--   0 milenpa    (501) staff       (20)      480 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/reports/ReportResult.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2847 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/reports/ReportUtil.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/reports/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.145066 immuneML-2.2.4/immuneML/reports/data_reports/
--rw-r--r--   0 milenpa    (501) staff       (20)     8755 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/reports/data_reports/CytoscapeNetworkExporter.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2473 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/reports/data_reports/DataReport.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3510 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/reports/data_reports/GLIPH2Exporter.py
--rw-r--r--   0 milenpa    (501) staff       (20)     4131 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/reports/data_reports/ReceptorDatasetOverview.py
--rw-r--r--   0 milenpa    (501) staff       (20)    12600 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/reports/data_reports/RecoveredSignificantFeatures.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3206 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/reports/data_reports/SequenceLengthDistribution.py
--rw-r--r--   0 milenpa    (501) staff       (20)     6358 2023-03-27 12:19:55.000000 immuneML-2.2.4/immuneML/reports/data_reports/SequencesWithSignificantKmers.py
--rw-r--r--   0 milenpa    (501) staff       (20)    12893 2023-03-27 12:19:55.000000 immuneML-2.2.4/immuneML/reports/data_reports/SignificantFeatures.py
--rw-r--r--   0 milenpa    (501) staff       (20)     8820 2022-09-19 11:30:27.000000 immuneML-2.2.4/immuneML/reports/data_reports/SignificantKmerPositions.py
--rw-r--r--   0 milenpa    (501) staff       (20)     4514 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/reports/data_reports/SimpleDatasetOverview.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/reports/data_reports/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.150119 immuneML-2.2.4/immuneML/reports/encoding_reports/
--rw-r--r--   0 milenpa    (501) staff       (20)     5814 2023-03-30 09:17:22.000000 immuneML-2.2.4/immuneML/reports/encoding_reports/DesignMatrixExporter.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2476 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/reports/encoding_reports/EncodingReport.py
--rw-r--r--   0 milenpa    (501) staff       (20)    11835 2023-03-27 12:19:55.000000 immuneML-2.2.4/immuneML/reports/encoding_reports/FeatureComparison.py
--rw-r--r--   0 milenpa    (501) staff       (20)     6182 2022-11-28 13:16:24.000000 immuneML-2.2.4/immuneML/reports/encoding_reports/FeatureDistribution.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3190 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/reports/encoding_reports/FeatureReport.py
--rw-r--r--   0 milenpa    (501) staff       (20)     4716 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/reports/encoding_reports/FeatureValueBarplot.py
--rw-r--r--   0 milenpa    (501) staff       (20)    12119 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/reports/encoding_reports/Matches.py
--rw-r--r--   0 milenpa    (501) staff       (20)     4148 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/reports/encoding_reports/RelevantSequenceExporter.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/reports/encoding_reports/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.159465 immuneML-2.2.4/immuneML/reports/ml_reports/
--rw-r--r--   0 milenpa    (501) staff       (20)      154 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/reports/ml_reports/CoefficientPlottingSetting.py
--rw-r--r--   0 milenpa    (501) staff       (20)      825 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/reports/ml_reports/CoefficientPlottingSettingList.py
--rw-r--r--   0 milenpa    (501) staff       (20)    10217 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/reports/ml_reports/Coefficients.py
--rw-r--r--   0 milenpa    (501) staff       (20)     6006 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/reports/ml_reports/ConfounderAnalysis.py
--rw-r--r--   0 milenpa    (501) staff       (20)    15785 2023-03-30 09:17:22.000000 immuneML-2.2.4/immuneML/reports/ml_reports/DeepRCMotifDiscovery.py
--rw-r--r--   0 milenpa    (501) staff       (20)     6221 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/reports/ml_reports/KernelSequenceLogo.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2852 2023-03-27 12:14:54.000000 immuneML-2.2.4/immuneML/reports/ml_reports/MLReport.py
--rw-r--r--   0 milenpa    (501) staff       (20)    14405 2023-03-27 12:19:55.000000 immuneML-2.2.4/immuneML/reports/ml_reports/MotifSeedRecovery.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3686 2023-03-27 12:19:55.000000 immuneML-2.2.4/immuneML/reports/ml_reports/ROCCurve.py
--rw-r--r--   0 milenpa    (501) staff       (20)     4445 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/reports/ml_reports/SequenceAssociationLikelihood.py
--rw-r--r--   0 milenpa    (501) staff       (20)     9321 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/reports/ml_reports/TCRdistMotifDiscovery.py
--rw-r--r--   0 milenpa    (501) staff       (20)     8890 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/reports/ml_reports/TrainingPerformance.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/reports/ml_reports/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.161697 immuneML-2.2.4/immuneML/reports/multi_dataset_reports/
--rw-r--r--   0 milenpa    (501) staff       (20)     4489 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/reports/multi_dataset_reports/DiseaseAssociatedSequenceOverlap.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2012 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/reports/multi_dataset_reports/MultiDatasetReport.py
--rw-r--r--   0 milenpa    (501) staff       (20)     7520 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/reports/multi_dataset_reports/PerformanceOverview.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/reports/multi_dataset_reports/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.166328 immuneML-2.2.4/immuneML/reports/train_ml_model_reports/
--rw-r--r--   0 milenpa    (501) staff       (20)     7897 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/reports/train_ml_model_reports/CVFeaturePerformance.py
--rw-r--r--   0 milenpa    (501) staff       (20)     7244 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/reports/train_ml_model_reports/DiseaseAssociatedSequenceCVOverlap.py
--rw-r--r--   0 milenpa    (501) staff       (20)     7942 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/reports/train_ml_model_reports/MLSettingsPerformance.py
--rw-r--r--   0 milenpa    (501) staff       (20)     4951 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/reports/train_ml_model_reports/ROCCurveSummary.py
--rw-r--r--   0 milenpa    (501) staff       (20)    10385 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/reports/train_ml_model_reports/ReferenceSequenceOverlap.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1910 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/reports/train_ml_model_reports/TrainMLModelReport.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/reports/train_ml_model_reports/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.168808 immuneML-2.2.4/immuneML/simulation/
--rw-r--r--   0 milenpa    (501) staff       (20)     4696 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/simulation/Implanting.py
--rw-r--r--   0 milenpa    (501) staff       (20)      296 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/simulation/Simulation.py
--rw-r--r--   0 milenpa    (501) staff       (20)      437 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/simulation/SimulationState.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/simulation/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.169957 immuneML-2.2.4/immuneML/simulation/dataset_generation/
--rw-r--r--   0 milenpa    (501) staff       (20)    15262 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/simulation/dataset_generation/RandomDatasetGenerator.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/simulation/dataset_generation/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.173894 immuneML-2.2.4/immuneML/simulation/implants/
--rw-r--r--   0 milenpa    (501) staff       (20)      179 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/simulation/implants/ImplantAnnotation.py
--rw-r--r--   0 milenpa    (501) staff       (20)     7001 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/simulation/implants/Motif.py
--rw-r--r--   0 milenpa    (501) staff       (20)      610 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/simulation/implants/MotifInstance.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3263 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/simulation/implants/Signal.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/simulation/implants/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.175415 immuneML-2.2.4/immuneML/simulation/motif_instantiation_strategy/
--rw-r--r--   0 milenpa    (501) staff       (20)     7395 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/simulation/motif_instantiation_strategy/GappedKmerInstantiation.py
--rw-r--r--   0 milenpa    (501) staff       (20)      306 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/simulation/motif_instantiation_strategy/MotifInstantiationStrategy.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/simulation/motif_instantiation_strategy/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.176877 immuneML-2.2.4/immuneML/simulation/sequence_implanting/
--rw-r--r--   0 milenpa    (501) staff       (20)     3518 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/simulation/sequence_implanting/GappedMotifImplanting.py
--rw-r--r--   0 milenpa    (501) staff       (20)      314 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/simulation/sequence_implanting/SequenceImplantingStrategy.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/simulation/sequence_implanting/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.180162 immuneML-2.2.4/immuneML/simulation/signal_implanting_strategy/
--rw-r--r--   0 milenpa    (501) staff       (20)     3956 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/simulation/signal_implanting_strategy/FullSequenceImplanting.py
--rw-r--r--   0 milenpa    (501) staff       (20)     7951 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/simulation/signal_implanting_strategy/HealthySequenceImplanting.py
--rw-r--r--   0 milenpa    (501) staff       (20)      665 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/simulation/signal_implanting_strategy/ImplantingComputation.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2284 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/simulation/signal_implanting_strategy/ReceptorImplanting.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2104 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/simulation/signal_implanting_strategy/SignalImplantingStrategy.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/simulation/signal_implanting_strategy/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.194558 immuneML-2.2.4/immuneML/util/
--rw-r--r--   0 milenpa    (501) staff       (20)     3776 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/util/AdaptiveImportHelper.py
--rw-r--r--   0 milenpa    (501) staff       (20)     5666 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/util/CompAIRRHelper.py
--rw-r--r--   0 milenpa    (501) staff       (20)      296 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/util/CompAIRRParams.py
--rw-r--r--   0 milenpa    (501) staff       (20)      448 2022-01-11 11:48:50.000000 immuneML-2.2.4/immuneML/util/DistanceMetrics.py
--rw-r--r--   0 milenpa    (501) staff       (20)      405 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/util/DocEnumHelper.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3141 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/util/EncoderHelper.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1157 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/util/FilenameHandler.py
--rw-r--r--   0 milenpa    (501) staff       (20)    28189 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/util/ImportHelper.py
--rw-r--r--   0 milenpa    (501) staff       (20)     5601 2022-08-16 15:04:59.000000 immuneML-2.2.4/immuneML/util/KmerHelper.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1157 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/util/Logger.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1043 2021-01-29 20:00:50.000000 immuneML-2.2.4/immuneML/util/NameBuilder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1602 2022-11-26 20:10:44.000000 immuneML-2.2.4/immuneML/util/NumpyHelper.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3840 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/util/ParameterValidator.py
--rw-r--r--   0 milenpa    (501) staff       (20)      553 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/util/PathBuilder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     4521 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/util/PositionHelper.py
--rw-r--r--   0 milenpa    (501) staff       (20)       85 2022-02-11 22:47:04.000000 immuneML-2.2.4/immuneML/util/ReadsType.py
--rw-r--r--   0 milenpa    (501) staff       (20)     4128 2023-03-23 12:33:14.000000 immuneML-2.2.4/immuneML/util/ReflectionHandler.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2883 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/util/RepertoireBuilder.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1927 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/util/SequenceAnalysisHelper.py
--rw-r--r--   0 milenpa    (501) staff       (20)     6171 2022-08-16 12:17:24.000000 immuneML-2.2.4/immuneML/util/SignificantFeaturesHelper.py
--rw-r--r--   0 milenpa    (501) staff       (20)      401 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/util/StringHelper.py
--rw-r--r--   0 milenpa    (501) staff       (20)     5834 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/util/TCRdistHelper.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/util/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.194830 immuneML-2.2.4/immuneML/workflows/
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/workflows/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.197814 immuneML-2.2.4/immuneML/workflows/instructions/
--rw-r--r--   0 milenpa    (501) staff       (20)      156 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/workflows/instructions/Instruction.py
--rw-r--r--   0 milenpa    (501) staff       (20)     7458 2022-11-28 13:16:24.000000 immuneML-2.2.4/immuneML/workflows/instructions/MLProcess.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3984 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/workflows/instructions/SimulationInstruction.py
--rw-r--r--   0 milenpa    (501) staff       (20)    17389 2022-11-28 13:16:24.000000 immuneML-2.2.4/immuneML/workflows/instructions/TrainMLModelInstruction.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/workflows/instructions/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.199597 immuneML-2.2.4/immuneML/workflows/instructions/dataset_generation/
--rw-r--r--   0 milenpa    (501) staff       (20)     4755 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/workflows/instructions/dataset_generation/DatasetExportInstruction.py
--rw-r--r--   0 milenpa    (501) staff       (20)      390 2021-05-14 20:04:47.000000 immuneML-2.2.4/immuneML/workflows/instructions/dataset_generation/DatasetExportState.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/workflows/instructions/dataset_generation/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.201512 immuneML-2.2.4/immuneML/workflows/instructions/exploratory_analysis/
--rw-r--r--   0 milenpa    (501) staff       (20)     6774 2023-03-27 12:15:28.000000 immuneML-2.2.4/immuneML/workflows/instructions/exploratory_analysis/ExploratoryAnalysisInstruction.py
--rw-r--r--   0 milenpa    (501) staff       (20)      191 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/workflows/instructions/exploratory_analysis/ExploratoryAnalysisState.py
--rw-r--r--   0 milenpa    (501) staff       (20)      596 2023-03-27 12:15:28.000000 immuneML-2.2.4/immuneML/workflows/instructions/exploratory_analysis/ExploratoryAnalysisUnit.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/workflows/instructions/exploratory_analysis/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.202923 immuneML-2.2.4/immuneML/workflows/instructions/ml_model_application/
--rw-r--r--   0 milenpa    (501) staff       (20)     3733 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/workflows/instructions/ml_model_application/MLApplicationInstruction.py
--rw-r--r--   0 milenpa    (501) staff       (20)      469 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/workflows/instructions/ml_model_application/MLApplicationState.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/workflows/instructions/ml_model_application/__init__.py
--rw-r--r--   0 milenpa    (501) staff       (20)     6243 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/workflows/instructions/quickstart.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.204383 immuneML-2.2.4/immuneML/workflows/instructions/subsampling/
--rw-r--r--   0 milenpa    (501) staff       (20)     4338 2021-06-24 13:55:25.000000 immuneML-2.2.4/immuneML/workflows/instructions/subsampling/SubsamplingInstruction.py
--rw-r--r--   0 milenpa    (501) staff       (20)      597 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/workflows/instructions/subsampling/SubsamplingState.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/workflows/instructions/subsampling/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.210360 immuneML-2.2.4/immuneML/workflows/steps/
--rw-r--r--   0 milenpa    (501) staff       (20)      834 2022-11-28 13:16:24.000000 immuneML-2.2.4/immuneML/workflows/steps/DataEncoder.py
--rw-r--r--   0 milenpa    (501) staff       (20)      404 2021-06-24 13:55:25.000000 immuneML-2.2.4/immuneML/workflows/steps/DataEncoderParams.py
--rw-r--r--   0 milenpa    (501) staff       (20)     6409 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/workflows/steps/MLMethodAssessment.py
--rw-r--r--   0 milenpa    (501) staff       (20)      867 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/workflows/steps/MLMethodAssessmentParams.py
--rw-r--r--   0 milenpa    (501) staff       (20)     2636 2023-03-27 12:19:55.000000 immuneML-2.2.4/immuneML/workflows/steps/MLMethodTrainer.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1019 2022-01-26 11:32:50.000000 immuneML-2.2.4/immuneML/workflows/steps/MLMethodTrainerParams.py
--rw-r--r--   0 milenpa    (501) staff       (20)     7924 2023-03-30 09:07:23.000000 immuneML-2.2.4/immuneML/workflows/steps/SignalImplanter.py
--rw-r--r--   0 milenpa    (501) staff       (20)      677 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/workflows/steps/Step.py
--rw-r--r--   0 milenpa    (501) staff       (20)       63 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/workflows/steps/StepParams.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/workflows/steps/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.214013 immuneML-2.2.4/immuneML/workflows/steps/data_splitter/
--rw-r--r--   0 milenpa    (501) staff       (20)     4886 2021-03-04 13:59:32.000000 immuneML-2.2.4/immuneML/workflows/steps/data_splitter/DataSplitter.py
--rw-r--r--   0 milenpa    (501) staff       (20)      641 2021-03-04 13:59:32.000000 immuneML-2.2.4/immuneML/workflows/steps/data_splitter/DataSplitterParams.py
--rw-r--r--   0 milenpa    (501) staff       (20)     4245 2023-03-27 12:15:28.000000 immuneML-2.2.4/immuneML/workflows/steps/data_splitter/LeaveOneOutSplitter.py
--rw-r--r--   0 milenpa    (501) staff       (20)     3830 2023-03-27 12:19:55.000000 immuneML-2.2.4/immuneML/workflows/steps/data_splitter/ManualSplitter.py
--rw-r--r--   0 milenpa    (501) staff       (20)      698 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/workflows/steps/data_splitter/Util.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.4/immuneML/workflows/steps/data_splitter/__init__.py
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:44.916975 immuneML-2.2.4/immuneML.egg-info/
--rw-r--r--   0 milenpa    (501) staff       (20)    11216 2023-03-30 09:32:44.000000 immuneML-2.2.4/immuneML.egg-info/PKG-INFO
--rw-r--r--   0 milenpa    (501) staff       (20)    25227 2023-03-30 09:32:44.000000 immuneML-2.2.4/immuneML.egg-info/SOURCES.txt
--rw-r--r--   0 milenpa    (501) staff       (20)        1 2023-03-30 09:32:44.000000 immuneML-2.2.4/immuneML.egg-info/dependency_links.txt
--rw-r--r--   0 milenpa    (501) staff       (20)      131 2023-03-30 09:32:44.000000 immuneML-2.2.4/immuneML.egg-info/entry_points.txt
--rw-r--r--   0 milenpa    (501) staff       (20)      316 2023-03-30 09:32:44.000000 immuneML-2.2.4/immuneML.egg-info/requires.txt
--rw-r--r--   0 milenpa    (501) staff       (20)       17 2023-03-30 09:32:44.000000 immuneML-2.2.4/immuneML.egg-info/top_level.txt
-drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-03-30 09:32:45.215760 immuneML-2.2.4/scripts/
--rw-r--r--   0 milenpa    (501) staff       (20)      326 2020-08-20 10:24:45.000000 immuneML-2.2.4/scripts/DocumentatonFormat.py
--rw-r--r--   0 milenpa    (501) staff       (20)        0 2020-08-20 10:24:45.000000 immuneML-2.2.4/scripts/__init__.py
--rw-r--r--   0 milenpa    (501) staff       (20)     1115 2021-01-21 12:25:11.000000 immuneML-2.2.4/scripts/specification_util.py
--rw-r--r--   0 milenpa    (501) staff       (20)      744 2021-01-29 13:07:48.000000 immuneML-2.2.4/scripts/specs_docs_generation.py
--rw-r--r--   0 milenpa    (501) staff       (20)       38 2023-03-30 09:32:45.217038 immuneML-2.2.4/setup.cfg
--rw-r--r--   0 milenpa    (501) staff       (20)     2107 2023-03-30 09:17:22.000000 immuneML-2.2.4/setup.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.137127 immuneML-2.2.5/
+-rw-r--r--   0 milenpa    (501) staff       (20)    34523 2020-11-01 17:12:10.000000 immuneML-2.2.5/LICENSE.md
+-rw-r--r--   0 milenpa    (501) staff       (20)    11216 2023-05-25 12:56:47.136677 immuneML-2.2.5/PKG-INFO
+-rw-r--r--   0 milenpa    (501) staff       (20)    10674 2023-04-25 08:33:54.000000 immuneML-2.2.5/README.md
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.824871 immuneML-2.2.5/immuneML/
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.828462 immuneML-2.2.5/immuneML/IO/
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/IO/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.831571 immuneML-2.2.5/immuneML/IO/dataset_export/
+-rw-r--r--   0 milenpa    (501) staff       (20)     9937 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/IO/dataset_export/AIRRExporter.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      350 2022-02-11 22:47:04.000000 immuneML-2.2.5/immuneML/IO/dataset_export/DataExporter.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     5680 2022-02-11 22:47:04.000000 immuneML-2.2.5/immuneML/IO/dataset_export/ImmuneMLExporter.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/IO/dataset_export/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.845811 immuneML-2.2.5/immuneML/IO/dataset_import/
+-rw-r--r--   0 milenpa    (501) staff       (20)    12997 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/IO/dataset_import/AIRRImport.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      247 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/IO/dataset_import/DataImport.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1688 2021-03-04 13:59:32.000000 immuneML-2.2.5/immuneML/IO/dataset_import/DatasetImportParams.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    10385 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/IO/dataset_import/GenericImport.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    10367 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/IO/dataset_import/IGoRImport.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    20610 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/IO/dataset_import/IReceptorImport.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     6620 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/IO/dataset_import/ImmuneMLImport.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    10716 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/IO/dataset_import/ImmunoSEQRearrangementImport.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    10246 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/IO/dataset_import/ImmunoSEQSampleImport.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    10596 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/IO/dataset_import/MiXCRImport.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     6487 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/IO/dataset_import/OLGAImport.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     5467 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/IO/dataset_import/RandomReceptorDatasetImport.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4180 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/IO/dataset_import/RandomRepertoireDatasetImport.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4542 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/IO/dataset_import/RandomSequenceDatasetImport.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    11644 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/IO/dataset_import/SingleLineReceptorImport.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    10684 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/IO/dataset_import/TenxGenomicsImport.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    12383 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/IO/dataset_import/VDJdbImport.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/IO/dataset_import/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.846129 immuneML-2.2.5/immuneML/IO/dataset_import/conversion/
+-rw-r--r--   0 milenpa    (501) staff       (20)    14265 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/IO/dataset_import/conversion/imgt_adaptive_conversion.csv
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.848715 immuneML-2.2.5/immuneML/IO/ml_method/
+-rw-r--r--   0 milenpa    (501) staff       (20)     3131 2023-03-30 09:08:07.000000 immuneML-2.2.5/immuneML/IO/ml_method/MLExporter.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2156 2023-03-30 09:08:07.000000 immuneML-2.2.5/immuneML/IO/ml_method/MLImport.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      959 2023-03-30 09:08:07.000000 immuneML-2.2.5/immuneML/IO/ml_method/MLMethodConfiguration.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1868 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/IO/ml_method/UtilIO.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/IO/ml_method/__init__.py
+-rw-r--r--   0 milenpa    (501) staff       (20)       86 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.850138 immuneML-2.2.5/immuneML/analysis/
+-rw-r--r--   0 milenpa    (501) staff       (20)       84 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/analysis/AxisType.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     5129 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/analysis/SequenceMatcher.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/analysis/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.853498 immuneML-2.2.5/immuneML/analysis/criteria_matches/
+-rw-r--r--   0 milenpa    (501) staff       (20)       73 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/analysis/criteria_matches/BooleanType.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     5413 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/analysis/criteria_matches/CriteriaMatcher.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      977 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/analysis/criteria_matches/CriteriaTypeInstantiator.py
+-rw-r--r--   0 milenpa    (501) staff       (20)       62 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/analysis/criteria_matches/DataType.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      163 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/analysis/criteria_matches/OperationType.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/analysis/criteria_matches/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.855743 immuneML-2.2.5/immuneML/analysis/data_manipulation/
+-rw-r--r--   0 milenpa    (501) staff       (20)     1717 2023-03-27 12:19:55.000000 immuneML-2.2.5/immuneML/analysis/data_manipulation/DataReshaper.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      156 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/analysis/data_manipulation/NormalizationType.py
+-rwxr-xr-x   0 milenpa    (501) staff       (20)       78 2021-01-29 20:00:50.000000 immuneML-2.2.5/immuneML/analysis/data_manipulation/ReductionMethod.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/analysis/data_manipulation/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.856360 immuneML-2.2.5/immuneML/analysis/entropy_calculations/
+-rw-r--r--   0 milenpa    (501) staff       (20)      977 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/analysis/entropy_calculations/EntropyCalculator.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/analysis/entropy_calculations/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.857246 immuneML-2.2.5/immuneML/analysis/similarities/
+-rw-r--r--   0 milenpa    (501) staff       (20)     1840 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/analysis/similarities/RepertoireSimilarityComputer.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      109 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/analysis/similarities/SimilarityMeasureType.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/analysis/similarities/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.857608 immuneML-2.2.5/immuneML/api/
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/api/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.858641 immuneML-2.2.5/immuneML/api/aggregated_runs/
+-rw-r--r--   0 milenpa    (501) staff       (20)     9965 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/api/aggregated_runs/MultiDatasetBenchmarkTool.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/api/aggregated_runs/__init__.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4069 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/api/api_encoding.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.867716 immuneML-2.2.5/immuneML/api/galaxy/
+-rw-r--r--   0 milenpa    (501) staff       (20)     2107 2022-01-19 10:07:52.000000 immuneML-2.2.5/immuneML/api/galaxy/DataSimulationTool.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4156 2022-11-28 13:16:24.000000 immuneML-2.2.5/immuneML/api/galaxy/DatasetGenerationTool.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2076 2022-11-28 13:16:24.000000 immuneML-2.2.5/immuneML/api/galaxy/GalaxyMLApplicationTool.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     5079 2022-01-19 10:07:52.000000 immuneML-2.2.5/immuneML/api/galaxy/GalaxySimulationTool.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      653 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/api/galaxy/GalaxyTool.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3494 2021-01-29 10:55:23.000000 immuneML-2.2.5/immuneML/api/galaxy/GalaxyTrainMLModel.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1058 2022-01-19 10:07:52.000000 immuneML-2.2.5/immuneML/api/galaxy/GalaxyYamlTool.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      638 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/api/galaxy/RepertoireClassificationTool.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     5259 2022-01-19 10:07:52.000000 immuneML-2.2.5/immuneML/api/galaxy/Util.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/api/galaxy/__init__.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4140 2021-06-24 13:55:25.000000 immuneML-2.2.5/immuneML/api/galaxy/build_dataset_yaml.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    11894 2022-02-11 22:47:04.000000 immuneML-2.2.5/immuneML/api/galaxy/build_yaml_from_arguments.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.869573 immuneML-2.2.5/immuneML/app/
+-rw-r--r--   0 milenpa    (501) staff       (20)     3698 2023-03-27 12:15:28.000000 immuneML-2.2.5/immuneML/app/ImmuneMLApp.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/app/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.872462 immuneML-2.2.5/immuneML/caching/
+-rw-r--r--   0 milenpa    (501) staff       (20)     3765 2021-10-21 14:19:15.000000 immuneML-2.2.5/immuneML/caching/CacheHandler.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      107 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/caching/CacheObjectType.py
+-rw-r--r--   0 milenpa    (501) staff       (20)       96 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/caching/CacheType.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/caching/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.807049 immuneML-2.2.5/immuneML/config/
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.808059 immuneML-2.2.5/immuneML/config/default_params/
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.880823 immuneML-2.2.5/immuneML/config/default_params/datasets/
+-rw-r--r--   0 milenpa    (501) staff       (20)      739 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/config/default_params/datasets/airr_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      424 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/config/default_params/datasets/generic_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      739 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/config/default_params/datasets/i_receptor_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      608 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/config/default_params/datasets/igor_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)     1258 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/config/default_params/datasets/immuno_seq_rearrangement_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)     1150 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/config/default_params/datasets/immuno_seq_sample_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      743 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/config/default_params/datasets/mixcr_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      608 2023-03-27 12:15:28.000000 immuneML-2.2.5/immuneML/config/default_params/datasets/olga_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      170 2023-03-07 21:32:01.000000 immuneML-2.2.5/immuneML/config/default_params/datasets/random_receptor_dataset_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      723 2023-03-07 21:31:54.000000 immuneML-2.2.5/immuneML/config/default_params/datasets/random_repertoire_dataset_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)       93 2023-03-07 21:31:47.000000 immuneML-2.2.5/immuneML/config/default_params/datasets/random_sequence_dataset_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      824 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/config/default_params/datasets/tenx_genomics_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      636 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/config/default_params/datasets/vdjdb_params.yaml
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.891082 immuneML-2.2.5/immuneML/config/default_params/encodings/
+-rw-r--r--   0 milenpa    (501) staff       (20)      101 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/config/default_params/encodings/atchley_kmer_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      128 2022-01-11 11:48:50.000000 immuneML-2.2.5/immuneML/config/default_params/encodings/comp_airr_distance_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      131 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/config/default_params/encodings/comp_airr_sequence_abundance_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)       90 2021-05-14 20:04:47.000000 immuneML-2.2.5/immuneML/config/default_params/encodings/distance_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      387 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/config/default_params/encodings/kmer_abundance_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      762 2021-02-25 10:05:14.000000 immuneML-2.2.5/immuneML/config/default_params/encodings/kmer_frequency_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      188 2022-02-11 22:47:04.000000 immuneML-2.2.5/immuneML/config/default_params/encodings/matched_receptors_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)       31 2022-02-11 22:47:04.000000 immuneML-2.2.5/immuneML/config/default_params/encodings/matched_regex_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)       95 2023-03-27 12:19:55.000000 immuneML-2.2.5/immuneML/config/default_params/encodings/matched_sequences_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      269 2021-03-04 22:07:02.000000 immuneML-2.2.5/immuneML/config/default_params/encodings/one_hot_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      119 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/config/default_params/encodings/sequence_abundance_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      258 2022-02-11 22:47:04.000000 immuneML-2.2.5/immuneML/config/default_params/encodings/word2_vec_params.yaml
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.895448 immuneML-2.2.5/immuneML/config/default_params/instructions/
+-rw-r--r--   0 milenpa    (501) staff       (20)       22 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/config/default_params/instructions/exploratory_analysis_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)       64 2021-02-18 19:16:00.000000 immuneML-2.2.5/immuneML/config/default_params/instructions/export_parser_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)       37 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/config/default_params/instructions/ml_application_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)       22 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/config/default_params/instructions/simulation_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)       62 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/config/default_params/instructions/split_config_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)       30 2021-02-18 19:16:00.000000 immuneML-2.2.5/immuneML/config/default_params/instructions/subsampling_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      905 2021-06-24 13:55:25.000000 immuneML-2.2.5/immuneML/config/default_params/instructions/train_ml_model_params.yaml
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.898152 immuneML-2.2.5/immuneML/config/default_params/ml_methods/
+-rw-r--r--   0 milenpa    (501) staff       (20)      196 2022-09-05 11:06:49.000000 immuneML-2.2.5/immuneML/config/default_params/ml_methods/atchley_kmer_mil_classifier_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      654 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/config/default_params/ml_methods/deep_rc_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      268 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/config/default_params/ml_methods/ml_method_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      307 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/config/default_params/ml_methods/receptor_cnn_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)       15 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/config/default_params/ml_methods/tcrdist_classifier_params.yaml
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.898587 immuneML-2.2.5/immuneML/config/default_params/motif_instantiation_strategy/
+-rw-r--r--   0 milenpa    (501) staff       (20)      105 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/config/default_params/motif_instantiation_strategy/gapped_kmer_params.yaml
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.899331 immuneML-2.2.5/immuneML/config/default_params/preprocessing/
+-rw-r--r--   0 milenpa    (501) staff       (20)       82 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/config/default_params/preprocessing/duplicate_sequence_filter_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)       48 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/config/default_params/preprocessing/sequence_length_filter_params.yaml
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.907972 immuneML-2.2.5/immuneML/config/default_params/reports/
+-rw-r--r--   0 milenpa    (501) staff       (20)       79 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/config/default_params/reports/amino_acid_frequency_distribution_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      131 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/config/default_params/reports/coefficients_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      125 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/config/default_params/reports/cv_feature_performance_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      340 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/config/default_params/reports/cytoscape_network_exporter_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)       26 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/config/default_params/reports/deep_rc_motif_discovery_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)       17 2021-01-29 10:55:23.000000 immuneML-2.2.5/immuneML/config/default_params/reports/design_matrix_exporter_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)       69 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/config/default_params/reports/feature_comparison_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      101 2021-03-12 15:52:25.000000 immuneML-2.2.5/immuneML/config/default_params/reports/feature_value_barplot_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)       73 2022-01-11 11:48:50.000000 immuneML-2.2.5/immuneML/config/default_params/reports/ml_settings_performance_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)       38 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/config/default_params/reports/motif_seed_recovery_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)       17 2021-02-18 19:16:00.000000 immuneML-2.2.5/immuneML/config/default_params/reports/receptor_dataset_overview_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)       28 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/config/default_params/reports/recovered_significant_features_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)       51 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/config/default_params/reports/reference_sequence_overlap_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)       20 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/config/default_params/reports/repertoire_clonotype_summary_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)       25 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/config/default_params/reports/sequence_length_distribution_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)       16 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/config/default_params/reports/significant_features_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)       60 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/config/default_params/reports/tcrdist_motif_discovery_params.yaml
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.908612 immuneML-2.2.5/immuneML/config/default_params/signal_implanting_strategy/
+-rw-r--r--   0 milenpa    (501) staff       (20)       97 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/config/default_params/signal_implanting_strategy/full_sequence_implanting_params.yaml
+-rw-r--r--   0 milenpa    (501) staff       (20)      213 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/config/default_params/signal_implanting_strategy/healthy_sequence_implanting_params.yaml
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.910488 immuneML-2.2.5/immuneML/data_model/
+-rw-r--r--   0 milenpa    (501) staff       (20)      133 2021-06-13 10:10:40.000000 immuneML-2.2.5/immuneML/data_model/DatasetItem.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/data_model/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.912663 immuneML-2.2.5/immuneML/data_model/cell/
+-rw-r--r--   0 milenpa    (501) staff       (20)      400 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/data_model/cell/Cell.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      711 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/data_model/cell/CellList.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/data_model/cell/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.916264 immuneML-2.2.5/immuneML/data_model/dataset/
+-rw-r--r--   0 milenpa    (501) staff       (20)     1191 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/data_model/dataset/Dataset.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3792 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/data_model/dataset/ElementDataset.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2813 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/data_model/dataset/ReceptorDataset.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     9053 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/data_model/dataset/RepertoireDataset.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2870 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/data_model/dataset/SequenceDataset.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/data_model/dataset/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.917355 immuneML-2.2.5/immuneML/data_model/encoded_data/
+-rw-r--r--   0 milenpa    (501) staff       (20)     2372 2023-03-27 12:15:28.000000 immuneML-2.2.5/immuneML/data_model/encoded_data/EncodedData.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/data_model/encoded_data/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.923946 immuneML-2.2.5/immuneML/data_model/receptor/
+-rw-r--r--   0 milenpa    (501) staff       (20)     1943 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/data_model/receptor/BCKReceptor.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1953 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/data_model/receptor/BCReceptor.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1249 2021-03-07 11:32:41.000000 immuneML-2.2.5/immuneML/data_model/receptor/ChainPair.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     5316 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/data_model/receptor/ElementGenerator.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1461 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/data_model/receptor/Receptor.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2599 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/data_model/receptor/ReceptorBuilder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      309 2021-01-25 16:31:21.000000 immuneML-2.2.5/immuneML/data_model/receptor/RegionType.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1966 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/data_model/receptor/TCABReceptor.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1977 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/data_model/receptor/TCGDReceptor.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/data_model/receptor/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.927785 immuneML-2.2.5/immuneML/data_model/receptor/receptor_sequence/
+-rw-r--r--   0 milenpa    (501) staff       (20)      957 2022-02-02 10:06:22.000000 immuneML-2.2.5/immuneML/data_model/receptor/receptor_sequence/Chain.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4212 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/data_model/receptor/receptor_sequence/ReceptorSequence.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      548 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/data_model/receptor/receptor_sequence/SequenceAnnotation.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      153 2021-06-24 13:55:25.000000 immuneML-2.2.5/immuneML/data_model/receptor/receptor_sequence/SequenceFrameType.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2605 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/data_model/receptor/receptor_sequence/SequenceMetadata.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/data_model/receptor/receptor_sequence/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.929310 immuneML-2.2.5/immuneML/data_model/repertoire/
+-rw-r--r--   0 milenpa    (501) staff       (20)    19013 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/data_model/repertoire/Repertoire.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/data_model/repertoire/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.930014 immuneML-2.2.5/immuneML/dev_util/
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/dev_util/__init__.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1778 2021-02-18 19:16:00.000000 immuneML-2.2.5/immuneML/dev_util/util.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.935362 immuneML-2.2.5/immuneML/dsl/
+-rw-r--r--   0 milenpa    (501) staff       (20)     1892 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/dsl/DefaultParamsLoader.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     7460 2022-11-28 13:16:24.000000 immuneML-2.2.5/immuneML/dsl/ImmuneMLParser.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     6393 2021-02-18 19:16:00.000000 immuneML-2.2.5/immuneML/dsl/InstructionParser.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3883 2021-02-18 19:16:00.000000 immuneML-2.2.5/immuneML/dsl/ObjectParser.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1093 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/dsl/OutputParser.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      139 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/dsl/Parser.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/dsl/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.941739 immuneML-2.2.5/immuneML/dsl/definition_parsers/
+-rw-r--r--   0 milenpa    (501) staff       (20)     7909 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/dsl/definition_parsers/DefinitionParser.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      523 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/dsl/definition_parsers/DefinitionParserOutput.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1852 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/dsl/definition_parsers/EncodingParser.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4497 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/dsl/definition_parsers/MLParser.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2469 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/dsl/definition_parsers/MotifParser.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1377 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/dsl/definition_parsers/PreprocessingParser.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1202 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/dsl/definition_parsers/ReportParser.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3180 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/dsl/definition_parsers/SignalParser.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4429 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/dsl/definition_parsers/SimulationParser.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/dsl/definition_parsers/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.942625 immuneML-2.2.5/immuneML/dsl/import_parsers/
+-rw-r--r--   0 milenpa    (501) staff       (20)     4589 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/dsl/import_parsers/ImportParser.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/dsl/import_parsers/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.947187 immuneML-2.2.5/immuneML/dsl/instruction_parsers/
+-rw-r--r--   0 milenpa    (501) staff       (20)     3560 2022-02-11 22:47:04.000000 immuneML-2.2.5/immuneML/dsl/instruction_parsers/DatasetExportParser.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3829 2023-03-27 12:15:28.000000 immuneML-2.2.5/immuneML/dsl/instruction_parsers/ExploratoryAnalysisParser.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2825 2022-02-11 22:47:04.000000 immuneML-2.2.5/immuneML/dsl/instruction_parsers/LabelHelper.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3300 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/dsl/instruction_parsers/MLApplicationParser.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4484 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/dsl/instruction_parsers/SimulationParser.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2323 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/dsl/instruction_parsers/SubsamplingParser.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    13497 2023-03-27 12:19:55.000000 immuneML-2.2.5/immuneML/dsl/instruction_parsers/TrainMLModelParser.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/dsl/instruction_parsers/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.948549 immuneML-2.2.5/immuneML/dsl/semantic_model/
+-rw-r--r--   0 milenpa    (501) staff       (20)       72 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/dsl/semantic_model/MLResult.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1882 2022-11-28 13:16:24.000000 immuneML-2.2.5/immuneML/dsl/semantic_model/SemanticModel.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/dsl/semantic_model/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.950291 immuneML-2.2.5/immuneML/dsl/symbol_table/
+-rw-r--r--   0 milenpa    (501) staff       (20)     2448 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/dsl/symbol_table/SymbolTable.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      298 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/dsl/symbol_table/SymbolTableEntry.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      220 2023-03-27 12:15:28.000000 immuneML-2.2.5/immuneML/dsl/symbol_table/SymbolType.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/dsl/symbol_table/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.951731 immuneML-2.2.5/immuneML/encodings/
+-rw-r--r--   0 milenpa    (501) staff       (20)     2006 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/encodings/DatasetEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      353 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/encodings/EncoderParams.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/encodings/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.954885 immuneML-2.2.5/immuneML/encodings/abundance_encoding/
+-rw-r--r--   0 milenpa    (501) staff       (20)     6212 2023-03-27 12:15:28.000000 immuneML-2.2.5/immuneML/encodings/abundance_encoding/AbundanceEncoderHelper.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1763 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/encodings/abundance_encoding/CompAIRRBatchIterator.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    19582 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/encodings/abundance_encoding/CompAIRRSequenceAbundanceEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    13959 2023-03-27 12:15:28.000000 immuneML-2.2.5/immuneML/encodings/abundance_encoding/KmerAbundanceEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    11123 2023-03-27 12:15:28.000000 immuneML-2.2.5/immuneML/encodings/abundance_encoding/SequenceAbundanceEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/encodings/abundance_encoding/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.956967 immuneML-2.2.5/immuneML/encodings/atchley_kmer_encoding/
+-rw-r--r--   0 milenpa    (501) staff       (20)    10094 2021-06-05 21:38:55.000000 immuneML-2.2.5/immuneML/encodings/atchley_kmer_encoding/AtchleyKmerEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      162 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/encodings/atchley_kmer_encoding/RelativeAbundanceType.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     5766 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/encodings/atchley_kmer_encoding/Util.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/encodings/atchley_kmer_encoding/__init__.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      751 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/encodings/atchley_kmer_encoding/atchley_factors.csv
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.957792 immuneML-2.2.5/immuneML/encodings/deeprc/
+-rw-r--r--   0 milenpa    (501) staff       (20)     4269 2021-03-04 20:37:49.000000 immuneML-2.2.5/immuneML/encodings/deeprc/DeepRCEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/encodings/deeprc/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.960544 immuneML-2.2.5/immuneML/encodings/distance_encoding/
+-rw-r--r--   0 milenpa    (501) staff       (20)    12292 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/encodings/distance_encoding/CompAIRRDistanceEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     7335 2021-08-03 14:43:33.000000 immuneML-2.2.5/immuneML/encodings/distance_encoding/DistanceEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      116 2022-01-11 11:48:50.000000 immuneML-2.2.5/immuneML/encodings/distance_encoding/DistanceMetricType.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3614 2023-02-07 13:47:33.000000 immuneML-2.2.5/immuneML/encodings/distance_encoding/TCRdistEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/encodings/distance_encoding/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.962785 immuneML-2.2.5/immuneML/encodings/evenness_profile/
+-rw-r--r--   0 milenpa    (501) staff       (20)     5330 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/encodings/evenness_profile/EvennessProfileEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3398 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/encodings/evenness_profile/EvennessProfileRepertoireEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/encodings/evenness_profile/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.966702 immuneML-2.2.5/immuneML/encodings/kmer_frequency/
+-rw-r--r--   0 milenpa    (501) staff       (20)     2222 2021-06-24 13:55:25.000000 immuneML-2.2.5/immuneML/encodings/kmer_frequency/KmerFreqReceptorEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2994 2023-03-23 12:33:14.000000 immuneML-2.2.5/immuneML/encodings/kmer_frequency/KmerFreqRepertoireEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1633 2021-01-29 10:55:23.000000 immuneML-2.2.5/immuneML/encodings/kmer_frequency/KmerFreqSequenceEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    15879 2023-03-27 12:19:55.000000 immuneML-2.2.5/immuneML/encodings/kmer_frequency/KmerFrequencyEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/encodings/kmer_frequency/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.972966 immuneML-2.2.5/immuneML/encodings/kmer_frequency/sequence_encoding/
+-rw-r--r--   0 milenpa    (501) staff       (20)     2015 2022-02-11 22:47:04.000000 immuneML-2.2.5/immuneML/encodings/kmer_frequency/sequence_encoding/GappedKmerSequenceEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2227 2022-02-11 22:47:04.000000 immuneML-2.2.5/immuneML/encodings/kmer_frequency/sequence_encoding/IMGTGappedKmerEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1693 2022-02-11 22:47:04.000000 immuneML-2.2.5/immuneML/encodings/kmer_frequency/sequence_encoding/IMGTKmerSequenceEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1864 2022-02-11 22:47:04.000000 immuneML-2.2.5/immuneML/encodings/kmer_frequency/sequence_encoding/IdentitySequenceEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1367 2022-11-08 20:23:03.000000 immuneML-2.2.5/immuneML/encodings/kmer_frequency/sequence_encoding/KmerSequenceEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      459 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/encodings/kmer_frequency/sequence_encoding/SequenceEncodingStrategy.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      289 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/encodings/kmer_frequency/sequence_encoding/SequenceEncodingType.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/encodings/kmer_frequency/sequence_encoding/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.976498 immuneML-2.2.5/immuneML/encodings/onehot/
+-rw-r--r--   0 milenpa    (501) staff       (20)    11023 2023-03-27 12:14:54.000000 immuneML-2.2.5/immuneML/encodings/onehot/OneHotEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3948 2021-06-24 13:55:25.000000 immuneML-2.2.5/immuneML/encodings/onehot/OneHotReceptorEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     5208 2021-03-04 22:07:02.000000 immuneML-2.2.5/immuneML/encodings/onehot/OneHotRepertoireEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3256 2021-03-04 22:07:02.000000 immuneML-2.2.5/immuneML/encodings/onehot/OneHotSequenceEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/encodings/onehot/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.977656 immuneML-2.2.5/immuneML/encodings/preprocessing/
+-rw-r--r--   0 milenpa    (501) staff       (20)     2922 2023-03-27 12:19:55.000000 immuneML-2.2.5/immuneML/encodings/preprocessing/FeatureScaler.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/encodings/preprocessing/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.982458 immuneML-2.2.5/immuneML/encodings/reference_encoding/
+-rw-r--r--   0 milenpa    (501) staff       (20)    15402 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/encodings/reference_encoding/MatchedReceptorsEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2946 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/encodings/reference_encoding/MatchedReferenceUtil.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     8410 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/encodings/reference_encoding/MatchedRegexEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     5366 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/encodings/reference_encoding/MatchedRegexRepertoireEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    11521 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/encodings/reference_encoding/MatchedSequencesEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      124 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/encodings/reference_encoding/SequenceMatchingSummaryType.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/encodings/reference_encoding/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.985084 immuneML-2.2.5/immuneML/encodings/word2vec/
+-rw-r--r--   0 milenpa    (501) staff       (20)     1492 2022-02-11 22:47:04.000000 immuneML-2.2.5/immuneML/encodings/word2vec/W2VRepertoireEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1228 2022-02-11 22:47:04.000000 immuneML-2.2.5/immuneML/encodings/word2vec/W2VSequenceEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    11780 2023-03-27 12:14:54.000000 immuneML-2.2.5/immuneML/encodings/word2vec/Word2VecEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/encodings/word2vec/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.988360 immuneML-2.2.5/immuneML/encodings/word2vec/model_creator/
+-rw-r--r--   0 milenpa    (501) staff       (20)     1367 2022-02-11 22:47:04.000000 immuneML-2.2.5/immuneML/encodings/word2vec/model_creator/KmerPairModelCreator.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      622 2022-02-11 22:47:04.000000 immuneML-2.2.5/immuneML/encodings/word2vec/model_creator/ModelCreatorStrategy.py
+-rw-r--r--   0 milenpa    (501) staff       (20)       83 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/encodings/word2vec/model_creator/ModelType.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2212 2022-02-11 22:47:04.000000 immuneML-2.2.5/immuneML/encodings/word2vec/model_creator/SequenceModelCreator.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/encodings/word2vec/model_creator/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.992911 immuneML-2.2.5/immuneML/environment/
+-rw-r--r--   0 milenpa    (501) staff       (20)      385 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/environment/Constants.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3330 2022-11-28 13:16:24.000000 immuneML-2.2.5/immuneML/environment/EnvironmentSettings.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1907 2023-03-27 12:19:55.000000 immuneML-2.2.5/immuneML/environment/Label.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3344 2023-03-27 12:19:55.000000 immuneML-2.2.5/immuneML/environment/LabelConfiguration.py
+-rw-r--r--   0 milenpa    (501) staff       (20)       89 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/environment/LabelType.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      111 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/environment/SequenceType.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/environment/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.994380 immuneML-2.2.5/immuneML/hyperparameter_optimization/
+-rw-r--r--   0 milenpa    (501) staff       (20)     1042 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/hyperparameter_optimization/HPSetting.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      688 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/hyperparameter_optimization/HPSettingResult.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/hyperparameter_optimization/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.998005 immuneML-2.2.5/immuneML/hyperparameter_optimization/config/
+-rw-r--r--   0 milenpa    (501) staff       (20)      125 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/hyperparameter_optimization/config/LeaveOneOutConfig.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      171 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/hyperparameter_optimization/config/ManualSplitConfig.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3527 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/hyperparameter_optimization/config/ReportConfig.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     7724 2023-03-27 12:15:28.000000 immuneML-2.2.5/immuneML/hyperparameter_optimization/config/SplitConfig.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      170 2021-03-04 13:59:32.000000 immuneML-2.2.5/immuneML/hyperparameter_optimization/config/SplitType.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/hyperparameter_optimization/config/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.999710 immuneML-2.2.5/immuneML/hyperparameter_optimization/core/
+-rw-r--r--   0 milenpa    (501) staff       (20)     7634 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/hyperparameter_optimization/core/HPAssessment.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4765 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/hyperparameter_optimization/core/HPSelection.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     6862 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/hyperparameter_optimization/core/HPUtil.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/hyperparameter_optimization/core/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.002549 immuneML-2.2.5/immuneML/hyperparameter_optimization/states/
+-rw-r--r--   0 milenpa    (501) staff       (20)      797 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/hyperparameter_optimization/states/HPAssessmentState.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      970 2021-11-07 11:51:14.000000 immuneML-2.2.5/immuneML/hyperparameter_optimization/states/HPItem.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      478 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/hyperparameter_optimization/states/HPLabelState.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      713 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/hyperparameter_optimization/states/HPSelectionState.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1507 2022-01-11 11:48:50.000000 immuneML-2.2.5/immuneML/hyperparameter_optimization/states/TrainMLModelState.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/hyperparameter_optimization/states/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.003758 immuneML-2.2.5/immuneML/hyperparameter_optimization/strategy/
+-rw-r--r--   0 milenpa    (501) staff       (20)     2328 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/hyperparameter_optimization/strategy/GridSearch.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1598 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/hyperparameter_optimization/strategy/HPOptimizationStrategy.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/hyperparameter_optimization/strategy/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.013193 immuneML-2.2.5/immuneML/ml_methods/
+-rw-r--r--   0 milenpa    (501) staff       (20)    10971 2023-03-27 12:19:55.000000 immuneML-2.2.5/immuneML/ml_methods/AtchleyKmerMILClassifier.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    21752 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/ml_methods/DeepRC.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3753 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/ml_methods/KNN.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3143 2021-10-22 09:13:56.000000 immuneML-2.2.5/immuneML/ml_methods/LogisticRegression.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    15572 2023-03-30 09:08:07.000000 immuneML-2.2.5/immuneML/ml_methods/MLMethod.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3105 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/ml_methods/PrecomputedKNN.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    20861 2023-03-27 12:19:55.000000 immuneML-2.2.5/immuneML/ml_methods/ProbabilisticBinaryClassifier.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3046 2021-02-18 19:16:00.000000 immuneML-2.2.5/immuneML/ml_methods/RandomForestClassifier.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    17041 2023-03-27 12:19:55.000000 immuneML-2.2.5/immuneML/ml_methods/ReceptorCNN.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2593 2022-01-11 11:48:50.000000 immuneML-2.2.5/immuneML/ml_methods/SVC.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2745 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/ml_methods/SVM.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    13710 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/ml_methods/SklearnMethod.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2896 2022-01-11 11:48:50.000000 immuneML-2.2.5/immuneML/ml_methods/TCRdistClassifier.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/ml_methods/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.015318 immuneML-2.2.5/immuneML/ml_methods/pytorch_implementations/
+-rw-r--r--   0 milenpa    (501) staff       (20)      531 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/ml_methods/pytorch_implementations/PyTorchLogisticRegression.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     6046 2021-03-04 13:59:32.000000 immuneML-2.2.5/immuneML/ml_methods/pytorch_implementations/PyTorchReceptorCNN.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/ml_methods/pytorch_implementations/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.016552 immuneML-2.2.5/immuneML/ml_methods/util/
+-rw-r--r--   0 milenpa    (501) staff       (20)     4598 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/ml_methods/util/Util.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/ml_methods/util/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.018556 immuneML-2.2.5/immuneML/ml_metrics/
+-rw-r--r--   0 milenpa    (501) staff       (20)     1132 2023-03-27 12:19:55.000000 immuneML-2.2.5/immuneML/ml_metrics/Metric.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2121 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/ml_metrics/MetricUtil.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/ml_metrics/__init__.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      925 2022-11-28 13:16:24.000000 immuneML-2.2.5/immuneML/ml_metrics/ml_metrics.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.021615 immuneML-2.2.5/immuneML/pairwise_repertoire_comparison/
+-rw-r--r--   0 milenpa    (501) staff       (20)     8646 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/pairwise_repertoire_comparison/ComparisonData.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2509 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/pairwise_repertoire_comparison/ComparisonDataBatch.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3436 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/pairwise_repertoire_comparison/PairwiseRepertoireComparison.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/pairwise_repertoire_comparison/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.023721 immuneML-2.2.5/immuneML/preprocessing/
+-rw-r--r--   0 milenpa    (501) staff       (20)     1282 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/preprocessing/Preprocessor.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    11134 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/preprocessing/ReferenceSequenceAnnotator.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3272 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/preprocessing/SubjectRepertoireCollector.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/preprocessing/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.028801 immuneML-2.2.5/immuneML/preprocessing/filters/
+-rw-r--r--   0 milenpa    (501) staff       (20)     2327 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/preprocessing/filters/ChainRepertoireFilter.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2638 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/preprocessing/filters/ClonesPerRepertoireFilter.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      166 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/preprocessing/filters/CountAggregationFunction.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4028 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/preprocessing/filters/CountPerSequenceFilter.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     8649 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/preprocessing/filters/DuplicateSequenceFilter.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1396 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/preprocessing/filters/Filter.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3015 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/preprocessing/filters/MetadataRepertoireFilter.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4326 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/preprocessing/filters/SequenceLengthFilter.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/preprocessing/filters/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.032444 immuneML-2.2.5/immuneML/presentation/
+-rw-r--r--   0 milenpa    (501) staff       (20)      170 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/presentation/InstructionPresentation.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2353 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/presentation/PresentationFactory.py
+-rw-r--r--   0 milenpa    (501) staff       (20)       74 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/presentation/PresentationFormat.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      456 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/presentation/TemplateParser.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/presentation/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.039845 immuneML-2.2.5/immuneML/presentation/html/
+-rw-r--r--   0 milenpa    (501) staff       (20)     3281 2021-05-14 20:04:47.000000 immuneML-2.2.5/immuneML/presentation/html/DatasetExportHTMLBuilder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4562 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/presentation/html/ExploratoryAnalysisHTMLBuilder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    21349 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/presentation/html/HPHTMLBuilder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3418 2021-06-23 22:15:10.000000 immuneML-2.2.5/immuneML/presentation/html/HTMLBuilder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2500 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/presentation/html/MLApplicationHTMLBuilder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1651 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/presentation/html/MultiDatasetBenchmarkHTMLBuilder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2985 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/presentation/html/SimulationHTMLBuilder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2879 2021-01-29 10:55:23.000000 immuneML-2.2.5/immuneML/presentation/html/SubsamplingHTMLBuilder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4783 2021-02-18 19:16:00.000000 immuneML-2.2.5/immuneML/presentation/html/Util.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/presentation/html/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.047168 immuneML-2.2.5/immuneML/presentation/html/templates/
+-rw-r--r--   0 milenpa    (501) staff       (20)     7651 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/presentation/html/templates/AssessmentSplitDetails.html
+-rw-r--r--   0 milenpa    (501) staff       (20)     2940 2021-05-14 20:04:47.000000 immuneML-2.2.5/immuneML/presentation/html/templates/DatasetExport.html
+-rw-r--r--   0 milenpa    (501) staff       (20)     6023 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/presentation/html/templates/ExploratoryAnalysis.html
+-rw-r--r--   0 milenpa    (501) staff       (20)     6961 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/presentation/html/templates/HPOptimization.html
+-rw-r--r--   0 milenpa    (501) staff       (20)     2456 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/presentation/html/templates/MLApplication.html
+-rw-r--r--   0 milenpa    (501) staff       (20)     2614 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/presentation/html/templates/MLTraining.html
+-rw-r--r--   0 milenpa    (501) staff       (20)     1799 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/presentation/html/templates/MultiDatasetBenchmark.html
+-rw-r--r--   0 milenpa    (501) staff       (20)     2889 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/presentation/html/templates/Reports.html
+-rw-r--r--   0 milenpa    (501) staff       (20)     9566 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/presentation/html/templates/SelectionDetails.html
+-rw-r--r--   0 milenpa    (501) staff       (20)     4760 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/presentation/html/templates/Simulation.html
+-rw-r--r--   0 milenpa    (501) staff       (20)     3078 2021-01-29 10:55:23.000000 immuneML-2.2.5/immuneML/presentation/html/templates/Subsampling.html
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.047922 immuneML-2.2.5/immuneML/presentation/html/templates/css/
+-rw-r--r--   0 milenpa    (501) staff       (20)     2465 2021-02-18 19:16:00.000000 immuneML-2.2.5/immuneML/presentation/html/templates/css/custom.css
+-rw-r--r--   0 milenpa    (501) staff       (20)      705 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/presentation/html/templates/index.html
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.052713 immuneML-2.2.5/immuneML/reports/
+-rw-r--r--   0 milenpa    (501) staff       (20)     1824 2021-03-07 11:32:41.000000 immuneML-2.2.5/immuneML/reports/PlotlyUtil.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     7326 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/reports/Report.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      201 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/reports/ReportOutput.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      480 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/reports/ReportResult.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2847 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/reports/ReportUtil.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/reports/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.061204 immuneML-2.2.5/immuneML/reports/data_reports/
+-rw-r--r--   0 milenpa    (501) staff       (20)    12973 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/reports/data_reports/AminoAcidFrequencyDistribution.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     8755 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/reports/data_reports/CytoscapeNetworkExporter.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2473 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/reports/data_reports/DataReport.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3510 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/reports/data_reports/GLIPH2Exporter.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4131 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/reports/data_reports/ReceptorDatasetOverview.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    12600 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/reports/data_reports/RecoveredSignificantFeatures.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3946 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/reports/data_reports/RepertoireClonotypeSummary.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4706 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/reports/data_reports/SequenceLengthDistribution.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     6358 2023-03-27 12:19:55.000000 immuneML-2.2.5/immuneML/reports/data_reports/SequencesWithSignificantKmers.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    12893 2023-03-27 12:19:55.000000 immuneML-2.2.5/immuneML/reports/data_reports/SignificantFeatures.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     8820 2022-09-19 11:30:27.000000 immuneML-2.2.5/immuneML/reports/data_reports/SignificantKmerPositions.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4514 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/reports/data_reports/SimpleDatasetOverview.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/reports/data_reports/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.067987 immuneML-2.2.5/immuneML/reports/encoding_reports/
+-rw-r--r--   0 milenpa    (501) staff       (20)     5814 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/reports/encoding_reports/DesignMatrixExporter.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2476 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/reports/encoding_reports/EncodingReport.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    11835 2023-03-27 12:19:55.000000 immuneML-2.2.5/immuneML/reports/encoding_reports/FeatureComparison.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     6182 2022-11-28 13:16:24.000000 immuneML-2.2.5/immuneML/reports/encoding_reports/FeatureDistribution.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3521 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/reports/encoding_reports/FeatureReport.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     6448 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/reports/encoding_reports/FeatureValueBarplot.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    12279 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/reports/encoding_reports/Matches.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4148 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/reports/encoding_reports/RelevantSequenceExporter.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/reports/encoding_reports/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.077632 immuneML-2.2.5/immuneML/reports/ml_reports/
+-rw-r--r--   0 milenpa    (501) staff       (20)      154 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/reports/ml_reports/CoefficientPlottingSetting.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      825 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/reports/ml_reports/CoefficientPlottingSettingList.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    10217 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/reports/ml_reports/Coefficients.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     6006 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/reports/ml_reports/ConfounderAnalysis.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    15785 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/reports/ml_reports/DeepRCMotifDiscovery.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     6221 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/reports/ml_reports/KernelSequenceLogo.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2852 2023-03-27 12:14:54.000000 immuneML-2.2.5/immuneML/reports/ml_reports/MLReport.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    14405 2023-03-27 12:19:55.000000 immuneML-2.2.5/immuneML/reports/ml_reports/MotifSeedRecovery.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3686 2023-03-27 12:19:55.000000 immuneML-2.2.5/immuneML/reports/ml_reports/ROCCurve.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4445 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/reports/ml_reports/SequenceAssociationLikelihood.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     9321 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/reports/ml_reports/TCRdistMotifDiscovery.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     7544 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/reports/ml_reports/TrainingPerformance.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/reports/ml_reports/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.080411 immuneML-2.2.5/immuneML/reports/multi_dataset_reports/
+-rw-r--r--   0 milenpa    (501) staff       (20)     4489 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/reports/multi_dataset_reports/DiseaseAssociatedSequenceOverlap.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2012 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/reports/multi_dataset_reports/MultiDatasetReport.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     7520 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/reports/multi_dataset_reports/PerformanceOverview.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/reports/multi_dataset_reports/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.084873 immuneML-2.2.5/immuneML/reports/train_ml_model_reports/
+-rw-r--r--   0 milenpa    (501) staff       (20)     7897 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/reports/train_ml_model_reports/CVFeaturePerformance.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     7244 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/reports/train_ml_model_reports/DiseaseAssociatedSequenceCVOverlap.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     7942 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/reports/train_ml_model_reports/MLSettingsPerformance.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4951 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/reports/train_ml_model_reports/ROCCurveSummary.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    10385 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/reports/train_ml_model_reports/ReferenceSequenceOverlap.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1910 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/reports/train_ml_model_reports/TrainMLModelReport.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/reports/train_ml_model_reports/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.087383 immuneML-2.2.5/immuneML/simulation/
+-rw-r--r--   0 milenpa    (501) staff       (20)     4696 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/simulation/Implanting.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      296 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/simulation/Simulation.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      437 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/simulation/SimulationState.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/simulation/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.088324 immuneML-2.2.5/immuneML/simulation/dataset_generation/
+-rw-r--r--   0 milenpa    (501) staff       (20)    15262 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/simulation/dataset_generation/RandomDatasetGenerator.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/simulation/dataset_generation/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.090983 immuneML-2.2.5/immuneML/simulation/implants/
+-rw-r--r--   0 milenpa    (501) staff       (20)      179 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/simulation/implants/ImplantAnnotation.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     7001 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/simulation/implants/Motif.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      610 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/simulation/implants/MotifInstance.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3263 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/simulation/implants/Signal.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/simulation/implants/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.092481 immuneML-2.2.5/immuneML/simulation/motif_instantiation_strategy/
+-rw-r--r--   0 milenpa    (501) staff       (20)     7395 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/simulation/motif_instantiation_strategy/GappedKmerInstantiation.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      306 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/simulation/motif_instantiation_strategy/MotifInstantiationStrategy.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/simulation/motif_instantiation_strategy/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.094168 immuneML-2.2.5/immuneML/simulation/sequence_implanting/
+-rw-r--r--   0 milenpa    (501) staff       (20)     3518 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/simulation/sequence_implanting/GappedMotifImplanting.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      314 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/simulation/sequence_implanting/SequenceImplantingStrategy.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/simulation/sequence_implanting/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.096826 immuneML-2.2.5/immuneML/simulation/signal_implanting_strategy/
+-rw-r--r--   0 milenpa    (501) staff       (20)     3956 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/simulation/signal_implanting_strategy/FullSequenceImplanting.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     7951 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/simulation/signal_implanting_strategy/HealthySequenceImplanting.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      665 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/simulation/signal_implanting_strategy/ImplantingComputation.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2284 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/simulation/signal_implanting_strategy/ReceptorImplanting.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2104 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/simulation/signal_implanting_strategy/SignalImplantingStrategy.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/simulation/signal_implanting_strategy/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.107752 immuneML-2.2.5/immuneML/util/
+-rw-r--r--   0 milenpa    (501) staff       (20)     3807 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/util/AdaptiveImportHelper.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     6529 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/util/CompAIRRHelper.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      447 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/util/CompAIRRParams.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      448 2022-01-11 11:48:50.000000 immuneML-2.2.5/immuneML/util/DistanceMetrics.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      405 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/util/DocEnumHelper.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3141 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/util/EncoderHelper.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1157 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/util/FilenameHandler.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    28432 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/util/ImportHelper.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     5601 2022-08-16 15:04:59.000000 immuneML-2.2.5/immuneML/util/KmerHelper.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1157 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/util/Logger.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1043 2021-01-29 20:00:50.000000 immuneML-2.2.5/immuneML/util/NameBuilder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1602 2022-11-26 20:10:44.000000 immuneML-2.2.5/immuneML/util/NumpyHelper.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     5742 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/util/ParameterValidator.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      749 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/util/PathBuilder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4521 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/util/PositionHelper.py
+-rw-r--r--   0 milenpa    (501) staff       (20)       85 2022-02-11 22:47:04.000000 immuneML-2.2.5/immuneML/util/ReadsType.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4128 2023-03-23 12:33:14.000000 immuneML-2.2.5/immuneML/util/ReflectionHandler.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2762 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/util/RepertoireBuilder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1927 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/util/SequenceAnalysisHelper.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     6171 2022-08-16 12:17:24.000000 immuneML-2.2.5/immuneML/util/SignificantFeaturesHelper.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      401 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/util/StringHelper.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     5834 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/util/TCRdistHelper.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/util/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.107946 immuneML-2.2.5/immuneML/workflows/
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/workflows/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.111132 immuneML-2.2.5/immuneML/workflows/instructions/
+-rw-r--r--   0 milenpa    (501) staff       (20)      156 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/workflows/instructions/Instruction.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     8187 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/workflows/instructions/MLProcess.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3984 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/workflows/instructions/SimulationInstruction.py
+-rw-r--r--   0 milenpa    (501) staff       (20)    17389 2022-11-28 13:16:24.000000 immuneML-2.2.5/immuneML/workflows/instructions/TrainMLModelInstruction.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/workflows/instructions/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.113466 immuneML-2.2.5/immuneML/workflows/instructions/dataset_generation/
+-rw-r--r--   0 milenpa    (501) staff       (20)     4995 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/workflows/instructions/dataset_generation/DatasetExportInstruction.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      390 2021-05-14 20:04:47.000000 immuneML-2.2.5/immuneML/workflows/instructions/dataset_generation/DatasetExportState.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/workflows/instructions/dataset_generation/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.116073 immuneML-2.2.5/immuneML/workflows/instructions/exploratory_analysis/
+-rw-r--r--   0 milenpa    (501) staff       (20)     6774 2023-03-27 12:15:28.000000 immuneML-2.2.5/immuneML/workflows/instructions/exploratory_analysis/ExploratoryAnalysisInstruction.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      191 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/workflows/instructions/exploratory_analysis/ExploratoryAnalysisState.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      596 2023-03-27 12:15:28.000000 immuneML-2.2.5/immuneML/workflows/instructions/exploratory_analysis/ExploratoryAnalysisUnit.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/workflows/instructions/exploratory_analysis/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.117620 immuneML-2.2.5/immuneML/workflows/instructions/ml_model_application/
+-rw-r--r--   0 milenpa    (501) staff       (20)     8418 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/workflows/instructions/ml_model_application/MLApplicationInstruction.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      524 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/workflows/instructions/ml_model_application/MLApplicationState.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/workflows/instructions/ml_model_application/__init__.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     6243 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/workflows/instructions/quickstart.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.119490 immuneML-2.2.5/immuneML/workflows/instructions/subsampling/
+-rw-r--r--   0 milenpa    (501) staff       (20)     4338 2021-06-24 13:55:25.000000 immuneML-2.2.5/immuneML/workflows/instructions/subsampling/SubsamplingInstruction.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      597 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/workflows/instructions/subsampling/SubsamplingState.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/workflows/instructions/subsampling/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.128400 immuneML-2.2.5/immuneML/workflows/steps/
+-rw-r--r--   0 milenpa    (501) staff       (20)      834 2022-11-28 13:16:24.000000 immuneML-2.2.5/immuneML/workflows/steps/DataEncoder.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      404 2021-06-24 13:55:25.000000 immuneML-2.2.5/immuneML/workflows/steps/DataEncoderParams.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4960 2023-05-25 12:56:15.000000 immuneML-2.2.5/immuneML/workflows/steps/MLMethodAssessment.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      867 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/workflows/steps/MLMethodAssessmentParams.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     2636 2023-03-27 12:19:55.000000 immuneML-2.2.5/immuneML/workflows/steps/MLMethodTrainer.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1019 2022-01-26 11:32:50.000000 immuneML-2.2.5/immuneML/workflows/steps/MLMethodTrainerParams.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     7924 2023-04-25 08:33:54.000000 immuneML-2.2.5/immuneML/workflows/steps/SignalImplanter.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      677 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/workflows/steps/Step.py
+-rw-r--r--   0 milenpa    (501) staff       (20)       63 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/workflows/steps/StepParams.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/workflows/steps/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.132763 immuneML-2.2.5/immuneML/workflows/steps/data_splitter/
+-rw-r--r--   0 milenpa    (501) staff       (20)     4886 2021-03-04 13:59:32.000000 immuneML-2.2.5/immuneML/workflows/steps/data_splitter/DataSplitter.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      641 2021-03-04 13:59:32.000000 immuneML-2.2.5/immuneML/workflows/steps/data_splitter/DataSplitterParams.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     4245 2023-03-27 12:15:28.000000 immuneML-2.2.5/immuneML/workflows/steps/data_splitter/LeaveOneOutSplitter.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     3830 2023-03-27 12:19:55.000000 immuneML-2.2.5/immuneML/workflows/steps/data_splitter/ManualSplitter.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      698 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/workflows/steps/data_splitter/Util.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2021-01-25 16:31:20.000000 immuneML-2.2.5/immuneML/workflows/steps/data_splitter/__init__.py
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:46.828086 immuneML-2.2.5/immuneML.egg-info/
+-rw-r--r--   0 milenpa    (501) staff       (20)    11216 2023-05-25 12:56:46.000000 immuneML-2.2.5/immuneML.egg-info/PKG-INFO
+-rw-r--r--   0 milenpa    (501) staff       (20)    25747 2023-05-25 12:56:46.000000 immuneML-2.2.5/immuneML.egg-info/SOURCES.txt
+-rw-r--r--   0 milenpa    (501) staff       (20)        1 2023-05-25 12:56:46.000000 immuneML-2.2.5/immuneML.egg-info/dependency_links.txt
+-rw-r--r--   0 milenpa    (501) staff       (20)      131 2023-05-25 12:56:46.000000 immuneML-2.2.5/immuneML.egg-info/entry_points.txt
+-rw-r--r--   0 milenpa    (501) staff       (20)      324 2023-05-25 12:56:46.000000 immuneML-2.2.5/immuneML.egg-info/requires.txt
+-rw-r--r--   0 milenpa    (501) staff       (20)       17 2023-05-25 12:56:46.000000 immuneML-2.2.5/immuneML.egg-info/top_level.txt
+drwxr-xr-x   0 milenpa    (501) staff       (20)        0 2023-05-25 12:56:47.135475 immuneML-2.2.5/scripts/
+-rw-r--r--   0 milenpa    (501) staff       (20)      326 2020-08-20 10:24:45.000000 immuneML-2.2.5/scripts/DocumentatonFormat.py
+-rw-r--r--   0 milenpa    (501) staff       (20)        0 2020-08-20 10:24:45.000000 immuneML-2.2.5/scripts/__init__.py
+-rw-r--r--   0 milenpa    (501) staff       (20)     1115 2021-01-21 12:25:11.000000 immuneML-2.2.5/scripts/specification_util.py
+-rw-r--r--   0 milenpa    (501) staff       (20)      744 2021-01-29 13:07:48.000000 immuneML-2.2.5/scripts/specs_docs_generation.py
+-rw-r--r--   0 milenpa    (501) staff       (20)       38 2023-05-25 12:56:47.137275 immuneML-2.2.5/setup.cfg
+-rw-r--r--   0 milenpa    (501) staff       (20)     2115 2023-05-25 12:56:15.000000 immuneML-2.2.5/setup.py
```

### Comparing `immuneML-2.2.4/LICENSE.md` & `immuneML-2.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/PKG-INFO` & `immuneML-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: immuneML
-Version: 2.2.4
+Version: 2.2.5
 Summary: immuneML is a software platform for machine learning analysis of immune receptor repertoires.
 Home-page: https://github.com/uio-bmi/immuneML
 Author: immuneML Team
 Author-email: milenpa@student.matnat.uio.no
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `immuneML-2.2.4/README.md` & `immuneML-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/IO/dataset_export/AIRRExporter.py` & `immuneML-2.2.5/immuneML/IO/dataset_export/AIRRExporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
                 index += 1
 
     @staticmethod
     def export_repertoire(repertoire: Repertoire, repertoire_path: Path):
         df = AIRRExporter._repertoire_to_dataframe(repertoire)
         df = AIRRExporter._postprocess_dataframe(df)
-        output_file = repertoire_path / f"{repertoire.data_filename.stem}.tsv"
+        output_file = repertoire_path / f"{repertoire.data_filename.stem if 'subject_id' not in repertoire.metadata else repertoire.metadata['subject_id']}.tsv"
         airr.dump_rearrangement(df, str(output_file))
 
     @staticmethod
     def get_sequence_field(region_type):
         if region_type == RegionType.IMGT_CDR3:
             return "cdr3"
         elif region_type == RegionType.IMGT_JUNCTION:
@@ -85,15 +85,16 @@
     def get_sequence_aa_field(region_type):
         return f"{AIRRExporter.get_sequence_field(region_type)}_aa"
 
     @staticmethod
     def export_updated_metadata(dataset: RepertoireDataset, result_path: Path, repertoire_folder: str):
         df = pd.read_csv(dataset.metadata_file, comment=Constants.COMMENT_SIGN)
         identifiers = df["identifier"].values.tolist() if "identifier" in df.columns else dataset.get_example_ids()
-        df["filename"] = [str(Path(repertoire_folder) / f"{repertoire.data_filename.stem}.tsv") for repertoire in dataset.get_data()]
+        df["filename"] = [f"{repertoire.data_filename.stem if 'subject_id' not in repertoire.metadata else repertoire.metadata['subject_id']}.tsv"
+                          for repertoire in dataset.get_data()]
         df['identifier'] = identifiers
         df.to_csv(result_path / "metadata.csv", index=False)
 
     @staticmethod
     def _repertoire_to_dataframe(repertoire: Repertoire):
         # get all fields (including custom fields)
         df = pd.DataFrame(repertoire.load_data())
```

### Comparing `immuneML-2.2.4/immuneML/IO/dataset_export/ImmuneMLExporter.py` & `immuneML-2.2.5/immuneML/IO/dataset_export/ImmuneMLExporter.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/IO/dataset_import/AIRRImport.py` & `immuneML-2.2.5/immuneML/IO/dataset_import/AIRRImport.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,20 +137,22 @@
                 if "cdr3" in df.columns:
                     df.rename(columns={"cdr3": "sequences"}, inplace=True)
                 if "cdr3_aa" in df.columns:
                     df.rename(columns={"cdr3_aa": "sequence_aas"}, inplace=True)
                 df.loc[:, "region_types"] = params.region_type.name
             elif "junction" in params.column_mapping or "junction_aa" in params.column_mapping:
                 ImportHelper.junction_to_cdr3(df, params.region_type)
+            else:
+                df.loc[:, 'region_types'] = params.region_type.name
         else:
             df.loc[:, "region_types"] = params.region_type.name
         # todo else: support "full_sequence" import through regiontype?
 
         ImportHelper.drop_empty_sequences(df, params.import_empty_aa_sequences, params.import_empty_nt_sequences)
-        ImportHelper.drop_illegal_character_sequences(df, params.import_illegal_characters)
+        ImportHelper.drop_illegal_character_sequences(df, params.import_illegal_characters, import_with_stop_codon=params.import_with_stop_codon)
         ImportHelper.update_gene_info(df)
         ImportHelper.load_chains(df)
 
         return df
 
     @staticmethod
     def alternative_load_func(filename, params):
```

### Comparing `immuneML-2.2.4/immuneML/IO/dataset_import/DatasetImportParams.py` & `immuneML-2.2.5/immuneML/IO/dataset_import/DatasetImportParams.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/IO/dataset_import/GenericImport.py` & `immuneML-2.2.5/immuneML/IO/dataset_import/GenericImport.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     @staticmethod
     def import_dataset(params: dict, dataset_name: str) -> Dataset:
         return ImportHelper.import_dataset(GenericImport, params, dataset_name)
 
     @staticmethod
     def preprocess_dataframe(df: pd.DataFrame, params: DatasetImportParams):
         ImportHelper.drop_empty_sequences(df, params.import_empty_aa_sequences, params.import_empty_nt_sequences)
-        ImportHelper.drop_illegal_character_sequences(df, params.import_illegal_characters)
+        ImportHelper.drop_illegal_character_sequences(df, params.import_illegal_characters, params.import_with_stop_codon)
         ImportHelper.junction_to_cdr3(df, params.region_type)
         df.loc[:, "region_types"] = params.region_type.name
         ImportHelper.update_gene_info(df)
         ImportHelper.load_chains(df)
 
         return df
```

### Comparing `immuneML-2.2.4/immuneML/IO/dataset_import/IGoRImport.py` & `immuneML-2.2.5/immuneML/IO/dataset_import/IGoRImport.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
             no_stop_codon = ["*" not in seq for seq in df.sequence_aas]
             df = df[no_stop_codon]
 
         ImportHelper.junction_to_cdr3(df, params.region_type)
         df.loc[:, "region_types"] = params.region_type.name
         # note: import_empty_aa_sequences is set to true here; since IGoR doesnt output aa, this parameter is insensible
         ImportHelper.drop_empty_sequences(df, True, params.import_empty_nt_sequences)
-        ImportHelper.drop_illegal_character_sequences(df, params.import_illegal_characters)
+        ImportHelper.drop_illegal_character_sequences(df, params.import_illegal_characters, params.import_with_stop_codon)
 
         # chain or at least receptorsequence?
 
         return df
 
     @staticmethod
     def translate_sequence(nt_seq):
```

### Comparing `immuneML-2.2.4/immuneML/IO/dataset_import/IReceptorImport.py` & `immuneML-2.2.5/immuneML/IO/dataset_import/IReceptorImport.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/IO/dataset_import/ImmuneMLImport.py` & `immuneML-2.2.5/immuneML/IO/dataset_import/ImmuneMLImport.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/IO/dataset_import/ImmunoSEQRearrangementImport.py` & `immuneML-2.2.5/immuneML/IO/dataset_import/ImmunoSEQRearrangementImport.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/IO/dataset_import/ImmunoSEQSampleImport.py` & `immuneML-2.2.5/immuneML/IO/dataset_import/ImmunoSEQSampleImport.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/IO/dataset_import/MiXCRImport.py` & `immuneML-2.2.5/immuneML/IO/dataset_import/MiXCRImport.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
         df["counts"] = df["counts"].astype(float).astype(int)
 
         df["v_alleles"] = MiXCRImport._load_alleles(df, "v_alleles")
         df["j_alleles"] = MiXCRImport._load_alleles(df, "j_alleles")
 
         ImportHelper.drop_empty_sequences(df, params.import_empty_aa_sequences, params.import_empty_nt_sequences)
-        ImportHelper.drop_illegal_character_sequences(df, params.import_illegal_characters)
+        ImportHelper.drop_illegal_character_sequences(df, params.import_illegal_characters, params.import_with_stop_codon)
         ImportHelper.update_gene_info(df)
         ImportHelper.load_chains(df)
 
         return df
 
     @staticmethod
     def _load_alleles(df: pd.DataFrame, column_name):
```

### Comparing `immuneML-2.2.4/immuneML/IO/dataset_import/OLGAImport.py` & `immuneML-2.2.5/immuneML/IO/dataset_import/OLGAImport.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
         if "counts" not in df.columns:
             df["counts"] = 1
 
         df["sequence_identifiers"] = None
 
         ImportHelper.drop_empty_sequences(df, params.import_empty_aa_sequences, params.import_empty_nt_sequences)
-        ImportHelper.drop_illegal_character_sequences(df, params.import_illegal_characters)
+        ImportHelper.drop_illegal_character_sequences(df, params.import_illegal_characters, params.import_with_stop_codon)
         ImportHelper.junction_to_cdr3(df, params.region_type)
         df.loc[:, "region_types"] = params.region_type.name
         ImportHelper.update_gene_info(df)
         ImportHelper.load_chains(df)
 
         return df
```

### Comparing `immuneML-2.2.4/immuneML/IO/dataset_import/RandomReceptorDatasetImport.py` & `immuneML-2.2.5/immuneML/IO/dataset_import/RandomReceptorDatasetImport.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/IO/dataset_import/RandomRepertoireDatasetImport.py` & `immuneML-2.2.5/immuneML/IO/dataset_import/RandomRepertoireDatasetImport.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/IO/dataset_import/RandomSequenceDatasetImport.py` & `immuneML-2.2.5/immuneML/IO/dataset_import/RandomSequenceDatasetImport.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/IO/dataset_import/SingleLineReceptorImport.py` & `immuneML-2.2.5/immuneML/IO/dataset_import/SingleLineReceptorImport.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/IO/dataset_import/TenxGenomicsImport.py` & `immuneML-2.2.5/immuneML/IO/dataset_import/TenxGenomicsImport.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
             allowed_productive_values.append("False")
 
         df = df[df.productive.isin(allowed_productive_values)]
 
         ImportHelper.junction_to_cdr3(df, params.region_type)
         df.loc[:, "region_types"] = params.region_type.name
         ImportHelper.drop_empty_sequences(df, params.import_empty_aa_sequences, params.import_empty_nt_sequences)
-        ImportHelper.drop_illegal_character_sequences(df, params.import_illegal_characters)
+        ImportHelper.drop_illegal_character_sequences(df, params.import_illegal_characters, params.import_with_stop_codon)
         ImportHelper.update_gene_info(df)
         ImportHelper.load_chains(df)
 
         return df
 
     @staticmethod
     def import_receptors(df, params):
```

### Comparing `immuneML-2.2.4/immuneML/IO/dataset_import/VDJdbImport.py` & `immuneML-2.2.5/immuneML/IO/dataset_import/VDJdbImport.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                 df.drop(df.loc[df["sequence_identifiers"] == "0"].index, inplace=True)
                 warnings.warn(f"VDJdbImport: {n_single_chains} single chains were removed when trying to create a ReceptorDataset.\n"
                               f"To import all chains as a SequenceDataset, use paired = False")
         else:
             df.loc[df["sequence_identifiers"] == "0", "sequence_identifiers"] = None
 
         ImportHelper.drop_empty_sequences(df, params.import_empty_aa_sequences, params.import_empty_nt_sequences)
-        ImportHelper.drop_illegal_character_sequences(df, params.import_illegal_characters)
+        ImportHelper.drop_illegal_character_sequences(df, params.import_illegal_characters, params.import_with_stop_codon)
         ImportHelper.update_gene_info(df)
         ImportHelper.load_chains(df)
 
         df["receptor_identifiers"] = df["sequence_identifiers"]
         df["sequence_identifiers"] = VDJdbImport.get_sequence_identifiers(df["sequence_identifiers"], df["chains"])
 
         df = VDJdbImport.extract_meta_columns(df, params)
@@ -163,15 +163,15 @@
     @staticmethod
     def get_sequence_identifiers(receptor_identifiers, chains):
         sequence_identifiers = receptor_identifiers + "_" + chains
         if sequence_identifiers.is_unique:
             return sequence_identifiers
         else:
             counts = sequence_identifiers.value_counts()
-            for id, count in counts[counts > 1].iteritems():
+            for id, count in counts[counts > 1].items():
                 unique_ids = [f"{id}{i}" for i in range(1, count+1)]
                 sequence_identifiers.loc[sequence_identifiers == id] = unique_ids
         return sequence_identifiers
 
     @staticmethod
     def import_receptors(df, params):
         return ImportHelper.import_receptors(df, params)
```

### Comparing `immuneML-2.2.4/immuneML/IO/dataset_import/conversion/imgt_adaptive_conversion.csv` & `immuneML-2.2.5/immuneML/IO/dataset_import/conversion/imgt_adaptive_conversion.csv`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/IO/ml_method/MLExporter.py` & `immuneML-2.2.5/immuneML/IO/ml_method/MLExporter.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/IO/ml_method/MLImport.py` & `immuneML-2.2.5/immuneML/IO/ml_method/MLImport.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/IO/ml_method/MLMethodConfiguration.py` & `immuneML-2.2.5/immuneML/IO/ml_method/MLMethodConfiguration.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/IO/ml_method/UtilIO.py` & `immuneML-2.2.5/immuneML/IO/ml_method/UtilIO.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/analysis/SequenceMatcher.py` & `immuneML-2.2.5/immuneML/analysis/SequenceMatcher.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/analysis/criteria_matches/CriteriaMatcher.py` & `immuneML-2.2.5/immuneML/analysis/criteria_matches/CriteriaMatcher.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/analysis/criteria_matches/CriteriaTypeInstantiator.py` & `immuneML-2.2.5/immuneML/analysis/criteria_matches/CriteriaTypeInstantiator.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/analysis/data_manipulation/DataReshaper.py` & `immuneML-2.2.5/immuneML/analysis/data_manipulation/DataReshaper.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/analysis/entropy_calculations/EntropyCalculator.py` & `immuneML-2.2.5/immuneML/analysis/entropy_calculations/EntropyCalculator.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/analysis/similarities/RepertoireSimilarityComputer.py` & `immuneML-2.2.5/immuneML/analysis/similarities/RepertoireSimilarityComputer.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/api/aggregated_runs/MultiDatasetBenchmarkTool.py` & `immuneML-2.2.5/immuneML/api/aggregated_runs/MultiDatasetBenchmarkTool.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/api/api_encoding.py` & `immuneML-2.2.5/immuneML/api/api_encoding.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/api/galaxy/DataSimulationTool.py` & `immuneML-2.2.5/immuneML/api/galaxy/DataSimulationTool.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/api/galaxy/DatasetGenerationTool.py` & `immuneML-2.2.5/immuneML/api/galaxy/DatasetGenerationTool.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/api/galaxy/GalaxyMLApplicationTool.py` & `immuneML-2.2.5/immuneML/api/galaxy/GalaxyMLApplicationTool.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/api/galaxy/GalaxySimulationTool.py` & `immuneML-2.2.5/immuneML/api/galaxy/GalaxySimulationTool.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/api/galaxy/GalaxyTool.py` & `immuneML-2.2.5/immuneML/api/galaxy/GalaxyTool.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/api/galaxy/GalaxyTrainMLModel.py` & `immuneML-2.2.5/immuneML/api/galaxy/GalaxyTrainMLModel.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/api/galaxy/GalaxyYamlTool.py` & `immuneML-2.2.5/immuneML/api/galaxy/GalaxyYamlTool.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/api/galaxy/RepertoireClassificationTool.py` & `immuneML-2.2.5/immuneML/api/galaxy/RepertoireClassificationTool.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/api/galaxy/Util.py` & `immuneML-2.2.5/immuneML/api/galaxy/Util.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/api/galaxy/build_dataset_yaml.py` & `immuneML-2.2.5/immuneML/api/galaxy/build_dataset_yaml.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/api/galaxy/build_yaml_from_arguments.py` & `immuneML-2.2.5/immuneML/api/galaxy/build_yaml_from_arguments.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/app/ImmuneMLApp.py` & `immuneML-2.2.5/immuneML/app/ImmuneMLApp.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/caching/CacheHandler.py` & `immuneML-2.2.5/immuneML/caching/CacheHandler.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/config/default_params/datasets/airr_params.yaml` & `immuneML-2.2.5/immuneML/config/default_params/datasets/airr_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/config/default_params/datasets/i_receptor_params.yaml` & `immuneML-2.2.5/immuneML/config/default_params/datasets/i_receptor_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/config/default_params/datasets/igor_params.yaml` & `immuneML-2.2.5/immuneML/config/default_params/datasets/igor_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/config/default_params/datasets/immuno_seq_rearrangement_params.yaml` & `immuneML-2.2.5/immuneML/config/default_params/datasets/immuno_seq_rearrangement_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/config/default_params/datasets/immuno_seq_sample_params.yaml` & `immuneML-2.2.5/immuneML/config/default_params/datasets/immuno_seq_sample_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/config/default_params/datasets/mixcr_params.yaml` & `immuneML-2.2.5/immuneML/config/default_params/datasets/mixcr_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/config/default_params/datasets/olga_params.yaml` & `immuneML-2.2.5/immuneML/config/default_params/datasets/olga_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/config/default_params/datasets/random_repertoire_dataset_params.yaml` & `immuneML-2.2.5/immuneML/config/default_params/datasets/random_repertoire_dataset_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/config/default_params/datasets/tenx_genomics_params.yaml` & `immuneML-2.2.5/immuneML/config/default_params/datasets/tenx_genomics_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/config/default_params/datasets/vdjdb_params.yaml` & `immuneML-2.2.5/immuneML/config/default_params/datasets/vdjdb_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/config/default_params/encodings/kmer_frequency_params.yaml` & `immuneML-2.2.5/immuneML/config/default_params/encodings/kmer_frequency_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/config/default_params/instructions/train_ml_model_params.yaml` & `immuneML-2.2.5/immuneML/config/default_params/instructions/train_ml_model_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/config/default_params/ml_methods/deep_rc_params.yaml` & `immuneML-2.2.5/immuneML/config/default_params/ml_methods/deep_rc_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/data_model/cell/CellList.py` & `immuneML-2.2.5/immuneML/data_model/cell/CellList.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/data_model/dataset/Dataset.py` & `immuneML-2.2.5/immuneML/data_model/dataset/Dataset.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/data_model/dataset/ElementDataset.py` & `immuneML-2.2.5/immuneML/data_model/dataset/ElementDataset.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/data_model/dataset/ReceptorDataset.py` & `immuneML-2.2.5/immuneML/data_model/dataset/ReceptorDataset.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/data_model/dataset/RepertoireDataset.py` & `immuneML-2.2.5/immuneML/data_model/dataset/RepertoireDataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,19 +6,35 @@
 import pandas as pd
 
 from immuneML.data_model.dataset.Dataset import Dataset
 from immuneML.data_model.encoded_data.EncodedData import EncodedData
 from immuneML.data_model.repertoire.Repertoire import Repertoire
 from immuneML.environment.Constants import Constants
 from immuneML.util.ParameterValidator import ParameterValidator
+from immuneML.util.PathBuilder import PathBuilder
 
 
 class RepertoireDataset(Dataset):
 
     @classmethod
+    def build_from_objects(cls, **kwargs):
+        ParameterValidator.assert_keys_present(list(kwargs.keys()), ['repertoires', 'path'], RepertoireDataset.__name__, RepertoireDataset.__name__)
+        ParameterValidator.assert_all_type_and_value(kwargs['repertoires'], Repertoire, RepertoireDataset.__name__, 'repertoires')
+
+        metadata_df = pd.DataFrame.from_records([{**rep.metadata, **{'filename': rep.data_filename}} for rep in kwargs['repertoires']])
+
+        if 'field_list' in metadata_df.columns:
+            metadata_df.drop(columns=['field_list'], inplace=True)
+
+        metadata_path = PathBuilder.build(kwargs['path']) / 'metadata.csv'
+        metadata_df.to_csv(metadata_path, index=False)
+
+        return RepertoireDataset(repertoires=kwargs['repertoires'], metadata_file=metadata_path)
+
+    @classmethod
     def build(cls, **kwargs):
         ParameterValidator.assert_keys_present(list(kwargs.keys()), ['metadata_file', 'name', 'repertoire_ids', 'metadata_fields'],
                                                RepertoireDataset.__name__, "repertoire dataset")
         repertoires = []
         metadata_df = pd.read_csv(kwargs['metadata_file'], comment=Constants.COMMENT_SIGN)
         for index, row in metadata_df.iterrows():
             filename = Path(kwargs['metadata_file']).parent / row['filename']
```

### Comparing `immuneML-2.2.4/immuneML/data_model/dataset/SequenceDataset.py` & `immuneML-2.2.5/immuneML/data_model/dataset/SequenceDataset.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/data_model/encoded_data/EncodedData.py` & `immuneML-2.2.5/immuneML/data_model/encoded_data/EncodedData.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/data_model/receptor/BCKReceptor.py` & `immuneML-2.2.5/immuneML/data_model/receptor/BCKReceptor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-from uuid import uuid4
 
 from immuneML.data_model.receptor.Receptor import Receptor
 from immuneML.data_model.receptor.receptor_sequence.ReceptorSequence import ReceptorSequence
 
 
 class BCKReceptor(Receptor):
     FIELDS = {'heavy': object, 'kappa': object, 'identifier': str, 'metadata': dict, 'version': str}
@@ -30,13 +29,13 @@
     @classmethod
     def get_record_names(cls):
         return ['heavy_' + name for name in ReceptorSequence.get_record_names()] \
                + ['kappa_' + name for name in ReceptorSequence.get_record_names()] \
                + [name for name in cls.FIELDS if name not in ['heavy', 'kappa']]
 
     def __init__(self, heavy: ReceptorSequence = None, kappa: ReceptorSequence = None, metadata: dict = None, identifier: str = None):
-        super().__init__(metadata, identifier)
+        super().__init__(metadata=metadata, identifier=identifier)
         self.heavy = heavy
         self.kappa = kappa
 
     def get_chains(self):
         return ["heavy", "kappa"]
```

### Comparing `immuneML-2.2.4/immuneML/data_model/receptor/BCReceptor.py` & `immuneML-2.2.5/immuneML/data_model/receptor/BCReceptor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-from uuid import uuid4
 
 from immuneML.data_model.receptor.Receptor import Receptor
 from immuneML.data_model.receptor.receptor_sequence.ReceptorSequence import ReceptorSequence
 
 
 class BCReceptor(Receptor):
     FIELDS = {'heavy': object, 'light': object, 'identifier': str, 'metadata': dict, 'version': str}
@@ -30,13 +29,13 @@
     def get_record_names(cls):
         return ['heavy_' + name for name in ReceptorSequence.get_record_names()] \
                + ['light_' + name for name in ReceptorSequence.get_record_names()] \
                + [name for name in cls.FIELDS if name not in ['heavy', 'light']]
 
     def __init__(self, heavy: ReceptorSequence = None, light: ReceptorSequence = None, metadata: dict = None,
                  identifier: str = None):
-        super().__init__(metadata, identifier)
+        super().__init__(metadata=metadata, identifier=identifier)
         self.heavy = heavy
         self.light = light
 
     def get_chains(self):
         return ["heavy", "light"]
```

### Comparing `immuneML-2.2.4/immuneML/data_model/receptor/ChainPair.py` & `immuneML-2.2.5/immuneML/data_model/receptor/ChainPair.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/data_model/receptor/ElementGenerator.py` & `immuneML-2.2.5/immuneML/data_model/receptor/ElementGenerator.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/data_model/receptor/Receptor.py` & `immuneML-2.2.5/immuneML/data_model/receptor/Receptor.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/data_model/receptor/ReceptorBuilder.py` & `immuneML-2.2.5/immuneML/data_model/receptor/ReceptorBuilder.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from immuneML.data_model.receptor.BCKReceptor import BCKReceptor
 from immuneML.data_model.receptor.BCReceptor import BCReceptor
 from immuneML.data_model.receptor.ChainPair import ChainPair
 from immuneML.data_model.receptor.Receptor import Receptor
 from immuneML.data_model.receptor.TCABReceptor import TCABReceptor
 from immuneML.data_model.receptor.TCGDReceptor import TCGDReceptor
 from immuneML.data_model.receptor.receptor_sequence.Chain import Chain
-from immuneML.data_model.receptor.receptor_sequence.ReceptorSequenceList import ReceptorSequenceList
+from immuneML.data_model.receptor.receptor_sequence.ReceptorSequence import ReceptorSequence
 
 
 class ReceptorBuilder:
 
     @classmethod
     def build_object(cls, sequences: dict, identifier: str = None, metadata: dict = None) -> Receptor:
         if all(chain in ChainPair.TRA_TRB.value for chain in sequences.keys()):
@@ -25,15 +25,15 @@
         elif all(chain in ChainPair.IGH_IGK.value for chain in sequences.keys()):
             return BCKReceptor(heavy=sequences[Chain.HEAVY.value], kappa=sequences[Chain.KAPPA.value], identifier=identifier, metadata=metadata)
         else:
             warnings.warn(f"ReceptorBuilder: attempt to build_from_objects receptor with chains {sequences.keys()}, returning None...")
             return None
 
     @classmethod
-    def build_objects(cls, sequences: ReceptorSequenceList) -> List[Receptor]:
+    def build_objects(cls, sequences: List[ReceptorSequence]) -> List[Receptor]:
         receptors = []
         sequences_per_chain = {chain.value: [sequence for sequence in sequences if sequence.metadata.chain.value == chain.value]
                                for chain in Chain}
         for chain_pair in ChainPair:
             all_chain_1 = sequences_per_chain[chain_pair.value[0]]
             all_chain_2 = sequences_per_chain[chain_pair.value[1]]
             combinations = list(itertools.product(all_chain_1, all_chain_2))
```

### Comparing `immuneML-2.2.4/immuneML/data_model/receptor/TCABReceptor.py` & `immuneML-2.2.5/immuneML/data_model/receptor/TCABReceptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-from uuid import uuid4
 
 import numpy as np
 
 from immuneML.data_model.receptor.Receptor import Receptor
 from immuneML.data_model.receptor.receptor_sequence.ReceptorSequence import ReceptorSequence
 
 
@@ -25,15 +24,15 @@
             return TCABReceptor(alpha=ReceptorSequence.create_from_record(alpha_record),
                                 beta=ReceptorSequence.create_from_record(beta_record),
                                 identifier=record['identifier'], metadata=metadata)
         else:
             raise NotImplementedError(f"Supported ({TCABReceptor.version}) and available version differ, but there is no converter available.")
 
     def __init__(self, alpha: ReceptorSequence = None, beta: ReceptorSequence = None, metadata: dict = None, identifier: str = None):
-        super().__init__(metadata, identifier)
+        super().__init__(metadata=metadata, identifier=identifier)
         self.alpha = alpha
         self.beta = beta
 
     @classmethod
     def get_record_names(cls):
         return ['alpha_' + name for name in ReceptorSequence.get_record_names()] \
                + ['beta_' + name for name in ReceptorSequence.get_record_names()] \
```

### Comparing `immuneML-2.2.4/immuneML/data_model/receptor/TCGDReceptor.py` & `immuneML-2.2.5/immuneML/data_model/receptor/TCGDReceptor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-from uuid import uuid4
 
 import numpy as np
 
 from immuneML.data_model.receptor.Receptor import Receptor
 from immuneML.data_model.receptor.receptor_sequence.ReceptorSequence import ReceptorSequence
 
 
@@ -31,13 +30,13 @@
     @classmethod
     def get_record_names(cls):
         return ['gamma_' + name for name in ReceptorSequence.get_record_names()] \
                + ['delta_' + name for name in ReceptorSequence.get_record_names()] \
                + [name for name in cls.FIELDS if name not in ['gamma', 'delta']]
 
     def __init__(self, gamma: ReceptorSequence = None, delta: ReceptorSequence = None, metadata: dict = None, identifier: str = None):
-        super().__init__(metadata, identifier)
+        super().__init__(metadata=metadata, identifier=identifier)
         self.gamma = gamma
         self.delta = delta
 
     def get_chains(self):
         return ["gamma", "delta"]
```

### Comparing `immuneML-2.2.4/immuneML/data_model/receptor/receptor_sequence/Chain.py` & `immuneML-2.2.5/immuneML/data_model/receptor/receptor_sequence/Chain.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/data_model/receptor/receptor_sequence/ReceptorSequence.py` & `immuneML-2.2.5/immuneML/data_model/receptor/receptor_sequence/ReceptorSequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # quality: gold
 import json
+from uuid import uuid4
 
 import numpy as np
 
 from immuneML.data_model.DatasetItem import DatasetItem
 from immuneML.data_model.receptor.receptor_sequence.SequenceAnnotation import SequenceAnnotation
 from immuneML.data_model.receptor.receptor_sequence.SequenceMetadata import SequenceMetadata
 from immuneML.environment.EnvironmentSettings import EnvironmentSettings
@@ -31,20 +32,20 @@
         return [key for key in cls.FIELDS]
 
     def __init__(self,
                  amino_acid_sequence: str = None,
                  nucleotide_sequence: str = None,
                  identifier: str = None,
                  annotation: SequenceAnnotation = None,
-                 metadata: SequenceMetadata = SequenceMetadata()):
-        self.identifier = identifier
+                 metadata: SequenceMetadata = None):
+        self.identifier = identifier if identifier is not None and identifier != "" else uuid4().hex
         self.amino_acid_sequence = amino_acid_sequence
         self.nucleotide_sequence = nucleotide_sequence
         self.annotation = annotation
-        self.metadata = metadata
+        self.metadata = metadata if metadata is not None else SequenceMetadata()
 
     def __repr__(self):
         return f"ReceptorSequence(sequence_aa={self.amino_acid_sequence}, sequence={self.nucleotide_sequence}, " \
                f"annotation={vars(self.annotation) if self.annotation is not None else '{}'}, " \
                f"metadata={vars(self.metadata) if self.metadata is not None else '{}'})"
 
     def set_metadata(self, metadata: SequenceMetadata):
```

### Comparing `immuneML-2.2.4/immuneML/data_model/receptor/receptor_sequence/ReceptorSequenceList.py` & `immuneML-2.2.5/immuneML/reports/ml_reports/CoefficientPlottingSettingList.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from collections.abc import MutableSequence
 
-from immuneML.data_model.receptor.receptor_sequence.ReceptorSequence import ReceptorSequence
+from immuneML.reports.ml_reports.CoefficientPlottingSetting import CoefficientPlottingSetting
 from immuneML.util.ParameterValidator import ParameterValidator
 
 
-class ReceptorSequenceList(MutableSequence):
+class CoefficientPlottingSettingList(MutableSequence):
 
     def __init__(self):
         self.list = list()
 
     def check(self, v):
-        ParameterValidator.assert_type_and_value(v, ReceptorSequence, "ReceptorSequenceList", "new item")
+        ParameterValidator.assert_type_and_value(v, CoefficientPlottingSetting, "CoefficientPlottingSettingList", "new item")
 
     def __len__(self): return len(self.list)
 
     def __getitem__(self, i): return self.list[i]
 
     def __delitem__(self, i): del self.list[i]
 
@@ -23,8 +23,8 @@
         self.list[i] = v
 
     def insert(self, i, v):
         self.check(v)
         self.list.insert(i, v)
 
     def __str__(self):
-        return str(self.list)
+        return str(self.list)
```

### Comparing `immuneML-2.2.4/immuneML/data_model/receptor/receptor_sequence/SequenceAnnotation.py` & `immuneML-2.2.5/immuneML/data_model/receptor/receptor_sequence/SequenceAnnotation.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/data_model/receptor/receptor_sequence/SequenceMetadata.py` & `immuneML-2.2.5/immuneML/data_model/receptor/receptor_sequence/SequenceMetadata.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/data_model/repertoire/Repertoire.py` & `immuneML-2.2.5/immuneML/data_model/repertoire/Repertoire.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from immuneML.data_model.cell.Cell import Cell
 from immuneML.data_model.cell.CellList import CellList
 from immuneML.data_model.receptor.Receptor import Receptor
 from immuneML.data_model.receptor.ReceptorBuilder import ReceptorBuilder
 from immuneML.data_model.receptor.RegionType import RegionType
 from immuneML.data_model.receptor.receptor_sequence.Chain import Chain
 from immuneML.data_model.receptor.receptor_sequence.ReceptorSequence import ReceptorSequence
-from immuneML.data_model.receptor.receptor_sequence.ReceptorSequenceList import ReceptorSequenceList
 from immuneML.data_model.receptor.receptor_sequence.SequenceAnnotation import SequenceAnnotation
 from immuneML.data_model.receptor.receptor_sequence.SequenceMetadata import SequenceMetadata
 from immuneML.environment.EnvironmentSettings import EnvironmentSettings
 from immuneML.simulation.implants.ImplantAnnotation import ImplantAnnotation
 from immuneML.util.NumpyHelper import NumpyHelper
 from immuneML.util.PathBuilder import PathBuilder
 
@@ -108,32 +107,29 @@
             yaml.dump(metadata, file)
 
         repertoire = Repertoire(data_filename, metadata_filename, identifier)
         return repertoire
 
     @classmethod
     def build_like(cls, repertoire, indices_to_keep: list, result_path: Path, filename_base: str = None):
-        if indices_to_keep is not None and len(indices_to_keep) > 0:
-            PathBuilder.build(result_path)
+        PathBuilder.build(result_path)
 
-            data = repertoire.load_data()
-            data = data[indices_to_keep]
-            identifier = uuid4().hex
-            filename_base = filename_base if filename_base is not None else identifier
+        data = repertoire.load_data()
+        data = data[indices_to_keep]
+        identifier = uuid4().hex
+        filename_base = filename_base if filename_base is not None else identifier
 
-            data_filename = result_path / f"{filename_base}.npy"
-            np.save(str(data_filename), data)
+        data_filename = result_path / f"{filename_base}.npy"
+        np.save(str(data_filename), data)
 
-            metadata_filename = result_path / f"{filename_base}_metadata.yaml"
-            shutil.copyfile(repertoire.metadata_filename, metadata_filename)
+        metadata_filename = result_path / f"{filename_base}_metadata.yaml"
+        shutil.copyfile(repertoire.metadata_filename, metadata_filename)
 
-            new_repertoire = Repertoire(data_filename, metadata_filename, identifier)
-            return new_repertoire
-        else:
-            return None
+        new_repertoire = Repertoire(data_filename, metadata_filename, identifier)
+        return new_repertoire
 
     @classmethod
     def build_from_sequence_objects(cls, sequence_objects: list, path: Path, metadata: dict, filename_base: str = None):
 
         assert all(isinstance(sequence, ReceptorSequence) for sequence in sequence_objects), \
             "Repertoire: all sequences have to be instances of ReceptorSequence class."
 
@@ -237,18 +233,23 @@
             if attribute in data.dtype.names:
                 result[attribute] = data[attribute]
             else:
                 logging.warning(f"{Repertoire.__name__}: attribute {attribute} is not present in the repertoire {self.identifier}, skipping...")
         return result
 
     def get_region_type(self):
-        region_types = set(self.get_attribute("region_types"))
-        assert len(region_types) == 1, f"Repertoire: expected one region_type, found: {region_types}"
+        region_types = self.get_attribute("region_types")
+        if region_types is not None:
+            region_types = set(region_types)
+            assert len(region_types) == 1, f"Repertoire {self.identifier}: expected one region_type, found: {region_types}"
 
-        return RegionType(region_types.pop())
+            return RegionType(region_types.pop())
+        else:
+            logging.warning(f'Repertoire {self.identifier}: region_types are not set for sequences.')
+            return None
 
     def free_memory(self):
         self.data = None
 
     def __getstate__(self):
         state = self.__dict__.copy()
         del state['data']
@@ -305,15 +306,15 @@
             f"Repertoire: cannot return receptor objects in repertoire {self.identifier} since cell_ids are not specified. " \
             f"Existing fields are: {str(data.dtype.names)[1:-1]}"
 
         same_cell_lists = NumpyHelper.group_structured_array_by(data, "cell_ids")
         return same_cell_lists
 
     def _make_receptors(self, cell_content):
-        sequences = ReceptorSequenceList()
+        sequences = []
         for item in cell_content:
             sequences.append(self._make_sequence_object(item))
         return ReceptorBuilder.build_objects(sequences)
 
     def get_sequence_objects(self, load_implants: bool = True) -> List[ReceptorSequence]:
         """
         Lazily loads sequences from disk to reduce RAM consumption
```

### Comparing `immuneML-2.2.4/immuneML/dev_util/util.py` & `immuneML-2.2.5/immuneML/dev_util/util.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/dsl/DefaultParamsLoader.py` & `immuneML-2.2.5/immuneML/dsl/DefaultParamsLoader.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/dsl/ImmuneMLParser.py` & `immuneML-2.2.5/immuneML/dsl/ImmuneMLParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/dsl/InstructionParser.py` & `immuneML-2.2.5/immuneML/dsl/InstructionParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/dsl/ObjectParser.py` & `immuneML-2.2.5/immuneML/dsl/ObjectParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/dsl/OutputParser.py` & `immuneML-2.2.5/immuneML/dsl/OutputParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/dsl/definition_parsers/DefinitionParser.py` & `immuneML-2.2.5/immuneML/dsl/definition_parsers/DefinitionParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/dsl/definition_parsers/DefinitionParserOutput.py` & `immuneML-2.2.5/immuneML/dsl/definition_parsers/DefinitionParserOutput.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/dsl/definition_parsers/EncodingParser.py` & `immuneML-2.2.5/immuneML/dsl/definition_parsers/EncodingParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/dsl/definition_parsers/MLParser.py` & `immuneML-2.2.5/immuneML/dsl/definition_parsers/MLParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/dsl/definition_parsers/MotifParser.py` & `immuneML-2.2.5/immuneML/dsl/definition_parsers/MotifParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/dsl/definition_parsers/PreprocessingParser.py` & `immuneML-2.2.5/immuneML/dsl/definition_parsers/PreprocessingParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/dsl/definition_parsers/ReportParser.py` & `immuneML-2.2.5/immuneML/dsl/definition_parsers/ReportParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/dsl/definition_parsers/SignalParser.py` & `immuneML-2.2.5/immuneML/dsl/definition_parsers/SignalParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/dsl/definition_parsers/SimulationParser.py` & `immuneML-2.2.5/immuneML/dsl/definition_parsers/SimulationParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/dsl/import_parsers/ImportParser.py` & `immuneML-2.2.5/immuneML/dsl/import_parsers/ImportParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/dsl/instruction_parsers/DatasetExportParser.py` & `immuneML-2.2.5/immuneML/dsl/instruction_parsers/DatasetExportParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/dsl/instruction_parsers/ExploratoryAnalysisParser.py` & `immuneML-2.2.5/immuneML/dsl/instruction_parsers/ExploratoryAnalysisParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/dsl/instruction_parsers/LabelHelper.py` & `immuneML-2.2.5/immuneML/dsl/instruction_parsers/LabelHelper.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/dsl/instruction_parsers/MLApplicationParser.py` & `immuneML-2.2.5/immuneML/dsl/instruction_parsers/MLApplicationParser.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from immuneML.IO.ml_method.MLImport import MLImport
 from immuneML.dsl.symbol_table.SymbolTable import SymbolTable
 from immuneML.dsl.symbol_table.SymbolType import SymbolType
 from immuneML.environment.Label import Label
 from immuneML.environment.LabelConfiguration import LabelConfiguration
 from immuneML.hyperparameter_optimization.HPSetting import HPSetting
+from immuneML.ml_metrics.Metric import Metric
 from immuneML.util.ParameterValidator import ParameterValidator
 from immuneML.util.PathBuilder import PathBuilder
 from immuneML.workflows.instructions.ml_model_application.MLApplicationInstruction import MLApplicationInstruction
 
 
 class MLApplicationParser:
     """
@@ -21,30 +22,42 @@
     .. highlight:: yaml
     .. code-block:: yaml
 
         instruction_name:
             type: MLApplication
             dataset: d1
             config_path: ./config.zip
+            metrics:
+            - accuracy
+            - precision
+            - recall
             number_of_processes: 4
-            label: CD
 
     """
 
     def parse(self, key: str, instruction: dict, symbol_table: SymbolTable, path: Path) -> MLApplicationInstruction:
         location = MLApplicationParser.__name__
-        ParameterValidator.assert_keys(instruction.keys(), ['type', 'dataset', 'number_of_processes', 'config_path'], location, key)
+        ParameterValidator.assert_keys(instruction.keys(), ['type', 'dataset', 'number_of_processes', 'config_path', 'metrics'], location, key)
         ParameterValidator.assert_in_valid_list(instruction['dataset'], symbol_table.get_keys_by_type(SymbolType.DATASET), location, f"{key}: dataset")
         ParameterValidator.assert_type_and_value(instruction['number_of_processes'], int, location, f"{key}: number_of_processes", min_inclusive=1)
         ParameterValidator.assert_type_and_value(instruction['config_path'], str, location, f'{key}: config_path')
 
+        if 'metrics' in instruction and instruction['metrics'] is not None:
+            ParameterValidator.assert_type_and_value(instruction['metrics'], list, location, f'{key}: metrics')
+            metrics = [Metric.get_metric(metric) for metric in instruction["metrics"]]
+        else:
+            metrics = []
+
         hp_setting, label = self._parse_hp_setting(instruction, path, key)
 
-        instruction = MLApplicationInstruction(dataset=symbol_table.get(instruction['dataset']), name=key, number_of_processes=instruction['number_of_processes'],
-                                               label_configuration=LabelConfiguration([label]), hp_setting=hp_setting)
+        instruction = MLApplicationInstruction(dataset=symbol_table.get(instruction['dataset']), name=key,
+                                               number_of_processes=instruction['number_of_processes'],
+                                               label_configuration=LabelConfiguration([label]),
+                                               hp_setting=hp_setting,
+                                               metrics=metrics)
 
         return instruction
 
     def _parse_hp_setting(self, instruction: dict, path: Path, key: str) -> Tuple[HPSetting, Label]:
 
         assert os.path.isfile(instruction['config_path']), f'MLApplicationParser: {instruction["config_path"]} is not file path.'
         assert '.zip' in instruction['config_path'], f'MLApplicationParser: {instruction["config_path"]} is not a zip file.'
```

### Comparing `immuneML-2.2.4/immuneML/dsl/instruction_parsers/SimulationParser.py` & `immuneML-2.2.5/immuneML/dsl/instruction_parsers/SimulationParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/dsl/instruction_parsers/SubsamplingParser.py` & `immuneML-2.2.5/immuneML/dsl/instruction_parsers/SubsamplingParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/dsl/instruction_parsers/TrainMLModelParser.py` & `immuneML-2.2.5/immuneML/dsl/instruction_parsers/TrainMLModelParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/dsl/semantic_model/SemanticModel.py` & `immuneML-2.2.5/immuneML/dsl/semantic_model/SemanticModel.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/dsl/symbol_table/SymbolTable.py` & `immuneML-2.2.5/immuneML/dsl/symbol_table/SymbolTable.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/DatasetEncoder.py` & `immuneML-2.2.5/immuneML/encodings/DatasetEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/abundance_encoding/AbundanceEncoderHelper.py` & `immuneML-2.2.5/immuneML/encodings/abundance_encoding/AbundanceEncoderHelper.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/abundance_encoding/CompAIRRBatchIterator.py` & `immuneML-2.2.5/immuneML/encodings/abundance_encoding/CompAIRRBatchIterator.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/abundance_encoding/CompAIRRSequenceAbundanceEncoder.py` & `immuneML-2.2.5/immuneML/encodings/abundance_encoding/CompAIRRSequenceAbundanceEncoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import numpy as np
 import pandas as pd
 
 from immuneML.caching.CacheHandler import CacheHandler
 from immuneML.data_model.dataset.RepertoireDataset import RepertoireDataset
 from immuneML.data_model.encoded_data.EncodedData import EncodedData
+from immuneML.data_model.receptor.RegionType import RegionType
 from immuneML.encodings.DatasetEncoder import DatasetEncoder
 from immuneML.encodings.EncoderParams import EncoderParams
 from immuneML.encodings.abundance_encoding.AbundanceEncoderHelper import AbundanceEncoderHelper
 from immuneML.encodings.abundance_encoding.CompAIRRBatchIterator import CompAIRRBatchIterator
 from immuneML.environment.EnvironmentSettings import EnvironmentSettings
 from immuneML.environment.SequenceType import SequenceType
 from immuneML.util.CompAIRRHelper import CompAIRRHelper
@@ -63,15 +64,15 @@
         sequence_batch_size (int): The number of sequences in a batch when comparing sequences across repertoires, typically 100s of thousands.
         This does not affect the results of the encoding, but may affect the speed and memory usage. The default value is 1.000.000
 
         threads (int): The number of threads to use for parallelization. This does not affect the results of the encoding, only the speed.
         The default number of threads is 8.
 
         keep_temporary_files (bool): whether to keep temporary files, including CompAIRR input, output and log files, and the sequence
-        presence matrix. This may take a lot of storage space if the input dataset is large. By default temporary files are not kept.
+        presence matrix. This may take a lot of storage space if the input dataset is large. By default, temporary files are not kept.
 
 
     YAML specification:
 
     .. indent with spaces
     .. code-block:: yaml
 
@@ -100,23 +101,19 @@
         self.relevant_indices_path = None
         self.relevant_sequence_path = None
         self.contingency_table_path = None
         self.p_values_path = None
         self.context = None
         self.compairr_sequence_presence = None
 
-        self.compairr_params = CompAIRRParams(compairr_path=Path(compairr_path),
-                                              keep_compairr_input=True,
-                                              differences=0,
-                                              indels=False,
-                                              ignore_counts=True,
-                                              ignore_genes=ignore_genes,
-                                              threads=threads,
-                                              output_filename=None,
-                                              log_filename=None)
+        self.compairr_params = CompAIRRParams(compairr_path=Path(compairr_path), keep_compairr_input=True,
+                                              differences=0, indels=False,
+                                              ignore_counts=True, ignore_genes=ignore_genes,
+                                              threads=threads, output_filename=None,
+                                              log_filename=None, output_pairs=False, pairs_filename=None)
 
     @staticmethod
     def _prepare_parameters(p_value_threshold: float, compairr_path: str, sequence_batch_size: int, ignore_genes: bool, keep_temporary_files: bool,  threads: int,
                             name: str = None):
         ParameterValidator.assert_type_and_value(p_value_threshold, float, "CompAIRRSequenceAbundanceEncoder", "p_value_threshold", min_inclusive=0,
                                                  max_inclusive=1)
         ParameterValidator.assert_type_and_value(sequence_batch_size, int, "CompAIRRSequenceAbundanceEncoder", "sequence_batch_size", min_inclusive=1)
@@ -140,14 +137,16 @@
     def build_object(dataset, **params):
         assert isinstance(dataset, RepertoireDataset), "CompAIRRSequenceAbundanceEncoder: this encoding only works on repertoire datasets."
         prepared_params = CompAIRRSequenceAbundanceEncoder._prepare_parameters(**params)
         return CompAIRRSequenceAbundanceEncoder(**prepared_params)
 
     def encode(self, dataset, params: EncoderParams):
         AbundanceEncoderHelper.check_labels(params.label_config, CompAIRRSequenceAbundanceEncoder.__name__)
+        self.compairr_params.is_cdr3 = dataset.repertoires[0].get_region_type() == RegionType.IMGT_CDR3
+
         self.compairr_sequence_presence = self._prepare_sequence_presence_data(dataset, params)
 
         return self._encode_data(dataset, params)
 
     def _prepare_sequence_presence_data(self, dataset, params):
         full_dataset = EncoderHelper.get_current_dataset(dataset, self.context)
 
@@ -223,27 +222,29 @@
             subset_end_index = min(self.sequence_batch_size, len(full_sequence_set))
 
             for file_index in range(n_sequence_files):
                 filename = result_path / f"compairr_sequences_batch{file_index}.tsv"
                 self.sequences_filepaths.append(filename)
                 sequence_subset = full_sequence_set[subset_start_index:subset_end_index]
 
-                self.write_sequence_set_file(sequence_subset, filename, offset=subset_start_index)
+                self.write_sequence_set_file(sequence_subset, filename, offset=subset_start_index, region_type=dataset.repertoires[0].get_region_type())
 
                 subset_start_index += self.sequence_batch_size
                 subset_end_index = min(subset_end_index + self.sequence_batch_size, len(full_sequence_set))
 
     def _remove_temporary_files(self, result_path):
         self.repertoires_filepath.unlink()
 
         for file in self.sequences_filepaths:
             file.unlink()
 
-    def write_sequence_set_file(self, sequence_set, filename, offset=0):
-        sequence_col = "junction_aa" if EnvironmentSettings.get_sequence_type() == SequenceType.AMINO_ACID else "junction"
+    def write_sequence_set_file(self, sequence_set, filename, offset=0, region_type=RegionType.IMGT_JUNCTION):
+        sequence_col = 'junction' if region_type == RegionType.IMGT_JUNCTION else 'cdr3'
+        if EnvironmentSettings.get_sequence_type() == SequenceType.AMINO_ACID:
+            sequence_col = f"{sequence_col}_aa"
         vj_header = "" if self.compairr_params.ignore_genes else "\tv_call\tj_call"
 
         with open(filename, "w") as file:
             file.write(f"{sequence_col}{vj_header}\tduplicate_count\trepertoire_id\n")
 
             for id, sequence_info in enumerate(sequence_set, offset):
                 file.write("\t".join(sequence_info) + f"\t1\t{id}\n")
```

### Comparing `immuneML-2.2.4/immuneML/encodings/abundance_encoding/KmerAbundanceEncoder.py` & `immuneML-2.2.5/immuneML/encodings/abundance_encoding/KmerAbundanceEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/abundance_encoding/SequenceAbundanceEncoder.py` & `immuneML-2.2.5/immuneML/encodings/abundance_encoding/SequenceAbundanceEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/atchley_kmer_encoding/AtchleyKmerEncoder.py` & `immuneML-2.2.5/immuneML/encodings/atchley_kmer_encoding/AtchleyKmerEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/atchley_kmer_encoding/Util.py` & `immuneML-2.2.5/immuneML/encodings/atchley_kmer_encoding/Util.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/atchley_kmer_encoding/atchley_factors.csv` & `immuneML-2.2.5/immuneML/encodings/atchley_kmer_encoding/atchley_factors.csv`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/deeprc/DeepRCEncoder.py` & `immuneML-2.2.5/immuneML/encodings/deeprc/DeepRCEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/distance_encoding/CompAIRRDistanceEncoder.py` & `immuneML-2.2.5/immuneML/encodings/distance_encoding/CompAIRRDistanceEncoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from tempfile import NamedTemporaryFile
 
 import numpy as np
 import pandas as pd
 
 from immuneML.data_model.dataset.RepertoireDataset import RepertoireDataset
 from immuneML.data_model.encoded_data.EncodedData import EncodedData
+from immuneML.data_model.receptor.RegionType import RegionType
 from immuneML.encodings.DatasetEncoder import DatasetEncoder
 from immuneML.encodings.EncoderParams import EncoderParams
 from immuneML.util.CompAIRRHelper import CompAIRRHelper
 from immuneML.util.CompAIRRParams import CompAIRRParams
 from immuneML.util.EncoderHelper import EncoderHelper
 from immuneML.util.ParameterValidator import ParameterValidator
 
@@ -78,15 +79,15 @@
                                               keep_compairr_input=keep_compairr_input,
                                               differences=differences,
                                               indels=indels,
                                               ignore_counts=ignore_counts,
                                               ignore_genes=ignore_genes,
                                               threads=threads,
                                               output_filename=CompAIRRDistanceEncoder.OUTPUT_FILENAME,
-                                              log_filename=CompAIRRDistanceEncoder.LOG_FILENAME)
+                                              log_filename=CompAIRRDistanceEncoder.LOG_FILENAME, output_pairs=False, pairs_filename=None)
 
         self.context = context
         self.name = name
 
     def set_context(self, context: dict):
         self.context = context
         return self
@@ -195,14 +196,15 @@
                 raw_distance_matrix, repertoire_sizes, repertoire_indices = self._run_compairr(dataset, params, tmp.name)
 
         return raw_distance_matrix, repertoire_sizes, repertoire_indices
 
     def _run_compairr(self, dataset, params, filename):
         repertoire_sizes, repertoire_indices = self._prepare_repertoire_file(dataset, filename)
 
+        self.compairr_params.is_cdr3 = dataset.repertoires[0].get_region_type() == RegionType.IMGT_CDR3
         args = CompAIRRHelper.get_cmd_args(self.compairr_params, [filename], params.result_path)
         compairr_result = subprocess.run(args, capture_output=True, text=True)
 
         raw_distance_matrix = CompAIRRHelper.process_compairr_output_file(compairr_result, self.compairr_params, params.result_path)
 
         return raw_distance_matrix, repertoire_sizes, repertoire_indices
```

### Comparing `immuneML-2.2.4/immuneML/encodings/distance_encoding/DistanceEncoder.py` & `immuneML-2.2.5/immuneML/encodings/distance_encoding/DistanceEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/distance_encoding/TCRdistEncoder.py` & `immuneML-2.2.5/immuneML/encodings/distance_encoding/TCRdistEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/evenness_profile/EvennessProfileEncoder.py` & `immuneML-2.2.5/immuneML/encodings/evenness_profile/EvennessProfileEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/evenness_profile/EvennessProfileRepertoireEncoder.py` & `immuneML-2.2.5/immuneML/encodings/evenness_profile/EvennessProfileRepertoireEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/kmer_frequency/KmerFreqReceptorEncoder.py` & `immuneML-2.2.5/immuneML/encodings/kmer_frequency/KmerFreqReceptorEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/kmer_frequency/KmerFreqRepertoireEncoder.py` & `immuneML-2.2.5/immuneML/encodings/kmer_frequency/KmerFreqRepertoireEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/kmer_frequency/KmerFreqSequenceEncoder.py` & `immuneML-2.2.5/immuneML/encodings/kmer_frequency/KmerFreqSequenceEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/kmer_frequency/KmerFrequencyEncoder.py` & `immuneML-2.2.5/immuneML/encodings/kmer_frequency/KmerFrequencyEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/kmer_frequency/sequence_encoding/GappedKmerSequenceEncoder.py` & `immuneML-2.2.5/immuneML/encodings/kmer_frequency/sequence_encoding/GappedKmerSequenceEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/kmer_frequency/sequence_encoding/IMGTGappedKmerEncoder.py` & `immuneML-2.2.5/immuneML/encodings/kmer_frequency/sequence_encoding/IMGTGappedKmerEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/kmer_frequency/sequence_encoding/IMGTKmerSequenceEncoder.py` & `immuneML-2.2.5/immuneML/encodings/kmer_frequency/sequence_encoding/IMGTKmerSequenceEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/kmer_frequency/sequence_encoding/IdentitySequenceEncoder.py` & `immuneML-2.2.5/immuneML/encodings/kmer_frequency/sequence_encoding/IdentitySequenceEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/kmer_frequency/sequence_encoding/KmerSequenceEncoder.py` & `immuneML-2.2.5/immuneML/encodings/kmer_frequency/sequence_encoding/KmerSequenceEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/onehot/OneHotEncoder.py` & `immuneML-2.2.5/immuneML/encodings/onehot/OneHotEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/onehot/OneHotReceptorEncoder.py` & `immuneML-2.2.5/immuneML/encodings/onehot/OneHotReceptorEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/onehot/OneHotRepertoireEncoder.py` & `immuneML-2.2.5/immuneML/encodings/onehot/OneHotRepertoireEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/onehot/OneHotSequenceEncoder.py` & `immuneML-2.2.5/immuneML/encodings/onehot/OneHotSequenceEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/preprocessing/FeatureScaler.py` & `immuneML-2.2.5/immuneML/encodings/preprocessing/FeatureScaler.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/reference_encoding/MatchedReceptorsEncoder.py` & `immuneML-2.2.5/immuneML/encodings/reference_encoding/MatchedReceptorsEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/reference_encoding/MatchedReferenceUtil.py` & `immuneML-2.2.5/immuneML/encodings/reference_encoding/MatchedReferenceUtil.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+import logging
 import os
 from pathlib import Path
-import logging
 
 from immuneML.IO.dataset_import.DatasetImportParams import DatasetImportParams
 from immuneML.dsl.DefaultParamsLoader import DefaultParamsLoader
 from immuneML.environment.EnvironmentSettings import EnvironmentSettings
 from immuneML.util.ImportHelper import ImportHelper
 from immuneML.util.ParameterValidator import ParameterValidator
 from immuneML.util.PathBuilder import PathBuilder
@@ -14,16 +14,15 @@
 class MatchedReferenceUtil:
     """
     Utility class for MatchedSequencesEncoder and MatchedReceptorsEncoder
     """
 
     @staticmethod
     def prepare_reference(reference_params: dict, location: str, paired: bool):
-        ParameterValidator.assert_keys(list(reference_params.keys()), ["format", "params"], location,
-                                       "reference")
+        ParameterValidator.assert_keys(list(reference_params.keys()), ["format", "params"], location, "reference")
 
         seq_import_params = reference_params["params"] if "params" in reference_params else {}
 
         assert os.path.isfile(seq_import_params["path"]), f"{location}: the file {seq_import_params['path']} does not exist. " \
                                                           f"Specify the correct path under reference."
 
         if "is_repertoire" in seq_import_params:
```

### Comparing `immuneML-2.2.4/immuneML/encodings/reference_encoding/MatchedRegexEncoder.py` & `immuneML-2.2.5/immuneML/encodings/reference_encoding/MatchedRegexEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/reference_encoding/MatchedRegexRepertoireEncoder.py` & `immuneML-2.2.5/immuneML/encodings/reference_encoding/MatchedRegexRepertoireEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/reference_encoding/MatchedSequencesEncoder.py` & `immuneML-2.2.5/immuneML/encodings/reference_encoding/MatchedSequencesEncoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-from pathlib import Path
+from multiprocessing.pool import Pool
+from typing import List
 
 import numpy as np
 import pandas as pd
-from multiprocessing.pool import Pool
 
+from immuneML.analysis.SequenceMatcher import SequenceMatcher
 from immuneML.caching.CacheHandler import CacheHandler
-from immuneML.data_model.receptor.receptor_sequence.ReceptorSequenceList import ReceptorSequenceList
+from immuneML.data_model.dataset.RepertoireDataset import RepertoireDataset
+from immuneML.data_model.encoded_data.EncodedData import EncodedData
+from immuneML.data_model.receptor.receptor_sequence.ReceptorSequence import ReceptorSequence
+from immuneML.data_model.repertoire.Repertoire import Repertoire
 from immuneML.encodings.DatasetEncoder import DatasetEncoder
 from immuneML.encodings.EncoderParams import EncoderParams
 from immuneML.encodings.reference_encoding.MatchedReferenceUtil import MatchedReferenceUtil
-from immuneML.util.CompAIRRHelper import CompAIRRHelper
 from immuneML.util.ParameterValidator import ParameterValidator
 from immuneML.util.ReadsType import ReadsType
-from immuneML.analysis.SequenceMatcher import SequenceMatcher
-from immuneML.data_model.dataset.RepertoireDataset import RepertoireDataset
-from immuneML.data_model.encoded_data.EncodedData import EncodedData
-from immuneML.data_model.repertoire.Repertoire import Repertoire
-
 
 
 class MatchedSequencesEncoder(DatasetEncoder):
     """
     Encodes the dataset based on the matches between a RepertoireDataset and a reference sequence dataset.
 
     This encoding can be used in combination with the :ref:`Matches` report.
@@ -51,19 +49,18 @@
         my_ms_encoding:
             MatchedSequences:
                 reference:
                     format: VDJDB
                     params:
                         path: path/to/file.txt
                 max_edit_distance: 1
-    """
-
 
+    """
 
-    def __init__(self, max_edit_distance: int, reference: ReceptorSequenceList, reads: ReadsType, sum_matches: bool, normalize: bool,
+    def __init__(self, max_edit_distance: int, reference: List[ReceptorSequence], reads: ReadsType, sum_matches: bool, normalize: bool,
                  name: str = None):
         self.max_edit_distance = max_edit_distance
         self.reference_sequences = reference
         self.reads = reads
         self.sum_matches = sum_matches
         self.normalize = normalize
         self.feature_count = 1 if self.sum_matches else len(self.reference_sequences)
@@ -117,26 +114,26 @@
 
         return (("dataset_identifiers", tuple(dataset.get_example_ids())),
                 ("dataset_metadata", dataset.metadata_file),
                 ("dataset_type", dataset.__class__.__name__),
                 ("labels", tuple(params.label_config.get_labels_by_name())),
                 ("encoding", MatchedSequencesEncoder.__name__),
                 ("learn_model", params.learn_model),
-                ("encoding_params", encoding_params_desc), )
+                ("encoding_params", encoding_params_desc),)
 
     def _encode_new_dataset(self, dataset, params: EncoderParams):
         encoded_dataset = RepertoireDataset(repertoires=dataset.repertoires, labels=dataset.labels,
                                             metadata_file=dataset.metadata_file)
 
         encoded_repertoires, labels = self._encode_repertoires(dataset, params)
 
         encoded_repertoires = self._normalize(dataset, encoded_repertoires) if self.normalize else encoded_repertoires
 
         feature_annotations = None if self.sum_matches else self._get_feature_info()
-        feature_names = [f"sum_of_{self.reads.value}_reads"] if self.sum_matches else list(feature_annotations["sequence_id"])
+        feature_names = [f"sum_of_{self.reads.value}_reads"] if self.sum_matches else list(feature_annotations["sequence_desc"])
 
         encoded_dataset.add_encoded_data(EncodedData(
             examples=encoded_repertoires,
             labels=labels,
             feature_names=feature_names,
             feature_annotations=feature_annotations,
             example_ids=[repertoire.identifier for repertoire in dataset.get_data()],
@@ -166,44 +163,59 @@
         features = [[] for i in range(0, self.feature_count)]
 
         for i, sequence in enumerate(self.reference_sequences):
             features[i] = [sequence.identifier,
                            sequence.get_attribute("chain").name.lower(),
                            sequence.get_sequence(),
                            sequence.get_attribute("v_gene"),
-                           sequence.get_attribute("j_gene")]
+                           sequence.get_attribute("j_gene"),
+                           self._get_sequence_desc(sequence)]
 
-        features = pd.DataFrame(features,
-                                columns=["sequence_id", "chain", "sequence", "v_gene", "j_gene"])
+        features = pd.DataFrame(features, columns=["sequence_id", "chain", "sequence", "v_gene", "j_gene", "sequence_desc"])
+        if features['sequence_desc'].unique().shape[0] < features.shape[0]:
+            features.loc[:, 'sequence_desc'] = [row['sequence_desc'] + "_" + row['sequence_id'] for ind, row in features.iterrows()]
 
         return features
 
+    def _get_sequence_desc(self, sequence: ReceptorSequence) -> str:
+        desc = ""
+        if sequence.get_attribute('v_gene') not in [None, ""]:
+            desc += f"{sequence.get_attribute('v_gene')}_"
+
+        desc += sequence.get_sequence()
+
+        if sequence.get_attribute('j_gene') not in ["", None]:
+            desc += f"_{sequence.get_attribute('j_gene')}"
+
+        return desc
+
     def _encode_repertoires(self, dataset: RepertoireDataset, params):
         labels = {label: [] for label in params.label_config.get_labels_by_name()} if params.encode_labels else None
 
         with Pool(params.pool_size) as pool:
             encoded_repertories = np.array(pool.map(self._get_repertoire_matches_to_reference, dataset.repertoires))
 
         for repertoire in dataset.repertoires:
             for label_name in params.label_config.get_labels_by_name():
                 labels[label_name].append(repertoire.metadata[label_name])
 
         return encoded_repertories, labels
 
     def _get_repertoire_matches_to_reference(self, repertoire):
-         return CacheHandler.memo_by_params(
-             (("repertoire_identifier", repertoire.identifier),
-              ("encoding", MatchedSequencesEncoder.__name__),
-              ("readstype", self.reads.name),
-              ("sum_matches", self.sum_matches),
-              ("max_edit_distance", self.max_edit_distance),
-              ("reference_sequences", tuple([(seq.get_attribute("chain"), seq.get_sequence(), seq.get_attribute("v_gene"), seq.get_attribute("j_gene")) for seq in self.reference_sequences]))),
+        return CacheHandler.memo_by_params(
+            (("repertoire_identifier", repertoire.identifier),
+             ("encoding", MatchedSequencesEncoder.__name__),
+             ("readstype", self.reads.name),
+             ("sum_matches", self.sum_matches),
+             ("max_edit_distance", self.max_edit_distance),
+             ("reference_sequences", tuple(
+                 [(seq.get_attribute("chain"), seq.get_sequence(), seq.get_attribute("v_gene"), seq.get_attribute("j_gene")) for seq in
+                  self.reference_sequences]))),
             lambda: self._compute_matches_to_reference(repertoire))
 
-
     def _compute_matches_to_reference(self, repertoire: Repertoire):
         matcher = SequenceMatcher()
         matches = np.zeros(self.feature_count, dtype=int)
         rep_seqs = repertoire.sequences
 
         for i, reference_seq in enumerate(self.reference_sequences):
```

### Comparing `immuneML-2.2.4/immuneML/encodings/word2vec/W2VRepertoireEncoder.py` & `immuneML-2.2.5/immuneML/encodings/word2vec/W2VRepertoireEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/word2vec/W2VSequenceEncoder.py` & `immuneML-2.2.5/immuneML/encodings/word2vec/W2VSequenceEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/word2vec/Word2VecEncoder.py` & `immuneML-2.2.5/immuneML/encodings/word2vec/Word2VecEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/word2vec/model_creator/KmerPairModelCreator.py` & `immuneML-2.2.5/immuneML/encodings/word2vec/model_creator/KmerPairModelCreator.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/word2vec/model_creator/ModelCreatorStrategy.py` & `immuneML-2.2.5/immuneML/encodings/word2vec/model_creator/ModelCreatorStrategy.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/encodings/word2vec/model_creator/SequenceModelCreator.py` & `immuneML-2.2.5/immuneML/encodings/word2vec/model_creator/SequenceModelCreator.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/environment/EnvironmentSettings.py` & `immuneML-2.2.5/immuneML/environment/EnvironmentSettings.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/environment/Label.py` & `immuneML-2.2.5/immuneML/environment/Label.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/environment/LabelConfiguration.py` & `immuneML-2.2.5/immuneML/environment/LabelConfiguration.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/hyperparameter_optimization/HPSetting.py` & `immuneML-2.2.5/immuneML/hyperparameter_optimization/HPSetting.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/hyperparameter_optimization/HPSettingResult.py` & `immuneML-2.2.5/immuneML/hyperparameter_optimization/HPSettingResult.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/hyperparameter_optimization/config/ReportConfig.py` & `immuneML-2.2.5/immuneML/hyperparameter_optimization/config/ReportConfig.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/hyperparameter_optimization/config/SplitConfig.py` & `immuneML-2.2.5/immuneML/hyperparameter_optimization/config/SplitConfig.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/hyperparameter_optimization/core/HPAssessment.py` & `immuneML-2.2.5/immuneML/hyperparameter_optimization/core/HPAssessment.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+import copy
 from pathlib import Path
 
 from immuneML.data_model.dataset.Dataset import Dataset
 from immuneML.environment.Label import Label
 from immuneML.environment.LabelConfiguration import LabelConfiguration
 from immuneML.hyperparameter_optimization.HPSetting import HPSetting
 from immuneML.hyperparameter_optimization.core.HPSelection import HPSelection
 from immuneML.hyperparameter_optimization.core.HPUtil import HPUtil
 from immuneML.hyperparameter_optimization.states.HPAssessmentState import HPAssessmentState
 from immuneML.hyperparameter_optimization.states.TrainMLModelState import TrainMLModelState
 from immuneML.ml_methods.MLMethod import MLMethod
+from immuneML.ml_methods.SklearnMethod import SklearnMethod
+from immuneML.ml_metrics.Metric import Metric
 from immuneML.reports.ReportUtil import ReportUtil
 from immuneML.util.Logger import print_log
 from immuneML.util.PathBuilder import PathBuilder
 from immuneML.workflows.instructions.MLProcess import MLProcess
 
 
 class HPAssessment:
@@ -46,15 +49,16 @@
         assessment_state = HPAssessmentState(split_index, train_val_dataset, test_dataset, current_path, state.label_configuration)
         state.assessment_states.append(assessment_state)
 
         state = HPSelection.run_selection(state, train_val_dataset, current_path, split_index)
         state = HPAssessment.run_assessment_split_per_label(state, split_index)
 
         assessment_state.train_val_data_reports = ReportUtil.run_data_reports(train_val_dataset, state.assessment.reports.data_split_reports.values(),
-                                                                              current_path / "data_report_train", state.number_of_processes, state.context)
+                                                                              current_path / "data_report_train", state.number_of_processes,
+                                                                              state.context)
         assessment_state.test_data_reports = ReportUtil.run_data_reports(test_dataset, state.assessment.reports.data_split_reports.values(),
                                                                          current_path / "data_report_test", state.number_of_processes, state.context)
 
         print_log(f'Training ML model: running outer CV loop: finished split {split_index + 1}/{n_splits}.\n', include_datetime=True)
 
         return state
 
@@ -62,15 +66,15 @@
     def run_assessment_split_per_label(state: TrainMLModelState, split_index: int):
         """iterate through labels and hp_settings and retrain all models"""
         n_labels = state.label_configuration.get_label_count()
 
         for idx, label in enumerate(state.label_configuration.get_label_objects()):
 
             print_log(f"Training ML model: running the inner loop of nested CV: "
-                  f"retrain models for label {label.name} (label {idx + 1} / {n_labels}).\n", include_datetime=True)
+                      f"retrain models for label {label.name} (label {idx + 1} / {n_labels}).\n", include_datetime=True)
 
             path = state.assessment_states[split_index].path
 
             for index, hp_setting in enumerate(state.hp_settings):
 
                 if hp_setting != state.assessment_states[split_index].label_states[label.name].optimal_hp_setting:
                     setting_path = path / f"{label.name}_{hp_setting}/"
@@ -78,31 +82,60 @@
                     setting_path = path / f"{label.name}_{hp_setting}_optimal/"
 
                 train_val_dataset = state.assessment_states[split_index].train_val_dataset
                 test_dataset = state.assessment_states[split_index].test_dataset
                 state = HPAssessment.reeval_on_assessment_split(state, train_val_dataset, test_dataset, hp_setting, setting_path, label, split_index)
 
             print_log(f"Training ML model: running the inner loop of nested CV: completed retraining models "
-                  f"for label {label.name} (label {idx + 1} / {n_labels}).\n", include_datetime=True)
+                      f"for label {label.name} (label {idx + 1} / {n_labels}).\n", include_datetime=True)
 
         return state
 
     @staticmethod
     def reeval_on_assessment_split(state, train_val_dataset: Dataset, test_dataset: Dataset, hp_setting: HPSetting, path: Path, label: Label,
                                    split_index: int) -> MLMethod:
         """retrain model for specific label, assessment split and hp_setting"""
 
+        updated_hp_setting = HPAssessment.update_hp_setting_for_assessment(hp_setting, state, split_index, label.name)
+
         assessment_item = MLProcess(train_dataset=train_val_dataset, test_dataset=test_dataset, label=label, metrics=state.metrics,
-                                    optimization_metric=state.optimization_metric, path=path, hp_setting=hp_setting, report_context=state.context,
-                                    ml_reports=state.assessment.reports.model_reports.values(), number_of_processes=state.number_of_processes,
+                                    optimization_metric=state.optimization_metric, path=path, hp_setting=updated_hp_setting,
+                                    report_context=state.context, ml_reports=state.assessment.reports.model_reports.values(),
+                                    number_of_processes=state.number_of_processes,
                                     encoding_reports=state.assessment.reports.encoding_reports.values(),
                                     label_config=LabelConfiguration([label])).run(split_index)
 
         state.assessment_states[split_index].label_states[label.name].assessment_items[str(hp_setting)] = assessment_item
 
         return state
 
     @staticmethod
+    def update_hp_setting_for_assessment(hp_setting: HPSetting, state: TrainMLModelState, split_index: int, label_name: str):
+
+        if isinstance(hp_setting.ml_method, SklearnMethod) and hp_setting.ml_params['model_selection_cv']:
+            updated_hp_setting = copy.deepcopy(hp_setting)
+            updated_hp_setting.ml_params['model_selection_cv'] = False
+            updated_hp_setting.ml_params['model_selection_n_folds'] = -1
+
+            comp_func = Metric.get_search_criterion(state.optimization_metric)
+            hp_items = state.assessment_states[split_index].label_states[label_name].selection_state.hp_items[hp_setting.get_key()]
+
+            optimal_params = {hp_item.performance[state.optimization_metric.name.lower()]:
+                                  HPAssessment._get_only_hyperparams(hp_item.method.get_params())
+                              for hp_item in hp_items}
+
+            updated_hp_setting.ml_params[updated_hp_setting.ml_method.__class__.__name__] = optimal_params[comp_func(optimal_params.keys())]
+
+            return updated_hp_setting
+
+        else:
+            return hp_setting
+
+    @staticmethod
+    def _get_only_hyperparams(params: dict):
+        return copy.deepcopy({k: v for k, v in params.items() if k not in ['intercept', 'coefficients']})
+
+    @staticmethod
     def create_assessment_path(state, split_index):
         current_path = state.path / f"split_{split_index + 1}"
         PathBuilder.build(current_path)
         return current_path
```

### Comparing `immuneML-2.2.4/immuneML/hyperparameter_optimization/core/HPSelection.py` & `immuneML-2.2.5/immuneML/hyperparameter_optimization/core/HPSelection.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,29 +29,29 @@
         train_datasets, val_datasets = HPUtil.split_data(train_val_dataset, state.selection, path, state.label_configuration)
 
         n_labels = state.label_configuration.get_label_count()
 
         for idx, label in enumerate(state.label_configuration.get_label_objects()):
 
             print_log(f"Hyperparameter optimization: running the inner loop of nested CV: selection for label {label.name} "
-                  f"(label {idx + 1} / {n_labels}).\n", include_datetime=True)
+                      f"(label {idx + 1} / {n_labels}).\n", include_datetime=True)
 
             selection_state = HPSelectionState(train_datasets, val_datasets, path, state.hp_strategy)
             state.assessment_states[split_index].label_states[label.name].selection_state = selection_state
 
             hp_setting = selection_state.hp_strategy.generate_next_setting()
             while hp_setting is not None:
                 performance = HPSelection.evaluate_hp_setting(state, hp_setting, train_datasets, val_datasets,
                                                               path, label, split_index)
                 hp_setting = selection_state.hp_strategy.generate_next_setting(hp_setting, performance)
 
             HPUtil.run_selection_reports(state, train_val_dataset, train_datasets, val_datasets, selection_state)
 
             print_log(f"Hyperparameter optimization: running the inner loop of nested CV: completed selection for "
-                  f"label {label.name} (label {idx + 1} / {n_labels}).\n", include_datetime=True)
+                      f"label {label.name} (label {idx + 1} / {n_labels}).\n", include_datetime=True)
 
         return state
 
     @staticmethod
     def evaluate_hp_setting(state: TrainMLModelState, hp_setting: HPSetting, train_datasets: list, val_datasets: list,
                             current_path: Path, label: Label, assessment_split_index: int):
 
@@ -67,15 +67,15 @@
     @staticmethod
     def run_setting(state: TrainMLModelState, hp_setting, train_dataset, val_dataset, split_index: int,
                     current_path: Path, label: Label, assessment_index: int):
 
         hp_item = MLProcess(train_dataset=train_dataset, test_dataset=val_dataset, encoding_reports=state.selection.reports.encoding_reports.values(),
                             label_config=LabelConfiguration([label]), report_context=state.context,
                             number_of_processes=state.number_of_processes, metrics=state.metrics, optimization_metric=state.optimization_metric,
-                            ml_reports=state.selection.reports.model_reports.values(), label=label, path=current_path, hp_setting=hp_setting)\
+                            ml_reports=state.selection.reports.model_reports.values(), label=label, path=current_path, hp_setting=hp_setting) \
             .run(split_index)
 
         state.assessment_states[assessment_index].label_states[label.name].selection_state.hp_items[hp_setting.get_key()].append(hp_item)
 
         return hp_item.performance[state.optimization_metric.name.lower()] if hp_item.performance is not None else None
 
     @staticmethod
```

### Comparing `immuneML-2.2.4/immuneML/hyperparameter_optimization/core/HPUtil.py` & `immuneML-2.2.5/immuneML/hyperparameter_optimization/core/HPUtil.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,24 +7,21 @@
 from immuneML.environment.Constants import Constants
 from immuneML.environment.Label import Label
 from immuneML.environment.LabelConfiguration import LabelConfiguration
 from immuneML.hyperparameter_optimization.HPSetting import HPSetting
 from immuneML.hyperparameter_optimization.config.SplitConfig import SplitConfig
 from immuneML.hyperparameter_optimization.states.HPSelectionState import HPSelectionState
 from immuneML.hyperparameter_optimization.states.TrainMLModelState import TrainMLModelState
-from immuneML.ml_methods.MLMethod import MLMethod
 from immuneML.reports.ReportResult import ReportResult
 from immuneML.reports.ReportUtil import ReportUtil
 from immuneML.util.PathBuilder import PathBuilder
 from immuneML.workflows.steps.DataEncoder import DataEncoder
 from immuneML.workflows.steps.DataEncoderParams import DataEncoderParams
 from immuneML.workflows.steps.MLMethodAssessment import MLMethodAssessment
 from immuneML.workflows.steps.MLMethodAssessmentParams import MLMethodAssessmentParams
-from immuneML.workflows.steps.MLMethodTrainer import MLMethodTrainer
-from immuneML.workflows.steps.MLMethodTrainerParams import MLMethodTrainerParams
 from immuneML.workflows.steps.data_splitter.DataSplitter import DataSplitter
 from immuneML.workflows.steps.data_splitter.DataSplitterParams import DataSplitterParams
 
 
 class HPUtil:
 
     @staticmethod
@@ -67,30 +64,14 @@
                     preprocessed_dataset = tmp_dataset
 
                 return preprocessed_dataset
             else:
                 return dataset
 
     @staticmethod
-    def train_method(label: Label, dataset, hp_setting: HPSetting, path: Path, train_predictions_path, ml_details_path, cores_for_training, optimization_metric) -> MLMethod:
-        method = MLMethodTrainer.run(MLMethodTrainerParams(
-            method=copy.deepcopy(hp_setting.ml_method),
-            result_path=path / "ml_method",
-            dataset=dataset,
-            label=label,
-            train_predictions_path=train_predictions_path,
-            ml_details_path=ml_details_path,
-            model_selection_cv=hp_setting.ml_params["model_selection_cv"],
-            model_selection_n_folds=hp_setting.ml_params["model_selection_n_folds"],
-            cores_for_training=cores_for_training,
-            optimization_metric=optimization_metric.name.lower()
-        ))
-        return method
-
-    @staticmethod
     def encode_dataset(dataset, hp_setting: HPSetting, path: Path, learn_model: bool, context: dict, number_of_processes: int,
                        label_configuration: LabelConfiguration, encode_labels: bool = True):
         PathBuilder.build(path)
 
         encoded_dataset = DataEncoder.run(DataEncoderParams(
             dataset=dataset,
             encoder=hp_setting.encoder,
```

### Comparing `immuneML-2.2.4/immuneML/hyperparameter_optimization/states/HPAssessmentState.py` & `immuneML-2.2.5/immuneML/hyperparameter_optimization/states/HPAssessmentState.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/hyperparameter_optimization/states/HPItem.py` & `immuneML-2.2.5/immuneML/hyperparameter_optimization/states/HPItem.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/hyperparameter_optimization/states/HPSelectionState.py` & `immuneML-2.2.5/immuneML/hyperparameter_optimization/states/HPSelectionState.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/hyperparameter_optimization/states/TrainMLModelState.py` & `immuneML-2.2.5/immuneML/hyperparameter_optimization/states/TrainMLModelState.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/hyperparameter_optimization/strategy/GridSearch.py` & `immuneML-2.2.5/immuneML/hyperparameter_optimization/strategy/GridSearch.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/hyperparameter_optimization/strategy/HPOptimizationStrategy.py` & `immuneML-2.2.5/immuneML/hyperparameter_optimization/strategy/HPOptimizationStrategy.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/ml_methods/AtchleyKmerMILClassifier.py` & `immuneML-2.2.5/immuneML/ml_methods/AtchleyKmerMILClassifier.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/ml_methods/DeepRC.py` & `immuneML-2.2.5/immuneML/ml_methods/DeepRC.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/ml_methods/KNN.py` & `immuneML-2.2.5/immuneML/ml_methods/KNN.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/ml_methods/LogisticRegression.py` & `immuneML-2.2.5/immuneML/ml_methods/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/ml_methods/MLMethod.py` & `immuneML-2.2.5/immuneML/ml_methods/MLMethod.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/ml_methods/PrecomputedKNN.py` & `immuneML-2.2.5/immuneML/ml_methods/PrecomputedKNN.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/ml_methods/ProbabilisticBinaryClassifier.py` & `immuneML-2.2.5/immuneML/ml_methods/ProbabilisticBinaryClassifier.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/ml_methods/RandomForestClassifier.py` & `immuneML-2.2.5/immuneML/ml_methods/RandomForestClassifier.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/ml_methods/ReceptorCNN.py` & `immuneML-2.2.5/immuneML/ml_methods/ReceptorCNN.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/ml_methods/SVC.py` & `immuneML-2.2.5/immuneML/ml_methods/SVC.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/ml_methods/SVM.py` & `immuneML-2.2.5/immuneML/ml_methods/SVM.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/ml_methods/SklearnMethod.py` & `immuneML-2.2.5/immuneML/ml_methods/SklearnMethod.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         return {label.name: Util.map_to_old_class_values(np.array(predictions), self.class_mapping)}
 
     def predict_proba(self, encoded_data: EncodedData, label: Label):
         if self.can_predict_proba():
             probabilities = self.model.predict_proba(encoded_data.examples)
             class_names = Util.map_to_old_class_values(self.model.classes_, self.class_mapping)
 
-            return {label.name: {class_name: probabilities[:,i] for i, class_name in enumerate(class_names)}}
+            return {label.name: {class_name: probabilities[:, i] for i, class_name in enumerate(class_names)}}
         else:
             return None
 
     def _fit(self, X, y, cores_for_training: int = 1):
         if not self.show_warnings:
             warnings.simplefilter("ignore")
             os.environ["PYTHONWARNINGS"] = "ignore"
@@ -136,15 +136,15 @@
 
         self.class_mapping = Util.make_class_mapping(encoded_data.labels[label.name], label.positive_class)
         self.feature_names = encoded_data.feature_names
         self.label = label
         mapped_y = Util.map_to_new_class_values(encoded_data.labels[self.label.name], self.class_mapping)
 
         self.model = self._fit_by_cross_validation(encoded_data.examples, mapped_y, number_of_splits, label, cores_for_training,
-                                                  optimization_metric)
+                                                   optimization_metric)
 
     def _fit_by_cross_validation(self, X, y, number_of_splits: int = 5, label: Label = None, cores_for_training: int = 1,
                                  optimization_metric: str = "balanced_accuracy"):
 
         model = self._get_ml_model()
         scoring = Metric.get_sklearn_score_name(Metric.get_metric(optimization_metric.upper()))
 
@@ -226,15 +226,15 @@
 
     @abc.abstractmethod
     def _get_ml_model(self, cores_for_training: int = 2, X=None):
         pass
 
     @abc.abstractmethod
     def get_params(self):
-        '''Returns the model parameters in a readable yaml-friendly way (consisting of lists, dictionaries and strings).'''
+        """Returns the model parameters in a readable yaml-friendly way (consisting of lists, dictionaries and strings)."""
         pass
 
     def get_label_name(self):
         return self.label.name
 
     def get_package_info(self) -> str:
         return 'scikit-learn ' + pkg_resources.get_distribution('scikit-learn').version
```

### Comparing `immuneML-2.2.4/immuneML/ml_methods/TCRdistClassifier.py` & `immuneML-2.2.5/immuneML/ml_methods/TCRdistClassifier.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/ml_methods/pytorch_implementations/PyTorchLogisticRegression.py` & `immuneML-2.2.5/immuneML/ml_methods/pytorch_implementations/PyTorchLogisticRegression.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/ml_methods/pytorch_implementations/PyTorchReceptorCNN.py` & `immuneML-2.2.5/immuneML/ml_methods/pytorch_implementations/PyTorchReceptorCNN.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/ml_methods/util/Util.py` & `immuneML-2.2.5/immuneML/ml_methods/util/Util.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,16 @@
     @staticmethod
     def binarize_label_classes(true_y, predicted_y, classes):
         """
         Binarizes the predictions in place using scikit-learn's label_binarize() method
 
         Necessary for some sklearn metrics, like roc_auc_score
         """
-        if hasattr(true_y, 'dtype') and true_y.dtype.type is np.str_ or isinstance(true_y, list) and any(isinstance(item, str) for item in true_y):
+        if hasattr(true_y, 'dtype') and (true_y.dtype.type is np.str_ or true_y.dtype.type is np.object_) \
+                or isinstance(true_y, list) and any(isinstance(item, str) for item in true_y):
             true_y = label_binarize(true_y, classes=classes)
             predicted_y = label_binarize(predicted_y, classes=classes)
 
         return true_y, predicted_y
 
     @staticmethod
     def setup_pytorch(number_of_threads, random_seed, pytorch_device_name=None):
```

### Comparing `immuneML-2.2.4/immuneML/ml_metrics/Metric.py` & `immuneML-2.2.5/immuneML/ml_metrics/Metric.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/ml_metrics/ml_metrics.py` & `immuneML-2.2.5/immuneML/ml_metrics/ml_metrics.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/pairwise_repertoire_comparison/ComparisonData.py` & `immuneML-2.2.5/immuneML/pairwise_repertoire_comparison/ComparisonData.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/pairwise_repertoire_comparison/ComparisonDataBatch.py` & `immuneML-2.2.5/immuneML/pairwise_repertoire_comparison/ComparisonDataBatch.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/pairwise_repertoire_comparison/PairwiseRepertoireComparison.py` & `immuneML-2.2.5/immuneML/pairwise_repertoire_comparison/PairwiseRepertoireComparison.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/preprocessing/Preprocessor.py` & `immuneML-2.2.5/immuneML/preprocessing/Preprocessor.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class Preprocessor(metaclass=abc.ABCMeta):
 
     def __init__(self, result_path: Path = None):
         self.result_path = result_path
 
     @abc.abstractmethod
-    def process_dataset(self, dataset: RepertoireDataset, result_path: Path) -> RepertoireDataset:
+    def process_dataset(self, dataset: RepertoireDataset, result_path: Path, number_of_processes: int = 1) -> RepertoireDataset:
         pass
 
     def check_dataset_type(self, dataset, valid_dataset_types: list, location: str):
         assert type(dataset) in valid_dataset_types, f"{location}: this preprocessing can only be applied to datasets of type: " \
                                                      f"{', '.join([dataset_type.__name__ for dataset_type in valid_dataset_types])}. " \
                                                      f"Your dataset is a {type(dataset).__name__}. " \
                                                      f"Please use a different preprocessing, or omit the preprocessing for this dataset."
```

### Comparing `immuneML-2.2.4/immuneML/preprocessing/SubjectRepertoireCollector.py` & `immuneML-2.2.5/immuneML/preprocessing/SubjectRepertoireCollector.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                 - my_filter: SubjectRepertoireCollector
 
     """
 
     def __init__(self, result_path: Path = None):
         super().__init__(result_path)
 
-    def process_dataset(self, dataset: RepertoireDataset, result_path: Path = None):
+    def process_dataset(self, dataset: RepertoireDataset, result_path: Path, number_of_processes=1):
         self.result_path = PathBuilder.build(result_path if result_path is not None else self.result_path)
         self.check_dataset_type(dataset, [RepertoireDataset], "SubjectRepertoireCollector")
 
         processed_dataset = self._merge_repertoires(dataset)
 
         return processed_dataset
```

### Comparing `immuneML-2.2.4/immuneML/preprocessing/filters/ChainRepertoireFilter.py` & `immuneML-2.2.5/immuneML/preprocessing/filters/ChainRepertoireFilter.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     """
 
     def __init__(self, keep_chain, result_path: Path = None):
         super().__init__(result_path)
         self.keep_chain = Chain.get_chain(keep_chain)
 
-    def process_dataset(self, dataset: RepertoireDataset, result_path: Path):
+    def process_dataset(self, dataset: RepertoireDataset, result_path: Path, number_of_processes=1):
         self.check_dataset_type(dataset, [RepertoireDataset], "ChainRepertoireFilter")
         processed_dataset = dataset.clone()
         self.result_path = result_path if result_path is not None else self.result_path
 
         repertoires = []
         indices = []
         for index, repertoire in enumerate(dataset.get_data()):
```

### Comparing `immuneML-2.2.4/immuneML/preprocessing/filters/ClonesPerRepertoireFilter.py` & `immuneML-2.2.5/immuneML/preprocessing/filters/ClonesPerRepertoireFilter.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,28 +40,26 @@
         super().__init__(result_path)
         self.lower_limit = lower_limit
         self.upper_limit = upper_limit
 
     def keeps_example_count(self) -> bool:
         return False
 
-    def process_dataset(self, dataset: RepertoireDataset, result_path: Path = None):
+    def process_dataset(self, dataset: RepertoireDataset, result_path: Path, number_of_processes=1):
         self.check_dataset_type(dataset, [RepertoireDataset], "ClonesPerRepertoireFilter")
         self.result_path = result_path if result_path is not None else self.result_path
 
-        processed_dataset = dataset.clone()
         repertoires, indices = [], []
 
         for index, repertoire in enumerate(dataset.get_data()):
             if self.lower_limit != -1 and len(repertoire.sequences) < self.lower_limit:
                 continue
             if self.upper_limit != -1 and len(repertoire.sequences) > self.upper_limit:
                 continue
             repertoires.append(dataset.repertoires[index])
             indices.append(index)
 
-        processed_dataset.repertoires = repertoires
-        processed_dataset.metadata_file = self._build_new_metadata(dataset, indices)
+        processed_dataset = RepertoireDataset.build_from_objects(repertoires=repertoires, path=result_path)
 
         self.check_dataset_not_empty(processed_dataset, "ClonesPerRepertoireFilter")
 
         return processed_dataset
```

### Comparing `immuneML-2.2.4/immuneML/preprocessing/filters/CountPerSequenceFilter.py` & `immuneML-2.2.5/immuneML/preprocessing/filters/CountPerSequenceFilter.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         self.remove_without_count = remove_without_count
         self.remove_empty_repertoires = remove_empty_repertoires
         self.batch_size = batch_size
 
     def keeps_example_count(self) -> bool:
         return not self.remove_empty_repertoires
 
-    def process_dataset(self, dataset: RepertoireDataset, result_path: Path) -> RepertoireDataset:
+    def process_dataset(self, dataset: RepertoireDataset, result_path: Path, number_of_processes=1) -> RepertoireDataset:
         self.check_dataset_type(dataset, [RepertoireDataset], "CountPerSequenceFilter")
         self.result_path = result_path if result_path is not None else self.result_path
 
         processed_dataset = copy.deepcopy(dataset)
 
         with Pool(self.batch_size) as pool:
             repertoires = pool.map(self._process_repertoire, dataset.repertoires)
```

### Comparing `immuneML-2.2.4/immuneML/preprocessing/filters/DuplicateSequenceFilter.py` & `immuneML-2.2.5/immuneML/preprocessing/filters/DuplicateSequenceFilter.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
         self.sequence_of_interest = "sequence_aas" if filter_sequence_type == SequenceType.AMINO_ACID else "sequences"
         self.sequence_to_ignore = "sequences" if self.sequence_of_interest == "sequence_aas" else "sequence_aas"
 
         assert self.sequence_of_interest in Repertoire.FIELDS
         assert self.sequence_to_ignore in Repertoire.FIELDS
 
-    def process_dataset(self, dataset: RepertoireDataset, result_path: Path) -> RepertoireDataset:
+    def process_dataset(self, dataset: RepertoireDataset, result_path: Path, number_of_processes=1) -> RepertoireDataset:
         self.result_path = result_path if result_path is not None else self.result_path
 
         self.check_dataset_type(dataset, [RepertoireDataset], "DuplicateSequenceFilter")
 
         processed_dataset = copy.deepcopy(dataset)
 
         with Pool(self.batch_size) as pool:
```

### Comparing `immuneML-2.2.4/immuneML/preprocessing/filters/Filter.py` & `immuneML-2.2.5/immuneML/preprocessing/filters/Filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from abc import ABC
-from pathlib import Path
 
 import pandas as pd
 
 from immuneML.data_model.dataset.Dataset import Dataset
 from immuneML.data_model.dataset.RepertoireDataset import RepertoireDataset
 from immuneML.preprocessing.Preprocessor import Preprocessor
 from immuneML.util.PathBuilder import PathBuilder
@@ -13,15 +12,15 @@
 
     def _build_new_metadata(self, dataset: RepertoireDataset, indices_to_keep: list):
         if dataset.metadata_file:
             df = pd.read_csv(dataset.metadata_file).iloc[indices_to_keep, :]
             df.reset_index(drop=True, inplace=True)
 
             PathBuilder.build(self.result_path)
-            path = self.result_path / f"{dataset.metadata_file.stem}_metadata_filtered.csv"
+            path = self.result_path / f"{dataset.metadata_file.stem}_filtered.csv"
             df.to_csv(path, index=False)
         else:
             path = None
         return path
 
     def _remove_empty_repertoires(self, repertoires: list):
         filtered_repertoires = []
```

### Comparing `immuneML-2.2.4/immuneML/preprocessing/filters/MetadataRepertoireFilter.py` & `immuneML-2.2.5/immuneML/preprocessing/filters/MetadataRepertoireFilter.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     def __init__(self, criteria: dict, result_path: Path = None):
         super().__init__(result_path)
         self.criteria = CriteriaTypeInstantiator.instantiate(criteria)
 
     def keeps_example_count(self) -> bool:
         return False
 
-    def process_dataset(self, dataset: RepertoireDataset, result_path: Path):
+    def process_dataset(self, dataset: RepertoireDataset, result_path: Path, number_of_processes=1):
         self.check_dataset_type(dataset, [RepertoireDataset], "MetadataRepertoireFilter")
         self.result_path = result_path if result_path is not None else self.result_path
 
         processed_dataset = dataset.clone()
         original_repertoires = processed_dataset.get_data()
         indices = self._get_matching_indices(processed_dataset)
         processed_dataset.repertoires = [original_repertoires[i] for i in indices]
```

### Comparing `immuneML-2.2.4/immuneML/presentation/PresentationFactory.py` & `immuneML-2.2.5/immuneML/presentation/PresentationFactory.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/presentation/html/DatasetExportHTMLBuilder.py` & `immuneML-2.2.5/immuneML/presentation/html/DatasetExportHTMLBuilder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/presentation/html/ExploratoryAnalysisHTMLBuilder.py` & `immuneML-2.2.5/immuneML/presentation/html/ExploratoryAnalysisHTMLBuilder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/presentation/html/HPHTMLBuilder.py` & `immuneML-2.2.5/immuneML/presentation/html/HPHTMLBuilder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/presentation/html/HTMLBuilder.py` & `immuneML-2.2.5/immuneML/presentation/html/HTMLBuilder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/presentation/html/MLApplicationHTMLBuilder.py` & `immuneML-2.2.5/immuneML/presentation/html/MLApplicationHTMLBuilder.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,9 +32,12 @@
             "dataset_name": state.dataset.name,
             "dataset_type": StringHelper.camel_case_to_word_string(type(state.dataset).__name__),
             "example_count": state.dataset.get_example_count(),
             "dataset_size": f"{state.dataset.get_example_count()} {type(state.dataset).__name__.replace('Dataset', 's').lower()}",
             "labels": [{"name": label_name, "values": str(state.label_config.get_label_values(label_name))[1:-1]}
                        for label_name in state.label_config.get_labels_by_name()],
             "predictions": Util.get_table_string_from_csv(state.predictions_path),
-            "predictions_download_link": os.path.relpath(state.predictions_path, base_path)
+            "predictions_download_link": os.path.relpath(state.predictions_path, base_path),
+            "show_metrics": state.metrics_path is not None,
+            "metrics": Util.get_table_string_from_csv(state.metrics_path) if state.metrics_path is not None else None,
+            "metrics_download_link": os.path.relpath(state.metrics_path, base_path) if state.metrics_path is not None else None
         }
```

### Comparing `immuneML-2.2.4/immuneML/presentation/html/MultiDatasetBenchmarkHTMLBuilder.py` & `immuneML-2.2.5/immuneML/presentation/html/MultiDatasetBenchmarkHTMLBuilder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/presentation/html/SimulationHTMLBuilder.py` & `immuneML-2.2.5/immuneML/presentation/html/SimulationHTMLBuilder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/presentation/html/SubsamplingHTMLBuilder.py` & `immuneML-2.2.5/immuneML/presentation/html/SubsamplingHTMLBuilder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/presentation/html/Util.py` & `immuneML-2.2.5/immuneML/presentation/html/Util.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/presentation/html/templates/AssessmentSplitDetails.html` & `immuneML-2.2.5/immuneML/presentation/html/templates/AssessmentSplitDetails.html`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/presentation/html/templates/DatasetExport.html` & `immuneML-2.2.5/immuneML/presentation/html/templates/DatasetExport.html`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/presentation/html/templates/ExploratoryAnalysis.html` & `immuneML-2.2.5/immuneML/presentation/html/templates/ExploratoryAnalysis.html`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/presentation/html/templates/HPOptimization.html` & `immuneML-2.2.5/immuneML/presentation/html/templates/HPOptimization.html`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/presentation/html/templates/MLApplication.html` & `immuneML-2.2.5/immuneML/presentation/html/templates/MLApplication.html`

 * *Files 10% similar despite different names*

```diff
@@ -55,10 +55,16 @@
                 </div>
             </div>
         </div>
         <h3>Predictions <small>(<a href="{{predictions_download_link}}">download link</a>)</small></h3>
         <div class="table-container padded">
             {{{predictions}}}
         </div>
+        {{#show_metrics}}
+        <h3>Metrics <small>(<a href="{{metrics_download_link}}">download link</a>)</small></h3>
+        <div class="table-container padded">
+            {{{metrics}}}
+        </div>
+        {{/show_metrics}}
     </div>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,7 +7,11 @@
 Type         {{dataset_type}}
 Dataset size {{dataset_size}}
 Analysis labels
 Label name Label values (classes)
 {{name}}   {{values}}
 **** Predictions (download_link) ****
 {{{predictions}}}
+{{#show_metrics}}
+**** Metrics (download_link) ****
+{{{metrics}}}
+{{/show_metrics}}
```

### Comparing `immuneML-2.2.4/immuneML/presentation/html/templates/MLTraining.html` & `immuneML-2.2.5/immuneML/presentation/html/templates/MLTraining.html`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/presentation/html/templates/MultiDatasetBenchmark.html` & `immuneML-2.2.5/immuneML/presentation/html/templates/MultiDatasetBenchmark.html`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/presentation/html/templates/Reports.html` & `immuneML-2.2.5/immuneML/presentation/html/templates/Reports.html`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/presentation/html/templates/SelectionDetails.html` & `immuneML-2.2.5/immuneML/presentation/html/templates/SelectionDetails.html`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/presentation/html/templates/Simulation.html` & `immuneML-2.2.5/immuneML/presentation/html/templates/Simulation.html`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/presentation/html/templates/Subsampling.html` & `immuneML-2.2.5/immuneML/presentation/html/templates/Subsampling.html`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/presentation/html/templates/css/custom.css` & `immuneML-2.2.5/immuneML/presentation/html/templates/css/custom.css`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/presentation/html/templates/index.html` & `immuneML-2.2.5/immuneML/presentation/html/templates/index.html`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/PlotlyUtil.py` & `immuneML-2.2.5/immuneML/reports/PlotlyUtil.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/Report.py` & `immuneML-2.2.5/immuneML/reports/Report.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import abc
 import logging
 
+from immuneML.reports.ReportOutput import ReportOutput
 from immuneML.reports.ReportResult import ReportResult
 
 
 class Report(metaclass=abc.ABCMeta):
     """
     This class defines what report classes should look like: they all have to inherit this class and implement the abstract methods: build_object()
     from parameters and generate() the report once all properties are set (in immuneML this will be taken care of by the instructions). If there are
@@ -103,15 +104,15 @@
             if self.check_prerequisites():
                 return self._generate()
         except Exception as e:
             logging.exception(f"An exception occurred while generating report {self.name}. See the details below:")
             logging.warning(f"Report {self.name} encountered an error and could not be generated: {e}.")
             return ReportResult(name=f"{self.name} (failed)", info="This report failed, see the log file for more information")
 
-    def _safe_plot(self, output_written=True, **kwargs):
+    def _safe_plot(self, output_written=True, plot_callable="_plot", **kwargs):
         """
         A wrapper around the function _plot() which catches any error that may be thrown by this function (e.g. errors in R),
         and shows an informative warning message instead. This is to prevent immuneML from crashing when the analysis has been
         completed but only a figure could not be plotted.
 
         Args:
 
@@ -126,12 +127,21 @@
         """
         warning_mssg = f"{self.__class__.__name__}: an error occurred when attempting to plot the data. \n"
         if output_written:
             warning_mssg += "\nThe data has been written to a file, but no plot has been created."
         else:
             warning_mssg += "\nNo plot has been created."
         try:
-            if callable(getattr(self, '_plot', None)):
-                return self._plot(**kwargs)
+            plot = getattr(self, plot_callable, None)
+            if callable(plot):
+                return plot(**kwargs)
         except Exception as e:
             logging.exception(f"An exception occurred while plotting the data in report {self.name}. See the details below:")
             logging.warning(warning_mssg)
+
+    def _write_output_table(self, table, file_path, name=None):
+        sep = "," if file_path.suffix == ".csv" else "\t"
+        table.to_csv(file_path, index=False, sep=sep)
+
+        return ReportOutput(path=file_path, name=name)
+
+
```

### Comparing `immuneML-2.2.4/immuneML/reports/ReportUtil.py` & `immuneML-2.2.5/immuneML/reports/ReportUtil.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/data_reports/CytoscapeNetworkExporter.py` & `immuneML-2.2.5/immuneML/reports/data_reports/CytoscapeNetworkExporter.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/data_reports/DataReport.py` & `immuneML-2.2.5/immuneML/reports/data_reports/DataReport.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/data_reports/GLIPH2Exporter.py` & `immuneML-2.2.5/immuneML/reports/data_reports/GLIPH2Exporter.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/data_reports/ReceptorDatasetOverview.py` & `immuneML-2.2.5/immuneML/reports/data_reports/ReceptorDatasetOverview.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/data_reports/RecoveredSignificantFeatures.py` & `immuneML-2.2.5/immuneML/reports/data_reports/RecoveredSignificantFeatures.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/data_reports/SequencesWithSignificantKmers.py` & `immuneML-2.2.5/immuneML/reports/data_reports/SequencesWithSignificantKmers.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/data_reports/SignificantFeatures.py` & `immuneML-2.2.5/immuneML/reports/data_reports/SignificantFeatures.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/data_reports/SignificantKmerPositions.py` & `immuneML-2.2.5/immuneML/reports/data_reports/SignificantKmerPositions.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/data_reports/SimpleDatasetOverview.py` & `immuneML-2.2.5/immuneML/reports/data_reports/SimpleDatasetOverview.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/encoding_reports/DesignMatrixExporter.py` & `immuneML-2.2.5/immuneML/reports/encoding_reports/DesignMatrixExporter.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/encoding_reports/EncodingReport.py` & `immuneML-2.2.5/immuneML/reports/encoding_reports/EncodingReport.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/encoding_reports/FeatureComparison.py` & `immuneML-2.2.5/immuneML/reports/encoding_reports/FeatureComparison.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/encoding_reports/FeatureDistribution.py` & `immuneML-2.2.5/immuneML/reports/encoding_reports/FeatureDistribution.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/encoding_reports/FeatureReport.py` & `immuneML-2.2.5/immuneML/reports/encoding_reports/FeatureReport.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,17 +24,24 @@
         self.facet_row = row_grouping_label
         self.facet_column = column_grouping_label
 
     def _generate_report_result(self) -> ReportResult:
         PathBuilder.build(self.result_path)
         data_long_format = DataReshaper.reshape(self.dataset, self.dataset.get_label_names())
         table_result = self._write_results_table(data_long_format)
-        report_output_fig = self._safe_plot(data_long_format=data_long_format)
-        output_figures = None if report_output_fig is None else [report_output_fig]
-        return ReportResult(name=self.name, output_figures=output_figures, output_tables=[table_result])
+        report_output = self._safe_plot(data_long_format=data_long_format)
+        output_tables = [table_result]
+        if report_output is None:
+            output_figures = None
+        elif isinstance(report_output, tuple):
+            output_figures = report_output[0] if isinstance(report_output[0], list) else [report_output[0]]
+            output_tables = report_output[1]
+        else:
+            output_figures = report_output if isinstance(report_output, list) else [report_output]
+        return ReportResult(name=self.name, output_figures=output_figures, output_tables=output_tables)
 
     def _write_results_table(self, data) -> ReportOutput:
         table_path = self.result_path / f"feature_values.csv"
         data.to_csv(table_path, index=False)
         return ReportOutput(table_path, "feature values")
 
     def std(self, x):
```

### Comparing `immuneML-2.2.4/immuneML/reports/encoding_reports/Matches.py` & `immuneML-2.2.5/immuneML/reports/encoding_reports/Matches.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,20 +72,22 @@
                 output_tables += self._write_receptor_info(self.result_path / "receptor_info")
 
         return ReportResult(self.name,
                             info=f"Reports the number of matches that were found when using {self.dataset.encoded_data.encoding}",
                             output_tables=output_tables)
 
     def _write_match_table(self):
-        id_df = pd.DataFrame({"repertoire_id": self.dataset.encoded_data.example_ids})
+        id_df = pd.DataFrame({"repertoire_id": self.dataset.encoded_data.example_ids,
+                              'subject_id': self.dataset.get_subject_ids()})
         label_df = pd.DataFrame(self.dataset.encoded_data.labels)
         matches_df = pd.DataFrame(self.dataset.encoded_data.examples, columns=self.dataset.encoded_data.feature_names)
+        different_cols = label_df.columns.difference(id_df.columns)
 
         result_path = self.result_path / "complete_match_count_table.csv"
-        id_df.join(label_df).join(matches_df).to_csv(result_path, index=False)
+        id_df.join(label_df[different_cols]).join(matches_df).to_csv(result_path, index=False)
 
         return ReportOutput(result_path, "All matches")
 
     def _write_paired_matches(self, paired_matches_path: Path) -> List[ReportOutput]:
         PathBuilder.build(paired_matches_path)
 
         report_outputs = []
```

### Comparing `immuneML-2.2.4/immuneML/reports/encoding_reports/RelevantSequenceExporter.py` & `immuneML-2.2.5/immuneML/reports/encoding_reports/RelevantSequenceExporter.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/ml_reports/Coefficients.py` & `immuneML-2.2.5/immuneML/reports/ml_reports/Coefficients.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/ml_reports/ConfounderAnalysis.py` & `immuneML-2.2.5/immuneML/reports/ml_reports/ConfounderAnalysis.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/ml_reports/DeepRCMotifDiscovery.py` & `immuneML-2.2.5/immuneML/reports/ml_reports/DeepRCMotifDiscovery.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/ml_reports/KernelSequenceLogo.py` & `immuneML-2.2.5/immuneML/reports/ml_reports/KernelSequenceLogo.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/ml_reports/MLReport.py` & `immuneML-2.2.5/immuneML/reports/ml_reports/MLReport.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/ml_reports/MotifSeedRecovery.py` & `immuneML-2.2.5/immuneML/reports/ml_reports/MotifSeedRecovery.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/ml_reports/ROCCurve.py` & `immuneML-2.2.5/immuneML/reports/ml_reports/ROCCurve.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/ml_reports/SequenceAssociationLikelihood.py` & `immuneML-2.2.5/immuneML/reports/ml_reports/SequenceAssociationLikelihood.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/ml_reports/TCRdistMotifDiscovery.py` & `immuneML-2.2.5/immuneML/reports/ml_reports/TCRdistMotifDiscovery.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/ml_reports/TrainingPerformance.py` & `immuneML-2.2.5/immuneML/reports/ml_reports/TrainingPerformance.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from immuneML.data_model.dataset.Dataset import Dataset
 from immuneML.environment.Constants import Constants
 from immuneML.hyperparameter_optimization import HPSetting
 from immuneML.ml_methods.MLMethod import MLMethod
 from immuneML.ml_metrics import ml_metrics
 from immuneML.ml_metrics.Metric import Metric
+from immuneML.ml_metrics.MetricUtil import MetricUtil
 from immuneML.reports.ReportOutput import ReportOutput
 from immuneML.reports.ReportResult import ReportResult
 from immuneML.reports.ml_reports.MLReport import MLReport
 from immuneML.util.ParameterValidator import ParameterValidator
 from immuneML.util.PathBuilder import PathBuilder
 
 
@@ -83,21 +84,18 @@
         scores = {}
         output = {
             'tables': [],
             'figures': []
         }
 
         for metric in self.metrics_set:
-            _score = TrainingPerformance._compute_score(
-                Metric.get_metric(metric),
-                predicted_y,
-                predicted_proba_y,
-                true_y,
-                classes,
-            )
+            _score = MetricUtil.score_for_metric(metric=Metric.get_metric(metric),
+                                                 predicted_y=predicted_y, predicted_proba_y=predicted_proba_y,
+                                                 true_y=true_y, classes=classes)
+
             if metric == 'CONFUSION_MATRIX':
                 self._generate_heatmap(classes, classes, _score, metric, output)
             else:
                 scores[metric] = _score
 
         scores_df = pd.DataFrame.from_dict(scores, orient='index')
         scores_df.columns = [self.label.name]
@@ -105,44 +103,14 @@
         self._generate_barplot(scores_df, output)
 
         return ReportResult(self.name,
                             info="Plots the evaluation metrics for the performance given machine learning model and training dataset.",
                             output_tables=output['tables'],
                             output_figures=output['figures'])
 
-    @staticmethod
-    def _compute_score(metric: Metric, predicted_y, predicted_proba_y, true_y, labels):
-        if hasattr(ml_metrics, metric.value):
-            fn = getattr(ml_metrics, metric.value)
-        else:
-            fn = getattr(sklearn_metrics, metric.value)
-
-        if hasattr(true_y, 'dtype') and true_y.dtype.type is np.str_ or isinstance(true_y, list) and any(isinstance(item, str) for item in true_y):
-            true_y = label_binarize(true_y, classes=labels)
-            predicted_y = label_binarize(predicted_y, classes=labels)
-
-        try:
-            if metric in Metric.get_probability_based_metric_types():
-                predictions = predicted_proba_y
-                if predicted_proba_y is None:
-                    warnings.warn(f"TrainingPerformance: metric {metric} is specified, but the chosen ML method does not output "
-                                  f"class probabilities. Using predicted classes instead...")
-                    predictions = predicted_y
-            else:
-                predictions = predicted_y
-            
-            score = fn(true_y, predictions)
-
-        except ValueError as err:
-            warnings.warn(f"TrainingPerformance: score for metric {metric.name} could not be calculated."
-                          f"\nPredicted values: {predicted_y}\nTrue values: {true_y}.\nMore details: {err}", RuntimeWarning)
-            score = Constants.NOT_COMPUTED
-
-        return score
-
     def _generate_barplot(self, df, output):
         import plotly.express as px
 
         path_csv = self.result_path / f"{self.name}.csv"
         path_html = self.result_path / f"{self.name}.html"
 
         df.to_csv(path_csv)
```

### Comparing `immuneML-2.2.4/immuneML/reports/multi_dataset_reports/DiseaseAssociatedSequenceOverlap.py` & `immuneML-2.2.5/immuneML/reports/multi_dataset_reports/DiseaseAssociatedSequenceOverlap.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/multi_dataset_reports/MultiDatasetReport.py` & `immuneML-2.2.5/immuneML/reports/multi_dataset_reports/MultiDatasetReport.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/multi_dataset_reports/PerformanceOverview.py` & `immuneML-2.2.5/immuneML/reports/multi_dataset_reports/PerformanceOverview.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/train_ml_model_reports/CVFeaturePerformance.py` & `immuneML-2.2.5/immuneML/reports/train_ml_model_reports/CVFeaturePerformance.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/train_ml_model_reports/DiseaseAssociatedSequenceCVOverlap.py` & `immuneML-2.2.5/immuneML/reports/train_ml_model_reports/DiseaseAssociatedSequenceCVOverlap.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/train_ml_model_reports/MLSettingsPerformance.py` & `immuneML-2.2.5/immuneML/reports/train_ml_model_reports/MLSettingsPerformance.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/train_ml_model_reports/ROCCurveSummary.py` & `immuneML-2.2.5/immuneML/reports/train_ml_model_reports/ROCCurveSummary.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/train_ml_model_reports/ReferenceSequenceOverlap.py` & `immuneML-2.2.5/immuneML/reports/train_ml_model_reports/ReferenceSequenceOverlap.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/reports/train_ml_model_reports/TrainMLModelReport.py` & `immuneML-2.2.5/immuneML/reports/train_ml_model_reports/TrainMLModelReport.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/simulation/Implanting.py` & `immuneML-2.2.5/immuneML/simulation/Implanting.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/simulation/dataset_generation/RandomDatasetGenerator.py` & `immuneML-2.2.5/immuneML/simulation/dataset_generation/RandomDatasetGenerator.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/simulation/implants/Motif.py` & `immuneML-2.2.5/immuneML/simulation/implants/Motif.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/simulation/implants/MotifInstance.py` & `immuneML-2.2.5/immuneML/simulation/implants/MotifInstance.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/simulation/implants/Signal.py` & `immuneML-2.2.5/immuneML/simulation/implants/Signal.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/simulation/motif_instantiation_strategy/GappedKmerInstantiation.py` & `immuneML-2.2.5/immuneML/simulation/motif_instantiation_strategy/GappedKmerInstantiation.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/simulation/sequence_implanting/GappedMotifImplanting.py` & `immuneML-2.2.5/immuneML/simulation/sequence_implanting/GappedMotifImplanting.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/simulation/signal_implanting_strategy/FullSequenceImplanting.py` & `immuneML-2.2.5/immuneML/simulation/signal_implanting_strategy/FullSequenceImplanting.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/simulation/signal_implanting_strategy/HealthySequenceImplanting.py` & `immuneML-2.2.5/immuneML/simulation/signal_implanting_strategy/HealthySequenceImplanting.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/simulation/signal_implanting_strategy/ImplantingComputation.py` & `immuneML-2.2.5/immuneML/simulation/signal_implanting_strategy/ImplantingComputation.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/simulation/signal_implanting_strategy/ReceptorImplanting.py` & `immuneML-2.2.5/immuneML/simulation/signal_implanting_strategy/ReceptorImplanting.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/simulation/signal_implanting_strategy/SignalImplantingStrategy.py` & `immuneML-2.2.5/immuneML/simulation/signal_implanting_strategy/SignalImplantingStrategy.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/util/AdaptiveImportHelper.py` & `immuneML-2.2.5/immuneML/util/AdaptiveImportHelper.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             dataframe.loc[:, 'sequences'] = [y[(81 - 3 * len(x)): 81] if x is not None else None for x, y in
                                              zip(dataframe['sequence_aas'], dataframe['sequences'])]
 
         dataframe = AdaptiveImportHelper.parse_adaptive_germline_to_imgt(dataframe, params.organism)
         ImportHelper.update_gene_info(dataframe)
         ImportHelper.load_chains(dataframe)
         ImportHelper.drop_empty_sequences(dataframe, params.import_empty_aa_sequences, params.import_empty_nt_sequences)
-        ImportHelper.drop_illegal_character_sequences(dataframe, params.import_illegal_characters)
+        ImportHelper.drop_illegal_character_sequences(dataframe, params.import_illegal_characters, params.import_with_stop_codon)
 
         return dataframe
 
     @staticmethod
     def parse_adaptive_germline_to_imgt(dataframe, organism):
         gene_name_replacement = pd.read_csv(
             EnvironmentSettings.root_path / "immuneML/IO/dataset_import/conversion/imgt_adaptive_conversion.csv")
```

### Comparing `immuneML-2.2.4/immuneML/util/CompAIRRHelper.py` & `immuneML-2.2.5/immuneML/util/CompAIRRHelper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 import subprocess
 import warnings
 from pathlib import Path
 
 import pandas as pd
 
+from immuneML.data_model.receptor.RegionType import RegionType
 from immuneML.environment.EnvironmentSettings import EnvironmentSettings
+from immuneML.util.CompAIRRParams import CompAIRRParams
 
 
 class CompAIRRHelper:
 
     @staticmethod
     def determine_compairr_path(compairr_path):
         if compairr_path is None:
@@ -44,31 +46,43 @@
             raise Exception(f"CompAIRRHelper: failed to call CompAIRR: {e}\n"
                             f"Please ensure the correct version of CompAIRR has been installed (version {required_major}.{required_minor}.{required_patch} or later), "
                             f"or provide the path to the CompAIRR executable.")
 
         return compairr_path
 
     @staticmethod
-    def get_cmd_args(compairr_params, input_file_list, result_path):
+    def get_cmd_args(compairr_params: CompAIRRParams, input_file_list, result_path):
         indels_args = ["-i"] if compairr_params.indels else []
         frequency_args = ["-f"] if compairr_params.ignore_counts else []
         ignore_genes = ["-g"] if compairr_params.ignore_genes else []
         output_args = ["-o", str(result_path / compairr_params.output_filename), "-l", str(result_path / compairr_params.log_filename)]
+        output_pairs = ['-p', str(result_path / compairr_params.pairs_filename)] if compairr_params.output_pairs else []
+        cdr3_indicator = ['--cdr3'] if compairr_params.is_cdr3 else []
+        command = '-m' if compairr_params.do_repertoire_overlap and not compairr_params.do_sequence_matching else '-x'
 
-        return [str(compairr_params.compairr_path), "-m", "-d", str(compairr_params.differences), "-t", str(compairr_params.threads)] + \
-               indels_args + frequency_args + ignore_genes + output_args + input_file_list
+        return [str(compairr_params.compairr_path), command, "-d", str(compairr_params.differences), "-t", str(compairr_params.threads)] + \
+                indels_args + frequency_args + ignore_genes + output_args + input_file_list + output_pairs + cdr3_indicator
 
     @staticmethod
-    def write_repertoire_file(repertoire_dataset, filename, compairr_params):
+    def write_repertoire_file(repertoire_dataset=None, filename=None, compairr_params=None, repertoires: list = None):
         mode = "w"
         header = True
 
-        for repertoire in repertoire_dataset.get_data():
+        columns_in_order = []
+
+        if repertoire_dataset is not None and repertoires is None:
+            repertoires = repertoire_dataset.get_data()
+
+        for ind, repertoire in enumerate(repertoires):
             repertoire_contents = CompAIRRHelper.get_repertoire_contents(repertoire, compairr_params)
-            repertoire_contents.to_csv(filename, mode=mode, header=header, index=False, sep="\t")
+
+            if ind == 0:
+                columns_in_order = sorted(repertoire_contents.columns)
+
+            repertoire_contents[columns_in_order].to_csv(filename, mode=mode, header=header, index=False, sep="\t")
 
             mode = "a"
             header = False
 
     @staticmethod
     def get_repertoire_contents(repertoire, compairr_params):
         attributes = [EnvironmentSettings.get_sequence_type().value, "counts"]
@@ -87,15 +101,15 @@
         if n_rows_before > len(repertoire_contents):
             warnings.warn(
                 f"CompAIRRHelper: removed {n_rows_before - len(repertoire_contents)} entries from repertoire {repertoire.identifier} due to missing values.")
 
         if compairr_params.ignore_counts:
             repertoire_contents["counts"] = 1
 
-        repertoire_contents.rename(columns={EnvironmentSettings.get_sequence_type().value: "junction_aa",
+        repertoire_contents.rename(columns={EnvironmentSettings.get_sequence_type().value: "cdr3_aa" if repertoire.get_region_type() == RegionType.IMGT_CDR3 else 'junction_aa',
                                             "v_genes": "v_call", "j_genes": "j_call",
                                             "counts": "duplicate_count", "identifier": "repertoire_id"},
                                    inplace=True)
 
         return repertoire_contents
 
     @staticmethod
```

### Comparing `immuneML-2.2.4/immuneML/util/EncoderHelper.py` & `immuneML-2.2.5/immuneML/util/EncoderHelper.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/util/FilenameHandler.py` & `immuneML-2.2.5/immuneML/util/FilenameHandler.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/util/ImportHelper.py` & `immuneML-2.2.5/immuneML/util/ImportHelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,16 @@
 
     @staticmethod
     def load_repertoire_as_object(import_class, metadata_row, params: DatasetImportParams):
         try:
             alternative_load_func = getattr(import_class, "alternative_load_func", None)
 
             filename = params.path / f"{metadata_row['filename']}"
+            if not filename.is_file():
+                filename = params.path / f"repertoires/{metadata_row['filename']}"
 
             dataframe = ImportHelper.load_sequence_dataframe(filename, params, alternative_load_func)
             dataframe = import_class.preprocess_dataframe(dataframe, params)
             sequence_lists = {field: dataframe[field].values.tolist() for field in Repertoire.FIELDS if field in dataframe.columns}
             sequence_lists["custom_lists"] = {field: dataframe[field].values.tolist()
                                               for field in list(set(dataframe.columns) - set(Repertoire.FIELDS))}
 
@@ -261,31 +263,32 @@
                         f"sequence after preprocessing. ")
             else:
                 warnings.warn(f"{ImportHelper.__name__}: column {sequence_colname} was not set, but is required for filtering. Skipping this filtering...")
 
         return dataframe
 
     @staticmethod
-    def drop_illegal_character_sequences(dataframe: pd.DataFrame, import_illegal_characters: bool) -> pd.DataFrame:
+    def drop_illegal_character_sequences(dataframe: pd.DataFrame, import_illegal_characters: bool, import_with_stop_codon: bool) -> pd.DataFrame:
         if not import_illegal_characters:
             sequence_type = EnvironmentSettings.get_sequence_type()
             sequence_name = sequence_type.name.lower().replace("_", " ")
 
             legal_alphabet = EnvironmentSettings.get_sequence_alphabet(sequence_type)
-            if sequence_type == SequenceType.AMINO_ACID:
+            if sequence_type == SequenceType.AMINO_ACID and import_with_stop_codon:
                 legal_alphabet.append(Constants.STOP_CODON)
 
             is_illegal_seq = [ImportHelper.is_illegal_sequence(sequence, legal_alphabet) for
                               sequence in dataframe[sequence_type.value]]
             n_illegal = sum(is_illegal_seq)
+            n_total = dataframe.shape[0]
 
             if n_illegal > 0:
                 dataframe.drop(dataframe.loc[is_illegal_seq].index, inplace=True)
-                warnings.warn(
-                    f"{ImportHelper.__name__}: {n_illegal} sequences were removed from the dataset because their {sequence_name} sequence contained illegal characters. ")
+                warnings.warn(f"{ImportHelper.__name__}: {n_illegal}/{n_total} sequences were removed from the dataset because their {sequence_name}"
+                              f" sequence contained illegal characters. ")
         return dataframe
 
     @staticmethod
     def is_illegal_sequence(sequence, legal_alphabet) -> bool:
         if sequence is None:
             return False
         else:
```

### Comparing `immuneML-2.2.4/immuneML/util/KmerHelper.py` & `immuneML-2.2.5/immuneML/util/KmerHelper.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/util/Logger.py` & `immuneML-2.2.5/immuneML/util/Logger.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/util/NameBuilder.py` & `immuneML-2.2.5/immuneML/util/NameBuilder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/util/NumpyHelper.py` & `immuneML-2.2.5/immuneML/util/NumpyHelper.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/util/ParameterValidator.py` & `immuneML-2.2.5/immuneML/util/ParameterValidator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+from pathlib import Path
+import pandas as pd
+
+from immuneML.environment.SequenceType import SequenceType
+
+
 class ParameterValidator:
 
     @staticmethod
     def assert_any_value_present(values: list, expected_values: list, location: str, parameter_name: str):
         assert any(exp_val in values for exp_val in expected_values), f"{location}: expected at least one of values {expected_values} for " \
                                                                       f"parameter {parameter_name} to be set, but none were found in {values}."
 
@@ -22,29 +28,39 @@
 
     @staticmethod
     def assert_all_type_and_value(values, parameter_type, location: str, parameter_name: str, min_inclusive=None, max_inclusive=None):
         for value in values:
             ParameterValidator.assert_type_and_value(value, parameter_type, location, parameter_name, min_inclusive, max_inclusive)
 
     @staticmethod
-    def assert_type_and_value(value, parameter_type, location: str, parameter_name: str, min_inclusive=None, max_inclusive=None, exact_value=None):
+    def assert_type_and_value(value, parameter_type, location: str, parameter_name: str,
+                              min_inclusive=None, max_inclusive=None,
+                              min_exclusive=None, max_exclusive=None, exact_value=None):
         assert isinstance(value, parameter_type), f"{location}: {value} is not a valid value for parameter {parameter_name}. " \
                                                   f"It has to be of type {parameter_type.__name__}, but is now of type {type(value).__name__}."
 
         if min_inclusive is not None:
             assert value >= min_inclusive, f"{location}: {value} is not a valid value for parameter {parameter_name}. " \
                                            f"It has to be greater or equal to {min_inclusive}."
 
         if max_inclusive is not None:
             assert value <= max_inclusive, f"{location}: {value} is not a valid value for parameter {parameter_name}. " \
                                            f"It has to be less or equal to {max_inclusive}."
 
+        if min_exclusive is not None:
+            assert value > min_exclusive, f"{location}: {value} is not a valid value for parameter {parameter_name}. " \
+                                           f"It has to be greater than {min_exclusive}."
+
+        if max_exclusive is not None:
+            assert value < max_exclusive, f"{location}: {value} is not a valid value for parameter {parameter_name}. " \
+                                           f"It has to be less than {max_exclusive}."
+
         if exact_value is not None:
             assert value == exact_value, f"{location}: {value} is not a valid value for parameter {parameter_name}. " \
-                                           f"It has to be equal to {exact_value}."
+                                         f"It has to be equal to {exact_value}."
 
     @staticmethod
     def assert_keys(keys, valid_keys, location: str, parameter_name: str, exclusive: bool = True):
         for key in keys:
             assert key in valid_keys, f"{location}: {key} is not a valid parameter under {parameter_name}. " \
                                       f"Valid parameters are: {str(valid_keys)[1:-1]}."
 
@@ -53,7 +69,24 @@
                 raise AssertionError(f"{location}: {str(list(set(keys) - set(valid_keys)))[1:-1]} are not valid parameters "
                                      f" under {parameter_name}. Valid parameters are: {str(valid_keys)[1:-1]}. "
                                      f"Remove invalid parameters.")
             elif len(keys) < len(valid_keys):
                 raise AssertionError(f"{location}: Missing parameters: {str(list(set(valid_keys) - set(keys)))[1:-1]} "
                                      f"under {parameter_name}. Valid parameters are: {str(valid_keys)[1:-1]}. "
                                      f"Please add missing parameters.")
+
+    @staticmethod
+    def assert_valid_tabular_file(file_path, location: str, parameter_name: str, sep="\t", expected_columns: list=None):
+        assert Path(file_path).is_file(), f"{location}: {parameter_name} {str(file_path)} is not an existing file."
+
+        if expected_columns is not None:
+            columns = pd.read_csv(file_path, index_col=0, nrows=0, sep=sep).columns.tolist()
+            assert set(columns) == set(expected_columns), f"{location}: columns for {parameter_name} are not as expected.\n" \
+                                                          f"Expected: {expected_columns}\n" \
+                                                          f"Found: {columns}"
+
+    @staticmethod
+    def assert_sequence_type(params, location: str = ""):
+        assert "sequence_type" in params, f"{location}: 'sequence_type' is missing: {params}."
+        assert params['sequence_type'].upper() in [st.name for st in
+                                                   SequenceType], f"{location}: {params['sequence_type']} is not a valid sequence type. " \
+                                                                  f"Valid sequence types are: {[st.name for st in SequenceType]}."
```

### Comparing `immuneML-2.2.4/immuneML/util/PathBuilder.py` & `immuneML-2.2.5/immuneML/util/PathBuilder.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # quality: gold
 
 import errno
 import os
+import shutil
 import warnings
 from pathlib import Path
 
 
 class PathBuilder:
 
     @staticmethod
@@ -17,7 +18,17 @@
             try:
                 os.makedirs(path)
             except OSError as e:
                 if e.errno != errno.EEXIST:
                     raise
 
         return path
+
+    @staticmethod
+    def remove_old_and_build(path):
+        path = Path(path)
+        if path.is_dir():
+            shutil.rmtree(path)
+
+        path.mkdir()
+
+        return path
```

### Comparing `immuneML-2.2.4/immuneML/util/PositionHelper.py` & `immuneML-2.2.5/immuneML/util/PositionHelper.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/util/ReflectionHandler.py` & `immuneML-2.2.5/immuneML/util/ReflectionHandler.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/util/RepertoireBuilder.py` & `immuneML-2.2.5/immuneML/util/RepertoireBuilder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from pathlib import Path
 
 import pandas as pd
 
 from immuneML.data_model.receptor.receptor_sequence.ReceptorSequence import ReceptorSequence
-from immuneML.data_model.receptor.receptor_sequence.ReceptorSequenceList import ReceptorSequenceList
 from immuneML.data_model.receptor.receptor_sequence.SequenceMetadata import SequenceMetadata
 from immuneML.data_model.repertoire.Repertoire import Repertoire
 from immuneML.util.PathBuilder import PathBuilder
 
 
 class RepertoireBuilder:
     """
@@ -28,15 +27,15 @@
         rep_path = PathBuilder.build(path / "repertoires")
 
         repertoires = []
         if subject_ids is None:
             subject_ids = []
 
         for rep_index, sequence_list in enumerate(sequences):
-            rep_sequences = ReceptorSequenceList()
+            rep_sequences = []
             if len(subject_ids) < len(sequences):
                 subject_ids.append("rep_" + str(rep_index))
             for seq_index, sequence in enumerate(sequence_list):
                 if seq_metadata is None:
                     m = SequenceMetadata(v_subgroup="TRBV1", v_gene="TRBV1-1", v_allele="TRBV1-1*01", j_subgroup="TRBJ1", j_gene="TRBJ1-1", j_allele="TRBJ1-1*01", count=1, chain="TRB", region_type="IMGT_CDR3")
                 else:
                     m = SequenceMetadata(**seq_metadata[rep_index][seq_index])
```

### Comparing `immuneML-2.2.4/immuneML/util/SequenceAnalysisHelper.py` & `immuneML-2.2.5/immuneML/util/SequenceAnalysisHelper.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/util/SignificantFeaturesHelper.py` & `immuneML-2.2.5/immuneML/util/SignificantFeaturesHelper.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/util/TCRdistHelper.py` & `immuneML-2.2.5/immuneML/util/TCRdistHelper.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/workflows/instructions/MLProcess.py` & `immuneML-2.2.5/immuneML/workflows/instructions/MLProcess.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 
 from immuneML.data_model.dataset.Dataset import Dataset
 from immuneML.environment.Label import Label
 from immuneML.environment.LabelConfiguration import LabelConfiguration
 from immuneML.hyperparameter_optimization.HPSetting import HPSetting
 from immuneML.hyperparameter_optimization.core.HPUtil import HPUtil
 from immuneML.hyperparameter_optimization.states.HPItem import HPItem
+from immuneML.ml_methods.MLMethod import MLMethod
 from immuneML.ml_metrics.Metric import Metric
 from immuneML.reports.ReportUtil import ReportUtil
 from immuneML.reports.ml_reports.MLReport import MLReport
 from immuneML.util.Logger import print_log
 from immuneML.util.PathBuilder import PathBuilder
+from immuneML.workflows.steps.MLMethodTrainer import MLMethodTrainer
+from immuneML.workflows.steps.MLMethodTrainerParams import MLMethodTrainerParams
 
 
 class MLProcess:
     """
     Class that implements the machine learning process:
         1. encodes the training dataset
         2. encodes the test dataset (using parameters learnt in step 1 if there are any such parameters)
@@ -40,15 +43,14 @@
         self.train_predictions_path = path / "train_predictions.csv" if path is not None else None
         self.test_predictions_path = path / "test_predictions.csv" if path is not None else None
         self.report_path = PathBuilder.build(path / "reports") if path is not None else None
         self.number_of_processes = number_of_processes
         assert all([isinstance(metric, Metric) for metric in metrics]), \
             "MLProcess: metrics are not set to be an instance of Metric."
         self.metrics = metrics
-        self.metrics.add(Metric.BALANCED_ACCURACY)
         self.optimization_metric = optimization_metric
         self.ml_reports = ml_reports if ml_reports is not None else []
         self.encoding_reports = encoding_reports if encoding_reports is not None else []
         self.data_reports = data_reports if data_reports is not None else []
         self.report_context = report_context
         self.hp_setting = copy.deepcopy(hp_setting)
 
@@ -71,24 +73,39 @@
         processed_dataset = HPUtil.preprocess_dataset(self.train_dataset, self.hp_setting.preproc_sequence, self.path / "preprocessed_train_dataset",
                                                       self.report_context)
 
         encoded_train_dataset = HPUtil.encode_dataset(processed_dataset, self.hp_setting, self.path / "encoded_datasets", learn_model=True,
                                                       context=self.report_context, number_of_processes=self.number_of_processes,
                                                       label_configuration=self.label_config)
 
-        method = HPUtil.train_method(self.label, encoded_train_dataset, self.hp_setting, self.path, self.train_predictions_path, self.ml_details_path, self.number_of_processes, self.optimization_metric)
+        method = self._train_method(encoded_train_dataset)
 
         encoding_train_results = ReportUtil.run_encoding_reports(encoded_train_dataset, self.encoding_reports, self.report_path / "encoding_train", self.number_of_processes)
 
         hp_item = self._assess_on_test_dataset(encoded_train_dataset, encoding_train_results, method, split_index)
 
         print_log(f"Completed hyperparameter setting {self.hp_setting}.\n", include_datetime=True)
 
         return hp_item
 
+    def _train_method(self, dataset) -> MLMethod:
+        method = MLMethodTrainer.run(MLMethodTrainerParams(
+            method=copy.deepcopy(self.hp_setting.ml_method),
+            result_path=self.path / "ml_method",
+            dataset=dataset,
+            label=self.label,
+            train_predictions_path=self.train_predictions_path,
+            ml_details_path=self.ml_details_path,
+            model_selection_cv=self.hp_setting.ml_params["model_selection_cv"],
+            model_selection_n_folds=self.hp_setting.ml_params["model_selection_n_folds"],
+            cores_for_training=self.number_of_processes,
+            optimization_metric=self.optimization_metric.name.lower()
+        ))
+        return method
+
     def _assess_on_test_dataset(self, encoded_train_dataset, encoding_train_results, method, split_index) -> HPItem:
         if self.test_dataset is not None and self.test_dataset.get_example_count() > 0:
             processed_test_dataset = HPUtil.preprocess_dataset(self.test_dataset, self.hp_setting.preproc_sequence,
                                                                self.path / "preprocessed_test_dataset")
             encoded_test_dataset = HPUtil.encode_dataset(processed_test_dataset, self.hp_setting, self.path / "encoded_datasets",
                                                          learn_model=False, context=self.report_context, number_of_processes=self.number_of_processes,
                                                          label_configuration=self.label_config)
```

### Comparing `immuneML-2.2.4/immuneML/workflows/instructions/SimulationInstruction.py` & `immuneML-2.2.5/immuneML/workflows/instructions/SimulationInstruction.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/workflows/instructions/TrainMLModelInstruction.py` & `immuneML-2.2.5/immuneML/workflows/instructions/TrainMLModelInstruction.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/workflows/instructions/dataset_generation/DatasetExportInstruction.py` & `immuneML-2.2.5/immuneML/workflows/instructions/dataset_generation/DatasetExportInstruction.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,16 +57,17 @@
         self.result_path = result_path / self.name
         paths = {}
 
         for dataset in self.datasets:
             dataset_name = dataset.name if dataset.name is not None else dataset.identifier
 
             if self.preprocessing_sequence is not None and len(self.preprocessing_sequence) > 0:
-                for preprocessing in self.preprocessing_sequence:
-                    dataset = preprocessing.process_dataset(dataset, result_path)
+                for index, preprocessing in enumerate(self.preprocessing_sequence):
+                    print_log(f"For dataset {dataset_name}, started preprocessing step {index+1}/{len(self.preprocessing_sequence)} with {preprocessing.__class__.__name__}", include_datetime=True)
+                    dataset = preprocessing.process_dataset(dataset, self.result_path / f"step_{index+1}")
                     print_log(f"Preprocessed dataset {dataset_name} with {preprocessing.__class__.__name__}", include_datetime=True)
 
             paths[dataset_name] = {}
             for exporter in self.exporters:
                 export_format = exporter.__name__[:-8]
                 path = self.result_path / dataset_name / export_format
                 exporter.export(dataset, path, number_of_processes=self.number_of_processes)
```

### Comparing `immuneML-2.2.4/immuneML/workflows/instructions/exploratory_analysis/ExploratoryAnalysisInstruction.py` & `immuneML-2.2.5/immuneML/workflows/instructions/exploratory_analysis/ExploratoryAnalysisInstruction.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/workflows/instructions/exploratory_analysis/ExploratoryAnalysisUnit.py` & `immuneML-2.2.5/immuneML/workflows/instructions/exploratory_analysis/ExploratoryAnalysisUnit.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/workflows/instructions/quickstart.py` & `immuneML-2.2.5/immuneML/workflows/instructions/quickstart.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/workflows/instructions/subsampling/SubsamplingInstruction.py` & `immuneML-2.2.5/immuneML/workflows/instructions/subsampling/SubsamplingInstruction.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/workflows/instructions/subsampling/SubsamplingState.py` & `immuneML-2.2.5/immuneML/workflows/instructions/subsampling/SubsamplingState.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/workflows/steps/DataEncoder.py` & `immuneML-2.2.5/immuneML/workflows/steps/DataEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/workflows/steps/MLMethodAssessment.py` & `immuneML-2.2.5/immuneML/workflows/steps/MLMethodAssessment.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from sklearn import metrics
 
 from immuneML.environment.Label import Label
 from immuneML.ml_methods.MLMethod import MLMethod
 from immuneML.ml_methods.util.Util import Util
 from immuneML.ml_metrics import ml_metrics
 from immuneML.ml_metrics.Metric import Metric
+from immuneML.ml_metrics.MetricUtil import MetricUtil
 from immuneML.util.PathBuilder import PathBuilder
 from immuneML.workflows.steps.MLMethodAssessmentParams import MLMethodAssessmentParams
 from immuneML.workflows.steps.Step import Step
 
 
 class MLMethodAssessment(Step):
     fieldnames = ["run", "optimal_method_params", "method", "encoding_params", "encoding", "evaluated_on"]
@@ -52,19 +53,20 @@
 
         metrics_with_optim_metric = set(metrics_list)
         metrics_with_optim_metric.add(optimization_metric)
 
         metrics_with_optim_metric = sorted(list(metrics_with_optim_metric), key=lambda metric: metric.name)
 
         for metric in metrics_with_optim_metric:
-            score = MLMethodAssessment._score_for_metric(metric=metric,
-                                                         predicted_y=predicted_y[label.name],
-                                                         true_y=true_y[label.name],
-                                                         classes=label.values,
-                                                         predicted_proba_y=predicted_proba_y)
+            score = MetricUtil.score_for_metric(metric=metric,
+                                                predicted_y=predicted_y[label.name],
+                                                true_y=true_y[label.name],
+                                                classes=label.values,
+                                                predicted_proba_y=predicted_proba_y)
+
             results[f"{label.name}_{metric.name.lower()}"] = score
             scores[metric.name.lower()] = score
 
         results["split_index"] = split_index
 
         df = pd.DataFrame([results])
 
@@ -72,45 +74,14 @@
             df.to_csv(ml_score_path, mode='a', header=False, index=False)
         else:
             df.to_csv(ml_score_path, index=False)
 
         return scores
 
     @staticmethod
-    def _score_for_metric(metric: Metric, predicted_y, predicted_proba_y, true_y, classes):
-        if hasattr(ml_metrics, metric.value):
-            fn = getattr(ml_metrics, metric.value)
-        else:
-            fn = getattr(metrics, metric.value)
-
-        true_y, predicted_y = Util.binarize_label_classes(true_y=true_y, predicted_y=predicted_y, classes=classes)
-
-        try:
-            if metric in Metric.get_probability_based_metric_types():
-                predictions = predicted_proba_y
-                if predicted_proba_y is None:
-                    warnings.warn(f"MLMethodAssessment: metric {metric} is specified, but the chosen ML method does not output "
-                                  f"class probabilities. Using predicted classes instead...")
-                    predictions = predicted_y
-            else:
-                predictions = predicted_y
-
-            if 'labels' in inspect.getfullargspec(fn).kwonlyargs or 'labels' in inspect.getfullargspec(fn).args:
-                score = fn(true_y, predictions, labels=classes)
-            else:
-                score = fn(true_y, predictions)
-
-        except ValueError as err:
-            warnings.warn(f"MLMethodAssessment: score for metric {metric.name} could not be calculated."
-                          f"\nPredicted values: {predicted_y}\nTrue values: {true_y}.\nMore details: {err}", RuntimeWarning)
-            score = "not computed"
-
-        return score
-
-    @staticmethod
     def _store_predictions(method: MLMethod, true_y, predicted_y, predicted_proba_y_per_class, label: Label, predictions_path, summary_path=None,
                            example_ids: list = None, split_index: int = None):
 
         df = pd.DataFrame()
         df["example_id"] = example_ids
         df["split_index"] = [split_index for i in range(len(example_ids))]
```

### Comparing `immuneML-2.2.4/immuneML/workflows/steps/MLMethodAssessmentParams.py` & `immuneML-2.2.5/immuneML/workflows/steps/MLMethodAssessmentParams.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/workflows/steps/MLMethodTrainer.py` & `immuneML-2.2.5/immuneML/workflows/steps/MLMethodTrainer.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/workflows/steps/MLMethodTrainerParams.py` & `immuneML-2.2.5/immuneML/workflows/steps/MLMethodTrainerParams.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/workflows/steps/SignalImplanter.py` & `immuneML-2.2.5/immuneML/workflows/steps/SignalImplanter.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/workflows/steps/Step.py` & `immuneML-2.2.5/immuneML/workflows/steps/Step.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/workflows/steps/data_splitter/DataSplitter.py` & `immuneML-2.2.5/immuneML/workflows/steps/data_splitter/DataSplitter.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/workflows/steps/data_splitter/DataSplitterParams.py` & `immuneML-2.2.5/immuneML/workflows/steps/data_splitter/DataSplitterParams.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/workflows/steps/data_splitter/LeaveOneOutSplitter.py` & `immuneML-2.2.5/immuneML/workflows/steps/data_splitter/LeaveOneOutSplitter.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/workflows/steps/data_splitter/ManualSplitter.py` & `immuneML-2.2.5/immuneML/workflows/steps/data_splitter/ManualSplitter.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML/workflows/steps/data_splitter/Util.py` & `immuneML-2.2.5/immuneML/workflows/steps/data_splitter/Util.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/immuneML.egg-info/PKG-INFO` & `immuneML-2.2.5/immuneML.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: immuneML
-Version: 2.2.4
+Version: 2.2.5
 Summary: immuneML is a software platform for machine learning analysis of immune receptor repertoires.
 Home-page: https://github.com/uio-bmi/immuneML
 Author: immuneML Team
 Author-email: milenpa@student.matnat.uio.no
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `immuneML-2.2.4/immuneML.egg-info/SOURCES.txt` & `immuneML-2.2.5/immuneML.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -112,26 +112,30 @@
 immuneML/config/default_params/ml_methods/atchley_kmer_mil_classifier_params.yaml
 immuneML/config/default_params/ml_methods/deep_rc_params.yaml
 immuneML/config/default_params/ml_methods/ml_method_params.yaml
 immuneML/config/default_params/ml_methods/receptor_cnn_params.yaml
 immuneML/config/default_params/ml_methods/tcrdist_classifier_params.yaml
 immuneML/config/default_params/motif_instantiation_strategy/gapped_kmer_params.yaml
 immuneML/config/default_params/preprocessing/duplicate_sequence_filter_params.yaml
+immuneML/config/default_params/preprocessing/sequence_length_filter_params.yaml
+immuneML/config/default_params/reports/amino_acid_frequency_distribution_params.yaml
 immuneML/config/default_params/reports/coefficients_params.yaml
 immuneML/config/default_params/reports/cv_feature_performance_params.yaml
 immuneML/config/default_params/reports/cytoscape_network_exporter_params.yaml
 immuneML/config/default_params/reports/deep_rc_motif_discovery_params.yaml
 immuneML/config/default_params/reports/design_matrix_exporter_params.yaml
 immuneML/config/default_params/reports/feature_comparison_params.yaml
 immuneML/config/default_params/reports/feature_value_barplot_params.yaml
 immuneML/config/default_params/reports/ml_settings_performance_params.yaml
 immuneML/config/default_params/reports/motif_seed_recovery_params.yaml
 immuneML/config/default_params/reports/receptor_dataset_overview_params.yaml
 immuneML/config/default_params/reports/recovered_significant_features_params.yaml
 immuneML/config/default_params/reports/reference_sequence_overlap_params.yaml
+immuneML/config/default_params/reports/repertoire_clonotype_summary_params.yaml
+immuneML/config/default_params/reports/sequence_length_distribution_params.yaml
 immuneML/config/default_params/reports/significant_features_params.yaml
 immuneML/config/default_params/reports/tcrdist_motif_discovery_params.yaml
 immuneML/config/default_params/signal_implanting_strategy/full_sequence_implanting_params.yaml
 immuneML/config/default_params/signal_implanting_strategy/healthy_sequence_implanting_params.yaml
 immuneML/data_model/DatasetItem.py
 immuneML/data_model/__init__.py
 immuneML/data_model/cell/Cell.py
@@ -153,15 +157,14 @@
 immuneML/data_model/receptor/ReceptorBuilder.py
 immuneML/data_model/receptor/RegionType.py
 immuneML/data_model/receptor/TCABReceptor.py
 immuneML/data_model/receptor/TCGDReceptor.py
 immuneML/data_model/receptor/__init__.py
 immuneML/data_model/receptor/receptor_sequence/Chain.py
 immuneML/data_model/receptor/receptor_sequence/ReceptorSequence.py
-immuneML/data_model/receptor/receptor_sequence/ReceptorSequenceList.py
 immuneML/data_model/receptor/receptor_sequence/SequenceAnnotation.py
 immuneML/data_model/receptor/receptor_sequence/SequenceFrameType.py
 immuneML/data_model/receptor/receptor_sequence/SequenceMetadata.py
 immuneML/data_model/receptor/receptor_sequence/__init__.py
 immuneML/data_model/repertoire/Repertoire.py
 immuneML/data_model/repertoire/__init__.py
 immuneML/dev_util/__init__.py
@@ -305,30 +308,33 @@
 immuneML/ml_methods/__init__.py
 immuneML/ml_methods/pytorch_implementations/PyTorchLogisticRegression.py
 immuneML/ml_methods/pytorch_implementations/PyTorchReceptorCNN.py
 immuneML/ml_methods/pytorch_implementations/__init__.py
 immuneML/ml_methods/util/Util.py
 immuneML/ml_methods/util/__init__.py
 immuneML/ml_metrics/Metric.py
+immuneML/ml_metrics/MetricUtil.py
 immuneML/ml_metrics/__init__.py
 immuneML/ml_metrics/ml_metrics.py
 immuneML/pairwise_repertoire_comparison/ComparisonData.py
 immuneML/pairwise_repertoire_comparison/ComparisonDataBatch.py
 immuneML/pairwise_repertoire_comparison/PairwiseRepertoireComparison.py
 immuneML/pairwise_repertoire_comparison/__init__.py
 immuneML/preprocessing/Preprocessor.py
+immuneML/preprocessing/ReferenceSequenceAnnotator.py
 immuneML/preprocessing/SubjectRepertoireCollector.py
 immuneML/preprocessing/__init__.py
 immuneML/preprocessing/filters/ChainRepertoireFilter.py
 immuneML/preprocessing/filters/ClonesPerRepertoireFilter.py
 immuneML/preprocessing/filters/CountAggregationFunction.py
 immuneML/preprocessing/filters/CountPerSequenceFilter.py
 immuneML/preprocessing/filters/DuplicateSequenceFilter.py
 immuneML/preprocessing/filters/Filter.py
 immuneML/preprocessing/filters/MetadataRepertoireFilter.py
+immuneML/preprocessing/filters/SequenceLengthFilter.py
 immuneML/preprocessing/filters/__init__.py
 immuneML/presentation/InstructionPresentation.py
 immuneML/presentation/PresentationFactory.py
 immuneML/presentation/PresentationFormat.py
 immuneML/presentation/TemplateParser.py
 immuneML/presentation/__init__.py
 immuneML/presentation/html/DatasetExportHTMLBuilder.py
@@ -356,19 +362,21 @@
 immuneML/presentation/html/templates/css/custom.css
 immuneML/reports/PlotlyUtil.py
 immuneML/reports/Report.py
 immuneML/reports/ReportOutput.py
 immuneML/reports/ReportResult.py
 immuneML/reports/ReportUtil.py
 immuneML/reports/__init__.py
+immuneML/reports/data_reports/AminoAcidFrequencyDistribution.py
 immuneML/reports/data_reports/CytoscapeNetworkExporter.py
 immuneML/reports/data_reports/DataReport.py
 immuneML/reports/data_reports/GLIPH2Exporter.py
 immuneML/reports/data_reports/ReceptorDatasetOverview.py
 immuneML/reports/data_reports/RecoveredSignificantFeatures.py
+immuneML/reports/data_reports/RepertoireClonotypeSummary.py
 immuneML/reports/data_reports/SequenceLengthDistribution.py
 immuneML/reports/data_reports/SequencesWithSignificantKmers.py
 immuneML/reports/data_reports/SignificantFeatures.py
 immuneML/reports/data_reports/SignificantKmerPositions.py
 immuneML/reports/data_reports/SimpleDatasetOverview.py
 immuneML/reports/data_reports/__init__.py
 immuneML/reports/encoding_reports/DesignMatrixExporter.py
```

### Comparing `immuneML-2.2.4/scripts/specification_util.py` & `immuneML-2.2.5/scripts/specification_util.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/scripts/specs_docs_generation.py` & `immuneML-2.2.5/scripts/specs_docs_generation.py`

 * *Files identical despite different names*

### Comparing `immuneML-2.2.4/setup.py` & `immuneML-2.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     version=Constants.VERSION,
     description="immuneML is a software platform for machine learning analysis of immune receptor repertoires.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="immuneML Team",
     author_email="milenpa@student.matnat.uio.no",
     url="https://github.com/uio-bmi/immuneML",
-    install_requires=["numpy>=1.18.5,<=1.23.5", "pytest>=4", "pandas>=1", "PyYAML>=5.3", "scikit-learn>=0.23", "gensim>=3.8,<4", "matplotlib>=3.1",
+    install_requires=["numpy>=1.18.5,<=1.23.5", "pytest>=4", "pandas>=1,<=1.5.3", "PyYAML>=5.3", "scikit-learn>=0.23", "gensim>=3.8,<4", "matplotlib>=3.1",
                       "editdistance==0.5.3", "regex", "tzlocal", "airr>=1,<1.4", "fishersapi", "pystache", "torch>=1.5.1", "dill>=0.3",
                       "tensorboard>=1.14.0", "plotly>=4", "logomaker>=0.8",  "matplotlib-venn>=0.11", "scipy", "Cython"],
     extras_require={
         "TCRdist": ["parasail==1.2", "tcrdist3>=0.1.6"]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
```

