# Comparing `tmp/humanloop-0.4.2.tar.gz` & `tmp/humanloop-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "humanloop-0.4.2.tar", max compression
+gzip compressed data, was "humanloop-0.4.3.tar", max compression
```

## Comparing `humanloop-0.4.2.tar` & `humanloop-0.4.3.tar`

### file list

```diff
@@ -1,371 +1,401 @@
--rw-r--r--   0        0        0     1081 2023-05-18 18:37:52.344259 humanloop-0.4.2/LICENSE
--rw-r--r--   0        0        0     8475 2023-05-18 18:37:52.385459 humanloop-0.4.2/README.md
--rw-r--r--   0        0        0     1059 2023-05-18 18:37:52.273096 humanloop-0.4.2/humanloop/__init__.py
--rw-r--r--   0        0        0    73009 2023-05-18 18:37:52.273303 humanloop-0.4.2/humanloop/api_client.py
--rw-r--r--   0        0        0      663 2023-05-18 18:37:52.273468 humanloop-0.4.2/humanloop/api_response.py
--rw-r--r--   0        0        0      214 2023-05-18 18:37:52.273611 humanloop-0.4.2/humanloop/apis/__init__.py
--rw-r--r--   0        0        0     5316 2023-05-18 18:37:52.273731 humanloop-0.4.2/humanloop/apis/path_to_api.py
--rw-r--r--   0        0        0      236 2023-05-18 18:37:52.273869 humanloop-0.4.2/humanloop/apis/paths/__init__.py
--rw-r--r--   0        0        0       88 2023-05-18 18:37:52.273993 humanloop-0.4.2/humanloop/apis/paths/apps.py
--rw-r--r--   0        0        0       93 2023-05-18 18:37:52.274106 humanloop-0.4.2/humanloop/apis/paths/apps_id.py
--rw-r--r--   0        0        0      110 2023-05-18 18:37:52.274220 humanloop-0.4.2/humanloop/apis/paths/apps_id_sessions.py
--rw-r--r--   0        0        0       91 2023-05-18 18:37:52.274347 humanloop-0.4.2/humanloop/apis/paths/chat.py
--rw-r--r--   0        0        0      108 2023-05-18 18:37:52.274474 humanloop-0.4.2/humanloop/apis/paths/chat_deployed.py
--rw-r--r--   0        0        0      112 2023-05-18 18:37:52.274623 humanloop-0.4.2/humanloop/apis/paths/chat_experiment.py
--rw-r--r--   0        0        0      115 2023-05-18 18:37:52.274753 humanloop-0.4.2/humanloop/apis/paths/chat_model_config.py
--rw-r--r--   0        0        0      103 2023-05-18 18:37:52.274880 humanloop-0.4.2/humanloop/apis/paths/completion.py
--rw-r--r--   0        0        0      120 2023-05-18 18:37:52.275007 humanloop-0.4.2/humanloop/apis/paths/completion_deployed.py
--rw-r--r--   0        0        0      124 2023-05-18 18:37:52.275142 humanloop-0.4.2/humanloop/apis/paths/completion_experiment.py
--rw-r--r--   0        0        0      127 2023-05-18 18:37:52.275273 humanloop-0.4.2/humanloop/apis/paths/completion_model_config.py
--rw-r--r--   0        0        0      226 2023-05-18 18:37:52.275398 humanloop-0.4.2/humanloop/apis/paths/experiments_experiment_id.py
--rw-r--r--   0        0        0      152 2023-05-18 18:37:52.275530 humanloop-0.4.2/humanloop/apis/paths/experiments_experiment_id_model_config.py
--rw-r--r--   0        0        0       99 2023-05-18 18:37:52.275655 humanloop-0.4.2/humanloop/apis/paths/feedback.py
--rw-r--r--   0        0        0       91 2023-05-18 18:37:52.275774 humanloop-0.4.2/humanloop/apis/paths/logs.py
--rw-r--r--   0        0        0      108 2023-05-18 18:37:52.275886 humanloop-0.4.2/humanloop/apis/paths/model_configs.py
--rw-r--r--   0        0        0      110 2023-05-18 18:37:52.275991 humanloop-0.4.2/humanloop/apis/paths/model_configs_id.py
--rw-r--r--   0        0        0      165 2023-05-18 18:37:52.276084 humanloop-0.4.2/humanloop/apis/paths/projects.py
--rw-r--r--   0        0        0      176 2023-05-18 18:37:52.276180 humanloop-0.4.2/humanloop/apis/paths/projects_id.py
--rw-r--r--   0        0        0      144 2023-05-18 18:37:52.276273 humanloop-0.4.2/humanloop/apis/paths/projects_id_active_experiment.py
--rw-r--r--   0        0        0      147 2023-05-18 18:37:52.276375 humanloop-0.4.2/humanloop/apis/paths/projects_id_active_model_config.py
--rw-r--r--   0        0        0      117 2023-05-18 18:37:52.276497 humanloop-0.4.2/humanloop/apis/paths/projects_id_export.py
--rw-r--r--   0        0        0      135 2023-05-18 18:37:52.276609 humanloop-0.4.2/humanloop/apis/paths/projects_id_feedback_types.py
--rw-r--r--   0        0        0      125 2023-05-18 18:37:52.276705 humanloop-0.4.2/humanloop/apis/paths/projects_id_model_config.py
--rw-r--r--   0        0        0      127 2023-05-18 18:37:52.276928 humanloop-0.4.2/humanloop/apis/paths/projects_id_model_configs.py
--rw-r--r--   0        0        0      231 2023-05-18 18:37:52.277061 humanloop-0.4.2/humanloop/apis/paths/projects_project_id_experiments.py
--rw-r--r--   0        0        0       99 2023-05-18 18:37:52.277153 humanloop-0.4.2/humanloop/apis/paths/sessions.py
--rw-r--r--   0        0        0      101 2023-05-18 18:37:52.277248 humanloop-0.4.2/humanloop/apis/paths/sessions_id.py
--rw-r--r--   0        0        0      114 2023-05-18 18:37:52.277346 humanloop-0.4.2/humanloop/apis/paths/sessions_id_events.py
--rw-r--r--   0        0        0     1642 2023-05-18 18:37:52.277436 humanloop-0.4.2/humanloop/apis/tag_to_api.py
--rw-r--r--   0        0        0      568 2023-05-18 18:37:52.277536 humanloop-0.4.2/humanloop/apis/tags/__init__.py
--rw-r--r--   0        0        0      839 2023-05-18 18:37:52.277629 humanloop-0.4.2/humanloop/apis/tags/apps_api.py
--rw-r--r--   0        0        0     1006 2023-05-18 18:37:52.277719 humanloop-0.4.2/humanloop/apis/tags/chats_api.py
--rw-r--r--   0        0        0     1020 2023-05-18 18:37:52.277806 humanloop-0.4.2/humanloop/apis/tags/completions_api.py
--rw-r--r--   0        0        0     1091 2023-05-18 18:37:52.277894 humanloop-0.4.2/humanloop/apis/tags/experiments_api.py
--rw-r--r--   0        0        0      721 2023-05-18 18:37:52.278008 humanloop-0.4.2/humanloop/apis/tags/feedback_api.py
--rw-r--r--   0        0        0      707 2023-05-18 18:37:52.278109 humanloop-0.4.2/humanloop/apis/tags/logs_api.py
--rw-r--r--   0        0        0      803 2023-05-18 18:37:52.278197 humanloop-0.4.2/humanloop/apis/tags/model_configurations_api.py
--rw-r--r--   0        0        0     1519 2023-05-18 18:37:52.278286 humanloop-0.4.2/humanloop/apis/tags/projects_api.py
--rw-r--r--   0        0        0      854 2023-05-18 18:37:52.278383 humanloop-0.4.2/humanloop/apis/tags/sessions_api.py
--rw-r--r--   0        0        0    27541 2023-05-18 18:37:52.278521 humanloop-0.4.2/humanloop/client.py
--rw-r--r--   0        0        0    27541 2023-05-18 18:37:52.278730 humanloop-0.4.2/humanloop/client.pyi
--rw-r--r--   0        0        0     7186 2023-05-18 09:14:14.289106 humanloop-0.4.2/humanloop/client_custom.py
--rw-r--r--   0        0        0    18674 2023-05-18 18:37:52.279132 humanloop-0.4.2/humanloop/configuration.py
--rw-r--r--   0        0        0     7678 2023-05-18 18:37:52.279297 humanloop-0.4.2/humanloop/exceptions.py
--rw-r--r--   0        0        0     2274 2023-05-18 18:37:52.279485 humanloop-0.4.2/humanloop/exceptions_base.py
--rw-r--r--   0        0        0      343 2023-05-18 18:37:52.279715 humanloop-0.4.2/humanloop/model/__init__.py
--rw-r--r--   0        0        0     6379 2023-05-18 18:37:52.279879 humanloop-0.4.2/humanloop/model/base_metric_response.py
--rw-r--r--   0        0        0     6379 2023-05-18 18:37:52.280044 humanloop-0.4.2/humanloop/model/base_metric_response.pyi
--rw-r--r--   0        0        0     5150 2023-05-18 18:37:52.280259 humanloop-0.4.2/humanloop/model/categorical_feedback_label.py
--rw-r--r--   0        0        0     5150 2023-05-18 18:37:52.280394 humanloop-0.4.2/humanloop/model/categorical_feedback_label.pyi
--rw-r--r--   0        0        0     8957 2023-05-18 18:37:52.280592 humanloop-0.4.2/humanloop/model/chat_data_response.py
--rw-r--r--   0        0        0     8957 2023-05-18 18:37:52.280857 humanloop-0.4.2/humanloop/model/chat_data_response.pyi
--rw-r--r--   0        0        0     9998 2023-05-18 18:37:52.281065 humanloop-0.4.2/humanloop/model/chat_deployed_request.py
--rw-r--r--   0        0        0     9998 2023-05-18 18:37:52.281331 humanloop-0.4.2/humanloop/model/chat_deployed_request.pyi
--rw-r--r--   0        0        0    10659 2023-05-18 18:37:52.281521 humanloop-0.4.2/humanloop/model/chat_experiment_request.py
--rw-r--r--   0        0        0    10659 2023-05-18 18:37:52.281774 humanloop-0.4.2/humanloop/model/chat_experiment_request.pyi
--rw-r--r--   0        0        0     3702 2023-05-18 18:37:52.281951 humanloop-0.4.2/humanloop/model/chat_message.py
--rw-r--r--   0        0        0     3702 2023-05-18 18:37:52.282114 humanloop-0.4.2/humanloop/model/chat_message.pyi
--rw-r--r--   0        0        0    10693 2023-05-18 18:37:52.282258 humanloop-0.4.2/humanloop/model/chat_model_config_request.py
--rw-r--r--   0        0        0    10693 2023-05-18 18:37:52.282462 humanloop-0.4.2/humanloop/model/chat_model_config_request.pyi
--rw-r--r--   0        0        0    12556 2023-05-18 18:37:52.282651 humanloop-0.4.2/humanloop/model/chat_request.py
--rw-r--r--   0        0        0    12556 2023-05-18 18:37:52.282827 humanloop-0.4.2/humanloop/model/chat_request.pyi
--rw-r--r--   0        0        0    11076 2023-05-18 18:37:52.283008 humanloop-0.4.2/humanloop/model/chat_response.py
--rw-r--r--   0        0        0    11076 2023-05-18 18:37:52.283281 humanloop-0.4.2/humanloop/model/chat_response.pyi
--rw-r--r--   0        0        0     1446 2023-05-18 18:37:52.283421 humanloop-0.4.2/humanloop/model/chat_role.py
--rw-r--r--   0        0        0     1285 2023-05-18 18:37:52.283556 humanloop-0.4.2/humanloop/model/chat_role.pyi
--rw-r--r--   0        0        0     9674 2023-05-18 18:37:52.283650 humanloop-0.4.2/humanloop/model/completion_deployed_request.py
--rw-r--r--   0        0        0     9674 2023-05-18 18:37:52.283821 humanloop-0.4.2/humanloop/model/completion_deployed_request.pyi
--rw-r--r--   0        0        0    10340 2023-05-18 18:37:52.284085 humanloop-0.4.2/humanloop/model/completion_experiment_request.py
--rw-r--r--   0        0        0    10340 2023-05-18 18:37:52.284275 humanloop-0.4.2/humanloop/model/completion_experiment_request.pyi
--rw-r--r--   0        0        0    10376 2023-05-18 18:37:52.284451 humanloop-0.4.2/humanloop/model/completion_model_config_request.py
--rw-r--r--   0        0        0    10376 2023-05-18 18:37:52.284619 humanloop-0.4.2/humanloop/model/completion_model_config_request.pyi
--rw-r--r--   0        0        0    12258 2023-05-18 18:37:52.284799 humanloop-0.4.2/humanloop/model/completion_request.py
--rw-r--r--   0        0        0    12258 2023-05-18 18:37:52.284971 humanloop-0.4.2/humanloop/model/completion_request.pyi
--rw-r--r--   0        0        0    11017 2023-05-18 18:37:52.285109 humanloop-0.4.2/humanloop/model/completion_response.py
--rw-r--r--   0        0        0    11017 2023-05-18 18:37:52.285287 humanloop-0.4.2/humanloop/model/completion_response.pyi
--rw-r--r--   0        0        0     6280 2023-05-18 18:37:52.285426 humanloop-0.4.2/humanloop/model/create_experiment_request.py
--rw-r--r--   0        0        0     6280 2023-05-18 18:37:52.285563 humanloop-0.4.2/humanloop/model/create_experiment_request.pyi
--rw-r--r--   0        0        0     3199 2023-05-18 18:37:52.285682 humanloop-0.4.2/humanloop/model/create_log_response.py
--rw-r--r--   0        0        0     3199 2023-05-18 18:37:52.285818 humanloop-0.4.2/humanloop/model/create_log_response.pyi
--rw-r--r--   0        0        0     4266 2023-05-18 18:37:52.285931 humanloop-0.4.2/humanloop/model/create_project_request.py
--rw-r--r--   0        0        0     4266 2023-05-18 18:37:52.286065 humanloop-0.4.2/humanloop/model/create_project_request.pyi
--rw-r--r--   0        0        0     2649 2023-05-18 18:37:52.286170 humanloop-0.4.2/humanloop/model/create_session_request.py
--rw-r--r--   0        0        0     2649 2023-05-18 18:37:52.286281 humanloop-0.4.2/humanloop/model/create_session_request.pyi
--rw-r--r--   0        0        0     7455 2023-05-18 18:37:52.286429 humanloop-0.4.2/humanloop/model/data_response.py
--rw-r--r--   0        0        0     7455 2023-05-18 18:37:52.286533 humanloop-0.4.2/humanloop/model/data_response.pyi
--rw-r--r--   0        0        0     9235 2023-05-18 18:37:52.286654 humanloop-0.4.2/humanloop/model/experiment_model_config_response.py
--rw-r--r--   0        0        0     9235 2023-05-18 18:37:52.286842 humanloop-0.4.2/humanloop/model/experiment_model_config_response.pyi
--rw-r--r--   0        0        0    12947 2023-05-18 18:37:52.286970 humanloop-0.4.2/humanloop/model/experiment_response.py
--rw-r--r--   0        0        0    12947 2023-05-18 18:37:52.287113 humanloop-0.4.2/humanloop/model/experiment_response.pyi
--rw-r--r--   0        0        0     1376 2023-05-18 18:37:52.287287 humanloop-0.4.2/humanloop/model/experiment_status.py
--rw-r--r--   0        0        0     1229 2023-05-18 18:37:52.287392 humanloop-0.4.2/humanloop/model/experiment_status.pyi
--rw-r--r--   0        0        0     1685 2023-05-18 18:37:52.287512 humanloop-0.4.2/humanloop/model/experiments_list_response.py
--rw-r--r--   0        0        0     1685 2023-05-18 18:37:52.287649 humanloop-0.4.2/humanloop/model/experiments_list_response.pyi
--rw-r--r--   0        0        0     6681 2023-05-18 18:37:52.287759 humanloop-0.4.2/humanloop/model/feedback.py
--rw-r--r--   0        0        0     6681 2023-05-18 18:37:52.287853 humanloop-0.4.2/humanloop/model/feedback.pyi
--rw-r--r--   0        0        0     1463 2023-05-18 18:37:52.287952 humanloop-0.4.2/humanloop/model/feedback_class.py
--rw-r--r--   0        0        0     1296 2023-05-18 18:37:52.288048 humanloop-0.4.2/humanloop/model/feedback_class.pyi
--rw-r--r--   0        0        0     3334 2023-05-18 18:37:52.288146 humanloop-0.4.2/humanloop/model/feedback_label_request.py
--rw-r--r--   0        0        0     3334 2023-05-18 18:37:52.288237 humanloop-0.4.2/humanloop/model/feedback_label_request.pyi
--rw-r--r--   0        0        0     7189 2023-05-18 18:37:52.288325 humanloop-0.4.2/humanloop/model/feedback_request.py
--rw-r--r--   0        0        0     7189 2023-05-18 18:37:52.288442 humanloop-0.4.2/humanloop/model/feedback_request.pyi
--rw-r--r--   0        0        0     7141 2023-05-18 18:37:52.288579 humanloop-0.4.2/humanloop/model/feedback_response.py
--rw-r--r--   0        0        0     7141 2023-05-18 18:37:52.288708 humanloop-0.4.2/humanloop/model/feedback_response.pyi
--rw-r--r--   0        0        0     3200 2023-05-18 18:37:52.288839 humanloop-0.4.2/humanloop/model/feedback_submit_request.py
--rw-r--r--   0        0        0     3200 2023-05-18 18:37:52.288999 humanloop-0.4.2/humanloop/model/feedback_submit_request.pyi
--rw-r--r--   0        0        0     3210 2023-05-18 18:37:52.289151 humanloop-0.4.2/humanloop/model/feedback_submit_response.py
--rw-r--r--   0        0        0     3210 2023-05-18 18:37:52.289295 humanloop-0.4.2/humanloop/model/feedback_submit_response.pyi
--rw-r--r--   0        0        0     1690 2023-05-18 18:37:52.289419 humanloop-0.4.2/humanloop/model/feedback_type.py
--rw-r--r--   0        0        0     1459 2023-05-18 18:37:52.289600 humanloop-0.4.2/humanloop/model/feedback_type.pyi
--rw-r--r--   0        0        0     6161 2023-05-18 18:37:52.289738 humanloop-0.4.2/humanloop/model/feedback_type_model.py
--rw-r--r--   0        0        0     6161 2023-05-18 18:37:52.289868 humanloop-0.4.2/humanloop/model/feedback_type_model.pyi
--rw-r--r--   0        0        0     6289 2023-05-18 18:37:52.290044 humanloop-0.4.2/humanloop/model/feedback_type_request.py
--rw-r--r--   0        0        0     6289 2023-05-18 18:37:52.290198 humanloop-0.4.2/humanloop/model/feedback_type_request.pyi
--rw-r--r--   0        0        0     1659 2023-05-18 18:37:52.290320 humanloop-0.4.2/humanloop/model/feedback_types.py
--rw-r--r--   0        0        0     1659 2023-05-18 18:37:52.290491 humanloop-0.4.2/humanloop/model/feedback_types.pyi
--rw-r--r--   0        0        0    24518 2023-05-18 18:37:52.291086 humanloop-0.4.2/humanloop/model/get_model_config_response.py
--rw-r--r--   0        0        0    24518 2023-05-18 18:37:52.291303 humanloop-0.4.2/humanloop/model/get_model_config_response.pyi
--rw-r--r--   0        0        0     3611 2023-05-18 18:37:52.291441 humanloop-0.4.2/humanloop/model/http_validation_error.py
--rw-r--r--   0        0        0     3611 2023-05-18 18:37:52.291577 humanloop-0.4.2/humanloop/model/http_validation_error.pyi
--rw-r--r--   0        0        0     1667 2023-05-18 18:37:52.291710 humanloop-0.4.2/humanloop/model/label_sentiment.py
--rw-r--r--   0        0        0     1468 2023-05-18 18:37:52.291814 humanloop-0.4.2/humanloop/model/label_sentiment.pyi
--rw-r--r--   0        0        0     3156 2023-05-18 18:37:52.291921 humanloop-0.4.2/humanloop/model/log_datapoint_request.py
--rw-r--r--   0        0        0     3156 2023-05-18 18:37:52.292019 humanloop-0.4.2/humanloop/model/log_datapoint_request.pyi
--rw-r--r--   0        0        0    14677 2023-05-18 18:37:52.292114 humanloop-0.4.2/humanloop/model/log_request.py
--rw-r--r--   0        0        0    14677 2023-05-18 18:37:52.292234 humanloop-0.4.2/humanloop/model/log_request.pyi
--rw-r--r--   0        0        0    18636 2023-05-18 18:37:52.292349 humanloop-0.4.2/humanloop/model/log_response.py
--rw-r--r--   0        0        0    18636 2023-05-18 18:37:52.292504 humanloop-0.4.2/humanloop/model/log_response.pyi
--rw-r--r--   0        0        0     3205 2023-05-18 18:37:52.292663 humanloop-0.4.2/humanloop/model/logs_log_response.py
--rw-r--r--   0        0        0     3205 2023-05-18 18:37:52.292764 humanloop-0.4.2/humanloop/model/logs_log_response.pyi
--rw-r--r--   0        0        0    16246 2023-05-18 18:37:52.292923 humanloop-0.4.2/humanloop/model/model_config_chat_request.py
--rw-r--r--   0        0        0    16246 2023-05-18 18:37:52.293106 humanloop-0.4.2/humanloop/model/model_config_chat_request.pyi
--rw-r--r--   0        0        0    15386 2023-05-18 18:37:52.293266 humanloop-0.4.2/humanloop/model/model_config_completion_request.py
--rw-r--r--   0        0        0    15386 2023-05-18 18:37:52.293408 humanloop-0.4.2/humanloop/model/model_config_completion_request.pyi
--rw-r--r--   0        0        0     1460 2023-05-18 18:37:52.293527 humanloop-0.4.2/humanloop/model/model_endpoints.py
--rw-r--r--   0        0        0     1305 2023-05-18 18:37:52.293659 humanloop-0.4.2/humanloop/model/model_endpoints.pyi
--rw-r--r--   0        0        0     1695 2023-05-18 18:37:52.293782 humanloop-0.4.2/humanloop/model/model_providers.py
--rw-r--r--   0        0        0     1468 2023-05-18 18:37:52.293927 humanloop-0.4.2/humanloop/model/model_providers.pyi
--rw-r--r--   0        0        0     5144 2023-05-18 18:37:52.294130 humanloop-0.4.2/humanloop/model/paginated_data_log_response.py
--rw-r--r--   0        0        0     5144 2023-05-18 18:37:52.294235 humanloop-0.4.2/humanloop/model/paginated_data_log_response.pyi
--rw-r--r--   0        0        0     5180 2023-05-18 18:37:52.294383 humanloop-0.4.2/humanloop/model/paginated_data_project_response.py
--rw-r--r--   0        0        0     5180 2023-05-18 18:37:52.294500 humanloop-0.4.2/humanloop/model/paginated_data_project_response.pyi
--rw-r--r--   0        0        0     3143 2023-05-18 18:37:52.294600 humanloop-0.4.2/humanloop/model/positive_label.py
--rw-r--r--   0        0        0     3143 2023-05-18 18:37:52.294746 humanloop-0.4.2/humanloop/model/positive_label.pyi
--rw-r--r--   0        0        0    18363 2023-05-18 18:37:52.294902 humanloop-0.4.2/humanloop/model/project_model_config_request.py
--rw-r--r--   0        0        0    18363 2023-05-18 18:37:52.295090 humanloop-0.4.2/humanloop/model/project_model_config_request.pyi
--rw-r--r--   0        0        0    13460 2023-05-18 18:37:52.295249 humanloop-0.4.2/humanloop/model/project_response.py
--rw-r--r--   0        0        0    13460 2023-05-18 18:37:52.295421 humanloop-0.4.2/humanloop/model/project_response.pyi
--rw-r--r--   0        0        0     1471 2023-05-18 18:37:52.295544 humanloop-0.4.2/humanloop/model/project_sort_by.py
--rw-r--r--   0        0        0     1300 2023-05-18 18:37:52.295657 humanloop-0.4.2/humanloop/model/project_sort_by.pyi
--rw-r--r--   0        0        0     3795 2023-05-18 18:37:52.295771 humanloop-0.4.2/humanloop/model/project_user_response.py
--rw-r--r--   0        0        0     3795 2023-05-18 18:37:52.295922 humanloop-0.4.2/humanloop/model/project_user_response.pyi
--rw-r--r--   0        0        0     2004 2023-05-18 18:37:52.296048 humanloop-0.4.2/humanloop/model/projects_get_model_configs_response.py
--rw-r--r--   0        0        0     2004 2023-05-18 18:37:52.296181 humanloop-0.4.2/humanloop/model/projects_get_model_configs_response.pyi
--rw-r--r--   0        0        0     1715 2023-05-18 18:37:52.296276 humanloop-0.4.2/humanloop/model/projects_update_feedback_types_request.py
--rw-r--r--   0        0        0     1715 2023-05-18 18:37:52.296373 humanloop-0.4.2/humanloop/model/projects_update_feedback_types_request.pyi
--rw-r--r--   0        0        0     4150 2023-05-18 18:37:52.296491 humanloop-0.4.2/humanloop/model/provider_api_keys.py
--rw-r--r--   0        0        0     4150 2023-05-18 18:37:52.296620 humanloop-0.4.2/humanloop/model/provider_api_keys.pyi
--rw-r--r--   0        0        0     3675 2023-05-18 18:37:52.296734 humanloop-0.4.2/humanloop/model/session_app_response.py
--rw-r--r--   0        0        0     3675 2023-05-18 18:37:52.296887 humanloop-0.4.2/humanloop/model/session_app_response.pyi
--rw-r--r--   0        0        0     4394 2023-05-18 18:37:52.297000 humanloop-0.4.2/humanloop/model/session_response.py
--rw-r--r--   0        0        0     4394 2023-05-18 18:37:52.297153 humanloop-0.4.2/humanloop/model/session_response.pyi
--rw-r--r--   0        0        0     1309 2023-05-18 18:37:52.297347 humanloop-0.4.2/humanloop/model/sort_order.py
--rw-r--r--   0        0        0     1192 2023-05-18 18:37:52.297625 humanloop-0.4.2/humanloop/model/sort_order.pyi
--rw-r--r--   0        0        0    17927 2023-05-18 18:37:52.297803 humanloop-0.4.2/humanloop/model/src_external_app_models_v3_model_configs_model_config_response.py
--rw-r--r--   0        0        0    17927 2023-05-18 18:37:52.297948 humanloop-0.4.2/humanloop/model/src_external_app_models_v3_model_configs_model_config_response.pyi
--rw-r--r--   0        0        0     4889 2023-05-18 18:37:52.298085 humanloop-0.4.2/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py
--rw-r--r--   0        0        0     4889 2023-05-18 18:37:52.298186 humanloop-0.4.2/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.pyi
--rw-r--r--   0        0        0    24036 2023-05-18 18:37:52.298302 humanloop-0.4.2/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_response.py
--rw-r--r--   0        0        0    24036 2023-05-18 18:37:52.298457 humanloop-0.4.2/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_response.pyi
--rw-r--r--   0        0        0    17927 2023-05-18 18:37:52.298607 humanloop-0.4.2/humanloop/model/src_external_app_models_v4_model_configs_model_config_response.py
--rw-r--r--   0        0        0    17927 2023-05-18 18:37:52.298765 humanloop-0.4.2/humanloop/model/src_external_app_models_v4_model_configs_model_config_response.pyi
--rw-r--r--   0        0        0     4889 2023-05-18 18:37:52.298912 humanloop-0.4.2/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_feedback_stats_response.py
--rw-r--r--   0        0        0     4889 2023-05-18 18:37:52.299025 humanloop-0.4.2/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_feedback_stats_response.pyi
--rw-r--r--   0        0        0    24036 2023-05-18 18:37:52.299163 humanloop-0.4.2/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_response.py
--rw-r--r--   0        0        0    24036 2023-05-18 18:37:52.299293 humanloop-0.4.2/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_response.pyi
--rw-r--r--   0        0        0     4232 2023-05-18 18:37:52.299415 humanloop-0.4.2/humanloop/model/tool_result_response.py
--rw-r--r--   0        0        0     4232 2023-05-18 18:37:52.299542 humanloop-0.4.2/humanloop/model/tool_result_response.pyi
--rw-r--r--   0        0        0     7302 2023-05-18 18:37:52.299665 humanloop-0.4.2/humanloop/model/update_experiment_request.py
--rw-r--r--   0        0        0     7302 2023-05-18 18:37:52.299776 humanloop-0.4.2/humanloop/model/update_experiment_request.pyi
--rw-r--r--   0        0        0     5125 2023-05-18 18:37:52.299888 humanloop-0.4.2/humanloop/model/update_project_request.py
--rw-r--r--   0        0        0     5125 2023-05-18 18:37:52.300001 humanloop-0.4.2/humanloop/model/update_project_request.pyi
--rw-r--r--   0        0        0     4118 2023-05-18 18:37:52.300139 humanloop-0.4.2/humanloop/model/usage.py
--rw-r--r--   0        0        0     4118 2023-05-18 18:37:52.300483 humanloop-0.4.2/humanloop/model/usage.pyi
--rw-r--r--   0        0        0     6805 2023-05-18 18:37:52.300810 humanloop-0.4.2/humanloop/model/validation_error.py
--rw-r--r--   0        0        0     6805 2023-05-18 18:37:52.300989 humanloop-0.4.2/humanloop/model/validation_error.pyi
--rw-r--r--   0        0        0     5725 2023-05-18 18:37:52.301126 humanloop-0.4.2/humanloop/models/__init__.py
--rw-r--r--   0        0        0     1603 2023-05-18 18:37:52.301256 humanloop-0.4.2/humanloop/paths/__init__.py
--rw-r--r--   0        0        0      285 2023-05-18 18:37:52.301395 humanloop-0.4.2/humanloop/paths/apps/__init__.py
--rw-r--r--   0        0        0    12735 2023-05-18 18:37:52.301538 humanloop-0.4.2/humanloop/paths/apps/get.py
--rw-r--r--   0        0        0    12592 2023-05-18 18:37:52.301706 humanloop-0.4.2/humanloop/paths/apps/get.pyi
--rw-r--r--   0        0        0      291 2023-05-18 18:37:52.301862 humanloop-0.4.2/humanloop/paths/apps_id/__init__.py
--rw-r--r--   0        0        0    11966 2023-05-18 18:37:52.302005 humanloop-0.4.2/humanloop/paths/apps_id/get.py
--rw-r--r--   0        0        0    11823 2023-05-18 18:37:52.302174 humanloop-0.4.2/humanloop/paths/apps_id/get.pyi
--rw-r--r--   0        0        0      309 2023-05-18 18:37:52.302330 humanloop-0.4.2/humanloop/paths/apps_id_sessions/__init__.py
--rw-r--r--   0        0        0    15570 2023-05-18 18:37:52.302449 humanloop-0.4.2/humanloop/paths/apps_id_sessions/get.py
--rw-r--r--   0        0        0    15427 2023-05-18 18:37:52.302581 humanloop-0.4.2/humanloop/paths/apps_id_sessions/get.pyi
--rw-r--r--   0        0        0      285 2023-05-18 18:37:52.302735 humanloop-0.4.2/humanloop/paths/chat/__init__.py
--rw-r--r--   0        0        0    17428 2023-05-18 18:37:52.302881 humanloop-0.4.2/humanloop/paths/chat/post.py
--rw-r--r--   0        0        0    17285 2023-05-18 18:37:52.303068 humanloop-0.4.2/humanloop/paths/chat/post.pyi
--rw-r--r--   0        0        0      302 2023-05-18 18:37:52.303225 humanloop-0.4.2/humanloop/paths/chat_deployed/__init__.py
--rw-r--r--   0        0        0    16991 2023-05-18 18:37:52.303341 humanloop-0.4.2/humanloop/paths/chat_deployed/post.py
--rw-r--r--   0        0        0    16848 2023-05-18 18:37:52.303548 humanloop-0.4.2/humanloop/paths/chat_deployed/post.pyi
--rw-r--r--   0        0        0      306 2023-05-18 18:37:52.303730 humanloop-0.4.2/humanloop/paths/chat_experiment/__init__.py
--rw-r--r--   0        0        0    17434 2023-05-18 18:37:52.303868 humanloop-0.4.2/humanloop/paths/chat_experiment/post.py
--rw-r--r--   0        0        0    17291 2023-05-18 18:37:52.304002 humanloop-0.4.2/humanloop/paths/chat_experiment/post.pyi
--rw-r--r--   0        0        0      309 2023-05-18 18:37:52.304136 humanloop-0.4.2/humanloop/paths/chat_model_config/__init__.py
--rw-r--r--   0        0        0    17609 2023-05-18 18:37:52.304261 humanloop-0.4.2/humanloop/paths/chat_model_config/post.py
--rw-r--r--   0        0        0    17466 2023-05-18 18:37:52.304400 humanloop-0.4.2/humanloop/paths/chat_model_config/post.pyi
--rw-r--r--   0        0        0      297 2023-05-18 18:37:52.304527 humanloop-0.4.2/humanloop/paths/completion/__init__.py
--rw-r--r--   0        0        0    17744 2023-05-18 18:37:52.304632 humanloop-0.4.2/humanloop/paths/completion/post.py
--rw-r--r--   0        0        0    17601 2023-05-18 18:37:52.304766 humanloop-0.4.2/humanloop/paths/completion/post.pyi
--rw-r--r--   0        0        0      314 2023-05-18 18:37:52.304888 humanloop-0.4.2/humanloop/paths/completion_deployed/__init__.py
--rw-r--r--   0        0        0    17247 2023-05-18 18:37:52.305008 humanloop-0.4.2/humanloop/paths/completion_deployed/post.py
--rw-r--r--   0        0        0    17104 2023-05-18 18:37:52.305133 humanloop-0.4.2/humanloop/paths/completion_deployed/post.pyi
--rw-r--r--   0        0        0      318 2023-05-18 18:37:52.305249 humanloop-0.4.2/humanloop/paths/completion_experiment/__init__.py
--rw-r--r--   0        0        0    17690 2023-05-18 18:37:52.305360 humanloop-0.4.2/humanloop/paths/completion_experiment/post.py
--rw-r--r--   0        0        0    17547 2023-05-18 18:37:52.305488 humanloop-0.4.2/humanloop/paths/completion_experiment/post.pyi
--rw-r--r--   0        0        0      321 2023-05-18 18:37:52.305615 humanloop-0.4.2/humanloop/paths/completion_model_config/__init__.py
--rw-r--r--   0        0        0    17865 2023-05-18 18:37:52.305744 humanloop-0.4.2/humanloop/paths/completion_model_config/post.py
--rw-r--r--   0        0        0    17722 2023-05-18 18:37:52.305876 humanloop-0.4.2/humanloop/paths/completion_model_config/post.pyi
--rw-r--r--   0        0        0      327 2023-05-18 18:37:52.306025 humanloop-0.4.2/humanloop/paths/experiments_experiment_id/__init__.py
--rw-r--r--   0        0        0    11995 2023-05-18 18:37:52.306144 humanloop-0.4.2/humanloop/paths/experiments_experiment_id/delete.py
--rw-r--r--   0        0        0    11852 2023-05-18 18:37:52.306295 humanloop-0.4.2/humanloop/paths/experiments_experiment_id/delete.pyi
--rw-r--r--   0        0        0    17043 2023-05-18 18:37:52.306463 humanloop-0.4.2/humanloop/paths/experiments_experiment_id/patch.py
--rw-r--r--   0        0        0    16900 2023-05-18 18:37:52.306684 humanloop-0.4.2/humanloop/paths/experiments_experiment_id/patch.pyi
--rw-r--r--   0        0        0      352 2023-05-18 18:37:52.306858 humanloop-0.4.2/humanloop/paths/experiments_experiment_id_model_config/__init__.py
--rw-r--r--   0        0        0    12496 2023-05-18 18:37:52.307034 humanloop-0.4.2/humanloop/paths/experiments_experiment_id_model_config/get.py
--rw-r--r--   0        0        0    12353 2023-05-18 18:37:52.307178 humanloop-0.4.2/humanloop/paths/experiments_experiment_id_model_config/get.pyi
--rw-r--r--   0        0        0      293 2023-05-18 18:37:52.307369 humanloop-0.4.2/humanloop/paths/feedback/__init__.py
--rw-r--r--   0        0        0    15089 2023-05-18 18:37:52.307477 humanloop-0.4.2/humanloop/paths/feedback/post.py
--rw-r--r--   0        0        0    14946 2023-05-18 18:37:52.307640 humanloop-0.4.2/humanloop/paths/feedback/post.pyi
--rw-r--r--   0        0        0      285 2023-05-18 18:37:52.307873 humanloop-0.4.2/humanloop/paths/logs/__init__.py
--rw-r--r--   0        0        0    19620 2023-05-18 18:37:52.307994 humanloop-0.4.2/humanloop/paths/logs/post.py
--rw-r--r--   0        0        0    19477 2023-05-18 18:37:52.308178 humanloop-0.4.2/humanloop/paths/logs/post.pyi
--rw-r--r--   0        0        0      302 2023-05-18 18:37:52.308327 humanloop-0.4.2/humanloop/paths/model_configs/__init__.py
--rw-r--r--   0        0        0    20552 2023-05-18 18:37:52.308511 humanloop-0.4.2/humanloop/paths/model_configs/post.py
--rw-r--r--   0        0        0    20409 2023-05-18 18:37:52.308651 humanloop-0.4.2/humanloop/paths/model_configs/post.pyi
--rw-r--r--   0        0        0      308 2023-05-18 18:37:52.308792 humanloop-0.4.2/humanloop/paths/model_configs_id/__init__.py
--rw-r--r--   0        0        0    12309 2023-05-18 18:37:52.308900 humanloop-0.4.2/humanloop/paths/model_configs_id/get.py
--rw-r--r--   0        0        0    12166 2023-05-18 18:37:52.309042 humanloop-0.4.2/humanloop/paths/model_configs_id/get.pyi
--rw-r--r--   0        0        0      293 2023-05-18 18:37:52.309195 humanloop-0.4.2/humanloop/paths/projects/__init__.py
--rw-r--r--   0        0        0    20518 2023-05-18 18:37:52.309320 humanloop-0.4.2/humanloop/paths/projects/get.py
--rw-r--r--   0        0        0    20375 2023-05-18 18:37:52.309448 humanloop-0.4.2/humanloop/paths/projects/get.pyi
--rw-r--r--   0        0        0    13007 2023-05-18 18:37:52.309558 humanloop-0.4.2/humanloop/paths/projects/post.py
--rw-r--r--   0        0        0    12864 2023-05-18 18:37:52.309676 humanloop-0.4.2/humanloop/paths/projects/post.pyi
--rw-r--r--   0        0        0      299 2023-05-18 18:37:52.309817 humanloop-0.4.2/humanloop/paths/projects_id/__init__.py
--rw-r--r--   0        0        0    11979 2023-05-18 18:37:52.309948 humanloop-0.4.2/humanloop/paths/projects_id/get.py
--rw-r--r--   0        0        0    11836 2023-05-18 18:37:52.310073 humanloop-0.4.2/humanloop/paths/projects_id/get.pyi
--rw-r--r--   0        0        0    16162 2023-05-18 18:37:52.310182 humanloop-0.4.2/humanloop/paths/projects_id/patch.py
--rw-r--r--   0        0        0    16019 2023-05-18 18:37:52.310315 humanloop-0.4.2/humanloop/paths/projects_id/patch.pyi
--rw-r--r--   0        0        0      334 2023-05-18 18:37:52.310428 humanloop-0.4.2/humanloop/paths/projects_id_active_experiment/__init__.py
--rw-r--r--   0        0        0    12306 2023-05-18 18:37:52.310542 humanloop-0.4.2/humanloop/paths/projects_id_active_experiment/delete.py
--rw-r--r--   0        0        0    12163 2023-05-18 18:37:52.310717 humanloop-0.4.2/humanloop/paths/projects_id_active_experiment/delete.pyi
--rw-r--r--   0        0        0      337 2023-05-18 18:37:52.310899 humanloop-0.4.2/humanloop/paths/projects_id_active_model_config/__init__.py
--rw-r--r--   0        0        0    12337 2023-05-18 18:37:52.310998 humanloop-0.4.2/humanloop/paths/projects_id_active_model_config/delete.py
--rw-r--r--   0        0        0    12194 2023-05-18 18:37:52.311131 humanloop-0.4.2/humanloop/paths/projects_id_active_model_config/delete.pyi
--rw-r--r--   0        0        0      313 2023-05-18 18:37:52.311241 humanloop-0.4.2/humanloop/paths/projects_id_export/__init__.py
--rw-r--r--   0        0        0    15728 2023-05-18 18:37:52.311370 humanloop-0.4.2/humanloop/paths/projects_id_export/post.py
--rw-r--r--   0        0        0    15585 2023-05-18 18:37:52.311532 humanloop-0.4.2/humanloop/paths/projects_id_export/post.pyi
--rw-r--r--   0        0        0      328 2023-05-18 18:37:52.311739 humanloop-0.4.2/humanloop/paths/projects_id_feedback_types/__init__.py
--rw-r--r--   0        0        0    14809 2023-05-18 18:37:52.311847 humanloop-0.4.2/humanloop/paths/projects_id_feedback_types/patch.py
--rw-r--r--   0        0        0    14666 2023-05-18 18:37:52.311987 humanloop-0.4.2/humanloop/paths/projects_id_feedback_types/patch.pyi
--rw-r--r--   0        0        0      324 2023-05-18 18:37:52.312157 humanloop-0.4.2/humanloop/paths/projects_id_model_config/__init__.py
--rw-r--r--   0        0        0    12229 2023-05-18 18:37:52.312306 humanloop-0.4.2/humanloop/paths/projects_id_model_config/get.py
--rw-r--r--   0        0        0    12086 2023-05-18 18:37:52.312454 humanloop-0.4.2/humanloop/paths/projects_id_model_config/get.pyi
--rw-r--r--   0        0        0      326 2023-05-18 18:37:52.312622 humanloop-0.4.2/humanloop/paths/projects_id_model_configs/__init__.py
--rw-r--r--   0        0        0    12319 2023-05-18 18:37:52.312728 humanloop-0.4.2/humanloop/paths/projects_id_model_configs/get.py
--rw-r--r--   0        0        0    12176 2023-05-18 18:37:52.312899 humanloop-0.4.2/humanloop/paths/projects_id_model_configs/get.pyi
--rw-r--r--   0        0        0      339 2023-05-18 18:37:52.313042 humanloop-0.4.2/humanloop/paths/projects_project_id_experiments/__init__.py
--rw-r--r--   0        0        0    12256 2023-05-18 18:37:52.313196 humanloop-0.4.2/humanloop/paths/projects_project_id_experiments/get.py
--rw-r--r--   0        0        0    12113 2023-05-18 18:37:52.313358 humanloop-0.4.2/humanloop/paths/projects_project_id_experiments/get.pyi
--rw-r--r--   0        0        0    16346 2023-05-18 18:37:52.313654 humanloop-0.4.2/humanloop/paths/projects_project_id_experiments/post.py
--rw-r--r--   0        0        0    16203 2023-05-18 18:37:52.313860 humanloop-0.4.2/humanloop/paths/projects_project_id_experiments/post.pyi
--rw-r--r--   0        0        0      293 2023-05-18 18:37:52.314039 humanloop-0.4.2/humanloop/paths/sessions/__init__.py
--rw-r--r--   0        0        0    12149 2023-05-18 18:37:52.314166 humanloop-0.4.2/humanloop/paths/sessions/post.py
--rw-r--r--   0        0        0    12006 2023-05-18 18:37:52.314381 humanloop-0.4.2/humanloop/paths/sessions/post.pyi
--rw-r--r--   0        0        0      299 2023-05-18 18:37:52.314505 humanloop-0.4.2/humanloop/paths/sessions_id/__init__.py
--rw-r--r--   0        0        0    11974 2023-05-18 18:37:52.314666 humanloop-0.4.2/humanloop/paths/sessions_id/get.py
--rw-r--r--   0        0        0    11831 2023-05-18 18:37:52.314803 humanloop-0.4.2/humanloop/paths/sessions_id/get.pyi
--rw-r--r--   0        0        0      313 2023-05-18 18:37:52.315065 humanloop-0.4.2/humanloop/paths/sessions_id_events/__init__.py
--rw-r--r--   0        0        0    12085 2023-05-18 18:37:52.315175 humanloop-0.4.2/humanloop/paths/sessions_id_events/get.py
--rw-r--r--   0        0        0    11942 2023-05-18 18:37:52.315299 humanloop-0.4.2/humanloop/paths/sessions_id_events/get.pyi
--rw-r--r--   0        0        0     1011 2023-05-18 18:37:52.315456 humanloop-0.4.2/humanloop/request_after_hook.py
--rw-r--r--   0        0        0     1783 2023-05-18 18:32:32.791241 humanloop-0.4.2/humanloop/request_before_hook.py
--rw-r--r--   0        0        0    11329 2023-05-18 18:37:52.315576 humanloop-0.4.2/humanloop/rest.py
--rw-r--r--   0        0        0    95913 2023-05-18 18:37:52.315904 humanloop-0.4.2/humanloop/schemas.py
--rw-r--r--   0        0        0        0 2023-05-18 18:37:52.316060 humanloop-0.4.2/humanloop/type/__init__.py
--rw-r--r--   0        0        0     1489 2023-05-18 18:37:52.316200 humanloop-0.4.2/humanloop/type/base_metric_response.py
--rw-r--r--   0        0        0     1137 2023-05-18 18:37:52.316302 humanloop-0.4.2/humanloop/type/categorical_feedback_label.py
--rw-r--r--   0        0        0     2272 2023-05-18 18:37:52.316437 humanloop-0.4.2/humanloop/type/chat_data_response.py
--rw-r--r--   0        0        0     2085 2023-05-18 18:37:52.316557 humanloop-0.4.2/humanloop/type/chat_deployed_request.py
--rw-r--r--   0        0        0     2337 2023-05-18 18:37:52.316691 humanloop-0.4.2/humanloop/type/chat_experiment_request.py
--rw-r--r--   0        0        0      980 2023-05-18 18:37:52.316804 humanloop-0.4.2/humanloop/type/chat_message.py
--rw-r--r--   0        0        0     2208 2023-05-18 18:37:52.316948 humanloop-0.4.2/humanloop/type/chat_model_config_request.py
--rw-r--r--   0        0        0     2212 2023-05-18 18:37:52.317067 humanloop-0.4.2/humanloop/type/chat_request.py
--rw-r--r--   0        0        0     1899 2023-05-18 18:37:52.317202 humanloop-0.4.2/humanloop/type/chat_response.py
--rw-r--r--   0        0        0      711 2023-05-18 18:37:52.317301 humanloop-0.4.2/humanloop/type/chat_role.py
--rw-r--r--   0        0        0     2205 2023-05-18 18:37:52.317407 humanloop-0.4.2/humanloop/type/completion_deployed_request.py
--rw-r--r--   0        0        0     2460 2023-05-18 18:37:52.317499 humanloop-0.4.2/humanloop/type/completion_experiment_request.py
--rw-r--r--   0        0        0     2328 2023-05-18 18:37:52.317631 humanloop-0.4.2/humanloop/type/completion_model_config_request.py
--rw-r--r--   0        0        0     2336 2023-05-18 18:37:52.317723 humanloop-0.4.2/humanloop/type/completion_request.py
--rw-r--r--   0        0        0     1957 2023-05-18 18:37:52.317865 humanloop-0.4.2/humanloop/type/completion_response.py
--rw-r--r--   0        0        0     1468 2023-05-18 18:37:52.318026 humanloop-0.4.2/humanloop/type/create_experiment_request.py
--rw-r--r--   0        0        0     1085 2023-05-18 18:37:52.318167 humanloop-0.4.2/humanloop/type/create_log_response.py
--rw-r--r--   0        0        0     1142 2023-05-18 18:37:52.318335 humanloop-0.4.2/humanloop/type/create_project_request.py
--rw-r--r--   0        0        0     1000 2023-05-18 18:37:52.318467 humanloop-0.4.2/humanloop/type/create_session_request.py
--rw-r--r--   0        0        0     2091 2023-05-18 18:37:52.318637 humanloop-0.4.2/humanloop/type/data_response.py
--rw-r--r--   0        0        0     1954 2023-05-18 18:37:52.318793 humanloop-0.4.2/humanloop/type/experiment_model_config_response.py
--rw-r--r--   0        0        0     1909 2023-05-18 18:37:52.318939 humanloop-0.4.2/humanloop/type/experiment_response.py
--rw-r--r--   0        0        0      718 2023-05-18 18:37:52.319099 humanloop-0.4.2/humanloop/type/experiment_status.py
--rw-r--r--   0        0        0      785 2023-05-18 18:37:52.319212 humanloop-0.4.2/humanloop/type/experiments_list_response.py
--rw-r--r--   0        0        0     1510 2023-05-18 18:37:52.319339 humanloop-0.4.2/humanloop/type/feedback.py
--rw-r--r--   0        0        0      719 2023-05-18 18:37:52.319467 humanloop-0.4.2/humanloop/type/feedback_class.py
--rw-r--r--   0        0        0     1046 2023-05-18 18:37:52.319599 humanloop-0.4.2/humanloop/type/feedback_label_request.py
--rw-r--r--   0        0        0     1624 2023-05-18 18:37:52.319727 humanloop-0.4.2/humanloop/type/feedback_request.py
--rw-r--r--   0        0        0     1658 2023-05-18 18:37:52.319836 humanloop-0.4.2/humanloop/type/feedback_response.py
--rw-r--r--   0        0        0      804 2023-05-18 18:37:52.319968 humanloop-0.4.2/humanloop/type/feedback_submit_request.py
--rw-r--r--   0        0        0      809 2023-05-18 18:37:52.320075 humanloop-0.4.2/humanloop/type/feedback_submit_response.py
--rw-r--r--   0        0        0      738 2023-05-18 18:37:52.320201 humanloop-0.4.2/humanloop/type/feedback_type.py
--rw-r--r--   0        0        0     1377 2023-05-18 18:37:52.320320 humanloop-0.4.2/humanloop/type/feedback_type_model.py
--rw-r--r--   0        0        0     1541 2023-05-18 18:37:52.320473 humanloop-0.4.2/humanloop/type/feedback_type_request.py
--rw-r--r--   0        0        0      773 2023-05-18 18:37:52.320600 humanloop-0.4.2/humanloop/type/feedback_types.py
--rw-r--r--   0        0        0     4271 2023-05-18 18:37:52.320766 humanloop-0.4.2/humanloop/type/get_model_config_response.py
--rw-r--r--   0        0        0     1034 2023-05-18 18:37:52.320895 humanloop-0.4.2/humanloop/type/http_validation_error.py
--rw-r--r--   0        0        0      730 2023-05-18 18:37:52.321010 humanloop-0.4.2/humanloop/type/label_sentiment.py
--rw-r--r--   0        0        0      782 2023-05-18 18:37:52.321171 humanloop-0.4.2/humanloop/type/log_datapoint_request.py
--rw-r--r--   0        0        0     2430 2023-05-18 18:37:52.321277 humanloop-0.4.2/humanloop/type/log_request.py
--rw-r--r--   0        0        0     2968 2023-05-18 18:37:52.321395 humanloop-0.4.2/humanloop/type/log_response.py
--rw-r--r--   0        0        0      807 2023-05-18 18:37:52.321552 humanloop-0.4.2/humanloop/type/logs_log_response.py
--rw-r--r--   0        0        0     2927 2023-05-18 18:37:52.321678 humanloop-0.4.2/humanloop/type/model_config_chat_request.py
--rw-r--r--   0        0        0     2832 2023-05-18 18:37:52.321812 humanloop-0.4.2/humanloop/type/model_config_completion_request.py
--rw-r--r--   0        0        0      714 2023-05-18 18:37:52.321954 humanloop-0.4.2/humanloop/type/model_endpoints.py
--rw-r--r--   0        0        0      738 2023-05-18 18:37:52.322055 humanloop-0.4.2/humanloop/type/model_providers.py
--rw-r--r--   0        0        0     1113 2023-05-18 18:37:52.322218 humanloop-0.4.2/humanloop/type/paginated_data_log_response.py
--rw-r--r--   0        0        0     1153 2023-05-18 18:37:52.322335 humanloop-0.4.2/humanloop/type/paginated_data_project_response.py
--rw-r--r--   0        0        0      924 2023-05-18 18:37:52.322466 humanloop-0.4.2/humanloop/type/positive_label.py
--rw-r--r--   0        0        0     3535 2023-05-18 18:37:52.322628 humanloop-0.4.2/humanloop/type/project_model_config_request.py
--rw-r--r--   0        0        0     2190 2023-05-18 18:37:52.322750 humanloop-0.4.2/humanloop/type/project_response.py
--rw-r--r--   0        0        0      721 2023-05-18 18:37:52.322875 humanloop-0.4.2/humanloop/type/project_sort_by.py
--rw-r--r--   0        0        0     1099 2023-05-18 18:37:52.323030 humanloop-0.4.2/humanloop/type/project_user_response.py
--rw-r--r--   0        0        0      928 2023-05-18 18:37:52.323146 humanloop-0.4.2/humanloop/type/projects_get_model_configs_response.py
--rw-r--r--   0        0        0      800 2023-05-18 18:37:52.323256 humanloop-0.4.2/humanloop/type/projects_update_feedback_types_request.py
--rw-r--r--   0        0        0      980 2023-05-18 18:37:52.323453 humanloop-0.4.2/humanloop/type/provider_api_keys.py
--rw-r--r--   0        0        0     1024 2023-05-18 18:37:52.323650 humanloop-0.4.2/humanloop/type/session_app_response.py
--rw-r--r--   0        0        0     1074 2023-05-18 18:37:52.323759 humanloop-0.4.2/humanloop/type/session_response.py
--rw-r--r--   0        0        0      696 2023-05-18 18:37:52.323867 humanloop-0.4.2/humanloop/type/sort_order.py
--rw-r--r--   0        0        0     3508 2023-05-18 18:37:52.323994 humanloop-0.4.2/humanloop/type/src_external_app_models_v3_model_configs_model_config_response.py
--rw-r--r--   0        0        0     1420 2023-05-18 18:37:52.324095 humanloop-0.4.2/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py
--rw-r--r--   0        0        0     4439 2023-05-18 18:37:52.324211 humanloop-0.4.2/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_response.py
--rw-r--r--   0        0        0     3528 2023-05-18 18:37:52.324375 humanloop-0.4.2/humanloop/type/src_external_app_models_v4_model_configs_model_config_response.py
--rw-r--r--   0        0        0     1420 2023-05-18 18:37:52.324504 humanloop-0.4.2/humanloop/type/src_external_app_models_v4_model_configs_project_model_config_feedback_stats_response.py
--rw-r--r--   0        0        0     4459 2023-05-18 18:37:52.324627 humanloop-0.4.2/humanloop/type/src_external_app_models_v4_model_configs_project_model_config_response.py
--rw-r--r--   0        0        0      999 2023-05-18 18:37:52.324729 humanloop-0.4.2/humanloop/type/tool_result_response.py
--rw-r--r--   0        0        0     1440 2023-05-18 18:37:52.324871 humanloop-0.4.2/humanloop/type/update_experiment_request.py
--rw-r--r--   0        0        0     1529 2023-05-18 18:37:52.324992 humanloop-0.4.2/humanloop/type/update_project_request.py
--rw-r--r--   0        0        0     1082 2023-05-18 18:37:52.325105 humanloop-0.4.2/humanloop/type/usage.py
--rw-r--r--   0        0        0     1011 2023-05-18 18:37:52.325252 humanloop-0.4.2/humanloop/type/validation_error.py
--rw-r--r--   0        0        0      868 2023-05-18 18:37:52.325401 humanloop-0.4.2/humanloop/type_util.py
--rw-r--r--   0        0        0     3165 2023-05-18 18:37:52.325533 humanloop-0.4.2/humanloop/validation_metadata.py
--rw-r--r--   0        0        0      714 2023-05-18 18:37:52.326123 humanloop-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     9366 1970-01-01 00:00:00.000000 humanloop-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-24 22:06:03.788313 humanloop-0.4.3/LICENSE
+-rw-r--r--   0        0        0     8475 2023-05-24 22:06:03.847069 humanloop-0.4.3/README.md
+-rw-r--r--   0        0        0     1059 2023-05-24 22:06:03.698102 humanloop-0.4.3/humanloop/__init__.py
+-rw-r--r--   0        0        0    73009 2023-05-24 22:06:03.698441 humanloop-0.4.3/humanloop/api_client.py
+-rw-r--r--   0        0        0      663 2023-05-24 22:06:03.698616 humanloop-0.4.3/humanloop/api_response.py
+-rw-r--r--   0        0        0      214 2023-05-24 22:06:03.698783 humanloop-0.4.3/humanloop/apis/__init__.py
+-rw-r--r--   0        0        0     4578 2023-05-24 22:06:03.698925 humanloop-0.4.3/humanloop/apis/path_to_api.py
+-rw-r--r--   0        0        0      236 2023-05-24 22:06:03.699095 humanloop-0.4.3/humanloop/apis/paths/__init__.py
+-rw-r--r--   0        0        0       91 2023-05-24 22:06:03.699244 humanloop-0.4.3/humanloop/apis/paths/chat.py
+-rw-r--r--   0        0        0      108 2023-05-24 22:06:03.699392 humanloop-0.4.3/humanloop/apis/paths/chat_deployed.py
+-rw-r--r--   0        0        0      112 2023-05-24 22:06:03.699552 humanloop-0.4.3/humanloop/apis/paths/chat_experiment.py
+-rw-r--r--   0        0        0      115 2023-05-24 22:06:03.699709 humanloop-0.4.3/humanloop/apis/paths/chat_model_config.py
+-rw-r--r--   0        0        0      103 2023-05-24 22:06:03.699869 humanloop-0.4.3/humanloop/apis/paths/completion.py
+-rw-r--r--   0        0        0      120 2023-05-24 22:06:03.700519 humanloop-0.4.3/humanloop/apis/paths/completion_deployed.py
+-rw-r--r--   0        0        0      124 2023-05-24 22:06:03.700621 humanloop-0.4.3/humanloop/apis/paths/completion_experiment.py
+-rw-r--r--   0        0        0      127 2023-05-24 22:06:03.700710 humanloop-0.4.3/humanloop/apis/paths/completion_model_config.py
+-rw-r--r--   0        0        0      226 2023-05-24 22:06:03.700822 humanloop-0.4.3/humanloop/apis/paths/experiments_experiment_id.py
+-rw-r--r--   0        0        0      152 2023-05-24 22:06:03.700965 humanloop-0.4.3/humanloop/apis/paths/experiments_experiment_id_model_config.py
+-rw-r--r--   0        0        0       99 2023-05-24 22:06:03.701106 humanloop-0.4.3/humanloop/apis/paths/feedback.py
+-rw-r--r--   0        0        0       91 2023-05-24 22:06:03.701240 humanloop-0.4.3/humanloop/apis/paths/logs.py
+-rw-r--r--   0        0        0      108 2023-05-24 22:06:03.701367 humanloop-0.4.3/humanloop/apis/paths/model_configs.py
+-rw-r--r--   0        0        0      110 2023-05-24 22:06:03.701456 humanloop-0.4.3/humanloop/apis/paths/model_configs_id.py
+-rw-r--r--   0        0        0      165 2023-05-24 22:06:03.701592 humanloop-0.4.3/humanloop/apis/paths/projects.py
+-rw-r--r--   0        0        0      176 2023-05-24 22:06:03.701725 humanloop-0.4.3/humanloop/apis/paths/projects_id.py
+-rw-r--r--   0        0        0      219 2023-05-24 22:06:03.701864 humanloop-0.4.3/humanloop/apis/paths/projects_id_active_config.py
+-rw-r--r--   0        0        0      144 2023-05-24 22:06:03.702005 humanloop-0.4.3/humanloop/apis/paths/projects_id_active_experiment.py
+-rw-r--r--   0        0        0      116 2023-05-24 22:06:03.702133 humanloop-0.4.3/humanloop/apis/paths/projects_id_configs.py
+-rw-r--r--   0        0        0      117 2023-05-24 22:06:03.702273 humanloop-0.4.3/humanloop/apis/paths/projects_id_export.py
+-rw-r--r--   0        0        0      135 2023-05-24 22:06:03.702432 humanloop-0.4.3/humanloop/apis/paths/projects_id_feedback_types.py
+-rw-r--r--   0        0        0      231 2023-05-24 22:06:03.702973 humanloop-0.4.3/humanloop/apis/paths/projects_project_id_experiments.py
+-rw-r--r--   0        0        0      165 2023-05-24 22:06:03.703230 humanloop-0.4.3/humanloop/apis/paths/sessions.py
+-rw-r--r--   0        0        0      101 2023-05-24 22:06:03.703487 humanloop-0.4.3/humanloop/apis/paths/sessions_id.py
+-rw-r--r--   0        0        0       95 2023-05-24 22:06:03.703696 humanloop-0.4.3/humanloop/apis/paths/traces.py
+-rw-r--r--   0        0        0     1654 2023-05-24 22:06:03.703840 humanloop-0.4.3/humanloop/apis/tag_to_api.py
+-rw-r--r--   0        0        0      572 2023-05-24 22:06:03.703959 humanloop-0.4.3/humanloop/apis/tags/__init__.py
+-rw-r--r--   0        0        0     1006 2023-05-24 22:06:03.704067 humanloop-0.4.3/humanloop/apis/tags/chats_api.py
+-rw-r--r--   0        0        0     1020 2023-05-24 22:06:03.704208 humanloop-0.4.3/humanloop/apis/tags/completions_api.py
+-rw-r--r--   0        0        0     1091 2023-05-24 22:06:03.704352 humanloop-0.4.3/humanloop/apis/tags/experiments_api.py
+-rw-r--r--   0        0        0      721 2023-05-24 22:06:03.704504 humanloop-0.4.3/humanloop/apis/tags/feedback_api.py
+-rw-r--r--   0        0        0      707 2023-05-24 22:06:03.704671 humanloop-0.4.3/humanloop/apis/tags/logs_api.py
+-rw-r--r--   0        0        0      803 2023-05-24 22:06:03.704948 humanloop-0.4.3/humanloop/apis/tags/model_configurations_api.py
+-rw-r--r--   0        0        0     1486 2023-05-24 22:06:03.705091 humanloop-0.4.3/humanloop/apis/tags/projects_api.py
+-rw-r--r--   0        0        0      834 2023-05-24 22:06:03.705260 humanloop-0.4.3/humanloop/apis/tags/sessions_api.py
+-rw-r--r--   0        0        0      717 2023-05-24 22:06:03.705450 humanloop-0.4.3/humanloop/apis/tags/traces_api.py
+-rw-r--r--   0        0        0    28032 2023-05-24 22:06:03.705692 humanloop-0.4.3/humanloop/client.py
+-rw-r--r--   0        0        0    28032 2023-05-24 22:06:03.706024 humanloop-0.4.3/humanloop/client.pyi
+-rw-r--r--   0        0        0     7186 2023-05-18 09:14:14.289106 humanloop-0.4.3/humanloop/client_custom.py
+-rw-r--r--   0        0        0    18674 2023-05-24 22:06:03.706348 humanloop-0.4.3/humanloop/configuration.py
+-rw-r--r--   0        0        0     7678 2023-05-24 22:06:03.706602 humanloop-0.4.3/humanloop/exceptions.py
+-rw-r--r--   0        0        0     2274 2023-05-24 22:06:03.706771 humanloop-0.4.3/humanloop/exceptions_base.py
+-rw-r--r--   0        0        0      343 2023-05-24 22:06:03.707079 humanloop-0.4.3/humanloop/model/__init__.py
+-rw-r--r--   0        0        0     9140 2023-05-24 22:06:03.707324 humanloop-0.4.3/humanloop/model/agent_config_request.py
+-rw-r--r--   0        0        0     8975 2023-05-24 22:06:03.707953 humanloop-0.4.3/humanloop/model/agent_config_request.pyi
+-rw-r--r--   0        0        0    11140 2023-05-24 22:06:03.712785 humanloop-0.4.3/humanloop/model/agent_config_response.py
+-rw-r--r--   0        0        0    11140 2023-05-24 22:06:03.713182 humanloop-0.4.3/humanloop/model/agent_config_response.pyi
+-rw-r--r--   0        0        0     6379 2023-05-24 22:06:03.713516 humanloop-0.4.3/humanloop/model/base_metric_response.py
+-rw-r--r--   0        0        0     6379 2023-05-24 22:06:03.713738 humanloop-0.4.3/humanloop/model/base_metric_response.pyi
+-rw-r--r--   0        0        0     5150 2023-05-24 22:06:03.713962 humanloop-0.4.3/humanloop/model/categorical_feedback_label.py
+-rw-r--r--   0        0        0     5150 2023-05-24 22:06:03.714167 humanloop-0.4.3/humanloop/model/categorical_feedback_label.pyi
+-rw-r--r--   0        0        0     8957 2023-05-24 22:06:03.714373 humanloop-0.4.3/humanloop/model/chat_data_response.py
+-rw-r--r--   0        0        0     8957 2023-05-24 22:06:03.714596 humanloop-0.4.3/humanloop/model/chat_data_response.pyi
+-rw-r--r--   0        0        0     9998 2023-05-24 22:06:03.714836 humanloop-0.4.3/humanloop/model/chat_deployed_request.py
+-rw-r--r--   0        0        0     9998 2023-05-24 22:06:03.715159 humanloop-0.4.3/humanloop/model/chat_deployed_request.pyi
+-rw-r--r--   0        0        0    10659 2023-05-24 22:06:03.715423 humanloop-0.4.3/humanloop/model/chat_experiment_request.py
+-rw-r--r--   0        0        0    10659 2023-05-24 22:06:03.715671 humanloop-0.4.3/humanloop/model/chat_experiment_request.pyi
+-rw-r--r--   0        0        0     3702 2023-05-24 22:06:03.715885 humanloop-0.4.3/humanloop/model/chat_message.py
+-rw-r--r--   0        0        0     3702 2023-05-24 22:06:03.716094 humanloop-0.4.3/humanloop/model/chat_message.pyi
+-rw-r--r--   0        0        0    10693 2023-05-24 22:06:03.716302 humanloop-0.4.3/humanloop/model/chat_model_config_request.py
+-rw-r--r--   0        0        0    10693 2023-05-24 22:06:03.716560 humanloop-0.4.3/humanloop/model/chat_model_config_request.pyi
+-rw-r--r--   0        0        0    12556 2023-05-24 22:06:03.716796 humanloop-0.4.3/humanloop/model/chat_request.py
+-rw-r--r--   0        0        0    12556 2023-05-24 22:06:03.717010 humanloop-0.4.3/humanloop/model/chat_request.pyi
+-rw-r--r--   0        0        0    11076 2023-05-24 22:06:03.717221 humanloop-0.4.3/humanloop/model/chat_response.py
+-rw-r--r--   0        0        0    11076 2023-05-24 22:06:03.717435 humanloop-0.4.3/humanloop/model/chat_response.pyi
+-rw-r--r--   0        0        0     1446 2023-05-24 22:06:03.717633 humanloop-0.4.3/humanloop/model/chat_role.py
+-rw-r--r--   0        0        0     1285 2023-05-24 22:06:03.717800 humanloop-0.4.3/humanloop/model/chat_role.pyi
+-rw-r--r--   0        0        0     9674 2023-05-24 22:06:03.717994 humanloop-0.4.3/humanloop/model/completion_deployed_request.py
+-rw-r--r--   0        0        0     9674 2023-05-24 22:06:03.718221 humanloop-0.4.3/humanloop/model/completion_deployed_request.pyi
+-rw-r--r--   0        0        0    10340 2023-05-24 22:06:03.718476 humanloop-0.4.3/humanloop/model/completion_experiment_request.py
+-rw-r--r--   0        0        0    10340 2023-05-24 22:06:03.718727 humanloop-0.4.3/humanloop/model/completion_experiment_request.pyi
+-rw-r--r--   0        0        0    10376 2023-05-24 22:06:03.718968 humanloop-0.4.3/humanloop/model/completion_model_config_request.py
+-rw-r--r--   0        0        0    10376 2023-05-24 22:06:03.719186 humanloop-0.4.3/humanloop/model/completion_model_config_request.pyi
+-rw-r--r--   0        0        0    12258 2023-05-24 22:06:03.719396 humanloop-0.4.3/humanloop/model/completion_request.py
+-rw-r--r--   0        0        0    12258 2023-05-24 22:06:03.719624 humanloop-0.4.3/humanloop/model/completion_request.pyi
+-rw-r--r--   0        0        0    11017 2023-05-24 22:06:03.719855 humanloop-0.4.3/humanloop/model/completion_response.py
+-rw-r--r--   0        0        0    11017 2023-05-24 22:06:03.720071 humanloop-0.4.3/humanloop/model/completion_response.pyi
+-rw-r--r--   0        0        0     2672 2023-05-24 22:06:03.720251 humanloop-0.4.3/humanloop/model/config_response.py
+-rw-r--r--   0        0        0     2672 2023-05-24 22:06:03.720399 humanloop-0.4.3/humanloop/model/config_response.pyi
+-rw-r--r--   0        0        0     1546 2023-05-24 22:06:03.720543 humanloop-0.4.3/humanloop/model/config_type.py
+-rw-r--r--   0        0        0     1361 2023-05-24 22:06:03.720704 humanloop-0.4.3/humanloop/model/config_type.pyi
+-rw-r--r--   0        0        0     6196 2023-05-24 22:06:03.720853 humanloop-0.4.3/humanloop/model/create_experiment_request.py
+-rw-r--r--   0        0        0     6196 2023-05-24 22:06:03.720990 humanloop-0.4.3/humanloop/model/create_experiment_request.pyi
+-rw-r--r--   0        0        0     3199 2023-05-24 22:06:03.721141 humanloop-0.4.3/humanloop/model/create_log_response.py
+-rw-r--r--   0        0        0     3199 2023-05-24 22:06:03.721287 humanloop-0.4.3/humanloop/model/create_log_response.pyi
+-rw-r--r--   0        0        0     4266 2023-05-24 22:06:03.721447 humanloop-0.4.3/humanloop/model/create_project_request.py
+-rw-r--r--   0        0        0     4266 2023-05-24 22:06:03.721584 humanloop-0.4.3/humanloop/model/create_project_request.pyi
+-rw-r--r--   0        0        0     2635 2023-05-24 22:06:03.721725 humanloop-0.4.3/humanloop/model/create_session_response.py
+-rw-r--r--   0        0        0     2635 2023-05-24 22:06:03.721847 humanloop-0.4.3/humanloop/model/create_session_response.pyi
+-rw-r--r--   0        0        0     3232 2023-05-24 22:06:03.722010 humanloop-0.4.3/humanloop/model/create_trace_request.py
+-rw-r--r--   0        0        0     3232 2023-05-24 22:06:03.722170 humanloop-0.4.3/humanloop/model/create_trace_request.pyi
+-rw-r--r--   0        0        0     3329 2023-05-24 22:06:03.722305 humanloop-0.4.3/humanloop/model/create_trace_response.py
+-rw-r--r--   0        0        0     3329 2023-05-24 22:06:03.722448 humanloop-0.4.3/humanloop/model/create_trace_response.pyi
+-rw-r--r--   0        0        0     7455 2023-05-24 22:06:03.722611 humanloop-0.4.3/humanloop/model/data_response.py
+-rw-r--r--   0        0        0     7455 2023-05-24 22:06:03.722795 humanloop-0.4.3/humanloop/model/data_response.pyi
+-rw-r--r--   0        0        0     8998 2023-05-24 22:06:03.722964 humanloop-0.4.3/humanloop/model/experiment_config_response.py
+-rw-r--r--   0        0        0     8998 2023-05-24 22:06:03.723181 humanloop-0.4.3/humanloop/model/experiment_config_response.pyi
+-rw-r--r--   0        0        0    12827 2023-05-24 22:06:03.723386 humanloop-0.4.3/humanloop/model/experiment_response.py
+-rw-r--r--   0        0        0    12827 2023-05-24 22:06:03.723646 humanloop-0.4.3/humanloop/model/experiment_response.pyi
+-rw-r--r--   0        0        0     1376 2023-05-24 22:06:03.723851 humanloop-0.4.3/humanloop/model/experiment_status.py
+-rw-r--r--   0        0        0     1229 2023-05-24 22:06:03.724015 humanloop-0.4.3/humanloop/model/experiment_status.pyi
+-rw-r--r--   0        0        0     1685 2023-05-24 22:06:03.724177 humanloop-0.4.3/humanloop/model/experiments_list_response.py
+-rw-r--r--   0        0        0     1685 2023-05-24 22:06:03.724320 humanloop-0.4.3/humanloop/model/experiments_list_response.pyi
+-rw-r--r--   0        0        0     6681 2023-05-24 22:06:03.724485 humanloop-0.4.3/humanloop/model/feedback.py
+-rw-r--r--   0        0        0     6681 2023-05-24 22:06:03.724632 humanloop-0.4.3/humanloop/model/feedback.pyi
+-rw-r--r--   0        0        0     1463 2023-05-24 22:06:03.724799 humanloop-0.4.3/humanloop/model/feedback_class.py
+-rw-r--r--   0        0        0     1296 2023-05-24 22:06:03.724961 humanloop-0.4.3/humanloop/model/feedback_class.pyi
+-rw-r--r--   0        0        0     3334 2023-05-24 22:06:03.725270 humanloop-0.4.3/humanloop/model/feedback_label_request.py
+-rw-r--r--   0        0        0     3334 2023-05-24 22:06:03.725442 humanloop-0.4.3/humanloop/model/feedback_label_request.pyi
+-rw-r--r--   0        0        0     7189 2023-05-24 22:06:03.725583 humanloop-0.4.3/humanloop/model/feedback_request.py
+-rw-r--r--   0        0        0     7189 2023-05-24 22:06:03.725820 humanloop-0.4.3/humanloop/model/feedback_request.pyi
+-rw-r--r--   0        0        0     7141 2023-05-24 22:06:03.726014 humanloop-0.4.3/humanloop/model/feedback_response.py
+-rw-r--r--   0        0        0     7141 2023-05-24 22:06:03.726184 humanloop-0.4.3/humanloop/model/feedback_response.pyi
+-rw-r--r--   0        0        0     3200 2023-05-24 22:06:03.726345 humanloop-0.4.3/humanloop/model/feedback_submit_request.py
+-rw-r--r--   0        0        0     3200 2023-05-24 22:06:03.726522 humanloop-0.4.3/humanloop/model/feedback_submit_request.pyi
+-rw-r--r--   0        0        0     3210 2023-05-24 22:06:03.726701 humanloop-0.4.3/humanloop/model/feedback_submit_response.py
+-rw-r--r--   0        0        0     3210 2023-05-24 22:06:03.726874 humanloop-0.4.3/humanloop/model/feedback_submit_response.pyi
+-rw-r--r--   0        0        0     1690 2023-05-24 22:06:03.727066 humanloop-0.4.3/humanloop/model/feedback_type.py
+-rw-r--r--   0        0        0     1459 2023-05-24 22:06:03.727243 humanloop-0.4.3/humanloop/model/feedback_type.pyi
+-rw-r--r--   0        0        0     6161 2023-05-24 22:06:03.727420 humanloop-0.4.3/humanloop/model/feedback_type_model.py
+-rw-r--r--   0        0        0     6161 2023-05-24 22:06:03.727586 humanloop-0.4.3/humanloop/model/feedback_type_model.pyi
+-rw-r--r--   0        0        0     6289 2023-05-24 22:06:03.727734 humanloop-0.4.3/humanloop/model/feedback_type_request.py
+-rw-r--r--   0        0        0     6289 2023-05-24 22:06:03.727899 humanloop-0.4.3/humanloop/model/feedback_type_request.pyi
+-rw-r--r--   0        0        0     1659 2023-05-24 22:06:03.728106 humanloop-0.4.3/humanloop/model/feedback_types.py
+-rw-r--r--   0        0        0     1659 2023-05-24 22:06:03.728425 humanloop-0.4.3/humanloop/model/feedback_types.pyi
+-rw-r--r--   0        0        0     4407 2023-05-24 22:06:03.728613 humanloop-0.4.3/humanloop/model/generic_config_request.py
+-rw-r--r--   0        0        0     4238 2023-05-24 22:06:03.728780 humanloop-0.4.3/humanloop/model/generic_config_request.pyi
+-rw-r--r--   0        0        0     6562 2023-05-24 22:06:03.728933 humanloop-0.4.3/humanloop/model/generic_config_response.py
+-rw-r--r--   0        0        0     6562 2023-05-24 22:06:03.729098 humanloop-0.4.3/humanloop/model/generic_config_response.pyi
+-rw-r--r--   0        0        0     9619 2023-05-24 22:06:03.729296 humanloop-0.4.3/humanloop/model/get_model_config_response.py
+-rw-r--r--   0        0        0     9619 2023-05-24 22:06:03.729546 humanloop-0.4.3/humanloop/model/get_model_config_response.pyi
+-rw-r--r--   0        0        0     3611 2023-05-24 22:06:03.729728 humanloop-0.4.3/humanloop/model/http_validation_error.py
+-rw-r--r--   0        0        0     3611 2023-05-24 22:06:03.729880 humanloop-0.4.3/humanloop/model/http_validation_error.pyi
+-rw-r--r--   0        0        0     1667 2023-05-24 22:06:03.730032 humanloop-0.4.3/humanloop/model/label_sentiment.py
+-rw-r--r--   0        0        0     1468 2023-05-24 22:06:03.730188 humanloop-0.4.3/humanloop/model/label_sentiment.pyi
+-rw-r--r--   0        0        0     3156 2023-05-24 22:06:03.730336 humanloop-0.4.3/humanloop/model/log_datapoint_request.py
+-rw-r--r--   0        0        0     3156 2023-05-24 22:06:03.730502 humanloop-0.4.3/humanloop/model/log_datapoint_request.pyi
+-rw-r--r--   0        0        0    17219 2023-05-24 22:06:03.730707 humanloop-0.4.3/humanloop/model/log_model_config_request.py
+-rw-r--r--   0        0        0    17219 2023-05-24 22:06:03.730945 humanloop-0.4.3/humanloop/model/log_model_config_request.pyi
+-rw-r--r--   0        0        0    15844 2023-05-24 22:06:03.731183 humanloop-0.4.3/humanloop/model/log_request.py
+-rw-r--r--   0        0        0    15844 2023-05-24 22:06:03.731400 humanloop-0.4.3/humanloop/model/log_request.pyi
+-rw-r--r--   0        0        0    20160 2023-05-24 22:06:03.731655 humanloop-0.4.3/humanloop/model/log_response.py
+-rw-r--r--   0        0        0    20160 2023-05-24 22:06:03.731908 humanloop-0.4.3/humanloop/model/log_response.pyi
+-rw-r--r--   0        0        0     3205 2023-05-24 22:06:03.732126 humanloop-0.4.3/humanloop/model/logs_log_response.py
+-rw-r--r--   0        0        0     3205 2023-05-24 22:06:03.732274 humanloop-0.4.3/humanloop/model/logs_log_response.pyi
+-rw-r--r--   0        0        0    16246 2023-05-24 22:06:03.732446 humanloop-0.4.3/humanloop/model/model_config_chat_request.py
+-rw-r--r--   0        0        0    16246 2023-05-24 22:06:03.732691 humanloop-0.4.3/humanloop/model/model_config_chat_request.pyi
+-rw-r--r--   0        0        0    15386 2023-05-24 22:06:03.732906 humanloop-0.4.3/humanloop/model/model_config_completion_request.py
+-rw-r--r--   0        0        0    15386 2023-05-24 22:06:03.733108 humanloop-0.4.3/humanloop/model/model_config_completion_request.pyi
+-rw-r--r--   0        0        0    17859 2023-05-24 22:06:03.733276 humanloop-0.4.3/humanloop/model/model_config_response.py
+-rw-r--r--   0        0        0    17859 2023-05-24 22:06:03.733423 humanloop-0.4.3/humanloop/model/model_config_response.pyi
+-rw-r--r--   0        0        0    20554 2023-05-24 22:06:03.733574 humanloop-0.4.3/humanloop/model/model_config_response2.py
+-rw-r--r--   0        0        0    20554 2023-05-24 22:06:03.733716 humanloop-0.4.3/humanloop/model/model_config_response2.pyi
+-rw-r--r--   0        0        0     1460 2023-05-24 22:06:03.733826 humanloop-0.4.3/humanloop/model/model_endpoints.py
+-rw-r--r--   0        0        0     1305 2023-05-24 22:06:03.733948 humanloop-0.4.3/humanloop/model/model_endpoints.pyi
+-rw-r--r--   0        0        0     1695 2023-05-24 22:06:03.734084 humanloop-0.4.3/humanloop/model/model_providers.py
+-rw-r--r--   0        0        0     1468 2023-05-24 22:06:03.734183 humanloop-0.4.3/humanloop/model/model_providers.pyi
+-rw-r--r--   0        0        0     5144 2023-05-24 22:06:03.734269 humanloop-0.4.3/humanloop/model/paginated_data_log_response.py
+-rw-r--r--   0        0        0     5144 2023-05-24 22:06:03.734394 humanloop-0.4.3/humanloop/model/paginated_data_log_response.pyi
+-rw-r--r--   0        0        0     5180 2023-05-24 22:06:03.734507 humanloop-0.4.3/humanloop/model/paginated_data_project_response.py
+-rw-r--r--   0        0        0     5180 2023-05-24 22:06:03.734604 humanloop-0.4.3/humanloop/model/paginated_data_project_response.pyi
+-rw-r--r--   0        0        0     5180 2023-05-24 22:06:03.734706 humanloop-0.4.3/humanloop/model/paginated_data_session_response.py
+-rw-r--r--   0        0        0     5180 2023-05-24 22:06:03.734798 humanloop-0.4.3/humanloop/model/paginated_data_session_response.pyi
+-rw-r--r--   0        0        0     3143 2023-05-24 22:06:03.734891 humanloop-0.4.3/humanloop/model/positive_label.py
+-rw-r--r--   0        0        0     3143 2023-05-24 22:06:03.734994 humanloop-0.4.3/humanloop/model/positive_label.pyi
+-rw-r--r--   0        0        0     8900 2023-05-24 22:06:03.735098 humanloop-0.4.3/humanloop/model/project_config_response.py
+-rw-r--r--   0        0        0     8900 2023-05-24 22:06:03.735217 humanloop-0.4.3/humanloop/model/project_config_response.pyi
+-rw-r--r--   0        0        0    18363 2023-05-24 22:06:03.735353 humanloop-0.4.3/humanloop/model/project_model_config_request.py
+-rw-r--r--   0        0        0    18363 2023-05-24 22:06:03.735479 humanloop-0.4.3/humanloop/model/project_model_config_request.pyi
+-rw-r--r--   0        0        0    23968 2023-05-24 22:06:03.735623 humanloop-0.4.3/humanloop/model/project_model_config_response.py
+-rw-r--r--   0        0        0    23968 2023-05-24 22:06:03.735787 humanloop-0.4.3/humanloop/model/project_model_config_response.pyi
+-rw-r--r--   0        0        0    13895 2023-05-24 22:06:03.735934 humanloop-0.4.3/humanloop/model/project_response.py
+-rw-r--r--   0        0        0    13895 2023-05-24 22:06:03.736095 humanloop-0.4.3/humanloop/model/project_response.pyi
+-rw-r--r--   0        0        0     1471 2023-05-24 22:06:03.736234 humanloop-0.4.3/humanloop/model/project_sort_by.py
+-rw-r--r--   0        0        0     1300 2023-05-24 22:06:03.736456 humanloop-0.4.3/humanloop/model/project_sort_by.pyi
+-rw-r--r--   0        0        0     3795 2023-05-24 22:06:03.736848 humanloop-0.4.3/humanloop/model/project_user_response.py
+-rw-r--r--   0        0        0     3795 2023-05-24 22:06:03.737012 humanloop-0.4.3/humanloop/model/project_user_response.pyi
+-rw-r--r--   0        0        0     1713 2023-05-24 22:06:03.737157 humanloop-0.4.3/humanloop/model/projects_get_configs_response.py
+-rw-r--r--   0        0        0     1713 2023-05-24 22:06:03.737389 humanloop-0.4.3/humanloop/model/projects_get_configs_response.pyi
+-rw-r--r--   0        0        0     1715 2023-05-24 22:06:03.737571 humanloop-0.4.3/humanloop/model/projects_update_feedback_types_request.py
+-rw-r--r--   0        0        0     1715 2023-05-24 22:06:03.737840 humanloop-0.4.3/humanloop/model/projects_update_feedback_types_request.pyi
+-rw-r--r--   0        0        0     4150 2023-05-24 22:06:03.738021 humanloop-0.4.3/humanloop/model/provider_api_keys.py
+-rw-r--r--   0        0        0     4150 2023-05-24 22:06:03.738178 humanloop-0.4.3/humanloop/model/provider_api_keys.pyi
+-rw-r--r--   0        0        0     3113 2023-05-24 22:06:03.738338 humanloop-0.4.3/humanloop/model/session_project_response.py
+-rw-r--r--   0        0        0     3113 2023-05-24 22:06:03.738509 humanloop-0.4.3/humanloop/model/session_project_response.pyi
+-rw-r--r--   0        0        0     6620 2023-05-24 22:06:03.738724 humanloop-0.4.3/humanloop/model/session_response.py
+-rw-r--r--   0        0        0     6620 2023-05-24 22:06:03.738903 humanloop-0.4.3/humanloop/model/session_response.pyi
+-rw-r--r--   0        0        0     1309 2023-05-24 22:06:03.739070 humanloop-0.4.3/humanloop/model/sort_order.py
+-rw-r--r--   0        0        0     1192 2023-05-24 22:06:03.739222 humanloop-0.4.3/humanloop/model/sort_order.pyi
+-rw-r--r--   0        0        0     4889 2023-05-24 22:06:03.739409 humanloop-0.4.3/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py
+-rw-r--r--   0        0        0     4889 2023-05-24 22:06:03.739606 humanloop-0.4.3/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.pyi
+-rw-r--r--   0        0        0     4893 2023-05-24 22:06:03.739757 humanloop-0.4.3/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py
+-rw-r--r--   0        0        0     4893 2023-05-24 22:06:03.739894 humanloop-0.4.3/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.pyi
+-rw-r--r--   0        0        0     4951 2023-05-24 22:06:03.740032 humanloop-0.4.3/humanloop/model/tool_config_request.py
+-rw-r--r--   0        0        0     4788 2023-05-24 22:06:03.740154 humanloop-0.4.3/humanloop/model/tool_config_request.pyi
+-rw-r--r--   0        0        0     7064 2023-05-24 22:06:03.740291 humanloop-0.4.3/humanloop/model/tool_config_response.py
+-rw-r--r--   0        0        0     7064 2023-05-24 22:06:03.740430 humanloop-0.4.3/humanloop/model/tool_config_response.pyi
+-rw-r--r--   0        0        0     4232 2023-05-24 22:06:03.740574 humanloop-0.4.3/humanloop/model/tool_result_response.py
+-rw-r--r--   0        0        0     4232 2023-05-24 22:06:03.740681 humanloop-0.4.3/humanloop/model/tool_result_response.pyi
+-rw-r--r--   0        0        0    13080 2023-05-24 22:06:03.740805 humanloop-0.4.3/humanloop/model/trace_log_request.py
+-rw-r--r--   0        0        0    13080 2023-05-24 22:06:03.740968 humanloop-0.4.3/humanloop/model/trace_log_request.pyi
+-rw-r--r--   0        0        0    19510 2023-05-24 22:06:03.741143 humanloop-0.4.3/humanloop/model/trace_model_config_request.py
+-rw-r--r--   0        0        0    19345 2023-05-24 22:06:03.741282 humanloop-0.4.3/humanloop/model/trace_model_config_request.pyi
+-rw-r--r--   0        0        0     7302 2023-05-24 22:06:03.741393 humanloop-0.4.3/humanloop/model/update_experiment_request.py
+-rw-r--r--   0        0        0     7302 2023-05-24 22:06:03.741496 humanloop-0.4.3/humanloop/model/update_experiment_request.pyi
+-rw-r--r--   0        0        0     5047 2023-05-24 22:06:03.741604 humanloop-0.4.3/humanloop/model/update_project_request.py
+-rw-r--r--   0        0        0     5047 2023-05-24 22:06:03.741696 humanloop-0.4.3/humanloop/model/update_project_request.pyi
+-rw-r--r--   0        0        0     4118 2023-05-24 22:06:03.741793 humanloop-0.4.3/humanloop/model/usage.py
+-rw-r--r--   0        0        0     4118 2023-05-24 22:06:03.741900 humanloop-0.4.3/humanloop/model/usage.pyi
+-rw-r--r--   0        0        0     6805 2023-05-24 22:06:03.742006 humanloop-0.4.3/humanloop/model/validation_error.py
+-rw-r--r--   0        0        0     6805 2023-05-24 22:06:03.742112 humanloop-0.4.3/humanloop/model/validation_error.pyi
+-rw-r--r--   0        0        0     6379 2023-05-24 22:06:03.742226 humanloop-0.4.3/humanloop/models/__init__.py
+-rw-r--r--   0        0        0     1404 2023-05-24 22:06:03.742335 humanloop-0.4.3/humanloop/paths/__init__.py
+-rw-r--r--   0        0        0      285 2023-05-24 22:06:03.742439 humanloop-0.4.3/humanloop/paths/chat/__init__.py
+-rw-r--r--   0        0        0    17428 2023-05-24 22:06:03.742552 humanloop-0.4.3/humanloop/paths/chat/post.py
+-rw-r--r--   0        0        0    17285 2023-05-24 22:06:03.742714 humanloop-0.4.3/humanloop/paths/chat/post.pyi
+-rw-r--r--   0        0        0      302 2023-05-24 22:06:03.742828 humanloop-0.4.3/humanloop/paths/chat_deployed/__init__.py
+-rw-r--r--   0        0        0    16991 2023-05-24 22:06:03.742949 humanloop-0.4.3/humanloop/paths/chat_deployed/post.py
+-rw-r--r--   0        0        0    16848 2023-05-24 22:06:03.743075 humanloop-0.4.3/humanloop/paths/chat_deployed/post.pyi
+-rw-r--r--   0        0        0      306 2023-05-24 22:06:03.743190 humanloop-0.4.3/humanloop/paths/chat_experiment/__init__.py
+-rw-r--r--   0        0        0    17434 2023-05-24 22:06:03.743305 humanloop-0.4.3/humanloop/paths/chat_experiment/post.py
+-rw-r--r--   0        0        0    17291 2023-05-24 22:06:03.743442 humanloop-0.4.3/humanloop/paths/chat_experiment/post.pyi
+-rw-r--r--   0        0        0      309 2023-05-24 22:06:03.743557 humanloop-0.4.3/humanloop/paths/chat_model_config/__init__.py
+-rw-r--r--   0        0        0    17609 2023-05-24 22:06:03.743675 humanloop-0.4.3/humanloop/paths/chat_model_config/post.py
+-rw-r--r--   0        0        0    17466 2023-05-24 22:06:03.743800 humanloop-0.4.3/humanloop/paths/chat_model_config/post.pyi
+-rw-r--r--   0        0        0      297 2023-05-24 22:06:03.743915 humanloop-0.4.3/humanloop/paths/completion/__init__.py
+-rw-r--r--   0        0        0    17744 2023-05-24 22:06:03.744028 humanloop-0.4.3/humanloop/paths/completion/post.py
+-rw-r--r--   0        0        0    17601 2023-05-24 22:06:03.744151 humanloop-0.4.3/humanloop/paths/completion/post.pyi
+-rw-r--r--   0        0        0      314 2023-05-24 22:06:03.744266 humanloop-0.4.3/humanloop/paths/completion_deployed/__init__.py
+-rw-r--r--   0        0        0    17247 2023-05-24 22:06:03.744375 humanloop-0.4.3/humanloop/paths/completion_deployed/post.py
+-rw-r--r--   0        0        0    17104 2023-05-24 22:06:03.744497 humanloop-0.4.3/humanloop/paths/completion_deployed/post.pyi
+-rw-r--r--   0        0        0      318 2023-05-24 22:06:03.744603 humanloop-0.4.3/humanloop/paths/completion_experiment/__init__.py
+-rw-r--r--   0        0        0    17690 2023-05-24 22:06:03.744719 humanloop-0.4.3/humanloop/paths/completion_experiment/post.py
+-rw-r--r--   0        0        0    17547 2023-05-24 22:06:03.744839 humanloop-0.4.3/humanloop/paths/completion_experiment/post.pyi
+-rw-r--r--   0        0        0      321 2023-05-24 22:06:03.744954 humanloop-0.4.3/humanloop/paths/completion_model_config/__init__.py
+-rw-r--r--   0        0        0    17865 2023-05-24 22:06:03.745072 humanloop-0.4.3/humanloop/paths/completion_model_config/post.py
+-rw-r--r--   0        0        0    17722 2023-05-24 22:06:03.745197 humanloop-0.4.3/humanloop/paths/completion_model_config/post.pyi
+-rw-r--r--   0        0        0      327 2023-05-24 22:06:03.745313 humanloop-0.4.3/humanloop/paths/experiments_experiment_id/__init__.py
+-rw-r--r--   0        0        0    11995 2023-05-24 22:06:03.745433 humanloop-0.4.3/humanloop/paths/experiments_experiment_id/delete.py
+-rw-r--r--   0        0        0    11852 2023-05-24 22:06:03.745596 humanloop-0.4.3/humanloop/paths/experiments_experiment_id/delete.pyi
+-rw-r--r--   0        0        0    17043 2023-05-24 22:06:03.745746 humanloop-0.4.3/humanloop/paths/experiments_experiment_id/patch.py
+-rw-r--r--   0        0        0    16900 2023-05-24 22:06:03.745904 humanloop-0.4.3/humanloop/paths/experiments_experiment_id/patch.pyi
+-rw-r--r--   0        0        0      352 2023-05-24 22:06:03.746050 humanloop-0.4.3/humanloop/paths/experiments_experiment_id_model_config/__init__.py
+-rw-r--r--   0        0        0    12496 2023-05-24 22:06:03.746196 humanloop-0.4.3/humanloop/paths/experiments_experiment_id_model_config/get.py
+-rw-r--r--   0        0        0    12353 2023-05-24 22:06:03.746363 humanloop-0.4.3/humanloop/paths/experiments_experiment_id_model_config/get.pyi
+-rw-r--r--   0        0        0      293 2023-05-24 22:06:03.746521 humanloop-0.4.3/humanloop/paths/feedback/__init__.py
+-rw-r--r--   0        0        0    15089 2023-05-24 22:06:03.746635 humanloop-0.4.3/humanloop/paths/feedback/post.py
+-rw-r--r--   0        0        0    14946 2023-05-24 22:06:03.746751 humanloop-0.4.3/humanloop/paths/feedback/post.pyi
+-rw-r--r--   0        0        0      285 2023-05-24 22:06:03.746882 humanloop-0.4.3/humanloop/paths/logs/__init__.py
+-rw-r--r--   0        0        0    20891 2023-05-24 22:06:03.746991 humanloop-0.4.3/humanloop/paths/logs/post.py
+-rw-r--r--   0        0        0    20748 2023-05-24 22:06:03.747118 humanloop-0.4.3/humanloop/paths/logs/post.pyi
+-rw-r--r--   0        0        0      302 2023-05-24 22:06:03.747236 humanloop-0.4.3/humanloop/paths/model_configs/__init__.py
+-rw-r--r--   0        0        0    20266 2023-05-24 22:06:03.747345 humanloop-0.4.3/humanloop/paths/model_configs/post.py
+-rw-r--r--   0        0        0    20123 2023-05-24 22:06:03.747469 humanloop-0.4.3/humanloop/paths/model_configs/post.pyi
+-rw-r--r--   0        0        0      308 2023-05-24 22:06:03.747607 humanloop-0.4.3/humanloop/paths/model_configs_id/__init__.py
+-rw-r--r--   0        0        0    12023 2023-05-24 22:06:03.747716 humanloop-0.4.3/humanloop/paths/model_configs_id/get.py
+-rw-r--r--   0        0        0    11880 2023-05-24 22:06:03.747848 humanloop-0.4.3/humanloop/paths/model_configs_id/get.pyi
+-rw-r--r--   0        0        0      293 2023-05-24 22:06:03.748006 humanloop-0.4.3/humanloop/paths/projects/__init__.py
+-rw-r--r--   0        0        0    20518 2023-05-24 22:06:03.748148 humanloop-0.4.3/humanloop/paths/projects/get.py
+-rw-r--r--   0        0        0    20375 2023-05-24 22:06:03.748310 humanloop-0.4.3/humanloop/paths/projects/get.pyi
+-rw-r--r--   0        0        0    13007 2023-05-24 22:06:03.748466 humanloop-0.4.3/humanloop/paths/projects/post.py
+-rw-r--r--   0        0        0    12864 2023-05-24 22:06:03.748695 humanloop-0.4.3/humanloop/paths/projects/post.pyi
+-rw-r--r--   0        0        0      299 2023-05-24 22:06:03.748985 humanloop-0.4.3/humanloop/paths/projects_id/__init__.py
+-rw-r--r--   0        0        0    11979 2023-05-24 22:06:03.749157 humanloop-0.4.3/humanloop/paths/projects_id/get.py
+-rw-r--r--   0        0        0    11836 2023-05-24 22:06:03.749353 humanloop-0.4.3/humanloop/paths/projects_id/get.pyi
+-rw-r--r--   0        0        0    16066 2023-05-24 22:06:03.749512 humanloop-0.4.3/humanloop/paths/projects_id/patch.py
+-rw-r--r--   0        0        0    15923 2023-05-24 22:06:03.749708 humanloop-0.4.3/humanloop/paths/projects_id/patch.pyi
+-rw-r--r--   0        0        0      326 2023-05-24 22:06:03.749882 humanloop-0.4.3/humanloop/paths/projects_id_active_config/__init__.py
+-rw-r--r--   0        0        0    12298 2023-05-24 22:06:03.750004 humanloop-0.4.3/humanloop/paths/projects_id_active_config/delete.py
+-rw-r--r--   0        0        0    12155 2023-05-24 22:06:03.750137 humanloop-0.4.3/humanloop/paths/projects_id_active_config/delete.pyi
+-rw-r--r--   0        0        0    12148 2023-05-24 22:06:03.750271 humanloop-0.4.3/humanloop/paths/projects_id_active_config/get.py
+-rw-r--r--   0        0        0    12005 2023-05-24 22:06:03.750392 humanloop-0.4.3/humanloop/paths/projects_id_active_config/get.pyi
+-rw-r--r--   0        0        0      334 2023-05-24 22:06:03.750516 humanloop-0.4.3/humanloop/paths/projects_id_active_experiment/__init__.py
+-rw-r--r--   0        0        0    12306 2023-05-24 22:06:03.750628 humanloop-0.4.3/humanloop/paths/projects_id_active_experiment/delete.py
+-rw-r--r--   0        0        0    12163 2023-05-24 22:06:03.750767 humanloop-0.4.3/humanloop/paths/projects_id_active_experiment/delete.pyi
+-rw-r--r--   0        0        0      315 2023-05-24 22:06:03.750894 humanloop-0.4.3/humanloop/paths/projects_id_configs/__init__.py
+-rw-r--r--   0        0        0    12182 2023-05-24 22:06:03.751001 humanloop-0.4.3/humanloop/paths/projects_id_configs/get.py
+-rw-r--r--   0        0        0    12039 2023-05-24 22:06:03.751129 humanloop-0.4.3/humanloop/paths/projects_id_configs/get.pyi
+-rw-r--r--   0        0        0      313 2023-05-24 22:06:03.751265 humanloop-0.4.3/humanloop/paths/projects_id_export/__init__.py
+-rw-r--r--   0        0        0    15728 2023-05-24 22:06:03.751382 humanloop-0.4.3/humanloop/paths/projects_id_export/post.py
+-rw-r--r--   0        0        0    15585 2023-05-24 22:06:03.751582 humanloop-0.4.3/humanloop/paths/projects_id_export/post.pyi
+-rw-r--r--   0        0        0      328 2023-05-24 22:06:03.751786 humanloop-0.4.3/humanloop/paths/projects_id_feedback_types/__init__.py
+-rw-r--r--   0        0        0    14798 2023-05-24 22:06:03.751939 humanloop-0.4.3/humanloop/paths/projects_id_feedback_types/patch.py
+-rw-r--r--   0        0        0    14655 2023-05-24 22:06:03.752106 humanloop-0.4.3/humanloop/paths/projects_id_feedback_types/patch.pyi
+-rw-r--r--   0        0        0      339 2023-05-24 22:06:03.752249 humanloop-0.4.3/humanloop/paths/projects_project_id_experiments/__init__.py
+-rw-r--r--   0        0        0    12256 2023-05-24 22:06:03.752365 humanloop-0.4.3/humanloop/paths/projects_project_id_experiments/get.py
+-rw-r--r--   0        0        0    12113 2023-05-24 22:06:03.752514 humanloop-0.4.3/humanloop/paths/projects_project_id_experiments/get.pyi
+-rw-r--r--   0        0        0    16250 2023-05-24 22:06:03.752654 humanloop-0.4.3/humanloop/paths/projects_project_id_experiments/post.py
+-rw-r--r--   0        0        0    16107 2023-05-24 22:06:03.752805 humanloop-0.4.3/humanloop/paths/projects_project_id_experiments/post.pyi
+-rw-r--r--   0        0        0      293 2023-05-24 22:06:03.752947 humanloop-0.4.3/humanloop/paths/sessions/__init__.py
+-rw-r--r--   0        0        0    14112 2023-05-24 22:06:03.753066 humanloop-0.4.3/humanloop/paths/sessions/get.py
+-rw-r--r--   0        0        0    13969 2023-05-24 22:06:03.753213 humanloop-0.4.3/humanloop/paths/sessions/get.pyi
+-rw-r--r--   0        0        0     9192 2023-05-24 22:06:03.753373 humanloop-0.4.3/humanloop/paths/sessions/post.py
+-rw-r--r--   0        0        0     9079 2023-05-24 22:06:03.753520 humanloop-0.4.3/humanloop/paths/sessions/post.pyi
+-rw-r--r--   0        0        0      299 2023-05-24 22:06:03.753632 humanloop-0.4.3/humanloop/paths/sessions_id/__init__.py
+-rw-r--r--   0        0        0    11979 2023-05-24 22:06:03.753726 humanloop-0.4.3/humanloop/paths/sessions_id/get.py
+-rw-r--r--   0        0        0    11836 2023-05-24 22:06:03.753835 humanloop-0.4.3/humanloop/paths/sessions_id/get.pyi
+-rw-r--r--   0        0        0      289 2023-05-24 22:06:03.753950 humanloop-0.4.3/humanloop/paths/traces/__init__.py
+-rw-r--r--   0        0        0    12450 2023-05-24 22:06:03.754045 humanloop-0.4.3/humanloop/paths/traces/post.py
+-rw-r--r--   0        0        0    12307 2023-05-24 22:06:03.754172 humanloop-0.4.3/humanloop/paths/traces/post.pyi
+-rw-r--r--   0        0        0     1011 2023-05-24 22:06:03.754339 humanloop-0.4.3/humanloop/request_after_hook.py
+-rw-r--r--   0        0        0     1783 2023-05-18 18:32:32.791241 humanloop-0.4.3/humanloop/request_before_hook.py
+-rw-r--r--   0        0        0    11329 2023-05-24 22:06:03.754495 humanloop-0.4.3/humanloop/rest.py
+-rw-r--r--   0        0        0    95913 2023-05-24 22:06:03.754835 humanloop-0.4.3/humanloop/schemas.py
+-rw-r--r--   0        0        0        0 2023-05-24 22:06:03.755019 humanloop-0.4.3/humanloop/type/__init__.py
+-rw-r--r--   0        0        0     1414 2023-05-24 22:06:03.755158 humanloop-0.4.3/humanloop/type/agent_config_request.py
+-rw-r--r--   0        0        0     1608 2023-05-24 22:06:03.755284 humanloop-0.4.3/humanloop/type/agent_config_response.py
+-rw-r--r--   0        0        0     1408 2023-05-24 22:06:03.755421 humanloop-0.4.3/humanloop/type/base_metric_response.py
+-rw-r--r--   0        0        0     1062 2023-05-24 22:06:03.755561 humanloop-0.4.3/humanloop/type/categorical_feedback_label.py
+-rw-r--r--   0        0        0     2183 2023-05-24 22:06:03.755696 humanloop-0.4.3/humanloop/type/chat_data_response.py
+-rw-r--r--   0        0        0     1990 2023-05-24 22:06:03.755854 humanloop-0.4.3/humanloop/type/chat_deployed_request.py
+-rw-r--r--   0        0        0     2235 2023-05-24 22:06:03.756004 humanloop-0.4.3/humanloop/type/chat_experiment_request.py
+-rw-r--r--   0        0        0      919 2023-05-24 22:06:03.756134 humanloop-0.4.3/humanloop/type/chat_message.py
+-rw-r--r--   0        0        0     2104 2023-05-24 22:06:03.756259 humanloop-0.4.3/humanloop/type/chat_model_config_request.py
+-rw-r--r--   0        0        0     2130 2023-05-24 22:06:03.756382 humanloop-0.4.3/humanloop/type/chat_request.py
+-rw-r--r--   0        0        0     1818 2023-05-24 22:06:03.756494 humanloop-0.4.3/humanloop/type/chat_response.py
+-rw-r--r--   0        0        0      711 2023-05-24 22:06:03.756615 humanloop-0.4.3/humanloop/type/chat_role.py
+-rw-r--r--   0        0        0     2095 2023-05-24 22:06:03.756732 humanloop-0.4.3/humanloop/type/completion_deployed_request.py
+-rw-r--r--   0        0        0     2343 2023-05-24 22:06:03.756847 humanloop-0.4.3/humanloop/type/completion_experiment_request.py
+-rw-r--r--   0        0        0     2209 2023-05-24 22:06:03.756957 humanloop-0.4.3/humanloop/type/completion_model_config_request.py
+-rw-r--r--   0        0        0     2239 2023-05-24 22:06:03.757075 humanloop-0.4.3/humanloop/type/completion_request.py
+-rw-r--r--   0        0        0     1864 2023-05-24 22:06:03.757193 humanloop-0.4.3/humanloop/type/completion_response.py
+-rw-r--r--   0        0        0     1054 2023-05-24 22:06:03.757293 humanloop-0.4.3/humanloop/type/config_response.py
+-rw-r--r--   0        0        0      719 2023-05-24 22:06:03.757420 humanloop-0.4.3/humanloop/type/config_type.py
+-rw-r--r--   0        0        0     1362 2023-05-24 22:06:03.757542 humanloop-0.4.3/humanloop/type/create_experiment_request.py
+-rw-r--r--   0        0        0     1024 2023-05-24 22:06:03.757663 humanloop-0.4.3/humanloop/type/create_log_response.py
+-rw-r--r--   0        0        0     1066 2023-05-24 22:06:03.757780 humanloop-0.4.3/humanloop/type/create_project_request.py
+-rw-r--r--   0        0        0      942 2023-05-24 22:06:03.757897 humanloop-0.4.3/humanloop/type/create_session_response.py
+-rw-r--r--   0        0        0     1045 2023-05-24 22:06:03.757998 humanloop-0.4.3/humanloop/type/create_trace_request.py
+-rw-r--r--   0        0        0      998 2023-05-24 22:06:03.758100 humanloop-0.4.3/humanloop/type/create_trace_response.py
+-rw-r--r--   0        0        0     2013 2023-05-24 22:06:03.758199 humanloop-0.4.3/humanloop/type/data_response.py
+-rw-r--r--   0        0        0     1677 2023-05-24 22:06:03.758296 humanloop-0.4.3/humanloop/type/experiment_config_response.py
+-rw-r--r--   0        0        0     1788 2023-05-24 22:06:03.758394 humanloop-0.4.3/humanloop/type/experiment_response.py
+-rw-r--r--   0        0        0      718 2023-05-24 22:06:03.758484 humanloop-0.4.3/humanloop/type/experiment_status.py
+-rw-r--r--   0        0        0      785 2023-05-24 22:06:03.758608 humanloop-0.4.3/humanloop/type/experiments_list_response.py
+-rw-r--r--   0        0        0     1449 2023-05-24 22:06:03.758837 humanloop-0.4.3/humanloop/type/feedback.py
+-rw-r--r--   0        0        0      719 2023-05-24 22:06:03.759458 humanloop-0.4.3/humanloop/type/feedback_class.py
+-rw-r--r--   0        0        0      970 2023-05-24 22:06:03.759997 humanloop-0.4.3/humanloop/type/feedback_label_request.py
+-rw-r--r--   0        0        0     1546 2023-05-24 22:06:03.762133 humanloop-0.4.3/humanloop/type/feedback_request.py
+-rw-r--r--   0        0        0     1578 2023-05-24 22:06:03.762307 humanloop-0.4.3/humanloop/type/feedback_response.py
+-rw-r--r--   0        0        0      804 2023-05-24 22:06:03.762411 humanloop-0.4.3/humanloop/type/feedback_submit_request.py
+-rw-r--r--   0        0        0      809 2023-05-24 22:06:03.762504 humanloop-0.4.3/humanloop/type/feedback_submit_response.py
+-rw-r--r--   0        0        0      738 2023-05-24 22:06:03.762594 humanloop-0.4.3/humanloop/type/feedback_type.py
+-rw-r--r--   0        0        0     1307 2023-05-24 22:06:03.762689 humanloop-0.4.3/humanloop/type/feedback_type_model.py
+-rw-r--r--   0        0        0     1541 2023-05-24 22:06:03.762785 humanloop-0.4.3/humanloop/type/feedback_type_request.py
+-rw-r--r--   0        0        0      773 2023-05-24 22:06:03.762880 humanloop-0.4.3/humanloop/type/feedback_types.py
+-rw-r--r--   0        0        0     1064 2023-05-24 22:06:03.762973 humanloop-0.4.3/humanloop/type/generic_config_request.py
+-rw-r--r--   0        0        0     1262 2023-05-24 22:06:03.763058 humanloop-0.4.3/humanloop/type/generic_config_response.py
+-rw-r--r--   0        0        0     1900 2023-05-24 22:06:03.763147 humanloop-0.4.3/humanloop/type/get_model_config_response.py
+-rw-r--r--   0        0        0      972 2023-05-24 22:06:03.763244 humanloop-0.4.3/humanloop/type/http_validation_error.py
+-rw-r--r--   0        0        0      730 2023-05-24 22:06:03.763332 humanloop-0.4.3/humanloop/type/label_sentiment.py
+-rw-r--r--   0        0        0      782 2023-05-24 22:06:03.763422 humanloop-0.4.3/humanloop/type/log_datapoint_request.py
+-rw-r--r--   0        0        0     3033 2023-05-24 22:06:03.763511 humanloop-0.4.3/humanloop/type/log_model_config_request.py
+-rw-r--r--   0        0        0     2652 2023-05-24 22:06:03.763609 humanloop-0.4.3/humanloop/type/log_request.py
+-rw-r--r--   0        0        0     2961 2023-05-24 22:06:03.763734 humanloop-0.4.3/humanloop/type/log_response.py
+-rw-r--r--   0        0        0      807 2023-05-24 22:06:03.763827 humanloop-0.4.3/humanloop/type/logs_log_response.py
+-rw-r--r--   0        0        0     2820 2023-05-24 22:06:03.763975 humanloop-0.4.3/humanloop/type/model_config_chat_request.py
+-rw-r--r--   0        0        0     2713 2023-05-24 22:06:03.764081 humanloop-0.4.3/humanloop/type/model_config_completion_request.py
+-rw-r--r--   0        0        0     3160 2023-05-24 22:06:03.764178 humanloop-0.4.3/humanloop/type/model_config_response.py
+-rw-r--r--   0        0        0     3281 2023-05-24 22:06:03.764276 humanloop-0.4.3/humanloop/type/model_config_response2.py
+-rw-r--r--   0        0        0      714 2023-05-24 22:06:03.764381 humanloop-0.4.3/humanloop/type/model_endpoints.py
+-rw-r--r--   0        0        0      738 2023-05-24 22:06:03.764475 humanloop-0.4.3/humanloop/type/model_providers.py
+-rw-r--r--   0        0        0     1032 2023-05-24 22:06:03.764575 humanloop-0.4.3/humanloop/type/paginated_data_log_response.py
+-rw-r--r--   0        0        0     1064 2023-05-24 22:06:03.764679 humanloop-0.4.3/humanloop/type/paginated_data_project_response.py
+-rw-r--r--   0        0        0     1064 2023-05-24 22:06:03.764787 humanloop-0.4.3/humanloop/type/paginated_data_session_response.py
+-rw-r--r--   0        0        0      871 2023-05-24 22:06:03.764902 humanloop-0.4.3/humanloop/type/positive_label.py
+-rw-r--r--   0        0        0     1820 2023-05-24 22:06:03.765015 humanloop-0.4.3/humanloop/type/project_config_response.py
+-rw-r--r--   0        0        0     3410 2023-05-24 22:06:03.765111 humanloop-0.4.3/humanloop/type/project_model_config_request.py
+-rw-r--r--   0        0        0     4053 2023-05-24 22:06:03.765205 humanloop-0.4.3/humanloop/type/project_model_config_response.py
+-rw-r--r--   0        0        0     2032 2023-05-24 22:06:03.765293 humanloop-0.4.3/humanloop/type/project_response.py
+-rw-r--r--   0        0        0      721 2023-05-24 22:06:03.765388 humanloop-0.4.3/humanloop/type/project_sort_by.py
+-rw-r--r--   0        0        0     1022 2023-05-24 22:06:03.765485 humanloop-0.4.3/humanloop/type/project_user_response.py
+-rw-r--r--   0        0        0      798 2023-05-24 22:06:03.765580 humanloop-0.4.3/humanloop/type/projects_get_configs_response.py
+-rw-r--r--   0        0        0      800 2023-05-24 22:06:03.765682 humanloop-0.4.3/humanloop/type/projects_update_feedback_types_request.py
+-rw-r--r--   0        0        0      917 2023-05-24 22:06:03.765798 humanloop-0.4.3/humanloop/type/provider_api_keys.py
+-rw-r--r--   0        0        0      985 2023-05-24 22:06:03.765927 humanloop-0.4.3/humanloop/type/session_project_response.py
+-rw-r--r--   0        0        0     1442 2023-05-24 22:06:03.766058 humanloop-0.4.3/humanloop/type/session_response.py
+-rw-r--r--   0        0        0      696 2023-05-24 22:06:03.766171 humanloop-0.4.3/humanloop/type/sort_order.py
+-rw-r--r--   0        0        0     1241 2023-05-24 22:06:03.766286 humanloop-0.4.3/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py
+-rw-r--r--   0        0        0     1251 2023-05-24 22:06:03.766402 humanloop-0.4.3/humanloop/type/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py
+-rw-r--r--   0        0        0     1066 2023-05-24 22:06:03.766520 humanloop-0.4.3/humanloop/type/tool_config_request.py
+-rw-r--r--   0        0        0     1295 2023-05-24 22:06:03.766635 humanloop-0.4.3/humanloop/type/tool_config_response.py
+-rw-r--r--   0        0        0      930 2023-05-24 22:06:03.766746 humanloop-0.4.3/humanloop/type/tool_result_response.py
+-rw-r--r--   0        0        0     2427 2023-05-24 22:06:03.766879 humanloop-0.4.3/humanloop/type/trace_log_request.py
+-rw-r--r--   0        0        0     3095 2023-05-24 22:06:03.767004 humanloop-0.4.3/humanloop/type/trace_model_config_request.py
+-rw-r--r--   0        0        0     1361 2023-05-24 22:06:03.767116 humanloop-0.4.3/humanloop/type/update_experiment_request.py
+-rw-r--r--   0        0        0     1434 2023-05-24 22:06:03.767212 humanloop-0.4.3/humanloop/type/update_project_request.py
+-rw-r--r--   0        0        0     1042 2023-05-24 22:06:03.767315 humanloop-0.4.3/humanloop/type/usage.py
+-rw-r--r--   0        0        0      951 2023-05-24 22:06:03.767416 humanloop-0.4.3/humanloop/type/validation_error.py
+-rw-r--r--   0        0        0      868 2023-05-24 22:06:03.767517 humanloop-0.4.3/humanloop/type_util.py
+-rw-r--r--   0        0        0     3165 2023-05-24 22:06:03.767629 humanloop-0.4.3/humanloop/validation_metadata.py
+-rw-r--r--   0        0        0      714 2023-05-24 22:06:03.768046 humanloop-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     9366 1970-01-01 00:00:00.000000 humanloop-0.4.3/PKG-INFO
```

### Comparing `humanloop-0.4.2/LICENSE` & `humanloop-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/README.md` & `humanloop-0.4.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# humanloop@0.4.2
+# humanloop@0.4.3
 
 
 ## Requirements
 
 Python >=3.7
 
 ## Installing
 
 ```sh
-pip install humanloop==0.4.2
+pip install humanloop==0.4.3
 ```
 
 ## Getting Started
 
 ```python
 from pprint import pprint
 from humanloop import Humanloop, ApiException
```

### Comparing `humanloop-0.4.2/humanloop/__init__.py` & `humanloop-0.4.3/humanloop/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The Humanloop API allows you to interact with Humanloop from your product or service.  You can do this through HTTP requests from any language or via our official Python SDK.  To install the official Python SDK, run the following command:  ```bash pip install humanloop ```  ---  Guides and further details about key concepts can be found in [our docs](https://humanloop.gitbook.io/humanloop-docs/).
 
     The version of the OpenAPI document: 4.0.0
     Generated by: https://konfigthis.com
 """
 
-__version__ = "0.4.2"
+__version__ = "0.4.3"
 
 # import ApiClient
 from humanloop.api_client import ApiClient
 
 # import Configuration
 from humanloop.configuration import Configuration
```

### Comparing `humanloop-0.4.2/humanloop/api_client.py` & `humanloop-0.4.3/humanloop/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2759,15 +2759,15 @@
 0000ac60: 6164 6572 5f6e 616d 655d 203d 2068 6561  ader_name] = hea
 0000ac70: 6465 725f 7661 6c75 650a 2020 2020 2020  der_value.      
 0000ac80: 2020 7365 6c66 2e63 6f6f 6b69 6520 3d20    self.cookie = 
 0000ac90: 636f 6f6b 6965 0a20 2020 2020 2020 2023  cookie.        #
 0000aca0: 2053 6574 2064 6566 6175 6c74 2055 7365   Set default Use
 0000acb0: 722d 4167 656e 742e 0a20 2020 2020 2020  r-Agent..       
 0000acc0: 2073 656c 662e 7573 6572 5f61 6765 6e74   self.user_agent
-0000acd0: 203d 2027 4b6f 6e66 6967 2f30 2e34 2e32   = 'Konfig/0.4.2
+0000acd0: 203d 2027 4b6f 6e66 6967 2f30 2e34 2e33   = 'Konfig/0.4.3
 0000ace0: 2f70 7974 686f 6e27 0a0a 2020 2020 6465  /python'..    de
 0000acf0: 6620 5f5f 656e 7465 725f 5f28 7365 6c66  f __enter__(self
 0000ad00: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
 0000ad10: 6e20 7365 6c66 0a0a 2020 2020 6465 6620  n self..    def 
 0000ad20: 5f5f 6578 6974 5f5f 2873 656c 662c 2065  __exit__(self, e
 0000ad30: 7863 5f74 7970 652c 2065 7863 5f76 616c  xc_type, exc_val
 0000ad40: 7565 2c20 7472 6163 6562 6163 6b29 3a0a  ue, traceback):.
```

### Comparing `humanloop-0.4.2/humanloop/api_response.py` & `humanloop-0.4.3/humanloop/api_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/apis/path_to_api.py` & `humanloop-0.4.3/humanloop/apis/path_to_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,31 +9,27 @@
 from humanloop.apis.paths.chat_deployed import ChatDeployed
 from humanloop.apis.paths.chat_experiment import ChatExperiment
 from humanloop.apis.paths.chat_model_config import ChatModelConfig
 from humanloop.apis.paths.logs import Logs
 from humanloop.apis.paths.feedback import Feedback
 from humanloop.apis.paths.projects import Projects
 from humanloop.apis.paths.projects_id import ProjectsId
-from humanloop.apis.paths.projects_id_model_configs import ProjectsIdModelConfigs
-from humanloop.apis.paths.projects_id_model_config import ProjectsIdModelConfig
-from humanloop.apis.paths.projects_id_active_model_config import ProjectsIdActiveModelConfig
+from humanloop.apis.paths.projects_id_configs import ProjectsIdConfigs
+from humanloop.apis.paths.projects_id_active_config import ProjectsIdActiveConfig
 from humanloop.apis.paths.projects_id_active_experiment import ProjectsIdActiveExperiment
 from humanloop.apis.paths.projects_id_feedback_types import ProjectsIdFeedbackTypes
 from humanloop.apis.paths.projects_id_export import ProjectsIdExport
-from humanloop.apis.paths.apps import Apps
-from humanloop.apis.paths.apps_id import AppsId
-from humanloop.apis.paths.apps_id_sessions import AppsIdSessions
-from humanloop.apis.paths.sessions import Sessions
-from humanloop.apis.paths.sessions_id import SessionsId
-from humanloop.apis.paths.sessions_id_events import SessionsIdEvents
 from humanloop.apis.paths.model_configs import ModelConfigs
 from humanloop.apis.paths.model_configs_id import ModelConfigsId
 from humanloop.apis.paths.projects_project_id_experiments import ProjectsProjectIdExperiments
 from humanloop.apis.paths.experiments_experiment_id import ExperimentsExperimentId
 from humanloop.apis.paths.experiments_experiment_id_model_config import ExperimentsExperimentIdModelConfig
+from humanloop.apis.paths.sessions import Sessions
+from humanloop.apis.paths.sessions_id import SessionsId
+from humanloop.apis.paths.traces import Traces
 
 PathToApi = typing_extensions.TypedDict(
     'PathToApi',
     {
         PathValues.COMPLETION: Completion,
         PathValues.COMPLETIONDEPLOYED: CompletionDeployed,
         PathValues.COMPLETIONEXPERIMENT: CompletionExperiment,
@@ -42,31 +38,27 @@
         PathValues.CHATDEPLOYED: ChatDeployed,
         PathValues.CHATEXPERIMENT: ChatExperiment,
         PathValues.CHATMODELCONFIG: ChatModelConfig,
         PathValues.LOGS: Logs,
         PathValues.FEEDBACK: Feedback,
         PathValues.PROJECTS: Projects,
         PathValues.PROJECTS_ID: ProjectsId,
-        PathValues.PROJECTS_ID_MODELCONFIGS: ProjectsIdModelConfigs,
-        PathValues.PROJECTS_ID_MODELCONFIG: ProjectsIdModelConfig,
-        PathValues.PROJECTS_ID_ACTIVEMODELCONFIG: ProjectsIdActiveModelConfig,
+        PathValues.PROJECTS_ID_CONFIGS: ProjectsIdConfigs,
+        PathValues.PROJECTS_ID_ACTIVECONFIG: ProjectsIdActiveConfig,
         PathValues.PROJECTS_ID_ACTIVEEXPERIMENT: ProjectsIdActiveExperiment,
         PathValues.PROJECTS_ID_FEEDBACKTYPES: ProjectsIdFeedbackTypes,
         PathValues.PROJECTS_ID_EXPORT: ProjectsIdExport,
-        PathValues.APPS: Apps,
-        PathValues.APPS_ID: AppsId,
-        PathValues.APPS_ID_SESSIONS: AppsIdSessions,
-        PathValues.SESSIONS: Sessions,
-        PathValues.SESSIONS_ID: SessionsId,
-        PathValues.SESSIONS_ID_EVENTS: SessionsIdEvents,
         PathValues.MODELCONFIGS: ModelConfigs,
         PathValues.MODELCONFIGS_ID: ModelConfigsId,
         PathValues.PROJECTS_PROJECT_ID_EXPERIMENTS: ProjectsProjectIdExperiments,
         PathValues.EXPERIMENTS_EXPERIMENT_ID: ExperimentsExperimentId,
         PathValues.EXPERIMENTS_EXPERIMENT_ID_MODELCONFIG: ExperimentsExperimentIdModelConfig,
+        PathValues.SESSIONS: Sessions,
+        PathValues.SESSIONS_ID: SessionsId,
+        PathValues.TRACES: Traces,
     }
 )
 
 path_to_api = PathToApi(
     {
         PathValues.COMPLETION: Completion,
         PathValues.COMPLETIONDEPLOYED: CompletionDeployed,
@@ -76,26 +68,22 @@
         PathValues.CHATDEPLOYED: ChatDeployed,
         PathValues.CHATEXPERIMENT: ChatExperiment,
         PathValues.CHATMODELCONFIG: ChatModelConfig,
         PathValues.LOGS: Logs,
         PathValues.FEEDBACK: Feedback,
         PathValues.PROJECTS: Projects,
         PathValues.PROJECTS_ID: ProjectsId,
-        PathValues.PROJECTS_ID_MODELCONFIGS: ProjectsIdModelConfigs,
-        PathValues.PROJECTS_ID_MODELCONFIG: ProjectsIdModelConfig,
-        PathValues.PROJECTS_ID_ACTIVEMODELCONFIG: ProjectsIdActiveModelConfig,
+        PathValues.PROJECTS_ID_CONFIGS: ProjectsIdConfigs,
+        PathValues.PROJECTS_ID_ACTIVECONFIG: ProjectsIdActiveConfig,
         PathValues.PROJECTS_ID_ACTIVEEXPERIMENT: ProjectsIdActiveExperiment,
         PathValues.PROJECTS_ID_FEEDBACKTYPES: ProjectsIdFeedbackTypes,
         PathValues.PROJECTS_ID_EXPORT: ProjectsIdExport,
-        PathValues.APPS: Apps,
-        PathValues.APPS_ID: AppsId,
-        PathValues.APPS_ID_SESSIONS: AppsIdSessions,
-        PathValues.SESSIONS: Sessions,
-        PathValues.SESSIONS_ID: SessionsId,
-        PathValues.SESSIONS_ID_EVENTS: SessionsIdEvents,
         PathValues.MODELCONFIGS: ModelConfigs,
         PathValues.MODELCONFIGS_ID: ModelConfigsId,
         PathValues.PROJECTS_PROJECT_ID_EXPERIMENTS: ProjectsProjectIdExperiments,
         PathValues.EXPERIMENTS_EXPERIMENT_ID: ExperimentsExperimentId,
         PathValues.EXPERIMENTS_EXPERIMENT_ID_MODELCONFIG: ExperimentsExperimentIdModelConfig,
+        PathValues.SESSIONS: Sessions,
+        PathValues.SESSIONS_ID: SessionsId,
+        PathValues.TRACES: Traces,
     }
 )
```

### Comparing `humanloop-0.4.2/humanloop/apis/tag_to_api.py` & `humanloop-0.4.3/humanloop/apis/tag_to_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 import typing_extensions
 
 from humanloop.apis.tags import TagValues
 from humanloop.apis.tags.projects_api import ProjectsApi
 from humanloop.apis.tags.experiments_api import ExperimentsApi
 from humanloop.apis.tags.completions_api import CompletionsApi
 from humanloop.apis.tags.chats_api import ChatsApi
-from humanloop.apis.tags.apps_api import AppsApi
 from humanloop.apis.tags.sessions_api import SessionsApi
 from humanloop.apis.tags.model_configurations_api import ModelConfigurationsApi
 from humanloop.apis.tags.logs_api import LogsApi
 from humanloop.apis.tags.feedback_api import FeedbackApi
+from humanloop.apis.tags.traces_api import TracesApi
 from humanloop.apis.tags.authentication_api import AuthenticationApi
 
 TagToApi = typing_extensions.TypedDict(
     'TagToApi',
     {
         TagValues.PROJECTS: ProjectsApi,
         TagValues.EXPERIMENTS: ExperimentsApi,
         TagValues.COMPLETIONS: CompletionsApi,
         TagValues.CHATS: ChatsApi,
-        TagValues.APPS: AppsApi,
         TagValues.SESSIONS: SessionsApi,
         TagValues.MODEL_CONFIGURATIONS: ModelConfigurationsApi,
         TagValues.LOGS: LogsApi,
         TagValues.FEEDBACK: FeedbackApi,
+        TagValues.TRACES: TracesApi,
         TagValues.AUTHENTICATION: AuthenticationApi,
     }
 )
 
 tag_to_api = TagToApi(
     {
         TagValues.PROJECTS: ProjectsApi,
         TagValues.EXPERIMENTS: ExperimentsApi,
         TagValues.COMPLETIONS: CompletionsApi,
         TagValues.CHATS: ChatsApi,
-        TagValues.APPS: AppsApi,
         TagValues.SESSIONS: SessionsApi,
         TagValues.MODEL_CONFIGURATIONS: ModelConfigurationsApi,
         TagValues.LOGS: LogsApi,
         TagValues.FEEDBACK: FeedbackApi,
+        TagValues.TRACES: TracesApi,
         TagValues.AUTHENTICATION: AuthenticationApi,
     }
 )
```

### Comparing `humanloop-0.4.2/humanloop/apis/tags/__init__.py` & `humanloop-0.4.3/humanloop/apis/tags/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 
 
 class TagValues(str, enum.Enum):
     PROJECTS = "Projects"
     EXPERIMENTS = "Experiments"
     COMPLETIONS = "Completions"
     CHATS = "Chats"
-    APPS = "Apps"
     SESSIONS = "Sessions"
     MODEL_CONFIGURATIONS = "Model Configurations"
     LOGS = "Logs"
     FEEDBACK = "Feedback"
+    TRACES = "Traces"
     AUTHENTICATION = "Authentication"
```

### Comparing `humanloop-0.4.2/humanloop/apis/tags/apps_api.py` & `humanloop-0.4.3/humanloop/apis/tags/experiments_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,21 +5,25 @@
 
     The Humanloop API allows you to interact with Humanloop from your product or service.  You can do this through HTTP requests from any language or via our official Python SDK.  To install the official Python SDK, run the following command:  ```bash pip install humanloop ```  ---  Guides and further details about key concepts can be found in [our docs](https://humanloop.gitbook.io/humanloop-docs/).
 
     The version of the OpenAPI document: 4.0.0
     Generated by: https://konfigthis.com
 """
 
-from humanloop.paths.apps_id.get import Get
-from humanloop.paths.apps_id_sessions.get import GetSessions
-from humanloop.paths.apps.get import List
+from humanloop.paths.projects_project_id_experiments.post import Create
+from humanloop.paths.experiments_experiment_id.delete import Delete
+from humanloop.paths.experiments_experiment_id_model_config.get import GetModelConfig
+from humanloop.paths.projects_project_id_experiments.get import List
+from humanloop.paths.experiments_experiment_id.patch import Update
 
 
-class AppsApi(
-    Get,
-    GetSessions,
+class ExperimentsApi(
+    Create,
+    Delete,
+    GetModelConfig,
     List,
+    Update,
 ):
     """NOTE:
     This class is auto generated by Konfig (https://konfigthis.com)
     """
     pass
```

### Comparing `humanloop-0.4.2/humanloop/apis/tags/chats_api.py` & `humanloop-0.4.3/humanloop/apis/tags/chats_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/apis/tags/completions_api.py` & `humanloop-0.4.3/humanloop/apis/tags/completions_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/apis/tags/experiments_api.py` & `humanloop-0.4.3/humanloop/apis/tags/model_configurations_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,25 +5,19 @@
 
     The Humanloop API allows you to interact with Humanloop from your product or service.  You can do this through HTTP requests from any language or via our official Python SDK.  To install the official Python SDK, run the following command:  ```bash pip install humanloop ```  ---  Guides and further details about key concepts can be found in [our docs](https://humanloop.gitbook.io/humanloop-docs/).
 
     The version of the OpenAPI document: 4.0.0
     Generated by: https://konfigthis.com
 """
 
-from humanloop.paths.projects_project_id_experiments.post import Create
-from humanloop.paths.experiments_experiment_id.delete import Delete
-from humanloop.paths.experiments_experiment_id_model_config.get import GetModelConfig
-from humanloop.paths.projects_project_id_experiments.get import List
-from humanloop.paths.experiments_experiment_id.patch import Update
+from humanloop.paths.model_configs_id.get import Get
+from humanloop.paths.model_configs.post import Register
 
 
-class ExperimentsApi(
-    Create,
-    Delete,
-    GetModelConfig,
-    List,
-    Update,
+class ModelConfigurationsApi(
+    Get,
+    Register,
 ):
     """NOTE:
     This class is auto generated by Konfig (https://konfigthis.com)
     """
     pass
```

### Comparing `humanloop-0.4.2/humanloop/apis/tags/feedback_api.py` & `humanloop-0.4.3/humanloop/apis/tags/feedback_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/apis/tags/logs_api.py` & `humanloop-0.4.3/humanloop/apis/tags/logs_api.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/apis/tags/model_configurations_api.py` & `humanloop-0.4.3/humanloop/apis/tags/sessions_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 
     The Humanloop API allows you to interact with Humanloop from your product or service.  You can do this through HTTP requests from any language or via our official Python SDK.  To install the official Python SDK, run the following command:  ```bash pip install humanloop ```  ---  Guides and further details about key concepts can be found in [our docs](https://humanloop.gitbook.io/humanloop-docs/).
 
     The version of the OpenAPI document: 4.0.0
     Generated by: https://konfigthis.com
 """
 
-from humanloop.paths.model_configs_id.get import Get
-from humanloop.paths.model_configs.post import Register
+from humanloop.paths.sessions.post import Create
+from humanloop.paths.sessions_id.get import Get
+from humanloop.paths.sessions.get import List
 
 
-class ModelConfigurationsApi(
+class SessionsApi(
+    Create,
     Get,
-    Register,
+    List,
 ):
     """NOTE:
     This class is auto generated by Konfig (https://konfigthis.com)
     """
     pass
```

### Comparing `humanloop-0.4.2/humanloop/apis/tags/projects_api.py` & `humanloop-0.4.3/humanloop/apis/tags/projects_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,33 +6,33 @@
     The Humanloop API allows you to interact with Humanloop from your product or service.  You can do this through HTTP requests from any language or via our official Python SDK.  To install the official Python SDK, run the following command:  ```bash pip install humanloop ```  ---  Guides and further details about key concepts can be found in [our docs](https://humanloop.gitbook.io/humanloop-docs/).
 
     The version of the OpenAPI document: 4.0.0
     Generated by: https://konfigthis.com
 """
 
 from humanloop.paths.projects.post import Create
+from humanloop.paths.projects_id_active_config.delete import DeactivateActiveConfig
 from humanloop.paths.projects_id_active_experiment.delete import DeleteActiveExperiment
-from humanloop.paths.projects_id_active_model_config.delete import DeleteActiveModelConfig
 from humanloop.paths.projects_id_export.post import ExportDatapoints
 from humanloop.paths.projects_id.get import Get
-from humanloop.paths.projects_id_model_config.get import GetModelConfig
-from humanloop.paths.projects_id_model_configs.get import GetModelConfigs
+from humanloop.paths.projects_id_active_config.get import GetConfig
+from humanloop.paths.projects_id_configs.get import GetConfigs
 from humanloop.paths.projects.get import List
 from humanloop.paths.projects_id.patch import Update
 from humanloop.paths.projects_id_feedback_types.patch import UpdateFeedbackTypes
 
 
 class ProjectsApi(
     Create,
+    DeactivateActiveConfig,
     DeleteActiveExperiment,
-    DeleteActiveModelConfig,
     ExportDatapoints,
     Get,
-    GetModelConfig,
-    GetModelConfigs,
+    GetConfig,
+    GetConfigs,
     List,
     Update,
     UpdateFeedbackTypes,
 ):
     """NOTE:
     This class is auto generated by Konfig (https://konfigthis.com)
     """
```

### Comparing `humanloop-0.4.2/humanloop/apis/tags/sessions_api.py` & `humanloop-0.4.3/humanloop/type/session_project_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,21 +5,24 @@
 
     The Humanloop API allows you to interact with Humanloop from your product or service.  You can do this through HTTP requests from any language or via our official Python SDK.  To install the official Python SDK, run the following command:  ```bash pip install humanloop ```  ---  Guides and further details about key concepts can be found in [our docs](https://humanloop.gitbook.io/humanloop-docs/).
 
     The version of the OpenAPI document: 4.0.0
     Generated by: https://konfigthis.com
 """
 
-from humanloop.paths.sessions.post import Create
-from humanloop.paths.sessions_id.get import Get
-from humanloop.paths.sessions_id_events.get import GetEvents
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
 
-class SessionsApi(
-    Create,
-    Get,
-    GetEvents,
-):
-    """NOTE:
-    This class is auto generated by Konfig (https://konfigthis.com)
-    """
+class RequiredSessionProjectResponse(TypedDict):
+    # String ID of project the datapoint belongs to. Starts with `pr_`.
+    id: str
+
+    name: str
+
+class OptionalSessionProjectResponse(TypedDict, total=False):
+    pass
+
+class SessionProjectResponse(RequiredSessionProjectResponse, OptionalSessionProjectResponse):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/client.py` & `humanloop-0.4.3/humanloop/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 import typing
 import inspect
 from datetime import date, datetime
 from humanloop.client_custom import ClientCustom
 from humanloop.configuration import Configuration
 from humanloop.api_client import ApiClient
 from humanloop.type_util import copy_signature
-from humanloop.apis.tags.apps_api import AppsApi
 from humanloop.apis.tags.chats_api import ChatsApi
 from humanloop.apis.tags.completions_api import CompletionsApi
 from humanloop.apis.tags.experiments_api import ExperimentsApi
 from humanloop.apis.tags.feedback_api import FeedbackApi
 from humanloop.apis.tags.logs_api import LogsApi
 from humanloop.apis.tags.model_configurations_api import ModelConfigurationsApi
 from humanloop.apis.tags.projects_api import ProjectsApi
 from humanloop.apis.tags.sessions_api import SessionsApi
+from humanloop.apis.tags.traces_api import TracesApi
 
 from humanloop.type.provider_api_keys import ProviderApiKeys
 from humanloop.type.chat_message import ChatMessage
 from humanloop.type.chat_request import ChatRequest
 from humanloop.type.chat_response import ChatResponse
 from humanloop.type.http_validation_error import HTTPValidationError
 from humanloop.type.model_config_chat_request import ModelConfigChatRequest
@@ -65,39 +65,41 @@
 from humanloop.type.http_validation_error import HTTPValidationError
 from humanloop.type.feedback_submit_request import FeedbackSubmitRequest
 from humanloop.type.feedback_type import FeedbackType
 from humanloop.type.feedback_submit_response import FeedbackSubmitResponse
 from humanloop.type.http_validation_error import HTTPValidationError
 from humanloop.type.feedback import Feedback
 from humanloop.type.chat_message import ChatMessage
-from humanloop.type.model_config_completion_request import ModelConfigCompletionRequest
+from humanloop.type.agent_config_request import AgentConfigRequest
+from humanloop.type.generic_config_request import GenericConfigRequest
+from humanloop.type.tool_config_request import ToolConfigRequest
 from humanloop.type.logs_log_response import LogsLogResponse
+from humanloop.type.trace_model_config_request import TraceModelConfigRequest
 from humanloop.type.log_datapoint_request import LogDatapointRequest
 from humanloop.type.http_validation_error import HTTPValidationError
-from humanloop.type.model_config_chat_request import ModelConfigChatRequest
 
 
 class Humanloop(ClientCustom):
 
     def __init__(self, configuration: typing.Union[Configuration, None] = None, **kwargs):
         super().__init__(configuration, **kwargs)
         if (len(kwargs) > 0):
             configuration = Configuration(**kwargs)
         if (configuration is None):
             raise Exception("configuration is required")
         api_client = ApiClient(configuration)
-        self.apps: AppsApi = AppsApi(api_client)
         self.chats_api: ChatsApi = ChatsApi(api_client)
         self.completions_api: CompletionsApi = CompletionsApi(api_client)
         self.experiments: ExperimentsApi = ExperimentsApi(api_client)
         self.feedback_api: FeedbackApi = FeedbackApi(api_client)
         self.logs_api: LogsApi = LogsApi(api_client)
         self.model_configurations: ModelConfigurationsApi = ModelConfigurationsApi(api_client)
         self.projects: ProjectsApi = ProjectsApi(api_client)
         self.sessions: SessionsApi = SessionsApi(api_client)
+        self.traces: TracesApi = TracesApi(api_client)
 
     @copy_signature(ChatsApi.aresponse)
     async def achat(
         self,
         project: str,
         messages: typing.List[ChatMessage],
         model_config: ModelConfigChatRequest,
@@ -585,60 +587,68 @@
         session_id: typing.Optional[str] = None,
         parent_id: typing.Optional[str] = None,
         trial_id: typing.Optional[str] = None,
         inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         messages: typing.Optional[typing.List[ChatMessage]] = None,
         output: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
-        model_config: typing.Optional[typing.Union[ModelConfigCompletionRequest, ModelConfigChatRequest]] = None,
+        config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
         metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         feedback: typing.Optional[typing.Union[Feedback, typing.List[Feedback]]] = None,
         created_at: typing.Optional[datetime] = None,
+        error: typing.Optional[str] = None,
+        duration: typing.Optional[typing.Union[int, float]] = None,
     ):
         return await self.logs_api.alog(
             body=body,
             project=project,
             session_id=session_id,
             parent_id=parent_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             output=output,
             source=source,
-            model_config=model_config,
+            config=config,
             metadata=metadata,
             feedback=feedback,
             created_at=created_at,
+            error=error,
+            duration=duration,
         )
 
     @copy_signature(LogsApi.log)
     def log(
         self,
         body: typing.Optional[LogDatapointRequest] = None,
         project: typing.Optional[str] = None,
         session_id: typing.Optional[str] = None,
         parent_id: typing.Optional[str] = None,
         trial_id: typing.Optional[str] = None,
         inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         messages: typing.Optional[typing.List[ChatMessage]] = None,
         output: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
-        model_config: typing.Optional[typing.Union[ModelConfigCompletionRequest, ModelConfigChatRequest]] = None,
+        config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
         metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         feedback: typing.Optional[typing.Union[Feedback, typing.List[Feedback]]] = None,
         created_at: typing.Optional[datetime] = None,
+        error: typing.Optional[str] = None,
+        duration: typing.Optional[typing.Union[int, float]] = None,
     ):
         return self.logs_api.log(
             body=body,
             project=project,
             session_id=session_id,
             parent_id=parent_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             output=output,
             source=source,
-            model_config=model_config,
+            config=config,
             metadata=metadata,
             feedback=feedback,
             created_at=created_at,
+            error=error,
+            duration=duration,
         )
```

### Comparing `humanloop-0.4.2/humanloop/client.pyi` & `humanloop-0.4.3/humanloop/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 import typing
 import inspect
 from datetime import date, datetime
 from humanloop.client_custom import ClientCustom
 from humanloop.configuration import Configuration
 from humanloop.api_client import ApiClient
 from humanloop.type_util import copy_signature
-from humanloop.apis.tags.apps_api import AppsApi
 from humanloop.apis.tags.chats_api import ChatsApi
 from humanloop.apis.tags.completions_api import CompletionsApi
 from humanloop.apis.tags.experiments_api import ExperimentsApi
 from humanloop.apis.tags.feedback_api import FeedbackApi
 from humanloop.apis.tags.logs_api import LogsApi
 from humanloop.apis.tags.model_configurations_api import ModelConfigurationsApi
 from humanloop.apis.tags.projects_api import ProjectsApi
 from humanloop.apis.tags.sessions_api import SessionsApi
+from humanloop.apis.tags.traces_api import TracesApi
 
 from humanloop.type.provider_api_keys import ProviderApiKeys
 from humanloop.type.chat_message import ChatMessage
 from humanloop.type.chat_request import ChatRequest
 from humanloop.type.chat_response import ChatResponse
 from humanloop.type.http_validation_error import HTTPValidationError
 from humanloop.type.model_config_chat_request import ModelConfigChatRequest
@@ -65,39 +65,41 @@
 from humanloop.type.http_validation_error import HTTPValidationError
 from humanloop.type.feedback_submit_request import FeedbackSubmitRequest
 from humanloop.type.feedback_type import FeedbackType
 from humanloop.type.feedback_submit_response import FeedbackSubmitResponse
 from humanloop.type.http_validation_error import HTTPValidationError
 from humanloop.type.feedback import Feedback
 from humanloop.type.chat_message import ChatMessage
-from humanloop.type.model_config_completion_request import ModelConfigCompletionRequest
+from humanloop.type.agent_config_request import AgentConfigRequest
+from humanloop.type.generic_config_request import GenericConfigRequest
+from humanloop.type.tool_config_request import ToolConfigRequest
 from humanloop.type.logs_log_response import LogsLogResponse
+from humanloop.type.trace_model_config_request import TraceModelConfigRequest
 from humanloop.type.log_datapoint_request import LogDatapointRequest
 from humanloop.type.http_validation_error import HTTPValidationError
-from humanloop.type.model_config_chat_request import ModelConfigChatRequest
 
 
 class Humanloop(ClientCustom):
 
     def __init__(self, configuration: typing.Union[Configuration, None] = None, **kwargs):
         super().__init__(configuration, **kwargs)
         if (len(kwargs) > 0):
             configuration = Configuration(**kwargs)
         if (configuration is None):
             raise Exception("configuration is required")
         api_client = ApiClient(configuration)
-        self.apps: AppsApi = AppsApi(api_client)
         self.chats_api: ChatsApi = ChatsApi(api_client)
         self.completions_api: CompletionsApi = CompletionsApi(api_client)
         self.experiments: ExperimentsApi = ExperimentsApi(api_client)
         self.feedback_api: FeedbackApi = FeedbackApi(api_client)
         self.logs_api: LogsApi = LogsApi(api_client)
         self.model_configurations: ModelConfigurationsApi = ModelConfigurationsApi(api_client)
         self.projects: ProjectsApi = ProjectsApi(api_client)
         self.sessions: SessionsApi = SessionsApi(api_client)
+        self.traces: TracesApi = TracesApi(api_client)
 
     @copy_signature(ChatsApi.aresponse)
     async def achat(
         self,
         project: str,
         messages: typing.List[ChatMessage],
         model_config: ModelConfigChatRequest,
@@ -585,60 +587,68 @@
         session_id: typing.Optional[str] = None,
         parent_id: typing.Optional[str] = None,
         trial_id: typing.Optional[str] = None,
         inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         messages: typing.Optional[typing.List[ChatMessage]] = None,
         output: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
-        model_config: typing.Optional[typing.Union[ModelConfigCompletionRequest, ModelConfigChatRequest]] = None,
+        config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
         metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         feedback: typing.Optional[typing.Union[Feedback, typing.List[Feedback]]] = None,
         created_at: typing.Optional[datetime] = None,
+        error: typing.Optional[str] = None,
+        duration: typing.Optional[typing.Union[int, float]] = None,
     ):
         return await self.logs_api.alog(
             body=body,
             project=project,
             session_id=session_id,
             parent_id=parent_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             output=output,
             source=source,
-            model_config=model_config,
+            config=config,
             metadata=metadata,
             feedback=feedback,
             created_at=created_at,
+            error=error,
+            duration=duration,
         )
 
     @copy_signature(LogsApi.log)
     def log(
         self,
         body: typing.Optional[LogDatapointRequest] = None,
         project: typing.Optional[str] = None,
         session_id: typing.Optional[str] = None,
         parent_id: typing.Optional[str] = None,
         trial_id: typing.Optional[str] = None,
         inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         messages: typing.Optional[typing.List[ChatMessage]] = None,
         output: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
-        model_config: typing.Optional[typing.Union[ModelConfigCompletionRequest, ModelConfigChatRequest]] = None,
+        config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
         metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         feedback: typing.Optional[typing.Union[Feedback, typing.List[Feedback]]] = None,
         created_at: typing.Optional[datetime] = None,
+        error: typing.Optional[str] = None,
+        duration: typing.Optional[typing.Union[int, float]] = None,
     ):
         return self.logs_api.log(
             body=body,
             project=project,
             session_id=session_id,
             parent_id=parent_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             output=output,
             source=source,
-            model_config=model_config,
+            config=config,
             metadata=metadata,
             feedback=feedback,
             created_at=created_at,
+            error=error,
+            duration=duration,
         )
```

### Comparing `humanloop-0.4.2/humanloop/client_custom.py` & `humanloop-0.4.3/humanloop/client_custom.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/configuration.py` & `humanloop-0.4.3/humanloop/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,15 +422,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 4.0.0\n"\
-               "SDK Package Version: 0.4.2".\
+               "SDK Package Version: 0.4.3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `humanloop-0.4.2/humanloop/exceptions.py` & `humanloop-0.4.3/humanloop/exceptions.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/exceptions_base.py` & `humanloop-0.4.3/humanloop/exceptions_base.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/base_metric_response.py` & `humanloop-0.4.3/humanloop/model/base_metric_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/base_metric_response.pyi` & `humanloop-0.4.3/humanloop/model/base_metric_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/categorical_feedback_label.py` & `humanloop-0.4.3/humanloop/model/categorical_feedback_label.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/categorical_feedback_label.pyi` & `humanloop-0.4.3/humanloop/model/categorical_feedback_label.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/chat_data_response.py` & `humanloop-0.4.3/humanloop/model/chat_data_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/chat_data_response.pyi` & `humanloop-0.4.3/humanloop/model/chat_data_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/chat_deployed_request.py` & `humanloop-0.4.3/humanloop/model/chat_deployed_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/chat_deployed_request.pyi` & `humanloop-0.4.3/humanloop/model/chat_deployed_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/chat_experiment_request.py` & `humanloop-0.4.3/humanloop/model/chat_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/chat_experiment_request.pyi` & `humanloop-0.4.3/humanloop/model/chat_experiment_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/chat_message.py` & `humanloop-0.4.3/humanloop/model/chat_message.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/chat_message.pyi` & `humanloop-0.4.3/humanloop/model/chat_message.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/chat_model_config_request.py` & `humanloop-0.4.3/humanloop/model/chat_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/chat_model_config_request.pyi` & `humanloop-0.4.3/humanloop/model/chat_model_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/chat_request.py` & `humanloop-0.4.3/humanloop/model/chat_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/chat_request.pyi` & `humanloop-0.4.3/humanloop/model/chat_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/chat_response.py` & `humanloop-0.4.3/humanloop/model/chat_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/chat_response.pyi` & `humanloop-0.4.3/humanloop/model/chat_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/chat_role.py` & `humanloop-0.4.3/humanloop/model/chat_role.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/chat_role.pyi` & `humanloop-0.4.3/humanloop/model/chat_role.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/completion_deployed_request.py` & `humanloop-0.4.3/humanloop/model/completion_deployed_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/completion_deployed_request.pyi` & `humanloop-0.4.3/humanloop/model/completion_deployed_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/completion_experiment_request.py` & `humanloop-0.4.3/humanloop/model/completion_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/completion_experiment_request.pyi` & `humanloop-0.4.3/humanloop/model/completion_experiment_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/completion_model_config_request.py` & `humanloop-0.4.3/humanloop/model/completion_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/completion_model_config_request.pyi` & `humanloop-0.4.3/humanloop/model/completion_model_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/completion_request.py` & `humanloop-0.4.3/humanloop/model/completion_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/completion_request.pyi` & `humanloop-0.4.3/humanloop/model/completion_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/completion_response.py` & `humanloop-0.4.3/humanloop/model/completion_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/completion_response.pyi` & `humanloop-0.4.3/humanloop/model/completion_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/create_experiment_request.py` & `humanloop-0.4.3/humanloop/model/create_experiment_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,100 +63,100 @@
                         _configuration=_configuration,
                     )
             
                 def __getitem__(self, i: int) -> 'PositiveLabel':
                     return super().__getitem__(i)
             
             
-            class model_config_ids(
+            class config_ids(
                 schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     items = schemas.StrSchema
             
                 def __new__(
                     cls,
                     arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'model_config_ids':
+                ) -> 'config_ids':
                     return super().__new__(
                         cls,
                         arg,
                         _configuration=_configuration,
                     )
             
                 def __getitem__(self, i: int) -> MetaOapg.items:
                     return super().__getitem__(i)
             set_active = schemas.BoolSchema
             __annotations__ = {
                 "name": name,
                 "positive_labels": positive_labels,
-                "model_config_ids": model_config_ids,
+                "config_ids": config_ids,
                 "set_active": set_active,
             }
     
     positive_labels: MetaOapg.properties.positive_labels
     name: MetaOapg.properties.name
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["positive_labels"]) -> MetaOapg.properties.positive_labels: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["model_config_ids"]) -> MetaOapg.properties.model_config_ids: ...
+    def __getitem__(self, name: typing_extensions.Literal["config_ids"]) -> MetaOapg.properties.config_ids: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["set_active"]) -> MetaOapg.properties.set_active: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "positive_labels", "model_config_ids", "set_active", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "positive_labels", "config_ids", "set_active", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["positive_labels"]) -> MetaOapg.properties.positive_labels: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["model_config_ids"]) -> typing.Union[MetaOapg.properties.model_config_ids, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["config_ids"]) -> typing.Union[MetaOapg.properties.config_ids, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["set_active"]) -> typing.Union[MetaOapg.properties.set_active, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "positive_labels", "model_config_ids", "set_active", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "positive_labels", "config_ids", "set_active", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         positive_labels: typing.Union[MetaOapg.properties.positive_labels, list, tuple, ],
         name: typing.Union[MetaOapg.properties.name, str, ],
-        model_config_ids: typing.Union[MetaOapg.properties.model_config_ids, list, tuple, schemas.Unset] = schemas.unset,
+        config_ids: typing.Union[MetaOapg.properties.config_ids, list, tuple, schemas.Unset] = schemas.unset,
         set_active: typing.Union[MetaOapg.properties.set_active, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'CreateExperimentRequest':
         return super().__new__(
             cls,
             *args,
             positive_labels=positive_labels,
             name=name,
-            model_config_ids=model_config_ids,
+            config_ids=config_ids,
             set_active=set_active,
             _configuration=_configuration,
             **kwargs,
         )
 
 from humanloop.model.positive_label import PositiveLabel
```

### Comparing `humanloop-0.4.2/humanloop/model/create_experiment_request.pyi` & `humanloop-0.4.3/humanloop/model/create_experiment_request.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -63,100 +63,100 @@
                         _configuration=_configuration,
                     )
             
                 def __getitem__(self, i: int) -> 'PositiveLabel':
                     return super().__getitem__(i)
             
             
-            class model_config_ids(
+            class config_ids(
                 schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     items = schemas.StrSchema
             
                 def __new__(
                     cls,
                     arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'model_config_ids':
+                ) -> 'config_ids':
                     return super().__new__(
                         cls,
                         arg,
                         _configuration=_configuration,
                     )
             
                 def __getitem__(self, i: int) -> MetaOapg.items:
                     return super().__getitem__(i)
             set_active = schemas.BoolSchema
             __annotations__ = {
                 "name": name,
                 "positive_labels": positive_labels,
-                "model_config_ids": model_config_ids,
+                "config_ids": config_ids,
                 "set_active": set_active,
             }
     
     positive_labels: MetaOapg.properties.positive_labels
     name: MetaOapg.properties.name
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["positive_labels"]) -> MetaOapg.properties.positive_labels: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["model_config_ids"]) -> MetaOapg.properties.model_config_ids: ...
+    def __getitem__(self, name: typing_extensions.Literal["config_ids"]) -> MetaOapg.properties.config_ids: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["set_active"]) -> MetaOapg.properties.set_active: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "positive_labels", "model_config_ids", "set_active", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "positive_labels", "config_ids", "set_active", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["positive_labels"]) -> MetaOapg.properties.positive_labels: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["model_config_ids"]) -> typing.Union[MetaOapg.properties.model_config_ids, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["config_ids"]) -> typing.Union[MetaOapg.properties.config_ids, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["set_active"]) -> typing.Union[MetaOapg.properties.set_active, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "positive_labels", "model_config_ids", "set_active", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "positive_labels", "config_ids", "set_active", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         positive_labels: typing.Union[MetaOapg.properties.positive_labels, list, tuple, ],
         name: typing.Union[MetaOapg.properties.name, str, ],
-        model_config_ids: typing.Union[MetaOapg.properties.model_config_ids, list, tuple, schemas.Unset] = schemas.unset,
+        config_ids: typing.Union[MetaOapg.properties.config_ids, list, tuple, schemas.Unset] = schemas.unset,
         set_active: typing.Union[MetaOapg.properties.set_active, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'CreateExperimentRequest':
         return super().__new__(
             cls,
             *args,
             positive_labels=positive_labels,
             name=name,
-            model_config_ids=model_config_ids,
+            config_ids=config_ids,
             set_active=set_active,
             _configuration=_configuration,
             **kwargs,
         )
 
 from humanloop.model.positive_label import PositiveLabel
```

### Comparing `humanloop-0.4.2/humanloop/model/create_log_response.py` & `humanloop-0.4.3/humanloop/model/create_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/create_log_response.pyi` & `humanloop-0.4.3/humanloop/model/create_log_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/create_project_request.py` & `humanloop-0.4.3/humanloop/model/create_project_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/create_project_request.pyi` & `humanloop-0.4.3/humanloop/model/create_project_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/create_session_request.py` & `humanloop-0.4.3/humanloop/model/create_session_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,63 +19,63 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class CreateSessionRequest(
+class CreateSessionResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
-            "app",
+            "id",
         }
         
         class properties:
-            app = schemas.StrSchema
+            id = schemas.StrSchema
             __annotations__ = {
-                "app": app,
+                "id": id,
             }
     
-    app: MetaOapg.properties.app
+    id: MetaOapg.properties.id
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["app"]) -> MetaOapg.properties.app: ...
+    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["app", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["app"]) -> MetaOapg.properties.app: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["app", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        app: typing.Union[MetaOapg.properties.app, str, ],
+        id: typing.Union[MetaOapg.properties.id, str, ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'CreateSessionRequest':
+    ) -> 'CreateSessionResponse':
         return super().__new__(
             cls,
             *args,
-            app=app,
+            id=id,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `humanloop-0.4.2/humanloop/model/create_session_request.pyi` & `humanloop-0.4.3/humanloop/model/create_session_response.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -19,63 +19,63 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class CreateSessionRequest(
+class CreateSessionResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
-            "app",
+            "id",
         }
         
         class properties:
-            app = schemas.StrSchema
+            id = schemas.StrSchema
             __annotations__ = {
-                "app": app,
+                "id": id,
             }
     
-    app: MetaOapg.properties.app
+    id: MetaOapg.properties.id
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["app"]) -> MetaOapg.properties.app: ...
+    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["app", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["app"]) -> MetaOapg.properties.app: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["app", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        app: typing.Union[MetaOapg.properties.app, str, ],
+        id: typing.Union[MetaOapg.properties.id, str, ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'CreateSessionRequest':
+    ) -> 'CreateSessionResponse':
         return super().__new__(
             cls,
             *args,
-            app=app,
+            id=id,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `humanloop-0.4.2/humanloop/model/data_response.py` & `humanloop-0.4.3/humanloop/model/data_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/data_response.pyi` & `humanloop-0.4.3/humanloop/model/data_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/experiment_model_config_response.py` & `humanloop-0.4.3/humanloop/model/experiment_config_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,41 +19,41 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class ExperimentModelConfigResponse(
+class ExperimentConfigResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
-            "model_config",
             "updated_at",
             "active",
             "created_at",
             "id",
             "display_name",
+            "config",
             "trials_count",
         }
         
         class properties:
             trials_count = schemas.IntSchema
             active = schemas.BoolSchema
             id = schemas.StrSchema
             display_name = schemas.StrSchema
             
             
-            class model_config(
+            class config(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
                     
                     @classmethod
@@ -63,24 +63,24 @@
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            SrcExternalAppModelsV4ModelConfigsModelConfigResponse,
+                            ConfigResponse,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'model_config':
+                ) -> 'config':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             created_at = schemas.DateTimeSchema
@@ -88,27 +88,27 @@
             mean = schemas.NumberSchema
             spread = schemas.NumberSchema
             __annotations__ = {
                 "trials_count": trials_count,
                 "active": active,
                 "id": id,
                 "display_name": display_name,
-                "model_config": model_config,
+                "config": config,
                 "created_at": created_at,
                 "updated_at": updated_at,
                 "mean": mean,
                 "spread": spread,
             }
     
-    model_config: MetaOapg.properties.model_config
     updated_at: MetaOapg.properties.updated_at
     active: MetaOapg.properties.active
     created_at: MetaOapg.properties.created_at
     id: MetaOapg.properties.id
     display_name: MetaOapg.properties.display_name
+    config: MetaOapg.properties.config
     trials_count: MetaOapg.properties.trials_count
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["trials_count"]) -> MetaOapg.properties.trials_count: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["active"]) -> MetaOapg.properties.active: ...
@@ -116,15 +116,15 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["display_name"]) -> MetaOapg.properties.display_name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
+    def __getitem__(self, name: typing_extensions.Literal["config"]) -> MetaOapg.properties.config: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
     
@@ -133,15 +133,15 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["spread"]) -> MetaOapg.properties.spread: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["trials_count", "active", "id", "display_name", "model_config", "created_at", "updated_at", "mean", "spread", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["trials_count", "active", "id", "display_name", "config", "created_at", "updated_at", "mean", "spread", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["trials_count"]) -> MetaOapg.properties.trials_count: ...
     
@@ -151,15 +151,15 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["display_name"]) -> MetaOapg.properties.display_name: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["config"]) -> MetaOapg.properties.config: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
     
@@ -168,43 +168,43 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["spread"]) -> typing.Union[MetaOapg.properties.spread, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["trials_count", "active", "id", "display_name", "model_config", "created_at", "updated_at", "mean", "spread", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["trials_count", "active", "id", "display_name", "config", "created_at", "updated_at", "mean", "spread", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        model_config: typing.Union[MetaOapg.properties.model_config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         updated_at: typing.Union[MetaOapg.properties.updated_at, str, datetime, ],
         active: typing.Union[MetaOapg.properties.active, bool, ],
         created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, ],
         id: typing.Union[MetaOapg.properties.id, str, ],
         display_name: typing.Union[MetaOapg.properties.display_name, str, ],
+        config: typing.Union[MetaOapg.properties.config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         trials_count: typing.Union[MetaOapg.properties.trials_count, decimal.Decimal, int, ],
         mean: typing.Union[MetaOapg.properties.mean, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         spread: typing.Union[MetaOapg.properties.spread, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'ExperimentModelConfigResponse':
+    ) -> 'ExperimentConfigResponse':
         return super().__new__(
             cls,
             *args,
-            model_config=model_config,
             updated_at=updated_at,
             active=active,
             created_at=created_at,
             id=id,
             display_name=display_name,
+            config=config,
             trials_count=trials_count,
             mean=mean,
             spread=spread,
             _configuration=_configuration,
             **kwargs,
         )
 
-from humanloop.model.src_external_app_models_v4_model_configs_model_config_response import SrcExternalAppModelsV4ModelConfigsModelConfigResponse
+from humanloop.model.config_response import ConfigResponse
```

### Comparing `humanloop-0.4.2/humanloop/model/experiment_model_config_response.pyi` & `humanloop-0.4.3/humanloop/model/experiment_config_response.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -19,41 +19,41 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class ExperimentModelConfigResponse(
+class ExperimentConfigResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
-            "model_config",
             "updated_at",
             "active",
             "created_at",
             "id",
             "display_name",
+            "config",
             "trials_count",
         }
         
         class properties:
             trials_count = schemas.IntSchema
             active = schemas.BoolSchema
             id = schemas.StrSchema
             display_name = schemas.StrSchema
             
             
-            class model_config(
+            class config(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
                     
                     @classmethod
@@ -63,24 +63,24 @@
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            SrcExternalAppModelsV4ModelConfigsModelConfigResponse,
+                            ConfigResponse,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'model_config':
+                ) -> 'config':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             created_at = schemas.DateTimeSchema
@@ -88,27 +88,27 @@
             mean = schemas.NumberSchema
             spread = schemas.NumberSchema
             __annotations__ = {
                 "trials_count": trials_count,
                 "active": active,
                 "id": id,
                 "display_name": display_name,
-                "model_config": model_config,
+                "config": config,
                 "created_at": created_at,
                 "updated_at": updated_at,
                 "mean": mean,
                 "spread": spread,
             }
     
-    model_config: MetaOapg.properties.model_config
     updated_at: MetaOapg.properties.updated_at
     active: MetaOapg.properties.active
     created_at: MetaOapg.properties.created_at
     id: MetaOapg.properties.id
     display_name: MetaOapg.properties.display_name
+    config: MetaOapg.properties.config
     trials_count: MetaOapg.properties.trials_count
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["trials_count"]) -> MetaOapg.properties.trials_count: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["active"]) -> MetaOapg.properties.active: ...
@@ -116,15 +116,15 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["display_name"]) -> MetaOapg.properties.display_name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
+    def __getitem__(self, name: typing_extensions.Literal["config"]) -> MetaOapg.properties.config: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
     
@@ -133,15 +133,15 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["spread"]) -> MetaOapg.properties.spread: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["trials_count", "active", "id", "display_name", "model_config", "created_at", "updated_at", "mean", "spread", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["trials_count", "active", "id", "display_name", "config", "created_at", "updated_at", "mean", "spread", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["trials_count"]) -> MetaOapg.properties.trials_count: ...
     
@@ -151,15 +151,15 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["display_name"]) -> MetaOapg.properties.display_name: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["config"]) -> MetaOapg.properties.config: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
     
@@ -168,43 +168,43 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["spread"]) -> typing.Union[MetaOapg.properties.spread, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["trials_count", "active", "id", "display_name", "model_config", "created_at", "updated_at", "mean", "spread", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["trials_count", "active", "id", "display_name", "config", "created_at", "updated_at", "mean", "spread", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        model_config: typing.Union[MetaOapg.properties.model_config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         updated_at: typing.Union[MetaOapg.properties.updated_at, str, datetime, ],
         active: typing.Union[MetaOapg.properties.active, bool, ],
         created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, ],
         id: typing.Union[MetaOapg.properties.id, str, ],
         display_name: typing.Union[MetaOapg.properties.display_name, str, ],
+        config: typing.Union[MetaOapg.properties.config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         trials_count: typing.Union[MetaOapg.properties.trials_count, decimal.Decimal, int, ],
         mean: typing.Union[MetaOapg.properties.mean, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         spread: typing.Union[MetaOapg.properties.spread, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'ExperimentModelConfigResponse':
+    ) -> 'ExperimentConfigResponse':
         return super().__new__(
             cls,
             *args,
-            model_config=model_config,
             updated_at=updated_at,
             active=active,
             created_at=created_at,
             id=id,
             display_name=display_name,
+            config=config,
             trials_count=trials_count,
             mean=mean,
             spread=spread,
             _configuration=_configuration,
             **kwargs,
         )
 
-from humanloop.model.src_external_app_models_v4_model_configs_model_config_response import SrcExternalAppModelsV4ModelConfigsModelConfigResponse
+from humanloop.model.config_response import ConfigResponse
```

### Comparing `humanloop-0.4.2/humanloop/model/experiment_response.py` & `humanloop-0.4.3/humanloop/model/experiment_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,48 +145,48 @@
             
                 def __getitem__(self, i: int) -> 'PositiveLabel':
                     return super().__getitem__(i)
             created_at = schemas.DateTimeSchema
             updated_at = schemas.DateTimeSchema
             
             
-            class model_configs(
+            class configs(
                 schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
                     @staticmethod
-                    def items() -> typing.Type['ExperimentModelConfigResponse']:
-                        return ExperimentModelConfigResponse
+                    def items() -> typing.Type['ExperimentConfigResponse']:
+                        return ExperimentConfigResponse
             
                 def __new__(
                     cls,
-                    arg: typing.Union[typing.Tuple['ExperimentModelConfigResponse'], typing.List['ExperimentModelConfigResponse']],
+                    arg: typing.Union[typing.Tuple['ExperimentConfigResponse'], typing.List['ExperimentConfigResponse']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'model_configs':
+                ) -> 'configs':
                     return super().__new__(
                         cls,
                         arg,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> 'ExperimentModelConfigResponse':
+                def __getitem__(self, i: int) -> 'ExperimentConfigResponse':
                     return super().__getitem__(i)
             __annotations__ = {
                 "id": id,
                 "project_id": project_id,
                 "name": name,
                 "status": status,
                 "metric": metric,
                 "positive_labels": positive_labels,
                 "created_at": created_at,
                 "updated_at": updated_at,
-                "model_configs": model_configs,
+                "configs": configs,
             }
     
     positive_labels: MetaOapg.properties.positive_labels
     updated_at: MetaOapg.properties.updated_at
     metric: MetaOapg.properties.metric
     project_id: MetaOapg.properties.project_id
     name: MetaOapg.properties.name
@@ -215,20 +215,20 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["model_configs"]) -> MetaOapg.properties.model_configs: ...
+    def __getitem__(self, name: typing_extensions.Literal["configs"]) -> MetaOapg.properties.configs: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "project_id", "name", "status", "metric", "positive_labels", "created_at", "updated_at", "model_configs", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "project_id", "name", "status", "metric", "positive_labels", "created_at", "updated_at", "configs", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
@@ -250,51 +250,51 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["model_configs"]) -> typing.Union[MetaOapg.properties.model_configs, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["configs"]) -> typing.Union[MetaOapg.properties.configs, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "project_id", "name", "status", "metric", "positive_labels", "created_at", "updated_at", "model_configs", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "project_id", "name", "status", "metric", "positive_labels", "created_at", "updated_at", "configs", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         positive_labels: typing.Union[MetaOapg.properties.positive_labels, list, tuple, ],
         updated_at: typing.Union[MetaOapg.properties.updated_at, str, datetime, ],
         metric: typing.Union[MetaOapg.properties.metric, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         project_id: typing.Union[MetaOapg.properties.project_id, str, ],
         name: typing.Union[MetaOapg.properties.name, str, ],
         created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, ],
         id: typing.Union[MetaOapg.properties.id, str, ],
         status: typing.Union[MetaOapg.properties.status, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        model_configs: typing.Union[MetaOapg.properties.model_configs, list, tuple, schemas.Unset] = schemas.unset,
+        configs: typing.Union[MetaOapg.properties.configs, list, tuple, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'ExperimentResponse':
         return super().__new__(
             cls,
             *args,
             positive_labels=positive_labels,
             updated_at=updated_at,
             metric=metric,
             project_id=project_id,
             name=name,
             created_at=created_at,
             id=id,
             status=status,
-            model_configs=model_configs,
+            configs=configs,
             _configuration=_configuration,
             **kwargs,
         )
 
 from humanloop.model.base_metric_response import BaseMetricResponse
-from humanloop.model.experiment_model_config_response import ExperimentModelConfigResponse
+from humanloop.model.experiment_config_response import ExperimentConfigResponse
 from humanloop.model.experiment_status import ExperimentStatus
 from humanloop.model.positive_label import PositiveLabel
```

### Comparing `humanloop-0.4.2/humanloop/model/experiment_response.pyi` & `humanloop-0.4.3/humanloop/model/experiment_response.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -145,48 +145,48 @@
             
                 def __getitem__(self, i: int) -> 'PositiveLabel':
                     return super().__getitem__(i)
             created_at = schemas.DateTimeSchema
             updated_at = schemas.DateTimeSchema
             
             
-            class model_configs(
+            class configs(
                 schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
                     @staticmethod
-                    def items() -> typing.Type['ExperimentModelConfigResponse']:
-                        return ExperimentModelConfigResponse
+                    def items() -> typing.Type['ExperimentConfigResponse']:
+                        return ExperimentConfigResponse
             
                 def __new__(
                     cls,
-                    arg: typing.Union[typing.Tuple['ExperimentModelConfigResponse'], typing.List['ExperimentModelConfigResponse']],
+                    arg: typing.Union[typing.Tuple['ExperimentConfigResponse'], typing.List['ExperimentConfigResponse']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'model_configs':
+                ) -> 'configs':
                     return super().__new__(
                         cls,
                         arg,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> 'ExperimentModelConfigResponse':
+                def __getitem__(self, i: int) -> 'ExperimentConfigResponse':
                     return super().__getitem__(i)
             __annotations__ = {
                 "id": id,
                 "project_id": project_id,
                 "name": name,
                 "status": status,
                 "metric": metric,
                 "positive_labels": positive_labels,
                 "created_at": created_at,
                 "updated_at": updated_at,
-                "model_configs": model_configs,
+                "configs": configs,
             }
     
     positive_labels: MetaOapg.properties.positive_labels
     updated_at: MetaOapg.properties.updated_at
     metric: MetaOapg.properties.metric
     project_id: MetaOapg.properties.project_id
     name: MetaOapg.properties.name
@@ -215,20 +215,20 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["model_configs"]) -> MetaOapg.properties.model_configs: ...
+    def __getitem__(self, name: typing_extensions.Literal["configs"]) -> MetaOapg.properties.configs: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "project_id", "name", "status", "metric", "positive_labels", "created_at", "updated_at", "model_configs", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "project_id", "name", "status", "metric", "positive_labels", "created_at", "updated_at", "configs", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
@@ -250,51 +250,51 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["model_configs"]) -> typing.Union[MetaOapg.properties.model_configs, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["configs"]) -> typing.Union[MetaOapg.properties.configs, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "project_id", "name", "status", "metric", "positive_labels", "created_at", "updated_at", "model_configs", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "project_id", "name", "status", "metric", "positive_labels", "created_at", "updated_at", "configs", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         positive_labels: typing.Union[MetaOapg.properties.positive_labels, list, tuple, ],
         updated_at: typing.Union[MetaOapg.properties.updated_at, str, datetime, ],
         metric: typing.Union[MetaOapg.properties.metric, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
         project_id: typing.Union[MetaOapg.properties.project_id, str, ],
         name: typing.Union[MetaOapg.properties.name, str, ],
         created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, ],
         id: typing.Union[MetaOapg.properties.id, str, ],
         status: typing.Union[MetaOapg.properties.status, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-        model_configs: typing.Union[MetaOapg.properties.model_configs, list, tuple, schemas.Unset] = schemas.unset,
+        configs: typing.Union[MetaOapg.properties.configs, list, tuple, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'ExperimentResponse':
         return super().__new__(
             cls,
             *args,
             positive_labels=positive_labels,
             updated_at=updated_at,
             metric=metric,
             project_id=project_id,
             name=name,
             created_at=created_at,
             id=id,
             status=status,
-            model_configs=model_configs,
+            configs=configs,
             _configuration=_configuration,
             **kwargs,
         )
 
 from humanloop.model.base_metric_response import BaseMetricResponse
-from humanloop.model.experiment_model_config_response import ExperimentModelConfigResponse
+from humanloop.model.experiment_config_response import ExperimentConfigResponse
 from humanloop.model.experiment_status import ExperimentStatus
 from humanloop.model.positive_label import PositiveLabel
```

### Comparing `humanloop-0.4.2/humanloop/model/experiment_status.py` & `humanloop-0.4.3/humanloop/model/experiment_status.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/experiment_status.pyi` & `humanloop-0.4.3/humanloop/model/experiment_status.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/experiments_list_response.py` & `humanloop-0.4.3/humanloop/model/experiments_list_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/experiments_list_response.pyi` & `humanloop-0.4.3/humanloop/model/experiments_list_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/feedback.py` & `humanloop-0.4.3/humanloop/model/feedback.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/feedback.pyi` & `humanloop-0.4.3/humanloop/model/feedback.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/feedback_class.py` & `humanloop-0.4.3/humanloop/model/feedback_class.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/feedback_class.pyi` & `humanloop-0.4.3/humanloop/model/feedback_class.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/feedback_label_request.py` & `humanloop-0.4.3/humanloop/model/feedback_label_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/feedback_label_request.pyi` & `humanloop-0.4.3/humanloop/model/feedback_label_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/feedback_request.py` & `humanloop-0.4.3/humanloop/model/feedback_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/feedback_request.pyi` & `humanloop-0.4.3/humanloop/model/feedback_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/feedback_response.py` & `humanloop-0.4.3/humanloop/model/feedback_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/feedback_response.pyi` & `humanloop-0.4.3/humanloop/model/feedback_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/feedback_submit_request.py` & `humanloop-0.4.3/humanloop/model/feedback_submit_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/feedback_submit_request.pyi` & `humanloop-0.4.3/humanloop/model/feedback_submit_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/feedback_submit_response.py` & `humanloop-0.4.3/humanloop/model/feedback_submit_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/feedback_submit_response.pyi` & `humanloop-0.4.3/humanloop/model/feedback_submit_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/feedback_type.py` & `humanloop-0.4.3/humanloop/model/feedback_type.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/feedback_type.pyi` & `humanloop-0.4.3/humanloop/model/feedback_type.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/feedback_type_model.py` & `humanloop-0.4.3/humanloop/model/feedback_type_model.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/feedback_type_model.pyi` & `humanloop-0.4.3/humanloop/model/feedback_type_model.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/feedback_type_request.py` & `humanloop-0.4.3/humanloop/model/feedback_type_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/feedback_type_request.pyi` & `humanloop-0.4.3/humanloop/model/feedback_type_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/feedback_types.py` & `humanloop-0.4.3/humanloop/model/feedback_types.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/feedback_types.pyi` & `humanloop-0.4.3/humanloop/model/feedback_types.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/get_model_config_response.py` & `humanloop-0.4.3/humanloop/model/project_model_config_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,22 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class GetModelConfigResponse(
+class ProjectModelConfigResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
 
-    A selected model configuration.
-
-If the model configuration was selected in the context of an experiment,
-the response will include a trial_id to associate a subsequent log() call.
+    Extends the core ModelConfig request object to include Humanloop generated
+identifier and method for serializing response from ModelConfig domain object.
     """
 
 
     class MetaOapg:
         required = {
             "updated_at",
             "last_used",
@@ -83,82 +81,50 @@
                 ) -> 'provider':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            max_tokens = schemas.IntSchema
-            temperature = schemas.NumberSchema
-            top_p = schemas.NumberSchema
             
             
-            class stop(
+            class endpoint(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
-                    any_of_0 = schemas.StrSchema
-                    
-                    
-                    class any_of_1(
-                        schemas.ListSchema
-                    ):
-                    
-                    
-                        class MetaOapg:
-                            items = schemas.StrSchema
-                    
-                        def __new__(
-                            cls,
-                            arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
-                            _configuration: typing.Optional[schemas.Configuration] = None,
-                        ) -> 'any_of_1':
-                            return super().__new__(
-                                cls,
-                                arg,
-                                _configuration=_configuration,
-                            )
-                    
-                        def __getitem__(self, i: int) -> MetaOapg.items:
-                            return super().__getitem__(i)
                     
                     @classmethod
                     @functools.lru_cache()
-                    def any_of(cls):
+                    def all_of(cls):
                         # we need this here to make our import statements work
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            cls.any_of_0,
-                            cls.any_of_1,
+                            ModelEndpoints,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'stop':
+                ) -> 'endpoint':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            presence_penalty = schemas.NumberSchema
-            frequency_penalty = schemas.NumberSchema
-            other = schemas.DictSchema
-            display_name = schemas.StrSchema
             prompt_template = schemas.StrSchema
             
             
             class chat_template(
                 schemas.ListSchema
             ):
             
@@ -178,105 +144,135 @@
                         cls,
                         arg,
                         _configuration=_configuration,
                     )
             
                 def __getitem__(self, i: int) -> 'ChatMessage':
                     return super().__getitem__(i)
+            temperature = schemas.NumberSchema
+            max_tokens = schemas.IntSchema
+            top_p = schemas.NumberSchema
             
             
-            class endpoint(
+            class stop(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
+                    any_of_0 = schemas.StrSchema
+                    
+                    
+                    class any_of_1(
+                        schemas.ListSchema
+                    ):
+                    
+                    
+                        class MetaOapg:
+                            items = schemas.StrSchema
+                    
+                        def __new__(
+                            cls,
+                            arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
+                            _configuration: typing.Optional[schemas.Configuration] = None,
+                        ) -> 'any_of_1':
+                            return super().__new__(
+                                cls,
+                                arg,
+                                _configuration=_configuration,
+                            )
+                    
+                        def __getitem__(self, i: int) -> MetaOapg.items:
+                            return super().__getitem__(i)
                     
                     @classmethod
                     @functools.lru_cache()
-                    def all_of(cls):
+                    def any_of(cls):
                         # we need this here to make our import statements work
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            ModelEndpoints,
+                            cls.any_of_0,
+                            cls.any_of_1,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'endpoint':
+                ) -> 'stop':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
+            presence_penalty = schemas.NumberSchema
+            frequency_penalty = schemas.NumberSchema
+            other = schemas.DictSchema
+            display_name = schemas.StrSchema
             project_id = schemas.StrSchema
             project_name = schemas.StrSchema
             
             
             class feedback_stats(
                 schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
                     @staticmethod
-                    def items() -> typing.Type['SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse']:
-                        return SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse
+                    def items() -> typing.Type['SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse']:
+                        return SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse
             
                 def __new__(
                     cls,
-                    arg: typing.Union[typing.Tuple['SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse'], typing.List['SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse']],
+                    arg: typing.Union[typing.Tuple['SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse'], typing.List['SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                 ) -> 'feedback_stats':
                     return super().__new__(
                         cls,
                         arg,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> 'SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse':
+                def __getitem__(self, i: int) -> 'SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse':
                     return super().__getitem__(i)
             num_datapoints = schemas.IntSchema
             experiment_id = schemas.StrSchema
-            trial_id = schemas.StrSchema
             __annotations__ = {
                 "model": model,
                 "id": id,
                 "created_at": created_at,
                 "updated_at": updated_at,
                 "last_used": last_used,
                 "provider": provider,
-                "max_tokens": max_tokens,
+                "endpoint": endpoint,
+                "prompt_template": prompt_template,
+                "chat_template": chat_template,
                 "temperature": temperature,
+                "max_tokens": max_tokens,
                 "top_p": top_p,
                 "stop": stop,
                 "presence_penalty": presence_penalty,
                 "frequency_penalty": frequency_penalty,
                 "other": other,
                 "display_name": display_name,
-                "prompt_template": prompt_template,
-                "chat_template": chat_template,
-                "endpoint": endpoint,
                 "project_id": project_id,
                 "project_name": project_name,
                 "feedback_stats": feedback_stats,
                 "num_datapoints": num_datapoints,
                 "experiment_id": experiment_id,
-                "trial_id": trial_id,
             }
     
     updated_at: MetaOapg.properties.updated_at
     last_used: MetaOapg.properties.last_used
     created_at: MetaOapg.properties.created_at
     model: MetaOapg.properties.model
     id: MetaOapg.properties.id
@@ -296,20 +292,29 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["last_used"]) -> MetaOapg.properties.last_used: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["provider"]) -> MetaOapg.properties.provider: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["max_tokens"]) -> MetaOapg.properties.max_tokens: ...
+    def __getitem__(self, name: typing_extensions.Literal["endpoint"]) -> MetaOapg.properties.endpoint: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["prompt_template"]) -> MetaOapg.properties.prompt_template: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["chat_template"]) -> MetaOapg.properties.chat_template: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["temperature"]) -> MetaOapg.properties.temperature: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["max_tokens"]) -> MetaOapg.properties.max_tokens: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["top_p"]) -> MetaOapg.properties.top_p: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["stop"]) -> MetaOapg.properties.stop: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["presence_penalty"]) -> MetaOapg.properties.presence_penalty: ...
@@ -320,23 +325,14 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["display_name"]) -> MetaOapg.properties.display_name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["prompt_template"]) -> MetaOapg.properties.prompt_template: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["chat_template"]) -> MetaOapg.properties.chat_template: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["endpoint"]) -> MetaOapg.properties.endpoint: ...
-    
-    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["project_id"]) -> MetaOapg.properties.project_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["project_name"]) -> MetaOapg.properties.project_name: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["feedback_stats"]) -> MetaOapg.properties.feedback_stats: ...
@@ -344,20 +340,17 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["num_datapoints"]) -> MetaOapg.properties.num_datapoints: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["experiment_id"]) -> MetaOapg.properties.experiment_id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["trial_id"]) -> MetaOapg.properties.trial_id: ...
-    
-    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model", "id", "created_at", "updated_at", "last_used", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "display_name", "prompt_template", "chat_template", "endpoint", "project_id", "project_name", "feedback_stats", "num_datapoints", "experiment_id", "trial_id", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model", "id", "created_at", "updated_at", "last_used", "provider", "endpoint", "prompt_template", "chat_template", "temperature", "max_tokens", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "display_name", "project_id", "project_name", "feedback_stats", "num_datapoints", "experiment_id", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
     
@@ -373,20 +366,29 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["last_used"]) -> MetaOapg.properties.last_used: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["provider"]) -> typing.Union[MetaOapg.properties.provider, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["max_tokens"]) -> typing.Union[MetaOapg.properties.max_tokens, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["endpoint"]) -> typing.Union[MetaOapg.properties.endpoint, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["prompt_template"]) -> typing.Union[MetaOapg.properties.prompt_template, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["chat_template"]) -> typing.Union[MetaOapg.properties.chat_template, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["temperature"]) -> typing.Union[MetaOapg.properties.temperature, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["max_tokens"]) -> typing.Union[MetaOapg.properties.max_tokens, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["top_p"]) -> typing.Union[MetaOapg.properties.top_p, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["stop"]) -> typing.Union[MetaOapg.properties.stop, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["presence_penalty"]) -> typing.Union[MetaOapg.properties.presence_penalty, schemas.Unset]: ...
@@ -397,23 +399,14 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["display_name"]) -> typing.Union[MetaOapg.properties.display_name, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["prompt_template"]) -> typing.Union[MetaOapg.properties.prompt_template, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["chat_template"]) -> typing.Union[MetaOapg.properties.chat_template, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["endpoint"]) -> typing.Union[MetaOapg.properties.endpoint, schemas.Unset]: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["project_id"]) -> typing.Union[MetaOapg.properties.project_id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["project_name"]) -> typing.Union[MetaOapg.properties.project_name, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["feedback_stats"]) -> typing.Union[MetaOapg.properties.feedback_stats, schemas.Unset]: ...
@@ -421,79 +414,74 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["num_datapoints"]) -> typing.Union[MetaOapg.properties.num_datapoints, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["experiment_id"]) -> typing.Union[MetaOapg.properties.experiment_id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["trial_id"]) -> typing.Union[MetaOapg.properties.trial_id, schemas.Unset]: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model", "id", "created_at", "updated_at", "last_used", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "display_name", "prompt_template", "chat_template", "endpoint", "project_id", "project_name", "feedback_stats", "num_datapoints", "experiment_id", "trial_id", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model", "id", "created_at", "updated_at", "last_used", "provider", "endpoint", "prompt_template", "chat_template", "temperature", "max_tokens", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "display_name", "project_id", "project_name", "feedback_stats", "num_datapoints", "experiment_id", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         updated_at: typing.Union[MetaOapg.properties.updated_at, str, datetime, ],
         last_used: typing.Union[MetaOapg.properties.last_used, str, datetime, ],
         created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, ],
         model: typing.Union[MetaOapg.properties.model, str, ],
         id: typing.Union[MetaOapg.properties.id, str, ],
         provider: typing.Union[MetaOapg.properties.provider, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-        max_tokens: typing.Union[MetaOapg.properties.max_tokens, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        endpoint: typing.Union[MetaOapg.properties.endpoint, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        prompt_template: typing.Union[MetaOapg.properties.prompt_template, str, schemas.Unset] = schemas.unset,
+        chat_template: typing.Union[MetaOapg.properties.chat_template, list, tuple, schemas.Unset] = schemas.unset,
         temperature: typing.Union[MetaOapg.properties.temperature, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        max_tokens: typing.Union[MetaOapg.properties.max_tokens, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         top_p: typing.Union[MetaOapg.properties.top_p, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         stop: typing.Union[MetaOapg.properties.stop, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         presence_penalty: typing.Union[MetaOapg.properties.presence_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         frequency_penalty: typing.Union[MetaOapg.properties.frequency_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         display_name: typing.Union[MetaOapg.properties.display_name, str, schemas.Unset] = schemas.unset,
-        prompt_template: typing.Union[MetaOapg.properties.prompt_template, str, schemas.Unset] = schemas.unset,
-        chat_template: typing.Union[MetaOapg.properties.chat_template, list, tuple, schemas.Unset] = schemas.unset,
-        endpoint: typing.Union[MetaOapg.properties.endpoint, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         project_id: typing.Union[MetaOapg.properties.project_id, str, schemas.Unset] = schemas.unset,
         project_name: typing.Union[MetaOapg.properties.project_name, str, schemas.Unset] = schemas.unset,
         feedback_stats: typing.Union[MetaOapg.properties.feedback_stats, list, tuple, schemas.Unset] = schemas.unset,
         num_datapoints: typing.Union[MetaOapg.properties.num_datapoints, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         experiment_id: typing.Union[MetaOapg.properties.experiment_id, str, schemas.Unset] = schemas.unset,
-        trial_id: typing.Union[MetaOapg.properties.trial_id, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'GetModelConfigResponse':
+    ) -> 'ProjectModelConfigResponse':
         return super().__new__(
             cls,
             *args,
             updated_at=updated_at,
             last_used=last_used,
             created_at=created_at,
             model=model,
             id=id,
             provider=provider,
-            max_tokens=max_tokens,
+            endpoint=endpoint,
+            prompt_template=prompt_template,
+            chat_template=chat_template,
             temperature=temperature,
+            max_tokens=max_tokens,
             top_p=top_p,
             stop=stop,
             presence_penalty=presence_penalty,
             frequency_penalty=frequency_penalty,
             other=other,
             display_name=display_name,
-            prompt_template=prompt_template,
-            chat_template=chat_template,
-            endpoint=endpoint,
             project_id=project_id,
             project_name=project_name,
             feedback_stats=feedback_stats,
             num_datapoints=num_datapoints,
             experiment_id=experiment_id,
-            trial_id=trial_id,
             _configuration=_configuration,
             **kwargs,
         )
 
 from humanloop.model.chat_message import ChatMessage
 from humanloop.model.model_endpoints import ModelEndpoints
 from humanloop.model.model_providers import ModelProviders
-from humanloop.model.src_external_app_models_v4_model_configs_project_model_config_feedback_stats_response import SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse
+from humanloop.model.src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response import SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse
```

### Comparing `humanloop-0.4.2/humanloop/model/get_model_config_response.pyi` & `humanloop-0.4.3/humanloop/model/project_model_config_response.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,22 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class GetModelConfigResponse(
+class ProjectModelConfigResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
 
-    A selected model configuration.
-
-If the model configuration was selected in the context of an experiment,
-the response will include a trial_id to associate a subsequent log() call.
+    Extends the core ModelConfig request object to include Humanloop generated
+identifier and method for serializing response from ModelConfig domain object.
     """
 
 
     class MetaOapg:
         required = {
             "updated_at",
             "last_used",
@@ -83,82 +81,50 @@
                 ) -> 'provider':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            max_tokens = schemas.IntSchema
-            temperature = schemas.NumberSchema
-            top_p = schemas.NumberSchema
             
             
-            class stop(
+            class endpoint(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
-                    any_of_0 = schemas.StrSchema
-                    
-                    
-                    class any_of_1(
-                        schemas.ListSchema
-                    ):
-                    
-                    
-                        class MetaOapg:
-                            items = schemas.StrSchema
-                    
-                        def __new__(
-                            cls,
-                            arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
-                            _configuration: typing.Optional[schemas.Configuration] = None,
-                        ) -> 'any_of_1':
-                            return super().__new__(
-                                cls,
-                                arg,
-                                _configuration=_configuration,
-                            )
-                    
-                        def __getitem__(self, i: int) -> MetaOapg.items:
-                            return super().__getitem__(i)
                     
                     @classmethod
                     @functools.lru_cache()
-                    def any_of(cls):
+                    def all_of(cls):
                         # we need this here to make our import statements work
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            cls.any_of_0,
-                            cls.any_of_1,
+                            ModelEndpoints,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'stop':
+                ) -> 'endpoint':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            presence_penalty = schemas.NumberSchema
-            frequency_penalty = schemas.NumberSchema
-            other = schemas.DictSchema
-            display_name = schemas.StrSchema
             prompt_template = schemas.StrSchema
             
             
             class chat_template(
                 schemas.ListSchema
             ):
             
@@ -178,105 +144,135 @@
                         cls,
                         arg,
                         _configuration=_configuration,
                     )
             
                 def __getitem__(self, i: int) -> 'ChatMessage':
                     return super().__getitem__(i)
+            temperature = schemas.NumberSchema
+            max_tokens = schemas.IntSchema
+            top_p = schemas.NumberSchema
             
             
-            class endpoint(
+            class stop(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
+                    any_of_0 = schemas.StrSchema
+                    
+                    
+                    class any_of_1(
+                        schemas.ListSchema
+                    ):
+                    
+                    
+                        class MetaOapg:
+                            items = schemas.StrSchema
+                    
+                        def __new__(
+                            cls,
+                            arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
+                            _configuration: typing.Optional[schemas.Configuration] = None,
+                        ) -> 'any_of_1':
+                            return super().__new__(
+                                cls,
+                                arg,
+                                _configuration=_configuration,
+                            )
+                    
+                        def __getitem__(self, i: int) -> MetaOapg.items:
+                            return super().__getitem__(i)
                     
                     @classmethod
                     @functools.lru_cache()
-                    def all_of(cls):
+                    def any_of(cls):
                         # we need this here to make our import statements work
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            ModelEndpoints,
+                            cls.any_of_0,
+                            cls.any_of_1,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'endpoint':
+                ) -> 'stop':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
+            presence_penalty = schemas.NumberSchema
+            frequency_penalty = schemas.NumberSchema
+            other = schemas.DictSchema
+            display_name = schemas.StrSchema
             project_id = schemas.StrSchema
             project_name = schemas.StrSchema
             
             
             class feedback_stats(
                 schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
                     @staticmethod
-                    def items() -> typing.Type['SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse']:
-                        return SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse
+                    def items() -> typing.Type['SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse']:
+                        return SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse
             
                 def __new__(
                     cls,
-                    arg: typing.Union[typing.Tuple['SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse'], typing.List['SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse']],
+                    arg: typing.Union[typing.Tuple['SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse'], typing.List['SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                 ) -> 'feedback_stats':
                     return super().__new__(
                         cls,
                         arg,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> 'SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse':
+                def __getitem__(self, i: int) -> 'SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse':
                     return super().__getitem__(i)
             num_datapoints = schemas.IntSchema
             experiment_id = schemas.StrSchema
-            trial_id = schemas.StrSchema
             __annotations__ = {
                 "model": model,
                 "id": id,
                 "created_at": created_at,
                 "updated_at": updated_at,
                 "last_used": last_used,
                 "provider": provider,
-                "max_tokens": max_tokens,
+                "endpoint": endpoint,
+                "prompt_template": prompt_template,
+                "chat_template": chat_template,
                 "temperature": temperature,
+                "max_tokens": max_tokens,
                 "top_p": top_p,
                 "stop": stop,
                 "presence_penalty": presence_penalty,
                 "frequency_penalty": frequency_penalty,
                 "other": other,
                 "display_name": display_name,
-                "prompt_template": prompt_template,
-                "chat_template": chat_template,
-                "endpoint": endpoint,
                 "project_id": project_id,
                 "project_name": project_name,
                 "feedback_stats": feedback_stats,
                 "num_datapoints": num_datapoints,
                 "experiment_id": experiment_id,
-                "trial_id": trial_id,
             }
     
     updated_at: MetaOapg.properties.updated_at
     last_used: MetaOapg.properties.last_used
     created_at: MetaOapg.properties.created_at
     model: MetaOapg.properties.model
     id: MetaOapg.properties.id
@@ -296,20 +292,29 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["last_used"]) -> MetaOapg.properties.last_used: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["provider"]) -> MetaOapg.properties.provider: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["max_tokens"]) -> MetaOapg.properties.max_tokens: ...
+    def __getitem__(self, name: typing_extensions.Literal["endpoint"]) -> MetaOapg.properties.endpoint: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["prompt_template"]) -> MetaOapg.properties.prompt_template: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["chat_template"]) -> MetaOapg.properties.chat_template: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["temperature"]) -> MetaOapg.properties.temperature: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["max_tokens"]) -> MetaOapg.properties.max_tokens: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["top_p"]) -> MetaOapg.properties.top_p: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["stop"]) -> MetaOapg.properties.stop: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["presence_penalty"]) -> MetaOapg.properties.presence_penalty: ...
@@ -320,23 +325,14 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["display_name"]) -> MetaOapg.properties.display_name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["prompt_template"]) -> MetaOapg.properties.prompt_template: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["chat_template"]) -> MetaOapg.properties.chat_template: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["endpoint"]) -> MetaOapg.properties.endpoint: ...
-    
-    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["project_id"]) -> MetaOapg.properties.project_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["project_name"]) -> MetaOapg.properties.project_name: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["feedback_stats"]) -> MetaOapg.properties.feedback_stats: ...
@@ -344,20 +340,17 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["num_datapoints"]) -> MetaOapg.properties.num_datapoints: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["experiment_id"]) -> MetaOapg.properties.experiment_id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["trial_id"]) -> MetaOapg.properties.trial_id: ...
-    
-    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model", "id", "created_at", "updated_at", "last_used", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "display_name", "prompt_template", "chat_template", "endpoint", "project_id", "project_name", "feedback_stats", "num_datapoints", "experiment_id", "trial_id", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model", "id", "created_at", "updated_at", "last_used", "provider", "endpoint", "prompt_template", "chat_template", "temperature", "max_tokens", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "display_name", "project_id", "project_name", "feedback_stats", "num_datapoints", "experiment_id", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
     
@@ -373,20 +366,29 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["last_used"]) -> MetaOapg.properties.last_used: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["provider"]) -> typing.Union[MetaOapg.properties.provider, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["max_tokens"]) -> typing.Union[MetaOapg.properties.max_tokens, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["endpoint"]) -> typing.Union[MetaOapg.properties.endpoint, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["prompt_template"]) -> typing.Union[MetaOapg.properties.prompt_template, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["chat_template"]) -> typing.Union[MetaOapg.properties.chat_template, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["temperature"]) -> typing.Union[MetaOapg.properties.temperature, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["max_tokens"]) -> typing.Union[MetaOapg.properties.max_tokens, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["top_p"]) -> typing.Union[MetaOapg.properties.top_p, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["stop"]) -> typing.Union[MetaOapg.properties.stop, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["presence_penalty"]) -> typing.Union[MetaOapg.properties.presence_penalty, schemas.Unset]: ...
@@ -397,23 +399,14 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["display_name"]) -> typing.Union[MetaOapg.properties.display_name, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["prompt_template"]) -> typing.Union[MetaOapg.properties.prompt_template, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["chat_template"]) -> typing.Union[MetaOapg.properties.chat_template, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["endpoint"]) -> typing.Union[MetaOapg.properties.endpoint, schemas.Unset]: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["project_id"]) -> typing.Union[MetaOapg.properties.project_id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["project_name"]) -> typing.Union[MetaOapg.properties.project_name, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["feedback_stats"]) -> typing.Union[MetaOapg.properties.feedback_stats, schemas.Unset]: ...
@@ -421,79 +414,74 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["num_datapoints"]) -> typing.Union[MetaOapg.properties.num_datapoints, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["experiment_id"]) -> typing.Union[MetaOapg.properties.experiment_id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["trial_id"]) -> typing.Union[MetaOapg.properties.trial_id, schemas.Unset]: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model", "id", "created_at", "updated_at", "last_used", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "display_name", "prompt_template", "chat_template", "endpoint", "project_id", "project_name", "feedback_stats", "num_datapoints", "experiment_id", "trial_id", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model", "id", "created_at", "updated_at", "last_used", "provider", "endpoint", "prompt_template", "chat_template", "temperature", "max_tokens", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "display_name", "project_id", "project_name", "feedback_stats", "num_datapoints", "experiment_id", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         updated_at: typing.Union[MetaOapg.properties.updated_at, str, datetime, ],
         last_used: typing.Union[MetaOapg.properties.last_used, str, datetime, ],
         created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, ],
         model: typing.Union[MetaOapg.properties.model, str, ],
         id: typing.Union[MetaOapg.properties.id, str, ],
         provider: typing.Union[MetaOapg.properties.provider, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-        max_tokens: typing.Union[MetaOapg.properties.max_tokens, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        endpoint: typing.Union[MetaOapg.properties.endpoint, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        prompt_template: typing.Union[MetaOapg.properties.prompt_template, str, schemas.Unset] = schemas.unset,
+        chat_template: typing.Union[MetaOapg.properties.chat_template, list, tuple, schemas.Unset] = schemas.unset,
         temperature: typing.Union[MetaOapg.properties.temperature, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        max_tokens: typing.Union[MetaOapg.properties.max_tokens, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         top_p: typing.Union[MetaOapg.properties.top_p, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         stop: typing.Union[MetaOapg.properties.stop, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         presence_penalty: typing.Union[MetaOapg.properties.presence_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         frequency_penalty: typing.Union[MetaOapg.properties.frequency_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         display_name: typing.Union[MetaOapg.properties.display_name, str, schemas.Unset] = schemas.unset,
-        prompt_template: typing.Union[MetaOapg.properties.prompt_template, str, schemas.Unset] = schemas.unset,
-        chat_template: typing.Union[MetaOapg.properties.chat_template, list, tuple, schemas.Unset] = schemas.unset,
-        endpoint: typing.Union[MetaOapg.properties.endpoint, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         project_id: typing.Union[MetaOapg.properties.project_id, str, schemas.Unset] = schemas.unset,
         project_name: typing.Union[MetaOapg.properties.project_name, str, schemas.Unset] = schemas.unset,
         feedback_stats: typing.Union[MetaOapg.properties.feedback_stats, list, tuple, schemas.Unset] = schemas.unset,
         num_datapoints: typing.Union[MetaOapg.properties.num_datapoints, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         experiment_id: typing.Union[MetaOapg.properties.experiment_id, str, schemas.Unset] = schemas.unset,
-        trial_id: typing.Union[MetaOapg.properties.trial_id, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'GetModelConfigResponse':
+    ) -> 'ProjectModelConfigResponse':
         return super().__new__(
             cls,
             *args,
             updated_at=updated_at,
             last_used=last_used,
             created_at=created_at,
             model=model,
             id=id,
             provider=provider,
-            max_tokens=max_tokens,
+            endpoint=endpoint,
+            prompt_template=prompt_template,
+            chat_template=chat_template,
             temperature=temperature,
+            max_tokens=max_tokens,
             top_p=top_p,
             stop=stop,
             presence_penalty=presence_penalty,
             frequency_penalty=frequency_penalty,
             other=other,
             display_name=display_name,
-            prompt_template=prompt_template,
-            chat_template=chat_template,
-            endpoint=endpoint,
             project_id=project_id,
             project_name=project_name,
             feedback_stats=feedback_stats,
             num_datapoints=num_datapoints,
             experiment_id=experiment_id,
-            trial_id=trial_id,
             _configuration=_configuration,
             **kwargs,
         )
 
 from humanloop.model.chat_message import ChatMessage
 from humanloop.model.model_endpoints import ModelEndpoints
 from humanloop.model.model_providers import ModelProviders
-from humanloop.model.src_external_app_models_v4_model_configs_project_model_config_feedback_stats_response import SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse
+from humanloop.model.src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response import SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse
```

### Comparing `humanloop-0.4.2/humanloop/model/http_validation_error.py` & `humanloop-0.4.3/humanloop/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/http_validation_error.pyi` & `humanloop-0.4.3/humanloop/model/http_validation_error.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/label_sentiment.py` & `humanloop-0.4.3/humanloop/model/label_sentiment.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/label_sentiment.pyi` & `humanloop-0.4.3/humanloop/model/label_sentiment.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/log_datapoint_request.py` & `humanloop-0.4.3/humanloop/model/log_datapoint_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/log_datapoint_request.pyi` & `humanloop-0.4.3/humanloop/model/log_datapoint_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/log_request.py` & `humanloop-0.4.3/humanloop/model/log_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,20 +30,19 @@
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
             "output",
-            "project",
         }
         
         class properties:
-            project = schemas.StrSchema
             output = schemas.StrSchema
+            project = schemas.StrSchema
             session_id = schemas.StrSchema
             parent_id = schemas.StrSchema
             trial_id = schemas.StrSchema
             inputs = schemas.DictSchema
             
             
             class messages(
@@ -69,43 +68,45 @@
                     )
             
                 def __getitem__(self, i: int) -> 'ChatMessage':
                     return super().__getitem__(i)
             source = schemas.StrSchema
             
             
-            class model_config(
+            class config(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
                     
                     @classmethod
                     @functools.lru_cache()
-                    def any_of(cls):
+                    def one_of(cls):
                         # we need this here to make our import statements work
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            ModelConfigCompletionRequest,
-                            ModelConfigChatRequest,
+                            TraceModelConfigRequest,
+                            ToolConfigRequest,
+                            GenericConfigRequest,
+                            AgentConfigRequest,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'model_config':
+                ) -> 'config':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             metadata = schemas.DictSchema
@@ -169,37 +170,40 @@
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             created_at = schemas.DateTimeSchema
+            error = schemas.StrSchema
+            duration = schemas.NumberSchema
             __annotations__ = {
-                "project": project,
                 "output": output,
+                "project": project,
                 "session_id": session_id,
                 "parent_id": parent_id,
                 "trial_id": trial_id,
                 "inputs": inputs,
                 "messages": messages,
                 "source": source,
-                "model_config": model_config,
+                "config": config,
                 "metadata": metadata,
                 "feedback": feedback,
                 "created_at": created_at,
+                "error": error,
+                "duration": duration,
             }
     
     output: MetaOapg.properties.output
-    project: MetaOapg.properties.project
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
+    def __getitem__(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
+    def __getitem__(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["session_id"]) -> MetaOapg.properties.session_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["parent_id"]) -> MetaOapg.properties.parent_id: ...
     
@@ -212,38 +216,44 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
+    def __getitem__(self, name: typing_extensions.Literal["config"]) -> MetaOapg.properties.config: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["metadata"]) -> MetaOapg.properties.metadata: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["feedback"]) -> MetaOapg.properties.feedback: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["error"]) -> MetaOapg.properties.error: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["duration"]) -> MetaOapg.properties.duration: ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["project", "output", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "model_config", "metadata", "feedback", "created_at", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["output", "project", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "config", "metadata", "feedback", "created_at", "error", "duration", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["project"]) -> typing.Union[MetaOapg.properties.project, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["session_id"]) -> typing.Union[MetaOapg.properties.session_id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["parent_id"]) -> typing.Union[MetaOapg.properties.parent_id, schemas.Unset]: ...
     
@@ -256,66 +266,78 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["messages"]) -> typing.Union[MetaOapg.properties.messages, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["model_config"]) -> typing.Union[MetaOapg.properties.model_config, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["config"]) -> typing.Union[MetaOapg.properties.config, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["metadata"]) -> typing.Union[MetaOapg.properties.metadata, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["feedback"]) -> typing.Union[MetaOapg.properties.feedback, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["created_at"]) -> typing.Union[MetaOapg.properties.created_at, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["error"]) -> typing.Union[MetaOapg.properties.error, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["duration"]) -> typing.Union[MetaOapg.properties.duration, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["project", "output", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "model_config", "metadata", "feedback", "created_at", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["output", "project", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "config", "metadata", "feedback", "created_at", "error", "duration", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         output: typing.Union[MetaOapg.properties.output, str, ],
-        project: typing.Union[MetaOapg.properties.project, str, ],
+        project: typing.Union[MetaOapg.properties.project, str, schemas.Unset] = schemas.unset,
         session_id: typing.Union[MetaOapg.properties.session_id, str, schemas.Unset] = schemas.unset,
         parent_id: typing.Union[MetaOapg.properties.parent_id, str, schemas.Unset] = schemas.unset,
         trial_id: typing.Union[MetaOapg.properties.trial_id, str, schemas.Unset] = schemas.unset,
         inputs: typing.Union[MetaOapg.properties.inputs, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         messages: typing.Union[MetaOapg.properties.messages, list, tuple, schemas.Unset] = schemas.unset,
         source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
-        model_config: typing.Union[MetaOapg.properties.model_config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        config: typing.Union[MetaOapg.properties.config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         metadata: typing.Union[MetaOapg.properties.metadata, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         feedback: typing.Union[MetaOapg.properties.feedback, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, schemas.Unset] = schemas.unset,
+        error: typing.Union[MetaOapg.properties.error, str, schemas.Unset] = schemas.unset,
+        duration: typing.Union[MetaOapg.properties.duration, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'LogRequest':
         return super().__new__(
             cls,
             *args,
             output=output,
             project=project,
             session_id=session_id,
             parent_id=parent_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             source=source,
-            model_config=model_config,
+            config=config,
             metadata=metadata,
             feedback=feedback,
             created_at=created_at,
+            error=error,
+            duration=duration,
             _configuration=_configuration,
             **kwargs,
         )
 
+from humanloop.model.agent_config_request import AgentConfigRequest
 from humanloop.model.chat_message import ChatMessage
 from humanloop.model.feedback import Feedback
-from humanloop.model.model_config_chat_request import ModelConfigChatRequest
-from humanloop.model.model_config_completion_request import ModelConfigCompletionRequest
+from humanloop.model.generic_config_request import GenericConfigRequest
+from humanloop.model.tool_config_request import ToolConfigRequest
+from humanloop.model.trace_model_config_request import TraceModelConfigRequest
```

### Comparing `humanloop-0.4.2/humanloop/model/log_request.pyi` & `humanloop-0.4.3/humanloop/model/log_request.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -30,20 +30,19 @@
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
             "output",
-            "project",
         }
         
         class properties:
-            project = schemas.StrSchema
             output = schemas.StrSchema
+            project = schemas.StrSchema
             session_id = schemas.StrSchema
             parent_id = schemas.StrSchema
             trial_id = schemas.StrSchema
             inputs = schemas.DictSchema
             
             
             class messages(
@@ -69,43 +68,45 @@
                     )
             
                 def __getitem__(self, i: int) -> 'ChatMessage':
                     return super().__getitem__(i)
             source = schemas.StrSchema
             
             
-            class model_config(
+            class config(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
                     
                     @classmethod
                     @functools.lru_cache()
-                    def any_of(cls):
+                    def one_of(cls):
                         # we need this here to make our import statements work
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            ModelConfigCompletionRequest,
-                            ModelConfigChatRequest,
+                            TraceModelConfigRequest,
+                            ToolConfigRequest,
+                            GenericConfigRequest,
+                            AgentConfigRequest,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'model_config':
+                ) -> 'config':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             metadata = schemas.DictSchema
@@ -169,37 +170,40 @@
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             created_at = schemas.DateTimeSchema
+            error = schemas.StrSchema
+            duration = schemas.NumberSchema
             __annotations__ = {
-                "project": project,
                 "output": output,
+                "project": project,
                 "session_id": session_id,
                 "parent_id": parent_id,
                 "trial_id": trial_id,
                 "inputs": inputs,
                 "messages": messages,
                 "source": source,
-                "model_config": model_config,
+                "config": config,
                 "metadata": metadata,
                 "feedback": feedback,
                 "created_at": created_at,
+                "error": error,
+                "duration": duration,
             }
     
     output: MetaOapg.properties.output
-    project: MetaOapg.properties.project
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
+    def __getitem__(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
+    def __getitem__(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["session_id"]) -> MetaOapg.properties.session_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["parent_id"]) -> MetaOapg.properties.parent_id: ...
     
@@ -212,38 +216,44 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
+    def __getitem__(self, name: typing_extensions.Literal["config"]) -> MetaOapg.properties.config: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["metadata"]) -> MetaOapg.properties.metadata: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["feedback"]) -> MetaOapg.properties.feedback: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["error"]) -> MetaOapg.properties.error: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["duration"]) -> MetaOapg.properties.duration: ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["project", "output", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "model_config", "metadata", "feedback", "created_at", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["output", "project", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "config", "metadata", "feedback", "created_at", "error", "duration", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["project"]) -> typing.Union[MetaOapg.properties.project, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["session_id"]) -> typing.Union[MetaOapg.properties.session_id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["parent_id"]) -> typing.Union[MetaOapg.properties.parent_id, schemas.Unset]: ...
     
@@ -256,66 +266,78 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["messages"]) -> typing.Union[MetaOapg.properties.messages, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["model_config"]) -> typing.Union[MetaOapg.properties.model_config, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["config"]) -> typing.Union[MetaOapg.properties.config, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["metadata"]) -> typing.Union[MetaOapg.properties.metadata, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["feedback"]) -> typing.Union[MetaOapg.properties.feedback, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["created_at"]) -> typing.Union[MetaOapg.properties.created_at, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["error"]) -> typing.Union[MetaOapg.properties.error, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["duration"]) -> typing.Union[MetaOapg.properties.duration, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["project", "output", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "model_config", "metadata", "feedback", "created_at", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["output", "project", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "config", "metadata", "feedback", "created_at", "error", "duration", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         output: typing.Union[MetaOapg.properties.output, str, ],
-        project: typing.Union[MetaOapg.properties.project, str, ],
+        project: typing.Union[MetaOapg.properties.project, str, schemas.Unset] = schemas.unset,
         session_id: typing.Union[MetaOapg.properties.session_id, str, schemas.Unset] = schemas.unset,
         parent_id: typing.Union[MetaOapg.properties.parent_id, str, schemas.Unset] = schemas.unset,
         trial_id: typing.Union[MetaOapg.properties.trial_id, str, schemas.Unset] = schemas.unset,
         inputs: typing.Union[MetaOapg.properties.inputs, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         messages: typing.Union[MetaOapg.properties.messages, list, tuple, schemas.Unset] = schemas.unset,
         source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
-        model_config: typing.Union[MetaOapg.properties.model_config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        config: typing.Union[MetaOapg.properties.config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         metadata: typing.Union[MetaOapg.properties.metadata, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         feedback: typing.Union[MetaOapg.properties.feedback, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, schemas.Unset] = schemas.unset,
+        error: typing.Union[MetaOapg.properties.error, str, schemas.Unset] = schemas.unset,
+        duration: typing.Union[MetaOapg.properties.duration, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'LogRequest':
         return super().__new__(
             cls,
             *args,
             output=output,
             project=project,
             session_id=session_id,
             parent_id=parent_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             source=source,
-            model_config=model_config,
+            config=config,
             metadata=metadata,
             feedback=feedback,
             created_at=created_at,
+            error=error,
+            duration=duration,
             _configuration=_configuration,
             **kwargs,
         )
 
+from humanloop.model.agent_config_request import AgentConfigRequest
 from humanloop.model.chat_message import ChatMessage
 from humanloop.model.feedback import Feedback
-from humanloop.model.model_config_chat_request import ModelConfigChatRequest
-from humanloop.model.model_config_completion_request import ModelConfigCompletionRequest
+from humanloop.model.generic_config_request import GenericConfigRequest
+from humanloop.model.tool_config_request import ToolConfigRequest
+from humanloop.model.trace_model_config_request import TraceModelConfigRequest
```

### Comparing `humanloop-0.4.2/humanloop/model/log_response.py` & `humanloop-0.4.3/humanloop/model/log_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,19 +33,24 @@
 
     class MetaOapg:
         required = {
             "output",
             "project_id",
             "project",
             "id",
+            "config",
         }
         
         class properties:
             project = schemas.StrSchema
             output = schemas.StrSchema
+        
+            @staticmethod
+            def config() -> typing.Type['ConfigResponse']:
+                return ConfigResponse
             id = schemas.StrSchema
             project_id = schemas.StrSchema
             session_id = schemas.StrSchema
             parent_id = schemas.StrSchema
             trial_id = schemas.StrSchema
             inputs = schemas.DictSchema
             
@@ -71,50 +76,14 @@
                         arg,
                         _configuration=_configuration,
                     )
             
                 def __getitem__(self, i: int) -> 'ChatMessage':
                     return super().__getitem__(i)
             source = schemas.StrSchema
-            
-            
-            class model_config(
-                schemas.ComposedSchema,
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    @classmethod
-                    @functools.lru_cache()
-                    def all_of(cls):
-                        # we need this here to make our import statements work
-                        # we must store _composed_schemas in here so the code is only run
-                        # when we invoke this method. If we kept this at the class
-                        # level we would get an error because the class level
-                        # code would be run when this module is imported, and these composed
-                        # classes don't exist yet because their module has not finished
-                        # loading
-                        return [
-                            SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse,
-                        ]
-            
-            
-                def __new__(
-                    cls,
-                    *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'model_config':
-                    return super().__new__(
-                        cls,
-                        *args,
-                        _configuration=_configuration,
-                        **kwargs,
-                    )
             metadata = schemas.DictSchema
             
             
             class feedback(
                 schemas.ComposedSchema,
             ):
             
@@ -172,53 +141,98 @@
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             created_at = schemas.DateTimeSchema
+            error = schemas.StrSchema
+            duration = schemas.NumberSchema
+            
+            
+            class model_config(
+                schemas.ComposedSchema,
+            ):
+            
+            
+                class MetaOapg:
+                    
+                    @classmethod
+                    @functools.lru_cache()
+                    def all_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            ProjectConfigResponse,
+                        ]
+            
+            
+                def __new__(
+                    cls,
+                    *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+                ) -> 'model_config':
+                    return super().__new__(
+                        cls,
+                        *args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
             user = schemas.StrSchema
             provider_response = schemas.DictSchema
             provider_latency = schemas.NumberSchema
             raw_output = schemas.StrSchema
             finish_reason = schemas.StrSchema
             __annotations__ = {
                 "project": project,
                 "output": output,
+                "config": config,
                 "id": id,
                 "project_id": project_id,
                 "session_id": session_id,
                 "parent_id": parent_id,
                 "trial_id": trial_id,
                 "inputs": inputs,
                 "messages": messages,
                 "source": source,
-                "model_config": model_config,
                 "metadata": metadata,
                 "feedback": feedback,
                 "created_at": created_at,
+                "error": error,
+                "duration": duration,
+                "model_config": model_config,
                 "user": user,
                 "provider_response": provider_response,
                 "provider_latency": provider_latency,
                 "raw_output": raw_output,
                 "finish_reason": finish_reason,
             }
     
     output: MetaOapg.properties.output
     project_id: MetaOapg.properties.project_id
     project: MetaOapg.properties.project
     id: MetaOapg.properties.id
+    config: 'ConfigResponse'
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["config"]) -> 'ConfigResponse': ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["project_id"]) -> MetaOapg.properties.project_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["session_id"]) -> MetaOapg.properties.session_id: ...
@@ -235,26 +249,32 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
-    
-    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["metadata"]) -> MetaOapg.properties.metadata: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["feedback"]) -> MetaOapg.properties.feedback: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["error"]) -> MetaOapg.properties.error: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["duration"]) -> MetaOapg.properties.duration: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["user"]) -> MetaOapg.properties.user: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["provider_response"]) -> MetaOapg.properties.provider_response: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["provider_latency"]) -> MetaOapg.properties.provider_latency: ...
@@ -264,26 +284,29 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["finish_reason"]) -> MetaOapg.properties.finish_reason: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["project", "output", "id", "project_id", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "model_config", "metadata", "feedback", "created_at", "user", "provider_response", "provider_latency", "raw_output", "finish_reason", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["project", "output", "config", "id", "project_id", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "metadata", "feedback", "created_at", "error", "duration", "model_config", "user", "provider_response", "provider_latency", "raw_output", "finish_reason", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["config"]) -> 'ConfigResponse': ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["project_id"]) -> MetaOapg.properties.project_id: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["session_id"]) -> typing.Union[MetaOapg.properties.session_id, schemas.Unset]: ...
@@ -300,26 +323,32 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["messages"]) -> typing.Union[MetaOapg.properties.messages, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["model_config"]) -> typing.Union[MetaOapg.properties.model_config, schemas.Unset]: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["metadata"]) -> typing.Union[MetaOapg.properties.metadata, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["feedback"]) -> typing.Union[MetaOapg.properties.feedback, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["created_at"]) -> typing.Union[MetaOapg.properties.created_at, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["error"]) -> typing.Union[MetaOapg.properties.error, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["duration"]) -> typing.Union[MetaOapg.properties.duration, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["model_config"]) -> typing.Union[MetaOapg.properties.model_config, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["user"]) -> typing.Union[MetaOapg.properties.user, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["provider_response"]) -> typing.Union[MetaOapg.properties.provider_response, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["provider_latency"]) -> typing.Union[MetaOapg.properties.provider_latency, schemas.Unset]: ...
@@ -329,35 +358,38 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["finish_reason"]) -> typing.Union[MetaOapg.properties.finish_reason, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["project", "output", "id", "project_id", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "model_config", "metadata", "feedback", "created_at", "user", "provider_response", "provider_latency", "raw_output", "finish_reason", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["project", "output", "config", "id", "project_id", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "metadata", "feedback", "created_at", "error", "duration", "model_config", "user", "provider_response", "provider_latency", "raw_output", "finish_reason", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         output: typing.Union[MetaOapg.properties.output, str, ],
         project_id: typing.Union[MetaOapg.properties.project_id, str, ],
         project: typing.Union[MetaOapg.properties.project, str, ],
         id: typing.Union[MetaOapg.properties.id, str, ],
+        config: 'ConfigResponse',
         session_id: typing.Union[MetaOapg.properties.session_id, str, schemas.Unset] = schemas.unset,
         parent_id: typing.Union[MetaOapg.properties.parent_id, str, schemas.Unset] = schemas.unset,
         trial_id: typing.Union[MetaOapg.properties.trial_id, str, schemas.Unset] = schemas.unset,
         inputs: typing.Union[MetaOapg.properties.inputs, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         messages: typing.Union[MetaOapg.properties.messages, list, tuple, schemas.Unset] = schemas.unset,
         source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
-        model_config: typing.Union[MetaOapg.properties.model_config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         metadata: typing.Union[MetaOapg.properties.metadata, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         feedback: typing.Union[MetaOapg.properties.feedback, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, schemas.Unset] = schemas.unset,
+        error: typing.Union[MetaOapg.properties.error, str, schemas.Unset] = schemas.unset,
+        duration: typing.Union[MetaOapg.properties.duration, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        model_config: typing.Union[MetaOapg.properties.model_config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         user: typing.Union[MetaOapg.properties.user, str, schemas.Unset] = schemas.unset,
         provider_response: typing.Union[MetaOapg.properties.provider_response, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         provider_latency: typing.Union[MetaOapg.properties.provider_latency, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         raw_output: typing.Union[MetaOapg.properties.raw_output, str, schemas.Unset] = schemas.unset,
         finish_reason: typing.Union[MetaOapg.properties.finish_reason, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
@@ -365,29 +397,33 @@
         return super().__new__(
             cls,
             *args,
             output=output,
             project_id=project_id,
             project=project,
             id=id,
+            config=config,
             session_id=session_id,
             parent_id=parent_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             source=source,
-            model_config=model_config,
             metadata=metadata,
             feedback=feedback,
             created_at=created_at,
+            error=error,
+            duration=duration,
+            model_config=model_config,
             user=user,
             provider_response=provider_response,
             provider_latency=provider_latency,
             raw_output=raw_output,
             finish_reason=finish_reason,
             _configuration=_configuration,
             **kwargs,
         )
 
 from humanloop.model.chat_message import ChatMessage
+from humanloop.model.config_response import ConfigResponse
 from humanloop.model.feedback import Feedback
-from humanloop.model.src_external_app_models_v4_model_configs_project_model_config_response import SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse
+from humanloop.model.project_config_response import ProjectConfigResponse
```

### Comparing `humanloop-0.4.2/humanloop/model/log_response.pyi` & `humanloop-0.4.3/humanloop/model/log_response.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -33,19 +33,24 @@
 
     class MetaOapg:
         required = {
             "output",
             "project_id",
             "project",
             "id",
+            "config",
         }
         
         class properties:
             project = schemas.StrSchema
             output = schemas.StrSchema
+        
+            @staticmethod
+            def config() -> typing.Type['ConfigResponse']:
+                return ConfigResponse
             id = schemas.StrSchema
             project_id = schemas.StrSchema
             session_id = schemas.StrSchema
             parent_id = schemas.StrSchema
             trial_id = schemas.StrSchema
             inputs = schemas.DictSchema
             
@@ -71,50 +76,14 @@
                         arg,
                         _configuration=_configuration,
                     )
             
                 def __getitem__(self, i: int) -> 'ChatMessage':
                     return super().__getitem__(i)
             source = schemas.StrSchema
-            
-            
-            class model_config(
-                schemas.ComposedSchema,
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    @classmethod
-                    @functools.lru_cache()
-                    def all_of(cls):
-                        # we need this here to make our import statements work
-                        # we must store _composed_schemas in here so the code is only run
-                        # when we invoke this method. If we kept this at the class
-                        # level we would get an error because the class level
-                        # code would be run when this module is imported, and these composed
-                        # classes don't exist yet because their module has not finished
-                        # loading
-                        return [
-                            SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse,
-                        ]
-            
-            
-                def __new__(
-                    cls,
-                    *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'model_config':
-                    return super().__new__(
-                        cls,
-                        *args,
-                        _configuration=_configuration,
-                        **kwargs,
-                    )
             metadata = schemas.DictSchema
             
             
             class feedback(
                 schemas.ComposedSchema,
             ):
             
@@ -172,53 +141,98 @@
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             created_at = schemas.DateTimeSchema
+            error = schemas.StrSchema
+            duration = schemas.NumberSchema
+            
+            
+            class model_config(
+                schemas.ComposedSchema,
+            ):
+            
+            
+                class MetaOapg:
+                    
+                    @classmethod
+                    @functools.lru_cache()
+                    def all_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            ProjectConfigResponse,
+                        ]
+            
+            
+                def __new__(
+                    cls,
+                    *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+                ) -> 'model_config':
+                    return super().__new__(
+                        cls,
+                        *args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
             user = schemas.StrSchema
             provider_response = schemas.DictSchema
             provider_latency = schemas.NumberSchema
             raw_output = schemas.StrSchema
             finish_reason = schemas.StrSchema
             __annotations__ = {
                 "project": project,
                 "output": output,
+                "config": config,
                 "id": id,
                 "project_id": project_id,
                 "session_id": session_id,
                 "parent_id": parent_id,
                 "trial_id": trial_id,
                 "inputs": inputs,
                 "messages": messages,
                 "source": source,
-                "model_config": model_config,
                 "metadata": metadata,
                 "feedback": feedback,
                 "created_at": created_at,
+                "error": error,
+                "duration": duration,
+                "model_config": model_config,
                 "user": user,
                 "provider_response": provider_response,
                 "provider_latency": provider_latency,
                 "raw_output": raw_output,
                 "finish_reason": finish_reason,
             }
     
     output: MetaOapg.properties.output
     project_id: MetaOapg.properties.project_id
     project: MetaOapg.properties.project
     id: MetaOapg.properties.id
+    config: 'ConfigResponse'
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["config"]) -> 'ConfigResponse': ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["project_id"]) -> MetaOapg.properties.project_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["session_id"]) -> MetaOapg.properties.session_id: ...
@@ -235,26 +249,32 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["messages"]) -> MetaOapg.properties.messages: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["source"]) -> MetaOapg.properties.source: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
-    
-    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["metadata"]) -> MetaOapg.properties.metadata: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["feedback"]) -> MetaOapg.properties.feedback: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["error"]) -> MetaOapg.properties.error: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["duration"]) -> MetaOapg.properties.duration: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["model_config"]) -> MetaOapg.properties.model_config: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["user"]) -> MetaOapg.properties.user: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["provider_response"]) -> MetaOapg.properties.provider_response: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["provider_latency"]) -> MetaOapg.properties.provider_latency: ...
@@ -264,26 +284,29 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["finish_reason"]) -> MetaOapg.properties.finish_reason: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["project", "output", "id", "project_id", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "model_config", "metadata", "feedback", "created_at", "user", "provider_response", "provider_latency", "raw_output", "finish_reason", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["project", "output", "config", "id", "project_id", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "metadata", "feedback", "created_at", "error", "duration", "model_config", "user", "provider_response", "provider_latency", "raw_output", "finish_reason", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["output"]) -> MetaOapg.properties.output: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["config"]) -> 'ConfigResponse': ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["project_id"]) -> MetaOapg.properties.project_id: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["session_id"]) -> typing.Union[MetaOapg.properties.session_id, schemas.Unset]: ...
@@ -300,26 +323,32 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["messages"]) -> typing.Union[MetaOapg.properties.messages, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["source"]) -> typing.Union[MetaOapg.properties.source, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["model_config"]) -> typing.Union[MetaOapg.properties.model_config, schemas.Unset]: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["metadata"]) -> typing.Union[MetaOapg.properties.metadata, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["feedback"]) -> typing.Union[MetaOapg.properties.feedback, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["created_at"]) -> typing.Union[MetaOapg.properties.created_at, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["error"]) -> typing.Union[MetaOapg.properties.error, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["duration"]) -> typing.Union[MetaOapg.properties.duration, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["model_config"]) -> typing.Union[MetaOapg.properties.model_config, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["user"]) -> typing.Union[MetaOapg.properties.user, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["provider_response"]) -> typing.Union[MetaOapg.properties.provider_response, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["provider_latency"]) -> typing.Union[MetaOapg.properties.provider_latency, schemas.Unset]: ...
@@ -329,35 +358,38 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["finish_reason"]) -> typing.Union[MetaOapg.properties.finish_reason, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["project", "output", "id", "project_id", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "model_config", "metadata", "feedback", "created_at", "user", "provider_response", "provider_latency", "raw_output", "finish_reason", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["project", "output", "config", "id", "project_id", "session_id", "parent_id", "trial_id", "inputs", "messages", "source", "metadata", "feedback", "created_at", "error", "duration", "model_config", "user", "provider_response", "provider_latency", "raw_output", "finish_reason", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         output: typing.Union[MetaOapg.properties.output, str, ],
         project_id: typing.Union[MetaOapg.properties.project_id, str, ],
         project: typing.Union[MetaOapg.properties.project, str, ],
         id: typing.Union[MetaOapg.properties.id, str, ],
+        config: 'ConfigResponse',
         session_id: typing.Union[MetaOapg.properties.session_id, str, schemas.Unset] = schemas.unset,
         parent_id: typing.Union[MetaOapg.properties.parent_id, str, schemas.Unset] = schemas.unset,
         trial_id: typing.Union[MetaOapg.properties.trial_id, str, schemas.Unset] = schemas.unset,
         inputs: typing.Union[MetaOapg.properties.inputs, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         messages: typing.Union[MetaOapg.properties.messages, list, tuple, schemas.Unset] = schemas.unset,
         source: typing.Union[MetaOapg.properties.source, str, schemas.Unset] = schemas.unset,
-        model_config: typing.Union[MetaOapg.properties.model_config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         metadata: typing.Union[MetaOapg.properties.metadata, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         feedback: typing.Union[MetaOapg.properties.feedback, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, schemas.Unset] = schemas.unset,
+        error: typing.Union[MetaOapg.properties.error, str, schemas.Unset] = schemas.unset,
+        duration: typing.Union[MetaOapg.properties.duration, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
+        model_config: typing.Union[MetaOapg.properties.model_config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         user: typing.Union[MetaOapg.properties.user, str, schemas.Unset] = schemas.unset,
         provider_response: typing.Union[MetaOapg.properties.provider_response, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         provider_latency: typing.Union[MetaOapg.properties.provider_latency, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         raw_output: typing.Union[MetaOapg.properties.raw_output, str, schemas.Unset] = schemas.unset,
         finish_reason: typing.Union[MetaOapg.properties.finish_reason, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
@@ -365,29 +397,33 @@
         return super().__new__(
             cls,
             *args,
             output=output,
             project_id=project_id,
             project=project,
             id=id,
+            config=config,
             session_id=session_id,
             parent_id=parent_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             source=source,
-            model_config=model_config,
             metadata=metadata,
             feedback=feedback,
             created_at=created_at,
+            error=error,
+            duration=duration,
+            model_config=model_config,
             user=user,
             provider_response=provider_response,
             provider_latency=provider_latency,
             raw_output=raw_output,
             finish_reason=finish_reason,
             _configuration=_configuration,
             **kwargs,
         )
 
 from humanloop.model.chat_message import ChatMessage
+from humanloop.model.config_response import ConfigResponse
 from humanloop.model.feedback import Feedback
-from humanloop.model.src_external_app_models_v4_model_configs_project_model_config_response import SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse
+from humanloop.model.project_config_response import ProjectConfigResponse
```

### Comparing `humanloop-0.4.2/humanloop/model/logs_log_response.py` & `humanloop-0.4.3/humanloop/model/logs_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/logs_log_response.pyi` & `humanloop-0.4.3/humanloop/model/logs_log_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/model_config_chat_request.py` & `humanloop-0.4.3/humanloop/model/model_config_chat_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/model_config_chat_request.pyi` & `humanloop-0.4.3/humanloop/model/model_config_chat_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/model_config_completion_request.py` & `humanloop-0.4.3/humanloop/model/model_config_completion_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/model_config_completion_request.pyi` & `humanloop-0.4.3/humanloop/model/model_config_completion_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/model_endpoints.py` & `humanloop-0.4.3/humanloop/model/model_endpoints.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/model_endpoints.pyi` & `humanloop-0.4.3/humanloop/model/model_endpoints.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/model_providers.py` & `humanloop-0.4.3/humanloop/model/model_providers.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/model_providers.pyi` & `humanloop-0.4.3/humanloop/model/model_providers.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/paginated_data_log_response.py` & `humanloop-0.4.3/humanloop/model/paginated_data_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/paginated_data_log_response.pyi` & `humanloop-0.4.3/humanloop/model/paginated_data_log_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/paginated_data_project_response.py` & `humanloop-0.4.3/humanloop/model/paginated_data_project_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/paginated_data_project_response.pyi` & `humanloop-0.4.3/humanloop/model/paginated_data_project_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/positive_label.py` & `humanloop-0.4.3/humanloop/model/positive_label.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/positive_label.pyi` & `humanloop-0.4.3/humanloop/model/positive_label.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/project_model_config_request.py` & `humanloop-0.4.3/humanloop/model/project_model_config_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/project_model_config_request.pyi` & `humanloop-0.4.3/humanloop/model/project_model_config_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/project_response.py` & `humanloop-0.4.3/humanloop/model/project_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -116,15 +116,15 @@
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             
             
-            class active_model_config(
+            class active_config(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
                     
                     @classmethod
@@ -134,42 +134,47 @@
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse,
+                            ProjectConfigResponse,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'active_model_config':
+                ) -> 'active_config':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
+        
+            @staticmethod
+            def config_type() -> typing.Type['ConfigType']:
+                return ConfigType
             __annotations__ = {
                 "id": id,
                 "internal_id": internal_id,
                 "name": name,
                 "users": users,
                 "data_count": data_count,
                 "feedback_types": feedback_types,
                 "team_id": team_id,
                 "created_at": created_at,
                 "updated_at": updated_at,
                 "active_experiment": active_experiment,
-                "active_model_config": active_model_config,
+                "active_config": active_config,
+                "config_type": config_type,
             }
     
     feedback_types: 'FeedbackTypes'
     internal_id: MetaOapg.properties.internal_id
     updated_at: MetaOapg.properties.updated_at
     name: MetaOapg.properties.name
     created_at: MetaOapg.properties.created_at
@@ -205,20 +210,23 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["active_experiment"]) -> MetaOapg.properties.active_experiment: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["active_model_config"]) -> MetaOapg.properties.active_model_config: ...
+    def __getitem__(self, name: typing_extensions.Literal["active_config"]) -> MetaOapg.properties.active_config: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["config_type"]) -> 'ConfigType': ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "internal_id", "name", "users", "data_count", "feedback_types", "team_id", "created_at", "updated_at", "active_experiment", "active_model_config", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "internal_id", "name", "users", "data_count", "feedback_types", "team_id", "created_at", "updated_at", "active_experiment", "active_config", "config_type", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
@@ -246,20 +254,23 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["active_experiment"]) -> typing.Union[MetaOapg.properties.active_experiment, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["active_model_config"]) -> typing.Union[MetaOapg.properties.active_model_config, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["active_config"]) -> typing.Union[MetaOapg.properties.active_config, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["config_type"]) -> typing.Union['ConfigType', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "internal_id", "name", "users", "data_count", "feedback_types", "team_id", "created_at", "updated_at", "active_experiment", "active_model_config", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "internal_id", "name", "users", "data_count", "feedback_types", "team_id", "created_at", "updated_at", "active_experiment", "active_config", "config_type", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         feedback_types: 'FeedbackTypes',
@@ -268,15 +279,16 @@
         name: typing.Union[MetaOapg.properties.name, str, ],
         created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, ],
         id: typing.Union[MetaOapg.properties.id, str, ],
         team_id: typing.Union[MetaOapg.properties.team_id, str, ],
         data_count: typing.Union[MetaOapg.properties.data_count, decimal.Decimal, int, ],
         users: typing.Union[MetaOapg.properties.users, list, tuple, ],
         active_experiment: typing.Union[MetaOapg.properties.active_experiment, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-        active_model_config: typing.Union[MetaOapg.properties.active_model_config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        active_config: typing.Union[MetaOapg.properties.active_config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        config_type: typing.Union['ConfigType', schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'ProjectResponse':
         return super().__new__(
             cls,
             *args,
             feedback_types=feedback_types,
@@ -285,16 +297,18 @@
             name=name,
             created_at=created_at,
             id=id,
             team_id=team_id,
             data_count=data_count,
             users=users,
             active_experiment=active_experiment,
-            active_model_config=active_model_config,
+            active_config=active_config,
+            config_type=config_type,
             _configuration=_configuration,
             **kwargs,
         )
 
+from humanloop.model.config_type import ConfigType
 from humanloop.model.experiment_response import ExperimentResponse
 from humanloop.model.feedback_types import FeedbackTypes
+from humanloop.model.project_config_response import ProjectConfigResponse
 from humanloop.model.project_user_response import ProjectUserResponse
-from humanloop.model.src_external_app_models_v4_model_configs_project_model_config_response import SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse
```

### Comparing `humanloop-0.4.2/humanloop/model/project_response.pyi` & `humanloop-0.4.3/humanloop/model/project_response.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -116,15 +116,15 @@
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             
             
-            class active_model_config(
+            class active_config(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
                     
                     @classmethod
@@ -134,42 +134,47 @@
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse,
+                            ProjectConfigResponse,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'active_model_config':
+                ) -> 'active_config':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
+        
+            @staticmethod
+            def config_type() -> typing.Type['ConfigType']:
+                return ConfigType
             __annotations__ = {
                 "id": id,
                 "internal_id": internal_id,
                 "name": name,
                 "users": users,
                 "data_count": data_count,
                 "feedback_types": feedback_types,
                 "team_id": team_id,
                 "created_at": created_at,
                 "updated_at": updated_at,
                 "active_experiment": active_experiment,
-                "active_model_config": active_model_config,
+                "active_config": active_config,
+                "config_type": config_type,
             }
     
     feedback_types: 'FeedbackTypes'
     internal_id: MetaOapg.properties.internal_id
     updated_at: MetaOapg.properties.updated_at
     name: MetaOapg.properties.name
     created_at: MetaOapg.properties.created_at
@@ -205,20 +210,23 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["active_experiment"]) -> MetaOapg.properties.active_experiment: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["active_model_config"]) -> MetaOapg.properties.active_model_config: ...
+    def __getitem__(self, name: typing_extensions.Literal["active_config"]) -> MetaOapg.properties.active_config: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["config_type"]) -> 'ConfigType': ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "internal_id", "name", "users", "data_count", "feedback_types", "team_id", "created_at", "updated_at", "active_experiment", "active_model_config", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "internal_id", "name", "users", "data_count", "feedback_types", "team_id", "created_at", "updated_at", "active_experiment", "active_config", "config_type", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
@@ -246,20 +254,23 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["active_experiment"]) -> typing.Union[MetaOapg.properties.active_experiment, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["active_model_config"]) -> typing.Union[MetaOapg.properties.active_model_config, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["active_config"]) -> typing.Union[MetaOapg.properties.active_config, schemas.Unset]: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["config_type"]) -> typing.Union['ConfigType', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "internal_id", "name", "users", "data_count", "feedback_types", "team_id", "created_at", "updated_at", "active_experiment", "active_model_config", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "internal_id", "name", "users", "data_count", "feedback_types", "team_id", "created_at", "updated_at", "active_experiment", "active_config", "config_type", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         feedback_types: 'FeedbackTypes',
@@ -268,15 +279,16 @@
         name: typing.Union[MetaOapg.properties.name, str, ],
         created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, ],
         id: typing.Union[MetaOapg.properties.id, str, ],
         team_id: typing.Union[MetaOapg.properties.team_id, str, ],
         data_count: typing.Union[MetaOapg.properties.data_count, decimal.Decimal, int, ],
         users: typing.Union[MetaOapg.properties.users, list, tuple, ],
         active_experiment: typing.Union[MetaOapg.properties.active_experiment, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-        active_model_config: typing.Union[MetaOapg.properties.active_model_config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        active_config: typing.Union[MetaOapg.properties.active_config, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        config_type: typing.Union['ConfigType', schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'ProjectResponse':
         return super().__new__(
             cls,
             *args,
             feedback_types=feedback_types,
@@ -285,16 +297,18 @@
             name=name,
             created_at=created_at,
             id=id,
             team_id=team_id,
             data_count=data_count,
             users=users,
             active_experiment=active_experiment,
-            active_model_config=active_model_config,
+            active_config=active_config,
+            config_type=config_type,
             _configuration=_configuration,
             **kwargs,
         )
 
+from humanloop.model.config_type import ConfigType
 from humanloop.model.experiment_response import ExperimentResponse
 from humanloop.model.feedback_types import FeedbackTypes
+from humanloop.model.project_config_response import ProjectConfigResponse
 from humanloop.model.project_user_response import ProjectUserResponse
-from humanloop.model.src_external_app_models_v4_model_configs_project_model_config_response import SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse
```

### Comparing `humanloop-0.4.2/humanloop/model/project_sort_by.py` & `humanloop-0.4.3/humanloop/model/project_sort_by.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/project_sort_by.pyi` & `humanloop-0.4.3/humanloop/model/project_sort_by.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/project_user_response.py` & `humanloop-0.4.3/humanloop/model/project_user_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/project_user_response.pyi` & `humanloop-0.4.3/humanloop/model/project_user_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/projects_get_model_configs_response.py` & `humanloop-0.4.3/humanloop/model/projects_update_feedback_types_request.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,36 +19,36 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class ProjectsGetModelConfigsResponse(
+class ProjectsUpdateFeedbackTypesRequest(
     schemas.ListSchema
 ):
     """NOTE:
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         @staticmethod
-        def items() -> typing.Type['SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse']:
-            return SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse
+        def items() -> typing.Type['FeedbackTypeRequest']:
+            return FeedbackTypeRequest
 
     def __new__(
         cls,
-        arg: typing.Union[typing.Tuple['SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse'], typing.List['SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse']],
+        arg: typing.Union[typing.Tuple['FeedbackTypeRequest'], typing.List['FeedbackTypeRequest']],
         _configuration: typing.Optional[schemas.Configuration] = None,
-    ) -> 'ProjectsGetModelConfigsResponse':
+    ) -> 'ProjectsUpdateFeedbackTypesRequest':
         return super().__new__(
             cls,
             arg,
             _configuration=_configuration,
         )
 
-    def __getitem__(self, i: int) -> 'SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse':
+    def __getitem__(self, i: int) -> 'FeedbackTypeRequest':
         return super().__getitem__(i)
 
-from humanloop.model.src_external_app_models_v4_model_configs_project_model_config_response import SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse
+from humanloop.model.feedback_type_request import FeedbackTypeRequest
```

### Comparing `humanloop-0.4.2/humanloop/model/projects_get_model_configs_response.pyi` & `humanloop-0.4.3/humanloop/model/projects_update_feedback_types_request.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -19,36 +19,36 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class ProjectsGetModelConfigsResponse(
+class ProjectsUpdateFeedbackTypesRequest(
     schemas.ListSchema
 ):
     """NOTE:
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         @staticmethod
-        def items() -> typing.Type['SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse']:
-            return SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse
+        def items() -> typing.Type['FeedbackTypeRequest']:
+            return FeedbackTypeRequest
 
     def __new__(
         cls,
-        arg: typing.Union[typing.Tuple['SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse'], typing.List['SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse']],
+        arg: typing.Union[typing.Tuple['FeedbackTypeRequest'], typing.List['FeedbackTypeRequest']],
         _configuration: typing.Optional[schemas.Configuration] = None,
-    ) -> 'ProjectsGetModelConfigsResponse':
+    ) -> 'ProjectsUpdateFeedbackTypesRequest':
         return super().__new__(
             cls,
             arg,
             _configuration=_configuration,
         )
 
-    def __getitem__(self, i: int) -> 'SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse':
+    def __getitem__(self, i: int) -> 'FeedbackTypeRequest':
         return super().__getitem__(i)
 
-from humanloop.model.src_external_app_models_v4_model_configs_project_model_config_response import SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse
+from humanloop.model.feedback_type_request import FeedbackTypeRequest
```

### Comparing `humanloop-0.4.2/humanloop/model/projects_update_feedback_types_request.py` & `humanloop-0.4.3/humanloop/model/sort_order.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -19,36 +19,24 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class ProjectsUpdateFeedbackTypesRequest(
-    schemas.ListSchema
+class SortOrder(
+    schemas.EnumBase,
+    schemas.StrSchema
 ):
-    """NOTE:
-    This class is auto generated by Konfig (https://konfigthis.com)
     """
+    This class is auto generated by Konfig (https://konfigthis.com)
 
-
-    class MetaOapg:
-        
-        @staticmethod
-        def items() -> typing.Type['FeedbackTypeRequest']:
-            return FeedbackTypeRequest
-
-    def __new__(
-        cls,
-        arg: typing.Union[typing.Tuple['FeedbackTypeRequest'], typing.List['FeedbackTypeRequest']],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-    ) -> 'ProjectsUpdateFeedbackTypesRequest':
-        return super().__new__(
-            cls,
-            arg,
-            _configuration=_configuration,
-        )
-
-    def __getitem__(self, i: int) -> 'FeedbackTypeRequest':
-        return super().__getitem__(i)
-
-from humanloop.model.feedback_type_request import FeedbackTypeRequest
+    An enumeration.
+    """
+    
+    @schemas.classproperty
+    def ASC(cls):
+        return cls("asc")
+    
+    @schemas.classproperty
+    def DESC(cls):
+        return cls("desc")
```

### Comparing `humanloop-0.4.2/humanloop/model/projects_update_feedback_types_request.pyi` & `humanloop-0.4.3/humanloop/model/projects_get_configs_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,36 +19,36 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class ProjectsUpdateFeedbackTypesRequest(
+class ProjectsGetConfigsResponse(
     schemas.ListSchema
 ):
     """NOTE:
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         
         @staticmethod
-        def items() -> typing.Type['FeedbackTypeRequest']:
-            return FeedbackTypeRequest
+        def items() -> typing.Type['ProjectConfigResponse']:
+            return ProjectConfigResponse
 
     def __new__(
         cls,
-        arg: typing.Union[typing.Tuple['FeedbackTypeRequest'], typing.List['FeedbackTypeRequest']],
+        arg: typing.Union[typing.Tuple['ProjectConfigResponse'], typing.List['ProjectConfigResponse']],
         _configuration: typing.Optional[schemas.Configuration] = None,
-    ) -> 'ProjectsUpdateFeedbackTypesRequest':
+    ) -> 'ProjectsGetConfigsResponse':
         return super().__new__(
             cls,
             arg,
             _configuration=_configuration,
         )
 
-    def __getitem__(self, i: int) -> 'FeedbackTypeRequest':
+    def __getitem__(self, i: int) -> 'ProjectConfigResponse':
         return super().__getitem__(i)
 
-from humanloop.model.feedback_type_request import FeedbackTypeRequest
+from humanloop.model.project_config_response import ProjectConfigResponse
```

### Comparing `humanloop-0.4.2/humanloop/model/provider_api_keys.py` & `humanloop-0.4.3/humanloop/model/provider_api_keys.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/provider_api_keys.pyi` & `humanloop-0.4.3/humanloop/model/provider_api_keys.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/session_app_response.py` & `humanloop-0.4.3/humanloop/model/create_trace_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,85 +19,73 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class SessionAppResponse(
+class CreateTraceResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
-            "name",
-            "id",
+            "session_id",
         }
         
         class properties:
-            id = schemas.StrSchema
-            name = schemas.StrSchema
-            description = schemas.StrSchema
+            session_id = schemas.StrSchema
+            function_id = schemas.StrSchema
             __annotations__ = {
-                "id": id,
-                "name": name,
-                "description": description,
+                "session_id": session_id,
+                "function_id": function_id,
             }
     
-    name: MetaOapg.properties.name
-    id: MetaOapg.properties.id
+    session_id: MetaOapg.properties.session_id
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    def __getitem__(self, name: typing_extensions.Literal["session_id"]) -> MetaOapg.properties.session_id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
+    def __getitem__(self, name: typing_extensions.Literal["function_id"]) -> MetaOapg.properties.function_id: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "name", "description", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["session_id", "function_id", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["session_id"]) -> MetaOapg.properties.session_id: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["function_id"]) -> typing.Union[MetaOapg.properties.function_id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "name", "description", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["session_id", "function_id", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        name: typing.Union[MetaOapg.properties.name, str, ],
-        id: typing.Union[MetaOapg.properties.id, str, ],
-        description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
+        session_id: typing.Union[MetaOapg.properties.session_id, str, ],
+        function_id: typing.Union[MetaOapg.properties.function_id, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SessionAppResponse':
+    ) -> 'CreateTraceResponse':
         return super().__new__(
             cls,
             *args,
-            name=name,
-            id=id,
-            description=description,
+            session_id=session_id,
+            function_id=function_id,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `humanloop-0.4.2/humanloop/model/session_app_response.pyi` & `humanloop-0.4.3/humanloop/model/create_trace_response.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -19,85 +19,73 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class SessionAppResponse(
+class CreateTraceResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
-            "name",
-            "id",
+            "session_id",
         }
         
         class properties:
-            id = schemas.StrSchema
-            name = schemas.StrSchema
-            description = schemas.StrSchema
+            session_id = schemas.StrSchema
+            function_id = schemas.StrSchema
             __annotations__ = {
-                "id": id,
-                "name": name,
-                "description": description,
+                "session_id": session_id,
+                "function_id": function_id,
             }
     
-    name: MetaOapg.properties.name
-    id: MetaOapg.properties.id
+    session_id: MetaOapg.properties.session_id
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    def __getitem__(self, name: typing_extensions.Literal["session_id"]) -> MetaOapg.properties.session_id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
+    def __getitem__(self, name: typing_extensions.Literal["function_id"]) -> MetaOapg.properties.function_id: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "name", "description", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["session_id", "function_id", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["session_id"]) -> MetaOapg.properties.session_id: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["function_id"]) -> typing.Union[MetaOapg.properties.function_id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "name", "description", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["session_id", "function_id", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        name: typing.Union[MetaOapg.properties.name, str, ],
-        id: typing.Union[MetaOapg.properties.id, str, ],
-        description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
+        session_id: typing.Union[MetaOapg.properties.session_id, str, ],
+        function_id: typing.Union[MetaOapg.properties.function_id, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SessionAppResponse':
+    ) -> 'CreateTraceResponse':
         return super().__new__(
             cls,
             *args,
-            name=name,
-            id=id,
-            description=description,
+            session_id=session_id,
+            function_id=function_id,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `humanloop-0.4.2/humanloop/model/session_response.py` & `humanloop-0.4.3/humanloop/model/paginated_data_session_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,104 +19,126 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class SessionResponse(
+class PaginatedDataSessionResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
-            "app",
-            "updated_at",
-            "created_at",
-            "id",
+            "total",
+            "size",
+            "records",
+            "page",
         }
         
         class properties:
-            id = schemas.StrSchema
-        
-            @staticmethod
-            def app() -> typing.Type['SessionAppResponse']:
-                return SessionAppResponse
-            created_at = schemas.DateTimeSchema
-            updated_at = schemas.DateTimeSchema
+            
+            
+            class records(
+                schemas.ListSchema
+            ):
+            
+            
+                class MetaOapg:
+                    
+                    @staticmethod
+                    def items() -> typing.Type['SessionResponse']:
+                        return SessionResponse
+            
+                def __new__(
+                    cls,
+                    arg: typing.Union[typing.Tuple['SessionResponse'], typing.List['SessionResponse']],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                ) -> 'records':
+                    return super().__new__(
+                        cls,
+                        arg,
+                        _configuration=_configuration,
+                    )
+            
+                def __getitem__(self, i: int) -> 'SessionResponse':
+                    return super().__getitem__(i)
+            page = schemas.IntSchema
+            size = schemas.IntSchema
+            total = schemas.IntSchema
             __annotations__ = {
-                "id": id,
-                "app": app,
-                "created_at": created_at,
-                "updated_at": updated_at,
+                "records": records,
+                "page": page,
+                "size": size,
+                "total": total,
             }
     
-    app: 'SessionAppResponse'
-    updated_at: MetaOapg.properties.updated_at
-    created_at: MetaOapg.properties.created_at
-    id: MetaOapg.properties.id
+    total: MetaOapg.properties.total
+    size: MetaOapg.properties.size
+    records: MetaOapg.properties.records
+    page: MetaOapg.properties.page
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    def __getitem__(self, name: typing_extensions.Literal["records"]) -> MetaOapg.properties.records: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["app"]) -> 'SessionAppResponse': ...
+    def __getitem__(self, name: typing_extensions.Literal["page"]) -> MetaOapg.properties.page: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
+    def __getitem__(self, name: typing_extensions.Literal["size"]) -> MetaOapg.properties.size: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
+    def __getitem__(self, name: typing_extensions.Literal["total"]) -> MetaOapg.properties.total: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "app", "created_at", "updated_at", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["records", "page", "size", "total", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["records"]) -> MetaOapg.properties.records: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["app"]) -> 'SessionAppResponse': ...
+    def get_item_oapg(self, name: typing_extensions.Literal["page"]) -> MetaOapg.properties.page: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["size"]) -> MetaOapg.properties.size: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["total"]) -> MetaOapg.properties.total: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "app", "created_at", "updated_at", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["records", "page", "size", "total", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        app: 'SessionAppResponse',
-        updated_at: typing.Union[MetaOapg.properties.updated_at, str, datetime, ],
-        created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, ],
-        id: typing.Union[MetaOapg.properties.id, str, ],
+        total: typing.Union[MetaOapg.properties.total, decimal.Decimal, int, ],
+        size: typing.Union[MetaOapg.properties.size, decimal.Decimal, int, ],
+        records: typing.Union[MetaOapg.properties.records, list, tuple, ],
+        page: typing.Union[MetaOapg.properties.page, decimal.Decimal, int, ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SessionResponse':
+    ) -> 'PaginatedDataSessionResponse':
         return super().__new__(
             cls,
             *args,
-            app=app,
-            updated_at=updated_at,
-            created_at=created_at,
-            id=id,
+            total=total,
+            size=size,
+            records=records,
+            page=page,
             _configuration=_configuration,
             **kwargs,
         )
 
-from humanloop.model.session_app_response import SessionAppResponse
+from humanloop.model.session_response import SessionResponse
```

### Comparing `humanloop-0.4.2/humanloop/model/session_response.pyi` & `humanloop-0.4.3/humanloop/model/paginated_data_session_response.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -19,104 +19,126 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class SessionResponse(
+class PaginatedDataSessionResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
     class MetaOapg:
         required = {
-            "app",
-            "updated_at",
-            "created_at",
-            "id",
+            "total",
+            "size",
+            "records",
+            "page",
         }
         
         class properties:
-            id = schemas.StrSchema
-        
-            @staticmethod
-            def app() -> typing.Type['SessionAppResponse']:
-                return SessionAppResponse
-            created_at = schemas.DateTimeSchema
-            updated_at = schemas.DateTimeSchema
+            
+            
+            class records(
+                schemas.ListSchema
+            ):
+            
+            
+                class MetaOapg:
+                    
+                    @staticmethod
+                    def items() -> typing.Type['SessionResponse']:
+                        return SessionResponse
+            
+                def __new__(
+                    cls,
+                    arg: typing.Union[typing.Tuple['SessionResponse'], typing.List['SessionResponse']],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                ) -> 'records':
+                    return super().__new__(
+                        cls,
+                        arg,
+                        _configuration=_configuration,
+                    )
+            
+                def __getitem__(self, i: int) -> 'SessionResponse':
+                    return super().__getitem__(i)
+            page = schemas.IntSchema
+            size = schemas.IntSchema
+            total = schemas.IntSchema
             __annotations__ = {
-                "id": id,
-                "app": app,
-                "created_at": created_at,
-                "updated_at": updated_at,
+                "records": records,
+                "page": page,
+                "size": size,
+                "total": total,
             }
     
-    app: 'SessionAppResponse'
-    updated_at: MetaOapg.properties.updated_at
-    created_at: MetaOapg.properties.created_at
-    id: MetaOapg.properties.id
+    total: MetaOapg.properties.total
+    size: MetaOapg.properties.size
+    records: MetaOapg.properties.records
+    page: MetaOapg.properties.page
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    def __getitem__(self, name: typing_extensions.Literal["records"]) -> MetaOapg.properties.records: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["app"]) -> 'SessionAppResponse': ...
+    def __getitem__(self, name: typing_extensions.Literal["page"]) -> MetaOapg.properties.page: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
+    def __getitem__(self, name: typing_extensions.Literal["size"]) -> MetaOapg.properties.size: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
+    def __getitem__(self, name: typing_extensions.Literal["total"]) -> MetaOapg.properties.total: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "app", "created_at", "updated_at", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["records", "page", "size", "total", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["records"]) -> MetaOapg.properties.records: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["app"]) -> 'SessionAppResponse': ...
+    def get_item_oapg(self, name: typing_extensions.Literal["page"]) -> MetaOapg.properties.page: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["size"]) -> MetaOapg.properties.size: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["total"]) -> MetaOapg.properties.total: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "app", "created_at", "updated_at", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["records", "page", "size", "total", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        app: 'SessionAppResponse',
-        updated_at: typing.Union[MetaOapg.properties.updated_at, str, datetime, ],
-        created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, ],
-        id: typing.Union[MetaOapg.properties.id, str, ],
+        total: typing.Union[MetaOapg.properties.total, decimal.Decimal, int, ],
+        size: typing.Union[MetaOapg.properties.size, decimal.Decimal, int, ],
+        records: typing.Union[MetaOapg.properties.records, list, tuple, ],
+        page: typing.Union[MetaOapg.properties.page, decimal.Decimal, int, ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SessionResponse':
+    ) -> 'PaginatedDataSessionResponse':
         return super().__new__(
             cls,
             *args,
-            app=app,
-            updated_at=updated_at,
-            created_at=created_at,
-            id=id,
+            total=total,
+            size=size,
+            records=records,
+            page=page,
             _configuration=_configuration,
             **kwargs,
         )
 
-from humanloop.model.session_app_response import SessionAppResponse
+from humanloop.model.session_response import SessionResponse
```

### Comparing `humanloop-0.4.2/humanloop/model/sort_order.py` & `humanloop-0.4.3/humanloop/model/sort_order.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/sort_order.pyi` & `humanloop-0.4.3/humanloop/model/config_type.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -19,24 +19,32 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class SortOrder(
+class ConfigType(
     schemas.EnumBase,
     schemas.StrSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
 
     An enumeration.
     """
     
     @schemas.classproperty
-    def ASC(cls):
-        return cls("asc")
+    def GENERIC(cls):
+        return cls("generic")
     
     @schemas.classproperty
-    def DESC(cls):
-        return cls("desc")
+    def MODEL(cls):
+        return cls("model")
+    
+    @schemas.classproperty
+    def TOOL(cls):
+        return cls("tool")
+    
+    @schemas.classproperty
+    def AGENT(cls):
+        return cls("agent")
```

### Comparing `humanloop-0.4.2/humanloop/model/src_external_app_models_v3_model_configs_model_config_response.py` & `humanloop-0.4.3/humanloop/model/model_config_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class SrcExternalAppModelsV3ModelConfigsModelConfigResponse(
+class ModelConfigResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
 
     Extends the core ModelConfig request object to include Humanloop generated
 identifier and method for serializing response from ModelConfig domain object.
@@ -344,15 +344,15 @@
         stop: typing.Union[MetaOapg.properties.stop, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         presence_penalty: typing.Union[MetaOapg.properties.presence_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         frequency_penalty: typing.Union[MetaOapg.properties.frequency_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         display_name: typing.Union[MetaOapg.properties.display_name, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SrcExternalAppModelsV3ModelConfigsModelConfigResponse':
+    ) -> 'ModelConfigResponse':
         return super().__new__(
             cls,
             *args,
             model=model,
             id=id,
             provider=provider,
             endpoint=endpoint,
```

### Comparing `humanloop-0.4.2/humanloop/model/src_external_app_models_v3_model_configs_model_config_response.pyi` & `humanloop-0.4.3/humanloop/model/model_config_response.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class SrcExternalAppModelsV3ModelConfigsModelConfigResponse(
+class ModelConfigResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
 
     Extends the core ModelConfig request object to include Humanloop generated
 identifier and method for serializing response from ModelConfig domain object.
@@ -344,15 +344,15 @@
         stop: typing.Union[MetaOapg.properties.stop, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         presence_penalty: typing.Union[MetaOapg.properties.presence_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         frequency_penalty: typing.Union[MetaOapg.properties.frequency_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         display_name: typing.Union[MetaOapg.properties.display_name, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SrcExternalAppModelsV3ModelConfigsModelConfigResponse':
+    ) -> 'ModelConfigResponse':
         return super().__new__(
             cls,
             *args,
             model=model,
             id=id,
             provider=provider,
             endpoint=endpoint,
```

### Comparing `humanloop-0.4.2/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py` & `humanloop-0.4.3/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.pyi` & `humanloop-0.4.3/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_response.py` & `humanloop-0.4.3/humanloop/model/model_config_response2.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,43 +19,37 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class SrcExternalAppModelsV3ModelConfigsProjectModelConfigResponse(
+class ModelConfigResponse2(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
 
-    Extends the core ModelConfig request object to include Humanloop generated
-identifier and method for serializing response from ModelConfig domain object.
+    Model config request
     """
 
 
     class MetaOapg:
         required = {
-            "updated_at",
-            "last_used",
-            "created_at",
+            "name",
             "model",
             "id",
+            "type",
         }
         
         class properties:
-            model = schemas.StrSchema
             id = schemas.StrSchema
-            created_at = schemas.DateTimeSchema
-            updated_at = schemas.DateTimeSchema
-            last_used = schemas.DateTimeSchema
             
             
-            class provider(
+            class type(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
                     
                     @classmethod
@@ -65,33 +59,37 @@
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            ModelProviders,
+                            ConfigType,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'provider':
+                ) -> 'type':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
+            name = schemas.StrSchema
+            model = schemas.StrSchema
+            description = schemas.StrSchema
+            other = schemas.DictSchema
             
             
-            class endpoint(
+            class provider(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
                     
                     @classmethod
@@ -101,59 +99,32 @@
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            ModelEndpoints,
+                            ModelProviders,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'endpoint':
+                ) -> 'provider':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            prompt_template = schemas.StrSchema
-            
-            
-            class chat_template(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['ChatMessage']:
-                        return ChatMessage
-            
-                def __new__(
-                    cls,
-                    arg: typing.Union[typing.Tuple['ChatMessage'], typing.List['ChatMessage']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'chat_template':
-                    return super().__new__(
-                        cls,
-                        arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'ChatMessage':
-                    return super().__getitem__(i)
-            temperature = schemas.NumberSchema
             max_tokens = schemas.IntSchema
+            temperature = schemas.NumberSchema
             top_p = schemas.NumberSchema
             
             
             class stop(
                 schemas.ComposedSchema,
             ):
             
@@ -210,278 +181,254 @@
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             presence_penalty = schemas.NumberSchema
             frequency_penalty = schemas.NumberSchema
-            other = schemas.DictSchema
-            display_name = schemas.StrSchema
-            project_id = schemas.StrSchema
-            project_name = schemas.StrSchema
+            prompt_template = schemas.StrSchema
             
             
-            class feedback_stats(
+            class chat_template(
                 schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
                     @staticmethod
-                    def items() -> typing.Type['SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse']:
-                        return SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse
+                    def items() -> typing.Type['ChatMessage']:
+                        return ChatMessage
             
                 def __new__(
                     cls,
-                    arg: typing.Union[typing.Tuple['SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse'], typing.List['SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse']],
+                    arg: typing.Union[typing.Tuple['ChatMessage'], typing.List['ChatMessage']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'feedback_stats':
+                ) -> 'chat_template':
                     return super().__new__(
                         cls,
                         arg,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> 'SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse':
+                def __getitem__(self, i: int) -> 'ChatMessage':
                     return super().__getitem__(i)
-            num_datapoints = schemas.IntSchema
-            experiment_id = schemas.StrSchema
+            
+            
+            class endpoint(
+                schemas.ComposedSchema,
+            ):
+            
+            
+                class MetaOapg:
+                    
+                    @classmethod
+                    @functools.lru_cache()
+                    def all_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            ModelEndpoints,
+                        ]
+            
+            
+                def __new__(
+                    cls,
+                    *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+                ) -> 'endpoint':
+                    return super().__new__(
+                        cls,
+                        *args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
             __annotations__ = {
-                "model": model,
                 "id": id,
-                "created_at": created_at,
-                "updated_at": updated_at,
-                "last_used": last_used,
+                "type": type,
+                "name": name,
+                "model": model,
+                "description": description,
+                "other": other,
                 "provider": provider,
-                "endpoint": endpoint,
-                "prompt_template": prompt_template,
-                "chat_template": chat_template,
-                "temperature": temperature,
                 "max_tokens": max_tokens,
+                "temperature": temperature,
                 "top_p": top_p,
                 "stop": stop,
                 "presence_penalty": presence_penalty,
                 "frequency_penalty": frequency_penalty,
-                "other": other,
-                "display_name": display_name,
-                "project_id": project_id,
-                "project_name": project_name,
-                "feedback_stats": feedback_stats,
-                "num_datapoints": num_datapoints,
-                "experiment_id": experiment_id,
+                "prompt_template": prompt_template,
+                "chat_template": chat_template,
+                "endpoint": endpoint,
             }
     
-    updated_at: MetaOapg.properties.updated_at
-    last_used: MetaOapg.properties.last_used
-    created_at: MetaOapg.properties.created_at
+    name: MetaOapg.properties.name
     model: MetaOapg.properties.model
     id: MetaOapg.properties.id
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
+    type: MetaOapg.properties.type
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
+    def __getitem__(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
+    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["last_used"]) -> MetaOapg.properties.last_used: ...
+    def __getitem__(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["provider"]) -> MetaOapg.properties.provider: ...
+    def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["endpoint"]) -> MetaOapg.properties.endpoint: ...
+    def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["prompt_template"]) -> MetaOapg.properties.prompt_template: ...
+    def __getitem__(self, name: typing_extensions.Literal["provider"]) -> MetaOapg.properties.provider: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["chat_template"]) -> MetaOapg.properties.chat_template: ...
+    def __getitem__(self, name: typing_extensions.Literal["max_tokens"]) -> MetaOapg.properties.max_tokens: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["temperature"]) -> MetaOapg.properties.temperature: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["max_tokens"]) -> MetaOapg.properties.max_tokens: ...
-    
-    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["top_p"]) -> MetaOapg.properties.top_p: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["stop"]) -> MetaOapg.properties.stop: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["presence_penalty"]) -> MetaOapg.properties.presence_penalty: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["frequency_penalty"]) -> MetaOapg.properties.frequency_penalty: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["display_name"]) -> MetaOapg.properties.display_name: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["project_id"]) -> MetaOapg.properties.project_id: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["project_name"]) -> MetaOapg.properties.project_name: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["feedback_stats"]) -> MetaOapg.properties.feedback_stats: ...
+    def __getitem__(self, name: typing_extensions.Literal["prompt_template"]) -> MetaOapg.properties.prompt_template: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["num_datapoints"]) -> MetaOapg.properties.num_datapoints: ...
+    def __getitem__(self, name: typing_extensions.Literal["chat_template"]) -> MetaOapg.properties.chat_template: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["experiment_id"]) -> MetaOapg.properties.experiment_id: ...
+    def __getitem__(self, name: typing_extensions.Literal["endpoint"]) -> MetaOapg.properties.endpoint: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model", "id", "created_at", "updated_at", "last_used", "provider", "endpoint", "prompt_template", "chat_template", "temperature", "max_tokens", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "display_name", "project_id", "project_name", "feedback_stats", "num_datapoints", "experiment_id", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "model", "description", "other", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "prompt_template", "chat_template", "endpoint", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["last_used"]) -> MetaOapg.properties.last_used: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["provider"]) -> typing.Union[MetaOapg.properties.provider, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["endpoint"]) -> typing.Union[MetaOapg.properties.endpoint, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["prompt_template"]) -> typing.Union[MetaOapg.properties.prompt_template, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["provider"]) -> typing.Union[MetaOapg.properties.provider, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["chat_template"]) -> typing.Union[MetaOapg.properties.chat_template, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["max_tokens"]) -> typing.Union[MetaOapg.properties.max_tokens, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["temperature"]) -> typing.Union[MetaOapg.properties.temperature, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["max_tokens"]) -> typing.Union[MetaOapg.properties.max_tokens, schemas.Unset]: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["top_p"]) -> typing.Union[MetaOapg.properties.top_p, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["stop"]) -> typing.Union[MetaOapg.properties.stop, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["presence_penalty"]) -> typing.Union[MetaOapg.properties.presence_penalty, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["frequency_penalty"]) -> typing.Union[MetaOapg.properties.frequency_penalty, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["display_name"]) -> typing.Union[MetaOapg.properties.display_name, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["project_id"]) -> typing.Union[MetaOapg.properties.project_id, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["project_name"]) -> typing.Union[MetaOapg.properties.project_name, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["feedback_stats"]) -> typing.Union[MetaOapg.properties.feedback_stats, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["prompt_template"]) -> typing.Union[MetaOapg.properties.prompt_template, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["num_datapoints"]) -> typing.Union[MetaOapg.properties.num_datapoints, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["chat_template"]) -> typing.Union[MetaOapg.properties.chat_template, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["experiment_id"]) -> typing.Union[MetaOapg.properties.experiment_id, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["endpoint"]) -> typing.Union[MetaOapg.properties.endpoint, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model", "id", "created_at", "updated_at", "last_used", "provider", "endpoint", "prompt_template", "chat_template", "temperature", "max_tokens", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "display_name", "project_id", "project_name", "feedback_stats", "num_datapoints", "experiment_id", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "model", "description", "other", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "prompt_template", "chat_template", "endpoint", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        updated_at: typing.Union[MetaOapg.properties.updated_at, str, datetime, ],
-        last_used: typing.Union[MetaOapg.properties.last_used, str, datetime, ],
-        created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, ],
+        name: typing.Union[MetaOapg.properties.name, str, ],
         model: typing.Union[MetaOapg.properties.model, str, ],
         id: typing.Union[MetaOapg.properties.id, str, ],
+        type: typing.Union[MetaOapg.properties.type, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
+        other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         provider: typing.Union[MetaOapg.properties.provider, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-        endpoint: typing.Union[MetaOapg.properties.endpoint, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-        prompt_template: typing.Union[MetaOapg.properties.prompt_template, str, schemas.Unset] = schemas.unset,
-        chat_template: typing.Union[MetaOapg.properties.chat_template, list, tuple, schemas.Unset] = schemas.unset,
-        temperature: typing.Union[MetaOapg.properties.temperature, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         max_tokens: typing.Union[MetaOapg.properties.max_tokens, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        temperature: typing.Union[MetaOapg.properties.temperature, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         top_p: typing.Union[MetaOapg.properties.top_p, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         stop: typing.Union[MetaOapg.properties.stop, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         presence_penalty: typing.Union[MetaOapg.properties.presence_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         frequency_penalty: typing.Union[MetaOapg.properties.frequency_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
-        other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
-        display_name: typing.Union[MetaOapg.properties.display_name, str, schemas.Unset] = schemas.unset,
-        project_id: typing.Union[MetaOapg.properties.project_id, str, schemas.Unset] = schemas.unset,
-        project_name: typing.Union[MetaOapg.properties.project_name, str, schemas.Unset] = schemas.unset,
-        feedback_stats: typing.Union[MetaOapg.properties.feedback_stats, list, tuple, schemas.Unset] = schemas.unset,
-        num_datapoints: typing.Union[MetaOapg.properties.num_datapoints, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        experiment_id: typing.Union[MetaOapg.properties.experiment_id, str, schemas.Unset] = schemas.unset,
+        prompt_template: typing.Union[MetaOapg.properties.prompt_template, str, schemas.Unset] = schemas.unset,
+        chat_template: typing.Union[MetaOapg.properties.chat_template, list, tuple, schemas.Unset] = schemas.unset,
+        endpoint: typing.Union[MetaOapg.properties.endpoint, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SrcExternalAppModelsV3ModelConfigsProjectModelConfigResponse':
+    ) -> 'ModelConfigResponse2':
         return super().__new__(
             cls,
             *args,
-            updated_at=updated_at,
-            last_used=last_used,
-            created_at=created_at,
+            name=name,
             model=model,
             id=id,
+            type=type,
+            description=description,
+            other=other,
             provider=provider,
-            endpoint=endpoint,
-            prompt_template=prompt_template,
-            chat_template=chat_template,
-            temperature=temperature,
             max_tokens=max_tokens,
+            temperature=temperature,
             top_p=top_p,
             stop=stop,
             presence_penalty=presence_penalty,
             frequency_penalty=frequency_penalty,
-            other=other,
-            display_name=display_name,
-            project_id=project_id,
-            project_name=project_name,
-            feedback_stats=feedback_stats,
-            num_datapoints=num_datapoints,
-            experiment_id=experiment_id,
+            prompt_template=prompt_template,
+            chat_template=chat_template,
+            endpoint=endpoint,
             _configuration=_configuration,
             **kwargs,
         )
 
 from humanloop.model.chat_message import ChatMessage
+from humanloop.model.config_type import ConfigType
 from humanloop.model.model_endpoints import ModelEndpoints
 from humanloop.model.model_providers import ModelProviders
-from humanloop.model.src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response import SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse
```

### Comparing `humanloop-0.4.2/humanloop/model/src_external_app_models_v3_model_configs_project_model_config_response.pyi` & `humanloop-0.4.3/humanloop/model/model_config_response2.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -19,43 +19,37 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class SrcExternalAppModelsV3ModelConfigsProjectModelConfigResponse(
+class ModelConfigResponse2(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
 
-    Extends the core ModelConfig request object to include Humanloop generated
-identifier and method for serializing response from ModelConfig domain object.
+    Model config request
     """
 
 
     class MetaOapg:
         required = {
-            "updated_at",
-            "last_used",
-            "created_at",
+            "name",
             "model",
             "id",
+            "type",
         }
         
         class properties:
-            model = schemas.StrSchema
             id = schemas.StrSchema
-            created_at = schemas.DateTimeSchema
-            updated_at = schemas.DateTimeSchema
-            last_used = schemas.DateTimeSchema
             
             
-            class provider(
+            class type(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
                     
                     @classmethod
@@ -65,33 +59,37 @@
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            ModelProviders,
+                            ConfigType,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'provider':
+                ) -> 'type':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
+            name = schemas.StrSchema
+            model = schemas.StrSchema
+            description = schemas.StrSchema
+            other = schemas.DictSchema
             
             
-            class endpoint(
+            class provider(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
                     
                     @classmethod
@@ -101,59 +99,32 @@
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            ModelEndpoints,
+                            ModelProviders,
                         ]
             
             
                 def __new__(
                     cls,
                     *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'endpoint':
+                ) -> 'provider':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            prompt_template = schemas.StrSchema
-            
-            
-            class chat_template(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['ChatMessage']:
-                        return ChatMessage
-            
-                def __new__(
-                    cls,
-                    arg: typing.Union[typing.Tuple['ChatMessage'], typing.List['ChatMessage']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'chat_template':
-                    return super().__new__(
-                        cls,
-                        arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'ChatMessage':
-                    return super().__getitem__(i)
-            temperature = schemas.NumberSchema
             max_tokens = schemas.IntSchema
+            temperature = schemas.NumberSchema
             top_p = schemas.NumberSchema
             
             
             class stop(
                 schemas.ComposedSchema,
             ):
             
@@ -210,278 +181,254 @@
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             presence_penalty = schemas.NumberSchema
             frequency_penalty = schemas.NumberSchema
-            other = schemas.DictSchema
-            display_name = schemas.StrSchema
-            project_id = schemas.StrSchema
-            project_name = schemas.StrSchema
+            prompt_template = schemas.StrSchema
             
             
-            class feedback_stats(
+            class chat_template(
                 schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
                     @staticmethod
-                    def items() -> typing.Type['SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse']:
-                        return SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse
+                    def items() -> typing.Type['ChatMessage']:
+                        return ChatMessage
             
                 def __new__(
                     cls,
-                    arg: typing.Union[typing.Tuple['SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse'], typing.List['SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse']],
+                    arg: typing.Union[typing.Tuple['ChatMessage'], typing.List['ChatMessage']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'feedback_stats':
+                ) -> 'chat_template':
                     return super().__new__(
                         cls,
                         arg,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> 'SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse':
+                def __getitem__(self, i: int) -> 'ChatMessage':
                     return super().__getitem__(i)
-            num_datapoints = schemas.IntSchema
-            experiment_id = schemas.StrSchema
+            
+            
+            class endpoint(
+                schemas.ComposedSchema,
+            ):
+            
+            
+                class MetaOapg:
+                    
+                    @classmethod
+                    @functools.lru_cache()
+                    def all_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            ModelEndpoints,
+                        ]
+            
+            
+                def __new__(
+                    cls,
+                    *args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+                ) -> 'endpoint':
+                    return super().__new__(
+                        cls,
+                        *args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
             __annotations__ = {
-                "model": model,
                 "id": id,
-                "created_at": created_at,
-                "updated_at": updated_at,
-                "last_used": last_used,
+                "type": type,
+                "name": name,
+                "model": model,
+                "description": description,
+                "other": other,
                 "provider": provider,
-                "endpoint": endpoint,
-                "prompt_template": prompt_template,
-                "chat_template": chat_template,
-                "temperature": temperature,
                 "max_tokens": max_tokens,
+                "temperature": temperature,
                 "top_p": top_p,
                 "stop": stop,
                 "presence_penalty": presence_penalty,
                 "frequency_penalty": frequency_penalty,
-                "other": other,
-                "display_name": display_name,
-                "project_id": project_id,
-                "project_name": project_name,
-                "feedback_stats": feedback_stats,
-                "num_datapoints": num_datapoints,
-                "experiment_id": experiment_id,
+                "prompt_template": prompt_template,
+                "chat_template": chat_template,
+                "endpoint": endpoint,
             }
     
-    updated_at: MetaOapg.properties.updated_at
-    last_used: MetaOapg.properties.last_used
-    created_at: MetaOapg.properties.created_at
+    name: MetaOapg.properties.name
     model: MetaOapg.properties.model
     id: MetaOapg.properties.id
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
+    type: MetaOapg.properties.type
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
+    def __getitem__(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
+    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["last_used"]) -> MetaOapg.properties.last_used: ...
+    def __getitem__(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["provider"]) -> MetaOapg.properties.provider: ...
+    def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["endpoint"]) -> MetaOapg.properties.endpoint: ...
+    def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["prompt_template"]) -> MetaOapg.properties.prompt_template: ...
+    def __getitem__(self, name: typing_extensions.Literal["provider"]) -> MetaOapg.properties.provider: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["chat_template"]) -> MetaOapg.properties.chat_template: ...
+    def __getitem__(self, name: typing_extensions.Literal["max_tokens"]) -> MetaOapg.properties.max_tokens: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["temperature"]) -> MetaOapg.properties.temperature: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["max_tokens"]) -> MetaOapg.properties.max_tokens: ...
-    
-    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["top_p"]) -> MetaOapg.properties.top_p: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["stop"]) -> MetaOapg.properties.stop: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["presence_penalty"]) -> MetaOapg.properties.presence_penalty: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["frequency_penalty"]) -> MetaOapg.properties.frequency_penalty: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["display_name"]) -> MetaOapg.properties.display_name: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["project_id"]) -> MetaOapg.properties.project_id: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["project_name"]) -> MetaOapg.properties.project_name: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["feedback_stats"]) -> MetaOapg.properties.feedback_stats: ...
+    def __getitem__(self, name: typing_extensions.Literal["prompt_template"]) -> MetaOapg.properties.prompt_template: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["num_datapoints"]) -> MetaOapg.properties.num_datapoints: ...
+    def __getitem__(self, name: typing_extensions.Literal["chat_template"]) -> MetaOapg.properties.chat_template: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["experiment_id"]) -> MetaOapg.properties.experiment_id: ...
+    def __getitem__(self, name: typing_extensions.Literal["endpoint"]) -> MetaOapg.properties.endpoint: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model", "id", "created_at", "updated_at", "last_used", "provider", "endpoint", "prompt_template", "chat_template", "temperature", "max_tokens", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "display_name", "project_id", "project_name", "feedback_stats", "num_datapoints", "experiment_id", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "model", "description", "other", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "prompt_template", "chat_template", "endpoint", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["last_used"]) -> MetaOapg.properties.last_used: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["provider"]) -> typing.Union[MetaOapg.properties.provider, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["endpoint"]) -> typing.Union[MetaOapg.properties.endpoint, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["prompt_template"]) -> typing.Union[MetaOapg.properties.prompt_template, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["provider"]) -> typing.Union[MetaOapg.properties.provider, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["chat_template"]) -> typing.Union[MetaOapg.properties.chat_template, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["max_tokens"]) -> typing.Union[MetaOapg.properties.max_tokens, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["temperature"]) -> typing.Union[MetaOapg.properties.temperature, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["max_tokens"]) -> typing.Union[MetaOapg.properties.max_tokens, schemas.Unset]: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["top_p"]) -> typing.Union[MetaOapg.properties.top_p, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["stop"]) -> typing.Union[MetaOapg.properties.stop, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["presence_penalty"]) -> typing.Union[MetaOapg.properties.presence_penalty, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["frequency_penalty"]) -> typing.Union[MetaOapg.properties.frequency_penalty, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["display_name"]) -> typing.Union[MetaOapg.properties.display_name, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["project_id"]) -> typing.Union[MetaOapg.properties.project_id, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["project_name"]) -> typing.Union[MetaOapg.properties.project_name, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["feedback_stats"]) -> typing.Union[MetaOapg.properties.feedback_stats, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["prompt_template"]) -> typing.Union[MetaOapg.properties.prompt_template, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["num_datapoints"]) -> typing.Union[MetaOapg.properties.num_datapoints, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["chat_template"]) -> typing.Union[MetaOapg.properties.chat_template, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["experiment_id"]) -> typing.Union[MetaOapg.properties.experiment_id, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["endpoint"]) -> typing.Union[MetaOapg.properties.endpoint, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model", "id", "created_at", "updated_at", "last_used", "provider", "endpoint", "prompt_template", "chat_template", "temperature", "max_tokens", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "display_name", "project_id", "project_name", "feedback_stats", "num_datapoints", "experiment_id", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "type", "name", "model", "description", "other", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "prompt_template", "chat_template", "endpoint", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        updated_at: typing.Union[MetaOapg.properties.updated_at, str, datetime, ],
-        last_used: typing.Union[MetaOapg.properties.last_used, str, datetime, ],
-        created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, ],
+        name: typing.Union[MetaOapg.properties.name, str, ],
         model: typing.Union[MetaOapg.properties.model, str, ],
         id: typing.Union[MetaOapg.properties.id, str, ],
+        type: typing.Union[MetaOapg.properties.type, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+        description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
+        other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         provider: typing.Union[MetaOapg.properties.provider, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-        endpoint: typing.Union[MetaOapg.properties.endpoint, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-        prompt_template: typing.Union[MetaOapg.properties.prompt_template, str, schemas.Unset] = schemas.unset,
-        chat_template: typing.Union[MetaOapg.properties.chat_template, list, tuple, schemas.Unset] = schemas.unset,
-        temperature: typing.Union[MetaOapg.properties.temperature, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         max_tokens: typing.Union[MetaOapg.properties.max_tokens, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        temperature: typing.Union[MetaOapg.properties.temperature, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         top_p: typing.Union[MetaOapg.properties.top_p, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         stop: typing.Union[MetaOapg.properties.stop, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         presence_penalty: typing.Union[MetaOapg.properties.presence_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         frequency_penalty: typing.Union[MetaOapg.properties.frequency_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
-        other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
-        display_name: typing.Union[MetaOapg.properties.display_name, str, schemas.Unset] = schemas.unset,
-        project_id: typing.Union[MetaOapg.properties.project_id, str, schemas.Unset] = schemas.unset,
-        project_name: typing.Union[MetaOapg.properties.project_name, str, schemas.Unset] = schemas.unset,
-        feedback_stats: typing.Union[MetaOapg.properties.feedback_stats, list, tuple, schemas.Unset] = schemas.unset,
-        num_datapoints: typing.Union[MetaOapg.properties.num_datapoints, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        experiment_id: typing.Union[MetaOapg.properties.experiment_id, str, schemas.Unset] = schemas.unset,
+        prompt_template: typing.Union[MetaOapg.properties.prompt_template, str, schemas.Unset] = schemas.unset,
+        chat_template: typing.Union[MetaOapg.properties.chat_template, list, tuple, schemas.Unset] = schemas.unset,
+        endpoint: typing.Union[MetaOapg.properties.endpoint, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SrcExternalAppModelsV3ModelConfigsProjectModelConfigResponse':
+    ) -> 'ModelConfigResponse2':
         return super().__new__(
             cls,
             *args,
-            updated_at=updated_at,
-            last_used=last_used,
-            created_at=created_at,
+            name=name,
             model=model,
             id=id,
+            type=type,
+            description=description,
+            other=other,
             provider=provider,
-            endpoint=endpoint,
-            prompt_template=prompt_template,
-            chat_template=chat_template,
-            temperature=temperature,
             max_tokens=max_tokens,
+            temperature=temperature,
             top_p=top_p,
             stop=stop,
             presence_penalty=presence_penalty,
             frequency_penalty=frequency_penalty,
-            other=other,
-            display_name=display_name,
-            project_id=project_id,
-            project_name=project_name,
-            feedback_stats=feedback_stats,
-            num_datapoints=num_datapoints,
-            experiment_id=experiment_id,
+            prompt_template=prompt_template,
+            chat_template=chat_template,
+            endpoint=endpoint,
             _configuration=_configuration,
             **kwargs,
         )
 
 from humanloop.model.chat_message import ChatMessage
+from humanloop.model.config_type import ConfigType
 from humanloop.model.model_endpoints import ModelEndpoints
 from humanloop.model.model_providers import ModelProviders
-from humanloop.model.src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response import SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse
```

### Comparing `humanloop-0.4.2/humanloop/model/src_external_app_models_v4_model_configs_model_config_response.py` & `humanloop-0.4.3/humanloop/model/log_model_config_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,34 +19,42 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class SrcExternalAppModelsV4ModelConfigsModelConfigResponse(
+class LogModelConfigRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
 
-    Extends the core ModelConfig request object to include Humanloop generated
-identifier and method for serializing response from ModelConfig domain object.
+    Model config request that supports both chat and completion.
+
+Implemented here with the full set of fields from both
+ChatModelConfigRequest and CompletionModelConfigRequest.
+
+Ideally we'd use `Union[ChatModelConfigRequest, CompletionModelConfigRequest]`
+but that seems to cause Pydantic errors, especially with the `type` discriminator.
+
+Validation is done to ensure that only one of `chat_template` and
+`prompt_template` is provided, and that the provided one properly
+corresponds to the endpoint.
+This defaults to `complete` endpoint.
     """
 
 
     class MetaOapg:
         required = {
             "model",
-            "id",
         }
         
         class properties:
             model = schemas.StrSchema
-            id = schemas.StrSchema
             
             
             class provider(
                 schemas.ComposedSchema,
             ):
             
             
@@ -142,42 +150,14 @@
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             presence_penalty = schemas.NumberSchema
             frequency_penalty = schemas.NumberSchema
             other = schemas.DictSchema
-            display_name = schemas.StrSchema
-            prompt_template = schemas.StrSchema
-            
-            
-            class chat_template(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['ChatMessage']:
-                        return ChatMessage
-            
-                def __new__(
-                    cls,
-                    arg: typing.Union[typing.Tuple['ChatMessage'], typing.List['ChatMessage']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'chat_template':
-                    return super().__new__(
-                        cls,
-                        arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'ChatMessage':
-                    return super().__getitem__(i)
             
             
             class endpoint(
                 schemas.ComposedSchema,
             ):
             
             
@@ -206,41 +186,62 @@
                 ) -> 'endpoint':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
+            prompt_template = schemas.StrSchema
+            
+            
+            class chat_template(
+                schemas.ListSchema
+            ):
+            
+            
+                class MetaOapg:
+                    
+                    @staticmethod
+                    def items() -> typing.Type['ChatMessage']:
+                        return ChatMessage
+            
+                def __new__(
+                    cls,
+                    arg: typing.Union[typing.Tuple['ChatMessage'], typing.List['ChatMessage']],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                ) -> 'chat_template':
+                    return super().__new__(
+                        cls,
+                        arg,
+                        _configuration=_configuration,
+                    )
+            
+                def __getitem__(self, i: int) -> 'ChatMessage':
+                    return super().__getitem__(i)
             __annotations__ = {
                 "model": model,
-                "id": id,
                 "provider": provider,
                 "max_tokens": max_tokens,
                 "temperature": temperature,
                 "top_p": top_p,
                 "stop": stop,
                 "presence_penalty": presence_penalty,
                 "frequency_penalty": frequency_penalty,
                 "other": other,
-                "display_name": display_name,
+                "endpoint": endpoint,
                 "prompt_template": prompt_template,
                 "chat_template": chat_template,
-                "endpoint": endpoint,
             }
     
     model: MetaOapg.properties.model
-    id: MetaOapg.properties.id
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
-    
-    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["provider"]) -> MetaOapg.properties.provider: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["max_tokens"]) -> MetaOapg.properties.max_tokens: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["temperature"]) -> MetaOapg.properties.temperature: ...
@@ -257,40 +258,34 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["frequency_penalty"]) -> MetaOapg.properties.frequency_penalty: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["display_name"]) -> MetaOapg.properties.display_name: ...
+    def __getitem__(self, name: typing_extensions.Literal["endpoint"]) -> MetaOapg.properties.endpoint: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["prompt_template"]) -> MetaOapg.properties.prompt_template: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["chat_template"]) -> MetaOapg.properties.chat_template: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["endpoint"]) -> MetaOapg.properties.endpoint: ...
-    
-    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model", "id", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "display_name", "prompt_template", "chat_template", "endpoint", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "endpoint", "prompt_template", "chat_template", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["provider"]) -> typing.Union[MetaOapg.properties.provider, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["max_tokens"]) -> typing.Union[MetaOapg.properties.max_tokens, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["temperature"]) -> typing.Union[MetaOapg.properties.temperature, schemas.Unset]: ...
@@ -307,69 +302,62 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["frequency_penalty"]) -> typing.Union[MetaOapg.properties.frequency_penalty, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["display_name"]) -> typing.Union[MetaOapg.properties.display_name, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["endpoint"]) -> typing.Union[MetaOapg.properties.endpoint, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["prompt_template"]) -> typing.Union[MetaOapg.properties.prompt_template, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["chat_template"]) -> typing.Union[MetaOapg.properties.chat_template, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["endpoint"]) -> typing.Union[MetaOapg.properties.endpoint, schemas.Unset]: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model", "id", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "display_name", "prompt_template", "chat_template", "endpoint", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "endpoint", "prompt_template", "chat_template", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         model: typing.Union[MetaOapg.properties.model, str, ],
-        id: typing.Union[MetaOapg.properties.id, str, ],
         provider: typing.Union[MetaOapg.properties.provider, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         max_tokens: typing.Union[MetaOapg.properties.max_tokens, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         temperature: typing.Union[MetaOapg.properties.temperature, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         top_p: typing.Union[MetaOapg.properties.top_p, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         stop: typing.Union[MetaOapg.properties.stop, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         presence_penalty: typing.Union[MetaOapg.properties.presence_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         frequency_penalty: typing.Union[MetaOapg.properties.frequency_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
-        display_name: typing.Union[MetaOapg.properties.display_name, str, schemas.Unset] = schemas.unset,
+        endpoint: typing.Union[MetaOapg.properties.endpoint, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         prompt_template: typing.Union[MetaOapg.properties.prompt_template, str, schemas.Unset] = schemas.unset,
         chat_template: typing.Union[MetaOapg.properties.chat_template, list, tuple, schemas.Unset] = schemas.unset,
-        endpoint: typing.Union[MetaOapg.properties.endpoint, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SrcExternalAppModelsV4ModelConfigsModelConfigResponse':
+    ) -> 'LogModelConfigRequest':
         return super().__new__(
             cls,
             *args,
             model=model,
-            id=id,
             provider=provider,
             max_tokens=max_tokens,
             temperature=temperature,
             top_p=top_p,
             stop=stop,
             presence_penalty=presence_penalty,
             frequency_penalty=frequency_penalty,
             other=other,
-            display_name=display_name,
+            endpoint=endpoint,
             prompt_template=prompt_template,
             chat_template=chat_template,
-            endpoint=endpoint,
             _configuration=_configuration,
             **kwargs,
         )
 
 from humanloop.model.chat_message import ChatMessage
 from humanloop.model.model_endpoints import ModelEndpoints
 from humanloop.model.model_providers import ModelProviders
```

### Comparing `humanloop-0.4.2/humanloop/model/src_external_app_models_v4_model_configs_model_config_response.pyi` & `humanloop-0.4.3/humanloop/model/log_model_config_request.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -19,34 +19,42 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class SrcExternalAppModelsV4ModelConfigsModelConfigResponse(
+class LogModelConfigRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
 
-    Extends the core ModelConfig request object to include Humanloop generated
-identifier and method for serializing response from ModelConfig domain object.
+    Model config request that supports both chat and completion.
+
+Implemented here with the full set of fields from both
+ChatModelConfigRequest and CompletionModelConfigRequest.
+
+Ideally we'd use `Union[ChatModelConfigRequest, CompletionModelConfigRequest]`
+but that seems to cause Pydantic errors, especially with the `type` discriminator.
+
+Validation is done to ensure that only one of `chat_template` and
+`prompt_template` is provided, and that the provided one properly
+corresponds to the endpoint.
+This defaults to `complete` endpoint.
     """
 
 
     class MetaOapg:
         required = {
             "model",
-            "id",
         }
         
         class properties:
             model = schemas.StrSchema
-            id = schemas.StrSchema
             
             
             class provider(
                 schemas.ComposedSchema,
             ):
             
             
@@ -142,42 +150,14 @@
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             presence_penalty = schemas.NumberSchema
             frequency_penalty = schemas.NumberSchema
             other = schemas.DictSchema
-            display_name = schemas.StrSchema
-            prompt_template = schemas.StrSchema
-            
-            
-            class chat_template(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['ChatMessage']:
-                        return ChatMessage
-            
-                def __new__(
-                    cls,
-                    arg: typing.Union[typing.Tuple['ChatMessage'], typing.List['ChatMessage']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'chat_template':
-                    return super().__new__(
-                        cls,
-                        arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'ChatMessage':
-                    return super().__getitem__(i)
             
             
             class endpoint(
                 schemas.ComposedSchema,
             ):
             
             
@@ -206,41 +186,62 @@
                 ) -> 'endpoint':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
+            prompt_template = schemas.StrSchema
+            
+            
+            class chat_template(
+                schemas.ListSchema
+            ):
+            
+            
+                class MetaOapg:
+                    
+                    @staticmethod
+                    def items() -> typing.Type['ChatMessage']:
+                        return ChatMessage
+            
+                def __new__(
+                    cls,
+                    arg: typing.Union[typing.Tuple['ChatMessage'], typing.List['ChatMessage']],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                ) -> 'chat_template':
+                    return super().__new__(
+                        cls,
+                        arg,
+                        _configuration=_configuration,
+                    )
+            
+                def __getitem__(self, i: int) -> 'ChatMessage':
+                    return super().__getitem__(i)
             __annotations__ = {
                 "model": model,
-                "id": id,
                 "provider": provider,
                 "max_tokens": max_tokens,
                 "temperature": temperature,
                 "top_p": top_p,
                 "stop": stop,
                 "presence_penalty": presence_penalty,
                 "frequency_penalty": frequency_penalty,
                 "other": other,
-                "display_name": display_name,
+                "endpoint": endpoint,
                 "prompt_template": prompt_template,
                 "chat_template": chat_template,
-                "endpoint": endpoint,
             }
     
     model: MetaOapg.properties.model
-    id: MetaOapg.properties.id
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
-    
-    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["provider"]) -> MetaOapg.properties.provider: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["max_tokens"]) -> MetaOapg.properties.max_tokens: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["temperature"]) -> MetaOapg.properties.temperature: ...
@@ -257,40 +258,34 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["frequency_penalty"]) -> MetaOapg.properties.frequency_penalty: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["display_name"]) -> MetaOapg.properties.display_name: ...
+    def __getitem__(self, name: typing_extensions.Literal["endpoint"]) -> MetaOapg.properties.endpoint: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["prompt_template"]) -> MetaOapg.properties.prompt_template: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["chat_template"]) -> MetaOapg.properties.chat_template: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["endpoint"]) -> MetaOapg.properties.endpoint: ...
-    
-    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model", "id", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "display_name", "prompt_template", "chat_template", "endpoint", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "endpoint", "prompt_template", "chat_template", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["provider"]) -> typing.Union[MetaOapg.properties.provider, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["max_tokens"]) -> typing.Union[MetaOapg.properties.max_tokens, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["temperature"]) -> typing.Union[MetaOapg.properties.temperature, schemas.Unset]: ...
@@ -307,69 +302,62 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["frequency_penalty"]) -> typing.Union[MetaOapg.properties.frequency_penalty, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["display_name"]) -> typing.Union[MetaOapg.properties.display_name, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["endpoint"]) -> typing.Union[MetaOapg.properties.endpoint, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["prompt_template"]) -> typing.Union[MetaOapg.properties.prompt_template, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["chat_template"]) -> typing.Union[MetaOapg.properties.chat_template, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["endpoint"]) -> typing.Union[MetaOapg.properties.endpoint, schemas.Unset]: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model", "id", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "display_name", "prompt_template", "chat_template", "endpoint", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "endpoint", "prompt_template", "chat_template", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         model: typing.Union[MetaOapg.properties.model, str, ],
-        id: typing.Union[MetaOapg.properties.id, str, ],
         provider: typing.Union[MetaOapg.properties.provider, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         max_tokens: typing.Union[MetaOapg.properties.max_tokens, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         temperature: typing.Union[MetaOapg.properties.temperature, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         top_p: typing.Union[MetaOapg.properties.top_p, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         stop: typing.Union[MetaOapg.properties.stop, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         presence_penalty: typing.Union[MetaOapg.properties.presence_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         frequency_penalty: typing.Union[MetaOapg.properties.frequency_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
-        display_name: typing.Union[MetaOapg.properties.display_name, str, schemas.Unset] = schemas.unset,
+        endpoint: typing.Union[MetaOapg.properties.endpoint, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         prompt_template: typing.Union[MetaOapg.properties.prompt_template, str, schemas.Unset] = schemas.unset,
         chat_template: typing.Union[MetaOapg.properties.chat_template, list, tuple, schemas.Unset] = schemas.unset,
-        endpoint: typing.Union[MetaOapg.properties.endpoint, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SrcExternalAppModelsV4ModelConfigsModelConfigResponse':
+    ) -> 'LogModelConfigRequest':
         return super().__new__(
             cls,
             *args,
             model=model,
-            id=id,
             provider=provider,
             max_tokens=max_tokens,
             temperature=temperature,
             top_p=top_p,
             stop=stop,
             presence_penalty=presence_penalty,
             frequency_penalty=frequency_penalty,
             other=other,
-            display_name=display_name,
+            endpoint=endpoint,
             prompt_template=prompt_template,
             chat_template=chat_template,
-            endpoint=endpoint,
             _configuration=_configuration,
             **kwargs,
         )
 
 from humanloop.model.chat_message import ChatMessage
 from humanloop.model.model_endpoints import ModelEndpoints
 from humanloop.model.model_providers import ModelProviders
```

### Comparing `humanloop-0.4.2/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_feedback_stats_response.py` & `humanloop-0.4.3/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse(
+class SrcExternalAppModelsV4ProjectConfigsProjectModelConfigFeedbackStatsResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
@@ -100,15 +100,15 @@
         *args: typing.Union[dict, frozendict.frozendict, ],
         feedback_value: typing.Union[MetaOapg.properties.feedback_value, str, ],
         feedback_type_id: typing.Union[MetaOapg.properties.feedback_type_id, decimal.Decimal, int, ],
         feedback_type: typing.Union[MetaOapg.properties.feedback_type, str, ],
         feedback_count: typing.Union[MetaOapg.properties.feedback_count, decimal.Decimal, int, ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse':
+    ) -> 'SrcExternalAppModelsV4ProjectConfigsProjectModelConfigFeedbackStatsResponse':
         return super().__new__(
             cls,
             *args,
             feedback_value=feedback_value,
             feedback_type_id=feedback_type_id,
             feedback_type=feedback_type,
             feedback_count=feedback_count,
```

### Comparing `humanloop-0.4.2/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_feedback_stats_response.pyi` & `humanloop-0.4.3/humanloop/model/src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse(
+class SrcExternalAppModelsV4ProjectConfigsProjectModelConfigFeedbackStatsResponse(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
     """
 
 
@@ -100,15 +100,15 @@
         *args: typing.Union[dict, frozendict.frozendict, ],
         feedback_value: typing.Union[MetaOapg.properties.feedback_value, str, ],
         feedback_type_id: typing.Union[MetaOapg.properties.feedback_type_id, decimal.Decimal, int, ],
         feedback_type: typing.Union[MetaOapg.properties.feedback_type, str, ],
         feedback_count: typing.Union[MetaOapg.properties.feedback_count, decimal.Decimal, int, ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse':
+    ) -> 'SrcExternalAppModelsV4ProjectConfigsProjectModelConfigFeedbackStatsResponse':
         return super().__new__(
             cls,
             *args,
             feedback_value=feedback_value,
             feedback_type_id=feedback_type_id,
             feedback_type=feedback_type,
             feedback_count=feedback_count,
```

### Comparing `humanloop-0.4.2/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_response.py` & `humanloop-0.4.3/humanloop/model/trace_model_config_request.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -19,40 +19,55 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse(
+class TraceModelConfigRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
 
-    Extends the core ModelConfig request object to include Humanloop generated
-identifier and method for serializing response from ModelConfig domain object.
+    Model config request that supports both chat and completion.
+
+Implemented here with the full set of fields from both
+ChatModelConfigRequest and CompletionModelConfigRequest.
+
+Ideally we'd use `Union[ChatModelConfigRequest, CompletionModelConfigRequest]`
+but that seems to cause Pydantic errors, especially with the `type` discriminator.
+
+Validation is done to ensure that only one of `chat_template` and
+`prompt_template` is provided, and that the provided one properly
+corresponds to the endpoint.
+This defaults to `complete` endpoint.
     """
 
 
     class MetaOapg:
         required = {
-            "updated_at",
-            "last_used",
-            "created_at",
             "model",
-            "id",
+            "type",
         }
         
         class properties:
             model = schemas.StrSchema
-            id = schemas.StrSchema
-            created_at = schemas.DateTimeSchema
-            updated_at = schemas.DateTimeSchema
-            last_used = schemas.DateTimeSchema
+            
+            
+            class type(
+                schemas.EnumBase,
+                schemas.StrSchema
+            ):
+                
+                @schemas.classproperty
+                def MODEL(cls):
+                    return cls("model")
+            description = schemas.StrSchema
+            name = schemas.StrSchema
             
             
             class provider(
                 schemas.ComposedSchema,
             ):
             
             
@@ -148,42 +163,14 @@
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             presence_penalty = schemas.NumberSchema
             frequency_penalty = schemas.NumberSchema
             other = schemas.DictSchema
-            display_name = schemas.StrSchema
-            prompt_template = schemas.StrSchema
-            
-            
-            class chat_template(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['ChatMessage']:
-                        return ChatMessage
-            
-                def __new__(
-                    cls,
-                    arg: typing.Union[typing.Tuple['ChatMessage'], typing.List['ChatMessage']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'chat_template':
-                    return super().__new__(
-                        cls,
-                        arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'ChatMessage':
-                    return super().__getitem__(i)
             
             
             class endpoint(
                 schemas.ComposedSchema,
             ):
             
             
@@ -212,89 +199,74 @@
                 ) -> 'endpoint':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            project_id = schemas.StrSchema
-            project_name = schemas.StrSchema
+            prompt_template = schemas.StrSchema
             
             
-            class feedback_stats(
+            class chat_template(
                 schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
                     @staticmethod
-                    def items() -> typing.Type['SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse']:
-                        return SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse
+                    def items() -> typing.Type['ChatMessage']:
+                        return ChatMessage
             
                 def __new__(
                     cls,
-                    arg: typing.Union[typing.Tuple['SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse'], typing.List['SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse']],
+                    arg: typing.Union[typing.Tuple['ChatMessage'], typing.List['ChatMessage']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'feedback_stats':
+                ) -> 'chat_template':
                     return super().__new__(
                         cls,
                         arg,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> 'SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse':
+                def __getitem__(self, i: int) -> 'ChatMessage':
                     return super().__getitem__(i)
-            num_datapoints = schemas.IntSchema
-            experiment_id = schemas.StrSchema
             __annotations__ = {
                 "model": model,
-                "id": id,
-                "created_at": created_at,
-                "updated_at": updated_at,
-                "last_used": last_used,
+                "type": type,
+                "description": description,
+                "name": name,
                 "provider": provider,
                 "max_tokens": max_tokens,
                 "temperature": temperature,
                 "top_p": top_p,
                 "stop": stop,
                 "presence_penalty": presence_penalty,
                 "frequency_penalty": frequency_penalty,
                 "other": other,
-                "display_name": display_name,
+                "endpoint": endpoint,
                 "prompt_template": prompt_template,
                 "chat_template": chat_template,
-                "endpoint": endpoint,
-                "project_id": project_id,
-                "project_name": project_name,
-                "feedback_stats": feedback_stats,
-                "num_datapoints": num_datapoints,
-                "experiment_id": experiment_id,
             }
+        additional_properties = schemas.NotAnyTypeSchema
     
-    updated_at: MetaOapg.properties.updated_at
-    last_used: MetaOapg.properties.last_used
-    created_at: MetaOapg.properties.created_at
     model: MetaOapg.properties.model
-    id: MetaOapg.properties.id
+    type: MetaOapg.properties.type
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    def __getitem__(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
+    def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["last_used"]) -> MetaOapg.properties.last_used: ...
+    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["provider"]) -> MetaOapg.properties.provider: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["max_tokens"]) -> MetaOapg.properties.max_tokens: ...
     
@@ -313,62 +285,37 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["frequency_penalty"]) -> MetaOapg.properties.frequency_penalty: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["display_name"]) -> MetaOapg.properties.display_name: ...
+    def __getitem__(self, name: typing_extensions.Literal["endpoint"]) -> MetaOapg.properties.endpoint: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["prompt_template"]) -> MetaOapg.properties.prompt_template: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["chat_template"]) -> MetaOapg.properties.chat_template: ...
     
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["endpoint"]) -> MetaOapg.properties.endpoint: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["project_id"]) -> MetaOapg.properties.project_id: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["project_name"]) -> MetaOapg.properties.project_name: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["feedback_stats"]) -> MetaOapg.properties.feedback_stats: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["num_datapoints"]) -> MetaOapg.properties.num_datapoints: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["experiment_id"]) -> MetaOapg.properties.experiment_id: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model", "id", "created_at", "updated_at", "last_used", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "display_name", "prompt_template", "chat_template", "endpoint", "project_id", "project_name", "feedback_stats", "num_datapoints", "experiment_id", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model"], typing_extensions.Literal["type"], typing_extensions.Literal["description"], typing_extensions.Literal["name"], typing_extensions.Literal["provider"], typing_extensions.Literal["max_tokens"], typing_extensions.Literal["temperature"], typing_extensions.Literal["top_p"], typing_extensions.Literal["stop"], typing_extensions.Literal["presence_penalty"], typing_extensions.Literal["frequency_penalty"], typing_extensions.Literal["other"], typing_extensions.Literal["endpoint"], typing_extensions.Literal["prompt_template"], typing_extensions.Literal["chat_template"], ]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
-    
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["last_used"]) -> MetaOapg.properties.last_used: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> typing.Union[MetaOapg.properties.name, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["provider"]) -> typing.Union[MetaOapg.properties.provider, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["max_tokens"]) -> typing.Union[MetaOapg.properties.max_tokens, schemas.Unset]: ...
     
@@ -387,101 +334,62 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["frequency_penalty"]) -> typing.Union[MetaOapg.properties.frequency_penalty, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["display_name"]) -> typing.Union[MetaOapg.properties.display_name, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["endpoint"]) -> typing.Union[MetaOapg.properties.endpoint, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["prompt_template"]) -> typing.Union[MetaOapg.properties.prompt_template, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["chat_template"]) -> typing.Union[MetaOapg.properties.chat_template, schemas.Unset]: ...
     
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["endpoint"]) -> typing.Union[MetaOapg.properties.endpoint, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["project_id"]) -> typing.Union[MetaOapg.properties.project_id, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["project_name"]) -> typing.Union[MetaOapg.properties.project_name, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["feedback_stats"]) -> typing.Union[MetaOapg.properties.feedback_stats, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["num_datapoints"]) -> typing.Union[MetaOapg.properties.num_datapoints, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["experiment_id"]) -> typing.Union[MetaOapg.properties.experiment_id, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model", "id", "created_at", "updated_at", "last_used", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "display_name", "prompt_template", "chat_template", "endpoint", "project_id", "project_name", "feedback_stats", "num_datapoints", "experiment_id", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model"], typing_extensions.Literal["type"], typing_extensions.Literal["description"], typing_extensions.Literal["name"], typing_extensions.Literal["provider"], typing_extensions.Literal["max_tokens"], typing_extensions.Literal["temperature"], typing_extensions.Literal["top_p"], typing_extensions.Literal["stop"], typing_extensions.Literal["presence_penalty"], typing_extensions.Literal["frequency_penalty"], typing_extensions.Literal["other"], typing_extensions.Literal["endpoint"], typing_extensions.Literal["prompt_template"], typing_extensions.Literal["chat_template"], ]):
         return super().get_item_oapg(name)
-    
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        updated_at: typing.Union[MetaOapg.properties.updated_at, str, datetime, ],
-        last_used: typing.Union[MetaOapg.properties.last_used, str, datetime, ],
-        created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, ],
         model: typing.Union[MetaOapg.properties.model, str, ],
-        id: typing.Union[MetaOapg.properties.id, str, ],
+        type: typing.Union[MetaOapg.properties.type, str, ],
+        description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
+        name: typing.Union[MetaOapg.properties.name, str, schemas.Unset] = schemas.unset,
         provider: typing.Union[MetaOapg.properties.provider, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         max_tokens: typing.Union[MetaOapg.properties.max_tokens, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         temperature: typing.Union[MetaOapg.properties.temperature, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         top_p: typing.Union[MetaOapg.properties.top_p, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         stop: typing.Union[MetaOapg.properties.stop, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         presence_penalty: typing.Union[MetaOapg.properties.presence_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         frequency_penalty: typing.Union[MetaOapg.properties.frequency_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
-        display_name: typing.Union[MetaOapg.properties.display_name, str, schemas.Unset] = schemas.unset,
+        endpoint: typing.Union[MetaOapg.properties.endpoint, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         prompt_template: typing.Union[MetaOapg.properties.prompt_template, str, schemas.Unset] = schemas.unset,
         chat_template: typing.Union[MetaOapg.properties.chat_template, list, tuple, schemas.Unset] = schemas.unset,
-        endpoint: typing.Union[MetaOapg.properties.endpoint, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-        project_id: typing.Union[MetaOapg.properties.project_id, str, schemas.Unset] = schemas.unset,
-        project_name: typing.Union[MetaOapg.properties.project_name, str, schemas.Unset] = schemas.unset,
-        feedback_stats: typing.Union[MetaOapg.properties.feedback_stats, list, tuple, schemas.Unset] = schemas.unset,
-        num_datapoints: typing.Union[MetaOapg.properties.num_datapoints, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        experiment_id: typing.Union[MetaOapg.properties.experiment_id, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse':
+    ) -> 'TraceModelConfigRequest':
         return super().__new__(
             cls,
             *args,
-            updated_at=updated_at,
-            last_used=last_used,
-            created_at=created_at,
             model=model,
-            id=id,
+            type=type,
+            description=description,
+            name=name,
             provider=provider,
             max_tokens=max_tokens,
             temperature=temperature,
             top_p=top_p,
             stop=stop,
             presence_penalty=presence_penalty,
             frequency_penalty=frequency_penalty,
             other=other,
-            display_name=display_name,
+            endpoint=endpoint,
             prompt_template=prompt_template,
             chat_template=chat_template,
-            endpoint=endpoint,
-            project_id=project_id,
-            project_name=project_name,
-            feedback_stats=feedback_stats,
-            num_datapoints=num_datapoints,
-            experiment_id=experiment_id,
             _configuration=_configuration,
-            **kwargs,
         )
 
 from humanloop.model.chat_message import ChatMessage
 from humanloop.model.model_endpoints import ModelEndpoints
 from humanloop.model.model_providers import ModelProviders
-from humanloop.model.src_external_app_models_v4_model_configs_project_model_config_feedback_stats_response import SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse
```

### Comparing `humanloop-0.4.2/humanloop/model/src_external_app_models_v4_model_configs_project_model_config_response.pyi` & `humanloop-0.4.3/humanloop/model/trace_model_config_request.py`

 * *Files 25% similar despite different names*

```diff
@@ -19,40 +19,61 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 
-class SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse(
+class TraceModelConfigRequest(
     schemas.DictSchema
 ):
     """
     This class is auto generated by Konfig (https://konfigthis.com)
 
-    Extends the core ModelConfig request object to include Humanloop generated
-identifier and method for serializing response from ModelConfig domain object.
+    Model config request that supports both chat and completion.
+
+Implemented here with the full set of fields from both
+ChatModelConfigRequest and CompletionModelConfigRequest.
+
+Ideally we'd use `Union[ChatModelConfigRequest, CompletionModelConfigRequest]`
+but that seems to cause Pydantic errors, especially with the `type` discriminator.
+
+Validation is done to ensure that only one of `chat_template` and
+`prompt_template` is provided, and that the provided one properly
+corresponds to the endpoint.
+This defaults to `complete` endpoint.
     """
 
 
     class MetaOapg:
         required = {
-            "updated_at",
-            "last_used",
-            "created_at",
             "model",
-            "id",
+            "type",
         }
         
         class properties:
             model = schemas.StrSchema
-            id = schemas.StrSchema
-            created_at = schemas.DateTimeSchema
-            updated_at = schemas.DateTimeSchema
-            last_used = schemas.DateTimeSchema
+            
+            
+            class type(
+                schemas.EnumBase,
+                schemas.StrSchema
+            ):
+            
+            
+                class MetaOapg:
+                    enum_value_to_name = {
+                        "model": "MODEL",
+                    }
+                
+                @schemas.classproperty
+                def MODEL(cls):
+                    return cls("model")
+            description = schemas.StrSchema
+            name = schemas.StrSchema
             
             
             class provider(
                 schemas.ComposedSchema,
             ):
             
             
@@ -148,42 +169,14 @@
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             presence_penalty = schemas.NumberSchema
             frequency_penalty = schemas.NumberSchema
             other = schemas.DictSchema
-            display_name = schemas.StrSchema
-            prompt_template = schemas.StrSchema
-            
-            
-            class chat_template(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['ChatMessage']:
-                        return ChatMessage
-            
-                def __new__(
-                    cls,
-                    arg: typing.Union[typing.Tuple['ChatMessage'], typing.List['ChatMessage']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'chat_template':
-                    return super().__new__(
-                        cls,
-                        arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'ChatMessage':
-                    return super().__getitem__(i)
             
             
             class endpoint(
                 schemas.ComposedSchema,
             ):
             
             
@@ -212,89 +205,74 @@
                 ) -> 'endpoint':
                     return super().__new__(
                         cls,
                         *args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            project_id = schemas.StrSchema
-            project_name = schemas.StrSchema
+            prompt_template = schemas.StrSchema
             
             
-            class feedback_stats(
+            class chat_template(
                 schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
                     @staticmethod
-                    def items() -> typing.Type['SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse']:
-                        return SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse
+                    def items() -> typing.Type['ChatMessage']:
+                        return ChatMessage
             
                 def __new__(
                     cls,
-                    arg: typing.Union[typing.Tuple['SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse'], typing.List['SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse']],
+                    arg: typing.Union[typing.Tuple['ChatMessage'], typing.List['ChatMessage']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'feedback_stats':
+                ) -> 'chat_template':
                     return super().__new__(
                         cls,
                         arg,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> 'SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse':
+                def __getitem__(self, i: int) -> 'ChatMessage':
                     return super().__getitem__(i)
-            num_datapoints = schemas.IntSchema
-            experiment_id = schemas.StrSchema
             __annotations__ = {
                 "model": model,
-                "id": id,
-                "created_at": created_at,
-                "updated_at": updated_at,
-                "last_used": last_used,
+                "type": type,
+                "description": description,
+                "name": name,
                 "provider": provider,
                 "max_tokens": max_tokens,
                 "temperature": temperature,
                 "top_p": top_p,
                 "stop": stop,
                 "presence_penalty": presence_penalty,
                 "frequency_penalty": frequency_penalty,
                 "other": other,
-                "display_name": display_name,
+                "endpoint": endpoint,
                 "prompt_template": prompt_template,
                 "chat_template": chat_template,
-                "endpoint": endpoint,
-                "project_id": project_id,
-                "project_name": project_name,
-                "feedback_stats": feedback_stats,
-                "num_datapoints": num_datapoints,
-                "experiment_id": experiment_id,
             }
+        additional_properties = schemas.NotAnyTypeSchema
     
-    updated_at: MetaOapg.properties.updated_at
-    last_used: MetaOapg.properties.last_used
-    created_at: MetaOapg.properties.created_at
     model: MetaOapg.properties.model
-    id: MetaOapg.properties.id
+    type: MetaOapg.properties.type
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
+    def __getitem__(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
+    def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["last_used"]) -> MetaOapg.properties.last_used: ...
+    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["provider"]) -> MetaOapg.properties.provider: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["max_tokens"]) -> MetaOapg.properties.max_tokens: ...
     
@@ -313,62 +291,37 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["frequency_penalty"]) -> MetaOapg.properties.frequency_penalty: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["other"]) -> MetaOapg.properties.other: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["display_name"]) -> MetaOapg.properties.display_name: ...
+    def __getitem__(self, name: typing_extensions.Literal["endpoint"]) -> MetaOapg.properties.endpoint: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["prompt_template"]) -> MetaOapg.properties.prompt_template: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["chat_template"]) -> MetaOapg.properties.chat_template: ...
     
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["endpoint"]) -> MetaOapg.properties.endpoint: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["project_id"]) -> MetaOapg.properties.project_id: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["project_name"]) -> MetaOapg.properties.project_name: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["feedback_stats"]) -> MetaOapg.properties.feedback_stats: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["num_datapoints"]) -> MetaOapg.properties.num_datapoints: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["experiment_id"]) -> MetaOapg.properties.experiment_id: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model", "id", "created_at", "updated_at", "last_used", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "display_name", "prompt_template", "chat_template", "endpoint", "project_id", "project_name", "feedback_stats", "num_datapoints", "experiment_id", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["model"], typing_extensions.Literal["type"], typing_extensions.Literal["description"], typing_extensions.Literal["name"], typing_extensions.Literal["provider"], typing_extensions.Literal["max_tokens"], typing_extensions.Literal["temperature"], typing_extensions.Literal["top_p"], typing_extensions.Literal["stop"], typing_extensions.Literal["presence_penalty"], typing_extensions.Literal["frequency_penalty"], typing_extensions.Literal["other"], typing_extensions.Literal["endpoint"], typing_extensions.Literal["prompt_template"], typing_extensions.Literal["chat_template"], ]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
-    
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["model"]) -> MetaOapg.properties.model: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["last_used"]) -> MetaOapg.properties.last_used: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> typing.Union[MetaOapg.properties.name, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["provider"]) -> typing.Union[MetaOapg.properties.provider, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["max_tokens"]) -> typing.Union[MetaOapg.properties.max_tokens, schemas.Unset]: ...
     
@@ -387,101 +340,62 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["frequency_penalty"]) -> typing.Union[MetaOapg.properties.frequency_penalty, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["other"]) -> typing.Union[MetaOapg.properties.other, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["display_name"]) -> typing.Union[MetaOapg.properties.display_name, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["endpoint"]) -> typing.Union[MetaOapg.properties.endpoint, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["prompt_template"]) -> typing.Union[MetaOapg.properties.prompt_template, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["chat_template"]) -> typing.Union[MetaOapg.properties.chat_template, schemas.Unset]: ...
     
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["endpoint"]) -> typing.Union[MetaOapg.properties.endpoint, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["project_id"]) -> typing.Union[MetaOapg.properties.project_id, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["project_name"]) -> typing.Union[MetaOapg.properties.project_name, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["feedback_stats"]) -> typing.Union[MetaOapg.properties.feedback_stats, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["num_datapoints"]) -> typing.Union[MetaOapg.properties.num_datapoints, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["experiment_id"]) -> typing.Union[MetaOapg.properties.experiment_id, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model", "id", "created_at", "updated_at", "last_used", "provider", "max_tokens", "temperature", "top_p", "stop", "presence_penalty", "frequency_penalty", "other", "display_name", "prompt_template", "chat_template", "endpoint", "project_id", "project_name", "feedback_stats", "num_datapoints", "experiment_id", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["model"], typing_extensions.Literal["type"], typing_extensions.Literal["description"], typing_extensions.Literal["name"], typing_extensions.Literal["provider"], typing_extensions.Literal["max_tokens"], typing_extensions.Literal["temperature"], typing_extensions.Literal["top_p"], typing_extensions.Literal["stop"], typing_extensions.Literal["presence_penalty"], typing_extensions.Literal["frequency_penalty"], typing_extensions.Literal["other"], typing_extensions.Literal["endpoint"], typing_extensions.Literal["prompt_template"], typing_extensions.Literal["chat_template"], ]):
         return super().get_item_oapg(name)
-    
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
-        updated_at: typing.Union[MetaOapg.properties.updated_at, str, datetime, ],
-        last_used: typing.Union[MetaOapg.properties.last_used, str, datetime, ],
-        created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, ],
         model: typing.Union[MetaOapg.properties.model, str, ],
-        id: typing.Union[MetaOapg.properties.id, str, ],
+        type: typing.Union[MetaOapg.properties.type, str, ],
+        description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
+        name: typing.Union[MetaOapg.properties.name, str, schemas.Unset] = schemas.unset,
         provider: typing.Union[MetaOapg.properties.provider, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         max_tokens: typing.Union[MetaOapg.properties.max_tokens, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         temperature: typing.Union[MetaOapg.properties.temperature, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         top_p: typing.Union[MetaOapg.properties.top_p, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         stop: typing.Union[MetaOapg.properties.stop, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         presence_penalty: typing.Union[MetaOapg.properties.presence_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         frequency_penalty: typing.Union[MetaOapg.properties.frequency_penalty, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
         other: typing.Union[MetaOapg.properties.other, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
-        display_name: typing.Union[MetaOapg.properties.display_name, str, schemas.Unset] = schemas.unset,
+        endpoint: typing.Union[MetaOapg.properties.endpoint, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         prompt_template: typing.Union[MetaOapg.properties.prompt_template, str, schemas.Unset] = schemas.unset,
         chat_template: typing.Union[MetaOapg.properties.chat_template, list, tuple, schemas.Unset] = schemas.unset,
-        endpoint: typing.Union[MetaOapg.properties.endpoint, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-        project_id: typing.Union[MetaOapg.properties.project_id, str, schemas.Unset] = schemas.unset,
-        project_name: typing.Union[MetaOapg.properties.project_name, str, schemas.Unset] = schemas.unset,
-        feedback_stats: typing.Union[MetaOapg.properties.feedback_stats, list, tuple, schemas.Unset] = schemas.unset,
-        num_datapoints: typing.Union[MetaOapg.properties.num_datapoints, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        experiment_id: typing.Union[MetaOapg.properties.experiment_id, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse':
+    ) -> 'TraceModelConfigRequest':
         return super().__new__(
             cls,
             *args,
-            updated_at=updated_at,
-            last_used=last_used,
-            created_at=created_at,
             model=model,
-            id=id,
+            type=type,
+            description=description,
+            name=name,
             provider=provider,
             max_tokens=max_tokens,
             temperature=temperature,
             top_p=top_p,
             stop=stop,
             presence_penalty=presence_penalty,
             frequency_penalty=frequency_penalty,
             other=other,
-            display_name=display_name,
+            endpoint=endpoint,
             prompt_template=prompt_template,
             chat_template=chat_template,
-            endpoint=endpoint,
-            project_id=project_id,
-            project_name=project_name,
-            feedback_stats=feedback_stats,
-            num_datapoints=num_datapoints,
-            experiment_id=experiment_id,
             _configuration=_configuration,
-            **kwargs,
         )
 
 from humanloop.model.chat_message import ChatMessage
 from humanloop.model.model_endpoints import ModelEndpoints
 from humanloop.model.model_providers import ModelProviders
-from humanloop.model.src_external_app_models_v4_model_configs_project_model_config_feedback_stats_response import SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse
```

### Comparing `humanloop-0.4.2/humanloop/model/tool_result_response.py` & `humanloop-0.4.3/humanloop/model/tool_result_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/tool_result_response.pyi` & `humanloop-0.4.3/humanloop/model/tool_result_response.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/update_experiment_request.py` & `humanloop-0.4.3/humanloop/model/update_experiment_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/update_experiment_request.pyi` & `humanloop-0.4.3/humanloop/model/update_experiment_request.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/update_project_request.py` & `humanloop-0.4.3/humanloop/model/update_project_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     """
 
 
     class MetaOapg:
         
         class properties:
             active_experiment_id = schemas.StrSchema
-            active_model_config_id = schemas.StrSchema
+            active_config_id = schemas.StrSchema
             
             
             class positive_labels(
                 schemas.ListSchema
             ):
             
             
@@ -60,64 +60,64 @@
                         _configuration=_configuration,
                     )
             
                 def __getitem__(self, i: int) -> 'PositiveLabel':
                     return super().__getitem__(i)
             __annotations__ = {
                 "active_experiment_id": active_experiment_id,
-                "active_model_config_id": active_model_config_id,
+                "active_config_id": active_config_id,
                 "positive_labels": positive_labels,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["active_experiment_id"]) -> MetaOapg.properties.active_experiment_id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["active_model_config_id"]) -> MetaOapg.properties.active_model_config_id: ...
+    def __getitem__(self, name: typing_extensions.Literal["active_config_id"]) -> MetaOapg.properties.active_config_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["positive_labels"]) -> MetaOapg.properties.positive_labels: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["active_experiment_id", "active_model_config_id", "positive_labels", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["active_experiment_id", "active_config_id", "positive_labels", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["active_experiment_id"]) -> typing.Union[MetaOapg.properties.active_experiment_id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["active_model_config_id"]) -> typing.Union[MetaOapg.properties.active_model_config_id, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["active_config_id"]) -> typing.Union[MetaOapg.properties.active_config_id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["positive_labels"]) -> typing.Union[MetaOapg.properties.positive_labels, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["active_experiment_id", "active_model_config_id", "positive_labels", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["active_experiment_id", "active_config_id", "positive_labels", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         active_experiment_id: typing.Union[MetaOapg.properties.active_experiment_id, str, schemas.Unset] = schemas.unset,
-        active_model_config_id: typing.Union[MetaOapg.properties.active_model_config_id, str, schemas.Unset] = schemas.unset,
+        active_config_id: typing.Union[MetaOapg.properties.active_config_id, str, schemas.Unset] = schemas.unset,
         positive_labels: typing.Union[MetaOapg.properties.positive_labels, list, tuple, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'UpdateProjectRequest':
         return super().__new__(
             cls,
             *args,
             active_experiment_id=active_experiment_id,
-            active_model_config_id=active_model_config_id,
+            active_config_id=active_config_id,
             positive_labels=positive_labels,
             _configuration=_configuration,
             **kwargs,
         )
 
 from humanloop.model.positive_label import PositiveLabel
```

### Comparing `humanloop-0.4.2/humanloop/model/update_project_request.pyi` & `humanloop-0.4.3/humanloop/model/update_project_request.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     """
 
 
     class MetaOapg:
         
         class properties:
             active_experiment_id = schemas.StrSchema
-            active_model_config_id = schemas.StrSchema
+            active_config_id = schemas.StrSchema
             
             
             class positive_labels(
                 schemas.ListSchema
             ):
             
             
@@ -60,64 +60,64 @@
                         _configuration=_configuration,
                     )
             
                 def __getitem__(self, i: int) -> 'PositiveLabel':
                     return super().__getitem__(i)
             __annotations__ = {
                 "active_experiment_id": active_experiment_id,
-                "active_model_config_id": active_model_config_id,
+                "active_config_id": active_config_id,
                 "positive_labels": positive_labels,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["active_experiment_id"]) -> MetaOapg.properties.active_experiment_id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["active_model_config_id"]) -> MetaOapg.properties.active_model_config_id: ...
+    def __getitem__(self, name: typing_extensions.Literal["active_config_id"]) -> MetaOapg.properties.active_config_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["positive_labels"]) -> MetaOapg.properties.positive_labels: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["active_experiment_id", "active_model_config_id", "positive_labels", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["active_experiment_id", "active_config_id", "positive_labels", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["active_experiment_id"]) -> typing.Union[MetaOapg.properties.active_experiment_id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["active_model_config_id"]) -> typing.Union[MetaOapg.properties.active_model_config_id, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["active_config_id"]) -> typing.Union[MetaOapg.properties.active_config_id, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["positive_labels"]) -> typing.Union[MetaOapg.properties.positive_labels, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["active_experiment_id", "active_model_config_id", "positive_labels", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["active_experiment_id", "active_config_id", "positive_labels", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         active_experiment_id: typing.Union[MetaOapg.properties.active_experiment_id, str, schemas.Unset] = schemas.unset,
-        active_model_config_id: typing.Union[MetaOapg.properties.active_model_config_id, str, schemas.Unset] = schemas.unset,
+        active_config_id: typing.Union[MetaOapg.properties.active_config_id, str, schemas.Unset] = schemas.unset,
         positive_labels: typing.Union[MetaOapg.properties.positive_labels, list, tuple, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'UpdateProjectRequest':
         return super().__new__(
             cls,
             *args,
             active_experiment_id=active_experiment_id,
-            active_model_config_id=active_model_config_id,
+            active_config_id=active_config_id,
             positive_labels=positive_labels,
             _configuration=_configuration,
             **kwargs,
         )
 
 from humanloop.model.positive_label import PositiveLabel
```

### Comparing `humanloop-0.4.2/humanloop/model/usage.py` & `humanloop-0.4.3/humanloop/model/usage.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/usage.pyi` & `humanloop-0.4.3/humanloop/model/usage.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/validation_error.py` & `humanloop-0.4.3/humanloop/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/model/validation_error.pyi` & `humanloop-0.4.3/humanloop/model/validation_error.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/models/__init__.py` & `humanloop-0.4.3/humanloop/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 # raise a RecursionError
 # to avoid this, import only the models that you directly need like:
 # from from humanloop.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
+from humanloop.model.agent_config_request import AgentConfigRequest
+from humanloop.model.agent_config_response import AgentConfigResponse
 from humanloop.model.base_metric_response import BaseMetricResponse
 from humanloop.model.categorical_feedback_label import CategoricalFeedbackLabel
 from humanloop.model.chat_data_response import ChatDataResponse
 from humanloop.model.chat_deployed_request import ChatDeployedRequest
 from humanloop.model.chat_experiment_request import ChatExperimentRequest
 from humanloop.model.chat_message import ChatMessage
 from humanloop.model.chat_model_config_request import ChatModelConfigRequest
@@ -22,62 +24,74 @@
 from humanloop.model.chat_response import ChatResponse
 from humanloop.model.chat_role import ChatRole
 from humanloop.model.completion_deployed_request import CompletionDeployedRequest
 from humanloop.model.completion_experiment_request import CompletionExperimentRequest
 from humanloop.model.completion_model_config_request import CompletionModelConfigRequest
 from humanloop.model.completion_request import CompletionRequest
 from humanloop.model.completion_response import CompletionResponse
+from humanloop.model.config_response import ConfigResponse
+from humanloop.model.config_type import ConfigType
 from humanloop.model.create_experiment_request import CreateExperimentRequest
 from humanloop.model.create_log_response import CreateLogResponse
 from humanloop.model.create_project_request import CreateProjectRequest
-from humanloop.model.create_session_request import CreateSessionRequest
+from humanloop.model.create_session_response import CreateSessionResponse
+from humanloop.model.create_trace_request import CreateTraceRequest
+from humanloop.model.create_trace_response import CreateTraceResponse
 from humanloop.model.data_response import DataResponse
-from humanloop.model.experiment_model_config_response import ExperimentModelConfigResponse
+from humanloop.model.experiment_config_response import ExperimentConfigResponse
 from humanloop.model.experiment_response import ExperimentResponse
 from humanloop.model.experiment_status import ExperimentStatus
 from humanloop.model.experiments_list_response import ExperimentsListResponse
 from humanloop.model.feedback import Feedback
 from humanloop.model.feedback_class import FeedbackClass
 from humanloop.model.feedback_label_request import FeedbackLabelRequest
 from humanloop.model.feedback_request import FeedbackRequest
 from humanloop.model.feedback_response import FeedbackResponse
 from humanloop.model.feedback_submit_request import FeedbackSubmitRequest
 from humanloop.model.feedback_submit_response import FeedbackSubmitResponse
 from humanloop.model.feedback_type import FeedbackType
 from humanloop.model.feedback_type_model import FeedbackTypeModel
 from humanloop.model.feedback_type_request import FeedbackTypeRequest
 from humanloop.model.feedback_types import FeedbackTypes
+from humanloop.model.generic_config_request import GenericConfigRequest
+from humanloop.model.generic_config_response import GenericConfigResponse
 from humanloop.model.get_model_config_response import GetModelConfigResponse
 from humanloop.model.http_validation_error import HTTPValidationError
 from humanloop.model.label_sentiment import LabelSentiment
 from humanloop.model.log_datapoint_request import LogDatapointRequest
+from humanloop.model.log_model_config_request import LogModelConfigRequest
 from humanloop.model.log_request import LogRequest
 from humanloop.model.log_response import LogResponse
 from humanloop.model.logs_log_response import LogsLogResponse
 from humanloop.model.model_config_chat_request import ModelConfigChatRequest
 from humanloop.model.model_config_completion_request import ModelConfigCompletionRequest
+from humanloop.model.model_config_response import ModelConfigResponse
+from humanloop.model.model_config_response2 import ModelConfigResponse2
 from humanloop.model.model_endpoints import ModelEndpoints
 from humanloop.model.model_providers import ModelProviders
 from humanloop.model.paginated_data_log_response import PaginatedDataLogResponse
 from humanloop.model.paginated_data_project_response import PaginatedDataProjectResponse
+from humanloop.model.paginated_data_session_response import PaginatedDataSessionResponse
 from humanloop.model.positive_label import PositiveLabel
+from humanloop.model.project_config_response import ProjectConfigResponse
 from humanloop.model.project_model_config_request import ProjectModelConfigRequest
+from humanloop.model.project_model_config_response import ProjectModelConfigResponse
 from humanloop.model.project_response import ProjectResponse
 from humanloop.model.project_sort_by import ProjectSortBy
 from humanloop.model.project_user_response import ProjectUserResponse
-from humanloop.model.projects_get_model_configs_response import ProjectsGetModelConfigsResponse
+from humanloop.model.projects_get_configs_response import ProjectsGetConfigsResponse
 from humanloop.model.projects_update_feedback_types_request import ProjectsUpdateFeedbackTypesRequest
 from humanloop.model.provider_api_keys import ProviderApiKeys
-from humanloop.model.session_app_response import SessionAppResponse
+from humanloop.model.session_project_response import SessionProjectResponse
 from humanloop.model.session_response import SessionResponse
 from humanloop.model.sort_order import SortOrder
-from humanloop.model.src_external_app_models_v3_model_configs_model_config_response import SrcExternalAppModelsV3ModelConfigsModelConfigResponse
 from humanloop.model.src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response import SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse
-from humanloop.model.src_external_app_models_v3_model_configs_project_model_config_response import SrcExternalAppModelsV3ModelConfigsProjectModelConfigResponse
-from humanloop.model.src_external_app_models_v4_model_configs_model_config_response import SrcExternalAppModelsV4ModelConfigsModelConfigResponse
-from humanloop.model.src_external_app_models_v4_model_configs_project_model_config_feedback_stats_response import SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse
-from humanloop.model.src_external_app_models_v4_model_configs_project_model_config_response import SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse
+from humanloop.model.src_external_app_models_v4_project_configs_project_model_config_feedback_stats_response import SrcExternalAppModelsV4ProjectConfigsProjectModelConfigFeedbackStatsResponse
+from humanloop.model.tool_config_request import ToolConfigRequest
+from humanloop.model.tool_config_response import ToolConfigResponse
 from humanloop.model.tool_result_response import ToolResultResponse
+from humanloop.model.trace_log_request import TraceLogRequest
+from humanloop.model.trace_model_config_request import TraceModelConfigRequest
 from humanloop.model.update_experiment_request import UpdateExperimentRequest
 from humanloop.model.update_project_request import UpdateProjectRequest
 from humanloop.model.usage import Usage
 from humanloop.model.validation_error import ValidationError
```

### Comparing `humanloop-0.4.2/humanloop/paths/__init__.py` & `humanloop-0.4.3/humanloop/paths/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,24 +14,20 @@
     CHATDEPLOYED = "/chat-deployed"
     CHATEXPERIMENT = "/chat-experiment"
     CHATMODELCONFIG = "/chat-model-config"
     LOGS = "/logs"
     FEEDBACK = "/feedback"
     PROJECTS = "/projects"
     PROJECTS_ID = "/projects/{id}"
-    PROJECTS_ID_MODELCONFIGS = "/projects/{id}/model-configs"
-    PROJECTS_ID_MODELCONFIG = "/projects/{id}/model-config"
-    PROJECTS_ID_ACTIVEMODELCONFIG = "/projects/{id}/active-model-config"
+    PROJECTS_ID_CONFIGS = "/projects/{id}/configs"
+    PROJECTS_ID_ACTIVECONFIG = "/projects/{id}/active-config"
     PROJECTS_ID_ACTIVEEXPERIMENT = "/projects/{id}/active-experiment"
     PROJECTS_ID_FEEDBACKTYPES = "/projects/{id}/feedback-types"
     PROJECTS_ID_EXPORT = "/projects/{id}/export"
-    APPS = "/apps"
-    APPS_ID = "/apps/{id}"
-    APPS_ID_SESSIONS = "/apps/{id}/sessions"
-    SESSIONS = "/sessions"
-    SESSIONS_ID = "/sessions/{id}"
-    SESSIONS_ID_EVENTS = "/sessions/{id}/events"
     MODELCONFIGS = "/model-configs"
     MODELCONFIGS_ID = "/model-configs/{id}"
     PROJECTS_PROJECT_ID_EXPERIMENTS = "/projects/{project_id}/experiments"
     EXPERIMENTS_EXPERIMENT_ID = "/experiments/{experiment_id}"
     EXPERIMENTS_EXPERIMENT_ID_MODELCONFIG = "/experiments/{experiment_id}/model-config"
+    SESSIONS = "/sessions"
+    SESSIONS_ID = "/sessions/{id}"
+    TRACES = "/traces"
```

### Comparing `humanloop-0.4.2/humanloop/paths/apps/get.py` & `humanloop-0.4.3/humanloop/paths/sessions/get.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,60 +27,78 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
+from humanloop.model.paginated_data_session_response import PaginatedDataSessionResponse as PaginatedDataSessionResponseSchema
 
+from humanloop.type.paginated_data_session_response import PaginatedDataSessionResponse
 from humanloop.type.http_validation_error import HTTPValidationError
 
 from . import path
 
 # Query params
-OrganizationIdSchema = schemas.StrSchema
+ProjectIdSchema = schemas.StrSchema
+PageSchema = schemas.IntSchema
+SizeSchema = schemas.IntSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
-        'organization_id': typing.Union[OrganizationIdSchema, str, ],
+        'project_id': typing.Union[ProjectIdSchema, str, ],
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
     'RequestOptionalQueryParams',
     {
+        'page': typing.Union[PageSchema, decimal.Decimal, int, ],
+        'size': typing.Union[SizeSchema, decimal.Decimal, int, ],
     },
     total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
 
 
-request_query_organization_id = api_client.QueryParameter(
-    name="organization_id",
+request_query_project_id = api_client.QueryParameter(
+    name="project_id",
     style=api_client.ParameterStyle.FORM,
-    schema=OrganizationIdSchema,
+    schema=ProjectIdSchema,
     required=True,
     explode=True,
 )
+request_query_page = api_client.QueryParameter(
+    name="page",
+    style=api_client.ParameterStyle.FORM,
+    schema=PageSchema,
+    explode=True,
+)
+request_query_size = api_client.QueryParameter(
+    name="size",
+    style=api_client.ParameterStyle.FORM,
+    schema=SizeSchema,
+    explode=True,
+)
 _auth = [
     'APIKeyHeader',
 ]
-SchemaFor200ResponseBodyApplicationJson = schemas.DictSchema
+SchemaFor200ResponseBodyApplicationJson = PaginatedDataSessionResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
+    body: PaginatedDataSessionResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
+    body: PaginatedDataSessionResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -117,20 +135,26 @@
 )
 
 
 class BaseApi(api_client.Api):
 
     def _list_mapped_args(
         self,
-        organization_id: str,
+        project_id: str,
+        page: typing.Optional[int] = None,
+        size: typing.Optional[int] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _query_params = {}
-        if organization_id is not None:
-            _query_params["organization_id"] = organization_id
+        if project_id is not None:
+            _query_params["project_id"] = project_id
+        if page is not None:
+            _query_params["page"] = page
+        if size is not None:
+            _query_params["size"] = size
         args.query = _query_params
         return args
 
     async def _alist_oapg(
         self,
             query_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
@@ -139,25 +163,27 @@
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        Get Apps
+        Get Sessions
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         used_path = path.value
     
         prefix_separator_iterator = None
         for parameter in (
-            request_query_organization_id,
+            request_query_project_id,
+            request_query_page,
+            request_query_size,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -232,25 +258,27 @@
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        Get Apps
+        Get Sessions
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         used_path = path.value
     
         prefix_separator_iterator = None
         for parameter in (
-            request_query_organization_id,
+            request_query_project_id,
+            request_query_page,
+            request_query_size,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
@@ -296,66 +324,82 @@
         return api_response
 
 class List(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     async def alist(
         self,
-        organization_id: str,
+        project_id: str,
+        page: typing.Optional[int] = None,
+        size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._list_mapped_args(
-            organization_id=organization_id,
+            project_id=project_id,
+            page=page,
+            size=size,
         )
         return await self._alist_oapg(
             query_params=args.query,
         )
     
     def list(
         self,
-        organization_id: str,
+        project_id: str,
+        page: typing.Optional[int] = None,
+        size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._list_mapped_args(
-            organization_id=organization_id,
+            project_id=project_id,
+            page=page,
+            size=size,
         )
         return self._list_oapg(
             query_params=args.query,
         )
 
 class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     async def aget(
         self,
-        organization_id: str,
+        project_id: str,
+        page: typing.Optional[int] = None,
+        size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._list_mapped_args(
-            organization_id=organization_id,
+            project_id=project_id,
+            page=page,
+            size=size,
         )
         return await self._alist_oapg(
             query_params=args.query,
         )
     
     def get(
         self,
-        organization_id: str,
+        project_id: str,
+        page: typing.Optional[int] = None,
+        size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._list_mapped_args(
-            organization_id=organization_id,
+            project_id=project_id,
+            page=page,
+            size=size,
         )
         return self._list_oapg(
             query_params=args.query,
         )
```

### Comparing `humanloop-0.4.2/humanloop/paths/apps/get.pyi` & `humanloop-0.4.3/humanloop/paths/projects_id_active_config/delete.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,56 +26,62 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
+from humanloop.model.project_response import ProjectResponse as ProjectResponseSchema
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
 
+from humanloop.type.project_response import ProjectResponse
 from humanloop.type.http_validation_error import HTTPValidationError
 
-# Query params
-OrganizationIdSchema = schemas.StrSchema
-RequestRequiredQueryParams = typing_extensions.TypedDict(
-    'RequestRequiredQueryParams',
+from . import path
+
+# Path params
+IdSchema = schemas.StrSchema
+RequestRequiredPathParams = typing_extensions.TypedDict(
+    'RequestRequiredPathParams',
     {
-        'organization_id': typing.Union[OrganizationIdSchema, str, ],
+        'id': typing.Union[IdSchema, str, ],
     }
 )
-RequestOptionalQueryParams = typing_extensions.TypedDict(
-    'RequestOptionalQueryParams',
+RequestOptionalPathParams = typing_extensions.TypedDict(
+    'RequestOptionalPathParams',
     {
     },
     total=False
 )
 
 
-class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
+class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
     pass
 
 
-request_query_organization_id = api_client.QueryParameter(
-    name="organization_id",
-    style=api_client.ParameterStyle.FORM,
-    schema=OrganizationIdSchema,
+request_path_id = api_client.PathParameter(
+    name="id",
+    style=api_client.ParameterStyle.SIMPLE,
+    schema=IdSchema,
     required=True,
-    explode=True,
 )
-SchemaFor200ResponseBodyApplicationJson = schemas.DictSchema
+_auth = [
+    'APIKeyHeader',
+]
+SchemaFor200ResponseBodyApplicationJson = ProjectResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
+    body: ProjectResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
+    body: ProjectResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -99,78 +105,81 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
+_status_code_to_response = {
+    '200': _response_for_200,
+    '422': _response_for_422,
+}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
-    def _list_mapped_args(
+    def _deactivate_active_config_mapped_args(
         self,
-        organization_id: str,
+        id: str,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
-        _query_params = {}
-        if organization_id is not None:
-            _query_params["organization_id"] = organization_id
-        args.query = _query_params
+        _path_params = {}
+        if id is not None:
+            _path_params["id"] = id
+        args.path = _path_params
         return args
 
-    async def _alist_oapg(
+    async def _adeactivate_active_config_oapg(
         self,
-            query_params: typing.Optional[dict] = {},
+            path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        Get Apps
+        Deactivate Config
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
-        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
+        self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
-        prefix_separator_iterator = None
+        _path_params = {}
         for parameter in (
-            request_query_organization_id,
+            request_path_id,
         ):
-            parameter_data = query_params.get(parameter.name, schemas.unset)
+            parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
-            if prefix_separator_iterator is None:
-                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
-            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
-            for serialized_value in serialized_data.values():
-                used_path += serialized_value
+            serialized_data = parameter.serialize(parameter_data)
+            _path_params.update(serialized_data)
+    
+        for k, v in _path_params.items():
+            used_path = used_path.replace('{%s}' % k, v)
     
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
     
         response = await self.api_client.async_call_api(
             resource_path=used_path,
-            method='get'.upper(),
+            method='delete'.upper(),
             headers=_headers,
             auth_settings=_auth,
-            prefix_separator_iterator=prefix_separator_iterator,
             timeout=timeout,
         )
         
         if stream:
             async def stream_iterator():
                 """
                 iterates over response.http_response.content and closes connection once iteration has finished
@@ -211,59 +220,58 @@
     
         # cleanup session / response
         response.http_response.close()
         await response.session.close()
     
         return api_response
 
-    def _list_oapg(
+    def _deactivate_active_config_oapg(
         self,
-            query_params: typing.Optional[dict] = {},
+            path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        Get Apps
+        Deactivate Config
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
-        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
+        self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
-        prefix_separator_iterator = None
+        _path_params = {}
         for parameter in (
-            request_query_organization_id,
+            request_path_id,
         ):
-            parameter_data = query_params.get(parameter.name, schemas.unset)
+            parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
-            if prefix_separator_iterator is None:
-                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
-            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
-            for serialized_value in serialized_data.values():
-                used_path += serialized_value
+            serialized_data = parameter.serialize(parameter_data)
+            _path_params.update(serialized_data)
+    
+        for k, v in _path_params.items():
+            used_path = used_path.replace('{%s}' % k, v)
     
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
     
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='get'.upper(),
+            method='delete'.upper(),
             headers=_headers,
             auth_settings=_auth,
-            prefix_separator_iterator=prefix_separator_iterator,
             timeout=timeout,
         )
     
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
         if response_for_status:
             api_response = response_for_status.deserialize(
                                                     response,
@@ -282,71 +290,71 @@
             )
     
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
     
         return api_response
 
-class List(BaseApi):
+class DeactivateActiveConfig(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    async def alist(
+    async def adeactivate_active_config(
         self,
-        organization_id: str,
+        id: str,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._list_mapped_args(
-            organization_id=organization_id,
+        args = self._deactivate_active_config_mapped_args(
+            id=id,
         )
-        return await self._alist_oapg(
-            query_params=args.query,
+        return await self._adeactivate_active_config_oapg(
+            path_params=args.path,
         )
     
-    def list(
+    def deactivate_active_config(
         self,
-        organization_id: str,
+        id: str,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._list_mapped_args(
-            organization_id=organization_id,
+        args = self._deactivate_active_config_mapped_args(
+            id=id,
         )
-        return self._list_oapg(
-            query_params=args.query,
+        return self._deactivate_active_config_oapg(
+            path_params=args.path,
         )
 
-class ApiForget(BaseApi):
+class ApiFordelete(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    async def aget(
+    async def adelete(
         self,
-        organization_id: str,
+        id: str,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._list_mapped_args(
-            organization_id=organization_id,
+        args = self._deactivate_active_config_mapped_args(
+            id=id,
         )
-        return await self._alist_oapg(
-            query_params=args.query,
+        return await self._adeactivate_active_config_oapg(
+            path_params=args.path,
         )
     
-    def get(
+    def delete(
         self,
-        organization_id: str,
+        id: str,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._list_mapped_args(
-            organization_id=organization_id,
+        args = self._deactivate_active_config_mapped_args(
+            id=id,
         )
-        return self._list_oapg(
-            query_params=args.query,
+        return self._deactivate_active_config_oapg(
+            path_params=args.path,
         )
```

### Comparing `humanloop-0.4.2/humanloop/paths/apps_id/get.py` & `humanloop-0.4.3/humanloop/paths/sessions_id/get.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
+from humanloop.model.session_response import SessionResponse as SessionResponseSchema
 
+from humanloop.type.session_response import SessionResponse
 from humanloop.type.http_validation_error import HTTPValidationError
 
 from . import path
 
 # Path params
 IdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
@@ -61,25 +63,25 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=IdSchema,
     required=True,
 )
 _auth = [
     'APIKeyHeader',
 ]
-SchemaFor200ResponseBodyApplicationJson = schemas.DictSchema
+SchemaFor200ResponseBodyApplicationJson = SessionResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
+    body: SessionResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
+    body: SessionResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -138,15 +140,15 @@
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        Get App
+        Get Session
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
@@ -230,15 +232,15 @@
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        Get App
+        Get Session
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
```

### Comparing `humanloop-0.4.2/humanloop/paths/apps_id/get.pyi` & `humanloop-0.4.3/humanloop/paths/sessions_id/get.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
+from humanloop.model.session_response import SessionResponse as SessionResponseSchema
 
+from humanloop.type.session_response import SessionResponse
 from humanloop.type.http_validation_error import HTTPValidationError
 
 # Path params
 IdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
@@ -56,25 +58,25 @@
 
 request_path_id = api_client.PathParameter(
     name="id",
     style=api_client.ParameterStyle.SIMPLE,
     schema=IdSchema,
     required=True,
 )
-SchemaFor200ResponseBodyApplicationJson = schemas.DictSchema
+SchemaFor200ResponseBodyApplicationJson = SessionResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
+    body: SessionResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
+    body: SessionResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -129,15 +131,15 @@
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        Get App
+        Get Session
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
@@ -221,15 +223,15 @@
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        Get App
+        Get Session
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
```

### Comparing `humanloop-0.4.2/humanloop/paths/apps_id_sessions/get.py` & `humanloop-0.4.3/humanloop/paths/projects_id_export/post.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
+from humanloop.model.paginated_data_log_response import PaginatedDataLogResponse as PaginatedDataLogResponseSchema
 
+from humanloop.type.paginated_data_log_response import PaginatedDataLogResponse
 from humanloop.type.http_validation_error import HTTPValidationError
 
 from . import path
 
 # Query params
 PageSchema = schemas.IntSchema
 SizeSchema = schemas.IntSchema
@@ -95,25 +97,25 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=IdSchema,
     required=True,
 )
 _auth = [
     'APIKeyHeader',
 ]
-SchemaFor200ResponseBodyApplicationJson = schemas.DictSchema
+SchemaFor200ResponseBodyApplicationJson = PaginatedDataLogResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
+    body: PaginatedDataLogResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
+    body: PaginatedDataLogResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -148,15 +150,15 @@
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
-    def _get_sessions_mapped_args(
+    def _export_datapoints_mapped_args(
         self,
         id: str,
         page: typing.Optional[int] = None,
         size: typing.Optional[int] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _query_params = {}
@@ -167,29 +169,29 @@
             _query_params["size"] = size
         if id is not None:
             _path_params["id"] = id
         args.query = _query_params
         args.path = _path_params
         return args
 
-    async def _aget_sessions_oapg(
+    async def _aexport_datapoints_oapg(
         self,
             query_params: typing.Optional[dict] = {},
             path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        Get App Sessions
+        Export Datapoints
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
@@ -225,15 +227,15 @@
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
     
         response = await self.api_client.async_call_api(
             resource_path=used_path,
-            method='get'.upper(),
+            method='post'.upper(),
             headers=_headers,
             auth_settings=_auth,
             prefix_separator_iterator=prefix_separator_iterator,
             timeout=timeout,
         )
         
         if stream:
@@ -277,28 +279,28 @@
     
         # cleanup session / response
         response.http_response.close()
         await response.session.close()
     
         return api_response
 
-    def _get_sessions_oapg(
+    def _export_datapoints_oapg(
         self,
             query_params: typing.Optional[dict] = {},
             path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        Get App Sessions
+        Export Datapoints
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
@@ -334,15 +336,15 @@
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
     
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='get'.upper(),
+            method='post'.upper(),
             headers=_headers,
             auth_settings=_auth,
             prefix_separator_iterator=prefix_separator_iterator,
             timeout=timeout,
         )
     
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
@@ -364,91 +366,91 @@
             )
     
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
     
         return api_response
 
-class GetSessions(BaseApi):
+class ExportDatapoints(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    async def aget_sessions(
+    async def aexport_datapoints(
         self,
         id: str,
         page: typing.Optional[int] = None,
         size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._get_sessions_mapped_args(
+        args = self._export_datapoints_mapped_args(
             id=id,
             page=page,
             size=size,
         )
-        return await self._aget_sessions_oapg(
+        return await self._aexport_datapoints_oapg(
             query_params=args.query,
             path_params=args.path,
         )
     
-    def get_sessions(
+    def export_datapoints(
         self,
         id: str,
         page: typing.Optional[int] = None,
         size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._get_sessions_mapped_args(
+        args = self._export_datapoints_mapped_args(
             id=id,
             page=page,
             size=size,
         )
-        return self._get_sessions_oapg(
+        return self._export_datapoints_oapg(
             query_params=args.query,
             path_params=args.path,
         )
 
-class ApiForget(BaseApi):
+class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    async def aget(
+    async def apost(
         self,
         id: str,
         page: typing.Optional[int] = None,
         size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._get_sessions_mapped_args(
+        args = self._export_datapoints_mapped_args(
             id=id,
             page=page,
             size=size,
         )
-        return await self._aget_sessions_oapg(
+        return await self._aexport_datapoints_oapg(
             query_params=args.query,
             path_params=args.path,
         )
     
-    def get(
+    def post(
         self,
         id: str,
         page: typing.Optional[int] = None,
         size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._get_sessions_mapped_args(
+        args = self._export_datapoints_mapped_args(
             id=id,
             page=page,
             size=size,
         )
-        return self._get_sessions_oapg(
+        return self._export_datapoints_oapg(
             query_params=args.query,
             path_params=args.path,
         )
```

### Comparing `humanloop-0.4.2/humanloop/paths/apps_id_sessions/get.pyi` & `humanloop-0.4.3/humanloop/paths/projects_id_export/post.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
+from humanloop.model.paginated_data_log_response import PaginatedDataLogResponse as PaginatedDataLogResponseSchema
 
+from humanloop.type.paginated_data_log_response import PaginatedDataLogResponse
 from humanloop.type.http_validation_error import HTTPValidationError
 
 # Query params
 PageSchema = schemas.IntSchema
 SizeSchema = schemas.IntSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
@@ -90,25 +92,25 @@
 
 request_path_id = api_client.PathParameter(
     name="id",
     style=api_client.ParameterStyle.SIMPLE,
     schema=IdSchema,
     required=True,
 )
-SchemaFor200ResponseBodyApplicationJson = schemas.DictSchema
+SchemaFor200ResponseBodyApplicationJson = PaginatedDataLogResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
+    body: PaginatedDataLogResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
+    body: PaginatedDataLogResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -139,15 +141,15 @@
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
-    def _get_sessions_mapped_args(
+    def _export_datapoints_mapped_args(
         self,
         id: str,
         page: typing.Optional[int] = None,
         size: typing.Optional[int] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _query_params = {}
@@ -158,29 +160,29 @@
             _query_params["size"] = size
         if id is not None:
             _path_params["id"] = id
         args.query = _query_params
         args.path = _path_params
         return args
 
-    async def _aget_sessions_oapg(
+    async def _aexport_datapoints_oapg(
         self,
             query_params: typing.Optional[dict] = {},
             path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        Get App Sessions
+        Export Datapoints
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
@@ -216,15 +218,15 @@
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
     
         response = await self.api_client.async_call_api(
             resource_path=used_path,
-            method='get'.upper(),
+            method='post'.upper(),
             headers=_headers,
             auth_settings=_auth,
             prefix_separator_iterator=prefix_separator_iterator,
             timeout=timeout,
         )
         
         if stream:
@@ -268,28 +270,28 @@
     
         # cleanup session / response
         response.http_response.close()
         await response.session.close()
     
         return api_response
 
-    def _get_sessions_oapg(
+    def _export_datapoints_oapg(
         self,
             query_params: typing.Optional[dict] = {},
             path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        Get App Sessions
+        Export Datapoints
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
@@ -325,15 +327,15 @@
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
     
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='get'.upper(),
+            method='post'.upper(),
             headers=_headers,
             auth_settings=_auth,
             prefix_separator_iterator=prefix_separator_iterator,
             timeout=timeout,
         )
     
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
@@ -355,91 +357,91 @@
             )
     
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
     
         return api_response
 
-class GetSessions(BaseApi):
+class ExportDatapoints(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    async def aget_sessions(
+    async def aexport_datapoints(
         self,
         id: str,
         page: typing.Optional[int] = None,
         size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._get_sessions_mapped_args(
+        args = self._export_datapoints_mapped_args(
             id=id,
             page=page,
             size=size,
         )
-        return await self._aget_sessions_oapg(
+        return await self._aexport_datapoints_oapg(
             query_params=args.query,
             path_params=args.path,
         )
     
-    def get_sessions(
+    def export_datapoints(
         self,
         id: str,
         page: typing.Optional[int] = None,
         size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._get_sessions_mapped_args(
+        args = self._export_datapoints_mapped_args(
             id=id,
             page=page,
             size=size,
         )
-        return self._get_sessions_oapg(
+        return self._export_datapoints_oapg(
             query_params=args.query,
             path_params=args.path,
         )
 
-class ApiForget(BaseApi):
+class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    async def aget(
+    async def apost(
         self,
         id: str,
         page: typing.Optional[int] = None,
         size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._get_sessions_mapped_args(
+        args = self._export_datapoints_mapped_args(
             id=id,
             page=page,
             size=size,
         )
-        return await self._aget_sessions_oapg(
+        return await self._aexport_datapoints_oapg(
             query_params=args.query,
             path_params=args.path,
         )
     
-    def get(
+    def post(
         self,
         id: str,
         page: typing.Optional[int] = None,
         size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._get_sessions_mapped_args(
+        args = self._export_datapoints_mapped_args(
             id=id,
             page=page,
             size=size,
         )
-        return self._get_sessions_oapg(
+        return self._export_datapoints_oapg(
             query_params=args.query,
             path_params=args.path,
         )
```

### Comparing `humanloop-0.4.2/humanloop/paths/chat/post.py` & `humanloop-0.4.3/humanloop/paths/chat/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/chat/post.pyi` & `humanloop-0.4.3/humanloop/paths/chat/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/chat_deployed/post.py` & `humanloop-0.4.3/humanloop/paths/chat_deployed/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/chat_deployed/post.pyi` & `humanloop-0.4.3/humanloop/paths/chat_deployed/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/chat_experiment/post.py` & `humanloop-0.4.3/humanloop/paths/chat_experiment/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/chat_experiment/post.pyi` & `humanloop-0.4.3/humanloop/paths/chat_experiment/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/chat_model_config/post.py` & `humanloop-0.4.3/humanloop/paths/chat_model_config/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/chat_model_config/post.pyi` & `humanloop-0.4.3/humanloop/paths/chat_model_config/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/completion/post.py` & `humanloop-0.4.3/humanloop/paths/completion/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/completion/post.pyi` & `humanloop-0.4.3/humanloop/paths/completion/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/completion_deployed/post.py` & `humanloop-0.4.3/humanloop/paths/completion_deployed/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/completion_deployed/post.pyi` & `humanloop-0.4.3/humanloop/paths/completion_deployed/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/completion_experiment/post.py` & `humanloop-0.4.3/humanloop/paths/completion_experiment/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/completion_experiment/post.pyi` & `humanloop-0.4.3/humanloop/paths/completion_experiment/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/completion_model_config/post.py` & `humanloop-0.4.3/humanloop/paths/completion_model_config/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/completion_model_config/post.pyi` & `humanloop-0.4.3/humanloop/paths/completion_model_config/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/experiments_experiment_id/delete.py` & `humanloop-0.4.3/humanloop/paths/experiments_experiment_id/delete.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/experiments_experiment_id/delete.pyi` & `humanloop-0.4.3/humanloop/paths/experiments_experiment_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/experiments_experiment_id/patch.py` & `humanloop-0.4.3/humanloop/paths/experiments_experiment_id/patch.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/experiments_experiment_id/patch.pyi` & `humanloop-0.4.3/humanloop/paths/experiments_experiment_id/patch.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/experiments_experiment_id_model_config/get.py` & `humanloop-0.4.3/humanloop/paths/experiments_experiment_id_model_config/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/experiments_experiment_id_model_config/get.pyi` & `humanloop-0.4.3/humanloop/paths/experiments_experiment_id_model_config/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/feedback/post.py` & `humanloop-0.4.3/humanloop/paths/feedback/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/feedback/post.pyi` & `humanloop-0.4.3/humanloop/paths/feedback/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/logs/post.py` & `humanloop-0.4.3/humanloop/paths/logs/post.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -26,46 +26,45 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
+from humanloop.model.agent_config_request import AgentConfigRequest as AgentConfigRequestSchema
+from humanloop.model.tool_config_request import ToolConfigRequest as ToolConfigRequestSchema
 from humanloop.model.log_datapoint_request import LogDatapointRequest as LogDatapointRequestSchema
-from humanloop.model.model_config_chat_request import ModelConfigChatRequest as ModelConfigChatRequestSchema
-from humanloop.model.model_config_completion_request import ModelConfigCompletionRequest as ModelConfigCompletionRequestSchema
+from humanloop.model.trace_model_config_request import TraceModelConfigRequest as TraceModelConfigRequestSchema
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
 from humanloop.model.feedback import Feedback as FeedbackSchema
 from humanloop.model.logs_log_response import LogsLogResponse as LogsLogResponseSchema
+from humanloop.model.generic_config_request import GenericConfigRequest as GenericConfigRequestSchema
 from humanloop.model.chat_message import ChatMessage as ChatMessageSchema
 
 from humanloop.type.feedback import Feedback
 from humanloop.type.chat_message import ChatMessage
-from humanloop.type.model_config_completion_request import ModelConfigCompletionRequest
+from humanloop.type.agent_config_request import AgentConfigRequest
+from humanloop.type.generic_config_request import GenericConfigRequest
+from humanloop.type.tool_config_request import ToolConfigRequest
 from humanloop.type.logs_log_response import LogsLogResponse
+from humanloop.type.trace_model_config_request import TraceModelConfigRequest
 from humanloop.type.log_datapoint_request import LogDatapointRequest
 from humanloop.type.http_validation_error import HTTPValidationError
-from humanloop.type.model_config_chat_request import ModelConfigChatRequest
-
-from . import path
 
 # body param
 SchemaForRequestBodyApplicationJson = LogDatapointRequestSchema
 
 
 request_body_log_datapoint_request = api_client.RequestBody(
     content={
         'application/json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
-_auth = [
-    'APIKeyHeader',
-]
 SchemaFor200ResponseBodyApplicationJson = LogsLogResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     body: LogsLogResponse
 
@@ -100,18 +99,14 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '422': _response_for_422,
-}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
@@ -122,18 +117,20 @@
         session_id: typing.Optional[str] = None,
         parent_id: typing.Optional[str] = None,
         trial_id: typing.Optional[str] = None,
         inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         messages: typing.Optional[typing.List[ChatMessage]] = None,
         output: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
-        model_config: typing.Optional[typing.Union[ModelConfigCompletionRequest, ModelConfigChatRequest]] = None,
+        config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
         metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         feedback: typing.Optional[typing.Union[Feedback, typing.List[Feedback]]] = None,
         created_at: typing.Optional[datetime] = None,
+        error: typing.Optional[str] = None,
+        duration: typing.Optional[typing.Union[int, float]] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _body = {}
         if project is not None:
             _body["project"] = project
         if session_id is not None:
             _body["session_id"] = session_id
@@ -145,22 +142,26 @@
             _body["inputs"] = inputs
         if messages is not None:
             _body["messages"] = messages
         if output is not None:
             _body["output"] = output
         if source is not None:
             _body["source"] = source
-        if model_config is not None:
-            _body["model_config"] = model_config
+        if config is not None:
+            _body["config"] = config
         if metadata is not None:
             _body["metadata"] = metadata
         if feedback is not None:
             _body["feedback"] = feedback
         if created_at is not None:
             _body["created_at"] = created_at
+        if error is not None:
+            _body["error"] = error
+        if duration is not None:
+            _body["duration"] = duration
         args.body = body if body is not None else _body
         return args
 
     async def _alog_oapg(
         self,
         body: typing.Any = None,
         skip_deserialization: bool = True,
@@ -335,18 +336,20 @@
         session_id: typing.Optional[str] = None,
         parent_id: typing.Optional[str] = None,
         trial_id: typing.Optional[str] = None,
         inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         messages: typing.Optional[typing.List[ChatMessage]] = None,
         output: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
-        model_config: typing.Optional[typing.Union[ModelConfigCompletionRequest, ModelConfigChatRequest]] = None,
+        config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
         metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         feedback: typing.Optional[typing.Union[Feedback, typing.List[Feedback]]] = None,
         created_at: typing.Optional[datetime] = None,
+        error: typing.Optional[str] = None,
+        duration: typing.Optional[typing.Union[int, float]] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._log_mapped_args(
             body=body,
@@ -354,18 +357,20 @@
             session_id=session_id,
             parent_id=parent_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             output=output,
             source=source,
-            model_config=model_config,
+            config=config,
             metadata=metadata,
             feedback=feedback,
             created_at=created_at,
+            error=error,
+            duration=duration,
         )
         return await self._alog_oapg(
             body=args.body,
         )
     
     def log(
         self,
@@ -374,36 +379,40 @@
         session_id: typing.Optional[str] = None,
         parent_id: typing.Optional[str] = None,
         trial_id: typing.Optional[str] = None,
         inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         messages: typing.Optional[typing.List[ChatMessage]] = None,
         output: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
-        model_config: typing.Optional[typing.Union[ModelConfigCompletionRequest, ModelConfigChatRequest]] = None,
+        config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
         metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         feedback: typing.Optional[typing.Union[Feedback, typing.List[Feedback]]] = None,
         created_at: typing.Optional[datetime] = None,
+        error: typing.Optional[str] = None,
+        duration: typing.Optional[typing.Union[int, float]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._log_mapped_args(
             body=body,
             project=project,
             session_id=session_id,
             parent_id=parent_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             output=output,
             source=source,
-            model_config=model_config,
+            config=config,
             metadata=metadata,
             feedback=feedback,
             created_at=created_at,
+            error=error,
+            duration=duration,
         )
         return self._log_oapg(
             body=args.body,
         )
 
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
@@ -415,18 +424,20 @@
         session_id: typing.Optional[str] = None,
         parent_id: typing.Optional[str] = None,
         trial_id: typing.Optional[str] = None,
         inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         messages: typing.Optional[typing.List[ChatMessage]] = None,
         output: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
-        model_config: typing.Optional[typing.Union[ModelConfigCompletionRequest, ModelConfigChatRequest]] = None,
+        config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
         metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         feedback: typing.Optional[typing.Union[Feedback, typing.List[Feedback]]] = None,
         created_at: typing.Optional[datetime] = None,
+        error: typing.Optional[str] = None,
+        duration: typing.Optional[typing.Union[int, float]] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._log_mapped_args(
             body=body,
@@ -434,18 +445,20 @@
             session_id=session_id,
             parent_id=parent_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             output=output,
             source=source,
-            model_config=model_config,
+            config=config,
             metadata=metadata,
             feedback=feedback,
             created_at=created_at,
+            error=error,
+            duration=duration,
         )
         return await self._alog_oapg(
             body=args.body,
         )
     
     def post(
         self,
@@ -454,34 +467,38 @@
         session_id: typing.Optional[str] = None,
         parent_id: typing.Optional[str] = None,
         trial_id: typing.Optional[str] = None,
         inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         messages: typing.Optional[typing.List[ChatMessage]] = None,
         output: typing.Optional[str] = None,
         source: typing.Optional[str] = None,
-        model_config: typing.Optional[typing.Union[ModelConfigCompletionRequest, ModelConfigChatRequest]] = None,
+        config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
         metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
         feedback: typing.Optional[typing.Union[Feedback, typing.List[Feedback]]] = None,
         created_at: typing.Optional[datetime] = None,
+        error: typing.Optional[str] = None,
+        duration: typing.Optional[typing.Union[int, float]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._log_mapped_args(
             body=body,
             project=project,
             session_id=session_id,
             parent_id=parent_id,
             trial_id=trial_id,
             inputs=inputs,
             messages=messages,
             output=output,
             source=source,
-            model_config=model_config,
+            config=config,
             metadata=metadata,
             feedback=feedback,
             created_at=created_at,
+            error=error,
+            duration=duration,
         )
         return self._log_oapg(
             body=args.body,
         )
```

### Comparing `humanloop-0.4.2/humanloop/paths/logs/post.pyi` & `humanloop-0.4.3/humanloop/paths/model_configs/post.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,52 +26,55 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
-from humanloop.model.log_datapoint_request import LogDatapointRequest as LogDatapointRequestSchema
-from humanloop.model.model_config_chat_request import ModelConfigChatRequest as ModelConfigChatRequestSchema
-from humanloop.model.model_config_completion_request import ModelConfigCompletionRequest as ModelConfigCompletionRequestSchema
+from humanloop.model.model_providers import ModelProviders as ModelProvidersSchema
+from humanloop.model.project_model_config_request import ProjectModelConfigRequest as ProjectModelConfigRequestSchema
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
-from humanloop.model.feedback import Feedback as FeedbackSchema
-from humanloop.model.logs_log_response import LogsLogResponse as LogsLogResponseSchema
+from humanloop.model.model_endpoints import ModelEndpoints as ModelEndpointsSchema
+from humanloop.model.project_model_config_response import ProjectModelConfigResponse as ProjectModelConfigResponseSchema
 from humanloop.model.chat_message import ChatMessage as ChatMessageSchema
 
-from humanloop.type.feedback import Feedback
 from humanloop.type.chat_message import ChatMessage
-from humanloop.type.model_config_completion_request import ModelConfigCompletionRequest
-from humanloop.type.logs_log_response import LogsLogResponse
-from humanloop.type.log_datapoint_request import LogDatapointRequest
+from humanloop.type.project_model_config_request import ProjectModelConfigRequest
+from humanloop.type.project_model_config_response import ProjectModelConfigResponse
+from humanloop.type.model_providers import ModelProviders
 from humanloop.type.http_validation_error import HTTPValidationError
-from humanloop.type.model_config_chat_request import ModelConfigChatRequest
+from humanloop.type.model_endpoints import ModelEndpoints
+
+from . import path
 
 # body param
-SchemaForRequestBodyApplicationJson = LogDatapointRequestSchema
+SchemaForRequestBodyApplicationJson = ProjectModelConfigRequestSchema
 
 
-request_body_log_datapoint_request = api_client.RequestBody(
+request_body_project_model_config_request = api_client.RequestBody(
     content={
         'application/json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
-SchemaFor200ResponseBodyApplicationJson = LogsLogResponseSchema
+_auth = [
+    'APIKeyHeader',
+]
+SchemaFor200ResponseBodyApplicationJson = ProjectModelConfigResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: LogsLogResponse
+    body: ProjectModelConfigResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: LogsLogResponse
+    body: ProjectModelConfigResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -95,81 +98,93 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
+_status_code_to_response = {
+    '200': _response_for_200,
+    '422': _response_for_422,
+}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
-    def _log_mapped_args(
+    def _register_mapped_args(
         self,
-        body: typing.Optional[LogDatapointRequest] = None,
-        project: typing.Optional[str] = None,
-        session_id: typing.Optional[str] = None,
-        parent_id: typing.Optional[str] = None,
-        trial_id: typing.Optional[str] = None,
-        inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
-        messages: typing.Optional[typing.List[ChatMessage]] = None,
-        output: typing.Optional[str] = None,
-        source: typing.Optional[str] = None,
-        model_config: typing.Optional[typing.Union[ModelConfigCompletionRequest, ModelConfigChatRequest]] = None,
-        metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
-        feedback: typing.Optional[typing.Union[Feedback, typing.List[Feedback]]] = None,
-        created_at: typing.Optional[datetime] = None,
+        model: str,
+        project: str,
+        provider: typing.Optional[ModelProviders] = None,
+        endpoint: typing.Optional[ModelEndpoints] = None,
+        prompt_template: typing.Optional[str] = None,
+        chat_template: typing.Optional[typing.List[ChatMessage]] = None,
+        temperature: typing.Optional[typing.Union[int, float]] = None,
+        max_tokens: typing.Optional[int] = None,
+        top_p: typing.Optional[typing.Union[int, float]] = None,
+        stop: typing.Optional[typing.Union[str, typing.List[str]]] = None,
+        presence_penalty: typing.Optional[typing.Union[int, float]] = None,
+        frequency_penalty: typing.Optional[typing.Union[int, float]] = None,
+        other: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
+        name: typing.Optional[str] = None,
+        experiment: typing.Optional[str] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _body = {}
+        if provider is not None:
+            _body["provider"] = provider
+        if endpoint is not None:
+            _body["endpoint"] = endpoint
+        if model is not None:
+            _body["model"] = model
+        if prompt_template is not None:
+            _body["prompt_template"] = prompt_template
+        if chat_template is not None:
+            _body["chat_template"] = chat_template
+        if temperature is not None:
+            _body["temperature"] = temperature
+        if max_tokens is not None:
+            _body["max_tokens"] = max_tokens
+        if top_p is not None:
+            _body["top_p"] = top_p
+        if stop is not None:
+            _body["stop"] = stop
+        if presence_penalty is not None:
+            _body["presence_penalty"] = presence_penalty
+        if frequency_penalty is not None:
+            _body["frequency_penalty"] = frequency_penalty
+        if other is not None:
+            _body["other"] = other
         if project is not None:
             _body["project"] = project
-        if session_id is not None:
-            _body["session_id"] = session_id
-        if parent_id is not None:
-            _body["parent_id"] = parent_id
-        if trial_id is not None:
-            _body["trial_id"] = trial_id
-        if inputs is not None:
-            _body["inputs"] = inputs
-        if messages is not None:
-            _body["messages"] = messages
-        if output is not None:
-            _body["output"] = output
-        if source is not None:
-            _body["source"] = source
-        if model_config is not None:
-            _body["model_config"] = model_config
-        if metadata is not None:
-            _body["metadata"] = metadata
-        if feedback is not None:
-            _body["feedback"] = feedback
-        if created_at is not None:
-            _body["created_at"] = created_at
-        args.body = body if body is not None else _body
+        if name is not None:
+            _body["name"] = name
+        if experiment is not None:
+            _body["experiment"] = experiment
+        args.body = _body
         return args
 
-    async def _alog_oapg(
+    async def _aregister_oapg(
         self,
         body: typing.Any = None,
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         content_type: str = 'application/json',
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        Log
+        Register Model Config
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
     
         _headers = HTTPHeaderDict()
@@ -179,15 +194,15 @@
                 _headers.add('Accept', accept_content_type)
     
         if body is schemas.unset:
             raise exceptions.ApiValueError(
                 'The required body parameter has an invalid value of: unset. Set a valid value instead')
         _fields = None
         _body = None
-        serialized_data = request_body_log_datapoint_request.serialize(body, content_type)
+        serialized_data = request_body_project_model_config_request.serialize(body, content_type)
         _headers.add('Content-Type', content_type)
         if 'fields' in serialized_data:
             _fields = serialized_data['fields']
         elif 'body' in serialized_data:
             _body = serialized_data['body']    
         response = await self.api_client.async_call_api(
             resource_path=used_path,
@@ -241,28 +256,28 @@
     
         # cleanup session / response
         response.http_response.close()
         await response.session.close()
     
         return api_response
 
-    def _log_oapg(
+    def _register_oapg(
         self,
         body: typing.Any = None,
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         content_type: str = 'application/json',
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        Log
+        Register Model Config
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
     
         _headers = HTTPHeaderDict()
@@ -272,15 +287,15 @@
                 _headers.add('Accept', accept_content_type)
     
         if body is schemas.unset:
             raise exceptions.ApiValueError(
                 'The required body parameter has an invalid value of: unset. Set a valid value instead')
         _fields = None
         _body = None
-        serialized_data = request_body_log_datapoint_request.serialize(body, content_type)
+        serialized_data = request_body_project_model_config_request.serialize(body, content_type)
         _headers.add('Content-Type', content_type)
         if 'fields' in serialized_data:
             _fields = serialized_data['fields']
         elif 'body' in serialized_data:
             _body = serialized_data['body']    
         response = self.api_client.call_api(
             resource_path=used_path,
@@ -312,167 +327,183 @@
             )
     
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
     
         return api_response
 
-class Log(BaseApi):
+class Register(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    async def alog(
+    async def aregister(
         self,
-        body: typing.Optional[LogDatapointRequest] = None,
-        project: typing.Optional[str] = None,
-        session_id: typing.Optional[str] = None,
-        parent_id: typing.Optional[str] = None,
-        trial_id: typing.Optional[str] = None,
-        inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
-        messages: typing.Optional[typing.List[ChatMessage]] = None,
-        output: typing.Optional[str] = None,
-        source: typing.Optional[str] = None,
-        model_config: typing.Optional[typing.Union[ModelConfigCompletionRequest, ModelConfigChatRequest]] = None,
-        metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
-        feedback: typing.Optional[typing.Union[Feedback, typing.List[Feedback]]] = None,
-        created_at: typing.Optional[datetime] = None,
+        model: str,
+        project: str,
+        provider: typing.Optional[ModelProviders] = None,
+        endpoint: typing.Optional[ModelEndpoints] = None,
+        prompt_template: typing.Optional[str] = None,
+        chat_template: typing.Optional[typing.List[ChatMessage]] = None,
+        temperature: typing.Optional[typing.Union[int, float]] = None,
+        max_tokens: typing.Optional[int] = None,
+        top_p: typing.Optional[typing.Union[int, float]] = None,
+        stop: typing.Optional[typing.Union[str, typing.List[str]]] = None,
+        presence_penalty: typing.Optional[typing.Union[int, float]] = None,
+        frequency_penalty: typing.Optional[typing.Union[int, float]] = None,
+        other: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
+        name: typing.Optional[str] = None,
+        experiment: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._log_mapped_args(
-            body=body,
+        args = self._register_mapped_args(
+            model=model,
             project=project,
-            session_id=session_id,
-            parent_id=parent_id,
-            trial_id=trial_id,
-            inputs=inputs,
-            messages=messages,
-            output=output,
-            source=source,
-            model_config=model_config,
-            metadata=metadata,
-            feedback=feedback,
-            created_at=created_at,
+            provider=provider,
+            endpoint=endpoint,
+            prompt_template=prompt_template,
+            chat_template=chat_template,
+            temperature=temperature,
+            max_tokens=max_tokens,
+            top_p=top_p,
+            stop=stop,
+            presence_penalty=presence_penalty,
+            frequency_penalty=frequency_penalty,
+            other=other,
+            name=name,
+            experiment=experiment,
         )
-        return await self._alog_oapg(
+        return await self._aregister_oapg(
             body=args.body,
         )
     
-    def log(
+    def register(
         self,
-        body: typing.Optional[LogDatapointRequest] = None,
-        project: typing.Optional[str] = None,
-        session_id: typing.Optional[str] = None,
-        parent_id: typing.Optional[str] = None,
-        trial_id: typing.Optional[str] = None,
-        inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
-        messages: typing.Optional[typing.List[ChatMessage]] = None,
-        output: typing.Optional[str] = None,
-        source: typing.Optional[str] = None,
-        model_config: typing.Optional[typing.Union[ModelConfigCompletionRequest, ModelConfigChatRequest]] = None,
-        metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
-        feedback: typing.Optional[typing.Union[Feedback, typing.List[Feedback]]] = None,
-        created_at: typing.Optional[datetime] = None,
+        model: str,
+        project: str,
+        provider: typing.Optional[ModelProviders] = None,
+        endpoint: typing.Optional[ModelEndpoints] = None,
+        prompt_template: typing.Optional[str] = None,
+        chat_template: typing.Optional[typing.List[ChatMessage]] = None,
+        temperature: typing.Optional[typing.Union[int, float]] = None,
+        max_tokens: typing.Optional[int] = None,
+        top_p: typing.Optional[typing.Union[int, float]] = None,
+        stop: typing.Optional[typing.Union[str, typing.List[str]]] = None,
+        presence_penalty: typing.Optional[typing.Union[int, float]] = None,
+        frequency_penalty: typing.Optional[typing.Union[int, float]] = None,
+        other: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
+        name: typing.Optional[str] = None,
+        experiment: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._log_mapped_args(
-            body=body,
+        args = self._register_mapped_args(
+            model=model,
             project=project,
-            session_id=session_id,
-            parent_id=parent_id,
-            trial_id=trial_id,
-            inputs=inputs,
-            messages=messages,
-            output=output,
-            source=source,
-            model_config=model_config,
-            metadata=metadata,
-            feedback=feedback,
-            created_at=created_at,
+            provider=provider,
+            endpoint=endpoint,
+            prompt_template=prompt_template,
+            chat_template=chat_template,
+            temperature=temperature,
+            max_tokens=max_tokens,
+            top_p=top_p,
+            stop=stop,
+            presence_penalty=presence_penalty,
+            frequency_penalty=frequency_penalty,
+            other=other,
+            name=name,
+            experiment=experiment,
         )
-        return self._log_oapg(
+        return self._register_oapg(
             body=args.body,
         )
 
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     async def apost(
         self,
-        body: typing.Optional[LogDatapointRequest] = None,
-        project: typing.Optional[str] = None,
-        session_id: typing.Optional[str] = None,
-        parent_id: typing.Optional[str] = None,
-        trial_id: typing.Optional[str] = None,
-        inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
-        messages: typing.Optional[typing.List[ChatMessage]] = None,
-        output: typing.Optional[str] = None,
-        source: typing.Optional[str] = None,
-        model_config: typing.Optional[typing.Union[ModelConfigCompletionRequest, ModelConfigChatRequest]] = None,
-        metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
-        feedback: typing.Optional[typing.Union[Feedback, typing.List[Feedback]]] = None,
-        created_at: typing.Optional[datetime] = None,
+        model: str,
+        project: str,
+        provider: typing.Optional[ModelProviders] = None,
+        endpoint: typing.Optional[ModelEndpoints] = None,
+        prompt_template: typing.Optional[str] = None,
+        chat_template: typing.Optional[typing.List[ChatMessage]] = None,
+        temperature: typing.Optional[typing.Union[int, float]] = None,
+        max_tokens: typing.Optional[int] = None,
+        top_p: typing.Optional[typing.Union[int, float]] = None,
+        stop: typing.Optional[typing.Union[str, typing.List[str]]] = None,
+        presence_penalty: typing.Optional[typing.Union[int, float]] = None,
+        frequency_penalty: typing.Optional[typing.Union[int, float]] = None,
+        other: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
+        name: typing.Optional[str] = None,
+        experiment: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._log_mapped_args(
-            body=body,
+        args = self._register_mapped_args(
+            model=model,
             project=project,
-            session_id=session_id,
-            parent_id=parent_id,
-            trial_id=trial_id,
-            inputs=inputs,
-            messages=messages,
-            output=output,
-            source=source,
-            model_config=model_config,
-            metadata=metadata,
-            feedback=feedback,
-            created_at=created_at,
+            provider=provider,
+            endpoint=endpoint,
+            prompt_template=prompt_template,
+            chat_template=chat_template,
+            temperature=temperature,
+            max_tokens=max_tokens,
+            top_p=top_p,
+            stop=stop,
+            presence_penalty=presence_penalty,
+            frequency_penalty=frequency_penalty,
+            other=other,
+            name=name,
+            experiment=experiment,
         )
-        return await self._alog_oapg(
+        return await self._aregister_oapg(
             body=args.body,
         )
     
     def post(
         self,
-        body: typing.Optional[LogDatapointRequest] = None,
-        project: typing.Optional[str] = None,
-        session_id: typing.Optional[str] = None,
-        parent_id: typing.Optional[str] = None,
-        trial_id: typing.Optional[str] = None,
-        inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
-        messages: typing.Optional[typing.List[ChatMessage]] = None,
-        output: typing.Optional[str] = None,
-        source: typing.Optional[str] = None,
-        model_config: typing.Optional[typing.Union[ModelConfigCompletionRequest, ModelConfigChatRequest]] = None,
-        metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
-        feedback: typing.Optional[typing.Union[Feedback, typing.List[Feedback]]] = None,
-        created_at: typing.Optional[datetime] = None,
+        model: str,
+        project: str,
+        provider: typing.Optional[ModelProviders] = None,
+        endpoint: typing.Optional[ModelEndpoints] = None,
+        prompt_template: typing.Optional[str] = None,
+        chat_template: typing.Optional[typing.List[ChatMessage]] = None,
+        temperature: typing.Optional[typing.Union[int, float]] = None,
+        max_tokens: typing.Optional[int] = None,
+        top_p: typing.Optional[typing.Union[int, float]] = None,
+        stop: typing.Optional[typing.Union[str, typing.List[str]]] = None,
+        presence_penalty: typing.Optional[typing.Union[int, float]] = None,
+        frequency_penalty: typing.Optional[typing.Union[int, float]] = None,
+        other: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
+        name: typing.Optional[str] = None,
+        experiment: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._log_mapped_args(
-            body=body,
+        args = self._register_mapped_args(
+            model=model,
             project=project,
-            session_id=session_id,
-            parent_id=parent_id,
-            trial_id=trial_id,
-            inputs=inputs,
-            messages=messages,
-            output=output,
-            source=source,
-            model_config=model_config,
-            metadata=metadata,
-            feedback=feedback,
-            created_at=created_at,
+            provider=provider,
+            endpoint=endpoint,
+            prompt_template=prompt_template,
+            chat_template=chat_template,
+            temperature=temperature,
+            max_tokens=max_tokens,
+            top_p=top_p,
+            stop=stop,
+            presence_penalty=presence_penalty,
+            frequency_penalty=frequency_penalty,
+            other=other,
+            name=name,
+            experiment=experiment,
         )
-        return self._log_oapg(
+        return self._register_oapg(
             body=args.body,
         )
```

### Comparing `humanloop-0.4.2/humanloop/paths/model_configs/post.py` & `humanloop-0.4.3/humanloop/paths/model_configs/post.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -30,51 +30,46 @@
 
 from humanloop import schemas  # noqa: F401
 
 from humanloop.model.model_providers import ModelProviders as ModelProvidersSchema
 from humanloop.model.project_model_config_request import ProjectModelConfigRequest as ProjectModelConfigRequestSchema
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
 from humanloop.model.model_endpoints import ModelEndpoints as ModelEndpointsSchema
-from humanloop.model.src_external_app_models_v3_model_configs_project_model_config_response import SrcExternalAppModelsV3ModelConfigsProjectModelConfigResponse as SrcExternalAppModelsV3ModelConfigsProjectModelConfigResponseSchema
+from humanloop.model.project_model_config_response import ProjectModelConfigResponse as ProjectModelConfigResponseSchema
 from humanloop.model.chat_message import ChatMessage as ChatMessageSchema
 
-from humanloop.type.src_external_app_models_v3_model_configs_project_model_config_response import SrcExternalAppModelsV3ModelConfigsProjectModelConfigResponse
 from humanloop.type.chat_message import ChatMessage
 from humanloop.type.project_model_config_request import ProjectModelConfigRequest
+from humanloop.type.project_model_config_response import ProjectModelConfigResponse
 from humanloop.type.model_providers import ModelProviders
 from humanloop.type.http_validation_error import HTTPValidationError
 from humanloop.type.model_endpoints import ModelEndpoints
 
-from . import path
-
 # body param
 SchemaForRequestBodyApplicationJson = ProjectModelConfigRequestSchema
 
 
 request_body_project_model_config_request = api_client.RequestBody(
     content={
         'application/json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
-_auth = [
-    'APIKeyHeader',
-]
-SchemaFor200ResponseBodyApplicationJson = SrcExternalAppModelsV3ModelConfigsProjectModelConfigResponseSchema
+SchemaFor200ResponseBodyApplicationJson = ProjectModelConfigResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: SrcExternalAppModelsV3ModelConfigsProjectModelConfigResponse
+    body: ProjectModelConfigResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: SrcExternalAppModelsV3ModelConfigsProjectModelConfigResponse
+    body: ProjectModelConfigResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -98,18 +93,14 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '422': _response_for_422,
-}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `humanloop-0.4.2/humanloop/paths/model_configs/post.pyi` & `humanloop-0.4.3/humanloop/paths/logs/post.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,50 +26,61 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
-from humanloop.model.model_providers import ModelProviders as ModelProvidersSchema
-from humanloop.model.project_model_config_request import ProjectModelConfigRequest as ProjectModelConfigRequestSchema
+from humanloop.model.agent_config_request import AgentConfigRequest as AgentConfigRequestSchema
+from humanloop.model.tool_config_request import ToolConfigRequest as ToolConfigRequestSchema
+from humanloop.model.log_datapoint_request import LogDatapointRequest as LogDatapointRequestSchema
+from humanloop.model.trace_model_config_request import TraceModelConfigRequest as TraceModelConfigRequestSchema
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
-from humanloop.model.model_endpoints import ModelEndpoints as ModelEndpointsSchema
-from humanloop.model.src_external_app_models_v3_model_configs_project_model_config_response import SrcExternalAppModelsV3ModelConfigsProjectModelConfigResponse as SrcExternalAppModelsV3ModelConfigsProjectModelConfigResponseSchema
+from humanloop.model.feedback import Feedback as FeedbackSchema
+from humanloop.model.logs_log_response import LogsLogResponse as LogsLogResponseSchema
+from humanloop.model.generic_config_request import GenericConfigRequest as GenericConfigRequestSchema
 from humanloop.model.chat_message import ChatMessage as ChatMessageSchema
 
-from humanloop.type.src_external_app_models_v3_model_configs_project_model_config_response import SrcExternalAppModelsV3ModelConfigsProjectModelConfigResponse
+from humanloop.type.feedback import Feedback
 from humanloop.type.chat_message import ChatMessage
-from humanloop.type.project_model_config_request import ProjectModelConfigRequest
-from humanloop.type.model_providers import ModelProviders
+from humanloop.type.agent_config_request import AgentConfigRequest
+from humanloop.type.generic_config_request import GenericConfigRequest
+from humanloop.type.tool_config_request import ToolConfigRequest
+from humanloop.type.logs_log_response import LogsLogResponse
+from humanloop.type.trace_model_config_request import TraceModelConfigRequest
+from humanloop.type.log_datapoint_request import LogDatapointRequest
 from humanloop.type.http_validation_error import HTTPValidationError
-from humanloop.type.model_endpoints import ModelEndpoints
+
+from . import path
 
 # body param
-SchemaForRequestBodyApplicationJson = ProjectModelConfigRequestSchema
+SchemaForRequestBodyApplicationJson = LogDatapointRequestSchema
 
 
-request_body_project_model_config_request = api_client.RequestBody(
+request_body_log_datapoint_request = api_client.RequestBody(
     content={
         'application/json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
-SchemaFor200ResponseBodyApplicationJson = SrcExternalAppModelsV3ModelConfigsProjectModelConfigResponseSchema
+_auth = [
+    'APIKeyHeader',
+]
+SchemaFor200ResponseBodyApplicationJson = LogsLogResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: SrcExternalAppModelsV3ModelConfigsProjectModelConfigResponse
+    body: LogsLogResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: SrcExternalAppModelsV3ModelConfigsProjectModelConfigResponse
+    body: LogsLogResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -93,89 +104,91 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
+_status_code_to_response = {
+    '200': _response_for_200,
+    '422': _response_for_422,
+}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
-    def _register_mapped_args(
+    def _log_mapped_args(
         self,
-        model: str,
-        project: str,
-        provider: typing.Optional[ModelProviders] = None,
-        endpoint: typing.Optional[ModelEndpoints] = None,
-        prompt_template: typing.Optional[str] = None,
-        chat_template: typing.Optional[typing.List[ChatMessage]] = None,
-        temperature: typing.Optional[typing.Union[int, float]] = None,
-        max_tokens: typing.Optional[int] = None,
-        top_p: typing.Optional[typing.Union[int, float]] = None,
-        stop: typing.Optional[typing.Union[str, typing.List[str]]] = None,
-        presence_penalty: typing.Optional[typing.Union[int, float]] = None,
-        frequency_penalty: typing.Optional[typing.Union[int, float]] = None,
-        other: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
-        name: typing.Optional[str] = None,
-        experiment: typing.Optional[str] = None,
+        body: typing.Optional[LogDatapointRequest] = None,
+        project: typing.Optional[str] = None,
+        session_id: typing.Optional[str] = None,
+        parent_id: typing.Optional[str] = None,
+        trial_id: typing.Optional[str] = None,
+        inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
+        messages: typing.Optional[typing.List[ChatMessage]] = None,
+        output: typing.Optional[str] = None,
+        source: typing.Optional[str] = None,
+        config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
+        metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
+        feedback: typing.Optional[typing.Union[Feedback, typing.List[Feedback]]] = None,
+        created_at: typing.Optional[datetime] = None,
+        error: typing.Optional[str] = None,
+        duration: typing.Optional[typing.Union[int, float]] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _body = {}
-        if provider is not None:
-            _body["provider"] = provider
-        if endpoint is not None:
-            _body["endpoint"] = endpoint
-        if model is not None:
-            _body["model"] = model
-        if prompt_template is not None:
-            _body["prompt_template"] = prompt_template
-        if chat_template is not None:
-            _body["chat_template"] = chat_template
-        if temperature is not None:
-            _body["temperature"] = temperature
-        if max_tokens is not None:
-            _body["max_tokens"] = max_tokens
-        if top_p is not None:
-            _body["top_p"] = top_p
-        if stop is not None:
-            _body["stop"] = stop
-        if presence_penalty is not None:
-            _body["presence_penalty"] = presence_penalty
-        if frequency_penalty is not None:
-            _body["frequency_penalty"] = frequency_penalty
-        if other is not None:
-            _body["other"] = other
         if project is not None:
             _body["project"] = project
-        if name is not None:
-            _body["name"] = name
-        if experiment is not None:
-            _body["experiment"] = experiment
-        args.body = _body
+        if session_id is not None:
+            _body["session_id"] = session_id
+        if parent_id is not None:
+            _body["parent_id"] = parent_id
+        if trial_id is not None:
+            _body["trial_id"] = trial_id
+        if inputs is not None:
+            _body["inputs"] = inputs
+        if messages is not None:
+            _body["messages"] = messages
+        if output is not None:
+            _body["output"] = output
+        if source is not None:
+            _body["source"] = source
+        if config is not None:
+            _body["config"] = config
+        if metadata is not None:
+            _body["metadata"] = metadata
+        if feedback is not None:
+            _body["feedback"] = feedback
+        if created_at is not None:
+            _body["created_at"] = created_at
+        if error is not None:
+            _body["error"] = error
+        if duration is not None:
+            _body["duration"] = duration
+        args.body = body if body is not None else _body
         return args
 
-    async def _aregister_oapg(
+    async def _alog_oapg(
         self,
         body: typing.Any = None,
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         content_type: str = 'application/json',
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        Register Model Config
+        Log
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
     
         _headers = HTTPHeaderDict()
@@ -185,15 +198,15 @@
                 _headers.add('Accept', accept_content_type)
     
         if body is schemas.unset:
             raise exceptions.ApiValueError(
                 'The required body parameter has an invalid value of: unset. Set a valid value instead')
         _fields = None
         _body = None
-        serialized_data = request_body_project_model_config_request.serialize(body, content_type)
+        serialized_data = request_body_log_datapoint_request.serialize(body, content_type)
         _headers.add('Content-Type', content_type)
         if 'fields' in serialized_data:
             _fields = serialized_data['fields']
         elif 'body' in serialized_data:
             _body = serialized_data['body']    
         response = await self.api_client.async_call_api(
             resource_path=used_path,
@@ -247,28 +260,28 @@
     
         # cleanup session / response
         response.http_response.close()
         await response.session.close()
     
         return api_response
 
-    def _register_oapg(
+    def _log_oapg(
         self,
         body: typing.Any = None,
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         content_type: str = 'application/json',
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        Register Model Config
+        Log
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
     
         _headers = HTTPHeaderDict()
@@ -278,15 +291,15 @@
                 _headers.add('Accept', accept_content_type)
     
         if body is schemas.unset:
             raise exceptions.ApiValueError(
                 'The required body parameter has an invalid value of: unset. Set a valid value instead')
         _fields = None
         _body = None
-        serialized_data = request_body_project_model_config_request.serialize(body, content_type)
+        serialized_data = request_body_log_datapoint_request.serialize(body, content_type)
         _headers.add('Content-Type', content_type)
         if 'fields' in serialized_data:
             _fields = serialized_data['fields']
         elif 'body' in serialized_data:
             _body = serialized_data['body']    
         response = self.api_client.call_api(
             resource_path=used_path,
@@ -318,183 +331,183 @@
             )
     
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
     
         return api_response
 
-class Register(BaseApi):
+class Log(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    async def aregister(
+    async def alog(
         self,
-        model: str,
-        project: str,
-        provider: typing.Optional[ModelProviders] = None,
-        endpoint: typing.Optional[ModelEndpoints] = None,
-        prompt_template: typing.Optional[str] = None,
-        chat_template: typing.Optional[typing.List[ChatMessage]] = None,
-        temperature: typing.Optional[typing.Union[int, float]] = None,
-        max_tokens: typing.Optional[int] = None,
-        top_p: typing.Optional[typing.Union[int, float]] = None,
-        stop: typing.Optional[typing.Union[str, typing.List[str]]] = None,
-        presence_penalty: typing.Optional[typing.Union[int, float]] = None,
-        frequency_penalty: typing.Optional[typing.Union[int, float]] = None,
-        other: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
-        name: typing.Optional[str] = None,
-        experiment: typing.Optional[str] = None,
+        body: typing.Optional[LogDatapointRequest] = None,
+        project: typing.Optional[str] = None,
+        session_id: typing.Optional[str] = None,
+        parent_id: typing.Optional[str] = None,
+        trial_id: typing.Optional[str] = None,
+        inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
+        messages: typing.Optional[typing.List[ChatMessage]] = None,
+        output: typing.Optional[str] = None,
+        source: typing.Optional[str] = None,
+        config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
+        metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
+        feedback: typing.Optional[typing.Union[Feedback, typing.List[Feedback]]] = None,
+        created_at: typing.Optional[datetime] = None,
+        error: typing.Optional[str] = None,
+        duration: typing.Optional[typing.Union[int, float]] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._register_mapped_args(
-            model=model,
+        args = self._log_mapped_args(
+            body=body,
             project=project,
-            provider=provider,
-            endpoint=endpoint,
-            prompt_template=prompt_template,
-            chat_template=chat_template,
-            temperature=temperature,
-            max_tokens=max_tokens,
-            top_p=top_p,
-            stop=stop,
-            presence_penalty=presence_penalty,
-            frequency_penalty=frequency_penalty,
-            other=other,
-            name=name,
-            experiment=experiment,
+            session_id=session_id,
+            parent_id=parent_id,
+            trial_id=trial_id,
+            inputs=inputs,
+            messages=messages,
+            output=output,
+            source=source,
+            config=config,
+            metadata=metadata,
+            feedback=feedback,
+            created_at=created_at,
+            error=error,
+            duration=duration,
         )
-        return await self._aregister_oapg(
+        return await self._alog_oapg(
             body=args.body,
         )
     
-    def register(
+    def log(
         self,
-        model: str,
-        project: str,
-        provider: typing.Optional[ModelProviders] = None,
-        endpoint: typing.Optional[ModelEndpoints] = None,
-        prompt_template: typing.Optional[str] = None,
-        chat_template: typing.Optional[typing.List[ChatMessage]] = None,
-        temperature: typing.Optional[typing.Union[int, float]] = None,
-        max_tokens: typing.Optional[int] = None,
-        top_p: typing.Optional[typing.Union[int, float]] = None,
-        stop: typing.Optional[typing.Union[str, typing.List[str]]] = None,
-        presence_penalty: typing.Optional[typing.Union[int, float]] = None,
-        frequency_penalty: typing.Optional[typing.Union[int, float]] = None,
-        other: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
-        name: typing.Optional[str] = None,
-        experiment: typing.Optional[str] = None,
+        body: typing.Optional[LogDatapointRequest] = None,
+        project: typing.Optional[str] = None,
+        session_id: typing.Optional[str] = None,
+        parent_id: typing.Optional[str] = None,
+        trial_id: typing.Optional[str] = None,
+        inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
+        messages: typing.Optional[typing.List[ChatMessage]] = None,
+        output: typing.Optional[str] = None,
+        source: typing.Optional[str] = None,
+        config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
+        metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
+        feedback: typing.Optional[typing.Union[Feedback, typing.List[Feedback]]] = None,
+        created_at: typing.Optional[datetime] = None,
+        error: typing.Optional[str] = None,
+        duration: typing.Optional[typing.Union[int, float]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._register_mapped_args(
-            model=model,
+        args = self._log_mapped_args(
+            body=body,
             project=project,
-            provider=provider,
-            endpoint=endpoint,
-            prompt_template=prompt_template,
-            chat_template=chat_template,
-            temperature=temperature,
-            max_tokens=max_tokens,
-            top_p=top_p,
-            stop=stop,
-            presence_penalty=presence_penalty,
-            frequency_penalty=frequency_penalty,
-            other=other,
-            name=name,
-            experiment=experiment,
+            session_id=session_id,
+            parent_id=parent_id,
+            trial_id=trial_id,
+            inputs=inputs,
+            messages=messages,
+            output=output,
+            source=source,
+            config=config,
+            metadata=metadata,
+            feedback=feedback,
+            created_at=created_at,
+            error=error,
+            duration=duration,
         )
-        return self._register_oapg(
+        return self._log_oapg(
             body=args.body,
         )
 
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     async def apost(
         self,
-        model: str,
-        project: str,
-        provider: typing.Optional[ModelProviders] = None,
-        endpoint: typing.Optional[ModelEndpoints] = None,
-        prompt_template: typing.Optional[str] = None,
-        chat_template: typing.Optional[typing.List[ChatMessage]] = None,
-        temperature: typing.Optional[typing.Union[int, float]] = None,
-        max_tokens: typing.Optional[int] = None,
-        top_p: typing.Optional[typing.Union[int, float]] = None,
-        stop: typing.Optional[typing.Union[str, typing.List[str]]] = None,
-        presence_penalty: typing.Optional[typing.Union[int, float]] = None,
-        frequency_penalty: typing.Optional[typing.Union[int, float]] = None,
-        other: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
-        name: typing.Optional[str] = None,
-        experiment: typing.Optional[str] = None,
+        body: typing.Optional[LogDatapointRequest] = None,
+        project: typing.Optional[str] = None,
+        session_id: typing.Optional[str] = None,
+        parent_id: typing.Optional[str] = None,
+        trial_id: typing.Optional[str] = None,
+        inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
+        messages: typing.Optional[typing.List[ChatMessage]] = None,
+        output: typing.Optional[str] = None,
+        source: typing.Optional[str] = None,
+        config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
+        metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
+        feedback: typing.Optional[typing.Union[Feedback, typing.List[Feedback]]] = None,
+        created_at: typing.Optional[datetime] = None,
+        error: typing.Optional[str] = None,
+        duration: typing.Optional[typing.Union[int, float]] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._register_mapped_args(
-            model=model,
+        args = self._log_mapped_args(
+            body=body,
             project=project,
-            provider=provider,
-            endpoint=endpoint,
-            prompt_template=prompt_template,
-            chat_template=chat_template,
-            temperature=temperature,
-            max_tokens=max_tokens,
-            top_p=top_p,
-            stop=stop,
-            presence_penalty=presence_penalty,
-            frequency_penalty=frequency_penalty,
-            other=other,
-            name=name,
-            experiment=experiment,
+            session_id=session_id,
+            parent_id=parent_id,
+            trial_id=trial_id,
+            inputs=inputs,
+            messages=messages,
+            output=output,
+            source=source,
+            config=config,
+            metadata=metadata,
+            feedback=feedback,
+            created_at=created_at,
+            error=error,
+            duration=duration,
         )
-        return await self._aregister_oapg(
+        return await self._alog_oapg(
             body=args.body,
         )
     
     def post(
         self,
-        model: str,
-        project: str,
-        provider: typing.Optional[ModelProviders] = None,
-        endpoint: typing.Optional[ModelEndpoints] = None,
-        prompt_template: typing.Optional[str] = None,
-        chat_template: typing.Optional[typing.List[ChatMessage]] = None,
-        temperature: typing.Optional[typing.Union[int, float]] = None,
-        max_tokens: typing.Optional[int] = None,
-        top_p: typing.Optional[typing.Union[int, float]] = None,
-        stop: typing.Optional[typing.Union[str, typing.List[str]]] = None,
-        presence_penalty: typing.Optional[typing.Union[int, float]] = None,
-        frequency_penalty: typing.Optional[typing.Union[int, float]] = None,
-        other: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
-        name: typing.Optional[str] = None,
-        experiment: typing.Optional[str] = None,
+        body: typing.Optional[LogDatapointRequest] = None,
+        project: typing.Optional[str] = None,
+        session_id: typing.Optional[str] = None,
+        parent_id: typing.Optional[str] = None,
+        trial_id: typing.Optional[str] = None,
+        inputs: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
+        messages: typing.Optional[typing.List[ChatMessage]] = None,
+        output: typing.Optional[str] = None,
+        source: typing.Optional[str] = None,
+        config: typing.Optional[typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]] = None,
+        metadata: typing.Optional[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]] = None,
+        feedback: typing.Optional[typing.Union[Feedback, typing.List[Feedback]]] = None,
+        created_at: typing.Optional[datetime] = None,
+        error: typing.Optional[str] = None,
+        duration: typing.Optional[typing.Union[int, float]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._register_mapped_args(
-            model=model,
+        args = self._log_mapped_args(
+            body=body,
             project=project,
-            provider=provider,
-            endpoint=endpoint,
-            prompt_template=prompt_template,
-            chat_template=chat_template,
-            temperature=temperature,
-            max_tokens=max_tokens,
-            top_p=top_p,
-            stop=stop,
-            presence_penalty=presence_penalty,
-            frequency_penalty=frequency_penalty,
-            other=other,
-            name=name,
-            experiment=experiment,
+            session_id=session_id,
+            parent_id=parent_id,
+            trial_id=trial_id,
+            inputs=inputs,
+            messages=messages,
+            output=output,
+            source=source,
+            config=config,
+            metadata=metadata,
+            feedback=feedback,
+            created_at=created_at,
+            error=error,
+            duration=duration,
         )
-        return self._register_oapg(
+        return self._log_oapg(
             body=args.body,
         )
```

### Comparing `humanloop-0.4.2/humanloop/paths/model_configs_id/get.py` & `humanloop-0.4.3/humanloop/paths/model_configs_id/get.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -26,21 +26,19 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
+from humanloop.model.model_config_response import ModelConfigResponse as ModelConfigResponseSchema
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
-from humanloop.model.src_external_app_models_v3_model_configs_model_config_response import SrcExternalAppModelsV3ModelConfigsModelConfigResponse as SrcExternalAppModelsV3ModelConfigsModelConfigResponseSchema
 
-from humanloop.type.src_external_app_models_v3_model_configs_model_config_response import SrcExternalAppModelsV3ModelConfigsModelConfigResponse
 from humanloop.type.http_validation_error import HTTPValidationError
-
-from . import path
+from humanloop.type.model_config_response import ModelConfigResponse
 
 # Path params
 IdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
         'id': typing.Union[IdSchema, str, ],
@@ -60,28 +58,25 @@
 
 request_path_id = api_client.PathParameter(
     name="id",
     style=api_client.ParameterStyle.SIMPLE,
     schema=IdSchema,
     required=True,
 )
-_auth = [
-    'APIKeyHeader',
-]
-SchemaFor200ResponseBodyApplicationJson = SrcExternalAppModelsV3ModelConfigsModelConfigResponseSchema
+SchemaFor200ResponseBodyApplicationJson = ModelConfigResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: SrcExternalAppModelsV3ModelConfigsModelConfigResponse
+    body: ModelConfigResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: SrcExternalAppModelsV3ModelConfigsModelConfigResponse
+    body: ModelConfigResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -105,18 +100,14 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '422': _response_for_422,
-}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `humanloop-0.4.2/humanloop/paths/model_configs_id/get.pyi` & `humanloop-0.4.3/humanloop/paths/projects_id/get.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,20 +26,22 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
+from humanloop.model.project_response import ProjectResponse as ProjectResponseSchema
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
-from humanloop.model.src_external_app_models_v3_model_configs_model_config_response import SrcExternalAppModelsV3ModelConfigsModelConfigResponse as SrcExternalAppModelsV3ModelConfigsModelConfigResponseSchema
 
-from humanloop.type.src_external_app_models_v3_model_configs_model_config_response import SrcExternalAppModelsV3ModelConfigsModelConfigResponse
+from humanloop.type.project_response import ProjectResponse
 from humanloop.type.http_validation_error import HTTPValidationError
 
+from . import path
+
 # Path params
 IdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
         'id': typing.Union[IdSchema, str, ],
     }
@@ -58,25 +60,28 @@
 
 request_path_id = api_client.PathParameter(
     name="id",
     style=api_client.ParameterStyle.SIMPLE,
     schema=IdSchema,
     required=True,
 )
-SchemaFor200ResponseBodyApplicationJson = SrcExternalAppModelsV3ModelConfigsModelConfigResponseSchema
+_auth = [
+    'APIKeyHeader',
+]
+SchemaFor200ResponseBodyApplicationJson = ProjectResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: SrcExternalAppModelsV3ModelConfigsModelConfigResponse
+    body: ProjectResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: SrcExternalAppModelsV3ModelConfigsModelConfigResponse
+    body: ProjectResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -100,14 +105,18 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
+_status_code_to_response = {
+    '200': _response_for_200,
+    '422': _response_for_422,
+}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
@@ -131,15 +140,15 @@
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        Get Model Config
+        Get Project
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
@@ -223,15 +232,15 @@
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        Get Model Config
+        Get Project
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
```

### Comparing `humanloop-0.4.2/humanloop/paths/projects/get.py` & `humanloop-0.4.3/humanloop/paths/projects/get.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/projects/get.pyi` & `humanloop-0.4.3/humanloop/paths/projects/get.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/projects/post.py` & `humanloop-0.4.3/humanloop/paths/projects/post.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/projects/post.pyi` & `humanloop-0.4.3/humanloop/paths/projects/post.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/projects_id/get.py` & `humanloop-0.4.3/humanloop/paths/projects_id/get.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,14 @@
 
 from humanloop.model.project_response import ProjectResponse as ProjectResponseSchema
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
 
 from humanloop.type.project_response import ProjectResponse
 from humanloop.type.http_validation_error import HTTPValidationError
 
-from . import path
-
 # Path params
 IdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
         'id': typing.Union[IdSchema, str, ],
     }
@@ -60,17 +58,14 @@
 
 request_path_id = api_client.PathParameter(
     name="id",
     style=api_client.ParameterStyle.SIMPLE,
     schema=IdSchema,
     required=True,
 )
-_auth = [
-    'APIKeyHeader',
-]
 SchemaFor200ResponseBodyApplicationJson = ProjectResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     body: ProjectResponse
 
@@ -105,18 +100,14 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '422': _response_for_422,
-}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `humanloop-0.4.2/humanloop/paths/projects_id/get.pyi` & `humanloop-0.4.3/humanloop/paths/model_configs_id/get.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,19 +26,21 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
-from humanloop.model.project_response import ProjectResponse as ProjectResponseSchema
+from humanloop.model.model_config_response import ModelConfigResponse as ModelConfigResponseSchema
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
 
-from humanloop.type.project_response import ProjectResponse
 from humanloop.type.http_validation_error import HTTPValidationError
+from humanloop.type.model_config_response import ModelConfigResponse
+
+from . import path
 
 # Path params
 IdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
         'id': typing.Union[IdSchema, str, ],
@@ -58,25 +60,28 @@
 
 request_path_id = api_client.PathParameter(
     name="id",
     style=api_client.ParameterStyle.SIMPLE,
     schema=IdSchema,
     required=True,
 )
-SchemaFor200ResponseBodyApplicationJson = ProjectResponseSchema
+_auth = [
+    'APIKeyHeader',
+]
+SchemaFor200ResponseBodyApplicationJson = ModelConfigResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: ProjectResponse
+    body: ModelConfigResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: ProjectResponse
+    body: ModelConfigResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -100,14 +105,18 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
+_status_code_to_response = {
+    '200': _response_for_200,
+    '422': _response_for_422,
+}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
@@ -131,15 +140,15 @@
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        Get Project
+        Get Model Config
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
@@ -223,15 +232,15 @@
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        Get Project
+        Get Model Config
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
```

### Comparing `humanloop-0.4.2/humanloop/paths/projects_id/patch.py` & `humanloop-0.4.3/humanloop/paths/projects_id/patch.py`

 * *Files 6% similar despite different names*

```diff
@@ -135,24 +135,24 @@
 
 class BaseApi(api_client.Api):
 
     def _update_mapped_args(
         self,
         id: str,
         active_experiment_id: typing.Optional[str] = None,
-        active_model_config_id: typing.Optional[str] = None,
+        active_config_id: typing.Optional[str] = None,
         positive_labels: typing.Optional[typing.List[PositiveLabel]] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _path_params = {}
         _body = {}
         if active_experiment_id is not None:
             _body["active_experiment_id"] = active_experiment_id
-        if active_model_config_id is not None:
-            _body["active_model_config_id"] = active_model_config_id
+        if active_config_id is not None:
+            _body["active_config_id"] = active_config_id
         if positive_labels is not None:
             _body["positive_labels"] = positive_labels
         args.body = _body
         if id is not None:
             _path_params["id"] = id
         args.path = _path_params
         return args
@@ -355,92 +355,92 @@
 class Update(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     async def aupdate(
         self,
         id: str,
         active_experiment_id: typing.Optional[str] = None,
-        active_model_config_id: typing.Optional[str] = None,
+        active_config_id: typing.Optional[str] = None,
         positive_labels: typing.Optional[typing.List[PositiveLabel]] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._update_mapped_args(
             id=id,
             active_experiment_id=active_experiment_id,
-            active_model_config_id=active_model_config_id,
+            active_config_id=active_config_id,
             positive_labels=positive_labels,
         )
         return await self._aupdate_oapg(
             body=args.body,
             path_params=args.path,
         )
     
     def update(
         self,
         id: str,
         active_experiment_id: typing.Optional[str] = None,
-        active_model_config_id: typing.Optional[str] = None,
+        active_config_id: typing.Optional[str] = None,
         positive_labels: typing.Optional[typing.List[PositiveLabel]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._update_mapped_args(
             id=id,
             active_experiment_id=active_experiment_id,
-            active_model_config_id=active_model_config_id,
+            active_config_id=active_config_id,
             positive_labels=positive_labels,
         )
         return self._update_oapg(
             body=args.body,
             path_params=args.path,
         )
 
 class ApiForpatch(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     async def apatch(
         self,
         id: str,
         active_experiment_id: typing.Optional[str] = None,
-        active_model_config_id: typing.Optional[str] = None,
+        active_config_id: typing.Optional[str] = None,
         positive_labels: typing.Optional[typing.List[PositiveLabel]] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._update_mapped_args(
             id=id,
             active_experiment_id=active_experiment_id,
-            active_model_config_id=active_model_config_id,
+            active_config_id=active_config_id,
             positive_labels=positive_labels,
         )
         return await self._aupdate_oapg(
             body=args.body,
             path_params=args.path,
         )
     
     def patch(
         self,
         id: str,
         active_experiment_id: typing.Optional[str] = None,
-        active_model_config_id: typing.Optional[str] = None,
+        active_config_id: typing.Optional[str] = None,
         positive_labels: typing.Optional[typing.List[PositiveLabel]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._update_mapped_args(
             id=id,
             active_experiment_id=active_experiment_id,
-            active_model_config_id=active_model_config_id,
+            active_config_id=active_config_id,
             positive_labels=positive_labels,
         )
         return self._update_oapg(
             body=args.body,
             path_params=args.path,
         )
```

### Comparing `humanloop-0.4.2/humanloop/paths/projects_id/patch.pyi` & `humanloop-0.4.3/humanloop/paths/projects_id/patch.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -126,24 +126,24 @@
 
 class BaseApi(api_client.Api):
 
     def _update_mapped_args(
         self,
         id: str,
         active_experiment_id: typing.Optional[str] = None,
-        active_model_config_id: typing.Optional[str] = None,
+        active_config_id: typing.Optional[str] = None,
         positive_labels: typing.Optional[typing.List[PositiveLabel]] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _path_params = {}
         _body = {}
         if active_experiment_id is not None:
             _body["active_experiment_id"] = active_experiment_id
-        if active_model_config_id is not None:
-            _body["active_model_config_id"] = active_model_config_id
+        if active_config_id is not None:
+            _body["active_config_id"] = active_config_id
         if positive_labels is not None:
             _body["positive_labels"] = positive_labels
         args.body = _body
         if id is not None:
             _path_params["id"] = id
         args.path = _path_params
         return args
@@ -346,92 +346,92 @@
 class Update(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     async def aupdate(
         self,
         id: str,
         active_experiment_id: typing.Optional[str] = None,
-        active_model_config_id: typing.Optional[str] = None,
+        active_config_id: typing.Optional[str] = None,
         positive_labels: typing.Optional[typing.List[PositiveLabel]] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._update_mapped_args(
             id=id,
             active_experiment_id=active_experiment_id,
-            active_model_config_id=active_model_config_id,
+            active_config_id=active_config_id,
             positive_labels=positive_labels,
         )
         return await self._aupdate_oapg(
             body=args.body,
             path_params=args.path,
         )
     
     def update(
         self,
         id: str,
         active_experiment_id: typing.Optional[str] = None,
-        active_model_config_id: typing.Optional[str] = None,
+        active_config_id: typing.Optional[str] = None,
         positive_labels: typing.Optional[typing.List[PositiveLabel]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._update_mapped_args(
             id=id,
             active_experiment_id=active_experiment_id,
-            active_model_config_id=active_model_config_id,
+            active_config_id=active_config_id,
             positive_labels=positive_labels,
         )
         return self._update_oapg(
             body=args.body,
             path_params=args.path,
         )
 
 class ApiForpatch(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     async def apatch(
         self,
         id: str,
         active_experiment_id: typing.Optional[str] = None,
-        active_model_config_id: typing.Optional[str] = None,
+        active_config_id: typing.Optional[str] = None,
         positive_labels: typing.Optional[typing.List[PositiveLabel]] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._update_mapped_args(
             id=id,
             active_experiment_id=active_experiment_id,
-            active_model_config_id=active_model_config_id,
+            active_config_id=active_config_id,
             positive_labels=positive_labels,
         )
         return await self._aupdate_oapg(
             body=args.body,
             path_params=args.path,
         )
     
     def patch(
         self,
         id: str,
         active_experiment_id: typing.Optional[str] = None,
-        active_model_config_id: typing.Optional[str] = None,
+        active_config_id: typing.Optional[str] = None,
         positive_labels: typing.Optional[typing.List[PositiveLabel]] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._update_mapped_args(
             id=id,
             active_experiment_id=active_experiment_id,
-            active_model_config_id=active_model_config_id,
+            active_config_id=active_config_id,
             positive_labels=positive_labels,
         )
         return self._update_oapg(
             body=args.body,
             path_params=args.path,
         )
```

### Comparing `humanloop-0.4.2/humanloop/paths/projects_id_active_experiment/delete.py` & `humanloop-0.4.3/humanloop/paths/projects_id_active_experiment/delete.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/projects_id_active_experiment/delete.pyi` & `humanloop-0.4.3/humanloop/paths/projects_id_active_experiment/delete.pyi`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/paths/projects_id_active_model_config/delete.py` & `humanloop-0.4.3/humanloop/paths/projects_id_active_config/delete.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -32,16 +32,14 @@
 
 from humanloop.model.project_response import ProjectResponse as ProjectResponseSchema
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
 
 from humanloop.type.project_response import ProjectResponse
 from humanloop.type.http_validation_error import HTTPValidationError
 
-from . import path
-
 # Path params
 IdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
         'id': typing.Union[IdSchema, str, ],
     }
@@ -60,17 +58,14 @@
 
 request_path_id = api_client.PathParameter(
     name="id",
     style=api_client.ParameterStyle.SIMPLE,
     schema=IdSchema,
     required=True,
 )
-_auth = [
-    'APIKeyHeader',
-]
 SchemaFor200ResponseBodyApplicationJson = ProjectResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     body: ProjectResponse
 
@@ -105,50 +100,46 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '422': _response_for_422,
-}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
-    def _delete_active_model_config_mapped_args(
+    def _deactivate_active_config_mapped_args(
         self,
         id: str,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _path_params = {}
         if id is not None:
             _path_params["id"] = id
         args.path = _path_params
         return args
 
-    async def _adelete_active_model_config_oapg(
+    async def _adeactivate_active_config_oapg(
         self,
             path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        Deactivate Model Config
+        Deactivate Config
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
@@ -220,27 +211,27 @@
     
         # cleanup session / response
         response.http_response.close()
         await response.session.close()
     
         return api_response
 
-    def _delete_active_model_config_oapg(
+    def _deactivate_active_config_oapg(
         self,
             path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        Deactivate Model Config
+        Deactivate Config
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
@@ -290,71 +281,71 @@
             )
     
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
     
         return api_response
 
-class DeleteActiveModelConfig(BaseApi):
+class DeactivateActiveConfig(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    async def adelete_active_model_config(
+    async def adeactivate_active_config(
         self,
         id: str,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._delete_active_model_config_mapped_args(
+        args = self._deactivate_active_config_mapped_args(
             id=id,
         )
-        return await self._adelete_active_model_config_oapg(
+        return await self._adeactivate_active_config_oapg(
             path_params=args.path,
         )
     
-    def delete_active_model_config(
+    def deactivate_active_config(
         self,
         id: str,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._delete_active_model_config_mapped_args(
+        args = self._deactivate_active_config_mapped_args(
             id=id,
         )
-        return self._delete_active_model_config_oapg(
+        return self._deactivate_active_config_oapg(
             path_params=args.path,
         )
 
 class ApiFordelete(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     async def adelete(
         self,
         id: str,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._delete_active_model_config_mapped_args(
+        args = self._deactivate_active_config_mapped_args(
             id=id,
         )
-        return await self._adelete_active_model_config_oapg(
+        return await self._adeactivate_active_config_oapg(
             path_params=args.path,
         )
     
     def delete(
         self,
         id: str,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._delete_active_model_config_mapped_args(
+        args = self._deactivate_active_config_mapped_args(
             id=id,
         )
-        return self._delete_active_model_config_oapg(
+        return self._deactivate_active_config_oapg(
             path_params=args.path,
         )
```

### Comparing `humanloop-0.4.2/humanloop/paths/projects_id_active_model_config/delete.pyi` & `humanloop-0.4.3/humanloop/paths/projects_id_active_config/get.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,20 +26,22 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
-from humanloop.model.project_response import ProjectResponse as ProjectResponseSchema
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
+from humanloop.model.get_model_config_response import GetModelConfigResponse as GetModelConfigResponseSchema
 
-from humanloop.type.project_response import ProjectResponse
+from humanloop.type.get_model_config_response import GetModelConfigResponse
 from humanloop.type.http_validation_error import HTTPValidationError
 
+from . import path
+
 # Path params
 IdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
         'id': typing.Union[IdSchema, str, ],
     }
@@ -58,25 +60,28 @@
 
 request_path_id = api_client.PathParameter(
     name="id",
     style=api_client.ParameterStyle.SIMPLE,
     schema=IdSchema,
     required=True,
 )
-SchemaFor200ResponseBodyApplicationJson = ProjectResponseSchema
+_auth = [
+    'APIKeyHeader',
+]
+SchemaFor200ResponseBodyApplicationJson = GetModelConfigResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: ProjectResponse
+    body: GetModelConfigResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: ProjectResponse
+    body: GetModelConfigResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -100,46 +105,50 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
+_status_code_to_response = {
+    '200': _response_for_200,
+    '422': _response_for_422,
+}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
-    def _delete_active_model_config_mapped_args(
+    def _get_config_mapped_args(
         self,
         id: str,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _path_params = {}
         if id is not None:
             _path_params["id"] = id
         args.path = _path_params
         return args
 
-    async def _adelete_active_model_config_oapg(
+    async def _aget_config_oapg(
         self,
             path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        Deactivate Model Config
+        Get Active Config
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
@@ -160,15 +169,15 @@
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
     
         response = await self.api_client.async_call_api(
             resource_path=used_path,
-            method='delete'.upper(),
+            method='get'.upper(),
             headers=_headers,
             auth_settings=_auth,
             timeout=timeout,
         )
         
         if stream:
             async def stream_iterator():
@@ -211,27 +220,27 @@
     
         # cleanup session / response
         response.http_response.close()
         await response.session.close()
     
         return api_response
 
-    def _delete_active_model_config_oapg(
+    def _get_config_oapg(
         self,
             path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        Deactivate Model Config
+        Get Active Config
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
@@ -252,15 +261,15 @@
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
     
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='delete'.upper(),
+            method='get'.upper(),
             headers=_headers,
             auth_settings=_auth,
             timeout=timeout,
         )
     
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
         if response_for_status:
@@ -281,71 +290,71 @@
             )
     
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
     
         return api_response
 
-class DeleteActiveModelConfig(BaseApi):
+class GetConfig(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    async def adelete_active_model_config(
+    async def aget_config(
         self,
         id: str,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._delete_active_model_config_mapped_args(
+        args = self._get_config_mapped_args(
             id=id,
         )
-        return await self._adelete_active_model_config_oapg(
+        return await self._aget_config_oapg(
             path_params=args.path,
         )
     
-    def delete_active_model_config(
+    def get_config(
         self,
         id: str,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._delete_active_model_config_mapped_args(
+        args = self._get_config_mapped_args(
             id=id,
         )
-        return self._delete_active_model_config_oapg(
+        return self._get_config_oapg(
             path_params=args.path,
         )
 
-class ApiFordelete(BaseApi):
+class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    async def adelete(
+    async def aget(
         self,
         id: str,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._delete_active_model_config_mapped_args(
+        args = self._get_config_mapped_args(
             id=id,
         )
-        return await self._adelete_active_model_config_oapg(
+        return await self._aget_config_oapg(
             path_params=args.path,
         )
     
-    def delete(
+    def get(
         self,
         id: str,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._delete_active_model_config_mapped_args(
+        args = self._get_config_mapped_args(
             id=id,
         )
-        return self._delete_active_model_config_oapg(
+        return self._get_config_oapg(
             path_params=args.path,
         )
```

### Comparing `humanloop-0.4.2/humanloop/paths/projects_id_export/post.py` & `humanloop-0.4.3/humanloop/paths/sessions/get.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -27,27 +27,27 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
-from humanloop.model.paginated_data_log_response import PaginatedDataLogResponse as PaginatedDataLogResponseSchema
+from humanloop.model.paginated_data_session_response import PaginatedDataSessionResponse as PaginatedDataSessionResponseSchema
 
-from humanloop.type.paginated_data_log_response import PaginatedDataLogResponse
+from humanloop.type.paginated_data_session_response import PaginatedDataSessionResponse
 from humanloop.type.http_validation_error import HTTPValidationError
 
-from . import path
-
 # Query params
+ProjectIdSchema = schemas.StrSchema
 PageSchema = schemas.IntSchema
 SizeSchema = schemas.IntSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
+        'project_id': typing.Union[ProjectIdSchema, str, ],
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
     'RequestOptionalQueryParams',
     {
         'page': typing.Union[PageSchema, decimal.Decimal, int, ],
         'size': typing.Union[SizeSchema, decimal.Decimal, int, ],
@@ -56,66 +56,44 @@
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
 
 
+request_query_project_id = api_client.QueryParameter(
+    name="project_id",
+    style=api_client.ParameterStyle.FORM,
+    schema=ProjectIdSchema,
+    required=True,
+    explode=True,
+)
 request_query_page = api_client.QueryParameter(
     name="page",
     style=api_client.ParameterStyle.FORM,
     schema=PageSchema,
     explode=True,
 )
 request_query_size = api_client.QueryParameter(
     name="size",
     style=api_client.ParameterStyle.FORM,
     schema=SizeSchema,
     explode=True,
 )
-# Path params
-IdSchema = schemas.StrSchema
-RequestRequiredPathParams = typing_extensions.TypedDict(
-    'RequestRequiredPathParams',
-    {
-        'id': typing.Union[IdSchema, str, ],
-    }
-)
-RequestOptionalPathParams = typing_extensions.TypedDict(
-    'RequestOptionalPathParams',
-    {
-    },
-    total=False
-)
-
-
-class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
-    pass
-
-
-request_path_id = api_client.PathParameter(
-    name="id",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=IdSchema,
-    required=True,
-)
-_auth = [
-    'APIKeyHeader',
-]
-SchemaFor200ResponseBodyApplicationJson = PaginatedDataLogResponseSchema
+SchemaFor200ResponseBodyApplicationJson = PaginatedDataSessionResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: PaginatedDataLogResponse
+    body: PaginatedDataSessionResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: PaginatedDataLogResponse
+    body: PaginatedDataSessionResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -139,82 +117,62 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '422': _response_for_422,
-}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
-    def _export_datapoints_mapped_args(
+    def _list_mapped_args(
         self,
-        id: str,
+        project_id: str,
         page: typing.Optional[int] = None,
         size: typing.Optional[int] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _query_params = {}
-        _path_params = {}
+        if project_id is not None:
+            _query_params["project_id"] = project_id
         if page is not None:
             _query_params["page"] = page
         if size is not None:
             _query_params["size"] = size
-        if id is not None:
-            _path_params["id"] = id
         args.query = _query_params
-        args.path = _path_params
         return args
 
-    async def _aexport_datapoints_oapg(
+    async def _alist_oapg(
         self,
             query_params: typing.Optional[dict] = {},
-            path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        Export Datapoints
+        Get Sessions
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
-        self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
-        _path_params = {}
-        for parameter in (
-            request_path_id,
-        ):
-            parameter_data = path_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            serialized_data = parameter.serialize(parameter_data)
-            _path_params.update(serialized_data)
-    
-        for k, v in _path_params.items():
-            used_path = used_path.replace('{%s}' % k, v)
-    
         prefix_separator_iterator = None
         for parameter in (
+            request_query_project_id,
             request_query_page,
             request_query_size,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
@@ -227,15 +185,15 @@
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
     
         response = await self.api_client.async_call_api(
             resource_path=used_path,
-            method='post'.upper(),
+            method='get'.upper(),
             headers=_headers,
             auth_settings=_auth,
             prefix_separator_iterator=prefix_separator_iterator,
             timeout=timeout,
         )
         
         if stream:
@@ -279,51 +237,37 @@
     
         # cleanup session / response
         response.http_response.close()
         await response.session.close()
     
         return api_response
 
-    def _export_datapoints_oapg(
+    def _list_oapg(
         self,
             query_params: typing.Optional[dict] = {},
-            path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        Export Datapoints
+        Get Sessions
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
-        self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
-        _path_params = {}
-        for parameter in (
-            request_path_id,
-        ):
-            parameter_data = path_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            serialized_data = parameter.serialize(parameter_data)
-            _path_params.update(serialized_data)
-    
-        for k, v in _path_params.items():
-            used_path = used_path.replace('{%s}' % k, v)
-    
         prefix_separator_iterator = None
         for parameter in (
+            request_query_project_id,
             request_query_page,
             request_query_size,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
@@ -336,15 +280,15 @@
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
     
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='post'.upper(),
+            method='get'.upper(),
             headers=_headers,
             auth_settings=_auth,
             prefix_separator_iterator=prefix_separator_iterator,
             timeout=timeout,
         )
     
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
@@ -366,91 +310,87 @@
             )
     
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
     
         return api_response
 
-class ExportDatapoints(BaseApi):
+class List(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    async def aexport_datapoints(
+    async def alist(
         self,
-        id: str,
+        project_id: str,
         page: typing.Optional[int] = None,
         size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._export_datapoints_mapped_args(
-            id=id,
+        args = self._list_mapped_args(
+            project_id=project_id,
             page=page,
             size=size,
         )
-        return await self._aexport_datapoints_oapg(
+        return await self._alist_oapg(
             query_params=args.query,
-            path_params=args.path,
         )
     
-    def export_datapoints(
+    def list(
         self,
-        id: str,
+        project_id: str,
         page: typing.Optional[int] = None,
         size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._export_datapoints_mapped_args(
-            id=id,
+        args = self._list_mapped_args(
+            project_id=project_id,
             page=page,
             size=size,
         )
-        return self._export_datapoints_oapg(
+        return self._list_oapg(
             query_params=args.query,
-            path_params=args.path,
         )
 
-class ApiForpost(BaseApi):
+class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    async def apost(
+    async def aget(
         self,
-        id: str,
+        project_id: str,
         page: typing.Optional[int] = None,
         size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._export_datapoints_mapped_args(
-            id=id,
+        args = self._list_mapped_args(
+            project_id=project_id,
             page=page,
             size=size,
         )
-        return await self._aexport_datapoints_oapg(
+        return await self._alist_oapg(
             query_params=args.query,
-            path_params=args.path,
         )
     
-    def post(
+    def get(
         self,
-        id: str,
+        project_id: str,
         page: typing.Optional[int] = None,
         size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._export_datapoints_mapped_args(
-            id=id,
+        args = self._list_mapped_args(
+            project_id=project_id,
             page=page,
             size=size,
         )
-        return self._export_datapoints_oapg(
+        return self._list_oapg(
             query_params=args.query,
-            path_params=args.path,
         )
```

### Comparing `humanloop-0.4.2/humanloop/paths/projects_id_export/post.pyi` & `humanloop-0.4.3/humanloop/paths/projects_id_feedback_types/patch.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,54 +26,24 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
+from humanloop.model.projects_update_feedback_types_request import ProjectsUpdateFeedbackTypesRequest as ProjectsUpdateFeedbackTypesRequestSchema
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
-from humanloop.model.paginated_data_log_response import PaginatedDataLogResponse as PaginatedDataLogResponseSchema
+from humanloop.model.feedback_types import FeedbackTypes as FeedbackTypesSchema
 
-from humanloop.type.paginated_data_log_response import PaginatedDataLogResponse
+from humanloop.type.projects_update_feedback_types_request import ProjectsUpdateFeedbackTypesRequest
+from humanloop.type.feedback_types import FeedbackTypes
 from humanloop.type.http_validation_error import HTTPValidationError
 
-# Query params
-PageSchema = schemas.IntSchema
-SizeSchema = schemas.IntSchema
-RequestRequiredQueryParams = typing_extensions.TypedDict(
-    'RequestRequiredQueryParams',
-    {
-    }
-)
-RequestOptionalQueryParams = typing_extensions.TypedDict(
-    'RequestOptionalQueryParams',
-    {
-        'page': typing.Union[PageSchema, decimal.Decimal, int, ],
-        'size': typing.Union[SizeSchema, decimal.Decimal, int, ],
-    },
-    total=False
-)
-
+from . import path
 
-class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
-    pass
-
-
-request_query_page = api_client.QueryParameter(
-    name="page",
-    style=api_client.ParameterStyle.FORM,
-    schema=PageSchema,
-    explode=True,
-)
-request_query_size = api_client.QueryParameter(
-    name="size",
-    style=api_client.ParameterStyle.FORM,
-    schema=SizeSchema,
-    explode=True,
-)
 # Path params
 IdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
         'id': typing.Union[IdSchema, str, ],
     }
@@ -92,25 +62,39 @@
 
 request_path_id = api_client.PathParameter(
     name="id",
     style=api_client.ParameterStyle.SIMPLE,
     schema=IdSchema,
     required=True,
 )
-SchemaFor200ResponseBodyApplicationJson = PaginatedDataLogResponseSchema
+# body param
+SchemaForRequestBodyApplicationJson = ProjectsUpdateFeedbackTypesRequestSchema
+
+
+request_body_projects_update_feedback_types_request = api_client.RequestBody(
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaForRequestBodyApplicationJson),
+    },
+    required=True,
+)
+_auth = [
+    'APIKeyHeader',
+]
+SchemaFor200ResponseBodyApplicationJson = FeedbackTypesSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: PaginatedDataLogResponse
+    body: FeedbackTypes
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: PaginatedDataLogResponse
+    body: FeedbackTypes
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -134,60 +118,59 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
+_status_code_to_response = {
+    '200': _response_for_200,
+    '422': _response_for_422,
+}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
-    def _export_datapoints_mapped_args(
+    def _update_feedback_types_mapped_args(
         self,
+        body: ProjectsUpdateFeedbackTypesRequest,
         id: str,
-        page: typing.Optional[int] = None,
-        size: typing.Optional[int] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
-        _query_params = {}
         _path_params = {}
-        if page is not None:
-            _query_params["page"] = page
-        if size is not None:
-            _query_params["size"] = size
+        _body = {}
+        args.body = body if body is not None else _body
         if id is not None:
             _path_params["id"] = id
-        args.query = _query_params
         args.path = _path_params
         return args
 
-    async def _aexport_datapoints_oapg(
+    async def _aupdate_feedback_types_oapg(
         self,
-            query_params: typing.Optional[dict] = {},
+        body: typing.Any = None,
             path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'application/json',
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        Export Datapoints
+        Update Feedback Types
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
-        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
         _path_params = {}
         for parameter in (
             request_path_id,
         ):
@@ -196,40 +179,39 @@
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _path_params.update(serialized_data)
     
         for k, v in _path_params.items():
             used_path = used_path.replace('{%s}' % k, v)
     
-        prefix_separator_iterator = None
-        for parameter in (
-            request_query_page,
-            request_query_size,
-        ):
-            parameter_data = query_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            if prefix_separator_iterator is None:
-                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
-            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
-            for serialized_value in serialized_data.values():
-                used_path += serialized_value
-    
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
     
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
+        _fields = None
+        _body = None
+        serialized_data = request_body_projects_update_feedback_types_request.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']    
         response = await self.api_client.async_call_api(
             resource_path=used_path,
-            method='post'.upper(),
+            method='patch'.upper(),
             headers=_headers,
+            fields=_fields,
+            serialized_body=_body,
+            body=body,
             auth_settings=_auth,
-            prefix_separator_iterator=prefix_separator_iterator,
             timeout=timeout,
         )
         
         if stream:
             async def stream_iterator():
                 """
                 iterates over response.http_response.content and closes connection once iteration has finished
@@ -270,33 +252,33 @@
     
         # cleanup session / response
         response.http_response.close()
         await response.session.close()
     
         return api_response
 
-    def _export_datapoints_oapg(
+    def _update_feedback_types_oapg(
         self,
-            query_params: typing.Optional[dict] = {},
+        body: typing.Any = None,
             path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'application/json',
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        Export Datapoints
+        Update Feedback Types
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
-        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
         _path_params = {}
         for parameter in (
             request_path_id,
         ):
@@ -305,40 +287,39 @@
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _path_params.update(serialized_data)
     
         for k, v in _path_params.items():
             used_path = used_path.replace('{%s}' % k, v)
     
-        prefix_separator_iterator = None
-        for parameter in (
-            request_query_page,
-            request_query_size,
-        ):
-            parameter_data = query_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            if prefix_separator_iterator is None:
-                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
-            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
-            for serialized_value in serialized_data.values():
-                used_path += serialized_value
-    
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
     
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
+        _fields = None
+        _body = None
+        serialized_data = request_body_projects_update_feedback_types_request.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']    
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='post'.upper(),
+            method='patch'.upper(),
             headers=_headers,
+            fields=_fields,
+            serialized_body=_body,
+            body=body,
             auth_settings=_auth,
-            prefix_separator_iterator=prefix_separator_iterator,
             timeout=timeout,
         )
     
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
         if response_for_status:
             api_response = response_for_status.deserialize(
                                                     response,
@@ -357,91 +338,83 @@
             )
     
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
     
         return api_response
 
-class ExportDatapoints(BaseApi):
+class UpdateFeedbackTypes(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    async def aexport_datapoints(
+    async def aupdate_feedback_types(
         self,
+        body: ProjectsUpdateFeedbackTypesRequest,
         id: str,
-        page: typing.Optional[int] = None,
-        size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._export_datapoints_mapped_args(
+        args = self._update_feedback_types_mapped_args(
+            body=body,
             id=id,
-            page=page,
-            size=size,
         )
-        return await self._aexport_datapoints_oapg(
-            query_params=args.query,
+        return await self._aupdate_feedback_types_oapg(
+            body=args.body,
             path_params=args.path,
         )
     
-    def export_datapoints(
+    def update_feedback_types(
         self,
+        body: ProjectsUpdateFeedbackTypesRequest,
         id: str,
-        page: typing.Optional[int] = None,
-        size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._export_datapoints_mapped_args(
+        args = self._update_feedback_types_mapped_args(
+            body=body,
             id=id,
-            page=page,
-            size=size,
         )
-        return self._export_datapoints_oapg(
-            query_params=args.query,
+        return self._update_feedback_types_oapg(
+            body=args.body,
             path_params=args.path,
         )
 
-class ApiForpost(BaseApi):
+class ApiForpatch(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    async def apost(
+    async def apatch(
         self,
+        body: ProjectsUpdateFeedbackTypesRequest,
         id: str,
-        page: typing.Optional[int] = None,
-        size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._export_datapoints_mapped_args(
+        args = self._update_feedback_types_mapped_args(
+            body=body,
             id=id,
-            page=page,
-            size=size,
         )
-        return await self._aexport_datapoints_oapg(
-            query_params=args.query,
+        return await self._aupdate_feedback_types_oapg(
+            body=args.body,
             path_params=args.path,
         )
     
-    def post(
+    def patch(
         self,
+        body: ProjectsUpdateFeedbackTypesRequest,
         id: str,
-        page: typing.Optional[int] = None,
-        size: typing.Optional[int] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._export_datapoints_mapped_args(
+        args = self._update_feedback_types_mapped_args(
+            body=body,
             id=id,
-            page=page,
-            size=size,
         )
-        return self._export_datapoints_oapg(
-            query_params=args.query,
+        return self._update_feedback_types_oapg(
+            body=args.body,
             path_params=args.path,
         )
```

### Comparing `humanloop-0.4.2/humanloop/paths/projects_id_feedback_types/patch.py` & `humanloop-0.4.3/humanloop/paths/projects_id_feedback_types/patch.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -28,20 +28,20 @@
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 from humanloop.model.projects_update_feedback_types_request import ProjectsUpdateFeedbackTypesRequest as ProjectsUpdateFeedbackTypesRequestSchema
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
+from humanloop.model.feedback_types import FeedbackTypes as FeedbackTypesSchema
 
 from humanloop.type.projects_update_feedback_types_request import ProjectsUpdateFeedbackTypesRequest
+from humanloop.type.feedback_types import FeedbackTypes
 from humanloop.type.http_validation_error import HTTPValidationError
 
-from . import path
-
 # Path params
 IdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
         'id': typing.Union[IdSchema, str, ],
     }
@@ -71,28 +71,25 @@
 request_body_projects_update_feedback_types_request = api_client.RequestBody(
     content={
         'application/json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
-_auth = [
-    'APIKeyHeader',
-]
-SchemaFor200ResponseBodyApplicationJson = schemas.DictSchema
+SchemaFor200ResponseBodyApplicationJson = FeedbackTypesSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
+    body: FeedbackTypes
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
+    body: FeedbackTypes
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -116,18 +113,14 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '422': _response_for_422,
-}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `humanloop-0.4.2/humanloop/paths/projects_id_feedback_types/patch.pyi` & `humanloop-0.4.3/humanloop/paths/projects_id_active_config/get.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
-from humanloop.model.projects_update_feedback_types_request import ProjectsUpdateFeedbackTypesRequest as ProjectsUpdateFeedbackTypesRequestSchema
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
+from humanloop.model.get_model_config_response import GetModelConfigResponse as GetModelConfigResponseSchema
 
-from humanloop.type.projects_update_feedback_types_request import ProjectsUpdateFeedbackTypesRequest
+from humanloop.type.get_model_config_response import GetModelConfigResponse
 from humanloop.type.http_validation_error import HTTPValidationError
 
 # Path params
 IdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
@@ -58,36 +58,25 @@
 
 request_path_id = api_client.PathParameter(
     name="id",
     style=api_client.ParameterStyle.SIMPLE,
     schema=IdSchema,
     required=True,
 )
-# body param
-SchemaForRequestBodyApplicationJson = ProjectsUpdateFeedbackTypesRequestSchema
-
-
-request_body_projects_update_feedback_types_request = api_client.RequestBody(
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaForRequestBodyApplicationJson),
-    },
-    required=True,
-)
-SchemaFor200ResponseBodyApplicationJson = schemas.DictSchema
+SchemaFor200ResponseBodyApplicationJson = GetModelConfigResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
+    body: GetModelConfigResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
+    body: GetModelConfigResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -118,44 +107,39 @@
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
-    def _update_feedback_types_mapped_args(
+    def _get_config_mapped_args(
         self,
-        body: ProjectsUpdateFeedbackTypesRequest,
         id: str,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _path_params = {}
-        _body = {}
-        args.body = body if body is not None else _body
         if id is not None:
             _path_params["id"] = id
         args.path = _path_params
         return args
 
-    async def _aupdate_feedback_types_oapg(
+    async def _aget_config_oapg(
         self,
-        body: typing.Any = None,
             path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        content_type: str = 'application/json',
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        Update Feedback Types
+        Get Active Config
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
@@ -174,32 +158,18 @@
     
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
     
-        if body is schemas.unset:
-            raise exceptions.ApiValueError(
-                'The required body parameter has an invalid value of: unset. Set a valid value instead')
-        _fields = None
-        _body = None
-        serialized_data = request_body_projects_update_feedback_types_request.serialize(body, content_type)
-        _headers.add('Content-Type', content_type)
-        if 'fields' in serialized_data:
-            _fields = serialized_data['fields']
-        elif 'body' in serialized_data:
-            _body = serialized_data['body']    
         response = await self.api_client.async_call_api(
             resource_path=used_path,
-            method='patch'.upper(),
+            method='get'.upper(),
             headers=_headers,
-            fields=_fields,
-            serialized_body=_body,
-            body=body,
             auth_settings=_auth,
             timeout=timeout,
         )
         
         if stream:
             async def stream_iterator():
                 """
@@ -241,29 +211,27 @@
     
         # cleanup session / response
         response.http_response.close()
         await response.session.close()
     
         return api_response
 
-    def _update_feedback_types_oapg(
+    def _get_config_oapg(
         self,
-        body: typing.Any = None,
             path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        content_type: str = 'application/json',
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        Update Feedback Types
+        Get Active Config
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
@@ -282,32 +250,18 @@
     
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
     
-        if body is schemas.unset:
-            raise exceptions.ApiValueError(
-                'The required body parameter has an invalid value of: unset. Set a valid value instead')
-        _fields = None
-        _body = None
-        serialized_data = request_body_projects_update_feedback_types_request.serialize(body, content_type)
-        _headers.add('Content-Type', content_type)
-        if 'fields' in serialized_data:
-            _fields = serialized_data['fields']
-        elif 'body' in serialized_data:
-            _body = serialized_data['body']    
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='patch'.upper(),
+            method='get'.upper(),
             headers=_headers,
-            fields=_fields,
-            serialized_body=_body,
-            body=body,
             auth_settings=_auth,
             timeout=timeout,
         )
     
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
         if response_for_status:
             api_response = response_for_status.deserialize(
@@ -327,83 +281,71 @@
             )
     
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
     
         return api_response
 
-class UpdateFeedbackTypes(BaseApi):
+class GetConfig(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    async def aupdate_feedback_types(
+    async def aget_config(
         self,
-        body: ProjectsUpdateFeedbackTypesRequest,
         id: str,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._update_feedback_types_mapped_args(
-            body=body,
+        args = self._get_config_mapped_args(
             id=id,
         )
-        return await self._aupdate_feedback_types_oapg(
-            body=args.body,
+        return await self._aget_config_oapg(
             path_params=args.path,
         )
     
-    def update_feedback_types(
+    def get_config(
         self,
-        body: ProjectsUpdateFeedbackTypesRequest,
         id: str,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._update_feedback_types_mapped_args(
-            body=body,
+        args = self._get_config_mapped_args(
             id=id,
         )
-        return self._update_feedback_types_oapg(
-            body=args.body,
+        return self._get_config_oapg(
             path_params=args.path,
         )
 
-class ApiForpatch(BaseApi):
+class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    async def apatch(
+    async def aget(
         self,
-        body: ProjectsUpdateFeedbackTypesRequest,
         id: str,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._update_feedback_types_mapped_args(
-            body=body,
+        args = self._get_config_mapped_args(
             id=id,
         )
-        return await self._aupdate_feedback_types_oapg(
-            body=args.body,
+        return await self._aget_config_oapg(
             path_params=args.path,
         )
     
-    def patch(
+    def get(
         self,
-        body: ProjectsUpdateFeedbackTypesRequest,
         id: str,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._update_feedback_types_mapped_args(
-            body=body,
+        args = self._get_config_mapped_args(
             id=id,
         )
-        return self._update_feedback_types_oapg(
-            body=args.body,
+        return self._get_config_oapg(
             path_params=args.path,
         )
```

### Comparing `humanloop-0.4.2/humanloop/paths/projects_id_model_config/get.py` & `humanloop-0.4.3/humanloop/paths/projects_id_configs/get.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
-from humanloop.model.get_model_config_response import GetModelConfigResponse as GetModelConfigResponseSchema
+from humanloop.model.projects_get_configs_response import ProjectsGetConfigsResponse as ProjectsGetConfigsResponseSchema
 
-from humanloop.type.get_model_config_response import GetModelConfigResponse
+from humanloop.type.projects_get_configs_response import ProjectsGetConfigsResponse
 from humanloop.type.http_validation_error import HTTPValidationError
 
 from . import path
 
 # Path params
 IdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
@@ -63,25 +63,25 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=IdSchema,
     required=True,
 )
 _auth = [
     'APIKeyHeader',
 ]
-SchemaFor200ResponseBodyApplicationJson = GetModelConfigResponseSchema
+SchemaFor200ResponseBodyApplicationJson = ProjectsGetConfigsResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: GetModelConfigResponse
+    body: ProjectsGetConfigsResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: GetModelConfigResponse
+    body: ProjectsGetConfigsResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -116,39 +116,39 @@
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
-    def _get_model_config_mapped_args(
+    def _get_configs_mapped_args(
         self,
         id: str,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _path_params = {}
         if id is not None:
             _path_params["id"] = id
         args.path = _path_params
         return args
 
-    async def _aget_model_config_oapg(
+    async def _aget_configs_oapg(
         self,
             path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        Get Model Config
+        Get Configs
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
@@ -220,27 +220,27 @@
     
         # cleanup session / response
         response.http_response.close()
         await response.session.close()
     
         return api_response
 
-    def _get_model_config_oapg(
+    def _get_configs_oapg(
         self,
             path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        Get Model Config
+        Get Configs
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
@@ -290,71 +290,71 @@
             )
     
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
     
         return api_response
 
-class GetModelConfig(BaseApi):
+class GetConfigs(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    async def aget_model_config(
+    async def aget_configs(
         self,
         id: str,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._get_model_config_mapped_args(
+        args = self._get_configs_mapped_args(
             id=id,
         )
-        return await self._aget_model_config_oapg(
+        return await self._aget_configs_oapg(
             path_params=args.path,
         )
     
-    def get_model_config(
+    def get_configs(
         self,
         id: str,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._get_model_config_mapped_args(
+        args = self._get_configs_mapped_args(
             id=id,
         )
-        return self._get_model_config_oapg(
+        return self._get_configs_oapg(
             path_params=args.path,
         )
 
 class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     async def aget(
         self,
         id: str,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._get_model_config_mapped_args(
+        args = self._get_configs_mapped_args(
             id=id,
         )
-        return await self._aget_model_config_oapg(
+        return await self._aget_configs_oapg(
             path_params=args.path,
         )
     
     def get(
         self,
         id: str,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._get_model_config_mapped_args(
+        args = self._get_configs_mapped_args(
             id=id,
         )
-        return self._get_model_config_oapg(
+        return self._get_configs_oapg(
             path_params=args.path,
         )
```

### Comparing `humanloop-0.4.2/humanloop/paths/projects_id_model_config/get.pyi` & `humanloop-0.4.3/humanloop/paths/projects_id_configs/get.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
-from humanloop.model.get_model_config_response import GetModelConfigResponse as GetModelConfigResponseSchema
+from humanloop.model.projects_get_configs_response import ProjectsGetConfigsResponse as ProjectsGetConfigsResponseSchema
 
-from humanloop.type.get_model_config_response import GetModelConfigResponse
+from humanloop.type.projects_get_configs_response import ProjectsGetConfigsResponse
 from humanloop.type.http_validation_error import HTTPValidationError
 
 # Path params
 IdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
@@ -58,25 +58,25 @@
 
 request_path_id = api_client.PathParameter(
     name="id",
     style=api_client.ParameterStyle.SIMPLE,
     schema=IdSchema,
     required=True,
 )
-SchemaFor200ResponseBodyApplicationJson = GetModelConfigResponseSchema
+SchemaFor200ResponseBodyApplicationJson = ProjectsGetConfigsResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: GetModelConfigResponse
+    body: ProjectsGetConfigsResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: GetModelConfigResponse
+    body: ProjectsGetConfigsResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -107,39 +107,39 @@
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
-    def _get_model_config_mapped_args(
+    def _get_configs_mapped_args(
         self,
         id: str,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _path_params = {}
         if id is not None:
             _path_params["id"] = id
         args.path = _path_params
         return args
 
-    async def _aget_model_config_oapg(
+    async def _aget_configs_oapg(
         self,
             path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        Get Model Config
+        Get Configs
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
@@ -211,27 +211,27 @@
     
         # cleanup session / response
         response.http_response.close()
         await response.session.close()
     
         return api_response
 
-    def _get_model_config_oapg(
+    def _get_configs_oapg(
         self,
             path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        Get Model Config
+        Get Configs
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
@@ -281,71 +281,71 @@
             )
     
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
     
         return api_response
 
-class GetModelConfig(BaseApi):
+class GetConfigs(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    async def aget_model_config(
+    async def aget_configs(
         self,
         id: str,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._get_model_config_mapped_args(
+        args = self._get_configs_mapped_args(
             id=id,
         )
-        return await self._aget_model_config_oapg(
+        return await self._aget_configs_oapg(
             path_params=args.path,
         )
     
-    def get_model_config(
+    def get_configs(
         self,
         id: str,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._get_model_config_mapped_args(
+        args = self._get_configs_mapped_args(
             id=id,
         )
-        return self._get_model_config_oapg(
+        return self._get_configs_oapg(
             path_params=args.path,
         )
 
 class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     async def aget(
         self,
         id: str,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._get_model_config_mapped_args(
+        args = self._get_configs_mapped_args(
             id=id,
         )
-        return await self._aget_model_config_oapg(
+        return await self._aget_configs_oapg(
             path_params=args.path,
         )
     
     def get(
         self,
         id: str,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._get_model_config_mapped_args(
+        args = self._get_configs_mapped_args(
             id=id,
         )
-        return self._get_model_config_oapg(
+        return self._get_configs_oapg(
             path_params=args.path,
         )
```

### Comparing `humanloop-0.4.2/humanloop/paths/projects_id_model_configs/get.py` & `humanloop-0.4.3/humanloop/paths/projects_project_id_experiments/get.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,62 +26,62 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
-from humanloop.model.projects_get_model_configs_response import ProjectsGetModelConfigsResponse as ProjectsGetModelConfigsResponseSchema
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
+from humanloop.model.experiments_list_response import ExperimentsListResponse as ExperimentsListResponseSchema
 
-from humanloop.type.projects_get_model_configs_response import ProjectsGetModelConfigsResponse
+from humanloop.type.experiments_list_response import ExperimentsListResponse
 from humanloop.type.http_validation_error import HTTPValidationError
 
 from . import path
 
 # Path params
-IdSchema = schemas.StrSchema
+ProjectIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
-        'id': typing.Union[IdSchema, str, ],
+        'project_id': typing.Union[ProjectIdSchema, str, ],
     }
 )
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams',
     {
     },
     total=False
 )
 
 
 class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
     pass
 
 
-request_path_id = api_client.PathParameter(
-    name="id",
+request_path_project_id = api_client.PathParameter(
+    name="project_id",
     style=api_client.ParameterStyle.SIMPLE,
-    schema=IdSchema,
+    schema=ProjectIdSchema,
     required=True,
 )
 _auth = [
     'APIKeyHeader',
 ]
-SchemaFor200ResponseBodyApplicationJson = ProjectsGetModelConfigsResponseSchema
+SchemaFor200ResponseBodyApplicationJson = ExperimentsListResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: ProjectsGetModelConfigsResponse
+    body: ExperimentsListResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: ProjectsGetModelConfigsResponse
+    body: ExperimentsListResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -116,49 +116,49 @@
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
-    def _get_model_configs_mapped_args(
+    def _list_mapped_args(
         self,
-        id: str,
+        project_id: str,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _path_params = {}
-        if id is not None:
-            _path_params["id"] = id
+        if project_id is not None:
+            _path_params["project_id"] = project_id
         args.path = _path_params
         return args
 
-    async def _aget_model_configs_oapg(
+    async def _alist_oapg(
         self,
             path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        Get Model Configs
+        Get Experiments
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
         _path_params = {}
         for parameter in (
-            request_path_id,
+            request_path_project_id,
         ):
             parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _path_params.update(serialized_data)
     
@@ -220,37 +220,37 @@
     
         # cleanup session / response
         response.http_response.close()
         await response.session.close()
     
         return api_response
 
-    def _get_model_configs_oapg(
+    def _list_oapg(
         self,
             path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        Get Model Configs
+        Get Experiments
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
         _path_params = {}
         for parameter in (
-            request_path_id,
+            request_path_project_id,
         ):
             parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _path_params.update(serialized_data)
     
@@ -290,71 +290,71 @@
             )
     
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
     
         return api_response
 
-class GetModelConfigs(BaseApi):
+class List(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    async def aget_model_configs(
+    async def alist(
         self,
-        id: str,
+        project_id: str,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._get_model_configs_mapped_args(
-            id=id,
+        args = self._list_mapped_args(
+            project_id=project_id,
         )
-        return await self._aget_model_configs_oapg(
+        return await self._alist_oapg(
             path_params=args.path,
         )
     
-    def get_model_configs(
+    def list(
         self,
-        id: str,
+        project_id: str,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._get_model_configs_mapped_args(
-            id=id,
+        args = self._list_mapped_args(
+            project_id=project_id,
         )
-        return self._get_model_configs_oapg(
+        return self._list_oapg(
             path_params=args.path,
         )
 
 class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     async def aget(
         self,
-        id: str,
+        project_id: str,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._get_model_configs_mapped_args(
-            id=id,
+        args = self._list_mapped_args(
+            project_id=project_id,
         )
-        return await self._aget_model_configs_oapg(
+        return await self._alist_oapg(
             path_params=args.path,
         )
     
     def get(
         self,
-        id: str,
+        project_id: str,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._get_model_configs_mapped_args(
-            id=id,
+        args = self._list_mapped_args(
+            project_id=project_id,
         )
-        return self._get_model_configs_oapg(
+        return self._list_oapg(
             path_params=args.path,
         )
```

### Comparing `humanloop-0.4.2/humanloop/paths/projects_id_model_configs/get.pyi` & `humanloop-0.4.3/humanloop/paths/projects_project_id_experiments/get.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -26,57 +26,57 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
-from humanloop.model.projects_get_model_configs_response import ProjectsGetModelConfigsResponse as ProjectsGetModelConfigsResponseSchema
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
+from humanloop.model.experiments_list_response import ExperimentsListResponse as ExperimentsListResponseSchema
 
-from humanloop.type.projects_get_model_configs_response import ProjectsGetModelConfigsResponse
+from humanloop.type.experiments_list_response import ExperimentsListResponse
 from humanloop.type.http_validation_error import HTTPValidationError
 
 # Path params
-IdSchema = schemas.StrSchema
+ProjectIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
-        'id': typing.Union[IdSchema, str, ],
+        'project_id': typing.Union[ProjectIdSchema, str, ],
     }
 )
 RequestOptionalPathParams = typing_extensions.TypedDict(
     'RequestOptionalPathParams',
     {
     },
     total=False
 )
 
 
 class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
     pass
 
 
-request_path_id = api_client.PathParameter(
-    name="id",
+request_path_project_id = api_client.PathParameter(
+    name="project_id",
     style=api_client.ParameterStyle.SIMPLE,
-    schema=IdSchema,
+    schema=ProjectIdSchema,
     required=True,
 )
-SchemaFor200ResponseBodyApplicationJson = ProjectsGetModelConfigsResponseSchema
+SchemaFor200ResponseBodyApplicationJson = ExperimentsListResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: ProjectsGetModelConfigsResponse
+    body: ExperimentsListResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: ProjectsGetModelConfigsResponse
+    body: ExperimentsListResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -107,49 +107,49 @@
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
-    def _get_model_configs_mapped_args(
+    def _list_mapped_args(
         self,
-        id: str,
+        project_id: str,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _path_params = {}
-        if id is not None:
-            _path_params["id"] = id
+        if project_id is not None:
+            _path_params["project_id"] = project_id
         args.path = _path_params
         return args
 
-    async def _aget_model_configs_oapg(
+    async def _alist_oapg(
         self,
             path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        Get Model Configs
+        Get Experiments
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
         _path_params = {}
         for parameter in (
-            request_path_id,
+            request_path_project_id,
         ):
             parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _path_params.update(serialized_data)
     
@@ -211,37 +211,37 @@
     
         # cleanup session / response
         response.http_response.close()
         await response.session.close()
     
         return api_response
 
-    def _get_model_configs_oapg(
+    def _list_oapg(
         self,
             path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        Get Model Configs
+        Get Experiments
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
         _path_params = {}
         for parameter in (
-            request_path_id,
+            request_path_project_id,
         ):
             parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _path_params.update(serialized_data)
     
@@ -281,71 +281,71 @@
             )
     
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
     
         return api_response
 
-class GetModelConfigs(BaseApi):
+class List(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    async def aget_model_configs(
+    async def alist(
         self,
-        id: str,
+        project_id: str,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._get_model_configs_mapped_args(
-            id=id,
+        args = self._list_mapped_args(
+            project_id=project_id,
         )
-        return await self._aget_model_configs_oapg(
+        return await self._alist_oapg(
             path_params=args.path,
         )
     
-    def get_model_configs(
+    def list(
         self,
-        id: str,
+        project_id: str,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._get_model_configs_mapped_args(
-            id=id,
+        args = self._list_mapped_args(
+            project_id=project_id,
         )
-        return self._get_model_configs_oapg(
+        return self._list_oapg(
             path_params=args.path,
         )
 
 class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     async def aget(
         self,
-        id: str,
+        project_id: str,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._get_model_configs_mapped_args(
-            id=id,
+        args = self._list_mapped_args(
+            project_id=project_id,
         )
-        return await self._aget_model_configs_oapg(
+        return await self._alist_oapg(
             path_params=args.path,
         )
     
     def get(
         self,
-        id: str,
+        project_id: str,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._get_model_configs_mapped_args(
-            id=id,
+        args = self._list_mapped_args(
+            project_id=project_id,
         )
-        return self._get_model_configs_oapg(
+        return self._list_oapg(
             path_params=args.path,
         )
```

### Comparing `humanloop-0.4.2/humanloop/paths/projects_project_id_experiments/get.py` & `humanloop-0.4.3/humanloop/paths/traces/post.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -26,62 +26,46 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
+from humanloop.model.create_trace_response import CreateTraceResponse as CreateTraceResponseSchema
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
-from humanloop.model.experiments_list_response import ExperimentsListResponse as ExperimentsListResponseSchema
+from humanloop.model.create_trace_request import CreateTraceRequest as CreateTraceRequestSchema
+from humanloop.model.trace_log_request import TraceLogRequest as TraceLogRequestSchema
 
-from humanloop.type.experiments_list_response import ExperimentsListResponse
+from humanloop.type.trace_log_request import TraceLogRequest
+from humanloop.type.create_trace_response import CreateTraceResponse
+from humanloop.type.create_trace_request import CreateTraceRequest
 from humanloop.type.http_validation_error import HTTPValidationError
 
-from . import path
-
-# Path params
-ProjectIdSchema = schemas.StrSchema
-RequestRequiredPathParams = typing_extensions.TypedDict(
-    'RequestRequiredPathParams',
-    {
-        'project_id': typing.Union[ProjectIdSchema, str, ],
-    }
-)
-RequestOptionalPathParams = typing_extensions.TypedDict(
-    'RequestOptionalPathParams',
-    {
-    },
-    total=False
-)
+# body param
+SchemaForRequestBodyApplicationJson = CreateTraceRequestSchema
 
 
-class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
-    pass
-
-
-request_path_project_id = api_client.PathParameter(
-    name="project_id",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=ProjectIdSchema,
+request_body_create_trace_request = api_client.RequestBody(
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaForRequestBodyApplicationJson),
+    },
     required=True,
 )
-_auth = [
-    'APIKeyHeader',
-]
-SchemaFor200ResponseBodyApplicationJson = ExperimentsListResponseSchema
+SchemaFor200ResponseBodyApplicationJson = CreateTraceResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: ExperimentsListResponse
+    body: CreateTraceResponse
 
 
 @dataclass
 class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: ExperimentsListResponse
+    body: CreateTraceResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
@@ -105,80 +89,77 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '422': _response_for_422,
-}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
-    def _list_mapped_args(
+    def _create_mapped_args(
         self,
-        project_id: str,
+        logs: typing.List[TraceLogRequest],
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
-        _path_params = {}
-        if project_id is not None:
-            _path_params["project_id"] = project_id
-        args.path = _path_params
+        _body = {}
+        if logs is not None:
+            _body["logs"] = logs
+        args.body = _body
         return args
 
-    async def _alist_oapg(
+    async def _acreate_oapg(
         self,
-            path_params: typing.Optional[dict] = {},
+        body: typing.Any = None,
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'application/json',
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        Get Experiments
+        Create Trace
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
-        self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
-        _path_params = {}
-        for parameter in (
-            request_path_project_id,
-        ):
-            parameter_data = path_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            serialized_data = parameter.serialize(parameter_data)
-            _path_params.update(serialized_data)
-    
-        for k, v in _path_params.items():
-            used_path = used_path.replace('{%s}' % k, v)
-    
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
     
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
+        _fields = None
+        _body = None
+        serialized_data = request_body_create_trace_request.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']    
         response = await self.api_client.async_call_api(
             resource_path=used_path,
-            method='get'.upper(),
+            method='post'.upper(),
             headers=_headers,
+            fields=_fields,
+            serialized_body=_body,
+            body=body,
             auth_settings=_auth,
             timeout=timeout,
         )
         
         if stream:
             async def stream_iterator():
                 """
@@ -220,57 +201,58 @@
     
         # cleanup session / response
         response.http_response.close()
         await response.session.close()
     
         return api_response
 
-    def _list_oapg(
+    def _create_oapg(
         self,
-            path_params: typing.Optional[dict] = {},
+        body: typing.Any = None,
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'application/json',
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        Get Experiments
+        Create Trace
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
-        self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
-        _path_params = {}
-        for parameter in (
-            request_path_project_id,
-        ):
-            parameter_data = path_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            serialized_data = parameter.serialize(parameter_data)
-            _path_params.update(serialized_data)
-    
-        for k, v in _path_params.items():
-            used_path = used_path.replace('{%s}' % k, v)
-    
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
     
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
+        _fields = None
+        _body = None
+        serialized_data = request_body_create_trace_request.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']    
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='get'.upper(),
+            method='post'.upper(),
             headers=_headers,
+            fields=_fields,
+            serialized_body=_body,
+            body=body,
             auth_settings=_auth,
             timeout=timeout,
         )
     
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
         if response_for_status:
             api_response = response_for_status.deserialize(
@@ -290,71 +272,71 @@
             )
     
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
     
         return api_response
 
-class List(BaseApi):
+class Create(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    async def alist(
+    async def acreate(
         self,
-        project_id: str,
+        logs: typing.List[TraceLogRequest],
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._list_mapped_args(
-            project_id=project_id,
+        args = self._create_mapped_args(
+            logs=logs,
         )
-        return await self._alist_oapg(
-            path_params=args.path,
+        return await self._acreate_oapg(
+            body=args.body,
         )
     
-    def list(
+    def create(
         self,
-        project_id: str,
+        logs: typing.List[TraceLogRequest],
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._list_mapped_args(
-            project_id=project_id,
+        args = self._create_mapped_args(
+            logs=logs,
         )
-        return self._list_oapg(
-            path_params=args.path,
+        return self._create_oapg(
+            body=args.body,
         )
 
-class ApiForget(BaseApi):
+class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    async def aget(
+    async def apost(
         self,
-        project_id: str,
+        logs: typing.List[TraceLogRequest],
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._list_mapped_args(
-            project_id=project_id,
+        args = self._create_mapped_args(
+            logs=logs,
         )
-        return await self._alist_oapg(
-            path_params=args.path,
+        return await self._acreate_oapg(
+            body=args.body,
         )
     
-    def get(
+    def post(
         self,
-        project_id: str,
+        logs: typing.List[TraceLogRequest],
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._list_mapped_args(
-            project_id=project_id,
+        args = self._create_mapped_args(
+            logs=logs,
         )
-        return self._list_oapg(
-            path_params=args.path,
+        return self._create_oapg(
+            body=args.body,
         )
```

### Comparing `humanloop-0.4.2/humanloop/paths/projects_project_id_experiments/get.pyi` & `humanloop-0.4.3/humanloop/paths/sessions/post.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -26,149 +26,80 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
-from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
-from humanloop.model.experiments_list_response import ExperimentsListResponse as ExperimentsListResponseSchema
+from humanloop.model.create_session_response import CreateSessionResponse as CreateSessionResponseSchema
 
-from humanloop.type.experiments_list_response import ExperimentsListResponse
-from humanloop.type.http_validation_error import HTTPValidationError
-
-# Path params
-ProjectIdSchema = schemas.StrSchema
-RequestRequiredPathParams = typing_extensions.TypedDict(
-    'RequestRequiredPathParams',
-    {
-        'project_id': typing.Union[ProjectIdSchema, str, ],
-    }
-)
-RequestOptionalPathParams = typing_extensions.TypedDict(
-    'RequestOptionalPathParams',
-    {
-    },
-    total=False
-)
-
-
-class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
-    pass
-
-
-request_path_project_id = api_client.PathParameter(
-    name="project_id",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=ProjectIdSchema,
-    required=True,
-)
-SchemaFor200ResponseBodyApplicationJson = ExperimentsListResponseSchema
-
-
-@dataclass
-class ApiResponseFor200(api_client.ApiResponse):
-    body: ExperimentsListResponse
+from humanloop.type.create_session_response import CreateSessionResponse
 
-
-@dataclass
-class ApiResponseFor200Async(api_client.AsyncApiResponse):
-    body: ExperimentsListResponse
-
-
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
-    response_cls_async=ApiResponseFor200Async,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
-    },
-)
-SchemaFor422ResponseBodyApplicationJson = HTTPValidationErrorSchema
+SchemaFor201ResponseBodyApplicationJson = CreateSessionResponseSchema
 
 
 @dataclass
-class ApiResponseFor422(api_client.ApiResponse):
-    body: HTTPValidationError
+class ApiResponseFor201(api_client.ApiResponse):
+    body: CreateSessionResponse
 
 
 @dataclass
-class ApiResponseFor422Async(api_client.AsyncApiResponse):
-    body: HTTPValidationError
+class ApiResponseFor201Async(api_client.AsyncApiResponse):
+    body: CreateSessionResponse
 
 
-_response_for_422 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor422,
-    response_cls_async=ApiResponseFor422Async,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
+    response_cls_async=ApiResponseFor201Async,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor422ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
-    def _list_mapped_args(
+    def _create_mapped_args(
         self,
-        project_id: str,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
-        _path_params = {}
-        if project_id is not None:
-            _path_params["project_id"] = project_id
-        args.path = _path_params
         return args
 
-    async def _alist_oapg(
+    async def _acreate_oapg(
         self,
-            path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
-        ApiResponseFor200Async,
+        ApiResponseFor201Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        Get Experiments
+        Create Session
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
-        self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
-        _path_params = {}
-        for parameter in (
-            request_path_project_id,
-        ):
-            parameter_data = path_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            serialized_data = parameter.serialize(parameter_data)
-            _path_params.update(serialized_data)
-    
-        for k, v in _path_params.items():
-            used_path = used_path.replace('{%s}' % k, v)
-    
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
     
         response = await self.api_client.async_call_api(
             resource_path=used_path,
-            method='get'.upper(),
+            method='post'.upper(),
             headers=_headers,
             auth_settings=_auth,
             timeout=timeout,
         )
         
         if stream:
             async def stream_iterator():
@@ -211,56 +142,41 @@
     
         # cleanup session / response
         response.http_response.close()
         await response.session.close()
     
         return api_response
 
-    def _list_oapg(
+    def _create_oapg(
         self,
-            path_params: typing.Optional[dict] = {},
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
     ) -> typing.Union[
-        ApiResponseFor200,
+        ApiResponseFor201,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        Get Experiments
+        Create Session
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
-        self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
     
-        _path_params = {}
-        for parameter in (
-            request_path_project_id,
-        ):
-            parameter_data = path_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            serialized_data = parameter.serialize(parameter_data)
-            _path_params.update(serialized_data)
-    
-        for k, v in _path_params.items():
-            used_path = used_path.replace('{%s}' % k, v)
-    
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
     
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='get'.upper(),
+            method='post'.upper(),
             headers=_headers,
             auth_settings=_auth,
             timeout=timeout,
         )
     
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
         if response_for_status:
@@ -281,71 +197,59 @@
             )
     
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
     
         return api_response
 
-class List(BaseApi):
+class Create(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    async def alist(
+    async def acreate(
         self,
-        project_id: str,
     ) -> typing.Union[
-        ApiResponseFor200Async,
+        ApiResponseFor201Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._list_mapped_args(
-            project_id=project_id,
+        args = self._create_mapped_args(
         )
-        return await self._alist_oapg(
-            path_params=args.path,
+        return await self._acreate_oapg(
         )
     
-    def list(
+    def create(
         self,
-        project_id: str,
     ) -> typing.Union[
-        ApiResponseFor200,
+        ApiResponseFor201,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._list_mapped_args(
-            project_id=project_id,
+        args = self._create_mapped_args(
         )
-        return self._list_oapg(
-            path_params=args.path,
+        return self._create_oapg(
         )
 
-class ApiForget(BaseApi):
+class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    async def aget(
+    async def apost(
         self,
-        project_id: str,
     ) -> typing.Union[
-        ApiResponseFor200Async,
+        ApiResponseFor201Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
-        args = self._list_mapped_args(
-            project_id=project_id,
+        args = self._create_mapped_args(
         )
-        return await self._alist_oapg(
-            path_params=args.path,
+        return await self._acreate_oapg(
         )
     
-    def get(
+    def post(
         self,
-        project_id: str,
     ) -> typing.Union[
-        ApiResponseFor200,
+        ApiResponseFor201,
         api_client.ApiResponseWithoutDeserialization,
     ]:
-        args = self._list_mapped_args(
-            project_id=project_id,
+        args = self._create_mapped_args(
         )
-        return self._list_oapg(
-            path_params=args.path,
+        return self._create_oapg(
         )
```

### Comparing `humanloop-0.4.2/humanloop/paths/projects_project_id_experiments/post.py` & `humanloop-0.4.3/humanloop/paths/projects_project_id_experiments/post.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -36,16 +36,14 @@
 from humanloop.model.create_experiment_request import CreateExperimentRequest as CreateExperimentRequestSchema
 
 from humanloop.type.create_experiment_request import CreateExperimentRequest
 from humanloop.type.experiment_response import ExperimentResponse
 from humanloop.type.positive_label import PositiveLabel
 from humanloop.type.http_validation_error import HTTPValidationError
 
-from . import path
-
 # Path params
 ProjectIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
         'project_id': typing.Union[ProjectIdSchema, str, ],
     }
@@ -75,17 +73,14 @@
 request_body_create_experiment_request = api_client.RequestBody(
     content={
         'application/json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
-_auth = [
-    'APIKeyHeader',
-]
 SchemaFor200ResponseBodyApplicationJson = ExperimentResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     body: ExperimentResponse
 
@@ -120,40 +115,36 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '422': _response_for_422,
-}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
     def _create_mapped_args(
         self,
         name: str,
         positive_labels: typing.List[PositiveLabel],
         project_id: str,
-        model_config_ids: typing.Optional[typing.List[str]] = None,
+        config_ids: typing.Optional[typing.List[str]] = None,
         set_active: typing.Optional[bool] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _path_params = {}
         _body = {}
         if name is not None:
             _body["name"] = name
-        if model_config_ids is not None:
-            _body["model_config_ids"] = model_config_ids
+        if config_ids is not None:
+            _body["config_ids"] = config_ids
         if positive_labels is not None:
             _body["positive_labels"] = positive_labels
         if set_active is not None:
             _body["set_active"] = set_active
         args.body = _body
         if project_id is not None:
             _path_params["project_id"] = project_id
@@ -359,49 +350,49 @@
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     async def acreate(
         self,
         name: str,
         positive_labels: typing.List[PositiveLabel],
         project_id: str,
-        model_config_ids: typing.Optional[typing.List[str]] = None,
+        config_ids: typing.Optional[typing.List[str]] = None,
         set_active: typing.Optional[bool] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._create_mapped_args(
             name=name,
             positive_labels=positive_labels,
             project_id=project_id,
-            model_config_ids=model_config_ids,
+            config_ids=config_ids,
             set_active=set_active,
         )
         return await self._acreate_oapg(
             body=args.body,
             path_params=args.path,
         )
     
     def create(
         self,
         name: str,
         positive_labels: typing.List[PositiveLabel],
         project_id: str,
-        model_config_ids: typing.Optional[typing.List[str]] = None,
+        config_ids: typing.Optional[typing.List[str]] = None,
         set_active: typing.Optional[bool] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._create_mapped_args(
             name=name,
             positive_labels=positive_labels,
             project_id=project_id,
-            model_config_ids=model_config_ids,
+            config_ids=config_ids,
             set_active=set_active,
         )
         return self._create_oapg(
             body=args.body,
             path_params=args.path,
         )
 
@@ -409,49 +400,49 @@
     # this class is used by api classes that refer to endpoints by path and http method names
 
     async def apost(
         self,
         name: str,
         positive_labels: typing.List[PositiveLabel],
         project_id: str,
-        model_config_ids: typing.Optional[typing.List[str]] = None,
+        config_ids: typing.Optional[typing.List[str]] = None,
         set_active: typing.Optional[bool] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._create_mapped_args(
             name=name,
             positive_labels=positive_labels,
             project_id=project_id,
-            model_config_ids=model_config_ids,
+            config_ids=config_ids,
             set_active=set_active,
         )
         return await self._acreate_oapg(
             body=args.body,
             path_params=args.path,
         )
     
     def post(
         self,
         name: str,
         positive_labels: typing.List[PositiveLabel],
         project_id: str,
-        model_config_ids: typing.Optional[typing.List[str]] = None,
+        config_ids: typing.Optional[typing.List[str]] = None,
         set_active: typing.Optional[bool] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._create_mapped_args(
             name=name,
             positive_labels=positive_labels,
             project_id=project_id,
-            model_config_ids=model_config_ids,
+            config_ids=config_ids,
             set_active=set_active,
         )
         return self._create_oapg(
             body=args.body,
             path_params=args.path,
         )
```

### Comparing `humanloop-0.4.2/humanloop/paths/projects_project_id_experiments/post.pyi` & `humanloop-0.4.3/humanloop/paths/projects_project_id_experiments/post.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 from humanloop.model.create_experiment_request import CreateExperimentRequest as CreateExperimentRequestSchema
 
 from humanloop.type.create_experiment_request import CreateExperimentRequest
 from humanloop.type.experiment_response import ExperimentResponse
 from humanloop.type.positive_label import PositiveLabel
 from humanloop.type.http_validation_error import HTTPValidationError
 
+from . import path
+
 # Path params
 ProjectIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
     'RequestRequiredPathParams',
     {
         'project_id': typing.Union[ProjectIdSchema, str, ],
     }
@@ -73,14 +75,17 @@
 request_body_create_experiment_request = api_client.RequestBody(
     content={
         'application/json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
+_auth = [
+    'APIKeyHeader',
+]
 SchemaFor200ResponseBodyApplicationJson = ExperimentResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     body: ExperimentResponse
 
@@ -115,36 +120,40 @@
     response_cls=ApiResponseFor422,
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
+_status_code_to_response = {
+    '200': _response_for_200,
+    '422': _response_for_422,
+}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
     def _create_mapped_args(
         self,
         name: str,
         positive_labels: typing.List[PositiveLabel],
         project_id: str,
-        model_config_ids: typing.Optional[typing.List[str]] = None,
+        config_ids: typing.Optional[typing.List[str]] = None,
         set_active: typing.Optional[bool] = None,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _path_params = {}
         _body = {}
         if name is not None:
             _body["name"] = name
-        if model_config_ids is not None:
-            _body["model_config_ids"] = model_config_ids
+        if config_ids is not None:
+            _body["config_ids"] = config_ids
         if positive_labels is not None:
             _body["positive_labels"] = positive_labels
         if set_active is not None:
             _body["set_active"] = set_active
         args.body = _body
         if project_id is not None:
             _path_params["project_id"] = project_id
@@ -350,49 +359,49 @@
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     async def acreate(
         self,
         name: str,
         positive_labels: typing.List[PositiveLabel],
         project_id: str,
-        model_config_ids: typing.Optional[typing.List[str]] = None,
+        config_ids: typing.Optional[typing.List[str]] = None,
         set_active: typing.Optional[bool] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._create_mapped_args(
             name=name,
             positive_labels=positive_labels,
             project_id=project_id,
-            model_config_ids=model_config_ids,
+            config_ids=config_ids,
             set_active=set_active,
         )
         return await self._acreate_oapg(
             body=args.body,
             path_params=args.path,
         )
     
     def create(
         self,
         name: str,
         positive_labels: typing.List[PositiveLabel],
         project_id: str,
-        model_config_ids: typing.Optional[typing.List[str]] = None,
+        config_ids: typing.Optional[typing.List[str]] = None,
         set_active: typing.Optional[bool] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._create_mapped_args(
             name=name,
             positive_labels=positive_labels,
             project_id=project_id,
-            model_config_ids=model_config_ids,
+            config_ids=config_ids,
             set_active=set_active,
         )
         return self._create_oapg(
             body=args.body,
             path_params=args.path,
         )
 
@@ -400,49 +409,49 @@
     # this class is used by api classes that refer to endpoints by path and http method names
 
     async def apost(
         self,
         name: str,
         positive_labels: typing.List[PositiveLabel],
         project_id: str,
-        model_config_ids: typing.Optional[typing.List[str]] = None,
+        config_ids: typing.Optional[typing.List[str]] = None,
         set_active: typing.Optional[bool] = None,
     ) -> typing.Union[
         ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._create_mapped_args(
             name=name,
             positive_labels=positive_labels,
             project_id=project_id,
-            model_config_ids=model_config_ids,
+            config_ids=config_ids,
             set_active=set_active,
         )
         return await self._acreate_oapg(
             body=args.body,
             path_params=args.path,
         )
     
     def post(
         self,
         name: str,
         positive_labels: typing.List[PositiveLabel],
         project_id: str,
-        model_config_ids: typing.Optional[typing.List[str]] = None,
+        config_ids: typing.Optional[typing.List[str]] = None,
         set_active: typing.Optional[bool] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._create_mapped_args(
             name=name,
             positive_labels=positive_labels,
             project_id=project_id,
-            model_config_ids=model_config_ids,
+            config_ids=config_ids,
             set_active=set_active,
         )
         return self._create_oapg(
             body=args.body,
             path_params=args.path,
         )
```

### Comparing `humanloop-0.4.2/humanloop/paths/sessions/post.py` & `humanloop-0.4.3/humanloop/paths/traces/post.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,57 +26,59 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
+from humanloop.model.create_trace_response import CreateTraceResponse as CreateTraceResponseSchema
 from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
-from humanloop.model.session_response import SessionResponse as SessionResponseSchema
-from humanloop.model.create_session_request import CreateSessionRequest as CreateSessionRequestSchema
+from humanloop.model.create_trace_request import CreateTraceRequest as CreateTraceRequestSchema
+from humanloop.model.trace_log_request import TraceLogRequest as TraceLogRequestSchema
 
-from humanloop.type.create_session_request import CreateSessionRequest
-from humanloop.type.session_response import SessionResponse
+from humanloop.type.trace_log_request import TraceLogRequest
+from humanloop.type.create_trace_response import CreateTraceResponse
+from humanloop.type.create_trace_request import CreateTraceRequest
 from humanloop.type.http_validation_error import HTTPValidationError
 
 from . import path
 
 # body param
-SchemaForRequestBodyApplicationJson = CreateSessionRequestSchema
+SchemaForRequestBodyApplicationJson = CreateTraceRequestSchema
 
 
-request_body_create_session_request = api_client.RequestBody(
+request_body_create_trace_request = api_client.RequestBody(
     content={
         'application/json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'APIKeyHeader',
 ]
-SchemaFor201ResponseBodyApplicationJson = SessionResponseSchema
+SchemaFor200ResponseBodyApplicationJson = CreateTraceResponseSchema
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
-    body: SessionResponse
+class ApiResponseFor200(api_client.ApiResponse):
+    body: CreateTraceResponse
 
 
 @dataclass
-class ApiResponseFor201Async(api_client.AsyncApiResponse):
-    body: SessionResponse
+class ApiResponseFor200Async(api_client.AsyncApiResponse):
+    body: CreateTraceResponse
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
-    response_cls_async=ApiResponseFor201Async,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
+    response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor422ResponseBodyApplicationJson = HTTPValidationErrorSchema
 
 
 @dataclass
 class ApiResponseFor422(api_client.ApiResponse):
@@ -93,50 +95,50 @@
     response_cls_async=ApiResponseFor422Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '201': _response_for_201,
+    '200': _response_for_200,
     '422': _response_for_422,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
     def _create_mapped_args(
         self,
-        app: str,
+        logs: typing.List[TraceLogRequest],
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
         _body = {}
-        if app is not None:
-            _body["app"] = app
+        if logs is not None:
+            _body["logs"] = logs
         args.body = _body
         return args
 
     async def _acreate_oapg(
         self,
         body: typing.Any = None,
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         content_type: str = 'application/json',
         stream: bool = False,
     ) -> typing.Union[
-        ApiResponseFor201Async,
+        ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
-        Create Session
+        Create Trace
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
     
         _headers = HTTPHeaderDict()
@@ -146,15 +148,15 @@
                 _headers.add('Accept', accept_content_type)
     
         if body is schemas.unset:
             raise exceptions.ApiValueError(
                 'The required body parameter has an invalid value of: unset. Set a valid value instead')
         _fields = None
         _body = None
-        serialized_data = request_body_create_session_request.serialize(body, content_type)
+        serialized_data = request_body_create_trace_request.serialize(body, content_type)
         _headers.add('Content-Type', content_type)
         if 'fields' in serialized_data:
             _fields = serialized_data['fields']
         elif 'body' in serialized_data:
             _body = serialized_data['body']    
         response = await self.api_client.async_call_api(
             resource_path=used_path,
@@ -217,19 +219,19 @@
         body: typing.Any = None,
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         content_type: str = 'application/json',
         stream: bool = False,
     ) -> typing.Union[
-        ApiResponseFor201,
+        ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
-        Create Session
+        Create Trace
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
     
         _headers = HTTPHeaderDict()
@@ -239,15 +241,15 @@
                 _headers.add('Accept', accept_content_type)
     
         if body is schemas.unset:
             raise exceptions.ApiValueError(
                 'The required body parameter has an invalid value of: unset. Set a valid value instead')
         _fields = None
         _body = None
-        serialized_data = request_body_create_session_request.serialize(body, content_type)
+        serialized_data = request_body_create_trace_request.serialize(body, content_type)
         _headers.add('Content-Type', content_type)
         if 'fields' in serialized_data:
             _fields = serialized_data['fields']
         elif 'body' in serialized_data:
             _body = serialized_data['body']    
         response = self.api_client.call_api(
             resource_path=used_path,
@@ -284,66 +286,66 @@
         return api_response
 
 class Create(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     async def acreate(
         self,
-        app: str,
+        logs: typing.List[TraceLogRequest],
     ) -> typing.Union[
-        ApiResponseFor201Async,
+        ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._create_mapped_args(
-            app=app,
+            logs=logs,
         )
         return await self._acreate_oapg(
             body=args.body,
         )
     
     def create(
         self,
-        app: str,
+        logs: typing.List[TraceLogRequest],
     ) -> typing.Union[
-        ApiResponseFor201,
+        ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._create_mapped_args(
-            app=app,
+            logs=logs,
         )
         return self._create_oapg(
             body=args.body,
         )
 
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     async def apost(
         self,
-        app: str,
+        logs: typing.List[TraceLogRequest],
     ) -> typing.Union[
-        ApiResponseFor201Async,
+        ApiResponseFor200Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._create_mapped_args(
-            app=app,
+            logs=logs,
         )
         return await self._acreate_oapg(
             body=args.body,
         )
     
     def post(
         self,
-        app: str,
+        logs: typing.List[TraceLogRequest],
     ) -> typing.Union[
-        ApiResponseFor201,
+        ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._create_mapped_args(
-            app=app,
+            logs=logs,
         )
         return self._create_oapg(
             body=args.body,
         )
```

### Comparing `humanloop-0.4.2/humanloop/paths/sessions/post.pyi` & `humanloop-0.4.3/humanloop/paths/sessions/post.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,100 +26,65 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from humanloop import schemas  # noqa: F401
 
-from humanloop.model.http_validation_error import HTTPValidationError as HTTPValidationErrorSchema
-from humanloop.model.session_response import SessionResponse as SessionResponseSchema
-from humanloop.model.create_session_request import CreateSessionRequest as CreateSessionRequestSchema
+from humanloop.model.create_session_response import CreateSessionResponse as CreateSessionResponseSchema
 
-from humanloop.type.create_session_request import CreateSessionRequest
-from humanloop.type.session_response import SessionResponse
-from humanloop.type.http_validation_error import HTTPValidationError
+from humanloop.type.create_session_response import CreateSessionResponse
 
-# body param
-SchemaForRequestBodyApplicationJson = CreateSessionRequestSchema
+from . import path
 
-
-request_body_create_session_request = api_client.RequestBody(
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaForRequestBodyApplicationJson),
-    },
-    required=True,
-)
-SchemaFor201ResponseBodyApplicationJson = SessionResponseSchema
+_auth = [
+    'APIKeyHeader',
+]
+SchemaFor201ResponseBodyApplicationJson = CreateSessionResponseSchema
 
 
 @dataclass
 class ApiResponseFor201(api_client.ApiResponse):
-    body: SessionResponse
+    body: CreateSessionResponse
 
 
 @dataclass
 class ApiResponseFor201Async(api_client.AsyncApiResponse):
-    body: SessionResponse
+    body: CreateSessionResponse
 
 
 _response_for_201 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor201,
     response_cls_async=ApiResponseFor201Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor422ResponseBodyApplicationJson = HTTPValidationErrorSchema
-
-
-@dataclass
-class ApiResponseFor422(api_client.ApiResponse):
-    body: HTTPValidationError
-
-
-@dataclass
-class ApiResponseFor422Async(api_client.AsyncApiResponse):
-    body: HTTPValidationError
-
-
-_response_for_422 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor422,
-    response_cls_async=ApiResponseFor422Async,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor422ResponseBodyApplicationJson),
-    },
-)
+_status_code_to_response = {
+    '201': _response_for_201,
+}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
 
     def _create_mapped_args(
         self,
-        app: str,
     ) -> api_client.MappedArgs:
         args: api_client.MappedArgs = api_client.MappedArgs()
-        _body = {}
-        if app is not None:
-            _body["app"] = app
-        args.body = _body
         return args
 
     async def _acreate_oapg(
         self,
-        body: typing.Any = None,
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        content_type: str = 'application/json',
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor201Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         """
@@ -132,32 +97,18 @@
     
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
     
-        if body is schemas.unset:
-            raise exceptions.ApiValueError(
-                'The required body parameter has an invalid value of: unset. Set a valid value instead')
-        _fields = None
-        _body = None
-        serialized_data = request_body_create_session_request.serialize(body, content_type)
-        _headers.add('Content-Type', content_type)
-        if 'fields' in serialized_data:
-            _fields = serialized_data['fields']
-        elif 'body' in serialized_data:
-            _body = serialized_data['body']    
         response = await self.api_client.async_call_api(
             resource_path=used_path,
             method='post'.upper(),
             headers=_headers,
-            fields=_fields,
-            serialized_body=_body,
-            body=body,
             auth_settings=_auth,
             timeout=timeout,
         )
         
         if stream:
             async def stream_iterator():
                 """
@@ -201,19 +152,17 @@
         response.http_response.close()
         await response.session.close()
     
         return api_response
 
     def _create_oapg(
         self,
-        body: typing.Any = None,
         skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        content_type: str = 'application/json',
         stream: bool = False,
     ) -> typing.Union[
         ApiResponseFor201,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         """
         Create Session
@@ -225,32 +174,18 @@
     
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
     
-        if body is schemas.unset:
-            raise exceptions.ApiValueError(
-                'The required body parameter has an invalid value of: unset. Set a valid value instead')
-        _fields = None
-        _body = None
-        serialized_data = request_body_create_session_request.serialize(body, content_type)
-        _headers.add('Content-Type', content_type)
-        if 'fields' in serialized_data:
-            _fields = serialized_data['fields']
-        elif 'body' in serialized_data:
-            _body = serialized_data['body']    
         response = self.api_client.call_api(
             resource_path=used_path,
             method='post'.upper(),
             headers=_headers,
-            fields=_fields,
-            serialized_body=_body,
-            body=body,
             auth_settings=_auth,
             timeout=timeout,
         )
     
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
         if response_for_status:
             api_response = response_for_status.deserialize(
@@ -275,66 +210,54 @@
         return api_response
 
 class Create(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     async def acreate(
         self,
-        app: str,
     ) -> typing.Union[
         ApiResponseFor201Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._create_mapped_args(
-            app=app,
         )
         return await self._acreate_oapg(
-            body=args.body,
         )
     
     def create(
         self,
-        app: str,
     ) -> typing.Union[
         ApiResponseFor201,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._create_mapped_args(
-            app=app,
         )
         return self._create_oapg(
-            body=args.body,
         )
 
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     async def apost(
         self,
-        app: str,
     ) -> typing.Union[
         ApiResponseFor201Async,
         api_client.ApiResponseWithoutDeserializationAsync,
         AsyncGeneratorResponse,
     ]:
         args = self._create_mapped_args(
-            app=app,
         )
         return await self._acreate_oapg(
-            body=args.body,
         )
     
     def post(
         self,
-        app: str,
     ) -> typing.Union[
         ApiResponseFor201,
         api_client.ApiResponseWithoutDeserialization,
     ]:
         args = self._create_mapped_args(
-            app=app,
         )
         return self._create_oapg(
-            body=args.body,
         )
```

### Comparing `humanloop-0.4.2/humanloop/request_after_hook.py` & `humanloop-0.4.3/humanloop/request_after_hook.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/request_before_hook.py` & `humanloop-0.4.3/humanloop/request_before_hook.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/rest.py` & `humanloop-0.4.3/humanloop/rest.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/schemas.py` & `humanloop-0.4.3/humanloop/schemas.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/type/categorical_feedback_label.py` & `humanloop-0.4.3/humanloop/type/tool_result_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,21 +10,22 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
-from humanloop.type.label_sentiment import LabelSentiment
 
-RequiredCategoricalFeedbackLabel = TypedDict("RequiredCategoricalFeedbackLabel", {
-    "value": str,
+class RequiredToolResultResponse(TypedDict):
+    id: str
 
-    # Whether the feedback sentiment is positive or negative.
-    "sentiment": LabelSentiment,
-    })
+    name: str
 
-OptionalCategoricalFeedbackLabel = TypedDict("OptionalCategoricalFeedbackLabel", {
-    }, total=False)
+    signature: str
 
-class CategoricalFeedbackLabel(RequiredCategoricalFeedbackLabel, OptionalCategoricalFeedbackLabel):
+    result: str
+
+class OptionalToolResultResponse(TypedDict, total=False):
+    pass
+
+class ToolResultResponse(RequiredToolResultResponse, OptionalToolResultResponse):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/chat_data_response.py` & `humanloop-0.4.3/humanloop/type/model_config_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,42 +11,56 @@
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.chat_message import ChatMessage
-from humanloop.type.tool_result_response import ToolResultResponse
+from humanloop.type.model_endpoints import ModelEndpoints
+from humanloop.type.model_providers import ModelProviders
 
-RequiredChatDataResponse = TypedDict("RequiredChatDataResponse", {
-    # Unique ID for the model inputs and output logged to Humanloop. Use this when recording feedback later.
-    "id": str,
+class RequiredModelConfigResponse(TypedDict):
+    # What model instance to use for the generation. e.g. text-davinci-002.
+    model: str
 
-    # The index for the sampled generation for a given input. The num_samples request parameter controls how many samples are generated.
-    "index": int,
+    # Model config unique identifier generated by Humanloop.
+    id: str
 
-    # Output text returned from the provider model with leading and trailing whitespaces stripped.
-    "output": str,
+class OptionalModelConfigResponse(TypedDict, total=False):
+    # The company providing the underlying model service.
+    provider: ModelProviders
 
-    # Raw output text returned from the provider model.
-    "raw_output": str,
+    # Which of the providers model endpoints to use. For example Complete or Edit.
+    endpoint: ModelEndpoints
 
-    # The model configuration used to create the generation.
-    "model_config_id": str,
-    })
+    # Prompt template that will take your specified inputs to form your final request to the provider model. NB: Input variables within the prompt template should be specified with syntax: {{INPUT_NAME}}.
+    prompt_template: str
 
-OptionalChatDataResponse = TypedDict("OptionalChatDataResponse", {
-    # The inputs passed to the chat template.
-    "inputs": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    # Messages prepended to the list of messages sent to the provider. These messages that will take your specified inputs to form your final request to the provider model. NB: Input variables within the prompt template should be specified with syntax: {{INPUT_NAME}}.
+    chat_template: typing.List[ChatMessage]
 
-    # Why the completion ended. Usually one of 'stop' (indicating a stop token was encountered), or 'length' (indicating the max tokens limit has been reached). It will be set as null for the intermediary responses during a stream, and will only be set as non-null for the final streamed token.
-    "finish_reason": str,
+    # What sampling temperature to use when making a generation. Higher values means the model will be more creative.
+    temperature: typing.Union[int, float]
 
-    # Results of any tools run during the generation.
-    "tools": typing.List[ToolResultResponse],
+    # The maximum number of tokens to generate in the completion.
+    max_tokens: int
 
-    # The messages passed to the to provider chat endpoint.
-    "messages": typing.List[ChatMessage],
-    }, total=False)
+    # An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with top_p probability mass.
+    top_p: typing.Union[int, float]
 
-class ChatDataResponse(RequiredChatDataResponse, OptionalChatDataResponse):
+    # The string (or list of strings) after which the model will stop generating. The returned text will not contain the stop sequence.
+    stop: typing.Union[str, typing.List[str]]
+
+    # Number between -2.0 and 2.0. Positive values penalize new tokens based on whether they appear in the generation so far.
+    presence_penalty: typing.Union[int, float]
+
+    # Number between -2.0 and 2.0. Positive values penalize new tokens based on how frequently they appear in the generation so far.
+    frequency_penalty: typing.Union[int, float]
+
+    # Other parameter values to be passed to the provider call.
+    other: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
+
+    # A friendly display name for the model config.
+    display_name: str
+
+class ModelConfigResponse(RequiredModelConfigResponse, OptionalModelConfigResponse):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/chat_deployed_request.py` & `humanloop-0.4.3/humanloop/type/chat_deployed_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,40 +13,38 @@
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.chat_message import ChatMessage
 from humanloop.type.provider_api_keys import ProviderApiKeys
 
-RequiredChatDeployedRequest = TypedDict("RequiredChatDeployedRequest", {
+class RequiredChatDeployedRequest(TypedDict):
     # Unique project name.
-    "project": str,
+    project: str
 
     # The messages passed to the to provider chat endpoint.
-    "messages": typing.List[ChatMessage],
-    })
+    messages: typing.List[ChatMessage]
 
-OptionalChatDeployedRequest = TypedDict("OptionalChatDeployedRequest", {
+class OptionalChatDeployedRequest(TypedDict, total=False):
     # The inputs passed to the chat template.
-    "inputs": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    inputs: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
     # Identifies where the model was called from.
-    "source": str,
+    source: str
 
     # API keys required by each provider to make API calls. The API keys provided here are not stored by Humanloop. If not specified here, Humanloop will fall back to the key saved to your organization.
-    "provider_api_keys": ProviderApiKeys,
+    provider_api_keys: ProviderApiKeys
 
     # The number of chat responses.
-    "num_samples": int,
+    num_samples: int
 
     # If true, tokens will be sent as data-only server-sent events. If num_samples > 1, samples are streamed back independently.
-    "stream": bool,
+    stream: bool
 
     # End-user ID passed through to provider call.
-    "user": str,
+    user: str
 
     # Any additional metadata to record.
-    "metadata": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
-    }, total=False)
+    metadata: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
 class ChatDeployedRequest(RequiredChatDeployedRequest, OptionalChatDeployedRequest):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/chat_experiment_request.py` & `humanloop-0.4.3/humanloop/type/chat_experiment_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,43 +13,41 @@
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.chat_message import ChatMessage
 from humanloop.type.provider_api_keys import ProviderApiKeys
 
-RequiredChatExperimentRequest = TypedDict("RequiredChatExperimentRequest", {
+class RequiredChatExperimentRequest(TypedDict):
     # Unique project name.
-    "project": str,
+    project: str
 
     # The messages passed to the to provider chat endpoint.
-    "messages": typing.List[ChatMessage],
+    messages: typing.List[ChatMessage]
 
     # If an experiment ID is provided a model configuration will be sampled from the experiments active model configurations.
-    "experiment_id": str,
-    })
+    experiment_id: str
 
-OptionalChatExperimentRequest = TypedDict("OptionalChatExperimentRequest", {
+class OptionalChatExperimentRequest(TypedDict, total=False):
     # The inputs passed to the chat template.
-    "inputs": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    inputs: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
     # Identifies where the model was called from.
-    "source": str,
+    source: str
 
     # API keys required by each provider to make API calls. The API keys provided here are not stored by Humanloop. If not specified here, Humanloop will fall back to the key saved to your organization.
-    "provider_api_keys": ProviderApiKeys,
+    provider_api_keys: ProviderApiKeys
 
     # The number of chat responses, where each chat response will use a model configuration sampled from the experiment.
-    "num_samples": int,
+    num_samples: int
 
     # If true, tokens will be sent as data-only server-sent events. If num_samples > 1, samples are streamed back independently.
-    "stream": bool,
+    stream: bool
 
     # End-user ID passed through to provider call.
-    "user": str,
+    user: str
 
     # Any additional metadata to record.
-    "metadata": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
-    }, total=False)
+    metadata: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
 class ChatExperimentRequest(RequiredChatExperimentRequest, OptionalChatExperimentRequest):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/chat_message.py` & `humanloop-0.4.3/humanloop/type/chat_message.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,19 +12,17 @@
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.chat_role import ChatRole
 
-RequiredChatMessage = TypedDict("RequiredChatMessage", {
-    "role": ChatRole,
+class RequiredChatMessage(TypedDict):
+    role: ChatRole
 
-    "content": str,
-    })
+    content: str
 
-OptionalChatMessage = TypedDict("OptionalChatMessage", {
-    "name": str,
-    }, total=False)
+class OptionalChatMessage(TypedDict, total=False):
+    name: str
 
 class ChatMessage(RequiredChatMessage, OptionalChatMessage):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/chat_model_config_request.py` & `humanloop-0.4.3/humanloop/type/chat_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,45 +11,44 @@
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.chat_message import ChatMessage
+from humanloop.type.model_config_chat_request import ModelConfigChatRequest
 from humanloop.type.provider_api_keys import ProviderApiKeys
 
-RequiredChatModelConfigRequest = TypedDict("RequiredChatModelConfigRequest", {
+class RequiredChatRequest(TypedDict):
     # Unique project name.
-    "project": str,
+    project: str
 
     # The messages passed to the to provider chat endpoint.
-    "messages": typing.List[ChatMessage],
+    messages: typing.List[ChatMessage]
 
-    # Identifies the model configuration used to create a chat response.
-    "model_config_id": str,
-    })
+    # The model configuration used to create a chat response.
+    model_config: ModelConfigChatRequest
 
-OptionalChatModelConfigRequest = TypedDict("OptionalChatModelConfigRequest", {
+class OptionalChatRequest(TypedDict, total=False):
     # The inputs passed to the chat template.
-    "inputs": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    inputs: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
     # Identifies where the model was called from.
-    "source": str,
+    source: str
 
     # API keys required by each provider to make API calls. The API keys provided here are not stored by Humanloop. If not specified here, Humanloop will fall back to the key saved to your organization.
-    "provider_api_keys": ProviderApiKeys,
+    provider_api_keys: ProviderApiKeys
 
     # The number of chat responses.
-    "num_samples": int,
+    num_samples: int
 
     # If true, tokens will be sent as data-only server-sent events. If num_samples > 1, samples are streamed back independently.
-    "stream": bool,
+    stream: bool
 
     # End-user ID passed through to provider call.
-    "user": str,
+    user: str
 
     # Any additional metadata to record.
-    "metadata": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
-    }, total=False)
+    metadata: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
-class ChatModelConfigRequest(RequiredChatModelConfigRequest, OptionalChatModelConfigRequest):
+class ChatRequest(RequiredChatRequest, OptionalChatRequest):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/chat_request.py` & `humanloop-0.4.3/humanloop/type/chat_model_config_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,46 +11,43 @@
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.chat_message import ChatMessage
-from humanloop.type.model_config_chat_request import ModelConfigChatRequest
 from humanloop.type.provider_api_keys import ProviderApiKeys
 
-RequiredChatRequest = TypedDict("RequiredChatRequest", {
+class RequiredChatModelConfigRequest(TypedDict):
     # Unique project name.
-    "project": str,
+    project: str
 
     # The messages passed to the to provider chat endpoint.
-    "messages": typing.List[ChatMessage],
+    messages: typing.List[ChatMessage]
 
-    # The model configuration used to create a chat response.
-    "model_config": ModelConfigChatRequest,
-    })
+    # Identifies the model configuration used to create a chat response.
+    model_config_id: str
 
-OptionalChatRequest = TypedDict("OptionalChatRequest", {
+class OptionalChatModelConfigRequest(TypedDict, total=False):
     # The inputs passed to the chat template.
-    "inputs": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    inputs: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
     # Identifies where the model was called from.
-    "source": str,
+    source: str
 
     # API keys required by each provider to make API calls. The API keys provided here are not stored by Humanloop. If not specified here, Humanloop will fall back to the key saved to your organization.
-    "provider_api_keys": ProviderApiKeys,
+    provider_api_keys: ProviderApiKeys
 
     # The number of chat responses.
-    "num_samples": int,
+    num_samples: int
 
     # If true, tokens will be sent as data-only server-sent events. If num_samples > 1, samples are streamed back independently.
-    "stream": bool,
+    stream: bool
 
     # End-user ID passed through to provider call.
-    "user": str,
+    user: str
 
     # Any additional metadata to record.
-    "metadata": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
-    }, total=False)
+    metadata: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
-class ChatRequest(RequiredChatRequest, OptionalChatRequest):
+class ChatModelConfigRequest(RequiredChatModelConfigRequest, OptionalChatModelConfigRequest):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/chat_response.py` & `humanloop-0.4.3/humanloop/type/completion_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,43 +10,41 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
-from humanloop.type.chat_data_response import ChatDataResponse
+from humanloop.type.data_response import DataResponse
 from humanloop.type.usage import Usage
 
-RequiredChatResponse = TypedDict("RequiredChatResponse", {
+class RequiredCompletionResponse(TypedDict):
     # Unique identifier of the parent project.
-    "project_id": str,
+    project_id: str
 
-    # Array containing the chat responses.
-    "data": typing.List[ChatDataResponse],
+    # Array containing the generation responses.
+    data: typing.List[DataResponse]
 
     # The raw responses returned by the model provider.
-    "provider_responses": typing.List[typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
-    })
+    provider_responses: typing.List[typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
-OptionalChatResponse = TypedDict("OptionalChatResponse", {
-    # The number of chat responses.
-    "num_samples": int,
+class OptionalCompletionResponse(TypedDict, total=False):
+    # How many completions to make for each set of inputs.
+    num_samples: int
 
     # Include the log probabilities of the top n tokens in the provider_response
-    "logprobs": int,
+    logprobs: int
 
     # The suffix that comes after a completion of inserted text. Useful for completions that act like inserts.
-    "suffix": str,
+    suffix: str
 
     # End-user ID passed through to provider call.
-    "user": str,
+    user: str
 
     # Counts of the number of tokens used and related stats.
-    "usage": Usage,
+    usage: Usage
 
     # Any additional metadata to record.
-    "metadata": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
-    }, total=False)
+    metadata: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
-class ChatResponse(RequiredChatResponse, OptionalChatResponse):
+class CompletionResponse(RequiredCompletionResponse, OptionalCompletionResponse):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/chat_role.py` & `humanloop-0.4.3/humanloop/type/chat_role.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/type/completion_deployed_request.py` & `humanloop-0.4.3/humanloop/type/completion_deployed_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,43 +12,41 @@
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.provider_api_keys import ProviderApiKeys
 
-RequiredCompletionDeployedRequest = TypedDict("RequiredCompletionDeployedRequest", {
+class RequiredCompletionDeployedRequest(TypedDict):
     # Unique project name.
-    "project": str,
+    project: str
 
     # The inputs passed to the prompt template.
-    "inputs": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
-    })
+    inputs: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
-OptionalCompletionDeployedRequest = TypedDict("OptionalCompletionDeployedRequest", {
+class OptionalCompletionDeployedRequest(TypedDict, total=False):
     # Identifies where the model was called from.
-    "source": str,
+    source: str
 
     # API keys required by each provider to make API calls. The API keys provided here are not stored by Humanloop. If not specified here, Humanloop will fall back to the key saved to your organization.
-    "provider_api_keys": ProviderApiKeys,
+    provider_api_keys: ProviderApiKeys
 
     # The number of generations.
-    "num_samples": int,
+    num_samples: int
 
     # Include the log probabilities of the top n tokens in the provider_response
-    "logprobs": int,
+    logprobs: int
 
     # If true, tokens will be sent as data-only server-sent events. If num_samples > 1, samples are streamed back independently.
-    "stream": bool,
+    stream: bool
 
     # The suffix that comes after a completion of inserted text. Useful for completions that act like inserts.
-    "suffix": str,
+    suffix: str
 
     # End-user ID passed through to provider call.
-    "user": str,
+    user: str
 
     # Any additional metadata to record.
-    "metadata": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
-    }, total=False)
+    metadata: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
 class CompletionDeployedRequest(RequiredCompletionDeployedRequest, OptionalCompletionDeployedRequest):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/completion_experiment_request.py` & `humanloop-0.4.3/humanloop/type/completion_experiment_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,46 +12,44 @@
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.provider_api_keys import ProviderApiKeys
 
-RequiredCompletionExperimentRequest = TypedDict("RequiredCompletionExperimentRequest", {
+class RequiredCompletionExperimentRequest(TypedDict):
     # Unique project name.
-    "project": str,
+    project: str
 
     # The inputs passed to the prompt template.
-    "inputs": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    inputs: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
     # If an experiment ID is provided a model configuration will be sampled from the experiments active model configurations.
-    "experiment_id": str,
-    })
+    experiment_id: str
 
-OptionalCompletionExperimentRequest = TypedDict("OptionalCompletionExperimentRequest", {
+class OptionalCompletionExperimentRequest(TypedDict, total=False):
     # Identifies where the model was called from.
-    "source": str,
+    source: str
 
     # API keys required by each provider to make API calls. The API keys provided here are not stored by Humanloop. If not specified here, Humanloop will fall back to the key saved to your organization.
-    "provider_api_keys": ProviderApiKeys,
+    provider_api_keys: ProviderApiKeys
 
     # The number of chat responses, where each chat response will use a model configuration sampled from the experiment.
-    "num_samples": int,
+    num_samples: int
 
     # Include the log probabilities of the top n tokens in the provider_response
-    "logprobs": int,
+    logprobs: int
 
     # If true, tokens will be sent as data-only server-sent events. If num_samples > 1, samples are streamed back independently.
-    "stream": bool,
+    stream: bool
 
     # The suffix that comes after a completion of inserted text. Useful for completions that act like inserts.
-    "suffix": str,
+    suffix: str
 
     # End-user ID passed through to provider call.
-    "user": str,
+    user: str
 
     # Any additional metadata to record.
-    "metadata": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
-    }, total=False)
+    metadata: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
 class CompletionExperimentRequest(RequiredCompletionExperimentRequest, OptionalCompletionExperimentRequest):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/completion_model_config_request.py` & `humanloop-0.4.3/humanloop/type/completion_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,48 +10,47 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
+from humanloop.type.model_config_completion_request import ModelConfigCompletionRequest
 from humanloop.type.provider_api_keys import ProviderApiKeys
 
-RequiredCompletionModelConfigRequest = TypedDict("RequiredCompletionModelConfigRequest", {
+class RequiredCompletionRequest(TypedDict):
     # Unique project name.
-    "project": str,
+    project: str
 
     # The inputs passed to the prompt template.
-    "inputs": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    inputs: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
-    # Identifies the model configuration used to create a chat response.
-    "model_config_id": str,
-    })
+    # The model configuration used to generate.
+    model_config: ModelConfigCompletionRequest
 
-OptionalCompletionModelConfigRequest = TypedDict("OptionalCompletionModelConfigRequest", {
+class OptionalCompletionRequest(TypedDict, total=False):
     # Identifies where the model was called from.
-    "source": str,
+    source: str
 
     # API keys required by each provider to make API calls. The API keys provided here are not stored by Humanloop. If not specified here, Humanloop will fall back to the key saved to your organization.
-    "provider_api_keys": ProviderApiKeys,
+    provider_api_keys: ProviderApiKeys
 
     # The number of generations.
-    "num_samples": int,
+    num_samples: int
 
     # Include the log probabilities of the top n tokens in the provider_response
-    "logprobs": int,
+    logprobs: int
 
     # If true, tokens will be sent as data-only server-sent events. If num_samples > 1, samples are streamed back independently.
-    "stream": bool,
+    stream: bool
 
     # The suffix that comes after a completion of inserted text. Useful for completions that act like inserts.
-    "suffix": str,
+    suffix: str
 
     # End-user ID passed through to provider call.
-    "user": str,
+    user: str
 
     # Any additional metadata to record.
-    "metadata": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
-    }, total=False)
+    metadata: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
-class CompletionModelConfigRequest(RequiredCompletionModelConfigRequest, OptionalCompletionModelConfigRequest):
+class CompletionRequest(RequiredCompletionRequest, OptionalCompletionRequest):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/completion_request.py` & `humanloop-0.4.3/humanloop/type/trace_log_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,49 +10,53 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
-from humanloop.type.model_config_completion_request import ModelConfigCompletionRequest
-from humanloop.type.provider_api_keys import ProviderApiKeys
-
-RequiredCompletionRequest = TypedDict("RequiredCompletionRequest", {
-    # Unique project name.
-    "project": str,
+from humanloop.type.agent_config_request import AgentConfigRequest
+from humanloop.type.chat_message import ChatMessage
+from humanloop.type.generic_config_request import GenericConfigRequest
+from humanloop.type.tool_config_request import ToolConfigRequest
+from humanloop.type.trace_model_config_request import TraceModelConfigRequest
+
+class RequiredTraceLogRequest(TypedDict):
+    # Unique function name. If no function exists with this name, a new function will be created.
+    function_name: str
+
+    # Generated output from your model for the provided inputs.
+    output: str
+
+class OptionalTraceLogRequest(TypedDict, total=False):
+    # Unique ID of an experiment trial to associate to the log.
+    trial_id: str
 
     # The inputs passed to the prompt template.
-    "inputs": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    inputs: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
-    # The model configuration used to generate.
-    "model_config": ModelConfigCompletionRequest,
-    })
+    # The messages passed to the to provider chat endpoint.
+    messages: typing.List[ChatMessage]
 
-OptionalCompletionRequest = TypedDict("OptionalCompletionRequest", {
     # Identifies where the model was called from.
-    "source": str,
-
-    # API keys required by each provider to make API calls. The API keys provided here are not stored by Humanloop. If not specified here, Humanloop will fall back to the key saved to your organization.
-    "provider_api_keys": ProviderApiKeys,
+    source: str
 
-    # The number of generations.
-    "num_samples": int,
+    # The model config used for this generation. Required unless `trial_id` is provided.
+    config: typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]
 
-    # Include the log probabilities of the top n tokens in the provider_response
-    "logprobs": int,
+    # Any additional metadata to record.
+    metadata: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
-    # If true, tokens will be sent as data-only server-sent events. If num_samples > 1, samples are streamed back independently.
-    "stream": bool,
+    # Error message if the log is an error.
+    error: str
 
-    # The suffix that comes after a completion of inserted text. Useful for completions that act like inserts.
-    "suffix": str,
+    # Duration of the logged event in seconds.
+    duration: typing.Union[int, float]
 
-    # End-user ID passed through to provider call.
-    "user": str,
+    # User-defined timestamp for when the log was created.
+    created_at: datetime
 
-    # Any additional metadata to record.
-    "metadata": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
-    }, total=False)
+    # List of children logs.
+    children: typing.List["TraceLogRequest"]
 
-class CompletionRequest(RequiredCompletionRequest, OptionalCompletionRequest):
+class TraceLogRequest(RequiredTraceLogRequest, OptionalTraceLogRequest):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/completion_response.py` & `humanloop-0.4.3/humanloop/type/data_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,43 +10,37 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
-from humanloop.type.data_response import DataResponse
-from humanloop.type.usage import Usage
+from humanloop.type.tool_result_response import ToolResultResponse
 
-RequiredCompletionResponse = TypedDict("RequiredCompletionResponse", {
-    # Unique identifier of the parent project.
-    "project_id": str,
+class RequiredDataResponse(TypedDict):
+    # Unique ID for the model inputs and output logged to Humanloop. Use this when recording feedback later.
+    id: str
 
-    # Array containing the generation responses.
-    "data": typing.List[DataResponse],
+    # The index for the sampled generation for a given input. The num_samples request parameter controls how many samples are generated.
+    index: int
 
-    # The raw responses returned by the model provider.
-    "provider_responses": typing.List[typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
-    })
+    # Output text returned from the provider model with leading and trailing whitespaces stripped.
+    output: str
 
-OptionalCompletionResponse = TypedDict("OptionalCompletionResponse", {
-    # How many completions to make for each set of inputs.
-    "num_samples": int,
+    # Raw output text returned from the provider model.
+    raw_output: str
 
-    # Include the log probabilities of the top n tokens in the provider_response
-    "logprobs": int,
+    # The inputs passed to the prompt template.
+    inputs: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
-    # The suffix that comes after a completion of inserted text. Useful for completions that act like inserts.
-    "suffix": str,
+    # The model configuration used to create the generation.
+    model_config_id: str
 
-    # End-user ID passed through to provider call.
-    "user": str,
+class OptionalDataResponse(TypedDict, total=False):
+    # Why the completion ended. Usually one of 'stop' (indicating a stop token was encountered), or 'length' (indicating the max tokens limit has been reached). It will be set as null for the intermediary responses during a stream, and will only be set as non-null for the final streamed token.
+    finish_reason: str
 
-    # Counts of the number of tokens used and related stats.
-    "usage": Usage,
+    # Results of any tools run during the generation.
+    tools: typing.List[ToolResultResponse]
 
-    # Any additional metadata to record.
-    "metadata": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
-    }, total=False)
-
-class CompletionResponse(RequiredCompletionResponse, OptionalCompletionResponse):
+class DataResponse(RequiredDataResponse, OptionalDataResponse):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/create_experiment_request.py` & `humanloop-0.4.3/humanloop/type/update_experiment_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.positive_label import PositiveLabel
 
-RequiredCreateExperimentRequest = TypedDict("RequiredCreateExperimentRequest", {
+class RequiredUpdateExperimentRequest(TypedDict):
+    pass
+
+class OptionalUpdateExperimentRequest(TypedDict, total=False):
     # Name of experiment.
-    "name": str,
+    name: str
 
     # Feedback labels to treat as positive user feedback. Used to monitor the performance of model configs in the experiment.
-    "positive_labels": typing.List[PositiveLabel],
-    })
+    positive_labels: typing.List[PositiveLabel]
+
+    # Model configs to add to this experiment.
+    config_ids_to_register: typing.List[str]
 
-OptionalCreateExperimentRequest = TypedDict("OptionalCreateExperimentRequest", {
-    # Model configs to add to this experiment. Further model configs can be added later.
-    "model_config_ids": typing.List[str],
-
-    # Whether to set the created project as the project's active experiment.
-    "set_active": bool,
-    }, total=False)
+    # Model configs in this experiment to be deactivated.
+    config_ids_to_deregister: typing.List[str]
 
-class CreateExperimentRequest(RequiredCreateExperimentRequest, OptionalCreateExperimentRequest):
+class UpdateExperimentRequest(RequiredUpdateExperimentRequest, OptionalUpdateExperimentRequest):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/create_project_request.py` & `humanloop-0.4.3/humanloop/type/create_project_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,17 @@
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.feedback_type_request import FeedbackTypeRequest
 
-RequiredCreateProjectRequest = TypedDict("RequiredCreateProjectRequest", {
+class RequiredCreateProjectRequest(TypedDict):
     # Unique project name.
-    "name": str,
-    })
+    name: str
 
-OptionalCreateProjectRequest = TypedDict("OptionalCreateProjectRequest", {
+class OptionalCreateProjectRequest(TypedDict, total=False):
     # Feedback types to be created.
-    "feedback_types": typing.List[FeedbackTypeRequest],
-    }, total=False)
+    feedback_types: typing.List[FeedbackTypeRequest]
 
 class CreateProjectRequest(RequiredCreateProjectRequest, OptionalCreateProjectRequest):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/create_session_request.py` & `humanloop-0.4.3/humanloop/type/categorical_feedback_label.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
+from humanloop.type.label_sentiment import LabelSentiment
 
-RequiredCreateSessionRequest = TypedDict("RequiredCreateSessionRequest", {
-    # App to associate the created session to.
-    "app": str,
-    })
+class RequiredCategoricalFeedbackLabel(TypedDict):
+    value: str
 
-OptionalCreateSessionRequest = TypedDict("OptionalCreateSessionRequest", {
-    }, total=False)
+    # Whether the feedback sentiment is positive or negative.
+    sentiment: LabelSentiment
 
-class CreateSessionRequest(RequiredCreateSessionRequest, OptionalCreateSessionRequest):
+class OptionalCategoricalFeedbackLabel(TypedDict, total=False):
+    pass
+
+class CategoricalFeedbackLabel(RequiredCategoricalFeedbackLabel, OptionalCategoricalFeedbackLabel):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/data_response.py` & `humanloop-0.4.3/humanloop/type/chat_data_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,39 +10,41 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
+from humanloop.type.chat_message import ChatMessage
 from humanloop.type.tool_result_response import ToolResultResponse
 
-RequiredDataResponse = TypedDict("RequiredDataResponse", {
+class RequiredChatDataResponse(TypedDict):
     # Unique ID for the model inputs and output logged to Humanloop. Use this when recording feedback later.
-    "id": str,
+    id: str
 
     # The index for the sampled generation for a given input. The num_samples request parameter controls how many samples are generated.
-    "index": int,
+    index: int
 
     # Output text returned from the provider model with leading and trailing whitespaces stripped.
-    "output": str,
+    output: str
 
     # Raw output text returned from the provider model.
-    "raw_output": str,
-
-    # The inputs passed to the prompt template.
-    "inputs": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    raw_output: str
 
     # The model configuration used to create the generation.
-    "model_config_id": str,
-    })
+    model_config_id: str
+
+class OptionalChatDataResponse(TypedDict, total=False):
+    # The inputs passed to the chat template.
+    inputs: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
-OptionalDataResponse = TypedDict("OptionalDataResponse", {
     # Why the completion ended. Usually one of 'stop' (indicating a stop token was encountered), or 'length' (indicating the max tokens limit has been reached). It will be set as null for the intermediary responses during a stream, and will only be set as non-null for the final streamed token.
-    "finish_reason": str,
+    finish_reason: str
 
     # Results of any tools run during the generation.
-    "tools": typing.List[ToolResultResponse],
-    }, total=False)
+    tools: typing.List[ToolResultResponse]
+
+    # The messages passed to the to provider chat endpoint.
+    messages: typing.List[ChatMessage]
 
-class DataResponse(RequiredDataResponse, OptionalDataResponse):
+class ChatDataResponse(RequiredChatDataResponse, OptionalChatDataResponse):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/experiment_model_config_response.py` & `humanloop-0.4.3/humanloop/type/experiment_config_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,40 +10,38 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
-from humanloop.type.src_external_app_models_v4_model_configs_model_config_response import SrcExternalAppModelsV4ModelConfigsModelConfigResponse
+from humanloop.type.config_response import ConfigResponse
 
-RequiredExperimentModelConfigResponse = TypedDict("RequiredExperimentModelConfigResponse", {
+class RequiredExperimentConfigResponse(TypedDict):
     # Number of datapoints with feedback associated to the experiment.
-    "trials_count": int,
+    trials_count: int
 
     # Whether the model config is active in the experiment. Only active model configs can be sampled from the experiment.
-    "active": bool,
+    active: bool
 
     # String ID of model config. Starts with `config_`.
-    "id": str,
+    id: str
 
     # Display name of model config. If this is not set by the user, a friendly name is generated.
-    "display_name": str,
+    display_name: str
 
-    # Definition of the model config used in the experiment.
-    "model_config": SrcExternalAppModelsV4ModelConfigsModelConfigResponse,
+    # Definition of the config used in the experiment.
+    config: ConfigResponse
 
-    "created_at": datetime,
+    created_at: datetime
 
-    "updated_at": datetime,
-    })
+    updated_at: datetime
 
-OptionalExperimentModelConfigResponse = TypedDict("OptionalExperimentModelConfigResponse", {
+class OptionalExperimentConfigResponse(TypedDict, total=False):
     # The mean performance of the model config.
-    "mean": typing.Union[int, float],
+    mean: typing.Union[int, float]
 
     # The spread of performance of the model config.
-    "spread": typing.Union[int, float],
-    }, total=False)
+    spread: typing.Union[int, float]
 
-class ExperimentModelConfigResponse(RequiredExperimentModelConfigResponse, OptionalExperimentModelConfigResponse):
+class ExperimentConfigResponse(RequiredExperimentConfigResponse, OptionalExperimentConfigResponse):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/experiment_response.py` & `humanloop-0.4.3/humanloop/type/experiment_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,42 +11,40 @@
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.base_metric_response import BaseMetricResponse
-from humanloop.type.experiment_model_config_response import ExperimentModelConfigResponse
+from humanloop.type.experiment_config_response import ExperimentConfigResponse
 from humanloop.type.experiment_status import ExperimentStatus
 from humanloop.type.positive_label import PositiveLabel
 
-RequiredExperimentResponse = TypedDict("RequiredExperimentResponse", {
+class RequiredExperimentResponse(TypedDict):
     # String ID of experiment. Starts with `exp_`.
-    "id": str,
+    id: str
 
     # String ID of project the experiment belongs to. Starts with `pr_`.
-    "project_id": str,
+    project_id: str
 
     # Name of experiment.
-    "name": str,
+    name: str
 
     # Status of experiment.
-    "status": ExperimentStatus,
+    status: ExperimentStatus
 
     # Metric used as the experiment's objective.
-    "metric": BaseMetricResponse,
+    metric: BaseMetricResponse
 
     # Feedback labels to treat as positive user feedback. Used to monitor the performance of model configs in the experiment.
-    "positive_labels": typing.List[PositiveLabel],
+    positive_labels: typing.List[PositiveLabel]
 
-    "created_at": datetime,
+    created_at: datetime
 
-    "updated_at": datetime,
-    })
+    updated_at: datetime
 
-OptionalExperimentResponse = TypedDict("OptionalExperimentResponse", {
-    # List of model configs associated to the experiment.
-    "model_configs": typing.List[ExperimentModelConfigResponse],
-    }, total=False)
+class OptionalExperimentResponse(TypedDict, total=False):
+    # List of configs associated to the experiment.
+    configs: typing.List[ExperimentConfigResponse]
 
 class ExperimentResponse(RequiredExperimentResponse, OptionalExperimentResponse):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/experiment_status.py` & `humanloop-0.4.3/humanloop/type/experiment_status.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/type/experiments_list_response.py` & `humanloop-0.4.3/humanloop/type/experiments_list_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/type/feedback.py` & `humanloop-0.4.3/humanloop/type/feedback_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,28 +12,29 @@
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.feedback_type import FeedbackType
 
-RequiredFeedback = TypedDict("RequiredFeedback", {
+class RequiredFeedbackResponse(TypedDict):
     # The type of feedback. The default feedback types available are 'rating', 'action', 'issue', 'correction', and 'comment'.
-    "type": typing.Union[FeedbackType, str],
+    type: typing.Union[FeedbackType, str]
 
     # The feedback value to set. This would be the appropriate text for 'correction' or 'comment', or a label to apply for 'rating', 'action', or 'issue'.
-    "value": str,
-    })
+    value: str
 
-OptionalFeedback = TypedDict("OptionalFeedback", {
+    # String ID of user feedback. Starts with `ann_`, short for annotation.
+    id: str
+
+class OptionalFeedbackResponse(TypedDict, total=False):
     # ID to associate the feedback to a previously logged datapoint.
-    "data_id": str,
+    data_id: str
 
     # A unique identifier to who provided the feedback.
-    "user": str,
+    user: str
 
     # User defined timestamp for when the feedback was created. 
-    "created_at": datetime,
-    }, total=False)
+    created_at: datetime
 
-class Feedback(RequiredFeedback, OptionalFeedback):
+class FeedbackResponse(RequiredFeedbackResponse, OptionalFeedbackResponse):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/feedback_class.py` & `humanloop-0.4.3/humanloop/type/feedback_class.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/type/feedback_label_request.py` & `humanloop-0.4.3/humanloop/type/feedback_types.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,19 +10,10 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
-from humanloop.type.label_sentiment import LabelSentiment
+from humanloop.type.feedback_type_model import FeedbackTypeModel
 
-RequiredFeedbackLabelRequest = TypedDict("RequiredFeedbackLabelRequest", {
-    "value": str,
-    })
-
-OptionalFeedbackLabelRequest = TypedDict("OptionalFeedbackLabelRequest", {
-    "sentiment": LabelSentiment,
-    }, total=False)
-
-class FeedbackLabelRequest(RequiredFeedbackLabelRequest, OptionalFeedbackLabelRequest):
-    pass
+FeedbackTypes = typing.List[FeedbackTypeModel]
```

### Comparing `humanloop-0.4.2/humanloop/type/feedback_request.py` & `humanloop-0.4.3/humanloop/type/feedback_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,31 +12,29 @@
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.feedback_type import FeedbackType
 
-RequiredFeedbackRequest = TypedDict("RequiredFeedbackRequest", {
+class RequiredFeedbackRequest(TypedDict):
     # The type of feedback. The default feedback types available are 'rating', 'action', 'issue', 'correction', and 'comment'.
-    "type": typing.Union[FeedbackType, str],
-    })
+    type: typing.Union[FeedbackType, str]
 
-OptionalFeedbackRequest = TypedDict("OptionalFeedbackRequest", {
+class OptionalFeedbackRequest(TypedDict, total=False):
     # The feedback value to be set. This field should be left blank when unsetting 'rating', 'correction' or 'comment', but is required otherwise.
-    "value": str,
+    value: str
 
     # ID to associate the feedback to a previously logged datapoint.
-    "data_id": str,
+    data_id: str
 
     # A unique identifier to who provided the feedback.
-    "user": str,
+    user: str
 
     # User defined timestamp for when the feedback was created. 
-    "created_at": datetime,
+    created_at: datetime
 
     # If true, the value for this feedback is unset.
-    "unset": bool,
-    }, total=False)
+    unset: bool
 
 class FeedbackRequest(RequiredFeedbackRequest, OptionalFeedbackRequest):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/feedback_response.py` & `humanloop-0.4.3/humanloop/type/feedback.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,31 +12,26 @@
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.feedback_type import FeedbackType
 
-RequiredFeedbackResponse = TypedDict("RequiredFeedbackResponse", {
+class RequiredFeedback(TypedDict):
     # The type of feedback. The default feedback types available are 'rating', 'action', 'issue', 'correction', and 'comment'.
-    "type": typing.Union[FeedbackType, str],
+    type: typing.Union[FeedbackType, str]
 
     # The feedback value to set. This would be the appropriate text for 'correction' or 'comment', or a label to apply for 'rating', 'action', or 'issue'.
-    "value": str,
+    value: str
 
-    # String ID of user feedback. Starts with `ann_`, short for annotation.
-    "id": str,
-    })
-
-OptionalFeedbackResponse = TypedDict("OptionalFeedbackResponse", {
+class OptionalFeedback(TypedDict, total=False):
     # ID to associate the feedback to a previously logged datapoint.
-    "data_id": str,
+    data_id: str
 
     # A unique identifier to who provided the feedback.
-    "user": str,
+    user: str
 
     # User defined timestamp for when the feedback was created. 
-    "created_at": datetime,
-    }, total=False)
+    created_at: datetime
 
-class FeedbackResponse(RequiredFeedbackResponse, OptionalFeedbackResponse):
+class Feedback(RequiredFeedback, OptionalFeedback):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/feedback_submit_request.py` & `humanloop-0.4.3/humanloop/type/feedback_submit_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/type/feedback_submit_response.py` & `humanloop-0.4.3/humanloop/type/feedback_submit_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/type/feedback_type.py` & `humanloop-0.4.3/humanloop/type/feedback_type.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/type/feedback_type_model.py` & `humanloop-0.4.3/humanloop/type/feedback_type_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,19 +13,17 @@
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.categorical_feedback_label import CategoricalFeedbackLabel
 from humanloop.type.feedback_type import FeedbackType
 
-RequiredFeedbackTypeModel = TypedDict("RequiredFeedbackTypeModel", {
+class RequiredFeedbackTypeModel(TypedDict):
     # The type of feedback. The default feedback types available are 'rating', 'action', 'issue', 'correction', and 'comment'.
-    "type": typing.Union[FeedbackType, str],
-    })
+    type: typing.Union[FeedbackType, str]
 
-OptionalFeedbackTypeModel = TypedDict("OptionalFeedbackTypeModel", {
+class OptionalFeedbackTypeModel(TypedDict, total=False):
     # The allowed values for categorical feedback types. Not populated for `correction` and `comment`.
-    "values": typing.List[CategoricalFeedbackLabel],
-    }, total=False)
+    values: typing.List[CategoricalFeedbackLabel]
 
 class FeedbackTypeModel(RequiredFeedbackTypeModel, OptionalFeedbackTypeModel):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/feedback_type_request.py` & `humanloop-0.4.3/humanloop/type/feedback_type_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/type/feedback_types.py` & `humanloop-0.4.3/humanloop/type/config_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,10 +10,9 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
-from humanloop.type.feedback_type_model import FeedbackTypeModel
 
-FeedbackTypes = typing.List[FeedbackTypeModel]
+ConfigType = Literal["generic", "model", "tool", "agent"]
```

### Comparing `humanloop-0.4.2/humanloop/type/get_model_config_response.py` & `humanloop-0.4.3/humanloop/type/project_model_config_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,81 +13,76 @@
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.chat_message import ChatMessage
 from humanloop.type.model_endpoints import ModelEndpoints
 from humanloop.type.model_providers import ModelProviders
-from humanloop.type.src_external_app_models_v4_model_configs_project_model_config_feedback_stats_response import SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse
+from humanloop.type.src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response import SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse
 
-RequiredGetModelConfigResponse = TypedDict("RequiredGetModelConfigResponse", {
-    # The model instance used. E.g. text-davinci-002.
-    "model": str,
+class RequiredProjectModelConfigResponse(TypedDict):
+    # What model instance to use for the generation. e.g. text-davinci-002.
+    model: str
 
     # Model config unique identifier generated by Humanloop.
-    "id": str,
+    id: str
 
-    "created_at": datetime,
+    created_at: datetime
 
-    "updated_at": datetime,
+    updated_at: datetime
 
-    "last_used": datetime,
-    })
+    last_used: datetime
 
-OptionalGetModelConfigResponse = TypedDict("OptionalGetModelConfigResponse", {
+class OptionalProjectModelConfigResponse(TypedDict, total=False):
     # The company providing the underlying model service.
-    "provider": ModelProviders,
+    provider: ModelProviders
 
-    # The maximum number of tokens to generate. Provide max_tokens=-1 to dynamically calculate the maximum number of tokens to generate given the length of the prompt
-    "max_tokens": int,
+    # Which of the providers model endpoints to use. For example Complete or Edit.
+    endpoint: ModelEndpoints
+
+    # Prompt template that will take your specified inputs to form your final request to the provider model. NB: Input variables within the prompt template should be specified with syntax: {{INPUT_NAME}}.
+    prompt_template: str
+
+    # Messages prepended to the list of messages sent to the provider. These messages that will take your specified inputs to form your final request to the provider model. NB: Input variables within the prompt template should be specified with syntax: {{INPUT_NAME}}.
+    chat_template: typing.List[ChatMessage]
 
     # What sampling temperature to use when making a generation. Higher values means the model will be more creative.
-    "temperature": typing.Union[int, float],
+    temperature: typing.Union[int, float]
+
+    # The maximum number of tokens to generate in the completion.
+    max_tokens: int
 
     # An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with top_p probability mass.
-    "top_p": typing.Union[int, float],
+    top_p: typing.Union[int, float]
 
     # The string (or list of strings) after which the model will stop generating. The returned text will not contain the stop sequence.
-    "stop": typing.Union[str, typing.List[str]],
+    stop: typing.Union[str, typing.List[str]]
 
     # Number between -2.0 and 2.0. Positive values penalize new tokens based on whether they appear in the generation so far.
-    "presence_penalty": typing.Union[int, float],
+    presence_penalty: typing.Union[int, float]
 
     # Number between -2.0 and 2.0. Positive values penalize new tokens based on how frequently they appear in the generation so far.
-    "frequency_penalty": typing.Union[int, float],
+    frequency_penalty: typing.Union[int, float]
 
     # Other parameter values to be passed to the provider call.
-    "other": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    other: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
     # A friendly display name for the model config.
-    "display_name": str,
-
-    # Prompt template that will take your specified inputs to form your final request to the model. NB: Input variables within the prompt template should be specified with syntax: {{INPUT_NAME}}.
-    "prompt_template": str,
-
-    # Messages prepended to the list of messages sent to the provider. These messages that will take your specified inputs to form your final request to the provider model. NB: Input variables within the template should be specified with syntax: {{INPUT_NAME}}.
-    "chat_template": typing.List[ChatMessage],
-
-    # The provider model endpoint used.
-    "endpoint": ModelEndpoints,
+    display_name: str
 
     # String ID of project the model config belongs to. Starts with `pr_`.
-    "project_id": str,
+    project_id: str
 
     # Name of the project the model config belongs to.
-    "project_name": str,
+    project_name: str
 
     # Feedback statistics for the project model config.
-    "feedback_stats": typing.List[SrcExternalAppModelsV4ModelConfigsProjectModelConfigFeedbackStatsResponse],
+    feedback_stats: typing.List[SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse]
 
     # Number of datapoints associated with this project model config.
-    "num_datapoints": int,
+    num_datapoints: int
 
     # The ID of the experiment the model config has been registered to. Only populated when registering a model config to an experiment.
-    "experiment_id": str,
-
-    # ID of trial to reference in subsequent log calls.
-    "trial_id": str,
-    }, total=False)
+    experiment_id: str
 
-class GetModelConfigResponse(RequiredGetModelConfigResponse, OptionalGetModelConfigResponse):
+class ProjectModelConfigResponse(RequiredProjectModelConfigResponse, OptionalProjectModelConfigResponse):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/http_validation_error.py` & `humanloop-0.4.3/humanloop/type/http_validation_error.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.validation_error import ValidationError
 
-RequiredHTTPValidationError = TypedDict("RequiredHTTPValidationError", {
-    })
+class RequiredHTTPValidationError(TypedDict):
+    pass
 
-OptionalHTTPValidationError = TypedDict("OptionalHTTPValidationError", {
-    "detail": typing.List[ValidationError],
-    }, total=False)
+class OptionalHTTPValidationError(TypedDict, total=False):
+    detail: typing.List[ValidationError]
 
 class HTTPValidationError(RequiredHTTPValidationError, OptionalHTTPValidationError):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/label_sentiment.py` & `humanloop-0.4.3/humanloop/type/label_sentiment.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/type/log_datapoint_request.py` & `humanloop-0.4.3/humanloop/type/log_datapoint_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/type/log_request.py` & `humanloop-0.4.3/humanloop/type/log_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,54 +10,60 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
+from humanloop.type.agent_config_request import AgentConfigRequest
 from humanloop.type.chat_message import ChatMessage
 from humanloop.type.feedback import Feedback
-from humanloop.type.model_config_chat_request import ModelConfigChatRequest
-from humanloop.type.model_config_completion_request import ModelConfigCompletionRequest
-
-RequiredLogRequest = TypedDict("RequiredLogRequest", {
-    # Unique project name. If it does not exist, a new project will be created.
-    "project": str,
+from humanloop.type.generic_config_request import GenericConfigRequest
+from humanloop.type.tool_config_request import ToolConfigRequest
+from humanloop.type.trace_model_config_request import TraceModelConfigRequest
 
+class RequiredLogRequest(TypedDict):
     # Generated output from your model for the provided inputs.
-    "output": str,
-    })
+    output: str
+
+class OptionalLogRequest(TypedDict, total=False):
+    # Unique function name. If no function exists with this name, a new function will be created.
+    project: str
 
-OptionalLogRequest = TypedDict("OptionalLogRequest", {
     # ID of the session to associate the datapoint.
-    "session_id": str,
+    session_id: str
 
     # ID associated to the parent datapoint in a session.
-    "parent_id": str,
+    parent_id: str
 
     # Unique ID of an experiment trial to associate to the log.
-    "trial_id": str,
+    trial_id: str
 
     # The inputs passed to the prompt template.
-    "inputs": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    inputs: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
     # The messages passed to the to provider chat endpoint.
-    "messages": typing.List[ChatMessage],
+    messages: typing.List[ChatMessage]
 
     # Identifies where the model was called from.
-    "source": str,
+    source: str
 
     # The model config used for this generation. Required unless `trial_id` is provided.
-    "model_config": typing.Union[ModelConfigCompletionRequest, ModelConfigChatRequest],
+    config: typing.Union[TraceModelConfigRequest, ToolConfigRequest, GenericConfigRequest, AgentConfigRequest]
 
     # Any additional metadata to record.
-    "metadata": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    metadata: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
     # Optional parameter to provide feedback with your logged datapoint.
-    "feedback": typing.Union[Feedback, typing.List[Feedback]],
+    feedback: typing.Union[Feedback, typing.List[Feedback]]
 
     # User defined timestamp for when the log was created. 
-    "created_at": datetime,
-    }, total=False)
+    created_at: datetime
+
+    # Error message if the log is an error.
+    error: str
+
+    # Duration of the logged event in seconds.
+    duration: typing.Union[int, float]
 
 class LogRequest(RequiredLogRequest, OptionalLogRequest):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/log_response.py` & `humanloop-0.4.3/humanloop/type/log_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,73 +11,80 @@
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.chat_message import ChatMessage
+from humanloop.type.config_response import ConfigResponse
 from humanloop.type.feedback import Feedback
-from humanloop.type.src_external_app_models_v4_model_configs_project_model_config_response import SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse
+from humanloop.type.project_config_response import ProjectConfigResponse
 
-RequiredLogResponse = TypedDict("RequiredLogResponse", {
+class RequiredLogResponse(TypedDict):
     # Function name. If it does not exist, a new function will be created.
-    "project": str,
+    project: str
 
     # Generated output from your model for the provided inputs.
-    "output": str,
+    output: str
+
+    config: ConfigResponse
 
     # String ID of logged datapoint. Starts with `data_`.
-    "id": str,
+    id: str
 
     # String ID of project the datapoint belongs to. Starts with `pr_`.
-    "project_id": str,
-    })
+    project_id: str
 
-OptionalLogResponse = TypedDict("OptionalLogResponse", {
+class OptionalLogResponse(TypedDict, total=False):
     # Session ID.
-    "session_id": str,
+    session_id: str
 
     # Id associated to the parent datapoint. Useful when providing a trace from a chain.
-    "parent_id": str,
+    parent_id: str
 
     # Unique ID of an experiment trial to associate to the log.
-    "trial_id": str,
+    trial_id: str
 
     # The inputs passed to the prompt template.
-    "inputs": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    inputs: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
     # The messages passed to the to provider chat endpoint.
-    "messages": typing.List[ChatMessage],
+    messages: typing.List[ChatMessage]
 
     # Identifies where the model was called from.
-    "source": str,
-
-    # The model config used for this datapoint.
-    "model_config": SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse,
+    source: str
 
     # Additional metadata logged for reference.
-    "metadata": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    metadata: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
     # Feedback associated to the datapoint.
-    "feedback": typing.Union[Feedback, typing.List[Feedback]],
+    feedback: typing.Union[Feedback, typing.List[Feedback]]
 
     # Timestamp for when the datapoint was created.
-    "created_at": datetime,
+    created_at: datetime
+
+    # Error message if the log is an error.
+    error: str
+
+    # Duration of the logged event in seconds.
+    duration: typing.Union[int, float]
+
+    # The config used for this datapoint.
+    model_config: ProjectConfigResponse
 
     # User email address provided when creating the datapoint.
-    "user": str,
+    user: str
 
     # Original response from the provider.
-    "provider_response": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    provider_response: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
     # Latency of provider response.
-    "provider_latency": typing.Union[int, float],
+    provider_latency: typing.Union[int, float]
 
     # Raw output from the provider.
-    "raw_output": str,
+    raw_output: str
 
     # Reason the generation finished.
-    "finish_reason": str,
-    }, total=False)
+    finish_reason: str
 
 class LogResponse(RequiredLogResponse, OptionalLogResponse):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/logs_log_response.py` & `humanloop-0.4.3/humanloop/type/logs_log_response.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/type/model_config_chat_request.py` & `humanloop-0.4.3/humanloop/type/log_model_config_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,46 +14,47 @@
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.chat_message import ChatMessage
 from humanloop.type.model_endpoints import ModelEndpoints
 from humanloop.type.model_providers import ModelProviders
 
-RequiredModelConfigChatRequest = TypedDict("RequiredModelConfigChatRequest", {
+class RequiredLogModelConfigRequest(TypedDict):
     # The model instance used. E.g. text-davinci-002.
-    "model": str,
-    })
+    model: str
 
-OptionalModelConfigChatRequest = TypedDict("OptionalModelConfigChatRequest", {
+class OptionalLogModelConfigRequest(TypedDict, total=False):
     # The company providing the underlying model service.
-    "provider": ModelProviders,
+    provider: ModelProviders
 
     # The maximum number of tokens to generate. Provide max_tokens=-1 to dynamically calculate the maximum number of tokens to generate given the length of the prompt
-    "max_tokens": int,
+    max_tokens: int
 
     # What sampling temperature to use when making a generation. Higher values means the model will be more creative.
-    "temperature": typing.Union[int, float],
+    temperature: typing.Union[int, float]
 
     # An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with top_p probability mass.
-    "top_p": typing.Union[int, float],
+    top_p: typing.Union[int, float]
 
     # The string (or list of strings) after which the model will stop generating. The returned text will not contain the stop sequence.
-    "stop": typing.Union[str, typing.List[str]],
+    stop: typing.Union[str, typing.List[str]]
 
     # Number between -2.0 and 2.0. Positive values penalize new tokens based on whether they appear in the generation so far.
-    "presence_penalty": typing.Union[int, float],
+    presence_penalty: typing.Union[int, float]
 
     # Number between -2.0 and 2.0. Positive values penalize new tokens based on how frequently they appear in the generation so far.
-    "frequency_penalty": typing.Union[int, float],
+    frequency_penalty: typing.Union[int, float]
 
     # Other parameter values to be passed to the provider call.
-    "other": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    other: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
     # The provider model endpoint used.
-    "endpoint": ModelEndpoints,
+    endpoint: ModelEndpoints
+
+    # Prompt template that will take your specified inputs to form your final request to the model. Input variables within the prompt template should be specified with syntax: {{INPUT_NAME}}.
+    prompt_template: str
 
     # Messages prepended to the list of messages sent to the provider. These messages that will take your specified inputs to form your final request to the provider model. Input variables within the template should be specified with syntax: {{INPUT_NAME}}.
-    "chat_template": typing.List[ChatMessage],
-    }, total=False)
+    chat_template: typing.List[ChatMessage]
 
-class ModelConfigChatRequest(RequiredModelConfigChatRequest, OptionalModelConfigChatRequest):
+class LogModelConfigRequest(RequiredLogModelConfigRequest, OptionalLogModelConfigRequest):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/model_config_completion_request.py` & `humanloop-0.4.3/humanloop/type/model_config_completion_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,46 +13,44 @@
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.model_endpoints import ModelEndpoints
 from humanloop.type.model_providers import ModelProviders
 
-RequiredModelConfigCompletionRequest = TypedDict("RequiredModelConfigCompletionRequest", {
+class RequiredModelConfigCompletionRequest(TypedDict):
     # The model instance used. E.g. text-davinci-002.
-    "model": str,
+    model: str
 
     # Prompt template that will take your specified inputs to form your final request to the model. Input variables within the prompt template should be specified with syntax: {{INPUT_NAME}}.
-    "prompt_template": str,
-    })
+    prompt_template: str
 
-OptionalModelConfigCompletionRequest = TypedDict("OptionalModelConfigCompletionRequest", {
+class OptionalModelConfigCompletionRequest(TypedDict, total=False):
     # The company providing the underlying model service.
-    "provider": ModelProviders,
+    provider: ModelProviders
 
     # The maximum number of tokens to generate. Provide max_tokens=-1 to dynamically calculate the maximum number of tokens to generate given the length of the prompt
-    "max_tokens": int,
+    max_tokens: int
 
     # What sampling temperature to use when making a generation. Higher values means the model will be more creative.
-    "temperature": typing.Union[int, float],
+    temperature: typing.Union[int, float]
 
     # An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with top_p probability mass.
-    "top_p": typing.Union[int, float],
+    top_p: typing.Union[int, float]
 
     # The string (or list of strings) after which the model will stop generating. The returned text will not contain the stop sequence.
-    "stop": typing.Union[str, typing.List[str]],
+    stop: typing.Union[str, typing.List[str]]
 
     # Number between -2.0 and 2.0. Positive values penalize new tokens based on whether they appear in the generation so far.
-    "presence_penalty": typing.Union[int, float],
+    presence_penalty: typing.Union[int, float]
 
     # Number between -2.0 and 2.0. Positive values penalize new tokens based on how frequently they appear in the generation so far.
-    "frequency_penalty": typing.Union[int, float],
+    frequency_penalty: typing.Union[int, float]
 
     # Other parameter values to be passed to the provider call.
-    "other": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    other: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
     # The provider model endpoint used.
-    "endpoint": ModelEndpoints,
-    }, total=False)
+    endpoint: ModelEndpoints
 
 class ModelConfigCompletionRequest(RequiredModelConfigCompletionRequest, OptionalModelConfigCompletionRequest):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/model_endpoints.py` & `humanloop-0.4.3/humanloop/type/model_endpoints.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/type/model_providers.py` & `humanloop-0.4.3/humanloop/type/model_providers.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/type/paginated_data_log_response.py` & `humanloop-0.4.3/humanloop/type/paginated_data_log_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,22 +12,21 @@
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.log_response import LogResponse
 
-RequiredPaginatedDataLogResponse = TypedDict("RequiredPaginatedDataLogResponse", {
-    "records": typing.List[LogResponse],
+class RequiredPaginatedDataLogResponse(TypedDict):
+    records: typing.List[LogResponse]
 
-    "page": int,
+    page: int
 
-    "size": int,
+    size: int
 
-    "total": int,
-    })
+    total: int
 
-OptionalPaginatedDataLogResponse = TypedDict("OptionalPaginatedDataLogResponse", {
-    }, total=False)
+class OptionalPaginatedDataLogResponse(TypedDict, total=False):
+    pass
 
 class PaginatedDataLogResponse(RequiredPaginatedDataLogResponse, OptionalPaginatedDataLogResponse):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/paginated_data_project_response.py` & `humanloop-0.4.3/humanloop/type/paginated_data_project_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,22 +12,21 @@
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.project_response import ProjectResponse
 
-RequiredPaginatedDataProjectResponse = TypedDict("RequiredPaginatedDataProjectResponse", {
-    "records": typing.List[ProjectResponse],
+class RequiredPaginatedDataProjectResponse(TypedDict):
+    records: typing.List[ProjectResponse]
 
-    "page": int,
+    page: int
 
-    "size": int,
+    size: int
 
-    "total": int,
-    })
+    total: int
 
-OptionalPaginatedDataProjectResponse = TypedDict("OptionalPaginatedDataProjectResponse", {
-    }, total=False)
+class OptionalPaginatedDataProjectResponse(TypedDict, total=False):
+    pass
 
 class PaginatedDataProjectResponse(RequiredPaginatedDataProjectResponse, OptionalPaginatedDataProjectResponse):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/positive_label.py` & `humanloop-0.4.3/humanloop/type/tool_config_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,18 +11,22 @@
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 
-RequiredPositiveLabel = TypedDict("RequiredPositiveLabel", {
-    "type": str,
+class RequiredToolConfigRequest(TypedDict):
+    source: str
 
-    "value": str,
-    })
+    type: str
 
-OptionalPositiveLabel = TypedDict("OptionalPositiveLabel", {
-    }, total=False)
+class OptionalToolConfigRequest(TypedDict, total=False):
+    description: str
 
-class PositiveLabel(RequiredPositiveLabel, OptionalPositiveLabel):
+    name: str
+
+    # Other parameters that define the config.
+    other: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
+
+class ToolConfigRequest(RequiredToolConfigRequest, OptionalToolConfigRequest):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/project_model_config_request.py` & `humanloop-0.4.3/humanloop/type/model_config_response2.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,61 +11,63 @@
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.chat_message import ChatMessage
+from humanloop.type.config_type import ConfigType
 from humanloop.type.model_endpoints import ModelEndpoints
 from humanloop.type.model_providers import ModelProviders
 
-RequiredProjectModelConfigRequest = TypedDict("RequiredProjectModelConfigRequest", {
-    # What model instance to use for the generation. e.g. text-davinci-002.
-    "model": str,
-
-    # Unique project name. If it does not exist, a new project will be created.
-    "project": str,
-    })
+class RequiredModelConfigResponse2(TypedDict):
+    # String ID of config. Starts with `config_`.
+    id: str
+
+    # Type of config.
+    type: ConfigType
+
+    # Name of config.
+    name: str
+
+    # The model instance used. E.g. text-davinci-002.
+    model: str
+
+class OptionalModelConfigResponse2(TypedDict, total=False):
+    # Description of config.
+    description: str
 
-OptionalProjectModelConfigRequest = TypedDict("OptionalProjectModelConfigRequest", {
-    # The company providing the underlying model service.
-    "provider": ModelProviders,
-
-    # Which of the providers model endpoints to use. For example Complete or Edit.
-    "endpoint": ModelEndpoints,
+    # Other parameter values to be passed to the provider call.
+    other: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
-    # Prompt template that will take your specified inputs to form your final request to the provider model. NB: Input variables within the prompt template should be specified with syntax: {{INPUT_NAME}}.
-    "prompt_template": str,
+    # The company providing the underlying model service.
+    provider: ModelProviders
 
-    # Messages prepended to the list of messages sent to the provider. These messages that will take your specified inputs to form your final request to the provider model. NB: Input variables within the prompt template should be specified with syntax: {{INPUT_NAME}}.
-    "chat_template": typing.List[ChatMessage],
+    # The maximum number of tokens to generate. Provide max_tokens=-1 to dynamically calculate the maximum number of tokens to generate given the length of the prompt
+    max_tokens: int
 
     # What sampling temperature to use when making a generation. Higher values means the model will be more creative.
-    "temperature": typing.Union[int, float],
-
-    # The maximum number of tokens to generate in the completion.
-    "max_tokens": int,
+    temperature: typing.Union[int, float]
 
     # An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with top_p probability mass.
-    "top_p": typing.Union[int, float],
+    top_p: typing.Union[int, float]
 
     # The string (or list of strings) after which the model will stop generating. The returned text will not contain the stop sequence.
-    "stop": typing.Union[str, typing.List[str]],
+    stop: typing.Union[str, typing.List[str]]
 
     # Number between -2.0 and 2.0. Positive values penalize new tokens based on whether they appear in the generation so far.
-    "presence_penalty": typing.Union[int, float],
+    presence_penalty: typing.Union[int, float]
 
     # Number between -2.0 and 2.0. Positive values penalize new tokens based on how frequently they appear in the generation so far.
-    "frequency_penalty": typing.Union[int, float],
+    frequency_penalty: typing.Union[int, float]
 
-    # Other parameter values to be passed to the provider call.
-    "other": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    # Prompt template that will take your specified inputs to form your final request to the model. NB: Input variables within the prompt template should be specified with syntax: {{INPUT_NAME}}.
+    prompt_template: str
 
-    # A friendly display name for the model config. If not provided, a name will be generated.
-    "name": str,
+    # Messages prepended to the list of messages sent to the provider. These messages that will take your specified inputs to form your final request to the provider model. NB: Input variables within the template should be specified with syntax: {{INPUT_NAME}}.
+    chat_template: typing.List[ChatMessage]
 
-    # If specified, the model config will be added to this experiment. Experiments are used for A/B testing and optimizing hyperparameters.
-    "experiment": str,
-    }, total=False)
+    # The provider model endpoint used.
+    endpoint: ModelEndpoints
 
-class ProjectModelConfigRequest(RequiredProjectModelConfigRequest, OptionalProjectModelConfigRequest):
+class ModelConfigResponse2(RequiredModelConfigResponse2, OptionalModelConfigResponse2):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/project_response.py` & `humanloop-0.4.3/humanloop/type/project_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,48 +10,49 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
+from humanloop.type.config_type import ConfigType
 from humanloop.type.experiment_response import ExperimentResponse
 from humanloop.type.feedback_types import FeedbackTypes
+from humanloop.type.project_config_response import ProjectConfigResponse
 from humanloop.type.project_user_response import ProjectUserResponse
-from humanloop.type.src_external_app_models_v4_model_configs_project_model_config_response import SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse
 
-RequiredProjectResponse = TypedDict("RequiredProjectResponse", {
+class RequiredProjectResponse(TypedDict):
     # Project ID
-    "id": str,
+    id: str
 
     # Project ID for internal Humanloop use.
-    "internal_id": int,
+    internal_id: int
 
     # Unique project name.
-    "name": str,
+    name: str
 
     # Users associated to the project.
-    "users": typing.List[ProjectUserResponse],
+    users: typing.List[ProjectUserResponse]
 
     # The count of datapoints that have been logged to the project.
-    "data_count": int,
+    data_count: int
 
-    "feedback_types": FeedbackTypes,
+    feedback_types: FeedbackTypes
 
     # Unique ID of the team the project belongs to. Starts with `tm_`.
-    "team_id": str,
+    team_id: str
 
-    "created_at": datetime,
+    created_at: datetime
 
-    "updated_at": datetime,
-    })
+    updated_at: datetime
 
-OptionalProjectResponse = TypedDict("OptionalProjectResponse", {
+class OptionalProjectResponse(TypedDict, total=False):
     # Experiment that has been set as the project's active deployment. At most one of active_experiment and active_model_config can be set.
-    "active_experiment": ExperimentResponse,
+    active_experiment: ExperimentResponse
 
-    # Model configuration that has been set as the project's active deployment. At most one of active_experiment and active_model_config can be set.
-    "active_model_config": SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse,
-    }, total=False)
+    # Config that has been set as the project's active deployment. At most one of active_experiment and active_model_config can be set.
+    active_config: ProjectConfigResponse
+
+    config_type: ConfigType
 
 class ProjectResponse(RequiredProjectResponse, OptionalProjectResponse):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/project_sort_by.py` & `humanloop-0.4.3/humanloop/type/project_sort_by.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/type/project_user_response.py` & `humanloop-0.4.3/humanloop/type/project_user_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,22 +11,20 @@
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 
-RequiredProjectUserResponse = TypedDict("RequiredProjectUserResponse", {
+class RequiredProjectUserResponse(TypedDict):
     # String ID of user. Starts with `usr_`.
-    "id": str,
+    id: str
 
     # The user's email address.
-    "email_address": str,
-    })
+    email_address: str
 
-OptionalProjectUserResponse = TypedDict("OptionalProjectUserResponse", {
+class OptionalProjectUserResponse(TypedDict, total=False):
     # The user's full name.
-    "full_name": str,
-    }, total=False)
+    full_name: str
 
 class ProjectUserResponse(RequiredProjectUserResponse, OptionalProjectUserResponse):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/projects_get_model_configs_response.py` & `humanloop-0.4.3/humanloop/type/tool_config_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,10 +10,31 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
-from humanloop.type.src_external_app_models_v4_model_configs_project_model_config_response import SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse
+from humanloop.type.config_type import ConfigType
 
-ProjectsGetModelConfigsResponse = typing.List[SrcExternalAppModelsV4ModelConfigsProjectModelConfigResponse]
+class RequiredToolConfigResponse(TypedDict):
+    # String ID of config. Starts with `config_`.
+    id: str
+
+    # Type of config.
+    type: ConfigType
+
+    # Name of config.
+    name: str
+
+    # Code source of the tool.
+    source: str
+
+class OptionalToolConfigResponse(TypedDict, total=False):
+    # Description of config.
+    description: str
+
+    # Other parameters that define the config.
+    other: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
+
+class ToolConfigResponse(RequiredToolConfigResponse, OptionalToolConfigResponse):
+    pass
```

### Comparing `humanloop-0.4.2/humanloop/type/projects_update_feedback_types_request.py` & `humanloop-0.4.3/humanloop/type/projects_update_feedback_types_request.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/type/provider_api_keys.py` & `humanloop-0.4.3/humanloop/type/generic_config_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,22 +11,20 @@
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 
-RequiredProviderApiKeys = TypedDict("RequiredProviderApiKeys", {
-    })
+class RequiredGenericConfigRequest(TypedDict):
+    type: str
 
-OptionalProviderApiKeys = TypedDict("OptionalProviderApiKeys", {
-    "openai": str,
+class OptionalGenericConfigRequest(TypedDict, total=False):
+    description: str
 
-    "ai21": str,
+    name: str
 
-    "mock": str,
+    # Other parameters that define the config.
+    other: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
 
-    "anthropic": str,
-    }, total=False)
-
-class ProviderApiKeys(RequiredProviderApiKeys, OptionalProviderApiKeys):
+class GenericConfigRequest(RequiredGenericConfigRequest, OptionalGenericConfigRequest):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/session_app_response.py` & `humanloop-0.4.3/humanloop/type/session_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,21 +10,30 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
+from humanloop.type.session_project_response import SessionProjectResponse
 
-RequiredSessionAppResponse = TypedDict("RequiredSessionAppResponse", {
-    # String ID of app. Starts with `app_`.
-    "id": str,
-
-    "name": str,
-    })
-
-OptionalSessionAppResponse = TypedDict("OptionalSessionAppResponse", {
-    "description": str,
-    }, total=False)
+class RequiredSessionResponse(TypedDict):
+    # String ID of session. Starts with `sesh_`.
+    id: str
 
-class SessionAppResponse(RequiredSessionAppResponse, OptionalSessionAppResponse):
+    # List of projects that have datapoints associated to this session.
+    projects: typing.List[SessionProjectResponse]
+
+    # Number of datapoints associated to this session.
+    datapoints_count: int
+
+    created_at: datetime
+
+class OptionalSessionResponse(TypedDict, total=False):
+    # Inputs for the first datapoint in the session.
+    first_inputs: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
+
+    # Output for the last datapoint in the session.
+    last_output: str
+
+class SessionResponse(RequiredSessionResponse, OptionalSessionResponse):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/session_response.py` & `humanloop-0.4.3/humanloop/type/feedback_label_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,24 +10,17 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
-from humanloop.type.session_app_response import SessionAppResponse
+from humanloop.type.label_sentiment import LabelSentiment
 
-RequiredSessionResponse = TypedDict("RequiredSessionResponse", {
-    "id": str,
+class RequiredFeedbackLabelRequest(TypedDict):
+    value: str
 
-    "app": SessionAppResponse,
+class OptionalFeedbackLabelRequest(TypedDict, total=False):
+    sentiment: LabelSentiment
 
-    "created_at": datetime,
-
-    "updated_at": datetime,
-    })
-
-OptionalSessionResponse = TypedDict("OptionalSessionResponse", {
-    }, total=False)
-
-class SessionResponse(RequiredSessionResponse, OptionalSessionResponse):
+class FeedbackLabelRequest(RequiredFeedbackLabelRequest, OptionalFeedbackLabelRequest):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/sort_order.py` & `humanloop-0.4.3/humanloop/type/sort_order.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/type/src_external_app_models_v3_model_configs_model_config_response.py` & `humanloop-0.4.3/humanloop/type/trace_model_config_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,55 +14,53 @@
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.chat_message import ChatMessage
 from humanloop.type.model_endpoints import ModelEndpoints
 from humanloop.type.model_providers import ModelProviders
 
-RequiredSrcExternalAppModelsV3ModelConfigsModelConfigResponse = TypedDict("RequiredSrcExternalAppModelsV3ModelConfigsModelConfigResponse", {
-    # What model instance to use for the generation. e.g. text-davinci-002.
-    "model": str,
-
-    # Model config unique identifier generated by Humanloop.
-    "id": str,
-    })
+class RequiredTraceModelConfigRequest(TypedDict):
+    # The model instance used. E.g. text-davinci-002.
+    model: str
 
-OptionalSrcExternalAppModelsV3ModelConfigsModelConfigResponse = TypedDict("OptionalSrcExternalAppModelsV3ModelConfigsModelConfigResponse", {
-    # The company providing the underlying model service.
-    "provider": ModelProviders,
+    type: str
 
-    # Which of the providers model endpoints to use. For example Complete or Edit.
-    "endpoint": ModelEndpoints,
+class OptionalTraceModelConfigRequest(TypedDict, total=False):
+    description: str
 
-    # Prompt template that will take your specified inputs to form your final request to the provider model. NB: Input variables within the prompt template should be specified with syntax: {{INPUT_NAME}}.
-    "prompt_template": str,
+    name: str
 
-    # Messages prepended to the list of messages sent to the provider. These messages that will take your specified inputs to form your final request to the provider model. NB: Input variables within the prompt template should be specified with syntax: {{INPUT_NAME}}.
-    "chat_template": typing.List[ChatMessage],
+    # The company providing the underlying model service.
+    provider: ModelProviders
 
-    # What sampling temperature to use when making a generation. Higher values means the model will be more creative.
-    "temperature": typing.Union[int, float],
+    # The maximum number of tokens to generate. Provide max_tokens=-1 to dynamically calculate the maximum number of tokens to generate given the length of the prompt
+    max_tokens: int
 
-    # The maximum number of tokens to generate in the completion.
-    "max_tokens": int,
+    # What sampling temperature to use when making a generation. Higher values means the model will be more creative.
+    temperature: typing.Union[int, float]
 
     # An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with top_p probability mass.
-    "top_p": typing.Union[int, float],
+    top_p: typing.Union[int, float]
 
     # The string (or list of strings) after which the model will stop generating. The returned text will not contain the stop sequence.
-    "stop": typing.Union[str, typing.List[str]],
+    stop: typing.Union[str, typing.List[str]]
 
     # Number between -2.0 and 2.0. Positive values penalize new tokens based on whether they appear in the generation so far.
-    "presence_penalty": typing.Union[int, float],
+    presence_penalty: typing.Union[int, float]
 
     # Number between -2.0 and 2.0. Positive values penalize new tokens based on how frequently they appear in the generation so far.
-    "frequency_penalty": typing.Union[int, float],
+    frequency_penalty: typing.Union[int, float]
 
     # Other parameter values to be passed to the provider call.
-    "other": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    other: typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]
+
+    # The provider model endpoint used.
+    endpoint: ModelEndpoints
+
+    # Prompt template that will take your specified inputs to form your final request to the model. Input variables within the prompt template should be specified with syntax: {{INPUT_NAME}}.
+    prompt_template: str
 
-    # A friendly display name for the model config.
-    "display_name": str,
-    }, total=False)
+    # Messages prepended to the list of messages sent to the provider. These messages that will take your specified inputs to form your final request to the provider model. Input variables within the template should be specified with syntax: {{INPUT_NAME}}.
+    chat_template: typing.List[ChatMessage]
 
-class SrcExternalAppModelsV3ModelConfigsModelConfigResponse(RequiredSrcExternalAppModelsV3ModelConfigsModelConfigResponse, OptionalSrcExternalAppModelsV3ModelConfigsModelConfigResponse):
+class TraceModelConfigRequest(RequiredTraceModelConfigRequest, OptionalTraceModelConfigRequest):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py` & `humanloop-0.4.3/humanloop/type/src_external_app_models_v3_model_configs_project_model_config_feedback_stats_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,22 +11,21 @@
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 
-RequiredSrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse = TypedDict("RequiredSrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse", {
-    "feedback_type_id": int,
+class RequiredSrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse(TypedDict):
+    feedback_type_id: int
 
-    "feedback_type": str,
+    feedback_type: str
 
-    "feedback_value": str,
+    feedback_value: str
 
-    "feedback_count": int,
-    })
+    feedback_count: int
 
-OptionalSrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse = TypedDict("OptionalSrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse", {
-    }, total=False)
+class OptionalSrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse(TypedDict, total=False):
+    pass
 
 class SrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse(RequiredSrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse, OptionalSrcExternalAppModelsV3ModelConfigsProjectModelConfigFeedbackStatsResponse):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/tool_result_response.py` & `humanloop-0.4.3/humanloop/type/projects_get_configs_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,23 +10,10 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
+from humanloop.type.project_config_response import ProjectConfigResponse
 
-RequiredToolResultResponse = TypedDict("RequiredToolResultResponse", {
-    "id": str,
-
-    "name": str,
-
-    "signature": str,
-
-    "result": str,
-    })
-
-OptionalToolResultResponse = TypedDict("OptionalToolResultResponse", {
-    }, total=False)
-
-class ToolResultResponse(RequiredToolResultResponse, OptionalToolResultResponse):
-    pass
+ProjectsGetConfigsResponse = typing.List[ProjectConfigResponse]
```

### Comparing `humanloop-0.4.2/humanloop/type/update_experiment_request.py` & `humanloop-0.4.3/humanloop/type/create_experiment_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,26 +12,23 @@
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.positive_label import PositiveLabel
 
-RequiredUpdateExperimentRequest = TypedDict("RequiredUpdateExperimentRequest", {
-    })
-
-OptionalUpdateExperimentRequest = TypedDict("OptionalUpdateExperimentRequest", {
+class RequiredCreateExperimentRequest(TypedDict):
     # Name of experiment.
-    "name": str,
+    name: str
 
     # Feedback labels to treat as positive user feedback. Used to monitor the performance of model configs in the experiment.
-    "positive_labels": typing.List[PositiveLabel],
+    positive_labels: typing.List[PositiveLabel]
 
-    # Model configs to add to this experiment.
-    "config_ids_to_register": typing.List[str],
+class OptionalCreateExperimentRequest(TypedDict, total=False):
+    # Configs to add to this experiment. Further configs can be added later.
+    config_ids: typing.List[str]
 
-    # Model configs in this experiment to be deactivated.
-    "config_ids_to_deregister": typing.List[str],
-    }, total=False)
+    # Whether to set the created project as the project's active experiment.
+    set_active: bool
 
-class UpdateExperimentRequest(RequiredUpdateExperimentRequest, OptionalUpdateExperimentRequest):
+class CreateExperimentRequest(RequiredCreateExperimentRequest, OptionalCreateExperimentRequest):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/update_project_request.py` & `humanloop-0.4.3/humanloop/type/update_project_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,23 +12,22 @@
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 from humanloop.type.positive_label import PositiveLabel
 
-RequiredUpdateProjectRequest = TypedDict("RequiredUpdateProjectRequest", {
-    })
+class RequiredUpdateProjectRequest(TypedDict):
+    pass
 
-OptionalUpdateProjectRequest = TypedDict("OptionalUpdateProjectRequest", {
+class OptionalUpdateProjectRequest(TypedDict, total=False):
     # ID for an experiment to set as the project's active deployment. Starts with 'exp_'. At most one of 'active_experiment_id' and 'active_model_config_id' can be set.
-    "active_experiment_id": str,
+    active_experiment_id: str
 
-    # ID for a model configuration to set as the project's active deployment. Starts with 'config_'. At most one of 'active_experiment_id' and 'active_model_config_id' can be set.
-    "active_model_config_id": str,
+    # ID for a config to set as the project's active deployment. Starts with 'config_'. At most one of 'active_experiment_id' and 'active_config_id' can be set.
+    active_config_id: str
 
     # The full list of labels to treat as positive user feedback.
-    "positive_labels": typing.List[PositiveLabel],
-    }, total=False)
+    positive_labels: typing.List[PositiveLabel]
 
 class UpdateProjectRequest(RequiredUpdateProjectRequest, OptionalUpdateProjectRequest):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/usage.py` & `humanloop-0.4.3/humanloop/type/usage.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,23 +11,22 @@
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 
-RequiredUsage = TypedDict("RequiredUsage", {
+class RequiredUsage(TypedDict):
     # Number of tokens used in the prompt.
-    "prompt_tokens": int,
+    prompt_tokens: int
 
     # Number of tokens produced by the generation.
-    "generation_tokens": int,
+    generation_tokens: int
 
     # Total number of tokens used by the prompt and generation combined.
-    "total_tokens": int,
-    })
+    total_tokens: int
 
-OptionalUsage = TypedDict("OptionalUsage", {
-    }, total=False)
+class OptionalUsage(TypedDict, total=False):
+    pass
 
 class Usage(RequiredUsage, OptionalUsage):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type/validation_error.py` & `humanloop-0.4.3/humanloop/type/validation_error.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,20 +11,19 @@
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal
 
 
-RequiredValidationError = TypedDict("RequiredValidationError", {
-    "loc": typing.List[typing.Union[typing.List[str], typing.List[int]]],
+class RequiredValidationError(TypedDict):
+    loc: typing.List[typing.Union[typing.List[str], typing.List[int]]]
 
-    "msg": str,
+    msg: str
 
-    "type": str,
-    })
+    type: str
 
-OptionalValidationError = TypedDict("OptionalValidationError", {
-    }, total=False)
+class OptionalValidationError(TypedDict, total=False):
+    pass
 
 class ValidationError(RequiredValidationError, OptionalValidationError):
     pass
```

### Comparing `humanloop-0.4.2/humanloop/type_util.py` & `humanloop-0.4.3/humanloop/type_util.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/humanloop/validation_metadata.py` & `humanloop-0.4.3/humanloop/validation_metadata.py`

 * *Files identical despite different names*

### Comparing `humanloop-0.4.2/pyproject.toml` & `humanloop-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "humanloop"
-version = "0.4.2"
+version = "0.4.3"
 description = "Client for Humanloop API"
 authors = ["Konfig <engineering@konfigthis.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "humanloop"}]
 
 [tool.poetry.dependencies]
```

### Comparing `humanloop-0.4.2/PKG-INFO` & `humanloop-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: humanloop
-Version: 0.4.2
+Version: 0.4.3
 Summary: Client for Humanloop API
 License: MIT
 Author: Konfig
 Author-email: engineering@konfigthis.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,25 +18,25 @@
 Requires-Dist: frozendict (>=2.3.4,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: typing_extensions (>=4.3.0,<5.0.0)
 Requires-Dist: urllib3 (>=1.26.7,<2.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Description-Content-Type: text/markdown
 
-# humanloop@0.4.2
+# humanloop@0.4.3
 
 
 ## Requirements
 
 Python >=3.7
 
 ## Installing
 
 ```sh
-pip install humanloop==0.4.2
+pip install humanloop==0.4.3
 ```
 
 ## Getting Started
 
 ```python
 from pprint import pprint
 from humanloop import Humanloop, ApiException
```

