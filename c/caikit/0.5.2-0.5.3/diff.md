# Comparing `tmp/caikit-0.5.2.tar.gz` & `tmp/caikit-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-0.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "caikit-0.5.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `caikit-0.5.2.tar` & `caikit-0.5.3.tar`

### file list

```diff
@@ -1,305 +1,305 @@
--rw-r--r--   0        0        0       60 2023-05-23 23:02:11.613405 caikit-0.5.2/.coveragerc
--rw-r--r--   0        0        0      676 2023-05-23 23:02:11.613405 caikit-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      579 2023-05-23 23:02:11.613405 caikit-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-05-23 23:02:11.613405 caikit-0.5.2/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0        0        0      106 2023-05-23 23:02:11.613405 caikit-0.5.2/.github/dependabot.yml
--rw-r--r--   0        0        0     1452 2023-05-23 23:02:11.613405 caikit-0.5.2/.github/workflows/build-library.yml
--rw-r--r--   0        0        0     1328 2023-05-23 23:02:11.613405 caikit-0.5.2/.github/workflows/lint-code.yml
--rw-r--r--   0        0        0     1136 2023-05-23 23:02:11.613405 caikit-0.5.2/.github/workflows/publish-library.yml
--rw-r--r--   0        0        0      261 2023-05-23 23:02:11.613405 caikit-0.5.2/.gitignore
--rw-r--r--   0        0        0      324 2023-05-23 23:02:11.613405 caikit-0.5.2/.isort.cfg
--rw-r--r--   0        0        0      370 2023-05-23 23:02:11.613405 caikit-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      122 2023-05-23 23:02:11.613405 caikit-0.5.2/.prettierignore
--rw-r--r--   0        0        0       12 2023-05-23 23:02:11.613405 caikit-0.5.2/.prettierrc.yaml
--rw-r--r--   0        0        0    21434 2023-05-23 23:02:11.613405 caikit-0.5.2/.pylintrc
--rw-r--r--   0        0        0       78 2023-05-23 23:02:11.613405 caikit-0.5.2/.whitesource
--rw-r--r--   0        0        0      368 2023-05-23 23:02:11.613405 caikit-0.5.2/CODEOWNERS
--rw-r--r--   0        0        0     7165 2023-05-23 23:02:11.613405 caikit-0.5.2/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-05-23 23:02:11.613405 caikit-0.5.2/LICENSE
--rw-r--r--   0        0        0     3626 2023-05-23 23:02:11.613405 caikit-0.5.2/README.md
--rw-r--r--   0        0        0      152 2023-05-23 23:02:11.613405 caikit-0.5.2/SECURITY.md
--rw-r--r--   0        0        0    44878 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit-overview.png
--rw-r--r--   0        0        0      427 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/__init__.py
--rw-r--r--   0        0        0      727 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/config/__init__.py
--rw-r--r--   0        0        0     6052 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/config/config.py
--rw-r--r--   0        0        0     6488 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/config/config.yml
--rw-r--r--   0        0        0     1642 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/__init__.py
--rw-r--r--   0        0        0      812 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/augmentors/__init__.py
--rw-r--r--   0        0        0     3506 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/augmentors/base.py
--rw-r--r--   0        0        0     2828 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/augmentors/merged_augmentor.py
--rw-r--r--   0        0        0      355 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/augmentors/schemes/__init__.py
--rw-r--r--   0        0        0     2052 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/augmentors/schemes/always_selection_scheme.py
--rw-r--r--   0        0        0     3164 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/augmentors/schemes/base.py
--rw-r--r--   0        0        0     3264 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
--rw-r--r--   0        0        0     2898 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/augmentors/schemes/random_single_selection_scheme.py
--rw-r--r--   0        0        0     1027 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/data_model/__init__.py
--rw-r--r--   0        0        0    35636 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/data_model/base.py
--rw-r--r--   0        0        0      750 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     2207 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/data_model/data_backends/base.py
--rw-r--r--   0        0        0     4050 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/data_model/data_backends/dict_backend.py
--rw-r--r--   0        0        0    14380 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/data_model/dataobject.py
--rw-r--r--   0        0        0     4858 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/data_model/enums.py
--rw-r--r--   0        0        0     1564 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/data_model/producer.py
--rw-r--r--   0        0        0     3914 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/data_model/protobufs/__init__.py
--rw-r--r--   0        0        0      577 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/data_model/streams/__init__.py
--rw-r--r--   0        0        0     5500 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/data_model/streams/converter.py
--rw-r--r--   0        0        0     4788 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/data_model/streams/csv_column_formatter.py
--rw-r--r--   0        0        0    40212 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/data_model/streams/data_stream.py
--rw-r--r--   0        0        0     3606 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/data_model/streams/resolver.py
--rw-r--r--   0        0        0     5245 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/data_model/streams/validator.py
--rw-r--r--   0        0        0    21296 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/model_manager.py
--rw-r--r--   0        0        0      684 2023-05-23 23:02:11.613405 caikit-0.5.2/caikit/core/module_backends/__init__.py
--rw-r--r--   0        0        0     2834 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/module_backends/backend_types.py
--rw-r--r--   0        0        0     4718 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/module_backends/base.py
--rw-r--r--   0        0        0     2802 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/module_backends/local_backend.py
--rw-r--r--   0        0        0     6002 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/module_backends/module_backend_config.py
--rw-r--r--   0        0        0      742 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/modules/__init__.py
--rw-r--r--   0        0        0    30065 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/modules/base.py
--rw-r--r--   0        0        0     6247 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/modules/config.py
--rw-r--r--   0        0        0    10859 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/modules/decorator.py
--rw-r--r--   0        0        0     4151 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/modules/loader.py
--rw-r--r--   0        0        0     6013 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/modules/meta.py
--rw-r--r--   0        0        0    13024 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/modules/saver.py
--rw-r--r--   0        0        0     3895 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/registries.py
--rw-r--r--   0        0        0     5358 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/task.py
--rw-r--r--   0        0        0     1001 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/toolkit/__init__.py
--rw-r--r--   0        0        0     4716 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/toolkit/compatibility.py
--rw-r--r--   0        0        0      637 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/toolkit/errors/__init__.py
--rw-r--r--   0        0        0    21366 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/toolkit/errors/error_handler.py
--rw-r--r--   0        0        0     1400 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/toolkit/errors/validation_error.py
--rw-r--r--   0        0        0     4935 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/toolkit/fileio.py
--rw-r--r--   0        0        0     2292 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/toolkit/isa.py
--rw-r--r--   0        0        0     1648 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/toolkit/logging.py
--rw-r--r--   0        0        0    32206 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/toolkit/quality_evaluation.py
--rw-r--r--   0        0        0     3439 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/toolkit/serializers.py
--rw-r--r--   0        0        0     5979 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/core/toolkit/wip_decorator.py
--rw-r--r--   0        0        0      530 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/interfaces/__init__.py
--rw-r--r--   0        0        0      748 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/interfaces/common/__init__.py
--rw-r--r--   0        0        0     1211 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/interfaces/common/data_model/__init__.py
--rw-r--r--   0        0        0     1431 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/interfaces/common/data_model/producer.py
--rw-r--r--   0        0        0      611 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/interfaces/runtime/__init__.py
--rw-r--r--   0        0        0      763 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/interfaces/runtime/data_model/__init__.py
--rw-r--r--   0        0        0     1886 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/interfaces/runtime/data_model/training_management.py
--rw-r--r--   0        0        0      577 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/__init__.py
--rw-r--r--   0        0        0     1827 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/dump_services.py
--rw-r--r--   0        0        0    14200 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/grpc_server.py
--rw-r--r--   0        0        0      577 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/interceptors/__init__.py
--rw-r--r--   0        0        0    16502 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
--rw-r--r--   0        0        0      577 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     4659 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/metrics/rpc_meter.py
--rw-r--r--   0        0        0      577 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    17143 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/model_management/batcher.py
--rw-r--r--   0        0        0     2648 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/model_management/loaded_model.py
--rw-r--r--   0        0        0     5802 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/model_management/model_loader.py
--rw-r--r--   0        0        0    12101 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/model_management/model_manager.py
--rw-r--r--   0        0        0     4311 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/model_management/model_sizer.py
--rw-r--r--   0        0        0     1480 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/model_management/training_manager.py
--rw-r--r--   0        0        0      367 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/protobufs/README.md
--rw-r--r--   0        0        0      698 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/protobufs/__init__.py
--rw-r--r--   0        0        0    11375 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/protobufs/model_mesh_pb2.py
--rw-r--r--   0        0        0    12846 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
--rw-r--r--   0        0        0    10107 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/protobufs/model_runtime_pb2.py
--rw-r--r--   0        0        0    10556 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     5535 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/protobufs/process_pb2.py
--rw-r--r--   0        0        0     2569 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/protobufs/process_pb2_grpc.py
--rw-r--r--   0        0        0     8844 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/protobufs/protos/model-mesh.proto
--rw-r--r--   0        0        0     6795 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/protobufs/protos/model-runtime.proto
--rw-r--r--   0        0        0     2479 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/protobufs/protos/process.proto
--rw-r--r--   0        0        0    16699 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/service_factory.py
--rw-r--r--   0        0        0      109 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     1779 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/service_generation/compatibility_checker.py
--rw-r--r--   0        0        0     3043 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/service_generation/core_module_helpers.py
--rw-r--r--   0        0        0     5838 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/service_generation/create_service.py
--rw-r--r--   0        0        0    13914 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/service_generation/data_stream_source.py
--rw-r--r--   0        0        0     7155 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/service_generation/primitives.py
--rw-r--r--   0        0        0    12800 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/service_generation/rpcs.py
--rw-r--r--   0        0        0      666 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0    10747 2023-05-23 23:02:11.617405 caikit-0.5.2/caikit/runtime/service_generation/signature_parsing/docstrings.py
--rw-r--r--   0        0        0     4794 2023-05-23 23:02:11.621405 caikit-0.5.2/caikit/runtime/service_generation/signature_parsing/module_signature.py
--rw-r--r--   0        0        0     8225 2023-05-23 23:02:11.621405 caikit-0.5.2/caikit/runtime/service_generation/signature_parsing/parsers.py
--rw-r--r--   0        0        0     2571 2023-05-23 23:02:11.621405 caikit-0.5.2/caikit/runtime/service_generation/type_helpers.py
--rw-r--r--   0        0        0      577 2023-05-23 23:02:11.621405 caikit-0.5.2/caikit/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     9476 2023-05-23 23:02:11.621405 caikit-0.5.2/caikit/runtime/servicers/global_predict_servicer.py
--rw-r--r--   0        0        0    15326 2023-05-23 23:02:11.621405 caikit-0.5.2/caikit/runtime/servicers/global_train_servicer.py
--rw-r--r--   0        0        0    10637 2023-05-23 23:02:11.621405 caikit-0.5.2/caikit/runtime/servicers/model_runtime_servicer.py
--rw-r--r--   0        0        0     5539 2023-05-23 23:02:11.621405 caikit-0.5.2/caikit/runtime/servicers/model_train_servicer.py
--rw-r--r--   0        0        0     1667 2023-05-23 23:02:11.621405 caikit-0.5.2/caikit/runtime/servicers/training_management_servicer.py
--rw-r--r--   0        0        0      577 2023-05-23 23:02:11.621405 caikit-0.5.2/caikit/runtime/types/__init__.py
--rw-r--r--   0        0        0      957 2023-05-23 23:02:11.621405 caikit-0.5.2/caikit/runtime/types/aborted_exception.py
--rw-r--r--   0        0        0     1558 2023-05-23 23:02:11.621405 caikit-0.5.2/caikit/runtime/types/caikit_runtime_exception.py
--rw-r--r--   0        0        0      960 2023-05-23 23:02:11.621405 caikit-0.5.2/caikit/runtime/types/thread_destroyed_exception.py
--rw-r--r--   0        0        0      577 2023-05-23 23:02:11.621405 caikit-0.5.2/caikit/runtime/utils/__init__.py
--rw-r--r--   0        0        0     6810 2023-05-23 23:02:11.621405 caikit-0.5.2/caikit/runtime/utils/import_util.py
--rw-r--r--   0        0        0    17892 2023-05-23 23:02:11.621405 caikit-0.5.2/caikit/runtime/utils/servicer_util.py
--rw-r--r--   0        0        0      577 2023-05-23 23:02:11.621405 caikit-0.5.2/caikit/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     3732 2023-05-23 23:02:11.621405 caikit-0.5.2/caikit/runtime/work_management/abortable_action.py
--rw-r--r--   0        0        0     2969 2023-05-23 23:02:11.621405 caikit-0.5.2/caikit/runtime/work_management/call_aborter.py
--rw-r--r--   0        0        0     7596 2023-05-23 23:02:11.621405 caikit-0.5.2/caikit/runtime/work_management/destroyable_thread.py
--rw-r--r--   0        0        0      169 2023-05-23 23:02:11.621405 caikit-0.5.2/code-of-conduct.md
--rw-r--r--   0        0        0       68 2023-05-23 23:02:11.621405 caikit-0.5.2/docs-requirements.txt
--rw-r--r--   0        0        0      634 2023-05-23 23:02:11.621405 caikit-0.5.2/docs/Makefile
--rw-r--r--   0        0        0     1610 2023-05-23 23:02:11.621405 caikit-0.5.2/docs/adrs/010-data-model-definition.md
--rw-r--r--   0        0        0     2352 2023-05-23 23:02:11.621405 caikit-0.5.2/docs/adrs/015-runtime-service-generation.md
--rw-r--r--   0        0        0     2581 2023-05-23 23:02:11.621405 caikit-0.5.2/docs/adrs/018-shared-backends.md
--rw-r--r--   0        0        0     1223 2023-05-23 23:02:11.621405 caikit-0.5.2/docs/adrs/019-loader-stack.md
--rw-r--r--   0        0        0      404 2023-05-23 23:02:11.621405 caikit-0.5.2/docs/adrs/README.md
--rw-r--r--   0        0        0     2423 2023-05-23 23:02:11.621405 caikit-0.5.2/docs/architecture_club/04-25-23.md
--rw-r--r--   0        0        0      342 2023-05-23 23:02:11.621405 caikit-0.5.2/docs/architecture_club/README.md
--rw-r--r--   0        0        0     2660 2023-05-23 23:02:11.621405 caikit-0.5.2/docs/conf.py
--rw-r--r--   0        0        0      225 2023-05-23 23:02:11.621405 caikit-0.5.2/docs/index.rst
--rw-r--r--   0        0        0      800 2023-05-23 23:02:11.621405 caikit-0.5.2/docs/make.bat
--rw-r--r--   0        0        0      837 2023-05-23 23:02:11.621405 caikit-0.5.2/examples/start_runtime_with_sample_lib.py
--rw-r--r--   0        0        0     6095 2023-05-23 23:02:11.621405 caikit-0.5.2/examples/text-sentiment/README.md
--rw-r--r--   0        0        0     1425 2023-05-23 23:02:11.621405 caikit-0.5.2/examples/text-sentiment/client.py
--rw-r--r--   0        0        0      673 2023-05-23 23:02:11.621405 caikit-0.5.2/examples/text-sentiment/models/text_sentiment/config.yml
--rw-r--r--   0        0        0       72 2023-05-23 23:02:11.621405 caikit-0.5.2/examples/text-sentiment/requirements.txt
--rw-r--r--   0        0        0      961 2023-05-23 23:02:11.621405 caikit-0.5.2/examples/text-sentiment/start_runtime.py
--rw-r--r--   0        0        0      816 2023-05-23 23:02:11.621405 caikit-0.5.2/examples/text-sentiment/text_sentiment/__init__.py
--rw-r--r--   0        0        0      742 2023-05-23 23:02:11.621405 caikit-0.5.2/examples/text-sentiment/text_sentiment/config.yml
--rw-r--r--   0        0        0      661 2023-05-23 23:02:11.621405 caikit-0.5.2/examples/text-sentiment/text_sentiment/data_model/__init__.py
--rw-r--r--   0        0        0     1422 2023-05-23 23:02:11.621405 caikit-0.5.2/examples/text-sentiment/text_sentiment/data_model/classification.py
--rw-r--r--   0        0        0      645 2023-05-23 23:02:11.621405 caikit-0.5.2/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
--rw-r--r--   0        0        0     3067 2023-05-23 23:02:11.621405 caikit-0.5.2/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py
--rw-r--r--   0        0        0     1196 2023-05-23 23:02:15.313636 caikit-0.5.2/pyproject.toml
--rwxr-xr-x   0        0        0      639 2023-05-23 23:02:11.621405 caikit-0.5.2/scripts/check_deps.sh
--rwxr-xr-x   0        0        0      720 2023-05-23 23:02:11.621405 caikit-0.5.2/scripts/fmt.sh
--rw-r--r--   0        0        0       33 2023-05-23 23:02:11.621405 caikit-0.5.2/setup_requirements.txt
--rw-r--r--   0        0        0     1006 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/__init__.py
--rw-r--r--   0        0        0     3439 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/base.py
--rw-r--r--   0        0        0        0 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/config/__init__.py
--rw-r--r--   0        0        0     5358 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/config/test_configs.py
--rw-r--r--   0        0        0     8956 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/__init__.py
--rw-r--r--   0        0        0     2853 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/augmentors/test_augmentor_base.py
--rw-r--r--   0        0        0     9114 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/augmentors/test_merged_augmentors.py
--rw-r--r--   0        0        0        0 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/data_model/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     5033 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/data_model/data_backends/test_dict_backend.py
--rw-r--r--   0        0        0     3306 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/data_model/streams/test_converter.py
--rw-r--r--   0        0        0     3314 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/data_model/streams/test_csv_column_formatter.py
--rw-r--r--   0        0        0    26459 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/data_model/streams/test_data_stream.py
--rw-r--r--   0        0        0     3498 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/data_model/streams/test_resolver.py
--rw-r--r--   0        0        0     2908 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/data_model/streams/test_validator.py
--rw-r--r--   0        0        0    16232 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/data_model/test_base.py
--rw-r--r--   0        0        0    20408 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/data_model/test_dataobject.py
--rw-r--r--   0        0        0     5083 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/data_model/test_enums.py
--rw-r--r--   0        0        0     1104 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/data_model/test_producer.py
--rw-r--r--   0        0        0     4357 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/helpers.py
--rw-r--r--   0        0        0        0 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/module_backends/__init__.py
--rw-r--r--   0        0        0     2320 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/module_backends/test_backend_types.py
--rw-r--r--   0        0        0     6922 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/module_backends/test_module_backend_config.py
--rw-r--r--   0        0        0        0 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/modules/__init__.py
--rw-r--r--   0        0        0    12293 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/modules/test_module.py
--rw-r--r--   0        0        0     6274 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/modules/test_module_metadata.py
--rw-r--r--   0        0        0      521 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/test_imports.py
--rw-r--r--   0        0        0    21421 2023-05-23 23:02:11.621405 caikit-0.5.2/tests/core/test_model_manager.py
--rw-r--r--   0        0        0     1038 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/core/test_no_write_permissions.py
--rw-r--r--   0        0        0     2460 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/core/test_task.py
--rw-r--r--   0        0        0     7967 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/core/toolkit/test_compatibility.py
--rw-r--r--   0        0        0    18396 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/core/toolkit/test_error_handler.py
--rw-r--r--   0        0        0     4997 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/core/toolkit/test_fileio.py
--rw-r--r--   0        0        0    25851 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/core/toolkit/test_quality_evaluation.py
--rw-r--r--   0        0        0     2634 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/core/toolkit/test_serializers.py
--rw-r--r--   0        0        0     7824 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/core/toolkit/test_wip_decorator.py
--rw-r--r--   0        0        0     6782 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/data_model_helpers.py
--rw-r--r--   0        0        0       39 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      647 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/config/config.yml
--rw-r--r--   0        0        0       27 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/data_stream_inputs/bad_file.json
--rw-r--r--   0        0        0      154 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/data_stream_inputs/control_chars.jsonl
--rw-r--r--   0        0        0      106 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/data_stream_inputs/sample.csv
--rw-r--r--   0        0        0       66 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/data_stream_inputs/sample.json
--rw-r--r--   0        0        0      233 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/data_stream_inputs/sample.jsonl
--rw-r--r--   0        0        0     1322 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/data_stream_inputs/sample.txt
--rw-r--r--   0        0        0       11 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
--rw-r--r--   0        0        0       11 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
--rw-r--r--   0        0        0       11 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
--rw-r--r--   0        0        0       27 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
--rw-r--r--   0        0        0       27 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
--rw-r--r--   0        0        0       63 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
--rw-r--r--   0        0        0      147 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
--rw-r--r--   0        0        0      218 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
--rw-r--r--   0        0        0       87 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
--rw-r--r--   0        0        0       52 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
--rw-r--r--   0        0        0       56 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
--rw-r--r--   0        0        0       55 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
--rw-r--r--   0        0        0      125 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/data_stream_inputs/sample_w_header.csv
--rw-r--r--   0        0        0      222 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/dummy_dataset.json
--rw-r--r--   0        0        0     1016 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/dummy_module.zip
--rw-r--r--   0        0        0      675 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/dummy_module/config.yml
--rw-r--r--   0        0        0      299 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/dummy_module/data.json
--rw-r--r--   0        0        0       14 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/dummy_module/data.pkl
--rw-r--r--   0        0        0      191 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/dummy_module_backend/config.yml
--rw-r--r--   0        0        0      179 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/dummy_module_foo/config.yml
--rw-r--r--   0        0        0      506 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/dummy_module_no_nesting.zip
--rw-r--r--   0        0        0      570 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/dummy_module_singleton/config.yml
--rw-r--r--   0        0        0      299 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/dummy_module_singleton/data.json
--rw-r--r--   0        0        0       14 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/dummy_module_singleton/data.pkl
--rw-r--r--   0        0        0      230 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/dummy_resource/config.yml
--rw-r--r--   0        0        0     3034 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/fixtures.py
--rw-r--r--   0        0        0      918 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/invalid.zip
--rw-r--r--   0        0        0     2551 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/linux.txt
--rw-r--r--   0        0        0       10 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/models/bad_archive.zip
--rw-r--r--   0        0        0      376 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/models/bad_model.zip
--rw-r--r--   0        0        0      360 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/models/bar/config.yml
--rw-r--r--   0        0        0      364 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/models/foo/config.yml
--rw-r--r--   0        0        0      422 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/models/foo_archive.zip
--rw-r--r--   0        0        0     2142 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/primitive_party.proto
--rw-r--r--   0        0        0      145 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/protobufs/__init__.py
--rw-r--r--   0        0        0     2080 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/protobufs/caikit_runtime_pb2.py
--rw-r--r--   0        0        0     2447 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     2217 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
--rw-r--r--   0        0        0     2602 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
--rw-r--r--   0        0        0     5995 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/protobufs/primitive_party_pb2.py
--rw-r--r--   0        0        0      416 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/protos/caikit_runtime.proto
--rw-r--r--   0        0        0      437 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/protos/caikit_runtime_train.proto
--rw-r--r--   0        0        0       24 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      294 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/sample_lib/__init__.py
--rw-r--r--   0        0        0      410 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/sample_lib/config.yml
--rw-r--r--   0        0        0      157 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/sample_lib/data_model/__init__.py
--rw-r--r--   0        0        0     1257 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/sample_lib/data_model/sample.py
--rw-r--r--   0        0        0      156 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/sample_lib/modules/__init__.py
--rw-r--r--   0        0        0       89 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/sample_lib/modules/other_task/__init__.py
--rw-r--r--   0        0        0     1882 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/sample_lib/modules/other_task/other_implementation.py
--rw-r--r--   0        0        0      250 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/sample_lib/modules/sample_task/__init__.py
--rw-r--r--   0        0        0     1720 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/sample_lib/modules/sample_task/composite_module.py
--rw-r--r--   0        0        0      651 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/sample_lib/modules/sample_task/inner_module.py
--rw-r--r--   0        0        0     2463 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py
--rw-r--r--   0        0        0     1312 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py
--rw-r--r--   0        0        0     2720 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py
--rw-r--r--   0        0        0      364 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/fixtures/sample_module/config.yml
--rw-r--r--   0        0        0        0 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/__init__.py
--rw-r--r--   0        0        0      756 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/generated/__init__.py
--rw-r--r--   0        0        0      577 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     3845 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/metrics/test_rpc_meter.py
--rw-r--r--   0        0        0      577 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    14141 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/model_management/test_batcher.py
--rw-r--r--   0        0        0    10266 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/model_management/test_model_loader.py
--rw-r--r--   0        0        0    17911 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/model_management/test_model_manager.py
--rw-r--r--   0        0        0     5303 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/model_management/test_model_sizer.py
--rw-r--r--   0        0        0     2254 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/model_management/test_training_manager.py
--rw-r--r--   0        0        0        0 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0      577 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0     5398 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/service_generation/signature_parsing/test_docstrings.py
--rw-r--r--   0        0        0     8706 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/service_generation/signature_parsing/test_parsers.py
--rw-r--r--   0        0        0     3349 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/service_generation/test_create_service.py
--rw-r--r--   0        0        0    18431 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/service_generation/test_data_stream_source.py
--rw-r--r--   0        0        0     4065 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/service_generation/test_primitives.py
--rw-r--r--   0        0        0     1721 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/service_generation/test_rpcs.py
--rw-r--r--   0        0        0     1376 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/service_generation/test_type_helpers.py
--rw-r--r--   0        0        0      577 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     7859 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/servicers/test_global_predict_servicer_impl.py
--rw-r--r--   0        0        0    15481 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/servicers/test_global_train_servicer_impl.py
--rw-r--r--   0        0        0     3640 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/servicers/test_model_runtime_servicer_impl.py
--rw-r--r--   0        0        0     7372 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/servicers/test_model_train_servicer_impl.py
--rw-r--r--   0        0        0     4204 2023-05-23 23:02:11.625405 caikit-0.5.2/tests/runtime/servicers/test_training_management_servicer.py
--rw-r--r--   0        0        0    30156 2023-05-23 23:02:11.629405 caikit-0.5.2/tests/runtime/test_grpc_server.py
--rw-r--r--   0        0        0    11106 2023-05-23 23:02:11.629405 caikit-0.5.2/tests/runtime/test_service_factory.py
--rw-r--r--   0        0        0      577 2023-05-23 23:02:11.629405 caikit-0.5.2/tests/runtime/utils/__init__.py
--rw-r--r--   0        0        0     4899 2023-05-23 23:02:11.629405 caikit-0.5.2/tests/runtime/utils/test_import_util.py
--rw-r--r--   0        0        0    26269 2023-05-23 23:02:11.629405 caikit-0.5.2/tests/runtime/utils/test_servicer_util.py
--rw-r--r--   0        0        0      577 2023-05-23 23:02:11.629405 caikit-0.5.2/tests/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     2758 2023-05-23 23:02:11.629405 caikit-0.5.2/tests/runtime/work_management/test_abortable_action.py
--rw-r--r--   0        0        0     1868 2023-05-23 23:02:11.629405 caikit-0.5.2/tests/runtime/work_management/test_call_aborter.py
--rw-r--r--   0        0        0     3355 2023-05-23 23:02:11.629405 caikit-0.5.2/tests/runtime/work_management/test_destroyable_thread.py
--rw-r--r--   0        0        0     2115 2023-05-23 23:02:11.629405 caikit-0.5.2/tox.ini
--rw-r--r--   0        0        0     4785 1970-01-01 00:00:00.000000 caikit-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-05-25 17:13:34.530774 caikit-0.5.3/.coveragerc
+-rw-r--r--   0        0        0      676 2023-05-25 17:13:34.530774 caikit-0.5.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      579 2023-05-25 17:13:34.530774 caikit-0.5.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-05-25 17:13:34.530774 caikit-0.5.3/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0        0        0      106 2023-05-25 17:13:34.530774 caikit-0.5.3/.github/dependabot.yml
+-rw-r--r--   0        0        0     1452 2023-05-25 17:13:34.530774 caikit-0.5.3/.github/workflows/build-library.yml
+-rw-r--r--   0        0        0     1328 2023-05-25 17:13:34.530774 caikit-0.5.3/.github/workflows/lint-code.yml
+-rw-r--r--   0        0        0     1136 2023-05-25 17:13:34.530774 caikit-0.5.3/.github/workflows/publish-library.yml
+-rw-r--r--   0        0        0      261 2023-05-25 17:13:34.530774 caikit-0.5.3/.gitignore
+-rw-r--r--   0        0        0      324 2023-05-25 17:13:34.530774 caikit-0.5.3/.isort.cfg
+-rw-r--r--   0        0        0      370 2023-05-25 17:13:34.530774 caikit-0.5.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      122 2023-05-25 17:13:34.530774 caikit-0.5.3/.prettierignore
+-rw-r--r--   0        0        0       12 2023-05-25 17:13:34.530774 caikit-0.5.3/.prettierrc.yaml
+-rw-r--r--   0        0        0    21434 2023-05-25 17:13:34.530774 caikit-0.5.3/.pylintrc
+-rw-r--r--   0        0        0       78 2023-05-25 17:13:34.530774 caikit-0.5.3/.whitesource
+-rw-r--r--   0        0        0      368 2023-05-25 17:13:34.530774 caikit-0.5.3/CODEOWNERS
+-rw-r--r--   0        0        0     7165 2023-05-25 17:13:34.530774 caikit-0.5.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-05-25 17:13:34.530774 caikit-0.5.3/LICENSE
+-rw-r--r--   0        0        0     3734 2023-05-25 17:13:34.530774 caikit-0.5.3/README.md
+-rw-r--r--   0        0        0      152 2023-05-25 17:13:34.530774 caikit-0.5.3/SECURITY.md
+-rw-r--r--   0        0        0    44878 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit-overview.png
+-rw-r--r--   0        0        0      427 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/__init__.py
+-rw-r--r--   0        0        0      727 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/config/__init__.py
+-rw-r--r--   0        0        0     6052 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/config/config.py
+-rw-r--r--   0        0        0     6488 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/config/config.yml
+-rw-r--r--   0        0        0     1642 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/__init__.py
+-rw-r--r--   0        0        0      812 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/augmentors/__init__.py
+-rw-r--r--   0        0        0     3506 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/augmentors/base.py
+-rw-r--r--   0        0        0     2828 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/augmentors/merged_augmentor.py
+-rw-r--r--   0        0        0      355 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/augmentors/schemes/__init__.py
+-rw-r--r--   0        0        0     2052 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/augmentors/schemes/always_selection_scheme.py
+-rw-r--r--   0        0        0     3164 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/augmentors/schemes/base.py
+-rw-r--r--   0        0        0     3264 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
+-rw-r--r--   0        0        0     2898 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/augmentors/schemes/random_single_selection_scheme.py
+-rw-r--r--   0        0        0     1027 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/data_model/__init__.py
+-rw-r--r--   0        0        0    35986 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/data_model/base.py
+-rw-r--r--   0        0        0      750 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     2207 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/data_model/data_backends/base.py
+-rw-r--r--   0        0        0     4050 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/data_model/data_backends/dict_backend.py
+-rw-r--r--   0        0        0    14380 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/data_model/dataobject.py
+-rw-r--r--   0        0        0     4858 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/data_model/enums.py
+-rw-r--r--   0        0        0     1564 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/data_model/producer.py
+-rw-r--r--   0        0        0     3914 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/data_model/protobufs/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/data_model/streams/__init__.py
+-rw-r--r--   0        0        0     5500 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/data_model/streams/converter.py
+-rw-r--r--   0        0        0     4788 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/data_model/streams/csv_column_formatter.py
+-rw-r--r--   0        0        0    40212 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/data_model/streams/data_stream.py
+-rw-r--r--   0        0        0     3606 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/data_model/streams/resolver.py
+-rw-r--r--   0        0        0     5245 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/data_model/streams/validator.py
+-rw-r--r--   0        0        0    21296 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/model_manager.py
+-rw-r--r--   0        0        0      684 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     2834 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/module_backends/backend_types.py
+-rw-r--r--   0        0        0     4718 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/module_backends/base.py
+-rw-r--r--   0        0        0     2802 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/module_backends/local_backend.py
+-rw-r--r--   0        0        0     6002 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/module_backends/module_backend_config.py
+-rw-r--r--   0        0        0      742 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/modules/__init__.py
+-rw-r--r--   0        0        0    30320 2023-05-25 17:13:34.530774 caikit-0.5.3/caikit/core/modules/base.py
+-rw-r--r--   0        0        0     6247 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/core/modules/config.py
+-rw-r--r--   0        0        0    11042 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/core/modules/decorator.py
+-rw-r--r--   0        0        0     4151 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/core/modules/loader.py
+-rw-r--r--   0        0        0     6013 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/core/modules/meta.py
+-rw-r--r--   0        0        0    13024 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/core/modules/saver.py
+-rw-r--r--   0        0        0     3895 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/core/registries.py
+-rw-r--r--   0        0        0      654 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/core/signature_parsing/__init__.py
+-rw-r--r--   0        0        0    10721 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/core/signature_parsing/docstrings.py
+-rw-r--r--   0        0        0     4688 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/core/signature_parsing/module_signature.py
+-rw-r--r--   0        0        0     7841 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/core/signature_parsing/parsers.py
+-rw-r--r--   0        0        0     6961 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/core/task.py
+-rw-r--r--   0        0        0     1001 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     4716 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/core/toolkit/compatibility.py
+-rw-r--r--   0        0        0      637 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/core/toolkit/errors/__init__.py
+-rw-r--r--   0        0        0    21366 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/core/toolkit/errors/error_handler.py
+-rw-r--r--   0        0        0     1400 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/core/toolkit/errors/validation_error.py
+-rw-r--r--   0        0        0     4935 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/core/toolkit/fileio.py
+-rw-r--r--   0        0        0     2292 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/core/toolkit/isa.py
+-rw-r--r--   0        0        0     1648 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/core/toolkit/logging.py
+-rw-r--r--   0        0        0    32206 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/core/toolkit/quality_evaluation.py
+-rw-r--r--   0        0        0     3439 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/core/toolkit/serializers.py
+-rw-r--r--   0        0        0     5979 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/core/toolkit/wip_decorator.py
+-rw-r--r--   0        0        0      530 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/interfaces/__init__.py
+-rw-r--r--   0        0        0      748 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/interfaces/common/__init__.py
+-rw-r--r--   0        0        0     1211 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/interfaces/common/data_model/__init__.py
+-rw-r--r--   0        0        0     1431 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/interfaces/common/data_model/producer.py
+-rw-r--r--   0        0        0      611 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/interfaces/runtime/__init__.py
+-rw-r--r--   0        0        0      763 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/interfaces/runtime/data_model/__init__.py
+-rw-r--r--   0        0        0     1886 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/interfaces/runtime/data_model/training_management.py
+-rw-r--r--   0        0        0      577 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/__init__.py
+-rw-r--r--   0        0        0     1827 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/dump_services.py
+-rw-r--r--   0        0        0    14200 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/grpc_server.py
+-rw-r--r--   0        0        0      577 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/interceptors/__init__.py
+-rw-r--r--   0        0        0    16502 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
+-rw-r--r--   0        0        0      577 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     4659 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/metrics/rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    17143 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/model_management/batcher.py
+-rw-r--r--   0        0        0     2648 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/model_management/loaded_model.py
+-rw-r--r--   0        0        0     5802 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/model_management/model_loader.py
+-rw-r--r--   0        0        0    12101 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/model_management/model_manager.py
+-rw-r--r--   0        0        0     4311 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/model_management/model_sizer.py
+-rw-r--r--   0        0        0     1480 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/model_management/training_manager.py
+-rw-r--r--   0        0        0      367 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/protobufs/README.md
+-rw-r--r--   0        0        0      698 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/protobufs/__init__.py
+-rw-r--r--   0        0        0    11375 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/protobufs/model_mesh_pb2.py
+-rw-r--r--   0        0        0    12846 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
+-rw-r--r--   0        0        0    10107 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/protobufs/model_runtime_pb2.py
+-rw-r--r--   0        0        0    10556 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     5535 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/protobufs/process_pb2.py
+-rw-r--r--   0        0        0     2569 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/protobufs/process_pb2_grpc.py
+-rw-r--r--   0        0        0     8844 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/protobufs/protos/model-mesh.proto
+-rw-r--r--   0        0        0     6795 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/protobufs/protos/model-runtime.proto
+-rw-r--r--   0        0        0     2479 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/protobufs/protos/process.proto
+-rw-r--r--   0        0        0    16699 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/service_factory.py
+-rw-r--r--   0        0        0      109 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     1779 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/service_generation/compatibility_checker.py
+-rw-r--r--   0        0        0     3043 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/service_generation/core_module_helpers.py
+-rw-r--r--   0        0        0     5809 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/service_generation/create_service.py
+-rw-r--r--   0        0        0    13914 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/service_generation/data_stream_source.py
+-rw-r--r--   0        0        0     7136 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/service_generation/primitives.py
+-rw-r--r--   0        0        0    12688 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/service_generation/rpcs.py
+-rw-r--r--   0        0        0     2571 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/service_generation/type_helpers.py
+-rw-r--r--   0        0        0      577 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     9476 2023-05-25 17:13:34.534774 caikit-0.5.3/caikit/runtime/servicers/global_predict_servicer.py
+-rw-r--r--   0        0        0    15326 2023-05-25 17:13:34.538774 caikit-0.5.3/caikit/runtime/servicers/global_train_servicer.py
+-rw-r--r--   0        0        0    10637 2023-05-25 17:13:34.538774 caikit-0.5.3/caikit/runtime/servicers/model_runtime_servicer.py
+-rw-r--r--   0        0        0     5539 2023-05-25 17:13:34.538774 caikit-0.5.3/caikit/runtime/servicers/model_train_servicer.py
+-rw-r--r--   0        0        0     1667 2023-05-25 17:13:34.538774 caikit-0.5.3/caikit/runtime/servicers/training_management_servicer.py
+-rw-r--r--   0        0        0      577 2023-05-25 17:13:34.538774 caikit-0.5.3/caikit/runtime/types/__init__.py
+-rw-r--r--   0        0        0      957 2023-05-25 17:13:34.538774 caikit-0.5.3/caikit/runtime/types/aborted_exception.py
+-rw-r--r--   0        0        0     1558 2023-05-25 17:13:34.538774 caikit-0.5.3/caikit/runtime/types/caikit_runtime_exception.py
+-rw-r--r--   0        0        0      960 2023-05-25 17:13:34.538774 caikit-0.5.3/caikit/runtime/types/thread_destroyed_exception.py
+-rw-r--r--   0        0        0      577 2023-05-25 17:13:34.538774 caikit-0.5.3/caikit/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     6810 2023-05-25 17:13:34.538774 caikit-0.5.3/caikit/runtime/utils/import_util.py
+-rw-r--r--   0        0        0    17892 2023-05-25 17:13:34.538774 caikit-0.5.3/caikit/runtime/utils/servicer_util.py
+-rw-r--r--   0        0        0      577 2023-05-25 17:13:34.538774 caikit-0.5.3/caikit/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     3732 2023-05-25 17:13:34.538774 caikit-0.5.3/caikit/runtime/work_management/abortable_action.py
+-rw-r--r--   0        0        0     2969 2023-05-25 17:13:34.538774 caikit-0.5.3/caikit/runtime/work_management/call_aborter.py
+-rw-r--r--   0        0        0     7596 2023-05-25 17:13:34.538774 caikit-0.5.3/caikit/runtime/work_management/destroyable_thread.py
+-rw-r--r--   0        0        0      169 2023-05-25 17:13:34.538774 caikit-0.5.3/code-of-conduct.md
+-rw-r--r--   0        0        0       68 2023-05-25 17:13:34.538774 caikit-0.5.3/docs-requirements.txt
+-rw-r--r--   0        0        0      634 2023-05-25 17:13:34.538774 caikit-0.5.3/docs/Makefile
+-rw-r--r--   0        0        0     1610 2023-05-25 17:13:34.538774 caikit-0.5.3/docs/adrs/010-data-model-definition.md
+-rw-r--r--   0        0        0     2352 2023-05-25 17:13:34.538774 caikit-0.5.3/docs/adrs/015-runtime-service-generation.md
+-rw-r--r--   0        0        0     2581 2023-05-25 17:13:34.538774 caikit-0.5.3/docs/adrs/018-shared-backends.md
+-rw-r--r--   0        0        0     1223 2023-05-25 17:13:34.538774 caikit-0.5.3/docs/adrs/019-loader-stack.md
+-rw-r--r--   0        0        0      404 2023-05-25 17:13:34.538774 caikit-0.5.3/docs/adrs/README.md
+-rw-r--r--   0        0        0     2423 2023-05-25 17:13:34.538774 caikit-0.5.3/docs/architecture_club/04-25-23.md
+-rw-r--r--   0        0        0      342 2023-05-25 17:13:34.538774 caikit-0.5.3/docs/architecture_club/README.md
+-rw-r--r--   0        0        0     2660 2023-05-25 17:13:34.538774 caikit-0.5.3/docs/conf.py
+-rw-r--r--   0        0        0      225 2023-05-25 17:13:34.538774 caikit-0.5.3/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-05-25 17:13:34.538774 caikit-0.5.3/docs/make.bat
+-rw-r--r--   0        0        0      837 2023-05-25 17:13:34.538774 caikit-0.5.3/examples/start_runtime_with_sample_lib.py
+-rw-r--r--   0        0        0     6095 2023-05-25 17:13:34.538774 caikit-0.5.3/examples/text-sentiment/README.md
+-rw-r--r--   0        0        0     1427 2023-05-25 17:13:34.538774 caikit-0.5.3/examples/text-sentiment/client.py
+-rw-r--r--   0        0        0      673 2023-05-25 17:13:34.538774 caikit-0.5.3/examples/text-sentiment/models/text_sentiment/config.yml
+-rw-r--r--   0        0        0       72 2023-05-25 17:13:34.538774 caikit-0.5.3/examples/text-sentiment/requirements.txt
+-rw-r--r--   0        0        0      961 2023-05-25 17:13:34.538774 caikit-0.5.3/examples/text-sentiment/start_runtime.py
+-rw-r--r--   0        0        0      816 2023-05-25 17:13:34.538774 caikit-0.5.3/examples/text-sentiment/text_sentiment/__init__.py
+-rw-r--r--   0        0        0      742 2023-05-25 17:13:34.538774 caikit-0.5.3/examples/text-sentiment/text_sentiment/config.yml
+-rw-r--r--   0        0        0      661 2023-05-25 17:13:34.538774 caikit-0.5.3/examples/text-sentiment/text_sentiment/data_model/__init__.py
+-rw-r--r--   0        0        0     1422 2023-05-25 17:13:34.538774 caikit-0.5.3/examples/text-sentiment/text_sentiment/data_model/classification.py
+-rw-r--r--   0        0        0      645 2023-05-25 17:13:34.538774 caikit-0.5.3/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
+-rw-r--r--   0        0        0     3067 2023-05-25 17:13:34.538774 caikit-0.5.3/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py
+-rw-r--r--   0        0        0     1196 2023-05-25 17:13:40.342871 caikit-0.5.3/pyproject.toml
+-rwxr-xr-x   0        0        0      639 2023-05-25 17:13:34.538774 caikit-0.5.3/scripts/check_deps.sh
+-rwxr-xr-x   0        0        0      720 2023-05-25 17:13:34.538774 caikit-0.5.3/scripts/fmt.sh
+-rw-r--r--   0        0        0       33 2023-05-25 17:13:34.538774 caikit-0.5.3/setup_requirements.txt
+-rw-r--r--   0        0        0     1006 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/__init__.py
+-rw-r--r--   0        0        0     3439 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/base.py
+-rw-r--r--   0        0        0        0 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/config/__init__.py
+-rw-r--r--   0        0        0     5358 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/config/test_configs.py
+-rw-r--r--   0        0        0     8956 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/__init__.py
+-rw-r--r--   0        0        0     2853 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/augmentors/test_augmentor_base.py
+-rw-r--r--   0        0        0     9114 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/augmentors/test_merged_augmentors.py
+-rw-r--r--   0        0        0        0 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/data_model/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     5033 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/data_model/data_backends/test_dict_backend.py
+-rw-r--r--   0        0        0     3306 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/data_model/streams/test_converter.py
+-rw-r--r--   0        0        0     3314 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/data_model/streams/test_csv_column_formatter.py
+-rw-r--r--   0        0        0    26459 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/data_model/streams/test_data_stream.py
+-rw-r--r--   0        0        0     3498 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/data_model/streams/test_resolver.py
+-rw-r--r--   0        0        0     2908 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/data_model/streams/test_validator.py
+-rw-r--r--   0        0        0    16232 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/data_model/test_base.py
+-rw-r--r--   0        0        0    20601 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/data_model/test_dataobject.py
+-rw-r--r--   0        0        0     5083 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/data_model/test_enums.py
+-rw-r--r--   0        0        0     1104 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/data_model/test_producer.py
+-rw-r--r--   0        0        0     4357 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/helpers.py
+-rw-r--r--   0        0        0        0 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     2320 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/module_backends/test_backend_types.py
+-rw-r--r--   0        0        0     6888 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/module_backends/test_module_backend_config.py
+-rw-r--r--   0        0        0        0 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/modules/__init__.py
+-rw-r--r--   0        0        0    12551 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/modules/test_module.py
+-rw-r--r--   0        0        0     6274 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/modules/test_module_metadata.py
+-rw-r--r--   0        0        0      577 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/signature_parsing/__init__.py
+-rw-r--r--   0        0        0     4872 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/signature_parsing/test_docstrings.py
+-rw-r--r--   0        0        0     8595 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/signature_parsing/test_parsers.py
+-rw-r--r--   0        0        0      521 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/test_imports.py
+-rw-r--r--   0        0        0    21373 2023-05-25 17:13:34.538774 caikit-0.5.3/tests/core/test_model_manager.py
+-rw-r--r--   0        0        0     1038 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/core/test_no_write_permissions.py
+-rw-r--r--   0        0        0     5110 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/core/test_task.py
+-rw-r--r--   0        0        0     7967 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/core/toolkit/test_compatibility.py
+-rw-r--r--   0        0        0    18396 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/core/toolkit/test_error_handler.py
+-rw-r--r--   0        0        0     4997 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/core/toolkit/test_fileio.py
+-rw-r--r--   0        0        0    25851 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/core/toolkit/test_quality_evaluation.py
+-rw-r--r--   0        0        0     2634 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/core/toolkit/test_serializers.py
+-rw-r--r--   0        0        0     7824 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/core/toolkit/test_wip_decorator.py
+-rw-r--r--   0        0        0     6782 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/data_model_helpers.py
+-rw-r--r--   0        0        0       39 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      647 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/config/config.yml
+-rw-r--r--   0        0        0       27 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/data_stream_inputs/bad_file.json
+-rw-r--r--   0        0        0      154 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/data_stream_inputs/control_chars.jsonl
+-rw-r--r--   0        0        0      106 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/data_stream_inputs/sample.csv
+-rw-r--r--   0        0        0       66 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/data_stream_inputs/sample.json
+-rw-r--r--   0        0        0      233 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/data_stream_inputs/sample.jsonl
+-rw-r--r--   0        0        0     1322 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/data_stream_inputs/sample.txt
+-rw-r--r--   0        0        0       11 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
+-rw-r--r--   0        0        0       11 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
+-rw-r--r--   0        0        0       11 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
+-rw-r--r--   0        0        0       27 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
+-rw-r--r--   0        0        0       27 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
+-rw-r--r--   0        0        0       63 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
+-rw-r--r--   0        0        0      147 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
+-rw-r--r--   0        0        0      218 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
+-rw-r--r--   0        0        0       87 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
+-rw-r--r--   0        0        0       52 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
+-rw-r--r--   0        0        0       56 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
+-rw-r--r--   0        0        0       55 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
+-rw-r--r--   0        0        0      125 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/data_stream_inputs/sample_w_header.csv
+-rw-r--r--   0        0        0      222 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/dummy_dataset.json
+-rw-r--r--   0        0        0     1016 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/dummy_module.zip
+-rw-r--r--   0        0        0      675 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/dummy_module/config.yml
+-rw-r--r--   0        0        0      299 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/dummy_module/data.json
+-rw-r--r--   0        0        0       14 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/dummy_module/data.pkl
+-rw-r--r--   0        0        0      191 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/dummy_module_backend/config.yml
+-rw-r--r--   0        0        0      179 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/dummy_module_foo/config.yml
+-rw-r--r--   0        0        0      506 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/dummy_module_no_nesting.zip
+-rw-r--r--   0        0        0      570 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/dummy_module_singleton/config.yml
+-rw-r--r--   0        0        0      299 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/dummy_module_singleton/data.json
+-rw-r--r--   0        0        0       14 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/dummy_module_singleton/data.pkl
+-rw-r--r--   0        0        0      230 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/dummy_resource/config.yml
+-rw-r--r--   0        0        0     3034 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/fixtures.py
+-rw-r--r--   0        0        0      918 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/invalid.zip
+-rw-r--r--   0        0        0     2551 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/linux.txt
+-rw-r--r--   0        0        0       10 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/models/bad_archive.zip
+-rw-r--r--   0        0        0      376 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/models/bad_model.zip
+-rw-r--r--   0        0        0      360 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/models/bar/config.yml
+-rw-r--r--   0        0        0      364 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/models/foo/config.yml
+-rw-r--r--   0        0        0      422 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/models/foo_archive.zip
+-rw-r--r--   0        0        0     2142 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/primitive_party.proto
+-rw-r--r--   0        0        0      145 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/protobufs/__init__.py
+-rw-r--r--   0        0        0     2080 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/protobufs/caikit_runtime_pb2.py
+-rw-r--r--   0        0        0     2447 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     2217 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
+-rw-r--r--   0        0        0     2602 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
+-rw-r--r--   0        0        0     5995 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/protobufs/primitive_party_pb2.py
+-rw-r--r--   0        0        0      416 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/protos/caikit_runtime.proto
+-rw-r--r--   0        0        0      437 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/protos/caikit_runtime_train.proto
+-rw-r--r--   0        0        0       24 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      294 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/sample_lib/__init__.py
+-rw-r--r--   0        0        0      410 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/sample_lib/config.yml
+-rw-r--r--   0        0        0      157 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/sample_lib/data_model/__init__.py
+-rw-r--r--   0        0        0     1257 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/sample_lib/data_model/sample.py
+-rw-r--r--   0        0        0      156 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/sample_lib/modules/__init__.py
+-rw-r--r--   0        0        0       89 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/sample_lib/modules/other_task/__init__.py
+-rw-r--r--   0        0        0     1882 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/sample_lib/modules/other_task/other_implementation.py
+-rw-r--r--   0        0        0      250 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/sample_lib/modules/sample_task/__init__.py
+-rw-r--r--   0        0        0     1720 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/sample_lib/modules/sample_task/composite_module.py
+-rw-r--r--   0        0        0      621 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/sample_lib/modules/sample_task/inner_module.py
+-rw-r--r--   0        0        0     2463 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py
+-rw-r--r--   0        0        0     1282 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py
+-rw-r--r--   0        0        0     2720 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0      364 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/fixtures/sample_module/config.yml
+-rw-r--r--   0        0        0        0 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/runtime/__init__.py
+-rw-r--r--   0        0        0      756 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/runtime/generated/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     3845 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/runtime/metrics/test_rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    14101 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/runtime/model_management/test_batcher.py
+-rw-r--r--   0        0        0    10266 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/runtime/model_management/test_model_loader.py
+-rw-r--r--   0        0        0    17911 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/runtime/model_management/test_model_manager.py
+-rw-r--r--   0        0        0     5303 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/runtime/model_management/test_model_sizer.py
+-rw-r--r--   0        0        0     2254 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/runtime/model_management/test_training_manager.py
+-rw-r--r--   0        0        0        0 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     3349 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/runtime/service_generation/test_create_service.py
+-rw-r--r--   0        0        0    18431 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/runtime/service_generation/test_data_stream_source.py
+-rw-r--r--   0        0        0     4065 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/runtime/service_generation/test_primitives.py
+-rw-r--r--   0        0        0     1688 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/runtime/service_generation/test_rpcs.py
+-rw-r--r--   0        0        0     1376 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/runtime/service_generation/test_type_helpers.py
+-rw-r--r--   0        0        0      577 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     7859 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/runtime/servicers/test_global_predict_servicer_impl.py
+-rw-r--r--   0        0        0    15481 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/runtime/servicers/test_global_train_servicer_impl.py
+-rw-r--r--   0        0        0     3640 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/runtime/servicers/test_model_runtime_servicer_impl.py
+-rw-r--r--   0        0        0     7372 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/runtime/servicers/test_model_train_servicer_impl.py
+-rw-r--r--   0        0        0     4204 2023-05-25 17:13:34.542774 caikit-0.5.3/tests/runtime/servicers/test_training_management_servicer.py
+-rw-r--r--   0        0        0    30156 2023-05-25 17:13:34.546774 caikit-0.5.3/tests/runtime/test_grpc_server.py
+-rw-r--r--   0        0        0    11106 2023-05-25 17:13:34.546774 caikit-0.5.3/tests/runtime/test_service_factory.py
+-rw-r--r--   0        0        0      577 2023-05-25 17:13:34.546774 caikit-0.5.3/tests/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     4899 2023-05-25 17:13:34.546774 caikit-0.5.3/tests/runtime/utils/test_import_util.py
+-rw-r--r--   0        0        0    26269 2023-05-25 17:13:34.546774 caikit-0.5.3/tests/runtime/utils/test_servicer_util.py
+-rw-r--r--   0        0        0      577 2023-05-25 17:13:34.546774 caikit-0.5.3/tests/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     2758 2023-05-25 17:13:34.546774 caikit-0.5.3/tests/runtime/work_management/test_abortable_action.py
+-rw-r--r--   0        0        0     1868 2023-05-25 17:13:34.546774 caikit-0.5.3/tests/runtime/work_management/test_call_aborter.py
+-rw-r--r--   0        0        0     3355 2023-05-25 17:13:34.546774 caikit-0.5.3/tests/runtime/work_management/test_destroyable_thread.py
+-rw-r--r--   0        0        0     2115 2023-05-25 17:13:34.546774 caikit-0.5.3/tox.ini
+-rw-r--r--   0        0        0     4893 1970-01-01 00:00:00.000000 caikit-0.5.3/PKG-INFO
```

