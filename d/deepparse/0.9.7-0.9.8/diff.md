# Comparing `tmp/deepparse-0.9.7.tar.gz` & `tmp/deepparse-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepparse-0.9.7.tar", last modified: Mon May 22 13:13:16 2023, max compression
+gzip compressed data, was "deepparse-0.9.8.tar", last modified: Thu May 25 15:49:14 2023, max compression
```

## Comparing `deepparse-0.9.7.tar` & `deepparse-0.9.8.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.332264 deepparse-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-22 13:13:05.000000 deepparse-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-05-22 13:13:16.332264 deepparse-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-05-22 13:13:05.000000 deepparse-0.9.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.316264 deepparse-0.9.7/deepparse/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.320264 deepparse-0.9.7/deepparse/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/cli/download_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/cli/download_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/cli/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/cli/parser_arguments_adder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/cli/retrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/cli/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/cli/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.320264 deepparse-0.9.7/deepparse/comparer/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/comparer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/comparer/addresses_comparer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/comparer/formatted_compared_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/comparer/formatted_compared_addresses_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/comparer/formatted_compared_addresses_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.320264 deepparse-0.9.7/deepparse/converter/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/converter/data_padder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/converter/data_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/converter/data_processor_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/converter/target_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.320264 deepparse-0.9.7/deepparse/data_validation/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/data_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/data_validation/data_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.320264 deepparse-0.9.7/deepparse/dataset_container/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/dataset_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/dataset_container/dataset_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/dataset_container/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.320264 deepparse-0.9.7/deepparse/embeddings_models/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/embeddings_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/embeddings_models/bpemb_embeddings_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/embeddings_models/embeddings_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/embeddings_models/embeddings_model_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/embeddings_models/fasttext_embeddings_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/embeddings_models/magnitude_embeddings_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.320264 deepparse-0.9.7/deepparse/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/errors/data_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/errors/model_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/errors/server_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/fasttext_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.320264 deepparse-0.9.7/deepparse/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/metrics/nll_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.320264 deepparse-0.9.7/deepparse/network/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/network/bpemb_seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/network/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/network/embedding_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/network/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/network/fasttext_seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/network/model_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/network/seq2seq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.324264 deepparse-0.9.7/deepparse/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65091 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/parser/address_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/parser/capturing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/parser/formatted_parsed_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/parser/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.324264 deepparse-0.9.7/deepparse/pre_processing/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/pre_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/pre_processing/pre_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.324264 deepparse-0.9.7/deepparse/vectorizer/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/vectorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/vectorizer/bpemb_vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/vectorizer/fasttext_vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/vectorizer/magnitude_vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/vectorizer/vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/vectorizer/vectorizer_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 13:13:16.000000 deepparse-0.9.7/deepparse/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/weights_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.320264 deepparse-0.9.7/deepparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-05-22 13:13:16.000000 deepparse-0.9.7/deepparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-05-22 13:13:16.000000 deepparse-0.9.7/deepparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:13:16.000000 deepparse-0.9.7/deepparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-22 13:13:16.000000 deepparse-0.9.7/deepparse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-22 13:13:16.000000 deepparse-0.9.7/deepparse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-22 13:13:16.000000 deepparse-0.9.7/deepparse.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.324264 deepparse-0.9.7/models_evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/models_evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-22 13:13:05.000000 deepparse-0.9.7/models_evaluation/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-22 13:13:05.000000 deepparse-0.9.7/models_evaluation/evaluate_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-22 13:13:05.000000 deepparse-0.9.7/models_evaluation/generate_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-22 13:13:05.000000 deepparse-0.9.7/models_evaluation/speed_test_evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.324264 deepparse-0.9.7/models_evaluation/timer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/models_evaluation/timer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-05-22 13:13:05.000000 deepparse-0.9.7/models_evaluation/timer/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-05-22 13:13:05.000000 deepparse-0.9.7/models_evaluation/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-22 13:13:05.000000 deepparse-0.9.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.324264 deepparse-0.9.7/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-22 13:13:05.000000 deepparse-0.9.7/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-22 13:13:16.332264 deepparse-0.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-22 13:13:05.000000 deepparse-0.9.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.324264 deepparse-0.9.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/base_capture_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/base_file_exist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.324264 deepparse-0.9.7/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/cli/test_download_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/cli/test_download_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/cli/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/cli/test_retrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/cli/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/cli/test_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.324264 deepparse-0.9.7/tests/comparer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/comparer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/comparer/test_addresses_comparer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/comparer/test_formatted_compared_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/comparer/test_formatted_compared_addresses_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/comparer/test_formatted_compared_addresses_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.328264 deepparse-0.9.7/tests/converter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/converter/test_data_padder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13254 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/converter/test_data_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/converter/test_data_processor_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/converter/test_target_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.328264 deepparse-0.9.7/tests/data_validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/data_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/data_validation/test_data_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.328264 deepparse-0.9.7/tests/dataset_container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/dataset_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23762 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/dataset_container/test_dataset_container.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/dataset_container/test_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.328264 deepparse-0.9.7/tests/embeddings_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/embeddings_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/embeddings_models/test_bpemb_embeddings_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/embeddings_models/test_embeddings_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/embeddings_models/test_embeddings_model_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/embeddings_models/test_fasttext_embeddings_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/embeddings_models/test_magnitude_embeddings_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.328264 deepparse-0.9.7/tests/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/metrics/test_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/metrics/test_nll_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.328264 deepparse-0.9.7/tests/models_evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/models_evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/models_evaluation/test_tools_models_evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.328264 deepparse-0.9.7/tests/network/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.328264 deepparse-0.9.7/tests/network/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/integration/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/integration/test_integration_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/integration/test_integration_embedding_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/integration/test_integration_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_bpemb_model_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_bpemb_model_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_fasttext_model_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_fasttext_model_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_model_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_model_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    18841 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/test_bpemb_seq2seq_model_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    18562 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/test_bpemb_seq2seq_model_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/test_embedding_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15212 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/test_fasttext_seq2seq_model_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    15426 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/test_fasttext_seq2seq_model_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/test_model_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/test_seq2seq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.332264 deepparse-0.9.7/tests/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.332264 deepparse-0.9.7/tests/parser/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/base_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/base_retrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_new_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_new_params_new_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_retrain_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_retrain_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_retrain_freeze_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_retrain_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    21743 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_retrain_new_address_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_test_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_reload_retrain_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_retrain_test_api_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_uri.py
--rw-r--r--   0 runner    (1001) docker     (123)    74223 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/test_address_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    70964 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/test_address_parser_retrain_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/test_address_parser_test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/test_formatted_parsed_address.py
--rw-r--r--   0 runner    (1001) docker     (123)    19555 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/test_user_fromatted_parsed_address.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.332264 deepparse-0.9.7/tests/pre_processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/pre_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/pre_processing/test_address_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)    13422 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/test_fasttext_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/test_integration_fasttext_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/test_weights_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.332264 deepparse-0.9.7/tests/vectorizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/vectorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/vectorizer/test_bpemb_vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/vectorizer/test_fasttext_vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/vectorizer/test_magnitude_vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/vectorizer/test_vectorizer_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.394719 deepparse-0.9.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-25 15:49:03.000000 deepparse-0.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-05-25 15:49:14.394719 deepparse-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-05-25 15:49:03.000000 deepparse-0.9.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.378718 deepparse-0.9.8/deepparse/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.382718 deepparse-0.9.8/deepparse/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/cli/download_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/cli/download_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/cli/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/cli/parser_arguments_adder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/cli/retrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/cli/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/cli/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.382718 deepparse-0.9.8/deepparse/comparer/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/comparer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/comparer/addresses_comparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/comparer/formatted_compared_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/comparer/formatted_compared_addresses_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/comparer/formatted_compared_addresses_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.382718 deepparse-0.9.8/deepparse/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/converter/data_padder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/converter/data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/converter/data_processor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/converter/target_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.382718 deepparse-0.9.8/deepparse/data_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/data_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/data_validation/data_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.382718 deepparse-0.9.8/deepparse/dataset_container/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/dataset_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/dataset_container/dataset_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/dataset_container/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.382718 deepparse-0.9.8/deepparse/embeddings_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/embeddings_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/embeddings_models/bpemb_embeddings_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/embeddings_models/embeddings_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/embeddings_models/embeddings_model_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/embeddings_models/fasttext_embeddings_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/embeddings_models/magnitude_embeddings_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.382718 deepparse-0.9.8/deepparse/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/errors/data_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/errors/model_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/errors/server_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/fasttext_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.382718 deepparse-0.9.8/deepparse/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/metrics/nll_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.382718 deepparse-0.9.8/deepparse/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/network/bpemb_seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/network/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/network/embedding_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/network/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/network/fasttext_seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/network/model_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/network/seq2seq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.382718 deepparse-0.9.8/deepparse/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65091 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/parser/address_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/parser/capturing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/parser/formatted_parsed_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/parser/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.382718 deepparse-0.9.8/deepparse/pre_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/pre_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/pre_processing/pre_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.386718 deepparse-0.9.8/deepparse/vectorizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/vectorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/vectorizer/bpemb_vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/vectorizer/fasttext_vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/vectorizer/magnitude_vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/vectorizer/vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/vectorizer/vectorizer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 15:49:14.000000 deepparse-0.9.8/deepparse/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-25 15:49:03.000000 deepparse-0.9.8/deepparse/weights_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.378718 deepparse-0.9.8/deepparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-05-25 15:49:14.000000 deepparse-0.9.8/deepparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-05-25 15:49:14.000000 deepparse-0.9.8/deepparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:49:14.000000 deepparse-0.9.8/deepparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-25 15:49:14.000000 deepparse-0.9.8/deepparse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-25 15:49:14.000000 deepparse-0.9.8/deepparse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-25 15:49:14.000000 deepparse-0.9.8/deepparse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.386718 deepparse-0.9.8/models_evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:03.000000 deepparse-0.9.8/models_evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-25 15:49:03.000000 deepparse-0.9.8/models_evaluation/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-25 15:49:03.000000 deepparse-0.9.8/models_evaluation/evaluate_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-25 15:49:03.000000 deepparse-0.9.8/models_evaluation/generate_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-25 15:49:03.000000 deepparse-0.9.8/models_evaluation/speed_test_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.386718 deepparse-0.9.8/models_evaluation/timer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:03.000000 deepparse-0.9.8/models_evaluation/timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-05-25 15:49:03.000000 deepparse-0.9.8/models_evaluation/timer/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-05-25 15:49:03.000000 deepparse-0.9.8/models_evaluation/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-25 15:49:03.000000 deepparse-0.9.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.386718 deepparse-0.9.8/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:03.000000 deepparse-0.9.8/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-25 15:49:03.000000 deepparse-0.9.8/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-25 15:49:14.394719 deepparse-0.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-25 15:49:03.000000 deepparse-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.386718 deepparse-0.9.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/base_capture_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/base_file_exist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.386718 deepparse-0.9.8/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/cli/test_download_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/cli/test_download_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/cli/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/cli/test_retrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/cli/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/cli/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.386718 deepparse-0.9.8/tests/comparer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/comparer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/comparer/test_addresses_comparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/comparer/test_formatted_compared_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/comparer/test_formatted_compared_addresses_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/comparer/test_formatted_compared_addresses_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.386718 deepparse-0.9.8/tests/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/converter/test_data_padder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13254 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/converter/test_data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/converter/test_data_processor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/converter/test_target_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.386718 deepparse-0.9.8/tests/data_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/data_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/data_validation/test_data_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.386718 deepparse-0.9.8/tests/dataset_container/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/dataset_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23762 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/dataset_container/test_dataset_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/dataset_container/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.390718 deepparse-0.9.8/tests/embeddings_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/embeddings_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/embeddings_models/test_bpemb_embeddings_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/embeddings_models/test_embeddings_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/embeddings_models/test_embeddings_model_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/embeddings_models/test_fasttext_embeddings_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/embeddings_models/test_magnitude_embeddings_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.390718 deepparse-0.9.8/tests/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/metrics/test_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/metrics/test_nll_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.390718 deepparse-0.9.8/tests/models_evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/models_evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/models_evaluation/test_tools_models_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.390718 deepparse-0.9.8/tests/network/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/network/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.390718 deepparse-0.9.8/tests/network/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/network/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/network/integration/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/network/integration/test_integration_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/network/integration/test_integration_embedding_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/network/integration/test_integration_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/network/integration/test_integration_seq2seq_bpemb_model_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/network/integration/test_integration_seq2seq_bpemb_model_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/network/integration/test_integration_seq2seq_fasttext_model_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/network/integration/test_integration_seq2seq_fasttext_model_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/network/integration/test_integration_seq2seq_model_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/network/integration/test_integration_seq2seq_model_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18841 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/network/test_bpemb_seq2seq_model_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18562 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/network/test_bpemb_seq2seq_model_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/network/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/network/test_embedding_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/network/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15212 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/network/test_fasttext_seq2seq_model_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15426 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/network/test_fasttext_seq2seq_model_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/network/test_model_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/network/test_seq2seq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.390718 deepparse-0.9.8/tests/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.394719 deepparse-0.9.8/tests/parser/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/integration/base_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/integration/base_retrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/integration/test_integration_address_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_new_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_new_params_new_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_retrain_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_retrain_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_retrain_freeze_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_retrain_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21743 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_retrain_new_address_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_test_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/integration/test_integration_reload_retrain_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/integration/test_integration_retrain_test_api_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/integration/test_integration_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74223 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/test_address_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70964 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/test_address_parser_retrain_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/test_address_parser_test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/test_formatted_parsed_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19555 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/parser/test_user_fromatted_parsed_address.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.394719 deepparse-0.9.8/tests/pre_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/pre_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/pre_processing/test_address_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13422 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/test_fasttext_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/test_integration_fasttext_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/test_weights_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:14.394719 deepparse-0.9.8/tests/vectorizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/vectorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/vectorizer/test_bpemb_vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/vectorizer/test_fasttext_vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/vectorizer/test_magnitude_vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-25 15:49:03.000000 deepparse-0.9.8/tests/vectorizer/test_vectorizer_factory.py
```

### Comparing `deepparse-0.9.7/LICENSE` & `deepparse-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/PKG-INFO` & `deepparse-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: deepparse
-Version: 0.9.7
+Version: 0.9.8
 Summary: A library for parsing multinational street addresses using deep learning.
 Home-page: https://deepparse.org/