### Comparing `caikit-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit-0.5.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit-0.5.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/.github/ISSUE_TEMPLATE/user_story.md` & `caikit-0.5.3/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/.github/workflows/build-library.yml` & `caikit-0.5.3/.github/workflows/build-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/.github/workflows/lint-code.yml` & `caikit-0.5.3/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/.github/workflows/publish-library.yml` & `caikit-0.5.3/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/.pylintrc` & `caikit-0.5.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/CONTRIBUTING.md` & `caikit-0.5.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/LICENSE` & `caikit-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/README.md` & `caikit-0.5.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,10 +35,14 @@
   - They take trained models, deploy them, and then infer the models in applications through APIs provided by Caikit
   - Examples of operators are cloud and embedded application developers whose applications need analysis of unstructured data
 
 ## AI Model Operator Example
 
 Check out the [Text Sentiment example](examples/text-sentiment/) to understand how to load and infer a model using Caikit.
 
+## Contributing
+
+Check out our [contributing](CONTRIBUTING.md) guide to learn how to contribute to Caikit.
+
 ## Code of conduct
 
 Participation in the Caikit community is governed by the [Code of Conduct](CODE-OF-CONDUCT.md).
```

### Comparing `caikit-0.5.2/caikit-overview.png` & `caikit-0.5.3/caikit-overview.png`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/config/__init__.py` & `caikit-0.5.3/caikit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/config/config.py` & `caikit-0.5.3/caikit/config/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/config/config.yml` & `caikit-0.5.3/caikit/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/__init__.py` & `caikit-0.5.3/caikit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/augmentors/__init__.py` & `caikit-0.5.3/caikit/core/augmentors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/augmentors/base.py` & `caikit-0.5.3/caikit/core/augmentors/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/augmentors/merged_augmentor.py` & `caikit-0.5.3/caikit/core/augmentors/merged_augmentor.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/augmentors/schemes/always_selection_scheme.py` & `caikit-0.5.3/caikit/core/augmentors/schemes/always_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/augmentors/schemes/base.py` & `caikit-0.5.3/caikit/core/augmentors/schemes/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/augmentors/schemes/random_multi_selection_scheme.py` & `caikit-0.5.3/caikit/core/augmentors/schemes/random_multi_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/augmentors/schemes/random_single_selection_scheme.py` & `caikit-0.5.3/caikit/core/augmentors/schemes/random_single_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/data_model/__init__.py` & `caikit-0.5.3/caikit/core/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/data_model/base.py` & `caikit-0.5.3/caikit/core/data_model/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,15 +263,14 @@
         #   registry shared for all
         _DataBaseMetaClass.class_registry[cls.full_name] = cls
 
         # Add properties that use the underlying backend. Also add fields that
         # existed in old_fields for supporting oneofs
         # see https://github.com/caikit/caikit/pull/107 for details
         for field in set(cls.fields + tuple(old_fields)):
-
             # If the field is the name of a field within a oneof and it was not
             # in the old fields, the data is held under the oneof's name if this
             # is the set value for the oneof
             if oneof_name := cls._fields_to_oneof.get(field):
                 setattr(cls, field, mcs._make_property_getter(field, oneof_name))
 
             # If the field is a plain field or the name of a oneof, it will be
@@ -367,15 +366,14 @@
                 for i, field_val in enumerate(args):
                     field_name = fields[i]
                     setattr(self, field_name, field_val)
                     used_fields.append(field_name)
 
             if num_kwargs > 0:  # Do a quick check for performance reason
                 for field_name, field_val in kwargs.items():
-
                     # If this is a oneof field, alias to the oneof name
                     if oneof_name := cls._fields_to_oneof.get(field_name):
                         which_oneof[oneof_name] = field_name
                         field_name = oneof_name
 
                     if (
                         field_name not in fields
@@ -771,15 +769,23 @@
                     ),
                 )
 
         return proto
 
     def to_dict(self) -> dict:
         """Convert to a dictionary representation."""
-        return {field: self._field_to_dict_element(field) for field in self.fields}
+        # maintain a list of fields to convert to dict, special handling for oneofs
+        fields_to_dict = []
+        for field in self.fields:
+            if (
+                not field in self._fields_to_oneof
+                or self.which_oneof(self._fields_to_oneof[field]) == field
+            ):
+                fields_to_dict.append(field)
+        return {field: self._field_to_dict_element(field) for field in fields_to_dict}
 
     def to_json(self, **kwargs) -> str:
         """Convert to a json representation."""
 
         def _default_serialization_overrides(obj):
             """Default handler for nonserializable objects; currently this only handles bytes."""
             if isinstance(obj, bytes):
```

### Comparing `caikit-0.5.2/caikit/core/data_model/data_backends/__init__.py` & `caikit-0.5.3/caikit/core/data_model/data_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/data_model/data_backends/base.py` & `caikit-0.5.3/caikit/core/data_model/data_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/data_model/data_backends/dict_backend.py` & `caikit-0.5.3/caikit/core/data_model/data_backends/dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/data_model/dataobject.py` & `caikit-0.5.3/caikit/core/data_model/dataobject.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/data_model/enums.py` & `caikit-0.5.3/caikit/core/data_model/enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/data_model/producer.py` & `caikit-0.5.3/caikit/core/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/data_model/protobufs/__init__.py` & `caikit-0.5.3/caikit/core/data_model/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/data_model/streams/__init__.py` & `caikit-0.5.3/caikit/core/data_model/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/data_model/streams/converter.py` & `caikit-0.5.3/caikit/core/data_model/streams/converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/data_model/streams/csv_column_formatter.py` & `caikit-0.5.3/caikit/core/data_model/streams/csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/data_model/streams/data_stream.py` & `caikit-0.5.3/caikit/core/data_model/streams/data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/data_model/streams/resolver.py` & `caikit-0.5.3/caikit/core/data_model/streams/resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/data_model/streams/validator.py` & `caikit-0.5.3/caikit/core/data_model/streams/validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/model_manager.py` & `caikit-0.5.3/caikit/core/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/module_backends/__init__.py` & `caikit-0.5.3/caikit/core/module_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/module_backends/backend_types.py` & `caikit-0.5.3/caikit/core/module_backends/backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/module_backends/base.py` & `caikit-0.5.3/caikit/core/module_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/module_backends/local_backend.py` & `caikit-0.5.3/caikit/core/module_backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/module_backends/module_backend_config.py` & `caikit-0.5.3/caikit/core/module_backends/module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/modules/__init__.py` & `caikit-0.5.3/caikit/core/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/modules/base.py` & `caikit-0.5.3/caikit/core/modules/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 # First Party
 import alog
 
 # Local
 from ..data_model import DataBase, DataStream
 from ..toolkit import fileio
 from ..toolkit.errors import DataValidationError, error_handler