-Download-URL: https://github.com/GRAAL-Research/deepparse/archive/v0.9.7.zip
+Download-URL: https://github.com/GRAAL-Research/deepparse/archive/v0.9.8.zip
 Author: Marouane Yassine, David Beauchemin
 Author-email: marouane.yassine.1@ulaval.ca, david.beauchemin.5@ulaval.ca
 License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: deepparse Version: 0.9.7 Summary: A library for
+Metadata-Version: 2.1 Name: deepparse Version: 0.9.8 Summary: A library for
 parsing multinational street addresses using deep learning. Home-page: https://
 deepparse.org/ Download-URL: https://github.com/GRAAL-Research/deepparse/
-archive/v0.9.7.zip Author: Marouane Yassine, David Beauchemin Author-email:
+archive/v0.9.8.zip Author: Marouane Yassine, David Beauchemin Author-email:
 marouane.yassine.1@ulaval.ca, david.beauchemin.5@ulaval.ca License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Education Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 GNU Lesser General Public License v3 (LGPLv3) Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `deepparse-0.9.7/README.md` & `deepparse-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/cli/download_model.py` & `deepparse-0.9.8/deepparse/cli/download_model.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/cli/download_models.py` & `deepparse-0.9.8/deepparse/cli/download_models.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/cli/parse.py` & `deepparse-0.9.8/deepparse/cli/parse.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/cli/parser_arguments_adder.py` & `deepparse-0.9.8/deepparse/cli/parser_arguments_adder.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/cli/retrain.py` & `deepparse-0.9.8/deepparse/cli/retrain.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/cli/test.py` & `deepparse-0.9.8/deepparse/cli/test.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/cli/tools.py` & `deepparse-0.9.8/deepparse/cli/tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/comparer/addresses_comparer.py` & `deepparse-0.9.8/deepparse/comparer/addresses_comparer.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/comparer/formatted_compared_addresses.py` & `deepparse-0.9.8/deepparse/comparer/formatted_compared_addresses.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/comparer/formatted_compared_addresses_raw.py` & `deepparse-0.9.8/deepparse/comparer/formatted_compared_addresses_raw.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/comparer/formatted_compared_addresses_tags.py` & `deepparse-0.9.8/deepparse/comparer/formatted_compared_addresses_tags.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/converter/data_padder.py` & `deepparse-0.9.8/deepparse/converter/data_padder.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/converter/data_processor.py` & `deepparse-0.9.8/deepparse/converter/data_processor.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/converter/data_processor_factory.py` & `deepparse-0.9.8/deepparse/converter/data_processor_factory.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/converter/target_converter.py` & `deepparse-0.9.8/deepparse/converter/target_converter.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/data_validation/data_validation.py` & `deepparse-0.9.8/deepparse/data_validation/data_validation.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/dataset_container/dataset_container.py` & `deepparse-0.9.8/deepparse/dataset_container/dataset_container.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/dataset_container/tools.py` & `deepparse-0.9.8/deepparse/dataset_container/tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/embeddings_models/bpemb_embeddings_model.py` & `deepparse-0.9.8/deepparse/embeddings_models/bpemb_embeddings_model.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/embeddings_models/embeddings_model_factory.py` & `deepparse-0.9.8/deepparse/embeddings_models/embeddings_model_factory.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/embeddings_models/fasttext_embeddings_model.py` & `deepparse-0.9.8/deepparse/embeddings_models/fasttext_embeddings_model.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/embeddings_models/magnitude_embeddings_model.py` & `deepparse-0.9.8/deepparse/embeddings_models/magnitude_embeddings_model.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/fasttext_tools.py` & `deepparse-0.9.8/deepparse/fasttext_tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/network/bpemb_seq2seq.py` & `deepparse-0.9.8/deepparse/network/bpemb_seq2seq.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/network/decoder.py` & `deepparse-0.9.8/deepparse/network/decoder.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/network/embedding_network.py` & `deepparse-0.9.8/deepparse/network/embedding_network.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/network/encoder.py` & `deepparse-0.9.8/deepparse/network/encoder.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/network/fasttext_seq2seq.py` & `deepparse-0.9.8/deepparse/network/fasttext_seq2seq.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/network/model_factory.py` & `deepparse-0.9.8/deepparse/network/model_factory.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/network/seq2seq.py` & `deepparse-0.9.8/deepparse/network/seq2seq.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/parser/address_parser.py` & `deepparse-0.9.8/deepparse/parser/address_parser.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/parser/formatted_parsed_address.py` & `deepparse-0.9.8/deepparse/parser/formatted_parsed_address.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/parser/tools.py` & `deepparse-0.9.8/deepparse/parser/tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/pre_processing/pre_processor.py` & `deepparse-0.9.8/deepparse/pre_processing/pre_processor.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/tools.py` & `deepparse-0.9.8/deepparse/tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/vectorizer/bpemb_vectorizer.py` & `deepparse-0.9.8/deepparse/vectorizer/bpemb_vectorizer.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/vectorizer/fasttext_vectorizer.py` & `deepparse-0.9.8/deepparse/vectorizer/fasttext_vectorizer.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/vectorizer/magnitude_vectorizer.py` & `deepparse-0.9.8/deepparse/vectorizer/magnitude_vectorizer.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/vectorizer/vectorizer.py` & `deepparse-0.9.8/deepparse/vectorizer/vectorizer.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/vectorizer/vectorizer_factory.py` & `deepparse-0.9.8/deepparse/vectorizer/vectorizer_factory.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse/weights_tools.py` & `deepparse-0.9.8/deepparse/weights_tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/deepparse.egg-info/PKG-INFO` & `deepparse-0.9.8/deepparse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: deepparse
-Version: 0.9.7
+Version: 0.9.8
 Summary: A library for parsing multinational street addresses using deep learning.
 Home-page: https://deepparse.org/
-Download-URL: https://github.com/GRAAL-Research/deepparse/archive/v0.9.7.zip
+Download-URL: https://github.com/GRAAL-Research/deepparse/archive/v0.9.8.zip
 Author: Marouane Yassine, David Beauchemin
 Author-email: marouane.yassine.1@ulaval.ca, david.beauchemin.5@ulaval.ca
 License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: deepparse Version: 0.9.7 Summary: A library for
+Metadata-Version: 2.1 Name: deepparse Version: 0.9.8 Summary: A library for
 parsing multinational street addresses using deep learning. Home-page: https://
 deepparse.org/ Download-URL: https://github.com/GRAAL-Research/deepparse/
-archive/v0.9.7.zip Author: Marouane Yassine, David Beauchemin Author-email:
+archive/v0.9.8.zip Author: Marouane Yassine, David Beauchemin Author-email:
 marouane.yassine.1@ulaval.ca, david.beauchemin.5@ulaval.ca License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Education Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 GNU Lesser General Public License v3 (LGPLv3) Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `deepparse-0.9.7/deepparse.egg-info/SOURCES.txt` & `deepparse-0.9.8/deepparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/models_evaluation/evaluate_model.py` & `deepparse-0.9.8/models_evaluation/evaluate_model.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/models_evaluation/generate_tables.py` & `deepparse-0.9.8/models_evaluation/generate_tables.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/models_evaluation/speed_test_evaluation.py` & `deepparse-0.9.8/models_evaluation/speed_test_evaluation.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/models_evaluation/timer/timer.py` & `deepparse-0.9.8/models_evaluation/timer/timer.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/models_evaluation/tools.py` & `deepparse-0.9.8/models_evaluation/tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/setup.py` & `deepparse-0.9.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,19 +70,20 @@
         packages=packages,
         install_requires=[
             "numpy",
             "torch",
             "bpemb",
             "gensim>=4.0.0",
             "requests",
-            "fasttext",
+            "fasttext-wheel",
             "pymagnitude-light",
             "poutyne",
             "pandas",
             "urllib3",
+            "cloudpathlib[s3, gs, azure]",
         ],
         python_requires=">=3.8",
         description="A library for parsing multinational street addresses using deep learning.",
         long_description=readme,
         long_description_content_type="text/markdown",
         extras_require={"colorama": "colorama>=0.4.3"},
     )