+from .loader import ModuleLoader
 from .meta import _ModuleBaseMeta
 from caikit import core
 
 log = alog.use_channel("MODULE")
 error = error_handler.get(log)
 
 
@@ -102,20 +103,25 @@
         error(
             "<COR92634438E>",
             NotImplementedError("This is not available in this module."),
         )
 
     @classmethod
     @alog.logged_function(log.debug)
-    def load(cls, *args, **kwargs):
-        """Load a model."""
-        error(
-            "<COR92634437E>",
-            NotImplementedError("This is not available in this module."),
-        )
+    def load(cls, model_path, *args, **kwargs):
+        """Load a new instance of workflow from a given model_path
+
+        Args:
+            model_path: str
+                Path to workflow
+        Returns:
+            caikit.core.workflows.base.WorkflowBase
+                A new instance of any given implementation of WorkflowBase
+        """
+        return cls._load(ModuleLoader(model_path), *args, **kwargs)
 
     @classmethod
     def _load(cls, module_loader, *args, **kwargs):
         """Load a model."""
         error(
             "<COR88356566E>",
             NotImplementedError("This is not available in this module."),
```

### Comparing `caikit-0.5.2/caikit/core/modules/config.py` & `caikit-0.5.3/caikit/core/modules/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/modules/decorator.py` & `caikit-0.5.3/caikit/core/modules/decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 # First Party
 import alog
 
 # Local
 from ..data_model import ProducerId
 from ..registries import module_backend_registry, module_backend_types, module_registry
+from ..signature_parsing import CaikitMethodSignature
 from ..task import TaskBase
 from ..toolkit.errors import error_handler
 from .base import ModuleBase
 import caikit.core
 
 log = alog.use_channel("MODULE_DEC")
 error = error_handler.get(log)
@@ -181,20 +182,24 @@
                     TypeError(
                         f"Class {cls_} has task {task} but superclass has task "
                         f"{parent_task}"
                     ),
                 )
             cls_.TASK_CLASS = parent_task
         else:
-            if not task:
-                # TODO: raise once @tasks are integrated into service generation
-                # raise TypeError(f"task argument is required for @{cls}")
-                pass
             cls_.TASK_CLASS = task
 
+        # Parse the `train` and `run` signatures
+        cls_.RUN_SIGNATURE = CaikitMethodSignature(cls_, "run")
+        cls_.TRAIN_SIGNATURE = CaikitMethodSignature(cls_, "train")
+
+        # If the module has a task, validate it:
+        if cls_.TASK_CLASS:
+            cls_.TASK_CLASS.validate_run_signature(cls_.RUN_SIGNATURE)
+
         # If no backend support described in the class, add current backend
         # as the only backend that can load models trained by this module
         cls_.SUPPORTED_LOAD_BACKENDS = getattr(
             cls_, SUPPORTED_LOAD_BACKENDS_VAR_NAME, [backend_type]
         )
 
         # Set its own backend_type as an attribute
```

### Comparing `caikit-0.5.2/caikit/core/modules/loader.py` & `caikit-0.5.3/caikit/core/modules/loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/modules/meta.py` & `caikit-0.5.3/caikit/core/modules/meta.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/modules/saver.py` & `caikit-0.5.3/caikit/core/modules/saver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/registries.py` & `caikit-0.5.3/caikit/core/registries.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/task.py` & `caikit-0.5.3/caikit/core/task.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Standard
 from typing import Callable, Dict, List, Type, Union
+import typing
 
 # First Party
 from alog import alog
 
 # Local
 from .data_model import DataStream
 from .data_model.base import DataBase
+from .signature_parsing import CaikitMethodSignature
 from .toolkit.errors import error_handler
 
 log = alog.use_channel("TASK_BASE")
 error = error_handler.get(log)
 
 ProtoableInputTypes = Type[Union[int, float, str, bytes, bool, DataBase]]
 ValidInputTypes = Union[
@@ -38,17 +40,51 @@
     An AI task is a logical function signature which, when implemented, performs
     a task in some AI domain. The key property of a task is that the set of
     required input argument types and the output value type are consistent
     across all implementations of the task.
     """
 
     @classmethod
-    def validate_run_signature(cls) -> bool:
-        # TODO: implement
-        pass
+    def validate_run_signature(cls, signature: CaikitMethodSignature) -> None:
+        if not signature.parameters:
+            raise ValueError(
+                "Task could not be validated, no .run parameters were provided"
+            )
+        if signature.return_type is None:
+            raise ValueError(
+                "Task could not be validated, no .run return type was provided"
+            )
+
+        missing_required_params = [
+            parameter_name
+            for parameter_name in cls.get_required_parameters()
+            if parameter_name not in signature.parameters
+        ]
+        if missing_required_params:
+            raise TypeError(
+                f"Required parameters {missing_required_params} not in signature for module: "
+                f"{signature.module}"
+            )
+
+        type_mismatch_errors = []
+        for parameter_name, parameter_type in cls.get_required_parameters().items():
+            signature_type = signature.parameters[parameter_name]
+            if parameter_type != signature_type:
+                if typing.get_origin(
+                    signature_type
+                ) == typing.Union and parameter_type in typing.get_args(signature_type):
+                    continue
+                type_mismatch_errors.append(
+                    f"Parameter {parameter_name} has type {signature_type} but type \
+                        {parameter_type} is required"
+                )
+        if type_mismatch_errors:
+            raise TypeError(
+                f"Wrong types provided for parameters to {signature.module}: {type_mismatch_errors}"
+            )
 
     @classmethod
     def get_required_parameters(cls) -> Dict[str, ValidInputTypes]:
         """Get the set of input types required by this task
 
         NOTE: This method is automatically configured by the @task decorator
             and should not be overwritten by child classes.
```

### Comparing `caikit-0.5.2/caikit/core/toolkit/__init__.py` & `caikit-0.5.3/caikit/core/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/toolkit/compatibility.py` & `caikit-0.5.3/caikit/core/toolkit/compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/toolkit/errors/__init__.py` & `caikit-0.5.3/caikit/core/toolkit/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/toolkit/errors/error_handler.py` & `caikit-0.5.3/caikit/core/toolkit/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/toolkit/errors/validation_error.py` & `caikit-0.5.3/caikit/core/toolkit/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/toolkit/fileio.py` & `caikit-0.5.3/caikit/core/toolkit/fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/toolkit/isa.py` & `caikit-0.5.3/caikit/core/toolkit/isa.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/toolkit/logging.py` & `caikit-0.5.3/caikit/core/toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/toolkit/quality_evaluation.py` & `caikit-0.5.3/caikit/core/toolkit/quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/toolkit/serializers.py` & `caikit-0.5.3/caikit/core/toolkit/serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/core/toolkit/wip_decorator.py` & `caikit-0.5.3/caikit/core/toolkit/wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/interfaces/__init__.py` & `caikit-0.5.3/caikit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/interfaces/common/__init__.py` & `caikit-0.5.3/caikit/interfaces/common/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/interfaces/common/data_model/__init__.py` & `caikit-0.5.3/caikit/interfaces/common/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/interfaces/common/data_model/producer.py` & `caikit-0.5.3/caikit/interfaces/common/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/interfaces/runtime/__init__.py` & `caikit-0.5.3/caikit/interfaces/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/interfaces/runtime/data_model/__init__.py` & `caikit-0.5.3/caikit/interfaces/runtime/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/interfaces/runtime/data_model/training_management.py` & `caikit-0.5.3/caikit/interfaces/runtime/data_model/training_management.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/__init__.py` & `caikit-0.5.3/caikit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/dump_services.py` & `caikit-0.5.3/caikit/runtime/dump_services.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/grpc_server.py` & `caikit-0.5.3/caikit/runtime/grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/interceptors/__init__.py` & `caikit-0.5.3/caikit/runtime/interceptors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py` & `caikit-0.5.3/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/metrics/__init__.py` & `caikit-0.5.3/caikit/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/metrics/rpc_meter.py` & `caikit-0.5.3/caikit/runtime/metrics/rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/model_management/__init__.py` & `caikit-0.5.3/caikit/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/model_management/batcher.py` & `caikit-0.5.3/caikit/runtime/model_management/batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/model_management/loaded_model.py` & `caikit-0.5.3/caikit/runtime/model_management/loaded_model.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/model_management/model_loader.py` & `caikit-0.5.3/caikit/runtime/model_management/model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/model_management/model_manager.py` & `caikit-0.5.3/caikit/runtime/model_management/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/model_management/model_sizer.py` & `caikit-0.5.3/caikit/runtime/model_management/model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/model_management/training_manager.py` & `caikit-0.5.3/caikit/runtime/model_management/training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/protobufs/__init__.py` & `caikit-0.5.3/caikit/runtime/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/protobufs/model_mesh_pb2.py` & `caikit-0.5.3/caikit/runtime/protobufs/model_mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/protobufs/model_mesh_pb2_grpc.py` & `caikit-0.5.3/caikit/runtime/protobufs/model_mesh_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/protobufs/model_runtime_pb2.py` & `caikit-0.5.3/caikit/runtime/protobufs/model_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/protobufs/model_runtime_pb2_grpc.py` & `caikit-0.5.3/caikit/runtime/protobufs/model_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/protobufs/process_pb2.py` & `caikit-0.5.3/caikit/runtime/protobufs/process_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/protobufs/process_pb2_grpc.py` & `caikit-0.5.3/caikit/runtime/protobufs/process_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/protobufs/protos/model-mesh.proto` & `caikit-0.5.3/caikit/runtime/protobufs/protos/model-mesh.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/protobufs/protos/model-runtime.proto` & `caikit-0.5.3/caikit/runtime/protobufs/protos/model-runtime.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/protobufs/protos/process.proto` & `caikit-0.5.3/caikit/runtime/protobufs/protos/process.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/service_factory.py` & `caikit-0.5.3/caikit/runtime/service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/service_generation/compatibility_checker.py` & `caikit-0.5.3/caikit/runtime/service_generation/compatibility_checker.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/service_generation/core_module_helpers.py` & `caikit-0.5.3/caikit/runtime/service_generation/core_module_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/service_generation/create_service.py` & `caikit-0.5.3/caikit/runtime/service_generation/create_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 import alog
 
 # Local
 from ... import get_config
 from .core_module_helpers import get_module_info
 from .primitives import is_primitive_method
 from .rpcs import CaikitRPCBase, ModuleClassTrainRPC, TaskPredictRPC
-from .signature_parsing.module_signature import CaikitCoreModuleMethodSignature
 from caikit.core import ModuleBase
+from caikit.core.signature_parsing.module_signature import CaikitMethodSignature
 
 log = alog.use_channel("CREATE-RPCS")
 
 ## Globals #####################################################################
 
 INFERENCE_FUNCTION_NAME = "run"
 TRAIN_FUNCTION_NAME = "train"
@@ -90,15 +90,15 @@
             log.debug(
                 "Skipping train API for %s with no %s function",
                 ck_module,
                 TRAIN_FUNCTION_NAME,
             )
             continue
 
-        signature = CaikitCoreModuleMethodSignature(ck_module, TRAIN_FUNCTION_NAME)
+        signature = CaikitMethodSignature(ck_module, TRAIN_FUNCTION_NAME)
         log.debug(
             "Function signature for %s::%s [%s -> %s]",
             ck_module,
             TRAIN_FUNCTION_NAME,
             signature.parameters,
             signature.return_type,
         )
@@ -119,15 +119,15 @@
 def _remove_non_primitive_modules(
     modules: List[Type[ModuleBase]],
     primitive_data_model_types: List[str],
 ) -> List[Type[ModuleBase]]:
     primitive_modules = []
     # If the module is not "primitive" we won't include it
     for ck_module in modules:
-        signature = CaikitCoreModuleMethodSignature(ck_module, "run")
+        signature = CaikitMethodSignature(ck_module, "run")
         if signature.parameters and signature.return_type:
             if not is_primitive_method(signature, primitive_data_model_types):
                 log.debug("Skipping non-primitive module %s", ck_module)
                 continue
 
             primitive_modules.append(ck_module)
     return primitive_modules
@@ -140,15 +140,15 @@
 ) -> List[CaikitRPCBase]:
     """Create the RPCs for each module"""
     rpcs = []
     task_groups = {}
 
     for ck_module in modules:
         module_info = get_module_info(ck_module)
-        signature = CaikitCoreModuleMethodSignature(ck_module, fname)
+        signature = CaikitMethodSignature(ck_module, fname)
         # Group each module by its task
         if module_info is not None:
             task_groups.setdefault((module_info.library, module_info.type), []).append(
                 signature
             )
 
     # Create the RPC for each task
```

### Comparing `caikit-0.5.2/caikit/runtime/service_generation/data_stream_source.py` & `caikit-0.5.3/caikit/runtime/service_generation/data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/service_generation/primitives.py` & `caikit-0.5.3/caikit/runtime/service_generation/primitives.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 import sys
 import typing
 
 # First Party
 import alog
 
 # Local
-from .signature_parsing.module_signature import CaikitCoreModuleMethodSignature
 from .type_helpers import PROTO_TYPE_MAP
 from caikit.core.data_model.base import DataBase
+from caikit.core.signature_parsing.module_signature import CaikitMethodSignature
 
 log = alog.use_channel("MODULE_PRIMS")
 
 
 def to_primitive_signature(
     signature: Dict[str, Type], primitive_data_model_types: List[str]
 ) -> Dict[str, Type]:
@@ -118,23 +118,23 @@
     # if it's anything else we just return as is
     # we don't actually want to throw errors from service generation
     log.warning("Return type [%s] not a DM type, returning as is", arg_type)
     return arg_type
 
 
 def is_primitive_method(
-    method: CaikitCoreModuleMethodSignature, primitive_data_model_types: List[str]
+    method: CaikitMethodSignature, primitive_data_model_types: List[str]
 ) -> bool:
     """Determine if the arguments to the module's run function meet the criteria
     for being a "primitive" interface this means that all **non-optional** arguments
     types must be either (a) a primitive data model type for the given library or
     (b) a language-primitive type.
 
     Args:
-        method (CaikitCoreModuleMethodSignature): The method signature of the "primitive"
+        method (CaikitMethodSignature): The method signature of the "primitive"
             data model types for each library
     """
 
     # pylint: disable=use-a-generator
     return all(
         [
             (
```

### Comparing `caikit-0.5.2/caikit/runtime/service_generation/rpcs.py` & `caikit-0.5.3/caikit/runtime/service_generation/rpcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,27 +27,24 @@
     FieldNumber,
 )
 import alog
 
 # Local
 from . import primitives, type_helpers
 from .compatibility_checker import ApiFieldNames
-from .signature_parsing.module_signature import (
-    CaikitCoreModuleMethodSignature,
-    CustomSignature,
-)
+from .data_stream_source import make_data_stream_source
 from caikit.core import ModuleBase
 from caikit.core.data_model.base import DataBase
 from caikit.core.data_model.dataobject import (
     DataObjectBase,
     _DataObjectBaseMetaClass,
     dataobject,
 )
+from caikit.core.signature_parsing import CaikitMethodSignature, CustomSignature
 from caikit.interfaces.runtime.data_model import ModelPointer, TrainingJob
-from caikit.runtime.service_generation.data_stream_source import make_data_stream_source
 
 log = alog.use_channel("RPC-SERIALIZERS")
 
 INDENT = "    "
 
 
 class CaikitRPCBase(abc.ABC):
@@ -111,21 +108,21 @@
 class ModuleClassTrainRPC(CaikitRPCBase):
     """Helper class to create a unique RPC corresponding with the train function
     for a given module class
     """
 
     def __init__(
         self,
-        method_signature: CaikitCoreModuleMethodSignature,
+        method_signature: CaikitMethodSignature,
         primitive_data_model_types: List[str],
     ):
         """Initialize a .proto generator with a single module to convert
 
         Args:
-            method_signature (CaikitCoreModuleMethodSignature): The module method signature to
+            method_signature (CaikitMethodSignature): The module method signature to
             generate an RPC for
 
             primitive_data_model_types: List[str]
                 List of primitive data model types for a caikit_* library, such as
                 caikit.interfaces.nlp.data_model.RawDocument for nlp domains
         """
         self.clz: Type[ModuleBase] = method_signature.module
@@ -177,15 +174,15 @@
         return snake_to_upper_camel(
             f"{module_split[1]}_{module_split[2]}_{self.clz.__name__}_TrainRequest"
         )
 
     @staticmethod
     def _mutate_method_signature_for_training(
         signature, primitive_data_model_types: List[str]
-    ) -> Optional[CaikitCoreModuleMethodSignature]:
+    ) -> Optional[CaikitMethodSignature]:
         # Change return type for async training interface
         return_type = TrainingJob
 
         new_params = {"model_name": str}
         for name, typ in signature.parameters.items():
             if type_helpers.has_data_stream(typ):
                 # Assume this is training data
@@ -215,24 +212,24 @@
     """Helper class to create a unique RPC for the aggregate set of Modules that
     implement the same task
     """
 
     def __init__(
         self,
         task: Tuple[str, str],
-        method_signatures: List[CaikitCoreModuleMethodSignature],
+        method_signatures: List[CaikitMethodSignature],
         primitive_data_model_types: List[str],
     ):
         """Initialize a .proto generator with all modules of a given task to convert
 
         Args:
             task (Tuple[str, str]): The library / ai-problem-task combo that describes the task
                 type. For example: ("my_caikit_library", "classification")
 
-            method_signatures (List[CaikitCoreModuleMethodSignature]): The list of method
+            method_signatures (List[CaikitMethodSignature]): The list of method
                 signatures from concrete modules implementing this task
 
             primitive_data_model_types: List[str]
                 List of primitive data model types for a caikit_* library, such as
                 caikit.interfaces.nlp.data_model.RawDocument for nlp domains
         """
         self.task = task
```

### Comparing `caikit-0.5.2/caikit/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.5.3/examples/text-sentiment/text_sentiment/data_model/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,11 +7,10 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 # Local
-from .docstrings import *
-from .module_signature import *
-from .parsers import *
+from .classification import ClassificationPrediction, ClassInfo, TextInput
```

### Comparing `caikit-0.5.2/caikit/runtime/service_generation/signature_parsing/docstrings.py` & `caikit-0.5.3/caikit/core/signature_parsing/docstrings.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,23 +16,22 @@
 
 # Standard
 from typing import Callable, Dict, List, Optional, Tuple, Type, Union
 import builtins
 import sys
 
 # Third Party
+from docstring_parser import ParseError
 import docstring_parser
-import grpc
 
 # First Party
 import alog
 
 # Local
 from caikit.core.data_model.base import DataBase
-from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 import caikit.core
 
 log = alog.use_channel("DOCSTRINGS")
 
 
 def get_return_type(fn: Callable) -> Optional[Type]:
     """
@@ -42,19 +41,17 @@
             e.g. my_caikit_library.modules.classification.Transformer.run
 
     Returns:
         The return type of `fn`, if it can be parsed from the docstring. Otherwise, None
     """
     try:
         docstring = docstring_parser.parse(fn.__doc__)
-    except Exception as exc:
-        raise CaikitRuntimeException(
-            grpc.StatusCode.INVALID_ARGUMENT,
-            f"ParseError when parsing docstring for function: {fn.__name__}",
-        ) from exc
+    except docstring_parser.ParseError as e:
+        log.warning("Could not parse docstring: %s fn.__doc__ ", fn.__doc__, exc_info=e)
+        return None
 
     type_names, desc_names = _get_candidate_type_names_from_docstring(docstring.returns)
 
     return_type = _get_docstring_type(type_names)
     if return_type:
         return return_type
 
@@ -71,19 +68,22 @@
         fn: The function to get the type of a parameter from
             e.g.  my_caikit_library.modules.classification.Transformer.run
         arg_name: The name of the parameter that we should try to get the type of
             e.g. "raw_document"
     """
     try:
         docstring = docstring_parser.parse(fn.__doc__)
-    except Exception as exc:
-        raise CaikitRuntimeException(
-            grpc.StatusCode.INVALID_ARGUMENT,
-            f"ParseError when parsing docstring for function: {fn.__name__}",
-        ) from exc
+    except ParseError as parse_error:
+        log.warning(
+            "Failed to parse docstring for %s when looking for optional flag on parameter %s",
+            fn,
+            arg_name,
+            exc_info=parse_error,
+        )
+        return False
 
     ds_param = [param for param in docstring.params if param.arg_name == arg_name]
     if ds_param:
         if len(ds_param) > 1:
             log.warning("Docstring has multiple args with the same name! %s", arg_name)
         ds_param = ds_param[0]
 
@@ -106,22 +106,24 @@
         fn: The function to get the type of a parameter from
             e.g. my_caikit_library.modules.classification.Transformer.run
         arg_name: The name of the parameter that we should try to get the type of
             e.g. "raw_document"
     Returns:
         The return type of `fn`, if it can be parsed from the docstring. Otherwise, None
     """
-
     try:
         docstring = docstring_parser.parse(fn.__doc__)
-    except Exception as exc:
-        raise CaikitRuntimeException(
-            grpc.StatusCode.INVALID_ARGUMENT,
-            f"ParseError when parsing docstring for function: {fn.__name__}",
-        ) from exc
+    except ParseError as parse_error:
+        log.warning(
+            "Failed to parse docstring for %s when looking for type on parameter %s",
+            fn,
+            arg_name,
+            exc_info=parse_error,
+        )
+        return None
 
     ds_param = [param for param in docstring.params if param.arg_name == arg_name]
     if ds_param:
         if len(ds_param) > 1:
             log.warning("Docstring has multiple args with the same name! %s", arg_name)
         ds_param = ds_param[0]
         type_names, desc_names = _get_candidate_type_names_from_docstring(ds_param)
```

### Comparing `caikit-0.5.2/caikit/runtime/service_generation/signature_parsing/module_signature.py` & `caikit-0.5.3/caikit/core/signature_parsing/module_signature.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,21 +24,20 @@
 import inspect
 
 # First Party
 import alog
 
 # Local
 from . import parsers
-from caikit.core import ModuleBase
+import caikit
 
-log = alog.use_channel("MODULE-SIGNR")
+log = alog.use_channel("SIGNATURE")
 
 
-# Maybe TODO: support for `INPUT_TYPES` and `OUTPUT_TYPE` from module annotations was removed
-class CaikitCoreModuleMethodSignature:
+class CaikitMethodSignature:
     """Metadata about a method on a caikit core module
 
     Determines the argument types and return type for a function (run, train, etc.)
     of the given caikit core module in any way possible!
 
     This is the most "heuristic" part of this process. Currently, there is no
     well-defined mechanism for defining the types of a module's run signature in
@@ -49,15 +48,17 @@
 
     1. Look for a known type mapping based on the name of the argument
     2. Look for python type annotations
     3. Look for a default value and check its type
     4. Parse the docstring
     """
 
-    def __init__(self, caikit_core_module: Type[ModuleBase], method_name: str):
+    def __init__(
+        self, caikit_core_module: Type["caikit.core.ModuleBase"], method_name: str
+    ):
         self._module = caikit_core_module
         self._method_name = method_name
 
         try:
             self._method_pointer = getattr(self._module, self._method_name)
             self._default_map = parsers.get_args_with_defaults(self._method_pointer)
             method_signature = inspect.signature(self._method_pointer)
@@ -72,15 +73,15 @@
                 self.method_name,
             )
             self._return_type = None
             self._parameters = None
             self._default_map = {}
 
     @property
-    def module(self) -> Type[ModuleBase]:
+    def module(self) -> Type["caikit.core.ModuleBase"]:
         """The concrete caikit.core.ModuleBase type"""
         return self._module
 
     @property
     def method_name(self) -> str:
         """The name of the method on this module, e.g. 'run' or 'train'"""
         return self._method_name
@@ -98,24 +99,24 @@
 
     @property
     def default_parameters(self) -> Dict[str, Any]:
         """A set of all parameter names which have default values"""
         return self._default_map
 
 
-class CustomSignature(CaikitCoreModuleMethodSignature):
+class CustomSignature(CaikitMethodSignature):
     """(TBD on new class)? Need something to hold an intentionally mutated representation of a
     method signature. This represents the extra indirection that lives in the runtime, between the
     service API and the actual method. For example: .train functions return a fully constructed
     module, but the runtime will invoke .train asynchronously and instead return some handle that
     can be used to check training status."""
 
     def __init__(
         self,
-        original_signature: CaikitCoreModuleMethodSignature,
+        original_signature: CaikitMethodSignature,
         parameters: Dict[str, Type],
         return_type: Optional[Type],
     ):
         super().__init__(original_signature.module, original_signature.method_name)
         self._module = original_signature.module
         self._method_name = original_signature.method_name
         self._method_pointer = original_signature._method_pointer
```

### Comparing `caikit-0.5.2/caikit/runtime/service_generation/signature_parsing/parsers.py` & `caikit-0.5.3/caikit/core/signature_parsing/parsers.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,18 +18,17 @@
 from typing import Any, Callable, Dict, List, Optional, Type
 import inspect
 
 # First Party
 import alog
 
 # Local
+from ..data_model.base import DataBase
+from ..modules import ModuleBase
 from . import docstrings
-from caikit.core import ModuleBase
-from caikit.core.data_model.base import DataBase
-from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 
 log = alog.use_channel("SIG-PARSING")
 
 # Constants ##################################
 KNOWN_ARG_TYPES = {
     "producer_id": "ProducerId",
 }
@@ -56,19 +55,15 @@
                     fn_signature.return_annotation,
                 )
                 return module_class
         else:
             return fn_signature.return_annotation
 
     # Check the docstring