```

### Comparing `deepparse-0.9.7/tests/cli/test_download_model.py` & `deepparse-0.9.8/tests/cli/test_download_model.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/cli/test_download_models.py` & `deepparse-0.9.8/tests/cli/test_download_models.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/cli/test_parse.py` & `deepparse-0.9.8/tests/cli/test_parse.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/cli/test_retrain.py` & `deepparse-0.9.8/tests/cli/test_retrain.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/cli/test_testing.py` & `deepparse-0.9.8/tests/cli/test_testing.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/cli/test_tools.py` & `deepparse-0.9.8/tests/cli/test_tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/comparer/test_addresses_comparer.py` & `deepparse-0.9.8/tests/comparer/test_addresses_comparer.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/comparer/test_formatted_compared_addresses.py` & `deepparse-0.9.8/tests/comparer/test_formatted_compared_addresses.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/comparer/test_formatted_compared_addresses_raw.py` & `deepparse-0.9.8/tests/comparer/test_formatted_compared_addresses_raw.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/comparer/test_formatted_compared_addresses_tags.py` & `deepparse-0.9.8/tests/comparer/test_formatted_compared_addresses_tags.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/converter/test_data_padder.py` & `deepparse-0.9.8/tests/converter/test_data_padder.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/converter/test_data_processor.py` & `deepparse-0.9.8/tests/converter/test_data_processor.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/converter/test_data_processor_factory.py` & `deepparse-0.9.8/tests/converter/test_data_processor_factory.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/converter/test_target_converter.py` & `deepparse-0.9.8/tests/converter/test_target_converter.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/data_validation/test_data_validation.py` & `deepparse-0.9.8/tests/data_validation/test_data_validation.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/dataset_container/test_dataset_container.py` & `deepparse-0.9.8/tests/dataset_container/test_dataset_container.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/dataset_container/test_tools.py` & `deepparse-0.9.8/tests/dataset_container/test_tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/embeddings_models/test_bpemb_embeddings_model.py` & `deepparse-0.9.8/tests/embeddings_models/test_bpemb_embeddings_model.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/embeddings_models/test_embeddings_model.py` & `deepparse-0.9.8/tests/embeddings_models/test_embeddings_model.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/embeddings_models/test_embeddings_model_factory.py` & `deepparse-0.9.8/tests/embeddings_models/test_embeddings_model_factory.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/embeddings_models/test_fasttext_embeddings_model.py` & `deepparse-0.9.8/tests/embeddings_models/test_fasttext_embeddings_model.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/embeddings_models/test_magnitude_embeddings_model.py` & `deepparse-0.9.8/tests/embeddings_models/test_magnitude_embeddings_model.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/metrics/test_accuracy.py` & `deepparse-0.9.8/tests/metrics/test_accuracy.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/metrics/test_nll_loss.py` & `deepparse-0.9.8/tests/metrics/test_nll_loss.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/models_evaluation/test_tools_models_evaluation.py` & `deepparse-0.9.8/tests/models_evaluation/test_tools_models_evaluation.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/network/base.py` & `deepparse-0.9.8/tests/network/base.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/network/integration/base.py` & `deepparse-0.9.8/tests/network/integration/base.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/network/integration/test_integration_decoder.py` & `deepparse-0.9.8/tests/network/integration/test_integration_decoder.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/network/integration/test_integration_embedding_network.py` & `deepparse-0.9.8/tests/network/integration/test_integration_embedding_network.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/network/integration/test_integration_encoder.py` & `deepparse-0.9.8/tests/network/integration/test_integration_encoder.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_bpemb_model_cpu.py` & `deepparse-0.9.8/tests/network/integration/test_integration_seq2seq_bpemb_model_cpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_bpemb_model_gpu.py` & `deepparse-0.9.8/tests/network/integration/test_integration_seq2seq_bpemb_model_gpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_fasttext_model_cpu.py` & `deepparse-0.9.8/tests/network/integration/test_integration_seq2seq_fasttext_model_cpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_fasttext_model_gpu.py` & `deepparse-0.9.8/tests/network/integration/test_integration_seq2seq_fasttext_model_gpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_model_cpu.py` & `deepparse-0.9.8/tests/network/integration/test_integration_seq2seq_model_cpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_model_gpu.py` & `deepparse-0.9.8/tests/network/integration/test_integration_seq2seq_model_gpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/network/test_bpemb_seq2seq_model_cpu.py` & `deepparse-0.9.8/tests/network/test_bpemb_seq2seq_model_cpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/network/test_bpemb_seq2seq_model_gpu.py` & `deepparse-0.9.8/tests/network/test_bpemb_seq2seq_model_gpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/network/test_decoder.py` & `deepparse-0.9.8/tests/network/test_decoder.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/network/test_embedding_network.py` & `deepparse-0.9.8/tests/network/test_embedding_network.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/network/test_encoder.py` & `deepparse-0.9.8/tests/network/test_encoder.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/network/test_fasttext_seq2seq_model_cpu.py` & `deepparse-0.9.8/tests/network/test_fasttext_seq2seq_model_cpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/network/test_fasttext_seq2seq_model_gpu.py` & `deepparse-0.9.8/tests/network/test_fasttext_seq2seq_model_gpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/network/test_model_factory.py` & `deepparse-0.9.8/tests/network/test_model_factory.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/network/test_seq2seq.py` & `deepparse-0.9.8/tests/network/test_seq2seq.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/base.py` & `deepparse-0.9.8/tests/parser/base.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/integration/base_predict.py` & `deepparse-0.9.8/tests/parser/integration/base_predict.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/integration/base_retrain.py` & `deepparse-0.9.8/tests/parser/integration/base_retrain.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser.py` & `deepparse-0.9.8/tests/parser/integration/test_integration_address_parser.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_cpu.py` & `deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_cpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_gpu.py` & `deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_gpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_new_params.py` & `deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_new_params.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_new_params_new_tags.py` & `deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_new_params_new_tags.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_retrain_api.py` & `deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_retrain_api.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_retrain_cpu.py` & `deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_retrain_cpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_retrain_freeze_layers.py` & `deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_retrain_freeze_layers.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_retrain_gpu.py` & `deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_retrain_gpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_retrain_new_address_components.py` & `deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_retrain_new_address_components.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_test_api.py` & `deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_test_api.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_test_cpu.py` & `deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_test_cpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_test_gpu.py` & `deepparse-0.9.8/tests/parser/integration/test_integration_address_parser_test_gpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/integration/test_integration_reload_retrain_parser.py` & `deepparse-0.9.8/tests/parser/integration/test_integration_reload_retrain_parser.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/integration/test_integration_retrain_test_api_integration.py` & `deepparse-0.9.8/tests/parser/integration/test_integration_retrain_test_api_integration.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/integration/test_integration_uri.py` & `deepparse-0.9.8/tests/parser/integration/test_integration_uri.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/test_address_parser.py` & `deepparse-0.9.8/tests/parser/test_address_parser.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/test_address_parser_retrain_api.py` & `deepparse-0.9.8/tests/parser/test_address_parser_retrain_api.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/test_address_parser_test_api.py` & `deepparse-0.9.8/tests/parser/test_address_parser_test_api.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/test_formatted_parsed_address.py` & `deepparse-0.9.8/tests/parser/test_formatted_parsed_address.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/test_tools.py` & `deepparse-0.9.8/tests/parser/test_tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/parser/test_user_fromatted_parsed_address.py` & `deepparse-0.9.8/tests/parser/test_user_fromatted_parsed_address.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/pre_processing/test_address_cleaner.py` & `deepparse-0.9.8/tests/pre_processing/test_address_cleaner.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/test_fasttext_tools.py` & `deepparse-0.9.8/tests/test_fasttext_tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/test_integration_fasttext_tools.py` & `deepparse-0.9.8/tests/test_integration_fasttext_tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/test_tools.py` & `deepparse-0.9.8/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/test_weights_tools.py` & `deepparse-0.9.8/tests/test_weights_tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/tools.py` & `deepparse-0.9.8/tests/tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/vectorizer/test_bpemb_vectorizer.py` & `deepparse-0.9.8/tests/vectorizer/test_bpemb_vectorizer.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/vectorizer/test_fasttext_vectorizer.py` & `deepparse-0.9.8/tests/vectorizer/test_fasttext_vectorizer.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/vectorizer/test_magnitude_vectorizer.py` & `deepparse-0.9.8/tests/vectorizer/test_magnitude_vectorizer.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.7/tests/vectorizer/test_vectorizer_factory.py` & `deepparse-0.9.8/tests/vectorizer/test_vectorizer_factory.py`

 * *Files identical despite different names*