-    type_from_docstring = None
-    try:
-        type_from_docstring = docstrings.get_return_type(fn)
-    except CaikitRuntimeException:
-        log.warning("Failed to parse the docstring for %s", fn)
+    type_from_docstring = docstrings.get_return_type(fn)
 
     if type_from_docstring:
         return type_from_docstring
 
     # If we get here, it means no annotation or docstring for type was provided
     log.warning(
         "Could not deduct output type from function %s for module class %s.",
@@ -134,22 +129,23 @@
     # Use known arg types first
     # This avoids cases where docstrings are very obviously flubbed, such as
     #   `raw_document` being annotated as a `str` only in caikit.interfaces.nlp
     dm_type_from_known_arg_types = _get_dm_type_from_name(KNOWN_ARG_TYPES.get(arg.name))
     if dm_type_from_known_arg_types:
         # Not checking if this is optional: These known types should never be optional (maybe...?)
         # This could totally be incorrect!
+        log.info(
+            "Using well known type %s for parameter name %s",
+            dm_type_from_known_arg_types,
+            arg.name,
+        )
         return dm_type_from_known_arg_types
 
     # Check docstring for optional arg
-    optional_arg = False
-    try:
-        optional_arg = docstrings.is_optional(module_method, arg.name)
-    except CaikitRuntimeException:
-        log.warning("Failed to parse the docstring for %s", module_method)
+    optional_arg = docstrings.is_optional(module_method, arg.name)
 
     # Look for a type annotation
     if arg.annotation != inspect.Parameter.empty:
         log.debug("Found annotation for %s", arg.name)
         if optional_arg:
             return Optional[arg.annotation]
         return arg.annotation
@@ -158,19 +154,15 @@
 
     # Check for a default argument and return its type
     default_type = _get_default_type(arg)
     if default_type:
         return default_type
 
     # Parse docstring
-    type_from_docstring = None
-    try:
-        type_from_docstring = docstrings.get_arg_type(module_method, arg.name)
-    except CaikitRuntimeException:
-        log.warning("Failed to parse the docstring for %s", module_method)
+    type_from_docstring = docstrings.get_arg_type(module_method, arg.name)
     if type_from_docstring:
         if optional_arg:
             return Optional[type_from_docstring]
         return type_from_docstring
 
     # Look for a data model object whose name matches the argument name and fall
     # back to the KNOWN_ARG_TYPES dict
```

### Comparing `caikit-0.5.2/caikit/runtime/service_generation/type_helpers.py` & `caikit-0.5.3/caikit/runtime/service_generation/type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/servicers/__init__.py` & `caikit-0.5.3/caikit/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/servicers/global_predict_servicer.py` & `caikit-0.5.3/caikit/runtime/servicers/global_predict_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/servicers/global_train_servicer.py` & `caikit-0.5.3/caikit/runtime/servicers/global_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/servicers/model_runtime_servicer.py` & `caikit-0.5.3/caikit/runtime/servicers/model_runtime_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/servicers/model_train_servicer.py` & `caikit-0.5.3/caikit/runtime/servicers/model_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/servicers/training_management_servicer.py` & `caikit-0.5.3/caikit/runtime/servicers/training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/types/__init__.py` & `caikit-0.5.3/caikit/runtime/types/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/types/aborted_exception.py` & `caikit-0.5.3/caikit/runtime/types/aborted_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/types/caikit_runtime_exception.py` & `caikit-0.5.3/caikit/runtime/types/caikit_runtime_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/types/thread_destroyed_exception.py` & `caikit-0.5.3/caikit/runtime/types/thread_destroyed_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/utils/__init__.py` & `caikit-0.5.3/caikit/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/utils/import_util.py` & `caikit-0.5.3/caikit/runtime/utils/import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/utils/servicer_util.py` & `caikit-0.5.3/caikit/runtime/utils/servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/work_management/__init__.py` & `caikit-0.5.3/caikit/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/work_management/abortable_action.py` & `caikit-0.5.3/caikit/runtime/work_management/abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/work_management/call_aborter.py` & `caikit-0.5.3/caikit/runtime/work_management/call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/caikit/runtime/work_management/destroyable_thread.py` & `caikit-0.5.3/caikit/runtime/work_management/destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/docs/Makefile` & `caikit-0.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/docs/adrs/010-data-model-definition.md` & `caikit-0.5.3/docs/adrs/010-data-model-definition.md`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/docs/adrs/015-runtime-service-generation.md` & `caikit-0.5.3/docs/adrs/015-runtime-service-generation.md`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/docs/adrs/018-shared-backends.md` & `caikit-0.5.3/docs/adrs/018-shared-backends.md`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/docs/adrs/019-loader-stack.md` & `caikit-0.5.3/docs/adrs/019-loader-stack.md`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/docs/architecture_club/04-25-23.md` & `caikit-0.5.3/docs/architecture_club/04-25-23.md`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/docs/conf.py` & `caikit-0.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/docs/make.bat` & `caikit-0.5.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/examples/start_runtime_with_sample_lib.py` & `caikit-0.5.3/examples/start_runtime_with_sample_lib.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/examples/text-sentiment/README.md` & `caikit-0.5.3/examples/text-sentiment/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/examples/text-sentiment/client.py` & `caikit-0.5.3/examples/text-sentiment/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,13 +29,13 @@
 
 client_stub = inference_service.stub_class(channel)
 
 # print(dir(client_stub))
 
 for text in ["I am not feeling well today!", "Today is a nice sunny day"]:
     input_text_proto = TextInput(text=text).to_proto()
-    request = inference_service.messages.HfBlockRequest(text_input=input_text_proto)
-    response = client_stub.HfBlockPredict(
+    request = inference_service.messages.HfModuleRequest(text_input=input_text_proto)
+    response = client_stub.HfModulePredict(
         request, metadata=[("mm-model-id", "text_sentiment")]
     )
     print("Text:", text)
     print("RESPONSE:", response)
```

### Comparing `caikit-0.5.2/examples/text-sentiment/models/text_sentiment/config.yml` & `caikit-0.5.3/examples/text-sentiment/models/text_sentiment/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/examples/text-sentiment/start_runtime.py` & `caikit-0.5.3/examples/text-sentiment/start_runtime.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/examples/text-sentiment/text_sentiment/__init__.py` & `caikit-0.5.3/examples/text-sentiment/text_sentiment/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/examples/text-sentiment/text_sentiment/config.yml` & `caikit-0.5.3/examples/text-sentiment/text_sentiment/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/examples/text-sentiment/text_sentiment/data_model/__init__.py` & `caikit-0.5.3/tests/core/signature_parsing/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,10 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-# Local
-from .classification import ClassificationPrediction, ClassInfo, TextInput
```

### Comparing `caikit-0.5.2/examples/text-sentiment/text_sentiment/data_model/classification.py` & `caikit-0.5.3/examples/text-sentiment/text_sentiment/data_model/classification.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/examples/text-sentiment/text_sentiment/runtime_model/__init__.py` & `caikit-0.5.3/examples/text-sentiment/text_sentiment/runtime_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py` & `caikit-0.5.3/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/pyproject.toml` & `caikit-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "caikit"
 # Not the actual current version: overwritten by CI
-version = "0.5.2"
+version = "0.5.3"
 description = "AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = "~=3.8"
 classifiers=[
     "License :: OSI Approved :: Apache Software License"
 ]
```

### Comparing `caikit-0.5.2/scripts/check_deps.sh` & `caikit-0.5.3/scripts/check_deps.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/scripts/fmt.sh` & `caikit-0.5.3/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/__init__.py` & `caikit-0.5.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/base.py` & `caikit-0.5.3/tests/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/config/test_configs.py` & `caikit-0.5.3/tests/config/test_configs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/conftest.py` & `caikit-0.5.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/core/augmentors/test_augmentor_base.py` & `caikit-0.5.3/tests/core/augmentors/test_augmentor_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/core/augmentors/test_merged_augmentors.py` & `caikit-0.5.3/tests/core/augmentors/test_merged_augmentors.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/core/data_model/data_backends/test_dict_backend.py` & `caikit-0.5.3/tests/core/data_model/data_backends/test_dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/core/data_model/streams/test_converter.py` & `caikit-0.5.3/tests/core/data_model/streams/test_converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/core/data_model/streams/test_csv_column_formatter.py` & `caikit-0.5.3/tests/core/data_model/streams/test_csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/core/data_model/streams/test_data_stream.py` & `caikit-0.5.3/tests/core/data_model/streams/test_data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/core/data_model/streams/test_resolver.py` & `caikit-0.5.3/tests/core/data_model/streams/test_resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/core/data_model/streams/test_validator.py` & `caikit-0.5.3/tests/core/data_model/streams/test_validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/core/data_model/test_base.py` & `caikit-0.5.3/tests/core/data_model/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/core/data_model/test_dataobject.py` & `caikit-0.5.3/tests/core/data_model/test_dataobject.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,26 +377,32 @@
     # Test other oneof field name
     bar1 = BazObj(bar=BazObj.Bar(data="world"))
     assert isinstance(bar1.data_stream, BazObj.Bar)
     assert bar1.which_oneof("data_stream") == "bar"
     assert bar1.bar is bar1.data_stream
     assert bar1.foo is None
 
+    # Test to_dict
+    dict_repr_foo = foo1.to_dict()
+    assert dict_repr_foo == {
+        "foo": {"data": ["hello"]},
+    }
+    assert dict_repr_foo["foo"]["data"] == ["hello"]
+
     # Test proto round trip
     proto_repr_foo = foo1.to_proto()
     assert proto_repr_foo.foo.data == ["hello"]
     assert BazObj.from_proto(proto=proto_repr_foo).to_proto() == proto_repr_foo
     proto_repr_bar = bar1.to_proto()
     assert proto_repr_bar.bar.data == "world"
 
     # Test json round trip
     json_repr_foo = foo1.to_json()
     assert json.loads(json_repr_foo) == {
         "foo": {"data": ["hello"]},
-        "bar": None,
     }
     assert BazObj.from_json(json_repr_foo) == foo1
 
     # Test setattr
     foo1.bar = BazObj.Bar(data="it's a bar")
     assert foo1.which_oneof("data_stream") == "bar"
     assert foo1.data_stream is foo1.bar
@@ -474,19 +480,21 @@
     assert Foo.from_proto(proto=proto_repr_foo).to_proto() == proto_repr_foo
 
     foo2 = Foo(foo=2)
     assert foo2.which_oneof("foo") == "foo_int"
     proto_repr_foo = foo2.to_proto()
     assert Foo.from_proto(proto=proto_repr_foo).to_proto() == proto_repr_foo
 
+    # dict test
+    assert foo1.to_dict() == {"foo_int": 2}
+
     # json round trip
     json_repr_foo = foo1.to_json()
     assert json.loads(json_repr_foo) == {
         "foo_int": 2,
-        "foo_float": None,
     }
     assert Foo.from_json(json_repr_foo) == foo1
 
 
 def test_dataobject_round_trip_json():
     """Make sure that a dataobject class can serialize to/from json"""
```

### Comparing `caikit-0.5.2/tests/core/data_model/test_enums.py` & `caikit-0.5.3/tests/core/data_model/test_enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/core/data_model/test_producer.py` & `caikit-0.5.3/tests/core/data_model/test_producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/core/helpers.py` & `caikit-0.5.3/tests/core/helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/core/module_backends/test_backend_types.py` & `caikit-0.5.3/tests/core/module_backends/test_backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/core/module_backends/test_module_backend_config.py` & `caikit-0.5.3/tests/core/module_backends/test_module_backend_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -188,28 +188,28 @@
 
 
 def test_multiple_module_same_backend_configures(reset_globals):
     """Test to check if multiple modules for same backend
     can override backend configurations"""
     # Register backend type
 
-    @module(id="foo", name="dummy base", version="0.0.1", task=SampleTask)
+    @module(id="foo", name="dummy base", version="0.0.1")
     class DummyFoo(base.ModuleBase):
         pass
 
     # Create dummy classes
     @module(
         base_module=DummyFoo,
         backend_type=backend_types.MOCK,
         backend_config_override={"bar1": 1},
     )
     class DummyBar(base.ModuleBase):
         pass
 
-    @module(id="foo2", name="dummy base", version="0.0.1", task=SampleTask)
+    @module(id="foo2", name="dummy base", version="0.0.1")
     class DummyFoo2(base.ModuleBase):
         pass
 
     # Create dummy classes
     @module(
         base_module=DummyFoo2,
         backend_type=backend_types.MOCK,
```

### Comparing `caikit-0.5.2/tests/core/modules/test_module.py` & `caikit-0.5.3/tests/core/modules/test_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,21 +17,20 @@
 import os
 import tempfile
 
 # First Party
 import aconfig
 
 # Local
-from caikit.core import ModuleConfig
+from caikit.core import ModuleConfig, ModuleLoader
 from caikit.core.module_backends.module_backend_config import configured_load_backends
 from caikit.core.modules.decorator import SUPPORTED_LOAD_BACKENDS_VAR_NAME
-from caikit.core.registries import module_backend_registry
 
 # pylint: disable=import-error
-from sample_lib.data_model.sample import SampleInputType, SampleTask
+from sample_lib.data_model.sample import SampleInputType
 
 # Unit Test Infrastructure
 from tests.conftest import temp_config
 
 # NOTE: We do need to import `reset_backend_types` and `reset_module_distribution_registry` for `reset_globals` to work
 from tests.core.helpers import *
 import caikit.core
@@ -57,17 +56,15 @@
 DUMMY_MODULE_ID = "foo"
 
 
 def configure_alternate_backend_impl():
     """Function to register a new backend type and register a module implementation
     of existing caikit.core module"""
 
-    @caikit.core.modules.module(
-        id=DUMMY_MODULE_ID, name="dummy base", version="0.0.1", task=SampleTask
-    )
+    @caikit.core.modules.module(id=DUMMY_MODULE_ID, name="dummy base", version="0.0.1")
     class DummyFoo(caikit.core.ModuleBase):
         pass
 
     # Register backend type
     backend_types.register_backend_type(MockBackend)
 
     @caikit.core.modules.module(base_module=DummyFoo, backend_type=backend_types.MOCK)
@@ -96,17 +93,28 @@
 
 def test_init_available():
     """Make sure that there is an __init__ that takes no args or kwargs"""
     model = caikit.core.ModuleBase()
     assert isinstance(model, caikit.core.ModuleBase)
 
 
-def test_load_not_implemented():
+def test_underscore_load_not_implemented():
     with pytest.raises(NotImplementedError):
-        caikit.core.ModuleBase.load()
+        caikit.core.ModuleBase._load(None)
+
+
+def test_load_delegates_to_underscore_load(good_model_path):
+    @caikit.core.modules.module(id="blah", name="dummy base", version="0.0.1")
+    class DummyFoo(caikit.core.ModuleBase):
+        @classmethod
+        def _load(cls, module_loader, **kwargs):
+            assert isinstance(module_loader, ModuleLoader)
+            return "foo"
+
+    assert DummyFoo.load(good_model_path) == "foo"
 
 
 def test_run_not_implemented(base_module_instance):
     with pytest.raises(NotImplementedError):
         base_module_instance.run()
 
 
@@ -325,17 +333,15 @@
     assert DummyBar.SUPPORTED_LOAD_BACKENDS[0] == backend_types.MOCK
 
 
 def test_override_load_supported_backend(reset_globals):
     """Test if the class can successfully define its own backends
     that it supports load from"""
 
-    @caikit.core.modules.module(
-        id=DUMMY_MODULE_ID, name="dummy base", version="0.0.1", task=SampleTask
-    )
+    @caikit.core.modules.module(id=DUMMY_MODULE_ID, name="dummy base", version="0.0.1")
     class DummyFoo(caikit.core.ModuleBase):
         pass
 
     class BazBackend(BackendBase):
         backend_type = "BAZ"
 
     class FooBackend(BackendBase):
@@ -363,17 +369,15 @@
 
     class FooBackend(BackendBase):
         backend_type = "FOO"
 
     backend_types.register_backend_type(BazBackend)
     backend_types.register_backend_type(FooBackend)
 
-    @caikit.core.modules.module(
-        id=DUMMY_MODULE_ID, name="dummy base", version="0.0.1", task=SampleTask
-    )
+    @caikit.core.modules.module(id=DUMMY_MODULE_ID, name="dummy base", version="0.0.1")
     class DummyLocal(caikit.core.ModuleBase):
         pass
 
     @caikit.core.modules.module(backend_type=backend_types.BAZ, base_module=DummyLocal)
     class DummyBaz(caikit.core.ModuleBase):
         pass
```

### Comparing `caikit-0.5.2/tests/core/modules/test_module_metadata.py` & `caikit-0.5.3/tests/core/modules/test_module_metadata.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/core/test_imports.py` & `caikit-0.5.3/tests/core/test_imports.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/core/test_model_manager.py` & `caikit-0.5.3/tests/core/test_model_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,17 +189,15 @@
 
 
 def setup_saved_model(mock_backend_class):
     """Fixture to create and cleanup a dummy loadable model"""
 
     backend_types.register_backend_type(LocalBackend)
 
-    @caikit.core.modules.module(
-        id=DUMMY_MODULE_ID, name="dummy base", version="0.0.1", task=SampleTask
-    )
+    @caikit.core.modules.module(id=DUMMY_MODULE_ID, name="dummy base", version="0.0.1")
     class DummyFoo(caikit.core.ModuleBase):
         @classmethod
         def load(cls, *args, **kwargs):
             return cls()
 
     # Register backend type
     backend_types.register_backend_type(mock_backend_class)
@@ -212,15 +210,15 @@
         def load(self, *args, **kwargs):
             return DummyBar()
 
     return DummyFoo, DummyBar
 
 
 @caikit.core.modules.module(
-    id="non-distributed", name="non distributed mod", version="0.0.1", task=SampleTask
+    id="non-distributed", name="non distributed mod", version="0.0.1"
 )
 class NonDistributedModule(caikit.core.ModuleBase):
     @classmethod
     def load(cls, *args, **kwargs):
         return cls()
 
     def save(self, model_path):
```

### Comparing `caikit-0.5.2/tests/core/test_no_write_permissions.py` & `caikit-0.5.3/tests/core/test_no_write_permissions.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/core/toolkit/test_compatibility.py` & `caikit-0.5.3/tests/core/toolkit/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/core/toolkit/test_error_handler.py` & `caikit-0.5.3/tests/core/toolkit/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/core/toolkit/test_fileio.py` & `caikit-0.5.3/tests/core/toolkit/test_fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/core/toolkit/test_quality_evaluation.py` & `caikit-0.5.3/tests/core/toolkit/test_quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/core/toolkit/test_serializers.py` & `caikit-0.5.3/tests/core/toolkit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/core/toolkit/test_wip_decorator.py` & `caikit-0.5.3/tests/core/toolkit/test_wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/data_model_helpers.py` & `caikit-0.5.3/tests/data_model_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/fixtures/config/config.yml` & `caikit-0.5.3/tests/fixtures/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/fixtures/data_stream_inputs/sample.txt` & `caikit-0.5.3/tests/fixtures/data_stream_inputs/sample.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/fixtures/dummy_module.zip` & `caikit-0.5.3/tests/fixtures/dummy_module.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/fixtures/dummy_module/config.yml` & `caikit-0.5.3/tests/fixtures/dummy_module/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/fixtures/dummy_module_singleton/config.yml` & `caikit-0.5.3/tests/fixtures/dummy_module_singleton/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/fixtures/fixtures.py` & `caikit-0.5.3/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/fixtures/invalid.zip` & `caikit-0.5.3/tests/fixtures/invalid.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/fixtures/linux.txt` & `caikit-0.5.3/tests/fixtures/linux.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/fixtures/primitive_party.proto` & `caikit-0.5.3/tests/fixtures/primitive_party.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/fixtures/protobufs/caikit_runtime_pb2.py` & `caikit-0.5.3/tests/fixtures/protobufs/caikit_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py` & `caikit-0.5.3/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/fixtures/protobufs/caikit_runtime_train_pb2.py` & `caikit-0.5.3/tests/fixtures/protobufs/caikit_runtime_train_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py` & `caikit-0.5.3/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/fixtures/protobufs/primitive_party_pb2.py` & `caikit-0.5.3/tests/fixtures/protobufs/primitive_party_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/fixtures/sample_lib/data_model/sample.py` & `caikit-0.5.3/tests/fixtures/sample_lib/data_model/sample.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/fixtures/sample_lib/modules/other_task/other_implementation.py` & `caikit-0.5.3/tests/fixtures/sample_lib/modules/other_task/other_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/fixtures/sample_lib/modules/sample_task/composite_module.py` & `caikit-0.5.3/tests/fixtures/sample_lib/modules/sample_task/composite_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/fixtures/sample_lib/modules/sample_task/inner_module.py` & `caikit-0.5.3/tests/fixtures/sample_lib/modules/sample_task/inner_module.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """
 A hypothetical inner module that transforms some output type rather than taking domain input
 """
 # Local
-from ...data_model.sample import SampleOutputType, SampleTask
+from ...data_model.sample import SampleOutputType
 import caikit.core
 
 
-@caikit.core.module(
-    "00110203-baad-beef-0809-0a0b02dd0e0f", "SampleModule", "0.0.1", SampleTask
-)
+@caikit.core.module("00110203-baad-beef-0809-0a0b02dd0e0f", "SampleModule", "0.0.1")
 class InnerModule(caikit.core.ModuleBase):
     def __init__(self, batch_size=64, learning_rate=0.0015):
         super().__init__()
         self.batch_size = batch_size
         self.learning_rate = learning_rate
 
     def run(self, some_input: SampleOutputType) -> SampleOutputType:
```

### Comparing `caikit-0.5.2/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py` & `caikit-0.5.3/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py` & `caikit-0.5.3/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """
 A module meant to flex a bit of the protobufs primitive support
 """
 # Standard
 from typing import List
 
 # Local
-from ...data_model.sample import SampleOutputType, SampleTask
+from ...data_model.sample import SampleOutputType
 from caikit.core.modules import ModuleSaver
 import caikit.core
 
 
-@caikit.core.module(
-    "00112233-0405-0607-0809-0a0b02dd0e0f", "SampleModule", "0.0.1", SampleTask
-)
+@caikit.core.module("00112233-0405-0607-0809-0a0b02dd0e0f", "SampleModule", "0.0.1")
 class SamplePrimitiveModule(caikit.core.ModuleBase):
     def __init__(self):
         super().__init__()
 
     @classmethod
     def load(cls, model_path, **kwargs):
         return cls()
```

### Comparing `caikit-0.5.2/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py` & `caikit-0.5.3/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/generated/__init__.py` & `caikit-0.5.3/tests/runtime/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/metrics/__init__.py` & `caikit-0.5.3/tests/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/metrics/test_rpc_meter.py` & `caikit-0.5.3/tests/runtime/metrics/test_rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/model_management/__init__.py` & `caikit-0.5.3/tests/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/model_management/test_batcher.py` & `caikit-0.5.3/tests/runtime/model_management/test_batcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import pytest
 
 # First Party
 import alog
 
 # Local
 from caikit.runtime.model_management.batcher import Batcher
-from sample_lib.data_model import SampleOutputType, SampleTask
+from sample_lib.data_model import SampleOutputType
 import caikit.core
 
 ## Helpers #####################################################################
 
 log = alog.use_channel("TEST")
 
 DUMMY_MODEL = os.path.realpath(
@@ -44,15 +44,15 @@
         "models",
         "foo_archive.zip",
     )
 )
 
 
 @caikit.core.module(
-    "7464f684-58e3-4e99-9a58-1c5bc085472b", "slow sample module", "0.0.1", SampleTask
+    "7464f684-58e3-4e99-9a58-1c5bc085472b", "slow sample module", "0.0.1"
 )
 class SlowSampleModule(caikit.core.ModuleBase):
     """This module is just a wrapper around another module that will inject a
     sleep
     """
 
     def __init__(self, model, sleep_time_s=0.1):
@@ -72,15 +72,14 @@
         return self._model.run_batch(*args, **kwargs)
 
 
 @caikit.core.module(
     "19b126aa-b55b-4349-94f1-d676f3e12c9b",
     "Really silly bunch of bobs!",
     "0.0.1",
-    SampleTask,
 )
 class StubModule(caikit.core.ModuleBase):
     # NOTE: The initial implementation had "num_bobs" which expected an int.
     #   This led to the discovery of the fact that lists of ints are not
     #   considered "expandable iterables" in the default run_batch impl.
     def __init__(self):
         super().__init__()
```

### Comparing `caikit-0.5.2/tests/runtime/model_management/test_model_loader.py` & `caikit-0.5.3/tests/runtime/model_management/test_model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/model_management/test_model_manager.py` & `caikit-0.5.3/tests/runtime/model_management/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/model_management/test_model_sizer.py` & `caikit-0.5.3/tests/runtime/model_management/test_model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/model_management/test_training_manager.py` & `caikit-0.5.3/tests/runtime/model_management/test_training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.5.3/tests/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/service_generation/signature_parsing/test_docstrings.py` & `caikit-0.5.3/tests/core/signature_parsing/test_docstrings.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,25 +17,23 @@
 """
 # Standard
 from typing import List, Optional, Union
 from unittest.mock import patch
 
 # Third Party
 from docstring_parser import ParseError
-import pytest
 
 # Local
-from caikit.runtime.service_generation.signature_parsing.docstrings import (
+from caikit.core.signature_parsing.docstrings import (
     _extract_nested_type,
     _get_docstring_type,
     get_arg_type,
     get_return_type,
     is_optional,
 )
-from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 from sample_lib.data_model import SampleInputType
 import caikit
 import sample_lib
 
 
 def test_get_docstring_type():
     # TODO: fun edge case where producer word in description is found in types
@@ -102,27 +100,25 @@
             some_input: I repeat myself
 
         Returns:
             None
         """
         pass
 
-    assert is_optional(_fn, "some_input") == True
+    assert is_optional(_fn, "some_input") is True
 
-    # test if docstring_parser.parse throws an exception, we throw an exception
+    # test if docstring_parser.parse throws an exception, we return False
     with patch("docstring_parser.parse", side_effect=ParseError("mocked error")):
-        with pytest.raises(CaikitRuntimeException) as e:
-            is_optional(_fn, "some_input")
-        assert "ParseError when parsing docstring for function: _fn" in e.value.message
+        assert is_optional(_fn, "some_input") is False
 
     def _fn(input):
         pass
 
     # test is_optional works on empty docstring
-    assert is_optional(_fn, "input") == False
+    assert is_optional(_fn, "input") is False
 
 
 def test_get_arg_type_works_on_corner_cases_docstrings():
     """
     Test that get_arg_type works on different corner cases of docstrings
     """
     # test docstring with multiple params of the same name still works, but
@@ -139,19 +135,17 @@
         Returns:
             None
         """
         pass
 
     assert get_arg_type(_fn, "some_input") == int
 
-    # test if docstring_parser.parse throws an exception, we throw an exception
+    # test if docstring_parser.parse throws an exception, we return None
     with patch("docstring_parser.parse", side_effect=ParseError("mocked error")):
-        with pytest.raises(CaikitRuntimeException) as e:
-            get_arg_type(_fn, "some_input")
-        assert "ParseError when parsing docstring for function: _fn" in e.value.message
+        assert get_arg_type(_fn, "some_input") is None
 
     # test get_arg_type works on empty docstring
     def _fn_no_docstring(input):
         pass
 
     assert get_arg_type(_fn_no_docstring, "input") == None
 
@@ -159,12 +153,10 @@
 def test_get_return_type_corner_case_with_exception():
     def _fn():
         pass
 
     # test get_return_type works on empty docstring
     assert get_return_type(_fn) == None
 
-    # test if docstring_parser.parse throws an exception, we throw an exception
+    # test if docstring_parser.parse throws an exception, we swallow and return none
     with patch("docstring_parser.parse", side_effect=ParseError("mocked error")):
-        with pytest.raises(CaikitRuntimeException) as e:
-            get_return_type(_fn)
-        assert "ParseError when parsing docstring for function: _fn" in e.value.message
+        assert get_return_type(_fn) is None
```

### Comparing `caikit-0.5.2/tests/runtime/service_generation/signature_parsing/test_parsers.py` & `caikit-0.5.3/tests/core/signature_parsing/test_parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,17 @@
 # Standard
 from typing import List, Optional
 from unittest.mock import patch
 import inspect
 
 # Third Party
 from docstring_parser import ParseError
-import pytest
 
 # Local
-from caikit.runtime.service_generation.signature_parsing import docstrings
-from caikit.runtime.service_generation.signature_parsing.parsers import (
+from caikit.core.signature_parsing.parsers import (
     _get_dm_type_from_name,
     _snake_to_camel,
     get_args_with_defaults,
     get_argument_types,
     get_output_type_name,
 )
 import caikit.core
```

### Comparing `caikit-0.5.2/tests/runtime/service_generation/test_create_service.py` & `caikit-0.5.3/tests/runtime/service_generation/test_create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/service_generation/test_data_stream_source.py` & `caikit-0.5.3/tests/runtime/service_generation/test_data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/service_generation/test_primitives.py` & `caikit-0.5.3/tests/runtime/service_generation/test_primitives.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/service_generation/test_rpcs.py` & `caikit-0.5.3/tests/runtime/service_generation/test_rpcs.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,37 +15,35 @@
 """Tests for the rpc objects that hold our in-memory representation of
 what an RPC for a service looks like"""
 # Standard
 import uuid
 
 # Local
 from caikit.core import ModuleBase, TaskBase
+from caikit.core.signature_parsing import CaikitMethodSignature
 from caikit.runtime.service_generation.rpcs import TaskPredictRPC
-from caikit.runtime.service_generation.signature_parsing import (
-    CaikitCoreModuleMethodSignature,
-)
 from sample_lib.data_model import SampleOutputType, SampleTask
 import caikit.core
 
 
 def test_task_inference_rpc_with_all_optional_params():
     @caikit.core.task(
         required_parameters={"str_val": str}, output_type=SampleOutputType
     )
     class TestTask(TaskBase):
         pass
 
     @caikit.core.module(
-        id=str(uuid.uuid4()), name="testest", version="9.9.9", task=SampleTask
+        id=str(uuid.uuid4()), name="testest", version="9.9.9", task=TestTask
     )
     class TestModule(ModuleBase):
-        def run(self, str_val="I have a default"):
+        def run(self, str_val="I have a default") -> SampleOutputType:
             pass
 
     rpc = TaskPredictRPC(
         task=("foo", "bar"),
-        method_signatures=[CaikitCoreModuleMethodSignature(TestModule, "run")],
+        method_signatures=[CaikitMethodSignature(TestModule, "run")],
         primitive_data_model_types=[],
     )
 
     data_model = rpc.create_request_data_model(package_name="blah")
     assert data_model is not None
```

### Comparing `caikit-0.5.2/tests/runtime/service_generation/test_type_helpers.py` & `caikit-0.5.3/tests/runtime/service_generation/test_type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/servicers/__init__.py` & `caikit-0.5.3/tests/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/servicers/test_global_predict_servicer_impl.py` & `caikit-0.5.3/tests/runtime/servicers/test_global_predict_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/servicers/test_global_train_servicer_impl.py` & `caikit-0.5.3/tests/runtime/servicers/test_global_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/servicers/test_model_runtime_servicer_impl.py` & `caikit-0.5.3/tests/runtime/servicers/test_model_runtime_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/servicers/test_model_train_servicer_impl.py` & `caikit-0.5.3/tests/runtime/servicers/test_model_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/servicers/test_training_management_servicer.py` & `caikit-0.5.3/tests/runtime/servicers/test_training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/test_grpc_server.py` & `caikit-0.5.3/tests/runtime/test_grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/test_service_factory.py` & `caikit-0.5.3/tests/runtime/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/utils/__init__.py` & `caikit-0.5.3/tests/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/utils/test_import_util.py` & `caikit-0.5.3/tests/runtime/utils/test_import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/utils/test_servicer_util.py` & `caikit-0.5.3/tests/runtime/utils/test_servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/work_management/test_abortable_action.py` & `caikit-0.5.3/tests/runtime/work_management/test_abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/work_management/test_call_aborter.py` & `caikit-0.5.3/tests/runtime/work_management/test_call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tests/runtime/work_management/test_destroyable_thread.py` & `caikit-0.5.3/tests/runtime/work_management/test_destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/tox.ini` & `caikit-0.5.3/tox.ini`

 * *Files identical despite different names*

### Comparing `caikit-0.5.2/PKG-INFO` & `caikit-0.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caikit
-Version: 0.5.2
+Version: 0.5.3
 Summary: AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: alchemy-config>=1.1.1,<2.0.0
 Requires-Dist: alchemy-logging>=1.0.4,<2.0.0
 Requires-Dist: anytree>=2.7.0,<3.0
@@ -63,11 +63,15 @@
   - They take trained models, deploy them, and then infer the models in applications through APIs provided by Caikit
   - Examples of operators are cloud and embedded application developers whose applications need analysis of unstructured data
 
 ## AI Model Operator Example
 
 Check out the [Text Sentiment example](examples/text-sentiment/) to understand how to load and infer a model using Caikit.
 
+## Contributing
+
+Check out our [contributing](CONTRIBUTING.md) guide to learn how to contribute to Caikit.
+
 ## Code of conduct
 
 Participation in the Caikit community is governed by the [Code of Conduct](CODE-OF-CONDUCT.md).
```

