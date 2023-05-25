# Comparing `tmp/dojah-python-sdk-3.0.0.tar.gz` & `tmp/dojah_python_sdk-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dojah-python-sdk-3.0.0.tar", last modified: Wed Feb 15 15:00:57 2023, max compression
+gzip compressed data, was "dojah_python_sdk-4.0.0.tar", max compression
```

## Comparing `dojah-python-sdk-3.0.0.tar` & `dojah_python_sdk-4.0.0.tar`

### file list

```diff
@@ -1,397 +1,562 @@
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-02-15 15:00:57.715857 dojah-python-sdk-3.0.0/
--rw-r--r--   0 dylanhuang   (501) staff       (20)    24441 2023-02-15 15:00:57.715989 dojah-python-sdk-3.0.0/PKG-INFO
--rw-r--r--   0 dylanhuang   (501) staff       (20)    24144 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/README.md
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-02-15 15:00:57.602610 dojah-python-sdk-3.0.0/dojah_client/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      707 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/__init__.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-02-15 15:00:57.606992 dojah-python-sdk-3.0.0/dojah_client/api/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      212 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/api/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    10760 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/api/aml_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    30610 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/api/authentication_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    51101 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/api/financial_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    35073 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/api/general_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    17245 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/api/ghkyc_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     6829 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/api/kekyc_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    20991 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/api/kyb_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    82262 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/api/kyc_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    21479 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/api/ml_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     6055 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/api/services_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     6077 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/api/ugkyc_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    30697 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/api/wallet_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    20347 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/api/web_hooks_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    39028 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/api_client.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-02-15 15:00:57.607308 dojah-python-sdk-3.0.0/dojah_client/apis/
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1068 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/apis/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    17491 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/configuration.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5055 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/exceptions.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-02-15 15:00:57.652196 dojah-python-sdk-3.0.0/dojah_client/model/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      346 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11704 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/analyze_document_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    13475 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/analyze_document_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11921 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/analyze_document_response_entity_document_images.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12467 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/analyze_document_response_entity_document_type.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12289 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/analyze_document_response_entity_status.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12053 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/analyze_document_response_entity_text_data_inner.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11636 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/categorize_transactions_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11774 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/categorize_transactions_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12937 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/categorize_transactions_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11633 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/collect_status_from_pdf_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11747 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/collect_status_from_pdf_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12036 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/collect_transactions_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12492 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/collect_transactions_request_transactions_inner.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11937 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/collect_transactions_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11435 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/collect_transactions_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12170 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/create_wallet_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11674 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/create_wallet_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12084 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/create_wallet_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11585 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/credit_subwallet_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11704 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/credit_subwallet_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    13679 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/credit_subwallet_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11379 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/delete_webhook_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11756 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/financial_get_basic_bvn_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12398 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/financial_get_basic_bvn_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11746 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/financial_get_full_bvn_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    16632 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/financial_get_full_bvn_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11705 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/general_get_nuban_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11661 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/general_get_nuban_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11736 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/general_get_wallet_balance_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11735 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_account_analysis_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    14760 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_account_analysis_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    14969 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_account_analysis_response_entity_account_breakdown.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    24690 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_account_analysis_response_entity_expense_breakdown.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    15678 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_account_analysis_response_entity_funds_management.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    14455 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_account_analysis_response_entity_inflow_breakdown.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    19181 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_account_analysis_response_entity_transaction_routine_breakdown.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12598 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_account_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11785 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_account_subscriptions_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12526 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_account_subscriptions_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11775 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_account_transactions_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    13014 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_account_transactions_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12912 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_account_transactions_response_entity_transactions_inner.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11674 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_advanced_cac_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11676 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_banks_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12558 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_banks_response_entity_inner.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11665 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_basic_bvn_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12371 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_basic_bvn_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11665 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_basic_cac_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12308 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_basic_cac_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11746 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_basic_phone_number_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    13876 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_basic_phone_number_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11614 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_bin_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12564 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_bin_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11614 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_cac_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12060 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_cac_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11716 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_data_plans_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11379 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_document_analysis_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11745 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_document_analysis_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11782 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_document_analysis_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    15513 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_document_analysis_response_entity_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11725 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_drivers_license_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    13799 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_drivers_license_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11745 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_earning_structure_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12172 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_earning_structure_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11735 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_email_reputation_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12624 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_email_reputation_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    16673 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_email_reputation_response_entity_details.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11655 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_full_bvn_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    16808 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_full_bvn_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11373 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_generic_ocr_text_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11676 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_generic_ocr_text_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11756 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_kyc_drivers_license_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11931 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_kyc_drivers_license_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    14861 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_kyc_drivers_license_response_entity_personal_details.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11695 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_kyc_passport_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    13525 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_kyc_passport_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11685 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_national_id_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    13687 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_national_id_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11634 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_nuban_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    15860 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_nuban_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11362 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_ocr_text_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11655 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_ocr_text_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11384 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_ocr_text_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11664 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_passport_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    14709 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_passport_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11704 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_phone_number404_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11695 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_phone_number_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    17561 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_phone_number_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11685 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_premium_bvn_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    16808 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_premium_bvn_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11715 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_screening_info_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11954 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_screening_info_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    17562 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_screening_info_response_entity_result.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11707 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_sender_id_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11834 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_sender_id_response_entity_inner.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11675 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_sms_status_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11394 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_sms_status_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11735 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_spending_pattern_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11808 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_spending_pattern_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    14231 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_spending_pattern_response_entity_pattern.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11860 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_spending_pattern_response_entity_pattern_airtime_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11863 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_spending_pattern_response_entity_pattern_bank_transfer.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11848 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_spending_pattern_response_entity_pattern_charges.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11839 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_spending_pattern_response_entity_pattern_food.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11845 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_spending_pattern_response_entity_pattern_others.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11634 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_ssnit_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    13098 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_ssnit_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11614 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_tin_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12777 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_tin_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11694 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_transaction_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    13676 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_transaction_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11614 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_vin_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    13496 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_vin_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11624 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_vnin_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12946 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_vnin_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11688 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_voter_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    14434 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_voter_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11715 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_wallet_balance_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11446 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_wallet_balance_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11644 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_wallet_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12278 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_wallet_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11654 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_wallets_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12123 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_wallets_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11706 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_webhooks_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12699 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/get_webhooks_response_entity_inner.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11843 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/notify_webhook_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11383 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/notify_webhook_request_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11379 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/notify_webhook_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11595 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/purchase_airtime_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11704 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/purchase_airtime_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12001 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/purchase_airtime_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11643 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/purchase_airtime_response_entity_data_inner.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11576 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/purchase_data_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11716 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/purchase_data_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11806 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/purchase_data_response_entity_inner.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11397 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/request_sender_id_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11747 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/request_sender_id_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11846 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/request_sender_id_response_entity_inner.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11810 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/screen_aml_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11644 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/screen_aml_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11603 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/screen_aml_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12174 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/send_otp_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11666 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/send_otp_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12028 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/send_otp_response_entity_inner.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11972 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/send_sms_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11624 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/send_sms_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11976 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/send_sms_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11583 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/subscribe_service_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11388 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/subscribe_service_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12110 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/transfer_funds_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11684 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/transfer_funds_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    13673 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/transfer_funds_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11664 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/validate_bvn_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12189 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/validate_bvn_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11586 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/validate_bvn_response_entity_bvn.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11665 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/validate_bvn_response_entity_first_name.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11664 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/validate_otp_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11389 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/validate_otp_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11644 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/verify_age_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    12052 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/verify_age_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11659 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/verify_photo_id_with_selfie_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11787 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/verify_photo_id_with_selfie_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11848 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/verify_photo_id_with_selfie_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    13073 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/verify_photo_id_with_selfie_response_entity_selfie.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11585 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/verify_selfie_bvn_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11705 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/verify_selfie_bvn_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    16925 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/verify_selfie_bvn_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11699 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/verify_selfie_bvn_response_entity_selfie_verification.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11585 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/verify_selfie_nin_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11705 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/verify_selfie_nin_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    22314 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/verify_selfie_nin_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    11699 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model/verify_selfie_nin_response_entity_selfie_verification.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    82580 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/model_utils.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-02-15 15:00:57.653195 dojah-python-sdk-3.0.0/dojah_client/models/
--rw-r--r--   0 dylanhuang   (501) staff       (20)    16002 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/models/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    14257 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/dojah_client/rest.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-02-15 15:00:57.654431 dojah-python-sdk-3.0.0/dojah_python_sdk.egg-info/
--rw-r--r--   0 dylanhuang   (501) staff       (20)    24441 2023-02-15 15:00:57.000000 dojah-python-sdk-3.0.0/dojah_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dylanhuang   (501) staff       (20)    18138 2023-02-15 15:00:57.000000 dojah-python-sdk-3.0.0/dojah_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dylanhuang   (501) staff       (20)        1 2023-02-15 15:00:57.000000 dojah-python-sdk-3.0.0/dojah_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dylanhuang   (501) staff       (20)       32 2023-02-15 15:00:57.000000 dojah-python-sdk-3.0.0/dojah_python_sdk.egg-info/requires.txt
--rw-r--r--   0 dylanhuang   (501) staff       (20)       13 2023-02-15 15:00:57.000000 dojah-python-sdk-3.0.0/dojah_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 dylanhuang   (501) staff       (20)       69 2023-02-15 15:00:57.716331 dojah-python-sdk-3.0.0/setup.cfg
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1156 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/setup.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-02-15 15:00:57.714395 dojah-python-sdk-3.0.0/test/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      795 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_aml_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      966 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_analyze_document_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1704 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_analyze_document_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      940 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_analyze_document_response_entity_document_images.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      926 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_analyze_document_response_entity_document_type.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      883 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_analyze_document_response_entity_status.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      934 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_analyze_document_response_entity_text_data_inner.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1446 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_authentication_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      839 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_categorize_transactions_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1043 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_categorize_transactions_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      889 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_categorize_transactions_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      827 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_collect_status_from_pdf_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1019 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_collect_status_from_pdf_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1044 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_collect_transactions_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      939 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_collect_transactions_request_transactions_inner.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1010 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_collect_transactions_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      868 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_collect_transactions_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      769 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_create_wallet_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      933 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_create_wallet_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      819 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_create_wallet_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      790 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_credit_subwallet_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      966 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_credit_subwallet_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      840 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_credit_subwallet_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      783 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_delete_webhook_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     2132 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_financial_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1025 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_financial_get_basic_bvn_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      877 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_financial_get_basic_bvn_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1014 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_financial_get_full_bvn_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      870 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_financial_get_full_bvn_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1541 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_general_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      968 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_general_get_nuban_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      841 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_general_get_nuban_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1029 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_general_get_wallet_balance_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1001 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_account_analysis_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     2139 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_account_analysis_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      976 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_account_analysis_response_entity_account_breakdown.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      976 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_account_analysis_response_entity_expense_breakdown.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      969 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_account_analysis_response_entity_funds_management.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      969 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_account_analysis_response_entity_inflow_breakdown.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1054 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_account_analysis_response_entity_transaction_routine_breakdown.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      762 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_account_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1056 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_account_subscriptions_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      897 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_account_subscriptions_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1045 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_account_transactions_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1158 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_account_transactions_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1011 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_account_transactions_response_entity_transactions_inner.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      945 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_advanced_cac_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      910 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_banks_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      827 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_banks_response_entity_inner.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      924 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_basic_bvn_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      813 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_basic_bvn_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      924 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_basic_cac_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      813 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_basic_cac_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1014 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_basic_phone_number_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      870 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_basic_phone_number_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      867 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_bin_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      777 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_bin_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      867 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_cac_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      777 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_cac_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      955 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_data_plans_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      819 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_document_analysis_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1012 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_document_analysis_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1072 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_document_analysis_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      898 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_document_analysis_response_entity_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      990 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_drivers_license_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      855 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_drivers_license_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1012 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_earning_structure_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      869 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_earning_structure_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1001 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_email_reputation_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1073 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_email_reputation_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      912 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_email_reputation_response_entity_details.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      913 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_full_bvn_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      806 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_full_bvn_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      806 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_generic_ocr_text_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      963 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_generic_ocr_text_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1025 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_kyc_drivers_license_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1130 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_kyc_drivers_license_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      984 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_kyc_drivers_license_response_entity_personal_details.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      957 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_kyc_passport_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      834 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_kyc_passport_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      946 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_national_id_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      827 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_national_id_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      889 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_nuban_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      791 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_nuban_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      756 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_ocr_text_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      913 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_ocr_text_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      806 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_ocr_text_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      922 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_passport_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      812 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_passport_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      978 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_phone_number404_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      957 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_phone_number_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      834 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_phone_number_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      946 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_premium_bvn_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      827 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_premium_bvn_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      979 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_screening_info_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1047 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_screening_info_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      891 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_screening_info_response_entity_result.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      945 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_sender_id_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      849 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_sender_id_response_entity_inner.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      935 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_sms_status_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      820 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_sms_status_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1001 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_spending_pattern_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1073 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_spending_pattern_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     2134 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_spending_pattern_response_entity_pattern.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      991 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_spending_pattern_response_entity_pattern_airtime_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      998 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_spending_pattern_response_entity_pattern_bank_transfer.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      962 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_spending_pattern_response_entity_pattern_charges.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      941 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_spending_pattern_response_entity_pattern_food.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      955 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_spending_pattern_response_entity_pattern_others.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      889 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_ssnit_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      791 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_ssnit_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      867 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_tin_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      777 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_tin_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      955 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_transaction_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      833 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_transaction_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      867 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_vin_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      777 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_vin_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      878 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_vnin_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      784 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_vnin_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      889 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_voter_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      791 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_voter_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      979 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_wallet_balance_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      848 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_wallet_balance_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      900 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_wallet_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      798 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_wallet_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      911 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_wallets_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      950 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_wallets_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      943 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_webhooks_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      848 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_get_webhooks_response_entity_inner.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1695 2023-02-03 04:57:38.000000 dojah-python-sdk-3.0.0/test/test_ghkyc_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      674 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_kekyc_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1060 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_kyb_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     2888 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_kyc_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1156 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_ml_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      925 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_notify_webhook_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      805 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_notify_webhook_request_data.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      783 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_notify_webhook_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      790 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_purchase_airtime_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      966 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_purchase_airtime_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1047 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_purchase_airtime_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      905 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_purchase_airtime_response_entity_data_inner.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      769 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_purchase_data_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      954 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_purchase_data_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      855 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_purchase_data_response_entity_inner.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      791 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_request_sender_id_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      989 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_request_sender_id_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      877 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_request_sender_id_response_entity_inner.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      748 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_screen_aml_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      900 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_screen_aml_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      798 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_screen_aml_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      734 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_send_otp_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      899 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_send_otp_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      820 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_send_otp_response_entity_inner.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      734 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_send_sms_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      878 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_send_sms_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      784 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_send_sms_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      711 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_services_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      797 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_subscribe_service_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      804 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_subscribe_service_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      776 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_transfer_funds_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      944 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_transfer_funds_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      826 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_transfer_funds_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      654 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_ugkyc_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      922 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_validate_bvn_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1169 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_validate_bvn_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      834 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_validate_bvn_response_entity_bvn.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      877 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_validate_bvn_response_entity_first_name.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      922 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_validate_otp_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      812 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_validate_otp_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      900 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_verify_age_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      798 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_verify_age_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      849 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_verify_photo_id_with_selfie_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1060 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_verify_photo_id_with_selfie_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1128 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_verify_photo_id_with_selfie_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      942 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_verify_photo_id_with_selfie_response_entity_selfie.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      791 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_verify_selfie_bvn_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      968 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_verify_selfie_bvn_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1085 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_verify_selfie_bvn_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      969 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_verify_selfie_bvn_response_entity_selfie_verification.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      791 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_verify_selfie_nin_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      968 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_verify_selfie_nin_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1085 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_verify_selfie_nin_response_entity.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      969 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_verify_selfie_nin_response_entity_selfie_verification.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1385 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_wallet_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1109 2023-02-15 14:47:20.000000 dojah-python-sdk-3.0.0/test/test_web_hooks_api.py
+-rw-r--r--   0        0        0     1081 2023-05-25 20:48:47.932705 dojah_python_sdk-4.0.0/LICENSE
+-rw-r--r--   0        0        0    18083 2023-05-25 20:48:47.932902 dojah_python_sdk-4.0.0/README.md
+-rw-r--r--   0        0        0      748 2023-05-25 20:48:47.949169 dojah_python_sdk-4.0.0/dojah_client/__init__.py
+-rw-r--r--   0        0        0    72699 2023-05-25 20:48:47.949426 dojah_python_sdk-4.0.0/dojah_client/api_client.py
+-rw-r--r--   0        0        0      663 2023-05-25 20:48:47.949513 dojah_python_sdk-4.0.0/dojah_client/api_response.py
+-rw-r--r--   0        0        0      214 2023-05-25 20:48:47.949649 dojah_python_sdk-4.0.0/dojah_client/apis/__init__.py
+-rw-r--r--   0        0        0    13258 2023-05-25 20:48:47.949725 dojah_python_sdk-4.0.0/dojah_client/apis/path_to_api.py
+-rw-r--r--   0        0        0      239 2023-05-25 20:48:47.949818 dojah_python_sdk-4.0.0/dojah_client/apis/paths/__init__.py
+-rw-r--r--   0        0        0      123 2023-05-25 20:48:47.949876 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_aml_screening.py
+-rw-r--r--   0        0        0      109 2023-05-25 20:48:47.949936 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_balance.py
+-rw-r--r--   0        0        0      131 2023-05-25 20:48:47.949995 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_document_analysis.py
+-rw-r--r--   0        0        0      151 2023-05-25 20:48:47.950066 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_financial_account_information.py
+-rw-r--r--   0        0        0      153 2023-05-25 20:48:47.950134 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_financial_account_transactions.py
+-rw-r--r--   0        0        0      130 2023-05-25 20:48:47.950200 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_financial_analysis.py
+-rw-r--r--   0        0        0      148 2023-05-25 20:48:47.950259 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_financial_transactions_pdf.py
+-rw-r--r--   0        0        0      111 2023-05-25 20:48:47.950317 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_gh_kyc_dl.py
+-rw-r--r--   0        0        0      123 2023-05-25 20:48:47.950370 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_gh_kyc_passport.py
+-rw-r--r--   0        0        0      117 2023-05-25 20:48:47.950426 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_gh_kyc_ssnit.py
+-rw-r--r--   0        0        0      111 2023-05-25 20:48:47.950499 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_ke_kyc_id.py
+-rw-r--r--   0        0        0      108 2023-05-25 20:48:47.950564 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_kyc_bvn.py
+-rw-r--r--   0        0        0      123 2023-05-25 20:48:47.950628 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_kyc_bvn_advance.py
+-rw-r--r--   0        0        0      119 2023-05-25 20:48:47.950697 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_kyc_bvn_basic.py
+-rw-r--r--   0        0        0      117 2023-05-25 20:48:47.950758 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_kyc_bvn_full.py
+-rw-r--r--   0        0        0      106 2023-05-25 20:48:47.950813 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_kyc_dl.py
+-rw-r--r--   0        0        0      112 2023-05-25 20:48:47.950873 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_kyc_nuban.py
+-rw-r--r--   0        0        0      118 2023-05-25 20:48:47.950932 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_kyc_passport.py
+-rw-r--r--   0        0        0      125 2023-05-25 20:48:47.950988 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_kyc_phone_number.py
+-rw-r--r--   0        0        0      108 2023-05-25 20:48:47.951044 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_kyc_vin.py
+-rw-r--r--   0        0        0      110 2023-05-25 20:48:47.951105 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_kyc_vnin.py
+-rw-r--r--   0        0        0      134 2023-05-25 20:48:47.951164 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_messaging_sender_id.py
+-rw-r--r--   0        0        0      133 2023-05-25 20:48:47.951225 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_messaging_sender_ids.py
+-rw-r--r--   0        0        0      123 2023-05-25 20:48:47.951280 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_messaging_sms.py
+-rw-r--r--   0        0        0      117 2023-05-25 20:48:47.951333 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_ug_kyc_voter.py
+-rw-r--r--   0        0        0      131 2023-05-25 20:48:47.951394 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_webhook_delete.py
+-rw-r--r--   0        0        0      120 2023-05-25 20:48:47.951454 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_webhook_fetch.py
+-rw-r--r--   0        0        0      125 2023-05-25 20:48:47.951530 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_webhook_notify.py
+-rw-r--r--   0        0        0      131 2023-05-25 20:48:47.951597 dojah_python_sdk-4.0.0/dojah_client/apis/paths/api_v1_webhook_subscribe.py
+-rw-r--r--   0        0        0      122 2023-05-25 20:48:47.951653 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_aml_screening_info.py
+-rw-r--r--   0        0        0      129 2023-05-25 20:48:47.951709 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_document_analysis_dl.py
+-rw-r--r--   0        0        0      146 2023-05-25 20:48:47.951778 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_financial_account_subscription.py
+-rw-r--r--   0        0        0      147 2023-05-25 20:48:47.951843 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_financial_bvn_information_basic.py
+-rw-r--r--   0        0        0      145 2023-05-25 20:48:47.951901 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_financial_bvn_information_full.py
+-rw-r--r--   0        0        0      140 2023-05-25 20:48:47.951966 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_financial_earning_structure.py
+-rw-r--r--   0        0        0      138 2023-05-25 20:48:47.952023 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_financial_spending_pattern.py
+-rw-r--r--   0        0        0      134 2023-05-25 20:48:47.952081 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_financial_transactions.py
+-rw-r--r--   0        0        0      117 2023-05-25 20:48:47.952133 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_general_account.py
+-rw-r--r--   0        0        0      113 2023-05-25 20:48:47.952194 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_general_banks.py
+-rw-r--r--   0        0        0      109 2023-05-25 20:48:47.952247 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_general_bin.py
+-rw-r--r--   0        0        0      126 2023-05-25 20:48:47.952308 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_kyc_age_verification.py
+-rw-r--r--   0        0        0      117 2023-05-25 20:48:47.952371 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_kyc_bvn_verify.py
+-rw-r--r--   0        0        0      101 2023-05-25 20:48:47.952442 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_kyc_cac.py
+-rw-r--r--   0        0        0      116 2023-05-25 20:48:47.952512 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_kyc_cac_advance.py
+-rw-r--r--   0        0        0      112 2023-05-25 20:48:47.952578 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_kyc_cac_basic.py
+-rw-r--r--   0        0        0      105 2023-05-25 20:48:47.952639 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_kyc_email.py
+-rw-r--r--   0        0        0      117 2023-05-25 20:48:47.952729 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_kyc_nin_verify.py
+-rw-r--r--   0        0        0      129 2023-05-25 20:48:47.952797 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_kyc_phone_number_basic.py
+-rw-r--r--   0        0        0      125 2023-05-25 20:48:47.952872 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_kyc_photoid_verify.py
+-rw-r--r--   0        0        0      101 2023-05-25 20:48:47.952952 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_kyc_tin.py
+-rw-r--r--   0        0        0      116 2023-05-25 20:48:47.953031 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_messaging_otp.py
+-rw-r--r--   0        0        0      130 2023-05-25 20:48:47.953104 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_messaging_otp_validate.py
+-rw-r--r--   0        0        0      133 2023-05-25 20:48:47.953182 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_messaging_sms_get_status.py
+-rw-r--r--   0        0        0      139 2023-05-25 20:48:47.953276 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_ml_categorize_transaction.py
+-rw-r--r--   0        0        0      102 2023-05-25 20:48:47.953355 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_ml_ocr.py
+-rw-r--r--   0        0        0      117 2023-05-25 20:48:47.953440 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_ml_ocr_generic.py
+-rw-r--r--   0        0        0      122 2023-05-25 20:48:47.953516 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_purchase_airtime.py
+-rw-r--r--   0        0        0      116 2023-05-25 20:48:47.953596 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_purchase_data.py
+-rw-r--r--   0        0        0      124 2023-05-25 20:48:47.953658 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_purchase_data_plans.py
+-rw-r--r--   0        0        0      124 2023-05-25 20:48:47.953727 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_wallet_ngn_accounts.py
+-rw-r--r--   0        0        0      123 2023-05-25 20:48:47.953791 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_wallet_ngn_create.py
+-rw-r--r--   0        0        0      123 2023-05-25 20:48:47.953872 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_wallet_ngn_credit.py
+-rw-r--r--   0        0        0      124 2023-05-25 20:48:47.953937 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_wallet_ngn_retrieve.py
+-rw-r--r--   0        0        0      130 2023-05-25 20:48:47.953997 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_wallet_ngn_transaction.py
+-rw-r--r--   0        0        0      127 2023-05-25 20:48:47.954052 dojah_python_sdk-4.0.0/dojah_client/apis/paths/v1_wallet_ngn_transfer.py
+-rw-r--r--   0        0        0     1879 2023-05-25 20:48:47.954125 dojah_python_sdk-4.0.0/dojah_client/apis/tag_to_api.py
+-rw-r--r--   0        0        0      578 2023-05-25 20:48:47.954237 dojah_python_sdk-4.0.0/dojah_client/apis/tags/__init__.py
+-rw-r--r--   0        0        0      499 2023-05-25 20:48:47.954307 dojah_python_sdk-4.0.0/dojah_client/apis/tags/aml_api.py
+-rw-r--r--   0        0        0      860 2023-05-25 20:48:47.954378 dojah_python_sdk-4.0.0/dojah_client/apis/tags/authentication_api.py
+-rw-r--r--   0        0        0     1414 2023-05-25 20:48:47.954444 dojah_python_sdk-4.0.0/dojah_client/apis/tags/financial_api.py
+-rw-r--r--   0        0        0      901 2023-05-25 20:48:47.954516 dojah_python_sdk-4.0.0/dojah_client/apis/tags/general_api.py
+-rw-r--r--   0        0        0      581 2023-05-25 20:48:47.954594 dojah_python_sdk-4.0.0/dojah_client/apis/tags/ghkyc_api.py
+-rw-r--r--   0        0        0      408 2023-05-25 20:48:47.954667 dojah_python_sdk-4.0.0/dojah_client/apis/tags/kekyc_api.py
+-rw-r--r--   0        0        0      621 2023-05-25 20:48:47.954740 dojah_python_sdk-4.0.0/dojah_client/apis/tags/kyb_api.py
+-rw-r--r--   0        0        0     1703 2023-05-25 20:48:47.954810 dojah_python_sdk-4.0.0/dojah_client/apis/tags/kyc_api.py
+-rw-r--r--   0        0        0      704 2023-05-25 20:48:47.954880 dojah_python_sdk-4.0.0/dojah_client/apis/tags/ml_api.py
+-rw-r--r--   0        0        0      442 2023-05-25 20:48:47.954967 dojah_python_sdk-4.0.0/dojah_client/apis/tags/services_api.py
+-rw-r--r--   0        0        0      401 2023-05-25 20:48:47.955038 dojah_python_sdk-4.0.0/dojah_client/apis/tags/ugkyc_api.py
+-rw-r--r--   0        0        0      862 2023-05-25 20:48:47.955108 dojah_python_sdk-4.0.0/dojah_client/apis/tags/wallet_api.py
+-rw-r--r--   0        0        0      695 2023-05-25 20:48:47.955196 dojah_python_sdk-4.0.0/dojah_client/apis/tags/web_hooks_api.py
+-rw-r--r--   0        0        0     2310 2023-05-25 20:48:47.955282 dojah_python_sdk-4.0.0/dojah_client/client.py
+-rw-r--r--   0        0        0     2310 2023-05-25 20:48:47.955360 dojah_python_sdk-4.0.0/dojah_client/client.pyi
+-rw-r--r--   0        0        0      708 2023-05-25 20:48:47.955443 dojah_python_sdk-4.0.0/dojah_client/client_custom.py
+-rw-r--r--   0        0        0    18401 2023-05-25 20:48:47.955657 dojah_python_sdk-4.0.0/dojah_client/configuration.py
+-rw-r--r--   0        0        0     7350 2023-05-25 20:48:47.955847 dojah_python_sdk-4.0.0/dojah_client/exceptions.py
+-rw-r--r--   0        0        0     2274 2023-05-25 20:48:47.955925 dojah_python_sdk-4.0.0/dojah_client/exceptions_base.py
+-rw-r--r--   0        0        0      346 2023-05-01 01:11:17.572249 dojah_python_sdk-4.0.0/dojah_client/model/__init__.py
+-rw-r--r--   0        0        0    30779 2023-05-25 20:48:47.957439 dojah_python_sdk-4.0.0/dojah_client/model/analyze_document_response.py
+-rw-r--r--   0        0        0    30779 2023-05-25 20:48:47.957666 dojah_python_sdk-4.0.0/dojah_client/model/analyze_document_response.pyi
+-rw-r--r--   0        0        0     2967 2023-05-25 20:48:47.957921 dojah_python_sdk-4.0.0/dojah_client/model/categorize_transactions_request.py
+-rw-r--r--   0        0        0     2967 2023-05-25 20:48:47.958045 dojah_python_sdk-4.0.0/dojah_client/model/categorize_transactions_request.pyi
+-rw-r--r--   0        0        0     9521 2023-05-25 20:48:47.958279 dojah_python_sdk-4.0.0/dojah_client/model/categorize_transactions_response.py
+-rw-r--r--   0        0        0     9521 2023-05-25 20:48:47.958411 dojah_python_sdk-4.0.0/dojah_client/model/categorize_transactions_response.pyi
+-rw-r--r--   0        0        0     2976 2023-05-25 20:48:47.958665 dojah_python_sdk-4.0.0/dojah_client/model/collect_status_from_pdf_request.py
+-rw-r--r--   0        0        0     2976 2023-05-25 20:48:47.958801 dojah_python_sdk-4.0.0/dojah_client/model/collect_status_from_pdf_request.pyi
+-rw-r--r--   0        0        0     4659 2023-05-25 20:48:47.959047 dojah_python_sdk-4.0.0/dojah_client/model/collect_status_from_pdf_response.py
+-rw-r--r--   0        0        0     4659 2023-05-25 20:48:47.959859 dojah_python_sdk-4.0.0/dojah_client/model/collect_status_from_pdf_response.pyi
+-rw-r--r--   0        0        0     9997 2023-05-25 20:48:47.960104 dojah_python_sdk-4.0.0/dojah_client/model/collect_transactions_request.py
+-rw-r--r--   0        0        0     9997 2023-05-25 20:48:47.960221 dojah_python_sdk-4.0.0/dojah_client/model/collect_transactions_request.pyi
+-rw-r--r--   0        0        0     5175 2023-05-25 20:48:47.960450 dojah_python_sdk-4.0.0/dojah_client/model/collect_transactions_response.py
+-rw-r--r--   0        0        0     5175 2023-05-25 20:48:47.960559 dojah_python_sdk-4.0.0/dojah_client/model/collect_transactions_response.pyi
+-rw-r--r--   0        0        0     4462 2023-05-25 20:48:47.960709 dojah_python_sdk-4.0.0/dojah_client/model/create_wallet_request.py
+-rw-r--r--   0        0        0     4462 2023-05-25 20:48:47.960825 dojah_python_sdk-4.0.0/dojah_client/model/create_wallet_request.pyi
+-rw-r--r--   0        0        0     6805 2023-05-25 20:48:47.961091 dojah_python_sdk-4.0.0/dojah_client/model/create_wallet_response.py
+-rw-r--r--   0        0        0     6805 2023-05-25 20:48:47.961182 dojah_python_sdk-4.0.0/dojah_client/model/create_wallet_response.pyi
+-rw-r--r--   0        0        0     2875 2023-05-25 20:48:47.961321 dojah_python_sdk-4.0.0/dojah_client/model/credit_subwallet_request.py
+-rw-r--r--   0        0        0     2875 2023-05-25 20:48:47.961401 dojah_python_sdk-4.0.0/dojah_client/model/credit_subwallet_request.pyi
+-rw-r--r--   0        0        0    12505 2023-05-25 20:48:47.961522 dojah_python_sdk-4.0.0/dojah_client/model/credit_subwallet_response.py
+-rw-r--r--   0        0        0    12505 2023-05-25 20:48:47.961598 dojah_python_sdk-4.0.0/dojah_client/model/credit_subwallet_response.pyi
+-rw-r--r--   0        0        0     2329 2023-05-25 20:48:47.961737 dojah_python_sdk-4.0.0/dojah_client/model/delete_webhook_response.py
+-rw-r--r--   0        0        0     2329 2023-05-25 20:48:47.961808 dojah_python_sdk-4.0.0/dojah_client/model/delete_webhook_response.pyi
+-rw-r--r--   0        0        0     7836 2023-05-25 20:48:47.961984 dojah_python_sdk-4.0.0/dojah_client/model/financial_get_basic_bvn_response.py
+-rw-r--r--   0        0        0     7836 2023-05-25 20:48:47.962073 dojah_python_sdk-4.0.0/dojah_client/model/financial_get_basic_bvn_response.pyi
+-rw-r--r--   0        0        0    21438 2023-05-25 20:48:47.962236 dojah_python_sdk-4.0.0/dojah_client/model/financial_get_full_bvn_response.py
+-rw-r--r--   0        0        0    21438 2023-05-25 20:48:47.962358 dojah_python_sdk-4.0.0/dojah_client/model/financial_get_full_bvn_response.pyi
+-rw-r--r--   0        0        0     5404 2023-05-25 20:48:47.962493 dojah_python_sdk-4.0.0/dojah_client/model/general_get_nuban_response.py
+-rw-r--r--   0        0        0     5404 2023-05-25 20:48:47.962564 dojah_python_sdk-4.0.0/dojah_client/model/general_get_nuban_response.pyi
+-rw-r--r--   0        0        0     4717 2023-05-25 20:48:47.962777 dojah_python_sdk-4.0.0/dojah_client/model/general_get_wallet_balance_response.py
+-rw-r--r--   0        0        0     4717 2023-05-25 20:48:47.962860 dojah_python_sdk-4.0.0/dojah_client/model/general_get_wallet_balance_response.pyi
+-rw-r--r--   0        0        0   134677 2023-05-25 20:48:47.963100 dojah_python_sdk-4.0.0/dojah_client/model/get_account_analysis_response.py
+-rw-r--r--   0        0        0   134677 2023-05-25 20:48:47.963292 dojah_python_sdk-4.0.0/dojah_client/model/get_account_analysis_response.pyi
+-rw-r--r--   0        0        0     5613 2023-05-25 20:48:47.963492 dojah_python_sdk-4.0.0/dojah_client/model/get_account_response.py
+-rw-r--r--   0        0        0     5613 2023-05-25 20:48:47.963582 dojah_python_sdk-4.0.0/dojah_client/model/get_account_response.pyi
+-rw-r--r--   0        0        0     9244 2023-05-25 20:48:47.963732 dojah_python_sdk-4.0.0/dojah_client/model/get_account_subscriptions_response.py
+-rw-r--r--   0        0        0     9244 2023-05-25 20:48:47.963815 dojah_python_sdk-4.0.0/dojah_client/model/get_account_subscriptions_response.pyi
+-rw-r--r--   0        0        0    18623 2023-05-25 20:48:47.963939 dojah_python_sdk-4.0.0/dojah_client/model/get_account_transactions_response.py
+-rw-r--r--   0        0        0    18623 2023-05-25 20:48:47.964055 dojah_python_sdk-4.0.0/dojah_client/model/get_account_transactions_response.pyi
+-rw-r--r--   0        0        0     7524 2023-05-25 20:48:47.964238 dojah_python_sdk-4.0.0/dojah_client/model/get_advanced_cac_response.py
+-rw-r--r--   0        0        0     7524 2023-05-25 20:48:47.964330 dojah_python_sdk-4.0.0/dojah_client/model/get_advanced_cac_response.pyi
+-rw-r--r--   0        0        0    11011 2023-05-25 20:48:47.964469 dojah_python_sdk-4.0.0/dojah_client/model/get_banks_response.py
+-rw-r--r--   0        0        0    11011 2023-05-25 20:48:47.964559 dojah_python_sdk-4.0.0/dojah_client/model/get_banks_response.pyi
+-rw-r--r--   0        0        0     7818 2023-05-25 20:48:47.964683 dojah_python_sdk-4.0.0/dojah_client/model/get_basic_bvn_response.py
+-rw-r--r--   0        0        0     7818 2023-05-25 20:48:47.964770 dojah_python_sdk-4.0.0/dojah_client/model/get_basic_bvn_response.pyi
+-rw-r--r--   0        0        0     7518 2023-05-25 20:48:47.964937 dojah_python_sdk-4.0.0/dojah_client/model/get_basic_cac_response.py
+-rw-r--r--   0        0        0     7518 2023-05-25 20:48:47.965020 dojah_python_sdk-4.0.0/dojah_client/model/get_basic_cac_response.pyi
+-rw-r--r--   0        0        0    12586 2023-05-25 20:48:47.965239 dojah_python_sdk-4.0.0/dojah_client/model/get_basic_phone_number_response.py
+-rw-r--r--   0        0        0    12586 2023-05-25 20:48:47.965352 dojah_python_sdk-4.0.0/dojah_client/model/get_basic_phone_number_response.pyi
+-rw-r--r--   0        0        0     8485 2023-05-25 20:48:47.965480 dojah_python_sdk-4.0.0/dojah_client/model/get_bin_response.py
+-rw-r--r--   0        0        0     8485 2023-05-25 20:48:47.965560 dojah_python_sdk-4.0.0/dojah_client/model/get_bin_response.pyi
+-rw-r--r--   0        0        0     6766 2023-05-25 20:48:47.965721 dojah_python_sdk-4.0.0/dojah_client/model/get_cac_response.py
+-rw-r--r--   0        0        0     6766 2023-05-25 20:48:47.965823 dojah_python_sdk-4.0.0/dojah_client/model/get_cac_response.pyi
+-rw-r--r--   0        0        0     7285 2023-05-25 20:48:47.966009 dojah_python_sdk-4.0.0/dojah_client/model/get_data_plans_response.py
+-rw-r--r--   0        0        0     7285 2023-05-25 20:48:47.966095 dojah_python_sdk-4.0.0/dojah_client/model/get_data_plans_response.pyi
+-rw-r--r--   0        0        0     2300 2023-05-25 20:48:47.966224 dojah_python_sdk-4.0.0/dojah_client/model/get_document_analysis_request.py
+-rw-r--r--   0        0        0     2300 2023-05-25 20:48:47.966304 dojah_python_sdk-4.0.0/dojah_client/model/get_document_analysis_request.pyi
+-rw-r--r--   0        0        0    22749 2023-05-25 20:48:47.966498 dojah_python_sdk-4.0.0/dojah_client/model/get_document_analysis_response.py
+-rw-r--r--   0        0        0    22749 2023-05-25 20:48:47.966624 dojah_python_sdk-4.0.0/dojah_client/model/get_document_analysis_response.pyi
+-rw-r--r--   0        0        0    12313 2023-05-25 20:48:47.966788 dojah_python_sdk-4.0.0/dojah_client/model/get_drivers_license_response.py
+-rw-r--r--   0        0        0    12313 2023-05-25 20:48:47.966879 dojah_python_sdk-4.0.0/dojah_client/model/get_drivers_license_response.pyi
+-rw-r--r--   0        0        0     6993 2023-05-25 20:48:47.967016 dojah_python_sdk-4.0.0/dojah_client/model/get_earning_structure_response.py
+-rw-r--r--   0        0        0     6993 2023-05-25 20:48:47.967086 dojah_python_sdk-4.0.0/dojah_client/model/get_earning_structure_response.pyi
+-rw-r--r--   0        0        0    30882 2023-05-25 20:48:47.967235 dojah_python_sdk-4.0.0/dojah_client/model/get_email_reputation_response.py
+-rw-r--r--   0        0        0    30882 2023-05-25 20:48:47.967366 dojah_python_sdk-4.0.0/dojah_client/model/get_email_reputation_response.pyi
+-rw-r--r--   0        0        0    22084 2023-05-25 20:48:47.967527 dojah_python_sdk-4.0.0/dojah_client/model/get_full_bvn_response.py
+-rw-r--r--   0        0        0    22084 2023-05-25 20:48:47.967615 dojah_python_sdk-4.0.0/dojah_client/model/get_full_bvn_response.pyi
+-rw-r--r--   0        0        0     2296 2023-05-25 20:48:47.967763 dojah_python_sdk-4.0.0/dojah_client/model/get_generic_ocr_text_request.py
+-rw-r--r--   0        0        0     2296 2023-05-25 20:48:47.967830 dojah_python_sdk-4.0.0/dojah_client/model/get_generic_ocr_text_request.pyi
+-rw-r--r--   0        0        0     5640 2023-05-25 20:48:47.967950 dojah_python_sdk-4.0.0/dojah_client/model/get_generic_ocr_text_response.py
+-rw-r--r--   0        0        0     5640 2023-05-25 20:48:47.968021 dojah_python_sdk-4.0.0/dojah_client/model/get_generic_ocr_text_response.pyi
+-rw-r--r--   0        0        0    20533 2023-05-25 20:48:47.968134 dojah_python_sdk-4.0.0/dojah_client/model/get_kyc_drivers_license_response.py
+-rw-r--r--   0        0        0    20533 2023-05-25 20:48:47.968218 dojah_python_sdk-4.0.0/dojah_client/model/get_kyc_drivers_license_response.pyi
+-rw-r--r--   0        0        0    11482 2023-05-25 20:48:47.968339 dojah_python_sdk-4.0.0/dojah_client/model/get_kyc_passport_response.py
+-rw-r--r--   0        0        0    11482 2023-05-25 20:48:47.968407 dojah_python_sdk-4.0.0/dojah_client/model/get_kyc_passport_response.pyi
+-rw-r--r--   0        0        0    11880 2023-05-25 20:48:47.968524 dojah_python_sdk-4.0.0/dojah_client/model/get_national_id_response.py
+-rw-r--r--   0        0        0    11880 2023-05-25 20:48:47.968598 dojah_python_sdk-4.0.0/dojah_client/model/get_national_id_response.pyi
+-rw-r--r--   0        0        0    19086 2023-05-25 20:48:47.968709 dojah_python_sdk-4.0.0/dojah_client/model/get_nuban_response.py
+-rw-r--r--   0        0        0    19086 2023-05-25 20:48:47.968790 dojah_python_sdk-4.0.0/dojah_client/model/get_nuban_response.pyi
+-rw-r--r--   0        0        0     2308 2023-05-25 20:48:47.968902 dojah_python_sdk-4.0.0/dojah_client/model/get_ocr_text_request.py
+-rw-r--r--   0        0        0     2308 2023-05-25 20:48:47.968965 dojah_python_sdk-4.0.0/dojah_client/model/get_ocr_text_request.pyi
+-rw-r--r--   0        0        0     5626 2023-05-25 20:48:47.969069 dojah_python_sdk-4.0.0/dojah_client/model/get_ocr_text_response.py
+-rw-r--r--   0        0        0     5626 2023-05-25 20:48:47.969129 dojah_python_sdk-4.0.0/dojah_client/model/get_ocr_text_response.pyi
+-rw-r--r--   0        0        0    15247 2023-05-25 20:48:47.969242 dojah_python_sdk-4.0.0/dojah_client/model/get_passport_response.py
+-rw-r--r--   0        0        0    15247 2023-05-25 20:48:47.969305 dojah_python_sdk-4.0.0/dojah_client/model/get_passport_response.pyi
+-rw-r--r--   0        0        0    24352 2023-05-25 20:48:47.969441 dojah_python_sdk-4.0.0/dojah_client/model/get_phone_number404_response.py
+-rw-r--r--   0        0        0    24352 2023-05-25 20:48:47.969547 dojah_python_sdk-4.0.0/dojah_client/model/get_phone_number404_response.pyi
+-rw-r--r--   0        0        0    24346 2023-05-25 20:48:47.969672 dojah_python_sdk-4.0.0/dojah_client/model/get_phone_number_response.py
+-rw-r--r--   0        0        0    24346 2023-05-25 20:48:47.969762 dojah_python_sdk-4.0.0/dojah_client/model/get_phone_number_response.pyi
+-rw-r--r--   0        0        0    22078 2023-05-25 20:48:47.969884 dojah_python_sdk-4.0.0/dojah_client/model/get_premium_bvn_response.py
+-rw-r--r--   0        0        0    22078 2023-05-25 20:48:47.969975 dojah_python_sdk-4.0.0/dojah_client/model/get_premium_bvn_response.pyi
+-rw-r--r--   0        0        0    35461 2023-05-25 20:48:47.970205 dojah_python_sdk-4.0.0/dojah_client/model/get_screening_info_response.py
+-rw-r--r--   0        0        0    35461 2023-05-25 20:48:47.970343 dojah_python_sdk-4.0.0/dojah_client/model/get_screening_info_response.pyi
+-rw-r--r--   0        0        0     7336 2023-05-25 20:48:47.970479 dojah_python_sdk-4.0.0/dojah_client/model/get_sender_id_response.py
+-rw-r--r--   0        0        0     7336 2023-05-25 20:48:47.970553 dojah_python_sdk-4.0.0/dojah_client/model/get_sender_id_response.pyi
+-rw-r--r--   0        0        0     4591 2023-05-25 20:48:47.970653 dojah_python_sdk-4.0.0/dojah_client/model/get_sms_status_response.py
+-rw-r--r--   0        0        0     4591 2023-05-25 20:48:47.970719 dojah_python_sdk-4.0.0/dojah_client/model/get_sms_status_response.pyi
+-rw-r--r--   0        0        0    36434 2023-05-25 20:48:47.970850 dojah_python_sdk-4.0.0/dojah_client/model/get_spending_pattern_response.py
+-rw-r--r--   0        0        0    36434 2023-05-25 20:48:47.970969 dojah_python_sdk-4.0.0/dojah_client/model/get_spending_pattern_response.pyi
+-rw-r--r--   0        0        0    10134 2023-05-25 20:48:47.971167 dojah_python_sdk-4.0.0/dojah_client/model/get_ssnit_response.py
+-rw-r--r--   0        0        0    10134 2023-05-25 20:48:47.971255 dojah_python_sdk-4.0.0/dojah_client/model/get_ssnit_response.pyi
+-rw-r--r--   0        0        0     9175 2023-05-25 20:48:47.971387 dojah_python_sdk-4.0.0/dojah_client/model/get_tin_response.py
+-rw-r--r--   0        0        0     9175 2023-05-25 20:48:47.971469 dojah_python_sdk-4.0.0/dojah_client/model/get_tin_response.pyi
+-rw-r--r--   0        0        0    12503 2023-05-25 20:48:47.971603 dojah_python_sdk-4.0.0/dojah_client/model/get_transaction_response.py
+-rw-r--r--   0        0        0    12503 2023-05-25 20:48:47.971690 dojah_python_sdk-4.0.0/dojah_client/model/get_transaction_response.pyi
+-rw-r--r--   0        0        0     9896 2023-05-25 20:48:47.971860 dojah_python_sdk-4.0.0/dojah_client/model/get_vin_response.py
+-rw-r--r--   0        0        0     9896 2023-05-25 20:48:47.971943 dojah_python_sdk-4.0.0/dojah_client/model/get_vin_response.pyi
+-rw-r--r--   0        0        0     9724 2023-05-25 20:48:47.972051 dojah_python_sdk-4.0.0/dojah_client/model/get_vnin_response.py
+-rw-r--r--   0        0        0     9724 2023-05-25 20:48:47.972118 dojah_python_sdk-4.0.0/dojah_client/model/get_vnin_response.pyi
+-rw-r--r--   0        0        0    12857 2023-05-25 20:48:47.972265 dojah_python_sdk-4.0.0/dojah_client/model/get_voter_response.py
+-rw-r--r--   0        0        0    12857 2023-05-25 20:48:47.972347 dojah_python_sdk-4.0.0/dojah_client/model/get_voter_response.pyi
+-rw-r--r--   0        0        0     4703 2023-05-25 20:48:47.972452 dojah_python_sdk-4.0.0/dojah_client/model/get_wallet_balance_response.py
+-rw-r--r--   0        0        0     4703 2023-05-25 20:48:47.972517 dojah_python_sdk-4.0.0/dojah_client/model/get_wallet_balance_response.pyi
+-rw-r--r--   0        0        0     7463 2023-05-25 20:48:47.972614 dojah_python_sdk-4.0.0/dojah_client/model/get_wallet_response.py
+-rw-r--r--   0        0        0     7463 2023-05-25 20:48:47.972689 dojah_python_sdk-4.0.0/dojah_client/model/get_wallet_response.pyi
+-rw-r--r--   0        0        0    14066 2023-05-25 20:48:47.972814 dojah_python_sdk-4.0.0/dojah_client/model/get_wallets_response.py
+-rw-r--r--   0        0        0    14066 2023-05-25 20:48:47.972896 dojah_python_sdk-4.0.0/dojah_client/model/get_wallets_response.pyi
+-rw-r--r--   0        0        0    10466 2023-05-25 20:48:47.973000 dojah_python_sdk-4.0.0/dojah_client/model/get_webhooks_response.py
+-rw-r--r--   0        0        0    10466 2023-05-25 20:48:47.973072 dojah_python_sdk-4.0.0/dojah_client/model/get_webhooks_response.pyi
+-rw-r--r--   0        0        0     5068 2023-05-25 20:48:47.973181 dojah_python_sdk-4.0.0/dojah_client/model/notify_webhook_request.py
+-rw-r--r--   0        0        0     5068 2023-05-25 20:48:47.973257 dojah_python_sdk-4.0.0/dojah_client/model/notify_webhook_request.pyi
+-rw-r--r--   0        0        0     2329 2023-05-25 20:48:47.973415 dojah_python_sdk-4.0.0/dojah_client/model/notify_webhook_response.py
+-rw-r--r--   0        0        0     2329 2023-05-25 20:48:47.973495 dojah_python_sdk-4.0.0/dojah_client/model/notify_webhook_response.pyi
+-rw-r--r--   0        0        0     2901 2023-05-25 20:48:47.973626 dojah_python_sdk-4.0.0/dojah_client/model/purchase_airtime_request.py
+-rw-r--r--   0        0        0     2901 2023-05-25 20:48:47.973706 dojah_python_sdk-4.0.0/dojah_client/model/purchase_airtime_request.pyi
+-rw-r--r--   0        0        0    10496 2023-05-25 20:48:47.973880 dojah_python_sdk-4.0.0/dojah_client/model/purchase_airtime_response.py
+-rw-r--r--   0        0        0    10496 2023-05-25 20:48:47.973968 dojah_python_sdk-4.0.0/dojah_client/model/purchase_airtime_response.pyi
+-rw-r--r--   0        0        0     2869 2023-05-25 20:48:47.974120 dojah_python_sdk-4.0.0/dojah_client/model/purchase_data_request.py
+-rw-r--r--   0        0        0     2869 2023-05-25 20:48:47.974197 dojah_python_sdk-4.0.0/dojah_client/model/purchase_data_request.pyi
+-rw-r--r--   0        0        0     7285 2023-05-25 20:48:47.974318 dojah_python_sdk-4.0.0/dojah_client/model/purchase_data_response.py
+-rw-r--r--   0        0        0     7285 2023-05-25 20:48:47.974396 dojah_python_sdk-4.0.0/dojah_client/model/purchase_data_response.pyi
+-rw-r--r--   0        0        0     2370 2023-05-25 20:48:47.974510 dojah_python_sdk-4.0.0/dojah_client/model/request_sender_id_request.py
+-rw-r--r--   0        0        0     2370 2023-05-25 20:48:47.974584 dojah_python_sdk-4.0.0/dojah_client/model/request_sender_id_request.pyi
+-rw-r--r--   0        0        0     7344 2023-05-25 20:48:47.974701 dojah_python_sdk-4.0.0/dojah_client/model/request_sender_id_response.py
+-rw-r--r--   0        0        0     7344 2023-05-25 20:48:47.974786 dojah_python_sdk-4.0.0/dojah_client/model/request_sender_id_response.pyi
+-rw-r--r--   0        0        0     3511 2023-05-25 20:48:47.974923 dojah_python_sdk-4.0.0/dojah_client/model/screen_aml_request.py
+-rw-r--r--   0        0        0     3511 2023-05-25 20:48:47.974999 dojah_python_sdk-4.0.0/dojah_client/model/screen_aml_request.pyi
+-rw-r--r--   0        0        0     5288 2023-05-25 20:48:47.975138 dojah_python_sdk-4.0.0/dojah_client/model/screen_aml_response.py
+-rw-r--r--   0        0        0     5288 2023-05-25 20:48:47.975218 dojah_python_sdk-4.0.0/dojah_client/model/screen_aml_response.pyi
+-rw-r--r--   0        0        0     4507 2023-05-25 20:48:47.975356 dojah_python_sdk-4.0.0/dojah_client/model/send_otp_request.py
+-rw-r--r--   0        0        0     4507 2023-05-25 20:48:47.975443 dojah_python_sdk-4.0.0/dojah_client/model/send_otp_request.pyi
+-rw-r--r--   0        0        0     8096 2023-05-25 20:48:47.975571 dojah_python_sdk-4.0.0/dojah_client/model/send_otp_response.py
+-rw-r--r--   0        0        0     8096 2023-05-25 20:48:47.975653 dojah_python_sdk-4.0.0/dojah_client/model/send_otp_response.pyi
+-rw-r--r--   0        0        0     3960 2023-05-25 20:48:47.975752 dojah_python_sdk-4.0.0/dojah_client/model/send_sms_request.py
+-rw-r--r--   0        0        0     3960 2023-05-25 20:48:47.975819 dojah_python_sdk-4.0.0/dojah_client/model/send_sms_request.pyi
+-rw-r--r--   0        0        0     6536 2023-05-25 20:48:47.975918 dojah_python_sdk-4.0.0/dojah_client/model/send_sms_response.py
+-rw-r--r--   0        0        0     6536 2023-05-25 20:48:47.975976 dojah_python_sdk-4.0.0/dojah_client/model/send_sms_response.pyi
+-rw-r--r--   0        0        0     2864 2023-05-25 20:48:47.976105 dojah_python_sdk-4.0.0/dojah_client/model/subscribe_service_request.py
+-rw-r--r--   0        0        0     2864 2023-05-25 20:48:47.976186 dojah_python_sdk-4.0.0/dojah_client/model/subscribe_service_request.pyi
+-rw-r--r--   0        0        0     2335 2023-05-25 20:48:47.976310 dojah_python_sdk-4.0.0/dojah_client/model/subscribe_service_response.py
+-rw-r--r--   0        0        0     2335 2023-05-25 20:48:47.976379 dojah_python_sdk-4.0.0/dojah_client/model/subscribe_service_response.pyi
+-rw-r--r--   0        0        0     4284 2023-05-25 20:48:47.976506 dojah_python_sdk-4.0.0/dojah_client/model/transfer_funds_request.py
+-rw-r--r--   0        0        0     4284 2023-05-25 20:48:47.976585 dojah_python_sdk-4.0.0/dojah_client/model/transfer_funds_request.pyi
+-rw-r--r--   0        0        0    12501 2023-05-25 20:48:47.976701 dojah_python_sdk-4.0.0/dojah_client/model/transfer_funds_response.py
+-rw-r--r--   0        0        0    12501 2023-05-25 20:48:47.976779 dojah_python_sdk-4.0.0/dojah_client/model/transfer_funds_response.pyi
+-rw-r--r--   0        0        0    12570 2023-05-25 20:48:47.976928 dojah_python_sdk-4.0.0/dojah_client/model/validate_bvn_response.py
+-rw-r--r--   0        0        0    12570 2023-05-25 20:48:47.977012 dojah_python_sdk-4.0.0/dojah_client/model/validate_bvn_response.pyi
+-rw-r--r--   0        0        0     4578 2023-05-25 20:48:47.977217 dojah_python_sdk-4.0.0/dojah_client/model/validate_otp_response.py
+-rw-r--r--   0        0        0     4578 2023-05-25 20:48:47.977340 dojah_python_sdk-4.0.0/dojah_client/model/validate_otp_response.pyi
+-rw-r--r--   0        0        0     6722 2023-05-25 20:48:47.977545 dojah_python_sdk-4.0.0/dojah_client/model/verify_age_response.py
+-rw-r--r--   0        0        0     6722 2023-05-25 20:48:47.977642 dojah_python_sdk-4.0.0/dojah_client/model/verify_age_response.pyi
+-rw-r--r--   0        0        0     3021 2023-05-25 20:48:47.977807 dojah_python_sdk-4.0.0/dojah_client/model/verify_photo_id_with_selfie_request.py
+-rw-r--r--   0        0        0     3021 2023-05-25 20:48:47.977943 dojah_python_sdk-4.0.0/dojah_client/model/verify_photo_id_with_selfie_request.pyi
+-rw-r--r--   0        0        0    13447 2023-05-25 20:48:47.978746 dojah_python_sdk-4.0.0/dojah_client/model/verify_photo_id_with_selfie_response.py
+-rw-r--r--   0        0        0    13447 2023-05-25 20:48:47.978890 dojah_python_sdk-4.0.0/dojah_client/model/verify_photo_id_with_selfie_response.pyi
+-rw-r--r--   0        0        0     2875 2023-05-25 20:48:47.979117 dojah_python_sdk-4.0.0/dojah_client/model/verify_selfie_bvn_request.py
+-rw-r--r--   0        0        0     2875 2023-05-25 20:48:47.979224 dojah_python_sdk-4.0.0/dojah_client/model/verify_selfie_bvn_request.pyi
+-rw-r--r--   0        0        0    24678 2023-05-25 20:48:47.979434 dojah_python_sdk-4.0.0/dojah_client/model/verify_selfie_bvn_response.py
+-rw-r--r--   0        0        0    24678 2023-05-25 20:48:47.979557 dojah_python_sdk-4.0.0/dojah_client/model/verify_selfie_bvn_response.pyi
+-rw-r--r--   0        0        0     2875 2023-05-25 20:48:47.979755 dojah_python_sdk-4.0.0/dojah_client/model/verify_selfie_nin_request.py
+-rw-r--r--   0        0        0     2875 2023-05-25 20:48:47.979846 dojah_python_sdk-4.0.0/dojah_client/model/verify_selfie_nin_request.pyi
+-rw-r--r--   0        0        0    42189 2023-05-25 20:48:47.980039 dojah_python_sdk-4.0.0/dojah_client/model/verify_selfie_nin_response.py
+-rw-r--r--   0        0        0    42189 2023-05-25 20:48:47.980251 dojah_python_sdk-4.0.0/dojah_client/model/verify_selfie_nin_response.pyi
+-rw-r--r--   0        0        0     7264 2023-05-25 20:48:47.981160 dojah_python_sdk-4.0.0/dojah_client/models/__init__.py
+-rw-r--r--   0        0        0     3743 2023-05-25 20:48:47.981351 dojah_python_sdk-4.0.0/dojah_client/paths/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-25 20:48:47.981519 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_aml_screening/__init__.py
+-rw-r--r--   0        0        0    15039 2023-05-25 20:48:47.981672 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_aml_screening/post.py
+-rw-r--r--   0        0        0    13264 2023-05-25 20:48:47.981831 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_aml_screening/post.pyi
+-rw-r--r--   0        0        0      311 2023-05-25 20:48:47.982031 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_balance/__init__.py
+-rw-r--r--   0        0        0     9930 2023-05-25 20:48:47.982240 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_balance/get.py
+-rw-r--r--   0        0        0     9772 2023-05-25 20:48:47.982459 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_balance/get.pyi
+-rw-r--r--   0        0        0      331 2023-05-25 20:48:47.982635 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_document_analysis/__init__.py
+-rw-r--r--   0        0        0     9063 2023-05-25 20:48:47.982765 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_document_analysis/post.py
+-rw-r--r--   0        0        0     8935 2023-05-25 20:48:47.982882 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_document_analysis/post.pyi
+-rw-r--r--   0        0        0      355 2023-05-25 20:48:47.983090 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_financial_account_information/__init__.py
+-rw-r--r--   0        0        0    13558 2023-05-25 20:48:47.983242 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_financial_account_information/get.py
+-rw-r--r--   0        0        0    12508 2023-05-25 20:48:47.983326 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_financial_account_information/get.pyi
+-rw-r--r--   0        0        0      357 2023-05-25 20:48:47.983433 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_financial_account_transactions/__init__.py
+-rw-r--r--   0        0        0    14575 2023-05-25 20:48:47.983516 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_financial_account_transactions/get.py
+-rw-r--r--   0        0        0    13525 2023-05-25 20:48:47.983638 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_financial_account_transactions/get.pyi
+-rw-r--r--   0        0        0      333 2023-05-25 20:48:47.983763 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_financial_analysis/__init__.py
+-rw-r--r--   0        0        0    13557 2023-05-25 20:48:47.983852 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_financial_analysis/get.py
+-rw-r--r--   0        0        0    10911 2023-05-25 20:48:47.983953 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_financial_analysis/get.pyi
+-rw-r--r--   0        0        0      349 2023-05-25 20:48:47.984053 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_financial_transactions_pdf/__init__.py
+-rw-r--r--   0        0        0    12027 2023-05-25 20:48:47.984119 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_financial_transactions_pdf/post.py
+-rw-r--r--   0        0        0    11899 2023-05-25 20:48:47.984189 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_financial_transactions_pdf/post.pyi
+-rw-r--r--   0        0        0      315 2023-05-25 20:48:47.984320 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_gh_kyc_dl/__init__.py
+-rw-r--r--   0        0        0    16530 2023-05-25 20:48:47.984440 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_gh_kyc_dl/get.py
+-rw-r--r--   0        0        0    14714 2023-05-25 20:48:47.984561 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_gh_kyc_dl/get.pyi
+-rw-r--r--   0        0        0      327 2023-05-25 20:48:47.984706 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_gh_kyc_passport/__init__.py
+-rw-r--r--   0        0        0    18005 2023-05-25 20:48:47.984837 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_gh_kyc_passport/get.py
+-rw-r--r--   0        0        0    16189 2023-05-25 20:48:47.984955 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_gh_kyc_passport/get.pyi
+-rw-r--r--   0        0        0      321 2023-05-25 20:48:47.985082 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_gh_kyc_ssnit/__init__.py
+-rw-r--r--   0        0        0    13245 2023-05-25 20:48:47.985155 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_gh_kyc_ssnit/get.py
+-rw-r--r--   0        0        0    13117 2023-05-25 20:48:47.985223 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_gh_kyc_ssnit/get.pyi
+-rw-r--r--   0        0        0      315 2023-05-25 20:48:47.985325 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_ke_kyc_id/__init__.py
+-rw-r--r--   0        0        0    15778 2023-05-25 20:48:47.985401 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_ke_kyc_id/get.py
+-rw-r--r--   0        0        0    15650 2023-05-25 20:48:47.985474 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_ke_kyc_id/get.pyi
+-rw-r--r--   0        0        0      311 2023-05-25 20:48:47.985569 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_bvn/__init__.py
+-rw-r--r--   0        0        0    13168 2023-05-25 20:48:47.985643 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_bvn/get.py
+-rw-r--r--   0        0        0    13040 2023-05-25 20:48:47.985708 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_bvn/get.pyi
+-rw-r--r--   0        0        0      327 2023-05-25 20:48:47.985810 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_bvn_advance/__init__.py
+-rw-r--r--   0        0        0    16234 2023-05-25 20:48:47.985879 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_bvn_advance/get.py
+-rw-r--r--   0        0        0    13575 2023-05-25 20:48:47.985955 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_bvn_advance/get.pyi
+-rw-r--r--   0        0        0      323 2023-05-25 20:48:47.986090 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_bvn_basic/__init__.py
+-rw-r--r--   0        0        0    11736 2023-05-25 20:48:47.986173 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_bvn_basic/get.py
+-rw-r--r--   0        0        0    11608 2023-05-25 20:48:47.986241 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_bvn_basic/get.pyi
+-rw-r--r--   0        0        0      321 2023-05-25 20:48:47.986344 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_bvn_full/__init__.py
+-rw-r--r--   0        0        0    11710 2023-05-25 20:48:47.986411 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_bvn_full/get.py
+-rw-r--r--   0        0        0    11582 2023-05-25 20:48:47.986483 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_bvn_full/get.pyi
+-rw-r--r--   0        0        0      309 2023-05-25 20:48:47.986590 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_dl/__init__.py
+-rw-r--r--   0        0        0    12150 2023-05-25 20:48:47.986676 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_dl/get.py
+-rw-r--r--   0        0        0    12022 2023-05-25 20:48:47.986754 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_dl/get.pyi
+-rw-r--r--   0        0        0      315 2023-05-25 20:48:47.986863 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_nuban/__init__.py
+-rw-r--r--   0        0        0    14440 2023-05-25 20:48:47.986945 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_nuban/get.py
+-rw-r--r--   0        0        0    13390 2023-05-25 20:48:47.987023 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_nuban/get.pyi
+-rw-r--r--   0        0        0      321 2023-05-25 20:48:47.987128 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_passport/__init__.py
+-rw-r--r--   0        0        0    12755 2023-05-25 20:48:47.987194 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_passport/get.py
+-rw-r--r--   0        0        0    12627 2023-05-25 20:48:47.987263 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_passport/get.pyi
+-rw-r--r--   0        0        0      329 2023-05-25 20:48:47.987360 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_phone_number/__init__.py
+-rw-r--r--   0        0        0    12800 2023-05-25 20:48:47.987419 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_phone_number/get.py
+-rw-r--r--   0        0        0    12642 2023-05-25 20:48:47.987487 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_phone_number/get.pyi
+-rw-r--r--   0        0        0      311 2023-05-25 20:48:47.987577 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_vin/__init__.py
+-rw-r--r--   0        0        0    18482 2023-05-25 20:48:47.987646 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_vin/get.py
+-rw-r--r--   0        0        0    16109 2023-05-25 20:48:47.987724 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_vin/get.pyi
+-rw-r--r--   0        0        0      313 2023-05-25 20:48:47.987822 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_vnin/__init__.py
+-rw-r--r--   0        0        0    11614 2023-05-25 20:48:47.987886 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_vnin/get.py
+-rw-r--r--   0        0        0    11486 2023-05-25 20:48:47.987953 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_kyc_vnin/get.pyi
+-rw-r--r--   0        0        0      335 2023-05-25 20:48:47.988068 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_messaging_sender_id/__init__.py
+-rw-r--r--   0        0        0    11354 2023-05-25 20:48:47.988155 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_messaging_sender_id/post.py
+-rw-r--r--   0        0        0    11226 2023-05-25 20:48:47.988220 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_messaging_sender_id/post.pyi
+-rw-r--r--   0        0        0      337 2023-05-25 20:48:47.988324 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_messaging_sender_ids/__init__.py
+-rw-r--r--   0        0        0    10704 2023-05-25 20:48:47.988385 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_messaging_sender_ids/get.py
+-rw-r--r--   0        0        0     9654 2023-05-25 20:48:47.988451 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_messaging_sender_ids/get.pyi
+-rw-r--r--   0        0        0      323 2023-05-25 20:48:47.988546 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_messaging_sms/__init__.py
+-rw-r--r--   0        0        0    14096 2023-05-25 20:48:47.988606 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_messaging_sms/post.py
+-rw-r--r--   0        0        0    13046 2023-05-25 20:48:47.988662 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_messaging_sms/post.pyi
+-rw-r--r--   0        0        0      321 2023-05-25 20:48:47.988757 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_ug_kyc_voter/__init__.py
+-rw-r--r--   0        0        0    13201 2023-05-25 20:48:47.988816 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_ug_kyc_voter/get.py
+-rw-r--r--   0        0        0    13073 2023-05-25 20:48:47.988881 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_ug_kyc_voter/get.pyi
+-rw-r--r--   0        0        0      325 2023-05-25 20:48:47.988981 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_webhook_delete/__init__.py
+-rw-r--r--   0        0        0     9011 2023-05-25 20:48:47.989068 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_webhook_delete/delete.py
+-rw-r--r--   0        0        0     8883 2023-05-25 20:48:47.989154 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_webhook_delete/delete.pyi
+-rw-r--r--   0        0        0      323 2023-05-25 20:48:47.989250 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_webhook_fetch/__init__.py
+-rw-r--r--   0        0        0    12944 2023-05-25 20:48:47.989311 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_webhook_fetch/get.py
+-rw-r--r--   0        0        0    10565 2023-05-25 20:48:47.989374 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_webhook_fetch/get.pyi
+-rw-r--r--   0        0        0      325 2023-05-25 20:48:47.989492 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_webhook_notify/__init__.py
+-rw-r--r--   0        0        0    15975 2023-05-25 20:48:47.989552 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_webhook_notify/post.py
+-rw-r--r--   0        0        0    13595 2023-05-25 20:48:47.989616 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_webhook_notify/post.pyi
+-rw-r--r--   0        0        0      331 2023-05-25 20:48:47.989723 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_webhook_subscribe/__init__.py
+-rw-r--r--   0        0        0    13445 2023-05-25 20:48:47.989794 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_webhook_subscribe/post.py
+-rw-r--r--   0        0        0    12395 2023-05-25 20:48:47.989882 dojah_python_sdk-4.0.0/dojah_client/paths/api_v1_webhook_subscribe/post.pyi
+-rw-r--r--   0        0        0      325 2023-05-25 20:48:47.989983 dojah_python_sdk-4.0.0/dojah_client/paths/v1_aml_screening_info/__init__.py
+-rw-r--r--   0        0        0    12018 2023-05-25 20:48:47.990050 dojah_python_sdk-4.0.0/dojah_client/paths/v1_aml_screening_info/get.py
+-rw-r--r--   0        0        0    11890 2023-05-25 20:48:47.990112 dojah_python_sdk-4.0.0/dojah_client/paths/v1_aml_screening_info/get.pyi
+-rw-r--r--   0        0        0      329 2023-05-25 20:48:47.990207 dojah_python_sdk-4.0.0/dojah_client/paths/v1_document_analysis_dl/__init__.py
+-rw-r--r--   0        0        0    14335 2023-05-25 20:48:47.990295 dojah_python_sdk-4.0.0/dojah_client/paths/v1_document_analysis_dl/post.py
+-rw-r--r--   0        0        0    12560 2023-05-25 20:48:47.990363 dojah_python_sdk-4.0.0/dojah_client/paths/v1_document_analysis_dl/post.pyi
+-rw-r--r--   0        0        0      349 2023-05-25 20:48:47.990456 dojah_python_sdk-4.0.0/dojah_client/paths/v1_financial_account_subscription/__init__.py
+-rw-r--r--   0        0        0    13863 2023-05-25 20:48:47.990515 dojah_python_sdk-4.0.0/dojah_client/paths/v1_financial_account_subscription/get.py
+-rw-r--r--   0        0        0    12813 2023-05-25 20:48:47.990579 dojah_python_sdk-4.0.0/dojah_client/paths/v1_financial_account_subscription/get.pyi
+-rw-r--r--   0        0        0      351 2023-05-25 20:48:47.990677 dojah_python_sdk-4.0.0/dojah_client/paths/v1_financial_bvn_information_basic/__init__.py
+-rw-r--r--   0        0        0    15929 2023-05-25 20:48:47.990742 dojah_python_sdk-4.0.0/dojah_client/paths/v1_financial_bvn_information_basic/get.py
+-rw-r--r--   0        0        0    13556 2023-05-25 20:48:47.990812 dojah_python_sdk-4.0.0/dojah_client/paths/v1_financial_bvn_information_basic/get.pyi
+-rw-r--r--   0        0        0      349 2023-05-25 20:48:47.990959 dojah_python_sdk-4.0.0/dojah_client/paths/v1_financial_bvn_information_full/__init__.py
+-rw-r--r--   0        0        0    15905 2023-05-25 20:48:47.991038 dojah_python_sdk-4.0.0/dojah_client/paths/v1_financial_bvn_information_full/get.py
+-rw-r--r--   0        0        0    13532 2023-05-25 20:48:47.991105 dojah_python_sdk-4.0.0/dojah_client/paths/v1_financial_bvn_information_full/get.pyi
+-rw-r--r--   0        0        0      343 2023-05-25 20:48:47.991207 dojah_python_sdk-4.0.0/dojah_client/paths/v1_financial_earning_structure/__init__.py
+-rw-r--r--   0        0        0    13767 2023-05-25 20:48:47.991285 dojah_python_sdk-4.0.0/dojah_client/paths/v1_financial_earning_structure/get.py
+-rw-r--r--   0        0        0    12717 2023-05-25 20:48:47.991348 dojah_python_sdk-4.0.0/dojah_client/paths/v1_financial_earning_structure/get.pyi
+-rw-r--r--   0        0        0      341 2023-05-25 20:48:47.991510 dojah_python_sdk-4.0.0/dojah_client/paths/v1_financial_spending_pattern/__init__.py
+-rw-r--r--   0        0        0    13743 2023-05-25 20:48:47.991574 dojah_python_sdk-4.0.0/dojah_client/paths/v1_financial_spending_pattern/get.py
+-rw-r--r--   0        0        0    12693 2023-05-25 20:48:47.991635 dojah_python_sdk-4.0.0/dojah_client/paths/v1_financial_spending_pattern/get.pyi
+-rw-r--r--   0        0        0      333 2023-05-25 20:48:47.991728 dojah_python_sdk-4.0.0/dojah_client/paths/v1_financial_transactions/__init__.py
+-rw-r--r--   0        0        0    12374 2023-05-25 20:48:47.991797 dojah_python_sdk-4.0.0/dojah_client/paths/v1_financial_transactions/post.py
+-rw-r--r--   0        0        0    12246 2023-05-25 20:48:47.991865 dojah_python_sdk-4.0.0/dojah_client/paths/v1_financial_transactions/post.pyi
+-rw-r--r--   0        0        0      319 2023-05-25 20:48:47.991951 dojah_python_sdk-4.0.0/dojah_client/paths/v1_general_account/__init__.py
+-rw-r--r--   0        0        0    14486 2023-05-25 20:48:47.992017 dojah_python_sdk-4.0.0/dojah_client/paths/v1_general_account/get.py
+-rw-r--r--   0        0        0    13436 2023-05-25 20:48:47.992085 dojah_python_sdk-4.0.0/dojah_client/paths/v1_general_account/get.pyi
+-rw-r--r--   0        0        0      315 2023-05-25 20:48:47.992176 dojah_python_sdk-4.0.0/dojah_client/paths/v1_general_banks/__init__.py
+-rw-r--r--   0        0        0     8896 2023-05-25 20:48:47.992242 dojah_python_sdk-4.0.0/dojah_client/paths/v1_general_banks/get.py
+-rw-r--r--   0        0        0     8768 2023-05-25 20:48:47.992310 dojah_python_sdk-4.0.0/dojah_client/paths/v1_general_banks/get.pyi
+-rw-r--r--   0        0        0      311 2023-05-25 20:48:47.992415 dojah_python_sdk-4.0.0/dojah_client/paths/v1_general_bin/__init__.py
+-rw-r--r--   0        0        0    11718 2023-05-25 20:48:47.992514 dojah_python_sdk-4.0.0/dojah_client/paths/v1_general_bin/get.py
+-rw-r--r--   0        0        0    11590 2023-05-25 20:48:47.992612 dojah_python_sdk-4.0.0/dojah_client/paths/v1_general_bin/get.pyi
+-rw-r--r--   0        0        0      329 2023-05-25 20:48:47.992750 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_age_verification/__init__.py
+-rw-r--r--   0        0        0    17370 2023-05-25 20:48:47.992870 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_age_verification/get.py
+-rw-r--r--   0        0        0    16320 2023-05-25 20:48:47.992976 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_age_verification/get.pyi
+-rw-r--r--   0        0        0      317 2023-05-25 20:48:47.993103 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_bvn_verify/__init__.py
+-rw-r--r--   0        0        0    11755 2023-05-25 20:48:47.993167 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_bvn_verify/post.py
+-rw-r--r--   0        0        0    11627 2023-05-25 20:48:47.993232 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_bvn_verify/post.pyi
+-rw-r--r--   0        0        0      303 2023-05-25 20:48:47.993331 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_cac/__init__.py
+-rw-r--r--   0        0        0    14305 2023-05-25 20:48:47.993399 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_cac/get.py
+-rw-r--r--   0        0        0    13255 2023-05-25 20:48:47.993472 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_cac/get.pyi
+-rw-r--r--   0        0        0      319 2023-05-25 20:48:47.993566 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_cac_advance/__init__.py
+-rw-r--r--   0        0        0    13173 2023-05-25 20:48:47.993648 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_cac_advance/get.py
+-rw-r--r--   0        0        0    13045 2023-05-25 20:48:47.993738 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_cac_advance/get.pyi
+-rw-r--r--   0        0        0      315 2023-05-25 20:48:47.993853 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_cac_basic/__init__.py
+-rw-r--r--   0        0        0    12365 2023-05-25 20:48:47.993926 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_cac_basic/get.py
+-rw-r--r--   0        0        0    12237 2023-05-25 20:48:47.994038 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_cac_basic/get.pyi
+-rw-r--r--   0        0        0      307 2023-05-25 20:48:47.994143 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_email/__init__.py
+-rw-r--r--   0        0        0    15837 2023-05-25 20:48:47.994209 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_email/get.py
+-rw-r--r--   0        0        0    13489 2023-05-25 20:48:47.994285 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_email/get.pyi
+-rw-r--r--   0        0        0      317 2023-05-25 20:48:47.994413 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_nin_verify/__init__.py
+-rw-r--r--   0        0        0    11755 2023-05-25 20:48:47.994497 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_nin_verify/post.py
+-rw-r--r--   0        0        0    11627 2023-05-25 20:48:47.994571 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_nin_verify/post.pyi
+-rw-r--r--   0        0        0      333 2023-05-25 20:48:47.994713 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_phone_number_basic/__init__.py
+-rw-r--r--   0        0        0    12150 2023-05-25 20:48:47.994814 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_phone_number_basic/get.py
+-rw-r--r--   0        0        0    12022 2023-05-25 20:48:47.994897 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_phone_number_basic/get.pyi
+-rw-r--r--   0        0        0      325 2023-05-25 20:48:47.995028 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_photoid_verify/__init__.py
+-rw-r--r--   0        0        0    12213 2023-05-25 20:48:47.995109 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_photoid_verify/post.py
+-rw-r--r--   0        0        0    12085 2023-05-25 20:48:47.995187 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_photoid_verify/post.pyi
+-rw-r--r--   0        0        0      303 2023-05-25 20:48:47.995293 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_tin/__init__.py
+-rw-r--r--   0        0        0    13289 2023-05-25 20:48:47.995364 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_tin/get.py
+-rw-r--r--   0        0        0    12239 2023-05-25 20:48:47.995438 dojah_python_sdk-4.0.0/dojah_client/paths/v1_kyc_tin/get.pyi
+-rw-r--r--   0        0        0      315 2023-05-25 20:48:47.995559 dojah_python_sdk-4.0.0/dojah_client/paths/v1_messaging_otp/__init__.py
+-rw-r--r--   0        0        0    16894 2023-05-25 20:48:47.995653 dojah_python_sdk-4.0.0/dojah_client/paths/v1_messaging_otp/post.py
+-rw-r--r--   0        0        0    14515 2023-05-25 20:48:47.995766 dojah_python_sdk-4.0.0/dojah_client/paths/v1_messaging_otp/post.pyi
+-rw-r--r--   0        0        0      333 2023-05-25 20:48:47.995887 dojah_python_sdk-4.0.0/dojah_client/paths/v1_messaging_otp_validate/__init__.py
+-rw-r--r--   0        0        0    14318 2023-05-25 20:48:47.995963 dojah_python_sdk-4.0.0/dojah_client/paths/v1_messaging_otp_validate/get.py
+-rw-r--r--   0        0        0    13268 2023-05-25 20:48:47.996047 dojah_python_sdk-4.0.0/dojah_client/paths/v1_messaging_otp_validate/get.pyi
+-rw-r--r--   0        0        0      337 2023-05-25 20:48:47.996220 dojah_python_sdk-4.0.0/dojah_client/paths/v1_messaging_sms_get_status/__init__.py
+-rw-r--r--   0        0        0    13623 2023-05-25 20:48:47.996355 dojah_python_sdk-4.0.0/dojah_client/paths/v1_messaging_sms_get_status/get.py
+-rw-r--r--   0        0        0    12573 2023-05-25 20:48:47.996508 dojah_python_sdk-4.0.0/dojah_client/paths/v1_messaging_sms_get_status/get.pyi
+-rw-r--r--   0        0        0      339 2023-05-25 20:48:47.996715 dojah_python_sdk-4.0.0/dojah_client/paths/v1_ml_categorize_transaction/__init__.py
+-rw-r--r--   0        0        0    13749 2023-05-25 20:48:47.996833 dojah_python_sdk-4.0.0/dojah_client/paths/v1_ml_categorize_transaction/post.py
+-rw-r--r--   0        0        0    12699 2023-05-25 20:48:47.996920 dojah_python_sdk-4.0.0/dojah_client/paths/v1_ml_categorize_transaction/post.pyi
+-rw-r--r--   0        0        0      301 2023-05-25 20:48:47.997065 dojah_python_sdk-4.0.0/dojah_client/paths/v1_ml_ocr/__init__.py
+-rw-r--r--   0        0        0    11091 2023-05-25 20:48:47.997185 dojah_python_sdk-4.0.0/dojah_client/paths/v1_ml_ocr/post.py
+-rw-r--r--   0        0        0    10963 2023-05-25 20:48:47.997304 dojah_python_sdk-4.0.0/dojah_client/paths/v1_ml_ocr/post.pyi
+-rw-r--r--   0        0        0      317 2023-05-25 20:48:47.997487 dojah_python_sdk-4.0.0/dojah_client/paths/v1_ml_ocr_generic/__init__.py
+-rw-r--r--   0        0        0    11320 2023-05-25 20:48:47.997594 dojah_python_sdk-4.0.0/dojah_client/paths/v1_ml_ocr_generic/post.py
+-rw-r--r--   0        0        0    11192 2023-05-25 20:48:47.997696 dojah_python_sdk-4.0.0/dojah_client/paths/v1_ml_ocr_generic/post.pyi
+-rw-r--r--   0        0        0      321 2023-05-25 20:48:47.997924 dojah_python_sdk-4.0.0/dojah_client/paths/v1_purchase_airtime/__init__.py
+-rw-r--r--   0        0        0    11755 2023-05-25 20:48:47.998073 dojah_python_sdk-4.0.0/dojah_client/paths/v1_purchase_airtime/post.py
+-rw-r--r--   0        0        0    11627 2023-05-25 20:48:47.998201 dojah_python_sdk-4.0.0/dojah_client/paths/v1_purchase_airtime/post.pyi
+-rw-r--r--   0        0        0      315 2023-05-25 20:48:47.998375 dojah_python_sdk-4.0.0/dojah_client/paths/v1_purchase_data/__init__.py
+-rw-r--r--   0        0        0    11622 2023-05-25 20:48:47.998531 dojah_python_sdk-4.0.0/dojah_client/paths/v1_purchase_data/post.py
+-rw-r--r--   0        0        0    11494 2023-05-25 20:48:47.998664 dojah_python_sdk-4.0.0/dojah_client/paths/v1_purchase_data/post.pyi
+-rw-r--r--   0        0        0      327 2023-05-25 20:48:47.998842 dojah_python_sdk-4.0.0/dojah_client/paths/v1_purchase_data_plans/__init__.py
+-rw-r--r--   0        0        0     9011 2023-05-25 20:48:47.998946 dojah_python_sdk-4.0.0/dojah_client/paths/v1_purchase_data_plans/get.py
+-rw-r--r--   0        0        0     8883 2023-05-25 20:48:47.999048 dojah_python_sdk-4.0.0/dojah_client/paths/v1_purchase_data_plans/get.pyi
+-rw-r--r--   0        0        0      327 2023-05-25 20:48:47.999211 dojah_python_sdk-4.0.0/dojah_client/paths/v1_wallet_ngn_accounts/__init__.py
+-rw-r--r--   0        0        0    16179 2023-05-25 20:48:47.999329 dojah_python_sdk-4.0.0/dojah_client/paths/v1_wallet_ngn_accounts/get.py
+-rw-r--r--   0        0        0    13520 2023-05-25 20:48:47.999594 dojah_python_sdk-4.0.0/dojah_client/paths/v1_wallet_ngn_accounts/get.pyi
+-rw-r--r--   0        0        0      323 2023-05-25 20:48:47.999897 dojah_python_sdk-4.0.0/dojah_client/paths/v1_wallet_ngn_create/__init__.py
+-rw-r--r--   0        0        0    14630 2023-05-25 20:48:48.000018 dojah_python_sdk-4.0.0/dojah_client/paths/v1_wallet_ngn_create/post.py
+-rw-r--r--   0        0        0    13580 2023-05-25 20:48:48.000139 dojah_python_sdk-4.0.0/dojah_client/paths/v1_wallet_ngn_create/post.pyi
+-rw-r--r--   0        0        0      323 2023-05-25 20:48:48.000347 dojah_python_sdk-4.0.0/dojah_client/paths/v1_wallet_ngn_credit/__init__.py
+-rw-r--r--   0        0        0    15606 2023-05-25 20:48:48.000451 dojah_python_sdk-4.0.0/dojah_client/paths/v1_wallet_ngn_credit/post.py
+-rw-r--r--   0        0        0    13275 2023-05-25 20:48:48.000615 dojah_python_sdk-4.0.0/dojah_client/paths/v1_wallet_ngn_credit/post.pyi
+-rw-r--r--   0        0        0      327 2023-05-25 20:48:48.000752 dojah_python_sdk-4.0.0/dojah_client/paths/v1_wallet_ngn_retrieve/__init__.py
+-rw-r--r--   0        0        0    16253 2023-05-25 20:48:48.000858 dojah_python_sdk-4.0.0/dojah_client/paths/v1_wallet_ngn_retrieve/get.py
+-rw-r--r--   0        0        0    13594 2023-05-25 20:48:48.001008 dojah_python_sdk-4.0.0/dojah_client/paths/v1_wallet_ngn_retrieve/get.pyi
+-rw-r--r--   0        0        0      333 2023-05-25 20:48:48.001213 dojah_python_sdk-4.0.0/dojah_client/paths/v1_wallet_ngn_transaction/__init__.py
+-rw-r--r--   0        0        0    15951 2023-05-25 20:48:48.001356 dojah_python_sdk-4.0.0/dojah_client/paths/v1_wallet_ngn_transaction/get.py
+-rw-r--r--   0        0        0    13603 2023-05-25 20:48:48.001487 dojah_python_sdk-4.0.0/dojah_client/paths/v1_wallet_ngn_transaction/get.pyi
+-rw-r--r--   0        0        0      327 2023-05-25 20:48:48.001648 dojah_python_sdk-4.0.0/dojah_client/paths/v1_wallet_ngn_transfer/__init__.py
+-rw-r--r--   0        0        0    16853 2023-05-25 20:48:48.001831 dojah_python_sdk-4.0.0/dojah_client/paths/v1_wallet_ngn_transfer/post.py
+-rw-r--r--   0        0        0    14505 2023-05-25 20:48:48.001998 dojah_python_sdk-4.0.0/dojah_client/paths/v1_wallet_ngn_transfer/post.pyi
+-rw-r--r--   0        0        0      680 2023-05-25 20:48:48.002108 dojah_python_sdk-4.0.0/dojah_client/request_after_hook.py
+-rw-r--r--   0        0        0      681 2023-05-25 20:48:48.002286 dojah_python_sdk-4.0.0/dojah_client/request_before_hook.py
+-rw-r--r--   0        0        0    10998 2023-05-25 20:48:48.002547 dojah_python_sdk-4.0.0/dojah_client/rest.py
+-rw-r--r--   0        0        0    95600 2023-05-25 20:48:48.002907 dojah_python_sdk-4.0.0/dojah_client/schemas.py
+-rw-r--r--   0        0        0        0 2023-05-25 20:48:48.003037 dojah_python_sdk-4.0.0/dojah_client/type/__init__.py
+-rw-r--r--   0        0        0      727 2023-05-25 20:48:48.003151 dojah_python_sdk-4.0.0/dojah_client/type/analyze_document_response.py
+-rw-r--r--   0        0        0      714 2023-05-25 20:48:48.003253 dojah_python_sdk-4.0.0/dojah_client/type/categorize_transactions_request.py
+-rw-r--r--   0        0        0      776 2023-05-25 20:48:48.003366 dojah_python_sdk-4.0.0/dojah_client/type/categorize_transactions_response.py
+-rw-r--r--   0        0        0      703 2023-05-25 20:48:48.003458 dojah_python_sdk-4.0.0/dojah_client/type/collect_status_from_pdf_request.py
+-rw-r--r--   0        0        0      762 2023-05-25 20:48:48.003551 dojah_python_sdk-4.0.0/dojah_client/type/collect_status_from_pdf_response.py
+-rw-r--r--   0        0        0      787 2023-05-25 20:48:48.003628 dojah_python_sdk-4.0.0/dojah_client/type/collect_transactions_request.py
+-rw-r--r--   0        0        0      776 2023-05-25 20:48:48.003726 dojah_python_sdk-4.0.0/dojah_client/type/collect_transactions_response.py
+-rw-r--r--   0        0        0      704 2023-05-25 20:48:48.003804 dojah_python_sdk-4.0.0/dojah_client/type/create_wallet_request.py
+-rw-r--r--   0        0        0      706 2023-05-25 20:48:48.003906 dojah_python_sdk-4.0.0/dojah_client/type/create_wallet_response.py
+-rw-r--r--   0        0        0      659 2023-05-25 20:48:48.004005 dojah_python_sdk-4.0.0/dojah_client/type/credit_subwallet_request.py
+-rw-r--r--   0        0        0      727 2023-05-25 20:48:48.004087 dojah_python_sdk-4.0.0/dojah_client/type/credit_subwallet_response.py
+-rw-r--r--   0        0        0      629 2023-05-25 20:48:48.004174 dojah_python_sdk-4.0.0/dojah_client/type/delete_webhook_response.py
+-rw-r--r--   0        0        0      762 2023-05-25 20:48:48.004296 dojah_python_sdk-4.0.0/dojah_client/type/financial_get_basic_bvn_response.py
+-rw-r--r--   0        0        0      755 2023-05-25 20:48:48.004407 dojah_python_sdk-4.0.0/dojah_client/type/financial_get_full_bvn_response.py
+-rw-r--r--   0        0        0      727 2023-05-25 20:48:48.004519 dojah_python_sdk-4.0.0/dojah_client/type/general_get_nuban_response.py
+-rw-r--r--   0        0        0      783 2023-05-25 20:48:48.004633 dojah_python_sdk-4.0.0/dojah_client/type/general_get_wallet_balance_response.py
+-rw-r--r--   0        0        0      748 2023-05-25 20:48:48.004749 dojah_python_sdk-4.0.0/dojah_client/type/get_account_analysis_response.py
+-rw-r--r--   0        0        0      748 2023-05-25 20:48:48.004875 dojah_python_sdk-4.0.0/dojah_client/type/get_account_response.py
+-rw-r--r--   0        0        0      783 2023-05-25 20:48:48.005009 dojah_python_sdk-4.0.0/dojah_client/type/get_account_subscriptions_response.py
+-rw-r--r--   0        0        0      776 2023-05-25 20:48:48.005108 dojah_python_sdk-4.0.0/dojah_client/type/get_account_transactions_response.py
+-rw-r--r--   0        0        0      720 2023-05-25 20:48:48.005192 dojah_python_sdk-4.0.0/dojah_client/type/get_advanced_cac_response.py
+-rw-r--r--   0        0        0      691 2023-05-25 20:48:48.005288 dojah_python_sdk-4.0.0/dojah_client/type/get_banks_response.py
+-rw-r--r--   0        0        0      699 2023-05-25 20:48:48.005366 dojah_python_sdk-4.0.0/dojah_client/type/get_basic_bvn_response.py
+-rw-r--r--   0        0        0      699 2023-05-25 20:48:48.005464 dojah_python_sdk-4.0.0/dojah_client/type/get_basic_cac_response.py
+-rw-r--r--   0        0        0      755 2023-05-25 20:48:48.005573 dojah_python_sdk-4.0.0/dojah_client/type/get_basic_phone_number_response.py
+-rw-r--r--   0        0        0      664 2023-05-25 20:48:48.005651 dojah_python_sdk-4.0.0/dojah_client/type/get_bin_response.py
+-rw-r--r--   0        0        0      664 2023-05-25 20:48:48.005731 dojah_python_sdk-4.0.0/dojah_client/type/get_cac_response.py
+-rw-r--r--   0        0        0      719 2023-05-25 20:48:48.005822 dojah_python_sdk-4.0.0/dojah_client/type/get_data_plans_response.py
+-rw-r--r--   0        0        0      661 2023-05-25 20:48:48.005928 dojah_python_sdk-4.0.0/dojah_client/type/get_document_analysis_request.py
+-rw-r--r--   0        0        0      755 2023-05-25 20:48:48.006064 dojah_python_sdk-4.0.0/dojah_client/type/get_document_analysis_response.py
+-rw-r--r--   0        0        0      741 2023-05-25 20:48:48.006141 dojah_python_sdk-4.0.0/dojah_client/type/get_drivers_license_response.py
+-rw-r--r--   0        0        0      755 2023-05-25 20:48:48.006248 dojah_python_sdk-4.0.0/dojah_client/type/get_earning_structure_response.py
+-rw-r--r--   0        0        0      748 2023-05-25 20:48:48.006394 dojah_python_sdk-4.0.0/dojah_client/type/get_email_reputation_response.py
+-rw-r--r--   0        0        0      692 2023-05-25 20:48:48.006496 dojah_python_sdk-4.0.0/dojah_client/type/get_full_bvn_response.py
+-rw-r--r--   0        0        0      647 2023-05-25 20:48:48.006598 dojah_python_sdk-4.0.0/dojah_client/type/get_generic_ocr_text_request.py
+-rw-r--r--   0        0        0      741 2023-05-25 20:48:48.006720 dojah_python_sdk-4.0.0/dojah_client/type/get_generic_ocr_text_response.py
+-rw-r--r--   0        0        0      762 2023-05-25 20:48:48.006830 dojah_python_sdk-4.0.0/dojah_client/type/get_kyc_drivers_license_response.py
+-rw-r--r--   0        0        0      720 2023-05-25 20:48:48.006912 dojah_python_sdk-4.0.0/dojah_client/type/get_kyc_passport_response.py
+-rw-r--r--   0        0        0      713 2023-05-25 20:48:48.007017 dojah_python_sdk-4.0.0/dojah_client/type/get_national_id_response.py
+-rw-r--r--   0        0        0      678 2023-05-25 20:48:48.007119 dojah_python_sdk-4.0.0/dojah_client/type/get_nuban_response.py
+-rw-r--r--   0        0        0      600 2023-05-25 20:48:48.007251 dojah_python_sdk-4.0.0/dojah_client/type/get_ocr_text_request.py
+-rw-r--r--   0        0        0      692 2023-05-25 20:48:48.007361 dojah_python_sdk-4.0.0/dojah_client/type/get_ocr_text_response.py
+-rw-r--r--   0        0        0      699 2023-05-25 20:48:48.007452 dojah_python_sdk-4.0.0/dojah_client/type/get_passport_response.py
+-rw-r--r--   0        0        0      741 2023-05-25 20:48:48.007562 dojah_python_sdk-4.0.0/dojah_client/type/get_phone_number404_response.py
+-rw-r--r--   0        0        0      720 2023-05-25 20:48:48.007647 dojah_python_sdk-4.0.0/dojah_client/type/get_phone_number_response.py
+-rw-r--r--   0        0        0      713 2023-05-25 20:48:48.007767 dojah_python_sdk-4.0.0/dojah_client/type/get_premium_bvn_response.py
+-rw-r--r--   0        0        0      734 2023-05-25 20:48:48.007902 dojah_python_sdk-4.0.0/dojah_client/type/get_screening_info_response.py
+-rw-r--r--   0        0        0      712 2023-05-25 20:48:48.007991 dojah_python_sdk-4.0.0/dojah_client/type/get_sender_id_response.py
+-rw-r--r--   0        0        0      706 2023-05-25 20:48:48.008138 dojah_python_sdk-4.0.0/dojah_client/type/get_sms_status_response.py
+-rw-r--r--   0        0        0      748 2023-05-25 20:48:48.008265 dojah_python_sdk-4.0.0/dojah_client/type/get_spending_pattern_response.py
+-rw-r--r--   0        0        0      678 2023-05-25 20:48:48.008353 dojah_python_sdk-4.0.0/dojah_client/type/get_ssnit_response.py
+-rw-r--r--   0        0        0      664 2023-05-25 20:48:48.008442 dojah_python_sdk-4.0.0/dojah_client/type/get_tin_response.py
+-rw-r--r--   0        0        0      720 2023-05-25 20:48:48.008530 dojah_python_sdk-4.0.0/dojah_client/type/get_transaction_response.py
+-rw-r--r--   0        0        0      664 2023-05-25 20:48:48.008670 dojah_python_sdk-4.0.0/dojah_client/type/get_vin_response.py
+-rw-r--r--   0        0        0      671 2023-05-25 20:48:48.008805 dojah_python_sdk-4.0.0/dojah_client/type/get_vnin_response.py
+-rw-r--r--   0        0        0      678 2023-05-25 20:48:48.008925 dojah_python_sdk-4.0.0/dojah_client/type/get_voter_response.py
+-rw-r--r--   0        0        0      734 2023-05-25 20:48:48.009016 dojah_python_sdk-4.0.0/dojah_client/type/get_wallet_balance_response.py
+-rw-r--r--   0        0        0      685 2023-05-25 20:48:48.009117 dojah_python_sdk-4.0.0/dojah_client/type/get_wallet_response.py
+-rw-r--r--   0        0        0      692 2023-05-25 20:48:48.009216 dojah_python_sdk-4.0.0/dojah_client/type/get_wallets_response.py
+-rw-r--r--   0        0        0      712 2023-05-25 20:48:48.009316 dojah_python_sdk-4.0.0/dojah_client/type/get_webhooks_response.py
+-rw-r--r--   0        0        0      725 2023-05-25 20:48:48.009405 dojah_python_sdk-4.0.0/dojah_client/type/notify_webhook_request.py
+-rw-r--r--   0        0        0      629 2023-05-25 20:48:48.009510 dojah_python_sdk-4.0.0/dojah_client/type/notify_webhook_response.py
+-rw-r--r--   0        0        0      661 2023-05-25 20:48:48.009623 dojah_python_sdk-4.0.0/dojah_client/type/purchase_airtime_request.py
+-rw-r--r--   0        0        0      727 2023-05-25 20:48:48.009750 dojah_python_sdk-4.0.0/dojah_client/type/purchase_airtime_response.py
+-rw-r--r--   0        0        0      638 2023-05-25 20:48:48.009837 dojah_python_sdk-4.0.0/dojah_client/type/purchase_data_request.py
+-rw-r--r--   0        0        0      719 2023-05-25 20:48:48.009916 dojah_python_sdk-4.0.0/dojah_client/type/purchase_data_response.py
+-rw-r--r--   0        0        0      639 2023-05-25 20:48:48.009990 dojah_python_sdk-4.0.0/dojah_client/type/request_sender_id_request.py
+-rw-r--r--   0        0        0      740 2023-05-25 20:48:48.010058 dojah_python_sdk-4.0.0/dojah_client/type/request_sender_id_response.py
+-rw-r--r--   0        0        0      648 2023-05-25 20:48:48.010132 dojah_python_sdk-4.0.0/dojah_client/type/screen_aml_request.py
+-rw-r--r--   0        0        0      685 2023-05-25 20:48:48.010205 dojah_python_sdk-4.0.0/dojah_client/type/screen_aml_response.py
+-rw-r--r--   0        0        0      693 2023-05-25 20:48:48.010272 dojah_python_sdk-4.0.0/dojah_client/type/send_otp_request.py
+-rw-r--r--   0        0        0      684 2023-05-25 20:48:48.010349 dojah_python_sdk-4.0.0/dojah_client/type/send_otp_response.py
+-rw-r--r--   0        0        0      650 2023-05-25 20:48:48.010427 dojah_python_sdk-4.0.0/dojah_client/type/send_sms_request.py
+-rw-r--r--   0        0        0      671 2023-05-25 20:48:48.010496 dojah_python_sdk-4.0.0/dojah_client/type/send_sms_response.py
+-rw-r--r--   0        0        0      665 2023-05-25 20:48:48.010573 dojah_python_sdk-4.0.0/dojah_client/type/subscribe_service_request.py
+-rw-r--r--   0        0        0      650 2023-05-25 20:48:48.010634 dojah_python_sdk-4.0.0/dojah_client/type/subscribe_service_response.py
+-rw-r--r--   0        0        0      716 2023-05-25 20:48:48.010697 dojah_python_sdk-4.0.0/dojah_client/type/transfer_funds_request.py
+-rw-r--r--   0        0        0      713 2023-05-25 20:48:48.010758 dojah_python_sdk-4.0.0/dojah_client/type/transfer_funds_response.py
+-rw-r--r--   0        0        0      699 2023-05-25 20:48:48.010820 dojah_python_sdk-4.0.0/dojah_client/type/validate_bvn_response.py
+-rw-r--r--   0        0        0      699 2023-05-25 20:48:48.010924 dojah_python_sdk-4.0.0/dojah_client/type/validate_otp_response.py
+-rw-r--r--   0        0        0      685 2023-05-25 20:48:48.011022 dojah_python_sdk-4.0.0/dojah_client/type/verify_age_response.py
+-rw-r--r--   0        0        0      725 2023-05-25 20:48:48.011086 dojah_python_sdk-4.0.0/dojah_client/type/verify_photo_id_with_selfie_request.py
+-rw-r--r--   0        0        0      783 2023-05-25 20:48:48.011160 dojah_python_sdk-4.0.0/dojah_client/type/verify_photo_id_with_selfie_response.py
+-rw-r--r--   0        0        0      659 2023-05-25 20:48:48.011279 dojah_python_sdk-4.0.0/dojah_client/type/verify_selfie_bvn_request.py
+-rw-r--r--   0        0        0      727 2023-05-25 20:48:48.011370 dojah_python_sdk-4.0.0/dojah_client/type/verify_selfie_bvn_response.py
+-rw-r--r--   0        0        0      659 2023-05-25 20:48:48.011449 dojah_python_sdk-4.0.0/dojah_client/type/verify_selfie_nin_request.py
+-rw-r--r--   0        0        0      727 2023-05-25 20:48:48.011532 dojah_python_sdk-4.0.0/dojah_client/type/verify_selfie_nin_response.py
+-rw-r--r--   0        0        0      534 2023-05-25 20:48:48.011618 dojah_python_sdk-4.0.0/dojah_client/type_util.py
+-rw-r--r--   0        0        0     3168 2023-05-25 20:48:48.011724 dojah_python_sdk-4.0.0/dojah_client/validation_metadata.py
+-rw-r--r--   0        0        0      721 2023-05-25 20:48:48.012326 dojah_python_sdk-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0    18978 1970-01-01 00:00:00.000000 dojah_python_sdk-4.0.0/PKG-INFO
```

### Comparing `dojah-python-sdk-3.0.0/dojah_client/__init__.py` & `dojah_python_sdk-4.0.0/dojah_client/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,30 @@
+# coding: utf-8
+
 # flake8: noqa
 
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
-
-__version__ = "3.0.0"
+__version__ = "4.0.0"
 
 # import ApiClient
 from dojah_client.api_client import ApiClient
 
 # import Configuration
 from dojah_client.configuration import Configuration
 
 # import exceptions
 from dojah_client.exceptions import OpenApiException
 from dojah_client.exceptions import ApiAttributeError
 from dojah_client.exceptions import ApiTypeError
 from dojah_client.exceptions import ApiValueError
 from dojah_client.exceptions import ApiKeyError
 from dojah_client.exceptions import ApiException
+
+from dojah_client.client import Dojah
```

### Comparing `dojah-python-sdk-3.0.0/dojah_client/configuration.py` & `dojah_python_sdk-4.0.0/dojah_client/configuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,43 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
-
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
+
+import validators
+from urllib.parse import urlparse
 from http import client as http_client
-from dojah_client.exceptions import ApiValueError
+from dojah_client.exceptions_base import ApiValueError
+from dojah_client.exceptions import ClientConfigurationError
+from dojah_client.exceptions import InvalidHostConfigurationError
 
 
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
-    'minLength', 'pattern', 'maxItems', 'minItems'
+    'minLength', 'pattern', 'maxItems', 'minItems',
+    'uniqueItems', 'maxProperties', 'minProperties',
 }
 
 class Configuration(object):
-    """NOTE: This class is auto generated by Konfig
-
-    Ref: https://konfigthis.com
-    Do not edit the class manually.
+    """NOTE:
+    This class is auto generated by Konfig (https://konfigthis.com)
 
     :param host: Base url
     :param api_key: Dict to store API key(s).
       Each entry in the dict specifies an API key.
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is the API key secret.
     :param api_key_prefix: Dict to store API prefix (e.g. Bearer)
@@ -69,16 +74,14 @@
       templated server configuration. The validation of enums is performed for
       variables with defined enum values before.
     :param server_operation_index: Mapping from operation ID to an index to server
       configuration.
     :param server_operation_variables: Mapping from operation ID to a mapping with
       string values to replace variables in templated server configuration.
       The validation of enums is performed for variables with defined enum values before.
-    :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
-      in PEM format
 
     :Example:
 
     API Key Authentication Example.
     Given the following security scheme in the OpenAPI specification:
       components:
         securitySchemes:
@@ -98,43 +101,51 @@
        Cookie: JSESSIONID abc123
     """
 
     _default = None
 
     def __init__(self, host=None,
                  api_key=None, api_key_prefix=None,
-                 access_token=None,
                  username=None, password=None,
                  discard_unknown_keys=False,
+                 authorization=None,
+                 app_id=None,
                  disabled_client_side_validations="",
                  server_index=None, server_variables=None,
                  server_operation_index=None, server_operation_variables=None,
-                 ssl_ca_cert=None,
                  ):
         """Constructor
         """
-        self._base_path = "https://api.dojah.io" if host is None else host
+        self.host = "https://api.dojah.io" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
         """Default server index
         """
         self.server_variables = server_variables or {}
         self.server_operation_variables = server_operation_variables or {}
         """Default server variables
         """
         self.temp_folder_path = None
         """Temp file folder for downloading files
         """
         # Authentication Settings
-        self.access_token = access_token
         self.api_key = {}
         if api_key:
-            self.api_key = api_key
+            if (isinstance(api_key, str)):
+                self.api_key = {'apikeyAuth': api_key}
+            else:
+                self.api_key = api_key
+        if authorization:
+            self.api_key['apikeyAuth'] = authorization
+        else:
+            raise ClientConfigurationError('API Key "apikeyAuth" is required')
+        if app_id:
+            self.api_key['appIdAuth'] = app_id
         """dict to store API key(s)
         """
         self.api_key_prefix = {}
         if api_key_prefix:
             self.api_key_prefix = api_key_prefix
         """dict to store API prefix (e.g. Bearer)
         """
@@ -171,15 +182,15 @@
         """
 
         self.verify_ssl = True
         """SSL/TLS verification
            Set this to false to skip verifying SSL certificate when calling API
            from https server.
         """
-        self.ssl_ca_cert = ssl_ca_cert
+        self.ssl_ca_cert = None
         """Set this to customize the certificate file to verify the peer.
         """
         self.cert_file = None
         """client certificate file
         """
         self.key_file = None
         """client key file
@@ -195,17 +206,14 @@
            requests to the same host, which is often the case here.
            cpu_count * 5 is used as default value to increase performance.
         """
 
         self.proxy = None
         """Proxy URL
         """
-        self.no_proxy = None
-        """bypass proxy for host in the no_proxy list.
-        """
         self.proxy_headers = None
         """Proxy headers
         """
         self.safe_chars_for_path_param = ''
         """Safe chars for path_param
         """
         self.retries = None
@@ -414,15 +422,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 3.0.0".\
+               "SDK Package Version: 4.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
@@ -480,9 +488,25 @@
     def host(self):
         """Return generated host."""
         return self.get_host_from_settings(self.server_index, variables=self.server_variables)
 
     @host.setter
     def host(self, value):
         """Fix base path."""
-        self._base_path = value
+        self._base_path = check_url(value)
         self.server_index = None
+        
+def check_url(url: str):
+    parsed = urlparse(url)
+    if parsed.query != '':
+        raise InvalidHostConfigurationError(url, "query string is not allowed")
+    if parsed.fragment != '':
+        raise InvalidHostConfigurationError(url, "fragment is not allowed")
+    if parsed.scheme not in ["http", "https"]:
+        raise InvalidHostConfigurationError(url, 'scheme must be "http" or "https"'.format(parsed.scheme))
+    if not validators.url(url):
+        raise InvalidHostConfigurationError(url, "invalid url")
+    if (url.endswith("/")):
+        return url[:-1]
+    return url
+
+
```

### Comparing `dojah-python-sdk-3.0.0/dojah_client/model_utils.py` & `dojah_python_sdk-4.0.0/dojah_client/schemas.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,2058 +1,2427 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
-
-from datetime import date, datetime  # noqa: F401
-from copy import deepcopy
-import inspect
+from collections import defaultdict
+from datetime import date, datetime, timedelta  # noqa: F401
+import functools
+import decimal
 import io
-import os
-import pprint
 import re
-import tempfile
+import types
+import typing
+import typing_extensions
 import uuid
 
-from dateutil.parser import parse
+from dateutil.parser.isoparser import isoparser, _takes_ascii
+import frozendict
 
-from dojah_client.exceptions import (
-    ApiKeyError,
-    ApiAttributeError,
+from dojah_client.exceptions_base import (
     ApiTypeError,
     ApiValueError,
 )
+from dojah_client.configuration import (
+    Configuration,
+)
+from dojah_client.exceptions import SchemaValidationError
+from dojah_client.exceptions import render_path
+from dojah_client.validation_metadata import ValidationMetadata
+from dojah_client.exceptions import AnyOfValidationError
+from dojah_client.exceptions import MissingRequiredPropertiesError
+
+Primitive: typing_extensions.TypeAlias = typing.Union[int, float, bool, str]
+
+class Unset(object):
+    """
+    An instance of this class is set as the default value for object type(dict) properties that are optional
+    When a property has an unset value, that property will not be assigned in the dict
+    """
+    pass
+
+unset = Unset()
 
 none_type = type(None)
 file_type = io.IOBase
 
 
-def convert_js_args_to_python_args(fn):
-    from functools import wraps
-    @wraps(fn)
-    def wrapped_init(_self, *args, **kwargs):
-        """
-        An attribute named `self` received from the api will conflicts with the reserved `self`
-        parameter of a class method. During generation, `self` attributes are mapped
-        to `_self` in models. Here, we name `_self` instead of `self` to avoid conflicts.
-        """
-        spec_property_naming = kwargs.get('_spec_property_naming', False)
-        if spec_property_naming:
-            kwargs = change_keys_js_to_python(
-                kwargs, _self if isinstance(
-                    _self, type) else _self.__class__)
-        return fn(_self, *args, **kwargs)
-    return wrapped_init
-
-
-class cached_property(object):
-    # this caches the result of the function call for fn with no inputs
-    # use this as a decorator on function methods that you want converted
-    # into cached properties
-    result_key = '_results'
-
-    def __init__(self, fn):
-        self._fn = fn
-
-    def __get__(self, instance, cls=None):
-        if self.result_key in vars(self):
-            return vars(self)[self.result_key]
-        else:
-            result = self._fn()
-            setattr(self, self.result_key, result)
-            return result
-
-
-PRIMITIVE_TYPES = (list, float, int, bool, datetime, date, str, file_type)
-
-
-def allows_single_value_input(cls):
-    """
-    This function returns True if the input composed schema model or any
-    descendant model allows a value only input
-    This is true for cases where oneOf contains items like:
-    oneOf:
-      - float
-      - NumberWithValidation
-      - StringEnum
-      - ArrayModel
-      - null
-    TODO: lru_cache this
-    """
-    if (
-        issubclass(cls, ModelSimple) or
-        cls in PRIMITIVE_TYPES
-    ):
-        return True
-    elif issubclass(cls, ModelComposed):
-        if not cls._composed_schemas['oneOf']:
-            return False
-        return any(allows_single_value_input(c) for c in cls._composed_schemas['oneOf'])
-    return False
+class FileIO(io.FileIO):
+    """
+    A class for storing files
+    Note: this class is not immutable
+    """
 
+    def __new__(cls, arg: typing.Union[io.FileIO, io.BufferedReader]):
+        if isinstance(arg, (io.FileIO, io.BufferedReader)):
+            if arg.closed:
+                raise ApiValueError('Invalid file state; file is closed and must be open')
+            arg.close()
+            inst = super(FileIO, cls).__new__(cls, arg.name)
+            super(FileIO, inst).__init__(arg.name)
+            return inst
+        raise ApiValueError('FileIO must be passed arg which contains the open file')
 
-def composed_model_input_classes(cls):
+    def __init__(self, arg: typing.Union[io.FileIO, io.BufferedReader]):
+        pass
+
+
+def update(d: dict, u: dict):
     """
-    This function returns a list of the possible models that can be accepted as
-    inputs.
-    TODO: lru_cache this
+    Adds u to d
+    Where each dict is defaultdict(set)
     """
-    if issubclass(cls, ModelSimple) or cls in PRIMITIVE_TYPES:
-        return [cls]
-    elif issubclass(cls, ModelNormal):
-        if cls.discriminator is None:
-            return [cls]
+    if not u:
+        return d
+    for k, v in u.items():
+        if k not in d:
+            d[k] = v
         else:
-            return get_discriminated_classes(cls)
-    elif issubclass(cls, ModelComposed):
-        if not cls._composed_schemas['oneOf']:
-            return []
-        if cls.discriminator is None:
-            input_classes = []
-            for c in cls._composed_schemas['oneOf']:
-                input_classes.extend(composed_model_input_classes(c))
-            return input_classes
-        else:
-            return get_discriminated_classes(cls)
-    return []
-
+            d[k] = d[k] | v
 
-class OpenApiModel(object):
-    """The base class for all OpenAPIModels"""
 
-    def set_attribute(self, name, value):
-        # this is only used to set properties on self
-
-        path_to_item = []
-        if self._path_to_item:
-            path_to_item.extend(self._path_to_item)
-        path_to_item.append(name)
-
-        if name in self.openapi_types:
-            required_types_mixed = self.openapi_types[name]
-        elif self.additional_properties_type is None:
-            raise ApiAttributeError(
-                "{0} has no attribute '{1}'".format(
-                    type(self).__name__, name),
-                path_to_item
-            )
-        elif self.additional_properties_type is not None:
-            required_types_mixed = self.additional_properties_type
-
-        if get_simple_class(name) != str:
-            error_msg = type_error_message(
-                var_name=name,
-                var_value=name,
-                valid_classes=(str,),
-                key_type=True
-            )
-            raise ApiTypeError(
-                error_msg,
-                path_to_item=path_to_item,
-                valid_classes=(str,),
-                key_type=True
-            )
+class Singleton:
+    """
+    Enums and singletons are the same
+    The same instance is returned for a given key of (cls, arg)
+    """
+    _instances = {}
 
-        if self._check_type:
-            value = validate_and_convert_types(
-                value, required_types_mixed, path_to_item, self._spec_property_naming,
-                self._check_type, configuration=self._configuration)
-        if (name,) in self.allowed_values:
-            check_allowed_values(
-                self.allowed_values,
-                (name,),
-                value
-            )
-        if (name,) in self.validations:
-            check_validations(
-                self.validations,
-                (name,),
-                value,
-                self._configuration
-            )
-        self.__dict__['_data_store'][name] = value
+    def __new__(cls, arg: typing.Any, **kwargs):
+        """
+        cls base classes: BoolClass, NoneClass, str, decimal.Decimal
+        The 3rd key is used in the tuple below for a corner case where an enum contains integer 1
+        However 1.0  can also be ingested into that enum schema because 1.0 == 1 and
+        Decimal('1.0') == Decimal('1')
+        But if we omitted the 3rd value in the key, then Decimal('1.0') would be stored as Decimal('1')
+        and json serializing that instance would be '1' rather than the expected '1.0'
+        Adding the 3rd value, the str of arg ensures that 1.0 -> Decimal('1.0') which is serialized as 1.0
+        """
+        key = (cls, arg, str(arg))
+        if key not in cls._instances:
+            if isinstance(arg, (none_type, bool, BoolClass, NoneClass)):
+                inst = super().__new__(cls)
+                cls._instances[key] = inst
+            else:
+                cls._instances[key] = super().__new__(cls, arg)
+        return cls._instances[key]
 
     def __repr__(self):
-        """For `print` and `pprint`"""
-        return self.to_str()
+        if isinstance(self, NoneClass):
+            return f'<{self.__class__.__name__}: None>'
+        elif isinstance(self, BoolClass):
+            if bool(self):
+                return f'<{self.__class__.__name__}: True>'
+            return f'<{self.__class__.__name__}: False>'
+        return f'<{self.__class__.__name__}: {super().__repr__()}>'
 
-    def __ne__(self, other):
-        """Returns true if both objects are not equal"""
-        return not self == other
-
-    def __setattr__(self, attr, value):
-        """set the value of an attribute using dot notation: `instance.attr = val`"""
-        self[attr] = value
-
-    def __getattr__(self, attr):
-        """get the value of an attribute using dot notation: `instance.attr`"""
-        return self.__getitem__(attr)
-
-    def __copy__(self):
-        cls = self.__class__
-        if self.get("_spec_property_naming", False):
-            return cls._new_from_openapi_data(**self.__dict__)
-        else:
-            return cls.__new__(cls, **self.__dict__)
 
-    def __deepcopy__(self, memo):
-        cls = self.__class__
+class classproperty:
 
-        if self.get("_spec_property_naming", False):
-            new_inst = cls._new_from_openapi_data()
-        else:
-            new_inst = cls.__new__(cls, **self.__dict__)
+    def __init__(self, fget):
+        self.fget = fget
 
-        for k, v in self.__dict__.items():
-            setattr(new_inst, k, deepcopy(v, memo))
-        return new_inst
+    def __get__(self, owner_self, owner_cls):
+        return self.fget(owner_cls)
 
 
-    def __new__(cls, *args, **kwargs):
-        # this function uses the discriminator to
-        # pick a new schema/class to instantiate because a discriminator
-        # propertyName value was passed in
-
-        if len(args) == 1:
-            arg = args[0]
-            if arg is None and is_type_nullable(cls):
-                # The input data is the 'null' value and the type is nullable.
-                return None
-
-            if issubclass(cls, ModelComposed) and allows_single_value_input(cls):
-                model_kwargs = {}
-                oneof_instance = get_oneof_instance(cls, model_kwargs, kwargs, model_arg=arg)
-                return oneof_instance
-
-        visited_composed_classes = kwargs.get('_visited_composed_classes', ())
-        if (
-            cls.discriminator is None or
-            cls in visited_composed_classes
-        ):
-            # Use case 1: this openapi schema (cls) does not have a discriminator
-            # Use case 2: we have already visited this class before and are sure that we
-            # want to instantiate it this time. We have visited this class deserializing
-            # a payload with a discriminator. During that process we traveled through
-            # this class but did not make an instance of it. Now we are making an
-            # instance of a composed class which contains cls in it, so this time make an instance of cls.
-            #
-            # Here's an example of use case 2: If Animal has a discriminator
-            # petType and we pass in "Dog", and the class Dog
-            # allOf includes Animal, we move through Animal
-            # once using the discriminator, and pick Dog.
-            # Then in the composed schema dog Dog, we will make an instance of the
-            # Animal class (because Dal has allOf: Animal) but this time we won't travel
-            # through Animal's discriminator because we passed in
-            # _visited_composed_classes = (Animal,)
-
-            return super(OpenApiModel, cls).__new__(cls)
-
-        # Get the name and value of the discriminator property.
-        # The discriminator name is obtained from the discriminator meta-data
-        # and the discriminator value is obtained from the input data.
-        discr_propertyname_py = list(cls.discriminator.keys())[0]
-        discr_propertyname_js = cls.attribute_map[discr_propertyname_py]
-        if discr_propertyname_js in kwargs:
-            discr_value = kwargs[discr_propertyname_js]
-        elif discr_propertyname_py in kwargs:
-            discr_value = kwargs[discr_propertyname_py]
-        else:
-            # The input data does not contain the discriminator property.
-            path_to_item = kwargs.get('_path_to_item', ())
-            raise ApiValueError(
-                "Cannot deserialize input data due to missing discriminator. "
-                "The discriminator property '%s' is missing at path: %s" %
-                (discr_propertyname_js, path_to_item)
-            )
+class NoneClass(Singleton):
+    @classproperty
+    def NONE(cls):
+        return cls(None)
 
-        # Implementation note: the last argument to get_discriminator_class
-        # is a list of visited classes. get_discriminator_class may recursively
-        # call itself and update the list of visited classes, and the initial
-        # value must be an empty list. Hence not using 'visited_composed_classes'
-        new_cls = get_discriminator_class(
-            cls, discr_propertyname_py, discr_value, [])
-        if new_cls is None:
-            path_to_item = kwargs.get('_path_to_item', ())
-            disc_prop_value = kwargs.get(
-                discr_propertyname_js, kwargs.get(discr_propertyname_py))
-            raise ApiValueError(
-                "Cannot deserialize input data due to invalid discriminator "
-                "value. The OpenAPI document has no mapping for discriminator "
-                "property '%s'='%s' at path: %s" %
-                (discr_propertyname_js, disc_prop_value, path_to_item)
-            )
-
-        if new_cls in visited_composed_classes:
-            # if we are making an instance of a composed schema Descendent
-            # which allOf includes Ancestor, then Ancestor contains
-            # a discriminator that includes Descendent.
-            # So if we make an instance of Descendent, we have to make an
-            # instance of Ancestor to hold the allOf properties.
-            # This code detects that use case and makes the instance of Ancestor
-            # For example:
-            # When making an instance of Dog, _visited_composed_classes = (Dog,)
-            # then we make an instance of Animal to include in dog._composed_instances
-            # so when we are here, cls is Animal
-            # cls.discriminator != None
-            # cls not in _visited_composed_classes
-            # new_cls = Dog
-            # but we know we know that we already have Dog
-            # because it is in visited_composed_classes
-            # so make Animal here
-            return super(OpenApiModel, cls).__new__(cls)
-
-        # Build a list containing all oneOf and anyOf descendants.
-        oneof_anyof_classes = None
-        if cls._composed_schemas is not None:
-            oneof_anyof_classes = (
-                cls._composed_schemas.get('oneOf', ()) +
-                cls._composed_schemas.get('anyOf', ()))
-        oneof_anyof_child = new_cls in oneof_anyof_classes
-        kwargs['_visited_composed_classes'] = visited_composed_classes + (cls,)
-
-        if cls._composed_schemas.get('allOf') and oneof_anyof_child:
-            # Validate that we can make self because when we make the
-            # new_cls it will not include the allOf validations in self
-            self_inst = super(OpenApiModel, cls).__new__(cls)
-            self_inst.__init__(*args, **kwargs)
-
-        if kwargs.get("_spec_property_naming", False):
-            # when true, implies new is from deserialization
-            new_inst = new_cls._new_from_openapi_data(*args, **kwargs)
-        else:
-            new_inst = new_cls.__new__(new_cls, *args, **kwargs)
-            new_inst.__init__(*args, **kwargs)
+    def __bool__(self) -> bool:
+        return False
 
-        return new_inst
+
+class BoolClass(Singleton):
+    @classproperty
+    def TRUE(cls):
+        return cls(True)
+
+    @classproperty
+    def FALSE(cls):
+        return cls(False)
+
+    @functools.lru_cache()
+    def __bool__(self) -> bool:
+        for key, instance in self._instances.items():
+            if self is instance:
+                return bool(key[1])
+        raise ValueError('Unable to find the boolean value of this instance')
+
+    def __str__(self) -> str:
+        return str(bool(self))
+
+
+class MetaOapgTyped:
+    exclusive_maximum: typing.Union[int, float]
+    inclusive_maximum: typing.Union[int, float]
+    exclusive_minimum: typing.Union[int, float]
+    inclusive_minimum: typing.Union[int, float]
+    max_items: int
+    min_items: int
+    discriminator: typing.Dict[str, typing.Dict[str, typing.Type['Schema']]]
+    x_konfig_strip: bool
+
+
+    class properties:
+        # to hold object properties
+        pass
+
+    additional_properties: typing.Optional[typing.Type['Schema']]
+    max_properties: int
+    min_properties: int
+    all_of: typing.Callable[[], typing.List[typing.Type['Schema']]]
+    one_of: typing.Callable[[], typing.List[typing.Type['Schema']]]
+    any_of: typing.Callable[[], typing.List[typing.Type['Schema']]]
+    not_schema: typing.Type['Schema']
+    max_length: int
+    min_length: int
+    items: typing.Type['Schema']
+
+
+class Schema:
+    """
+    the base class of all swagger/openapi schemas/models
+    """
+    __inheritable_primitive_types_set = {decimal.Decimal, str, tuple, frozendict.frozendict, FileIO, bytes, BoolClass, NoneClass}
+    _types: typing.Set[typing.Type]
+    MetaOapg = MetaOapgTyped
+
+    @staticmethod
+    def __get_valid_classes_phrase(input_classes):
+        """Returns a string phrase describing what types are allowed"""
+        all_classes = list(input_classes)
+        all_classes = sorted(all_classes, key=lambda cls: cls.__name__)
+        all_class_names = [cls.__name__ for cls in all_classes]
+        if len(all_class_names) == 1:
+            return "is {0}".format(all_class_names[0])
+        return "is one of [{0}]".format(", ".join(all_class_names))
+
+    @staticmethod
+    def _get_class_oapg(item_cls: typing.Union[types.FunctionType, staticmethod, typing.Type['Schema']]) -> typing.Type['Schema']:
+        if isinstance(item_cls, types.FunctionType):
+            # referenced schema
+            return item_cls()
+        elif isinstance(item_cls, staticmethod):
+            # referenced schema
+            return item_cls.__func__()
+        return item_cls
 
     @classmethod
-    @convert_js_args_to_python_args
-    def _new_from_openapi_data(cls, *args, **kwargs):
-        # this function uses the discriminator to
-        # pick a new schema/class to instantiate because a discriminator
-        # propertyName value was passed in
-
-        if len(args) == 1:
-            arg = args[0]
-            if arg is None and is_type_nullable(cls):
-                # The input data is the 'null' value and the type is nullable.
-                return None
-
-            if issubclass(cls, ModelComposed) and allows_single_value_input(cls):
-                model_kwargs = {}
-                oneof_instance = get_oneof_instance(cls, model_kwargs, kwargs, model_arg=arg)
-                return oneof_instance
-
-        visited_composed_classes = kwargs.get('_visited_composed_classes', ())
-        if (
-            cls.discriminator is None or
-            cls in visited_composed_classes
-        ):
-            # Use case 1: this openapi schema (cls) does not have a discriminator
-            # Use case 2: we have already visited this class before and are sure that we
-            # want to instantiate it this time. We have visited this class deserializing
-            # a payload with a discriminator. During that process we traveled through
-            # this class but did not make an instance of it. Now we are making an
-            # instance of a composed class which contains cls in it, so this time make an instance of cls.
-            #
-            # Here's an example of use case 2: If Animal has a discriminator
-            # petType and we pass in "Dog", and the class Dog
-            # allOf includes Animal, we move through Animal
-            # once using the discriminator, and pick Dog.
-            # Then in the composed schema dog Dog, we will make an instance of the
-            # Animal class (because Dal has allOf: Animal) but this time we won't travel
-            # through Animal's discriminator because we passed in
-            # _visited_composed_classes = (Animal,)
-
-            return cls._from_openapi_data(*args, **kwargs)
-
-        # Get the name and value of the discriminator property.
-        # The discriminator name is obtained from the discriminator meta-data
-        # and the discriminator value is obtained from the input data.
-        discr_propertyname_py = list(cls.discriminator.keys())[0]
-        discr_propertyname_js = cls.attribute_map[discr_propertyname_py]
-        if discr_propertyname_js in kwargs:
-            discr_value = kwargs[discr_propertyname_js]
-        elif discr_propertyname_py in kwargs:
-            discr_value = kwargs[discr_propertyname_py]
-        else:
-            # The input data does not contain the discriminator property.
-            path_to_item = kwargs.get('_path_to_item', ())
-            raise ApiValueError(
-                "Cannot deserialize input data due to missing discriminator. "
-                "The discriminator property '%s' is missing at path: %s" %
-                (discr_propertyname_js, path_to_item)
+    def __type_error_message(
+        cls, var_value=None, var_name=None, valid_classes=None, key_type=None
+    ):
+        """
+        Keyword Args:
+            var_value (any): the variable which has the type_error
+            var_name (str): the name of the variable which has the typ error
+            valid_classes (tuple): the accepted classes for current_item's
+                                      value
+            key_type (bool): False if our value is a value in a dict
+                             True if it is a key in a dict
+                             False if our item is an item in a tuple
+        """
+        key_or_value = "value"
+        if key_type:
+            key_or_value = "key"
+        valid_classes_phrase = cls.__get_valid_classes_phrase(valid_classes)
+        msg = "Invalid type. Required {0} type {1} and " "passed type was {2} for \"{3}\"".format(
+            key_or_value,
+            valid_classes_phrase,
+            type(var_value).__name__,
+            var_name,
+        )
+        return msg
+
+    @classmethod
+    def __get_type_error(cls, var_value, path_to_item, valid_classes, key_type=False):
+        error_msg = cls.__type_error_message(
+            var_name=path_to_item[-1],
+            var_value=var_value,
+            valid_classes=valid_classes,
+            key_type=key_type,
+        )
+        return ApiTypeError(
+            error_msg,
+            invalid_value=var_value,
+            path_to_item=path_to_item,
+            valid_classes=valid_classes,
+            key_type=key_type,
+        )
+
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ) -> typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Union['Schema', str, decimal.Decimal, BoolClass, NoneClass, frozendict.frozendict, tuple]]]:
+        """
+        Schema _validate_oapg
+        All keyword validation except for type checking was done in calling stack frames
+        If those validations passed, the validated classes are collected in path_to_schemas
+
+        Returns:
+            path_to_schemas: a map of path to schemas
+
+        Raises:
+            ApiValueError: when a string can't be converted into a date or datetime and it must be one of those classes
+            ApiTypeError: when the input type is not in the list of allowed spec types
+        """
+        base_class = type(arg)
+        if base_class not in cls._types:
+            raise cls.__get_type_error(
+                arg,
+                validation_metadata.path_to_item,
+                cls._types,
+                key_type=False,
             )
 
-        # Implementation note: the last argument to get_discriminator_class
-        # is a list of visited classes. get_discriminator_class may recursively
-        # call itself and update the list of visited classes, and the initial
-        # value must be an empty list. Hence not using 'visited_composed_classes'
-        new_cls = get_discriminator_class(
-            cls, discr_propertyname_py, discr_value, [])
-        if new_cls is None:
-            path_to_item = kwargs.get('_path_to_item', ())
-            disc_prop_value = kwargs.get(
-                discr_propertyname_js, kwargs.get(discr_propertyname_py))
-            raise ApiValueError(
-                "Cannot deserialize input data due to invalid discriminator "
-                "value. The OpenAPI document has no mapping for discriminator "
-                "property '%s'='%s' at path: %s" %
-                (discr_propertyname_js, disc_prop_value, path_to_item)
-            )
-
-        if new_cls in visited_composed_classes:
-            # if we are making an instance of a composed schema Descendent
-            # which allOf includes Ancestor, then Ancestor contains
-            # a discriminator that includes Descendent.
-            # So if we make an instance of Descendent, we have to make an
-            # instance of Ancestor to hold the allOf properties.
-            # This code detects that use case and makes the instance of Ancestor
-            # For example:
-            # When making an instance of Dog, _visited_composed_classes = (Dog,)
-            # then we make an instance of Animal to include in dog._composed_instances
-            # so when we are here, cls is Animal
-            # cls.discriminator != None
-            # cls not in _visited_composed_classes
-            # new_cls = Dog
-            # but we know we know that we already have Dog
-            # because it is in visited_composed_classes
-            # so make Animal here
-            return cls._from_openapi_data(*args, **kwargs)
-
-        # Build a list containing all oneOf and anyOf descendants.
-        oneof_anyof_classes = None
-        if cls._composed_schemas is not None:
-            oneof_anyof_classes = (
-                cls._composed_schemas.get('oneOf', ()) +
-                cls._composed_schemas.get('anyOf', ()))
-        oneof_anyof_child = new_cls in oneof_anyof_classes
-        kwargs['_visited_composed_classes'] = visited_composed_classes + (cls,)
-
-        if cls._composed_schemas.get('allOf') and oneof_anyof_child:
-            # Validate that we can make self because when we make the
-            # new_cls it will not include the allOf validations in self
-            self_inst = cls._from_openapi_data(*args, **kwargs)
+        path_to_schemas = {validation_metadata.path_to_item: set()}
+        path_to_schemas[validation_metadata.path_to_item].add(cls)
+        path_to_schemas[validation_metadata.path_to_item].add(base_class)
+        return path_to_schemas
+
+    @staticmethod
+    def _process_schema_classes_oapg(
+        schema_classes: typing.Set[typing.Union['Schema', str, decimal.Decimal, BoolClass, NoneClass, frozendict.frozendict, tuple]]
+    ):
+        """
+        Processes and mutates schema_classes
+        If a SomeSchema is a subclass of DictSchema then remove DictSchema because it is already included
+        """
+        if len(schema_classes) < 2:
+            return
+        if len(schema_classes) > 2 and UnsetAnyTypeSchema in schema_classes:
+            schema_classes.remove(UnsetAnyTypeSchema)
+        x_schema = schema_type_classes & schema_classes
+        if not x_schema:
+            return
+        x_schema = x_schema.pop()
+        if any(c is not x_schema and issubclass(c, x_schema) for c in schema_classes):
+            # needed to not have a mro error in get_new_class
+            schema_classes.remove(x_schema)
+
+    @classmethod
+    def __get_new_cls(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata
+    ) -> typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Type['Schema']]:
+        """
+        Make a new dynamic class and return an instance of that class
+        We are making an instance of cls, but instead of making cls
+        make a new class, new_cls
+        which includes dynamic bases including cls
+        return an instance of that new class
+
+        Dict property + List Item Assignment Use cases:
+        1. value is NOT an instance of the required schema class
+            the value is validated by _validate_oapg
+            _validate_oapg returns a key value pair
+            where the key is the path to the item, and the value will be the required manufactured class
+            made out of the matching schemas
+        2. value is an instance of the the correct schema type
+            the value is NOT validated by _validate_oapg, _validate_oapg only checks that the instance is of the correct schema type
+            for this value, _validate_oapg does NOT return an entry for it in _path_to_schemas
+            and in list/dict _get_items_oapg,_get_properties_oapg the value will be directly assigned
+            because value is of the correct type, and validation was run earlier when the instance was created
+        """
+        _path_to_schemas = {}
+        if validation_metadata.validated_path_to_schemas:
+            update(_path_to_schemas, validation_metadata.validated_path_to_schemas)
+        if not validation_metadata.validation_ran_earlier(cls):
+            other_path_to_schemas = cls._validate_oapg(arg, validation_metadata=validation_metadata)
+            update(_path_to_schemas, other_path_to_schemas)
+        # loop through it make a new class for each entry
+        # do not modify the returned result because it is cached and we would be modifying the cached value
+        path_to_schemas = {}
+        for path, schema_classes in _path_to_schemas.items():
+            """
+            Use cases
+            1. N number of schema classes + enum + type != bool/None, classes in path_to_schemas: tuple/frozendict.frozendict/str/Decimal/bytes/FileIo
+                needs Singleton added
+            2. N number of schema classes + enum + type == bool/None, classes in path_to_schemas: BoolClass/NoneClass
+                Singleton already added
+            3. N number of schema classes, classes in path_to_schemas: BoolClass/NoneClass/tuple/frozendict.frozendict/str/Decimal/bytes/FileIo
+            """
+            cls._process_schema_classes_oapg(schema_classes)
+            enum_schema = any(
+                issubclass(this_cls, EnumBase) for this_cls in schema_classes)
+            inheritable_primitive_type = schema_classes.intersection(cls.__inheritable_primitive_types_set)
+            chosen_schema_classes = schema_classes - inheritable_primitive_type
+            suffix = tuple(inheritable_primitive_type)
+            if enum_schema and suffix[0] not in {NoneClass, BoolClass}:
+                suffix = (Singleton,) + suffix
+
+            used_classes = tuple(sorted(chosen_schema_classes, key=lambda a_cls: a_cls.__name__)) + suffix
+            mfg_cls = get_new_class(class_name='DynamicSchema', bases=used_classes)
+            path_to_schemas[path] = mfg_cls
+
+        return path_to_schemas
+
+    @classmethod
+    def _get_new_instance_without_conversion_oapg(
+        cls,
+        arg: typing.Any,
+        path_to_item: typing.Tuple[typing.Union[str, int], ...],
+        path_to_schemas: typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Type['Schema']]
+    ):
+        # We have a Dynamic class and we are making an instance of it
+        if issubclass(cls, frozendict.frozendict) and issubclass(cls, DictBase):
+            properties = cls._get_properties_oapg(arg, path_to_item, path_to_schemas)
+            return super(Schema, cls).__new__(cls, properties)
+        elif issubclass(cls, tuple) and issubclass(cls, ListBase):
+            items = cls._get_items_oapg(arg, path_to_item, path_to_schemas)
+            return super(Schema, cls).__new__(cls, items)
+        """
+        str = openapi str, date, and datetime
+        decimal.Decimal = openapi int and float
+        FileIO = openapi binary type and the user inputs a file
+        bytes = openapi binary type and the user inputs bytes
+        """
+        return super(Schema, cls).__new__(cls, arg)
 
-        new_inst = new_cls._new_from_openapi_data(*args, **kwargs)
+    @classmethod
+    def from_openapi_data_oapg(
+        cls,
+        arg: typing.Union[
+            str,
+            date,
+            datetime,
+            int,
+            float,
+            decimal.Decimal,
+            bool,
+            None,
+            'Schema',
+            dict,
+            frozendict.frozendict,
+            tuple,
+            list,
+            io.FileIO,
+            io.BufferedReader,
+            bytes
+        ],
+        _configuration: typing.Optional[Configuration]
+    ):
+        """
+        Schema from_openapi_data_oapg
+        """
+        from_server = True
+        validated_path_to_schemas = {}
+        arg = cast_to_allowed_types(arg, from_server, validated_path_to_schemas)
+        validation_metadata = ValidationMetadata(
+            from_server=from_server, configuration=_configuration, validated_path_to_schemas=validated_path_to_schemas)
+        path_to_schemas = cls.__get_new_cls(arg, validation_metadata)
+        new_cls = path_to_schemas[validation_metadata.path_to_item]
+        new_inst = new_cls._get_new_instance_without_conversion_oapg(
+            arg,
+            validation_metadata.path_to_item,
+            path_to_schemas
+        )
         return new_inst
 
+    @staticmethod
+    def __get_input_dict(*args, **kwargs) -> frozendict.frozendict:
+        input_dict = {}
+        if args and isinstance(args[0], (dict, frozendict.frozendict)):
+            input_dict.update(args[0])
+        if kwargs:
+            input_dict.update(kwargs)
+        return frozendict.frozendict(input_dict)
+
+    @staticmethod
+    def __remove_unsets(kwargs):
+        return {key: val for key, val in kwargs.items() if val is not unset}
 
-class ModelSimple(OpenApiModel):
-    """the parent class of models whose type != object in their
-    swagger/openapi"""
-
-    def __setitem__(self, name, value):
-        """set the value of an attribute using square-bracket notation: `instance[attr] = val`"""
-        if name in self.required_properties:
-            self.__dict__[name] = value
-            return
+    def __new__(cls, *args: typing.Union[dict, frozendict.frozendict, list, tuple, decimal.Decimal, float, int, str, date, datetime, bool, None, 'Schema'], _configuration: typing.Optional[Configuration] = None, **kwargs: typing.Union[dict, frozendict.frozendict, list, tuple, decimal.Decimal, float, int, str, date, datetime, bool, None, 'Schema', Unset]):
+        """
+        Schema __new__
 
-        self.set_attribute(name, value)
+        Args:
+            args (int/float/decimal.Decimal/str/list/tuple/dict/frozendict.frozendict/bool/None): the value
+            kwargs (str, int/float/decimal.Decimal/str/list/tuple/dict/frozendict.frozendict/bool/None): dict values
+            _configuration: contains the Configuration that enables json schema validation keywords
+                like minItems, minLength etc
 
-    def get(self, name, default=None):
-        """returns the value of an attribute or some default value if the attribute was not set"""
-        if name in self.required_properties:
-            return self.__dict__[name]
-
-        return self.__dict__['_data_store'].get(name, default)
-
-    def __getitem__(self, name):
-        """get the value of an attribute using square-bracket notation: `instance[attr]`"""
-        if name in self:
-            return self.get(name)
-
-        raise ApiAttributeError(
-            "{0} has no attribute '{1}'".format(
-                type(self).__name__, name),
-            [e for e in [self._path_to_item, name] if e]
+        Note: double underscores are used here because pycharm thinks that these variables
+        are instance properties if they are named normally :(
+        """
+        _kwargs = cls.__remove_unsets(kwargs)
+        if not args and not _kwargs:
+            raise TypeError(
+                'No input given. args or kwargs must be given.'
+            )
+        if not _kwargs and args and not isinstance(args[0], dict):
+            _arg = args[0]
+        else:
+            _arg = cls.__get_input_dict(*args, **_kwargs)
+        _from_server = False
+        _validated_path_to_schemas = {}
+        _arg = cast_to_allowed_types(
+            _arg, _from_server, _validated_path_to_schemas, schema=cls)
+        _validation_metadata = ValidationMetadata(
+            configuration=_configuration, from_server=_from_server, validated_path_to_schemas=_validated_path_to_schemas)
+        _path_to_schemas = cls.__get_new_cls(_arg, _validation_metadata)
+        _new_cls = _path_to_schemas[_validation_metadata.path_to_item]
+        return _new_cls._get_new_instance_without_conversion_oapg(
+            _arg,
+            _validation_metadata.path_to_item,
+            _path_to_schemas
         )
 
-    def __contains__(self, name):
-        """used by `in` operator to check if an attribute value was set in an instance: `'attr' in instance`"""
-        if name in self.required_properties:
-            return name in self.__dict__
-
-        return name in self.__dict__['_data_store']
-
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return str(self.value)
-
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, self.__class__):
-            return False
+    def __init__(
+        self,
+        *args: typing.Union[
+            dict, frozendict.frozendict, list, tuple, decimal.Decimal, float, int, str, date, datetime, bool, None, 'Schema'],
+        _configuration: typing.Optional[Configuration] = None,
+        **kwargs: typing.Union[
+            dict, frozendict.frozendict, list, tuple, decimal.Decimal, float, int, str, date, datetime, bool, None, 'Schema', Unset
+        ]
+    ):
+        """
+        this is needed to fix 'Unexpected argument' warning in pycharm
+        this code does nothing because all Schema instances are immutable
+        this means that all input data is passed into and used in new, and after the new instance is made
+        no new attributes are assigned and init is not used
+        """
+        pass
 
-        this_val = self._data_store['value']
-        that_val = other._data_store['value']
-        types = set()
-        types.add(this_val.__class__)
-        types.add(that_val.__class__)
-        vals_equal = this_val == that_val
-        return vals_equal
-
-
-class ModelNormal(OpenApiModel):
-    """the parent class of models whose type == object in their
-    swagger/openapi"""
-
-    def __setitem__(self, name, value):
-        """set the value of an attribute using square-bracket notation: `instance[attr] = val`"""
-        if name in self.required_properties:
-            self.__dict__[name] = value
-            return
+"""
+import itertools
+data_types = ('None', 'FrozenDict', 'Tuple', 'Str', 'Decimal', 'Bool')
+type_to_cls = {
+    'None': 'NoneClass',
+    'FrozenDict': 'frozendict.frozendict',
+    'Tuple': 'tuple',
+    'Str': 'str',
+    'Decimal': 'decimal.Decimal',
+    'Bool': 'BoolClass'
+}
+cls_tuples = [v for v in itertools.combinations(data_types, 5)]
+typed_classes = [f"class {''.join(cls_tuple)}Mixin({', '.join(type_to_cls[typ] for typ in cls_tuple)}):\n    pass" for cls_tuple in cls_tuples]
+for cls in typed_classes:
+    print(cls)
+object_classes = [f"{''.join(cls_tuple)}Mixin = object" for cls_tuple in cls_tuples]
+for cls in object_classes:
+    print(cls)
+"""
+if typing.TYPE_CHECKING:
+    # qty 1
+    NoneMixin = NoneClass
+    FrozenDictMixin = frozendict.frozendict
+    IntMixin = int
+    TupleMixin = tuple
+    StrMixin = str
+    DecimalMixin = decimal.Decimal
+    BoolMixin = BoolClass
+    BytesMixin = bytes
+    FileMixin = FileIO
+    # qty 2
+    class NumberMixin(decimal.Decimal, int):
+        pass
+    class BinaryMixin(bytes, FileIO):
+        pass
+    class NoneFrozenDictMixin(NoneClass, frozendict.frozendict):
+        pass
+    class NoneTupleMixin(NoneClass, tuple):
+        pass
+    class NoneStrMixin(NoneClass, str):
+        pass
+    class NoneDecimalMixin(NoneClass, decimal.Decimal):
+        pass
+    class NoneBoolMixin(NoneClass, BoolClass):
+        pass
+    class FrozenDictTupleMixin(frozendict.frozendict, tuple):
+        pass
+    class FrozenDictStrMixin(frozendict.frozendict, str):
+        pass
+    class FrozenDictDecimalMixin(frozendict.frozendict, decimal.Decimal):
+        pass
+    class FrozenDictBoolMixin(frozendict.frozendict, BoolClass):
+        pass
+    class TupleStrMixin(tuple, str):
+        pass
+    class TupleDecimalMixin(tuple, decimal.Decimal):
+        pass
+    class TupleBoolMixin(tuple, BoolClass):
+        pass
+    class StrDecimalMixin(str, decimal.Decimal):
+        pass
+    class StrBoolMixin(str, BoolClass):
+        pass
+    class DecimalBoolMixin(decimal.Decimal, BoolClass):
+        pass
+    # qty 3
+    class NoneFrozenDictTupleMixin(NoneClass, frozendict.frozendict, tuple):
+        pass
+    class NoneFrozenDictStrMixin(NoneClass, frozendict.frozendict, str):
+        pass
+    class NoneFrozenDictDecimalMixin(NoneClass, frozendict.frozendict, decimal.Decimal):
+        pass
+    class NoneFrozenDictBoolMixin(NoneClass, frozendict.frozendict, BoolClass):
+        pass
+    class NoneTupleStrMixin(NoneClass, tuple, str):
+        pass
+    class NoneTupleDecimalMixin(NoneClass, tuple, decimal.Decimal):
+        pass
+    class NoneTupleBoolMixin(NoneClass, tuple, BoolClass):
+        pass
+    class NoneStrDecimalMixin(NoneClass, str, decimal.Decimal):
+        pass
+    class NoneStrBoolMixin(NoneClass, str, BoolClass):
+        pass
+    class NoneDecimalBoolMixin(NoneClass, decimal.Decimal, BoolClass):
+        pass
+    class FrozenDictTupleStrMixin(frozendict.frozendict, tuple, str):
+        pass
+    class FrozenDictTupleDecimalMixin(frozendict.frozendict, tuple, decimal.Decimal):
+        pass
+    class FrozenDictTupleBoolMixin(frozendict.frozendict, tuple, BoolClass):
+        pass
+    class FrozenDictStrDecimalMixin(frozendict.frozendict, str, decimal.Decimal):
+        pass
+    class FrozenDictStrBoolMixin(frozendict.frozendict, str, BoolClass):
+        pass
+    class FrozenDictDecimalBoolMixin(frozendict.frozendict, decimal.Decimal, BoolClass):
+        pass
+    class TupleStrDecimalMixin(tuple, str, decimal.Decimal):
+        pass
+    class TupleStrBoolMixin(tuple, str, BoolClass):
+        pass
+    class TupleDecimalBoolMixin(tuple, decimal.Decimal, BoolClass):
+        pass
+    class StrDecimalBoolMixin(str, decimal.Decimal, BoolClass):
+        pass
+    # qty 4
+    class NoneFrozenDictTupleStrMixin(NoneClass, frozendict.frozendict, tuple, str):
+        pass
+    class NoneFrozenDictTupleDecimalMixin(NoneClass, frozendict.frozendict, tuple, decimal.Decimal):
+        pass
+    class NoneFrozenDictTupleBoolMixin(NoneClass, frozendict.frozendict, tuple, BoolClass):
+        pass
+    class NoneFrozenDictStrDecimalMixin(NoneClass, frozendict.frozendict, str, decimal.Decimal):
+        pass
+    class NoneFrozenDictStrBoolMixin(NoneClass, frozendict.frozendict, str, BoolClass):
+        pass
+    class NoneFrozenDictDecimalBoolMixin(NoneClass, frozendict.frozendict, decimal.Decimal, BoolClass):
+        pass
+    class NoneTupleStrDecimalMixin(NoneClass, tuple, str, decimal.Decimal):
+        pass
+    class NoneTupleStrBoolMixin(NoneClass, tuple, str, BoolClass):
+        pass
+    class NoneTupleDecimalBoolMixin(NoneClass, tuple, decimal.Decimal, BoolClass):
+        pass
+    class NoneStrDecimalBoolMixin(NoneClass, str, decimal.Decimal, BoolClass):
+        pass
+    class FrozenDictTupleStrDecimalMixin(frozendict.frozendict, tuple, str, decimal.Decimal):
+        pass
+    class FrozenDictTupleStrBoolMixin(frozendict.frozendict, tuple, str, BoolClass):
+        pass
+    class FrozenDictTupleDecimalBoolMixin(frozendict.frozendict, tuple, decimal.Decimal, BoolClass):
+        pass
+    class FrozenDictStrDecimalBoolMixin(frozendict.frozendict, str, decimal.Decimal, BoolClass):
+        pass
+    class TupleStrDecimalBoolMixin(tuple, str, decimal.Decimal, BoolClass):
+        pass
+    # qty 5
+    class NoneFrozenDictTupleStrDecimalMixin(NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal):
+        pass
+    class NoneFrozenDictTupleStrBoolMixin(NoneClass, frozendict.frozendict, tuple, str, BoolClass):
+        pass
+    class NoneFrozenDictTupleDecimalBoolMixin(NoneClass, frozendict.frozendict, tuple, decimal.Decimal, BoolClass):
+        pass
+    class NoneFrozenDictStrDecimalBoolMixin(NoneClass, frozendict.frozendict, str, decimal.Decimal, BoolClass):
+        pass
+    class NoneTupleStrDecimalBoolMixin(NoneClass, tuple, str, decimal.Decimal, BoolClass):
+        pass
+    class FrozenDictTupleStrDecimalBoolMixin(frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass):
+        pass
+    # qty 6
+    class NoneFrozenDictTupleStrDecimalBoolMixin(NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass):
+        pass
+    # qty 9
+    class NoneFrozenDictTupleStrIntDecimalBoolFileBytesMixin(NoneClass, frozendict.frozendict, tuple, str, int, decimal.Decimal, BoolClass, FileIO, bytes):
+        pass
+else:
+    # qty 1
+    class NoneMixin:
+        _types = {NoneClass}
+    class FrozenDictMixin:
+        _types = {frozendict.frozendict}
+    class TupleMixin:
+        _types = {tuple}
+    class StrMixin:
+        _types = {str}
+    class DecimalMixin:
+        _types = {decimal.Decimal}
+    class IntMixin:
+        _types = {int}
+    class BoolMixin:
+        _types = {BoolClass}
+    class BytesMixin:
+        _types = {bytes}
+    class FileMixin:
+        _types = {FileIO}
+    # qty 2
+    class NumberMixin:
+        _types = {decimal.Decimal, int}
+    class BinaryMixin:
+        _types = {bytes, FileIO}
+    class NoneFrozenDictMixin:
+        _types = {NoneClass, frozendict.frozendict}
+    class NoneTupleMixin:
+        _types = {NoneClass, tuple}
+    class NoneStrMixin:
+        _types = {NoneClass, str}
+    class NoneDecimalMixin:
+        _types = {NoneClass, decimal.Decimal}
+    class NoneBoolMixin:
+        _types = {NoneClass, BoolClass}
+    class FrozenDictTupleMixin:
+        _types = {frozendict.frozendict, tuple}
+    class FrozenDictStrMixin:
+        _types = {frozendict.frozendict, str}
+    class FrozenDictDecimalMixin:
+        _types = {frozendict.frozendict, decimal.Decimal}
+    class FrozenDictBoolMixin:
+        _types = {frozendict.frozendict, BoolClass}
+    class TupleStrMixin:
+        _types = {tuple, str}
+    class TupleDecimalMixin:
+        _types = {tuple, decimal.Decimal}
+    class TupleBoolMixin:
+        _types = {tuple, BoolClass}
+    class StrDecimalMixin:
+        _types = {str, decimal.Decimal}
+    class StrBoolMixin:
+        _types = {str, BoolClass}
+    class DecimalBoolMixin:
+        _types = {decimal.Decimal, BoolClass}
+    # qty 3
+    class NoneFrozenDictTupleMixin:
+        _types = {NoneClass, frozendict.frozendict, tuple}
+    class NoneFrozenDictStrMixin:
+        _types = {NoneClass, frozendict.frozendict, str}
+    class NoneFrozenDictDecimalMixin:
+        _types = {NoneClass, frozendict.frozendict, decimal.Decimal}
+    class NoneFrozenDictBoolMixin:
+        _types = {NoneClass, frozendict.frozendict, BoolClass}
+    class NoneTupleStrMixin:
+        _types = {NoneClass, tuple, str}
+    class NoneTupleDecimalMixin:
+        _types = {NoneClass, tuple, decimal.Decimal}
+    class NoneTupleBoolMixin:
+        _types = {NoneClass, tuple, BoolClass}
+    class NoneStrDecimalMixin:
+        _types = {NoneClass, str, decimal.Decimal}
+    class NoneStrBoolMixin:
+        _types = {NoneClass, str, BoolClass}
+    class NoneDecimalBoolMixin:
+        _types = {NoneClass, decimal.Decimal, BoolClass}
+    class FrozenDictTupleStrMixin:
+        _types = {frozendict.frozendict, tuple, str}
+    class FrozenDictTupleDecimalMixin:
+        _types = {frozendict.frozendict, tuple, decimal.Decimal}
+    class FrozenDictTupleBoolMixin:
+        _types = {frozendict.frozendict, tuple, BoolClass}
+    class FrozenDictStrDecimalMixin:
+        _types = {frozendict.frozendict, str, decimal.Decimal}
+    class FrozenDictStrBoolMixin:
+        _types = {frozendict.frozendict, str, BoolClass}
+    class FrozenDictDecimalBoolMixin:
+        _types = {frozendict.frozendict, decimal.Decimal, BoolClass}
+    class TupleStrDecimalMixin:
+        _types = {tuple, str, decimal.Decimal}
+    class TupleStrBoolMixin:
+        _types = {tuple, str, BoolClass}
+    class TupleDecimalBoolMixin:
+        _types = {tuple, decimal.Decimal, BoolClass}
+    class StrDecimalBoolMixin:
+        _types = {str, decimal.Decimal, BoolClass}
+    # qty 4
+    class NoneFrozenDictTupleStrMixin:
+        _types = {NoneClass, frozendict.frozendict, tuple, str}
+    class NoneFrozenDictTupleDecimalMixin:
+        _types = {NoneClass, frozendict.frozendict, tuple, decimal.Decimal}
+    class NoneFrozenDictTupleBoolMixin:
+        _types = {NoneClass, frozendict.frozendict, tuple, BoolClass}
+    class NoneFrozenDictStrDecimalMixin:
+        _types = {NoneClass, frozendict.frozendict, str, decimal.Decimal}
+    class NoneFrozenDictStrBoolMixin:
+        _types = {NoneClass, frozendict.frozendict, str, BoolClass}
+    class NoneFrozenDictDecimalBoolMixin:
+        _types = {NoneClass, frozendict.frozendict, decimal.Decimal, BoolClass}
+    class NoneTupleStrDecimalMixin:
+        _types = {NoneClass, tuple, str, decimal.Decimal}
+    class NoneTupleStrBoolMixin:
+        _types = {NoneClass, tuple, str, BoolClass}
+    class NoneTupleDecimalBoolMixin:
+        _types = {NoneClass, tuple, decimal.Decimal, BoolClass}
+    class NoneStrDecimalBoolMixin:
+        _types = {NoneClass, str, decimal.Decimal, BoolClass}
+    class FrozenDictTupleStrDecimalMixin:
+        _types = {frozendict.frozendict, tuple, str, decimal.Decimal}
+    class FrozenDictTupleStrBoolMixin:
+        _types = {frozendict.frozendict, tuple, str, BoolClass}
+    class FrozenDictTupleDecimalBoolMixin:
+        _types = {frozendict.frozendict, tuple, decimal.Decimal, BoolClass}
+    class FrozenDictStrDecimalBoolMixin:
+        _types = {frozendict.frozendict, str, decimal.Decimal, BoolClass}
+    class TupleStrDecimalBoolMixin:
+        _types = {tuple, str, decimal.Decimal, BoolClass}
+    # qty 5
+    class NoneFrozenDictTupleStrDecimalMixin:
+        _types = {NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal}
+    class NoneFrozenDictTupleStrBoolMixin:
+        _types = {NoneClass, frozendict.frozendict, tuple, str, BoolClass}
+    class NoneFrozenDictTupleDecimalBoolMixin:
+        _types = {NoneClass, frozendict.frozendict, tuple, decimal.Decimal, BoolClass}
+    class NoneFrozenDictStrDecimalBoolMixin:
+        _types = {NoneClass, frozendict.frozendict, str, decimal.Decimal, BoolClass}
+    class NoneTupleStrDecimalBoolMixin:
+        _types = {NoneClass, tuple, str, decimal.Decimal, BoolClass}
+    class FrozenDictTupleStrDecimalBoolMixin:
+        _types = {frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass}
+    # qty 6
+    class NoneFrozenDictTupleStrDecimalBoolMixin:
+        _types = {NoneClass, frozendict.frozendict, tuple, str, decimal.Decimal, BoolClass}
+    # qty 9
+    class NoneFrozenDictTupleStrIntDecimalBoolFileBytesMixin:
+        _types = {NoneClass, frozendict.frozendict, tuple, str, int, decimal.Decimal, BoolClass, FileIO, bytes}
+
+
+class ValidatorBase:
+    @staticmethod
+    def _is_json_validation_enabled_oapg(schema_keyword, configuration=None):
+        """Returns true if JSON schema validation is enabled for the specified
+        validation keyword. This can be used to skip JSON schema structural validation
+        as requested in the configuration.
+        Note: the suffix _oapg stands for openapi python (experimental) generator and
+        it has been added to prevent collisions with other methods and properties
+
+        Args:
+            schema_keyword (string): the name of a JSON schema validation keyword.
+            configuration (Configuration): the configuration class.
+        """
 
-        self.set_attribute(name, value)
+        return (configuration is None or
+            not hasattr(configuration, '_disabled_client_side_validations') or
+            schema_keyword not in configuration._disabled_client_side_validations)
 
-    def get(self, name, default=None):
-        """returns the value of an attribute or some default value if the attribute was not set"""
-        if name in self.required_properties:
-            return self.__dict__[name]
-
-        return self.__dict__['_data_store'].get(name, default)
-
-    def __getitem__(self, name):
-        """get the value of an attribute using square-bracket notation: `instance[attr]`"""
-        if name in self:
-            return self.get(name)
-
-        raise ApiAttributeError(
-            "{0} has no attribute '{1}'".format(
-                type(self).__name__, name),
-            [e for e in [self._path_to_item, name] if e]
+    @staticmethod
+    def _raise_validation_errror_message_oapg(value, constraint_msg, constraint_value, path_to_item, additional_txt=""):
+        raise ApiValueError(
+            "Invalid value `{value}`, {constraint_msg} `{constraint_value}`{additional_txt} at {path_to_item}".format(
+                value=value,
+                constraint_msg=constraint_msg,
+                constraint_value=constraint_value,
+                additional_txt=additional_txt,
+                path_to_item=render_path(path_to_item),
+            )
         )
 
-    def __contains__(self, name):
-        """used by `in` operator to check if an attribute value was set in an instance: `'attr' in instance`"""
-        if name in self.required_properties:
-            return name in self.__dict__
-
-        return name in self.__dict__['_data_store']
-
-    def to_dict(self):
-        """Returns the model properties as a dict"""
-        return model_to_dict(self, serialize=False)
-
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return pprint.pformat(self.to_dict())
-
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, self.__class__):
+
+class EnumBase:
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ) -> typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Union['Schema', str, decimal.Decimal, BoolClass, NoneClass, frozendict.frozendict, tuple]]]:
+        """
+        EnumBase _validate_oapg
+        Validates that arg is in the enum's allowed values
+        """
+        try:
+            cls.MetaOapg.enum_value_to_name[arg]
+        except KeyError:
+            raise ApiValueError("Invalid value {} passed in to {}, allowed_values={}".format(arg, cls, cls.MetaOapg.enum_value_to_name.keys()))
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
+
+
+class BoolBase:
+    def is_true_oapg(self) -> bool:
+        """
+        A replacement for x is True
+        True if the instance is a BoolClass True Singleton
+        """
+        if not issubclass(self.__class__, BoolClass):
             return False
+        return bool(self)
 
-        if not set(self._data_store.keys()) == set(other._data_store.keys()):
+    def is_false_oapg(self) -> bool:
+        """
+        A replacement for x is False
+        True if the instance is a BoolClass False Singleton
+        """
+        if not issubclass(self.__class__, BoolClass):
             return False
-        for _var_name, this_val in self._data_store.items():
-            that_val = other._data_store[_var_name]
-            types = set()
-            types.add(this_val.__class__)
-            types.add(that_val.__class__)
-            vals_equal = this_val == that_val
-            if not vals_equal:
-                return False
-        return True
-
-
-class ModelComposed(OpenApiModel):
-    """the parent class of models whose type == object in their
-    swagger/openapi and have oneOf/allOf/anyOf
-
-    When one sets a property we use var_name_to_model_instances to store the value in
-    the correct class instances + run any type checking + validation code.
-    When one gets a property we use var_name_to_model_instances to get the value
-    from the correct class instances.
-    This allows multiple composed schemas to contain the same property with additive
-    constraints on the value.
-
-    _composed_schemas (dict) stores the anyOf/allOf/oneOf classes
-    key (str): allOf/oneOf/anyOf
-    value (list): the classes in the XOf definition.
-        Note: none_type can be included when the openapi document version >= 3.1.0
-    _composed_instances (list): stores a list of instances of the composed schemas
-    defined in _composed_schemas. When properties are accessed in the self instance,
-    they are returned from the self._data_store or the data stores in the instances
-    in self._composed_schemas
-    _var_name_to_model_instances (dict): maps between a variable name on self and
-    the composed instances (self included) which contain that data
-    key (str): property name
-    value (list): list of class instances, self or instances in _composed_instances
-    which contain the value that the key is referring to.
-    """
-
-    def __setitem__(self, name, value):
-        """set the value of an attribute using square-bracket notation: `instance[attr] = val`"""
-        if name in self.required_properties:
-            self.__dict__[name] = value
+        return bool(self) is False
+
+
+class NoneBase:
+    def is_none_oapg(self) -> bool:
+        """
+        A replacement for x is None
+        True if the instance is a NoneClass None Singleton
+        """
+        if issubclass(self.__class__, NoneClass):
+            return True
+        return False
+
+
+class StrBase(ValidatorBase):
+    MetaOapg: MetaOapgTyped
+
+    @property
+    def as_str_oapg(self) -> str:
+        return self
+
+    @property
+    def as_date_oapg(self) -> date:
+        raise Exception('not implemented')
+
+    @property
+    def as_datetime_oapg(self) -> datetime:
+        raise Exception('not implemented')
+
+    @property
+    def as_decimal_oapg(self) -> decimal.Decimal:
+        raise Exception('not implemented')
+
+    @property
+    def as_uuid_oapg(self) -> uuid.UUID:
+        raise Exception('not implemented')
+
+    @classmethod
+    def __check_str_validations(
+        cls,
+        arg: str,
+        validation_metadata: ValidationMetadata
+    ):
+        if not hasattr(cls, 'MetaOapg'):
             return
+        if (cls._is_json_validation_enabled_oapg('maxLength', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'max_length') and
+                len(arg) > cls.MetaOapg.max_length):
+            cls._raise_validation_errror_message_oapg(
+                value=arg,
+                constraint_msg="length must be less than or equal to",
+                constraint_value=cls.MetaOapg.max_length,
+                path_to_item=validation_metadata.path_to_item
+            )
+
+        if (cls._is_json_validation_enabled_oapg('minLength', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'min_length') and
+                len(arg) < cls.MetaOapg.min_length):
+            cls._raise_validation_errror_message_oapg(
+                value=arg,
+                constraint_msg="length must be greater than or equal to",
+                constraint_value=cls.MetaOapg.min_length,
+                path_to_item=validation_metadata.path_to_item
+            )
+
+        if (cls._is_json_validation_enabled_oapg('pattern', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'regex')):
+            for regex_dict in cls.MetaOapg.regex:
+                flags = regex_dict.get('flags', 0)
+                if not re.search(regex_dict['pattern'], arg, flags=flags):
+                    if flags != 0:
+                        # Don't print the regex flags if the flags are not
+                        # specified in the OAS document.
+                        cls._raise_validation_errror_message_oapg(
+                            value=arg,
+                            constraint_msg="must match regular expression",
+                            constraint_value=regex_dict['pattern'],
+                            path_to_item=validation_metadata.path_to_item,
+                            additional_txt=" with flags=`{}`".format(flags)
+                        )
+                    cls._raise_validation_errror_message_oapg(
+                        value=arg,
+                        constraint_msg="must match regular expression",
+                        constraint_value=regex_dict['pattern'],
+                        path_to_item=validation_metadata.path_to_item
+                    )
 
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ) -> typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Union['Schema', str, decimal.Decimal, BoolClass, NoneClass, frozendict.frozendict, tuple]]]:
         """
-        Use cases:
-        1. additional_properties_type is None (additionalProperties == False in spec)
-            Check for property presence in self.openapi_types
-            if not present then throw an error
-            if present set in self, set attribute
-            always set on composed schemas
-        2.  additional_properties_type exists
-            set attribute on self
-            always set on composed schemas
+        StrBase _validate_oapg
+        Validates that validations pass
         """
-        if self.additional_properties_type is None:
-            """
-            For an attribute to exist on a composed schema it must:
-            - fulfill schema_requirements in the self composed schema not considering oneOf/anyOf/allOf schemas AND
-            - fulfill schema_requirements in each oneOf/anyOf/allOf schemas
-
-            schema_requirements:
-            For an attribute to exist on a schema it must:
-            - be present in properties at the schema OR
-            - have additionalProperties unset (defaults additionalProperties = any type) OR
-            - have additionalProperties set
-            """
-            if name not in self.openapi_types:
-                raise ApiAttributeError(
-                    "{0} has no attribute '{1}'".format(
-                        type(self).__name__, name),
-                    [e for e in [self._path_to_item, name] if e]
+        if isinstance(arg, str):
+            if hasattr(cls.MetaOapg, 'x_konfig_strip') and cls.MetaOapg.x_konfig_strip:
+                arg = arg.strip()
+            cls.__check_str_validations(arg, validation_metadata)
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
+
+
+class UUIDBase:
+    @property
+    @functools.lru_cache()
+    def as_uuid_oapg(self) -> uuid.UUID:
+        return uuid.UUID(self)
+
+    @classmethod
+    def __validate_format(cls, arg: typing.Optional[str], validation_metadata: ValidationMetadata):
+        if isinstance(arg, str):
+            try:
+                uuid.UUID(arg)
+                return True
+            except ValueError:
+                raise ApiValueError(
+                    "Invalid value '{}' for type UUID at {}".format(arg, validation_metadata.path_to_item)
                 )
-        # attribute must be set on self and composed instances
-        self.set_attribute(name, value)
-        for model_instance in self._composed_instances:
-            setattr(model_instance, name, value)
-        if name not in self._var_name_to_model_instances:
-            # we assigned an additional property
-            self.__dict__['_var_name_to_model_instances'][name] = self._composed_instances + [self]
-        return None
 
-    __unset_attribute_value__ = object()
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: typing.Optional[ValidationMetadata] = None,
+    ):
+        """
+        UUIDBase _validate_oapg
+        """
+        cls.__validate_format(arg, validation_metadata=validation_metadata)
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
 
-    def get(self, name, default=None):
-        """returns the value of an attribute or some default value if the attribute was not set"""
-        if name in self.required_properties:
-            return self.__dict__[name]
-
-        # get the attribute from the correct instance
-        model_instances = self._var_name_to_model_instances.get(name)
-        values = []
-        # A composed model stores self and child (oneof/anyOf/allOf) models under
-        # self._var_name_to_model_instances.
-        # Any property must exist in self and all model instances
-        # The value stored in all model instances must be the same
-        if model_instances:
-            for model_instance in model_instances:
-                if name in model_instance._data_store:
-                    v = model_instance._data_store[name]
-                    if v not in values:
-                        values.append(v)
-        len_values = len(values)
-        if len_values == 0:
-            return default
-        elif len_values == 1:
-            return values[0]
-        elif len_values > 1:
-            raise ApiValueError(
-                "Values stored for property {0} in {1} differ when looking "
-                "at self and self's composed instances. All values must be "
-                "the same".format(name, type(self).__name__),
-                [e for e in [self._path_to_item, name] if e]
-            )
-
-    def __getitem__(self, name):
-        """get the value of an attribute using square-bracket notation: `instance[attr]`"""
-        value = self.get(name, self.__unset_attribute_value__)
-        if value is self.__unset_attribute_value__:
-            raise ApiAttributeError(
-                "{0} has no attribute '{1}'".format(
-                    type(self).__name__, name),
-                    [e for e in [self._path_to_item, name] if e]
-            )
-        return value
-
-    def __contains__(self, name):
-        """used by `in` operator to check if an attribute value was set in an instance: `'attr' in instance`"""
-
-        if name in self.required_properties:
-            return name in self.__dict__
-
-        model_instances = self._var_name_to_model_instances.get(
-            name, self._additional_properties_model_instances)
-
-        if model_instances:
-            for model_instance in model_instances:
-                if name in model_instance._data_store:
-                    return True
 
-        return False
+class CustomIsoparser(isoparser):
 
-    def to_dict(self):
-        """Returns the model properties as a dict"""
-        return model_to_dict(self, serialize=False)
-
-    def to_str(self):
-        """Returns the string representation of the model"""
-        return pprint.pformat(self.to_dict())
-
-    def __eq__(self, other):
-        """Returns true if both objects are equal"""
-        if not isinstance(other, self.__class__):
-            return False
+    @_takes_ascii
+    def parse_isodatetime(self, dt_str):
+        components, pos = self._parse_isodate(dt_str)
+        if len(dt_str) > pos:
+            if self._sep is None or dt_str[pos:pos + 1] == self._sep:
+                components += self._parse_isotime(dt_str[pos + 1:])
+            else:
+                raise ValueError('String contains unknown ISO components')
 
-        if not set(self._data_store.keys()) == set(other._data_store.keys()):
-            return False
-        for _var_name, this_val in self._data_store.items():
-            that_val = other._data_store[_var_name]
-            types = set()
-            types.add(this_val.__class__)
-            types.add(that_val.__class__)
-            vals_equal = this_val == that_val
-            if not vals_equal:
-                return False
-        return True
-
-
-COERCION_INDEX_BY_TYPE = {
-    ModelComposed: 0,
-    ModelNormal: 1,
-    ModelSimple: 2,
-    none_type: 3,    # The type of 'None'.
-    list: 4,
-    dict: 5,
-    float: 6,
-    int: 7,
-    bool: 8,
-    datetime: 9,
-    date: 10,
-    str: 11,
-    file_type: 12,   # 'file_type' is an alias for the built-in 'file' or 'io.IOBase' type.
-}
+        if len(components) > 3 and components[3] == 24:
+            components[3] = 0
+            return datetime(*components) + timedelta(days=1)
 
-# these are used to limit what type conversions we try to do
-# when we have a valid type already and we want to try converting
-# to another type
-UPCONVERSION_TYPE_PAIRS = (
-    (str, datetime),
-    (str, date),
-    # A float may be serialized as an integer, e.g. '3' is a valid serialized float.
-    (int, float),
-    (list, ModelComposed),
-    (dict, ModelComposed),
-    (str, ModelComposed),
-    (int, ModelComposed),
-    (float, ModelComposed),
-    (list, ModelComposed),
-    (list, ModelNormal),
-    (dict, ModelNormal),
-    (str, ModelSimple),
-    (int, ModelSimple),
-    (float, ModelSimple),
-    (list, ModelSimple),
-)
+        if len(components) <= 3:
+            raise ValueError('Value is not a datetime')
 
-COERCIBLE_TYPE_PAIRS = {
-    False: (  # client instantiation of a model with client data
-        # (dict, ModelComposed),
-        # (list, ModelComposed),
-        # (dict, ModelNormal),
-        # (list, ModelNormal),
-        # (str, ModelSimple),
-        # (int, ModelSimple),
-        # (float, ModelSimple),
-        # (list, ModelSimple),
-        # (str, int),
-        # (str, float),
-        # (str, datetime),
-        # (str, date),
-        # (int, str),
-        # (float, str),
-    ),
-    True: (  # server -> client data
-        (dict, ModelComposed),
-        (list, ModelComposed),
-        (dict, ModelNormal),
-        (list, ModelNormal),
-        (str, ModelSimple),
-        (int, ModelSimple),
-        (float, ModelSimple),
-        (list, ModelSimple),
-        # (str, int),
-        # (str, float),
-        (str, datetime),
-        (str, date),
-        # (int, str),
-        # (float, str),
-        (str, file_type)
-    ),
-}
+        return datetime(*components)
 
+    @_takes_ascii
+    def parse_isodate(self, datestr):
+        components, pos = self._parse_isodate(datestr)
 
-def get_simple_class(input_value):
-    """Returns an input_value's simple class that we will use for type checking
-    Python2:
-    float and int will return int, where int is the python3 int backport
-    str and unicode will return str, where str is the python3 str backport
-    Note: float and int ARE both instances of int backport
-    Note: str_py2 and unicode_py2 are NOT both instances of str backport
+        if len(datestr) > pos:
+            raise ValueError('String contains invalid time components')
 
-    Args:
-        input_value (class/class_instance): the item for which we will return
-                                            the simple class
+        if len(components) > 3:
+            raise ValueError('String contains invalid time components')
+
+        return date(*components)
+
+
+DEFAULT_ISOPARSER = CustomIsoparser()
+
+
+class DateBase:
+    @property
+    @functools.lru_cache()
+    def as_date_oapg(self) -> date:
+        return DEFAULT_ISOPARSER.parse_isodate(self)
+
+    @classmethod
+    def __validate_format(cls, arg: typing.Optional[str], validation_metadata: ValidationMetadata):
+        if isinstance(arg, str):
+            try:
+                DEFAULT_ISOPARSER.parse_isodate(arg)
+                return True
+            except ValueError:
+                raise ApiValueError(
+                    "Value does not conform to the required ISO-8601 date format. "
+                    "Invalid value '{}' for type date at {}".format(arg, validation_metadata.path_to_item)
+                )
+
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: typing.Optional[ValidationMetadata] = None,
+    ):
+        """
+        DateBase _validate_oapg
+        """
+        cls.__validate_format(arg, validation_metadata=validation_metadata)
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
+
+
+class DateTimeBase:
+    @property
+    @functools.lru_cache()
+    def as_datetime_oapg(self) -> datetime:
+        return DEFAULT_ISOPARSER.parse_isodatetime(self)
+
+    @classmethod
+    def __validate_format(cls, arg: typing.Optional[str], validation_metadata: ValidationMetadata):
+        if isinstance(arg, str):
+            try:
+                DEFAULT_ISOPARSER.parse_isodatetime(arg)
+                return True
+            except ValueError:
+                raise ApiValueError(
+                    "Value does not conform to the required ISO-8601 datetime format. "
+                    "Invalid value '{}' for type datetime at {}".format(arg, validation_metadata.path_to_item)
+                )
+
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ):
+        """
+        DateTimeBase _validate_oapg
+        """
+        cls.__validate_format(arg, validation_metadata=validation_metadata)
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
+
+
+class DecimalBase:
+    """
+    A class for storing decimals that are sent over the wire as strings
+    These schemas must remain based on StrBase rather than NumberBase
+    because picking base classes must be deterministic
     """
-    if isinstance(input_value, type):
-        # input_value is a class
-        return input_value
-    elif isinstance(input_value, tuple):
-        return tuple
-    elif isinstance(input_value, list):
-        return list
-    elif isinstance(input_value, dict):
-        return dict
-    elif isinstance(input_value, none_type):
-        return none_type
-    elif isinstance(input_value, file_type):
-        return file_type
-    elif isinstance(input_value, bool):
-        # this must be higher than the int check because
-        # isinstance(True, int) == True
-        return bool
-    elif isinstance(input_value, int):
-        return int
-    elif isinstance(input_value, datetime):
-        # this must be higher than the date check because
-        # isinstance(datetime_instance, date) == True
-        return datetime
-    elif isinstance(input_value, date):
-        return date
-    elif isinstance(input_value, str):
-        return str
-    return type(input_value)
 
+    @property
+    @functools.lru_cache()
+    def as_decimal_oapg(self) -> decimal.Decimal:
+        return decimal.Decimal(self)
 
-def check_allowed_values(allowed_values, input_variable_path, input_values):
-    """Raises an exception if the input_values are not allowed
+    @classmethod
+    def __validate_format(cls, arg: typing.Optional[str], validation_metadata: ValidationMetadata):
+        if isinstance(arg, str):
+            try:
+                decimal.Decimal(arg)
+                return True
+            except decimal.InvalidOperation:
+                raise ApiValueError(
+                    "Value cannot be converted to a decimal. "
+                    "Invalid value '{}' for type decimal at {}".format(arg, validation_metadata.path_to_item)
+                )
 
-    Args:
-        allowed_values (dict): the allowed_values dict
-        input_variable_path (tuple): the path to the input variable
-        input_values (list/str/int/float/date/datetime): the values that we
-            are checking to see if they are in allowed_values
-    """
-    these_allowed_values = list(allowed_values[input_variable_path].values())
-    if (isinstance(input_values, list)
-            and not set(input_values).issubset(
-                set(these_allowed_values))):
-        invalid_values = ", ".join(
-            map(str, set(input_values) - set(these_allowed_values))),
-        raise ApiValueError(
-            "Invalid values for `%s` [%s], must be a subset of [%s]" %
-            (
-                input_variable_path[0],
-                invalid_values,
-                ", ".join(map(str, these_allowed_values))
-            )
-        )
-    elif (isinstance(input_values, dict)
-            and not set(
-                input_values.keys()).issubset(set(these_allowed_values))):
-        invalid_values = ", ".join(
-            map(str, set(input_values.keys()) - set(these_allowed_values)))
-        raise ApiValueError(
-            "Invalid keys in `%s` [%s], must be a subset of [%s]" %
-            (
-                input_variable_path[0],
-                invalid_values,
-                ", ".join(map(str, these_allowed_values))
-            )
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ):
+        """
+        DecimalBase _validate_oapg
+        """
+        cls.__validate_format(arg, validation_metadata=validation_metadata)
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
+
+
+class NumberBase(ValidatorBase):
+    MetaOapg: MetaOapgTyped
+
+    @property
+    def as_int_oapg(self) -> int:
+        try:
+            return self._as_int
+        except AttributeError:
+            """
+            Note: for some numbers like 9.0 they could be represented as an
+            integer but our code chooses to store them as
+            >>> Decimal('9.0').as_tuple()
+            DecimalTuple(sign=0, digits=(9, 0), exponent=-1)
+            so we can tell that the value came from a float and convert it back to a float
+            during later serialization
+            """
+            if self.as_tuple().exponent < 0:
+                # this could be represented as an integer but should be represented as a float
+                # because that's what it was serialized from
+                raise ApiValueError(f'{self} is not an integer')
+            self._as_int = int(self)
+            return self._as_int
+
+    @property
+    def as_float_oapg(self) -> float:
+        try:
+            return self._as_float
+        except AttributeError:
+            if self.as_tuple().exponent >= 0:
+                raise ApiValueError(f'{self} is not an float')
+            self._as_float = float(self)
+            return self._as_float
+
+    @classmethod
+    def __check_numeric_validations(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata
+    ):
+        if not hasattr(cls, 'MetaOapg'):
+            return
+        if cls._is_json_validation_enabled_oapg('multipleOf',
+                                      validation_metadata.configuration) and hasattr(cls.MetaOapg, 'multiple_of'):
+            multiple_of_value = cls.MetaOapg.multiple_of
+            if (not (float(arg) / multiple_of_value).is_integer()):
+                # Note 'multipleOf' will be as good as the floating point arithmetic.
+                cls._raise_validation_errror_message_oapg(
+                    value=arg,
+                    constraint_msg="value must be a multiple of",
+                    constraint_value=multiple_of_value,
+                    path_to_item=validation_metadata.path_to_item
+                )
+
+        checking_max_or_min_values = any(
+            hasattr(cls.MetaOapg, validation_key) for validation_key in {
+                'exclusive_maximum',
+                'inclusive_maximum',
+                'exclusive_minimum',
+                'inclusive_minimum',
+            }
         )
-    elif (not isinstance(input_values, (list, dict))
-            and input_values not in these_allowed_values):
-        raise ApiValueError(
-            "Invalid value for `%s` (%s), must be one of %s" %
-            (
-                input_variable_path[0],
-                input_values,
-                these_allowed_values
+        if not checking_max_or_min_values:
+            return
+
+        if (cls._is_json_validation_enabled_oapg('exclusiveMaximum', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'exclusive_maximum') and
+                arg >= cls.MetaOapg.exclusive_maximum):
+            cls._raise_validation_errror_message_oapg(
+                value=arg,
+                constraint_msg="must be a value less than",
+                constraint_value=cls.MetaOapg.exclusive_maximum,
+                path_to_item=validation_metadata.path_to_item
+            )
+
+        if (cls._is_json_validation_enabled_oapg('maximum', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'inclusive_maximum') and
+                arg > cls.MetaOapg.inclusive_maximum):
+            cls._raise_validation_errror_message_oapg(
+                value=arg,
+                constraint_msg="must be a value less than or equal to",
+                constraint_value=cls.MetaOapg.inclusive_maximum,
+                path_to_item=validation_metadata.path_to_item
+            )
+
+        if (cls._is_json_validation_enabled_oapg('exclusiveMinimum', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'exclusive_minimum') and
+                arg <= cls.MetaOapg.exclusive_minimum):
+            cls._raise_validation_errror_message_oapg(
+                value=arg,
+                constraint_msg="must be a value greater than",
+                constraint_value=cls.MetaOapg.exclusive_maximum,
+                path_to_item=validation_metadata.path_to_item
+            )
+
+        if (cls._is_json_validation_enabled_oapg('minimum', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'inclusive_minimum') and
+                arg < cls.MetaOapg.inclusive_minimum):
+            cls._raise_validation_errror_message_oapg(
+                value=arg,
+                constraint_msg="must be a value greater than or equal to",
+                constraint_value=cls.MetaOapg.inclusive_minimum,
+                path_to_item=validation_metadata.path_to_item
             )
-        )
 
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ) -> typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Union['Schema', str, decimal.Decimal, BoolClass, NoneClass, frozendict.frozendict, tuple]]]:
+        """
+        NumberBase _validate_oapg
+        Validates that validations pass
+        """
+        if isinstance(arg, decimal.Decimal):
+            cls.__check_numeric_validations(arg, validation_metadata)
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
 
-def is_json_validation_enabled(schema_keyword, configuration=None):
-    """Returns true if JSON schema validation is enabled for the specified
-    validation keyword. This can be used to skip JSON schema structural validation
-    as requested in the configuration.
 
-    Args:
-        schema_keyword (string): the name of a JSON schema validation keyword.
-        configuration (Configuration): the configuration class.
-    """
+class ListBase(ValidatorBase):
+    MetaOapg: MetaOapgTyped
 
-    return (configuration is None or
-            not hasattr(configuration, '_disabled_client_side_validations') or
-            schema_keyword not in configuration._disabled_client_side_validations)
+    @classmethod
+    def __validate_items(cls, list_items, validation_metadata: ValidationMetadata):
+        """
+        Ensures that:
+        - values passed in for items are valid
+        Exceptions will be raised if:
+        - invalid arguments were passed in
 
+        Args:
+            list_items: the input list of items
 
-def check_validations(
-        validations, input_variable_path, input_values,
-        configuration=None):
-    """Raises an exception if the input_values are invalid
+        Raises:
+            ApiTypeError - for missing required arguments, or for invalid properties
+        """
 
-    Args:
-        validations (dict): the validation dictionary.
-        input_variable_path (tuple): the path to the input variable.
-        input_values (list/str/int/float/date/datetime): the values that we
-            are checking.
-        configuration (Configuration): the configuration class.
-    """
-
-    if input_values is None:
-        return
-
-    current_validations = validations[input_variable_path]
-    if (is_json_validation_enabled('multipleOf', configuration) and
-            'multiple_of' in current_validations and
-            isinstance(input_values, (int, float)) and
-            not (float(input_values) / current_validations['multiple_of']).is_integer()):
-        # Note 'multipleOf' will be as good as the floating point arithmetic.
-        raise ApiValueError(
-            "Invalid value for `%s`, value must be a multiple of "
-            "`%s`" % (
-                input_variable_path[0],
-                current_validations['multiple_of']
+        # if we have definitions for an items schema, use it
+        # otherwise accept anything
+        item_cls = getattr(cls.MetaOapg, 'items', UnsetAnyTypeSchema)
+        item_cls = cls._get_class_oapg(item_cls)
+        path_to_schemas = {}
+        for i, value in enumerate(list_items):
+            item_validation_metadata = ValidationMetadata(
+                from_server=validation_metadata.from_server,
+                configuration=validation_metadata.configuration,
+                path_to_item=validation_metadata.path_to_item+(i,),
+                validated_path_to_schemas=validation_metadata.validated_path_to_schemas
             )
+            if item_validation_metadata.validation_ran_earlier(item_cls):
+                continue
+            other_path_to_schemas = item_cls._validate_oapg(
+                value, validation_metadata=item_validation_metadata)
+            update(path_to_schemas, other_path_to_schemas)
+        return path_to_schemas
+
+    @classmethod
+    def __check_tuple_validations(
+            cls, arg,
+            validation_metadata: ValidationMetadata):
+        if not hasattr(cls, 'MetaOapg'):
+            return
+        if (cls._is_json_validation_enabled_oapg('maxItems', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'max_items') and
+                len(arg) > cls.MetaOapg.max_items):
+            cls._raise_validation_errror_message_oapg(
+                value=arg,
+                constraint_msg="number of items must be less than or equal to",
+                constraint_value=cls.MetaOapg.max_items,
+                path_to_item=validation_metadata.path_to_item
+            )
+
+        if (cls._is_json_validation_enabled_oapg('minItems', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'min_items') and
+                len(arg) < cls.MetaOapg.min_items):
+            cls._raise_validation_errror_message_oapg(
+                value=arg,
+                constraint_msg="number of items must be greater than or equal to",
+                constraint_value=cls.MetaOapg.min_items,
+                path_to_item=validation_metadata.path_to_item
+            )
+
+        if (cls._is_json_validation_enabled_oapg('uniqueItems', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'unique_items') and cls.MetaOapg.unique_items and arg):
+            unique_items = set(arg)
+            if len(arg) > len(unique_items):
+                cls._raise_validation_errror_message_oapg(
+                    value=arg,
+                    constraint_msg="duplicate items were found, and the tuple must not contain duplicates because",
+                    constraint_value='unique_items==True',
+                    path_to_item=validation_metadata.path_to_item
+                )
+
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ):
+        """
+        ListBase _validate_oapg
+        We return dynamic classes of different bases depending upon the inputs
+        This makes it so:
+        - the returned instance is always a subclass of our defining schema
+            - this allows us to check type based on whether an instance is a subclass of a schema
+        - the returned instance is a serializable type (except for None, True, and False) which are enums
+
+        Returns:
+            new_cls (type): the new class
+
+        Raises:
+            ApiValueError: when a string can't be converted into a date or datetime and it must be one of those classes
+            ApiTypeError: when the input type is not in the list of allowed spec types
+        """
+        if isinstance(arg, tuple):
+            cls.__check_tuple_validations(arg, validation_metadata)
+        _path_to_schemas = super()._validate_oapg(arg, validation_metadata=validation_metadata)
+        if not isinstance(arg, tuple):
+            return _path_to_schemas
+        updated_vm = ValidationMetadata(
+            configuration=validation_metadata.configuration,
+            from_server=validation_metadata.from_server,
+            path_to_item=validation_metadata.path_to_item,
+            seen_classes=validation_metadata.seen_classes | frozenset({cls}),
+            validated_path_to_schemas=validation_metadata.validated_path_to_schemas
         )
+        other_path_to_schemas = cls.__validate_items(arg, validation_metadata=updated_vm)
+        update(_path_to_schemas, other_path_to_schemas)
+        return _path_to_schemas
 
-    if (is_json_validation_enabled('maxLength', configuration) and
-            'max_length' in current_validations and
-            len(input_values) > current_validations['max_length']):
-        raise ApiValueError(
-            "Invalid value for `%s`, length must be less than or equal to "
-            "`%s`" % (
-                input_variable_path[0],
-                current_validations['max_length']
+    @classmethod
+    def _get_items_oapg(
+        cls: 'Schema',
+        arg: typing.List[typing.Any],
+        path_to_item: typing.Tuple[typing.Union[str, int], ...],
+        path_to_schemas: typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Type['Schema']]
+    ):
+        '''
+        ListBase _get_items_oapg
+        '''
+        cast_items = []
+
+        for i, value in enumerate(arg):
+            item_path_to_item = path_to_item + (i,)
+            item_cls = path_to_schemas[item_path_to_item]
+            new_value = item_cls._get_new_instance_without_conversion_oapg(
+                value,
+                item_path_to_item,
+                path_to_schemas
             )
-        )
+            cast_items.append(new_value)
 
-    if (is_json_validation_enabled('minLength', configuration) and
-            'min_length' in current_validations and
-            len(input_values) < current_validations['min_length']):
-        raise ApiValueError(
-            "Invalid value for `%s`, length must be greater than or equal to "
-            "`%s`" % (
-                input_variable_path[0],
-                current_validations['min_length']
+        return cast_items
+
+
+class Discriminable:
+    MetaOapg: MetaOapgTyped
+
+    @classmethod
+    def _ensure_discriminator_value_present_oapg(cls, disc_property_name: str, validation_metadata: ValidationMetadata, *args):
+        if not args or args and disc_property_name not in args[0]:
+            # The input data does not contain the discriminator property
+            raise ApiValueError(
+                "Cannot deserialize input data due to missing discriminator. "
+                "The discriminator property '{}' is missing at path: {}".format(disc_property_name, validation_metadata.path_to_item)
             )
-        )
 
-    if (is_json_validation_enabled('maxItems', configuration) and
-            'max_items' in current_validations and
-            len(input_values) > current_validations['max_items']):
-        raise ApiValueError(
-            "Invalid value for `%s`, number of items must be less than or "
-            "equal to `%s`" % (
-                input_variable_path[0],
-                current_validations['max_items']
+    @classmethod
+    def get_discriminated_class_oapg(cls, disc_property_name: str, disc_payload_value: str):
+        """
+        Used in schemas with discriminators
+        """
+        if not hasattr(cls.MetaOapg, 'discriminator'):
+            return None
+        disc = cls.MetaOapg.discriminator()
+        if disc_property_name not in disc:
+            return None
+        discriminated_cls = disc[disc_property_name].get(disc_payload_value)
+        if discriminated_cls is not None:
+            return discriminated_cls
+        if not hasattr(cls, 'MetaOapg'):
+            return None
+        elif not (
+            hasattr(cls.MetaOapg, 'all_of') or
+            hasattr(cls.MetaOapg, 'one_of') or
+            hasattr(cls.MetaOapg, 'any_of')
+        ):
+            return None
+        # TODO stop traveling if a cycle is hit
+        if hasattr(cls.MetaOapg, 'all_of'):
+            for allof_cls in cls.MetaOapg.all_of():
+                discriminated_cls = allof_cls.get_discriminated_class_oapg(
+                    disc_property_name=disc_property_name, disc_payload_value=disc_payload_value)
+                if discriminated_cls is not None:
+                    return discriminated_cls
+        if hasattr(cls.MetaOapg, 'one_of'):
+            for oneof_cls in cls.MetaOapg.one_of():
+                discriminated_cls = oneof_cls.get_discriminated_class_oapg(
+                    disc_property_name=disc_property_name, disc_payload_value=disc_payload_value)
+                if discriminated_cls is not None:
+                    return discriminated_cls
+        if hasattr(cls.MetaOapg, 'any_of'):
+            for anyof_cls in cls.MetaOapg.any_of():
+                discriminated_cls = anyof_cls.get_discriminated_class_oapg(
+                    disc_property_name=disc_property_name, disc_payload_value=disc_payload_value)
+                if discriminated_cls is not None:
+                    return discriminated_cls
+        return None
+
+
+class DictBase(Discriminable, ValidatorBase):
+
+    @classmethod
+    def __validate_arg_presence(cls, arg, validation_metadata: ValidationMetadata):
+        """
+        Ensures that:
+        - all required arguments are passed in
+        - the input variable names are valid
+            - present in properties or
+            - accepted because additionalProperties exists
+        Exceptions will be raised if:
+        - invalid arguments were passed in
+            - a var_name is invalid if additional_properties == NotAnyTypeSchema
+            and var_name not in properties.__annotations__
+        - required properties were not passed in
+
+        Args:
+            arg: the input dict
+
+        Raises:
+            ApiTypeError - for missing required arguments, or for invalid properties
+        """
+        seen_required_properties = set()
+        invalid_arguments = []
+        required_property_names = getattr(cls.MetaOapg, 'required', set())
+        additional_properties = getattr(cls.MetaOapg, 'additional_properties', UnsetAnyTypeSchema)
+        properties = getattr(cls.MetaOapg, 'properties', {})
+        property_annotations = getattr(properties, '__annotations__', {})
+        for property_name in arg:
+            if property_name in required_property_names:
+                seen_required_properties.add(property_name)
+            elif property_name in property_annotations:
+                continue
+            elif additional_properties is not NotAnyTypeSchema:
+                continue
+            else:
+                invalid_arguments.append(property_name)
+        missing_required_arguments = list(required_property_names - seen_required_properties)
+        if missing_required_arguments:
+            missing_required_arguments.sort()
+            raise MissingRequiredPropertiesError(
+                "{} is missing {} required propert{}{}: {}".format(
+                    cls.__name__,
+                    len(missing_required_arguments),
+                    "ies" if len(missing_required_arguments) > 1 else "y",
+                    " at '{}'".format('.'.join([str(i) for i in validation_metadata.path_to_item[1:]])) if len(validation_metadata.path_to_item) > 1 else "",
+                    missing_required_arguments
+                )
             )
-        )
+        if invalid_arguments:
+            invalid_arguments.sort()
+            raise ApiTypeError(
+                "{} was passed {} invalid argument{}: {}".format(
+                    cls.__name__,
+                    len(invalid_arguments),
+                    "s" if len(invalid_arguments) > 1 else "",
+                    invalid_arguments
+                )
+            )
+
+    @classmethod
+    def __validate_args(cls, arg, validation_metadata: ValidationMetadata):
+        """
+        Ensures that:
+        - values passed in for properties are valid
+        Exceptions will be raised if:
+        - invalid arguments were passed in
 
-    if (is_json_validation_enabled('minItems', configuration) and
-            'min_items' in current_validations and
-            len(input_values) < current_validations['min_items']):
-        raise ValueError(
-            "Invalid value for `%s`, number of items must be greater than or "
-            "equal to `%s`" % (
-                input_variable_path[0],
-                current_validations['min_items']
+        Args:
+            arg: the input dict
+
+        Raises:
+            ApiTypeError - for missing required arguments, or for invalid properties
+        """
+        path_to_schemas = {}
+        additional_properties = getattr(cls.MetaOapg, 'additional_properties', UnsetAnyTypeSchema)
+        properties = getattr(cls.MetaOapg, 'properties', {})
+        property_annotations = getattr(properties, '__annotations__', {})
+        validation_errors = []
+        for property_name, value in arg.items():
+            path_to_item = validation_metadata.path_to_item+(property_name,)
+            if property_name in property_annotations:
+                schema = property_annotations[property_name]
+            elif additional_properties is not NotAnyTypeSchema:
+                if additional_properties is UnsetAnyTypeSchema:
+                    """
+                    If additionalProperties is unset and this path_to_item does not yet have
+                    any validations on it, validate it.
+                    If it already has validations on it, skip this validation.
+                    """
+                    if path_to_item in path_to_schemas:
+                        continue
+                schema = additional_properties
+            else:
+                raise ApiTypeError('Unable to find schema for value={} in class={} at path_to_item={}'.format(
+                    value, cls, validation_metadata.path_to_item+(property_name,)
+                ))
+            schema = cls._get_class_oapg(schema)
+            arg_validation_metadata = ValidationMetadata(
+                from_server=validation_metadata.from_server,
+                configuration=validation_metadata.configuration,
+                path_to_item=path_to_item,
+                validated_path_to_schemas=validation_metadata.validated_path_to_schemas
             )
-        )
+            if arg_validation_metadata.validation_ran_earlier(schema):
+                continue
+            try:
+                other_path_to_schemas = schema._validate_oapg(value, validation_metadata=arg_validation_metadata)
+                update(path_to_schemas, other_path_to_schemas)
+            except (ApiTypeError, ApiValueError, MissingRequiredPropertiesError) as e:
+                validation_errors.append(e)
+        if len(validation_errors) > 0:
+            raise SchemaValidationError(validation_errors)
+        return path_to_schemas
 
-    items = ('exclusive_maximum', 'inclusive_maximum', 'exclusive_minimum',
-             'inclusive_minimum')
-    if (any(item in current_validations for item in items)):
-        if isinstance(input_values, list):
-            max_val = max(input_values)
-            min_val = min(input_values)
-        elif isinstance(input_values, dict):
-            max_val = max(input_values.values())
-            min_val = min(input_values.values())
-        else:
-            max_val = input_values
-            min_val = input_values
+    @classmethod
+    def __check_dict_validations(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata
+    ):
+        if not hasattr(cls, 'MetaOapg'):
+            return
+        if (cls._is_json_validation_enabled_oapg('maxProperties', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'max_properties') and
+                len(arg) > cls.MetaOapg.max_properties):
+            cls._raise_validation_errror_message_oapg(
+                value=arg,
+                constraint_msg="number of properties must be less than or equal to",
+                constraint_value=cls.MetaOapg.max_properties,
+                path_to_item=validation_metadata.path_to_item
+            )
+
+        if (cls._is_json_validation_enabled_oapg('minProperties', validation_metadata.configuration) and
+                hasattr(cls.MetaOapg, 'min_properties') and
+                len(arg) < cls.MetaOapg.min_properties):
+            cls._raise_validation_errror_message_oapg(
+                value=arg,
+                constraint_msg="number of properties must be greater than or equal to",
+                constraint_value=cls.MetaOapg.min_properties,
+                path_to_item=validation_metadata.path_to_item
+            )
 
-    if (is_json_validation_enabled('exclusiveMaximum', configuration) and
-            'exclusive_maximum' in current_validations and
-            max_val >= current_validations['exclusive_maximum']):
-        raise ApiValueError(
-            "Invalid value for `%s`, must be a value less than `%s`" % (
-                input_variable_path[0],
-                current_validations['exclusive_maximum']
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ):
+        """
+        DictBase _validate_oapg
+        We return dynamic classes of different bases depending upon the inputs
+        This makes it so:
+        - the returned instance is always a subclass of our defining schema
+            - this allows us to check type based on whether an instance is a subclass of a schema
+        - the returned instance is a serializable type (except for None, True, and False) which are enums
+
+        Returns:
+            new_cls (type): the new class
+
+        Raises:
+            ApiValueError: when a string can't be converted into a date or datetime and it must be one of those classes
+            ApiTypeError: when the input type is not in the list of allowed spec types
+        """
+        if isinstance(arg, frozendict.frozendict):
+            cls.__check_dict_validations(arg, validation_metadata)
+        _path_to_schemas = super()._validate_oapg(arg, validation_metadata=validation_metadata)
+        if not isinstance(arg, frozendict.frozendict):
+            return _path_to_schemas
+        cls.__validate_arg_presence(arg, validation_metadata)
+        other_path_to_schemas = cls.__validate_args(arg, validation_metadata=validation_metadata)
+        update(_path_to_schemas, other_path_to_schemas)
+        try:
+            discriminator = cls.MetaOapg.discriminator()
+        except AttributeError:
+            return _path_to_schemas
+        # discriminator exists
+        disc_prop_name = list(discriminator.keys())[0]
+        cls._ensure_discriminator_value_present_oapg(disc_prop_name, validation_metadata, arg)
+        discriminated_cls = cls.get_discriminated_class_oapg(
+            disc_property_name=disc_prop_name, disc_payload_value=arg[disc_prop_name])
+        if discriminated_cls is None:
+            raise ApiValueError(
+                "Invalid discriminator value was passed in to {}.{} Only the values {} are allowed at {}".format(
+                    cls.__name__,
+                    disc_prop_name,
+                    list(discriminator[disc_prop_name].keys()),
+                    validation_metadata.path_to_item + (disc_prop_name,)
+                )
             )
+        updated_vm = ValidationMetadata(
+            configuration=validation_metadata.configuration,
+            from_server=validation_metadata.from_server,
+            path_to_item=validation_metadata.path_to_item,
+            seen_classes=validation_metadata.seen_classes | frozenset({cls}),
+            validated_path_to_schemas=validation_metadata.validated_path_to_schemas
         )
+        if updated_vm.validation_ran_earlier(discriminated_cls):
+            return _path_to_schemas
+        other_path_to_schemas = discriminated_cls._validate_oapg(arg, validation_metadata=updated_vm)
+        update(_path_to_schemas, other_path_to_schemas)
+        return _path_to_schemas
 
-    if (is_json_validation_enabled('maximum', configuration) and
-            'inclusive_maximum' in current_validations and
-            max_val > current_validations['inclusive_maximum']):
-        raise ApiValueError(
-            "Invalid value for `%s`, must be a value less than or equal to "
-            "`%s`" % (
-                input_variable_path[0],
-                current_validations['inclusive_maximum']
+    @classmethod
+    def _get_properties_oapg(
+        cls,
+        arg: typing.Dict[str, typing.Any],
+        path_to_item: typing.Tuple[typing.Union[str, int], ...],
+        path_to_schemas: typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Type['Schema']]
+    ):
+        """
+        DictBase _get_properties_oapg, this is how properties are set
+        These values already passed validation
+        """
+        dict_items = {}
+
+        for property_name_js, value in arg.items():
+            property_path_to_item = path_to_item + (property_name_js,)
+            property_cls = path_to_schemas[property_path_to_item]
+            new_value = property_cls._get_new_instance_without_conversion_oapg(
+                value,
+                property_path_to_item,
+                path_to_schemas
             )
-        )
+            dict_items[property_name_js] = new_value
 
-    if (is_json_validation_enabled('exclusiveMinimum', configuration) and
-            'exclusive_minimum' in current_validations and
-            min_val <= current_validations['exclusive_minimum']):
-        raise ApiValueError(
-            "Invalid value for `%s`, must be a value greater than `%s`" %
-            (
-                input_variable_path[0],
-                current_validations['exclusive_maximum']
+        return dict_items
+
+    def __setattr__(self, name: str, value: typing.Any):
+        if not isinstance(self, FileIO):
+            raise AttributeError('property setting not supported on immutable instances')
+
+    def __getattr__(self, name: str):
+        """
+        for instance.name access
+        Properties are only type hinted for required properties
+        so that hasattr(instance, 'optionalProp') is False when that key is not present
+        """
+        if not isinstance(self, frozendict.frozendict):
+            return super().__getattr__(name)
+        if name not in self.__class__.__annotations__:
+            raise AttributeError(f"{self} has no attribute '{name}'")
+        try:
+            value = self[name]
+            return value
+        except KeyError as ex:
+            raise AttributeError(str(ex))
+
+    def __getitem__(self, name: str):
+        """
+        dict_instance[name] accessor
+        key errors thrown
+        """
+        if not isinstance(self, frozendict.frozendict):
+            return super().__getattr__(name)
+        return super().__getitem__(name)
+
+    def get_item_oapg(self, name: str) -> typing.Union['AnyTypeSchema', Unset]:
+        # dict_instance[name] accessor
+        if not isinstance(self, frozendict.frozendict):
+            raise NotImplementedError()
+        try:
+            return super().__getitem__(name)
+        except KeyError:
+            return unset
+
+
+def cast_to_allowed_types(
+    arg: typing.Union[str, date, datetime, uuid.UUID, decimal.Decimal, int, float, None, dict, frozendict.frozendict, list, tuple, bytes, Schema, io.FileIO, io.BufferedReader],
+    from_server: bool,
+    validated_path_to_schemas: typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Union['Schema', str, decimal.Decimal, BoolClass, NoneClass, frozendict.frozendict, tuple]]],
+    path_to_item: typing.Tuple[typing.Union[str, int], ...] = tuple(['args[0]']),
+    schema: Schema = None,
+) -> typing.Union[frozendict.frozendict, tuple, decimal.Decimal, str, bytes, BoolClass, NoneClass, FileIO]:
+    """
+    Casts the input payload arg into the allowed types
+    The input validated_path_to_schemas is mutated by running this function
+
+    When from_server is False then
+    - date/datetime is cast to str
+    - int/float is cast to Decimal
+
+    If a Schema instance is passed in it is converted back to a primitive instance because
+    One may need to validate that data to the original Schema class AND additional different classes
+    those additional classes will need to be added to the new manufactured class for that payload
+    If the code didn't do this and kept the payload as a Schema instance it would fail to validate to other
+    Schema classes and the code wouldn't be able to mfg a new class that includes all valid schemas
+    TODO: store the validated schema classes in validation_metadata
+
+    Args:
+        arg: the payload
+        from_server: whether this payload came from the server or not
+        validated_path_to_schemas: a dict that stores the validated classes at any path location in the payload
+    """
+    if isinstance(arg, Schema):
+        # store the already run validations
+        schema_classes = set()
+        source_schema_was_unset = len(arg.__class__.__bases__) == 2 and UnsetAnyTypeSchema in arg.__class__.__bases__
+        if not source_schema_was_unset:
+            """
+            Do not include UnsetAnyTypeSchema and its base class because
+            it did not exist in the original spec schema definition
+            It was added to ensure that all instances are of type Schema and the allowed base types
+            """
+            for cls in arg.__class__.__bases__:
+                if cls is Singleton:
+                    # Skip Singleton
+                    continue
+                schema_classes.add(cls)
+        validated_path_to_schemas[path_to_item] = schema_classes
+
+    type_error = ApiTypeError(f"Invalid type. Required value type is str and passed type was {type(arg)} at {path_to_item}")
+    if isinstance(arg, str):
+        return str(arg)
+    elif isinstance(arg, (dict, frozendict.frozendict)):
+        return frozendict.frozendict({key: cast_to_allowed_types(val, from_server, validated_path_to_schemas, path_to_item + (key,)) for key, val in arg.items()})
+    elif isinstance(arg, (bool, BoolClass)):
+        """
+        this check must come before isinstance(arg, (int, float))
+        because isinstance(True, int) is True
+        """
+        if arg:
+            return BoolClass.TRUE
+        return BoolClass.FALSE
+    elif isinstance(arg, int):
+        return arg
+    elif isinstance(arg, float):
+        decimal_from_float = decimal.Decimal(arg)
+        if decimal_from_float.as_integer_ratio()[1] == 1:
+            # 9.0 -> Decimal('9.0')
+            # 3.4028234663852886e+38 -> Decimal('340282346638528859811704183484516925440.0')
+            return decimal.Decimal(str(decimal_from_float)+'.0')
+        return decimal_from_float
+    elif isinstance(arg, (tuple, list)):
+        return tuple([cast_to_allowed_types(item, from_server, validated_path_to_schemas, path_to_item + (i,)) for i, item in enumerate(arg)])
+    elif isinstance(arg, (none_type, NoneClass)):
+        return NoneClass.NONE
+    elif isinstance(arg, (date, datetime)):
+        if not from_server:
+            # if schema itself is the DateTimeSchema class then convert to isoformat
+            # if schema itself is the DateSchema class then convert to yyyy-mm-dd using strftime
+            if schema is None:
+                return arg.isoformat()
+            if schema is DateTimeSchema:
+                return arg.isoformat()
+            if schema is DateSchema:
+                return arg.strftime('%Y-%m-%d')
+        raise type_error
+    elif isinstance(arg, uuid.UUID):
+        if not from_server:
+            return str(arg)
+        raise type_error
+    elif isinstance(arg, decimal.Decimal):
+        return decimal.Decimal(arg)
+    elif isinstance(arg, bytes):
+        return bytes(arg)
+    elif isinstance(arg, (io.FileIO, io.BufferedReader)):
+        return FileIO(arg)
+    raise ValueError('Invalid type passed in got input={} type={}'.format(arg, type(arg)))
+
+
+class ComposedBase(Discriminable):
+
+    @classmethod
+    def __get_allof_classes(cls, arg, validation_metadata: ValidationMetadata):
+        path_to_schemas = defaultdict(set)
+        for allof_cls in cls.MetaOapg.all_of():
+            if validation_metadata.validation_ran_earlier(allof_cls):
+                continue
+            other_path_to_schemas = allof_cls._validate_oapg(arg, validation_metadata=validation_metadata)
+            update(path_to_schemas, other_path_to_schemas)
+        return path_to_schemas
+
+    @classmethod
+    def __get_oneof_class(
+        cls,
+        arg,
+        discriminated_cls,
+        validation_metadata: ValidationMetadata,
+    ):
+        oneof_classes = []
+        path_to_schemas = defaultdict(set)
+        for oneof_cls in cls.MetaOapg.one_of():
+            if oneof_cls in path_to_schemas[validation_metadata.path_to_item]:
+                oneof_classes.append(oneof_cls)
+                continue
+            if validation_metadata.validation_ran_earlier(oneof_cls):
+                oneof_classes.append(oneof_cls)
+                continue
+            try:
+                path_to_schemas = oneof_cls._validate_oapg(arg, validation_metadata=validation_metadata)
+            except (ApiValueError, ApiTypeError) as ex:
+                if discriminated_cls is not None and oneof_cls is discriminated_cls:
+                    raise ex
+                continue
+            oneof_classes.append(oneof_cls)
+        if not oneof_classes:
+            raise ApiValueError(
+                "Invalid inputs given to generate an instance of {}. None "
+                "of the oneOf schemas matched the input data.".format(cls)
             )
+        elif len(oneof_classes) > 1:
+            raise ApiValueError(
+                "Invalid inputs given to generate an instance of {}. Multiple "
+                "oneOf schemas {} matched the inputs, but a max of one is allowed.".format(cls, oneof_classes)
+            )
+        # exactly one class matches
+        return path_to_schemas
+
+    @classmethod
+    def __get_anyof_classes(
+        cls,
+        arg,
+        discriminated_cls,
+        validation_metadata: ValidationMetadata
+    ):
+        anyof_classes = []
+        exceptions: typing.List[typing.Union[ApiTypeError, ApiValueError]] = []
+        path_to_schemas = defaultdict(set)
+        for anyof_cls in cls.MetaOapg.any_of():
+            if validation_metadata.validation_ran_earlier(anyof_cls):
+                anyof_classes.append(anyof_cls)
+                continue
+
+            try:
+                other_path_to_schemas = anyof_cls._validate_oapg(arg, validation_metadata=validation_metadata)
+            except (ApiValueError, ApiTypeError) as ex:
+                if discriminated_cls is not None and anyof_cls is discriminated_cls:
+                    raise ex
+                exceptions.append(ex)
+                continue
+            anyof_classes.append(anyof_cls)
+            update(path_to_schemas, other_path_to_schemas)
+        if not anyof_classes:
+            raise AnyOfValidationError(error_list=exceptions)
+        return path_to_schemas
+
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ) -> typing.Dict[typing.Tuple[typing.Union[str, int], ...], typing.Set[typing.Union['Schema', str, decimal.Decimal, BoolClass, NoneClass, frozendict.frozendict, tuple]]]:
+        """
+        ComposedBase _validate_oapg
+        We return dynamic classes of different bases depending upon the inputs
+        This makes it so:
+        - the returned instance is always a subclass of our defining schema
+            - this allows us to check type based on whether an instance is a subclass of a schema
+        - the returned instance is a serializable type (except for None, True, and False) which are enums
+
+        Returns:
+            new_cls (type): the new class
+
+        Raises:
+            ApiValueError: when a string can't be converted into a date or datetime and it must be one of those classes
+            ApiTypeError: when the input type is not in the list of allowed spec types
+        """
+        # validation checking on types, validations, and enums
+        path_to_schemas = super()._validate_oapg(arg, validation_metadata=validation_metadata)
+
+        updated_vm = ValidationMetadata(
+            configuration=validation_metadata.configuration,
+            from_server=validation_metadata.from_server,
+            path_to_item=validation_metadata.path_to_item,
+            seen_classes=validation_metadata.seen_classes | frozenset({cls}),
+            validated_path_to_schemas=validation_metadata.validated_path_to_schemas
         )
 
-    if (is_json_validation_enabled('minimum', configuration) and
-            'inclusive_minimum' in current_validations and
-            min_val < current_validations['inclusive_minimum']):
-        raise ApiValueError(
-            "Invalid value for `%s`, must be a value greater than or equal "
-            "to `%s`" % (
-                input_variable_path[0],
-                current_validations['inclusive_minimum']
+        # process composed schema
+        discriminator = None
+        if hasattr(cls, 'MetaOapg') and hasattr(cls.MetaOapg, 'discriminator'):
+            discriminator = cls.MetaOapg.discriminator()
+        discriminated_cls = None
+        if discriminator and arg and isinstance(arg, frozendict.frozendict):
+            disc_property_name = list(discriminator.keys())[0]
+            cls._ensure_discriminator_value_present_oapg(disc_property_name, updated_vm, arg)
+            # get discriminated_cls by looking at the dict in the current class
+            discriminated_cls = cls.get_discriminated_class_oapg(
+                disc_property_name=disc_property_name, disc_payload_value=arg[disc_property_name])
+            if discriminated_cls is None:
+                raise ApiValueError(
+                    "Invalid discriminator value '{}' was passed in to {}.{} Only the values {} are allowed at {}".format(
+                        arg[disc_property_name],
+                        cls.__name__,
+                        disc_property_name,
+                        list(discriminator[disc_property_name].keys()),
+                        updated_vm.path_to_item + (disc_property_name,)
+                    )
+                )
+
+        if hasattr(cls, 'MetaOapg') and hasattr(cls.MetaOapg, 'all_of'):
+            other_path_to_schemas = cls.__get_allof_classes(arg, validation_metadata=updated_vm)
+            update(path_to_schemas, other_path_to_schemas)
+        if hasattr(cls, 'MetaOapg') and hasattr(cls.MetaOapg, 'one_of'):
+            other_path_to_schemas = cls.__get_oneof_class(
+                arg,
+                discriminated_cls=discriminated_cls,
+                validation_metadata=updated_vm
+            )
+            update(path_to_schemas, other_path_to_schemas)
+        if hasattr(cls, 'MetaOapg') and hasattr(cls.MetaOapg, 'any_of'):
+            other_path_to_schemas = cls.__get_anyof_classes(
+                arg,
+                discriminated_cls=discriminated_cls,
+                validation_metadata=updated_vm
+            )
+            update(path_to_schemas, other_path_to_schemas)
+        not_cls = None
+        if hasattr(cls, 'MetaOapg') and hasattr(cls.MetaOapg, 'not_schema'):
+            not_cls = cls.MetaOapg.not_schema
+            not_cls = cls._get_class_oapg(not_cls)
+        if not_cls:
+            other_path_to_schemas = None
+            not_exception = ApiValueError(
+                "Invalid value '{}' was passed in to {}. Value is invalid because it is disallowed by {}".format(
+                    arg,
+                    cls.__name__,
+                    not_cls.__name__,
+                )
             )
-        )
-    flags = current_validations.get('regex', {}).get('flags', 0)
-    if (is_json_validation_enabled('pattern', configuration) and
-            'regex' in current_validations and
-            not re.search(current_validations['regex']['pattern'],
-                          input_values, flags=flags)):
-        err_msg = r"Invalid value for `%s`, must match regular expression `%s`" % (
-            input_variable_path[0],
-            current_validations['regex']['pattern']
-        )
-        if flags != 0:
-            # Don't print the regex flags if the flags are not
-            # specified in the OAS document.
-            err_msg = r"%s with flags=`%s`" % (err_msg, flags)
-        raise ApiValueError(err_msg)
+            if updated_vm.validation_ran_earlier(not_cls):
+                raise not_exception
+
+            try:
+                other_path_to_schemas = not_cls._validate_oapg(arg, validation_metadata=updated_vm)
+            except (ApiValueError, ApiTypeError):
+                pass
+            if other_path_to_schemas:
+                raise not_exception
 
+        if discriminated_cls is not None and not updated_vm.validation_ran_earlier(discriminated_cls):
+            if discriminated_cls not in path_to_schemas[updated_vm.path_to_item]:
+                raise ApiValueError("Could not find discriminator in value")
+        return path_to_schemas
+
+
+# DictBase, ListBase, NumberBase, StrBase, BoolBase, NoneBase
+class ComposedSchema(
+    ComposedBase,
+    DictBase,
+    ListBase,
+    NumberBase,
+    StrBase,
+    BoolBase,
+    NoneBase,
+    Schema,
+    NoneFrozenDictTupleStrDecimalBoolMixin
+):
+    @classmethod
+    def from_openapi_data_oapg(cls, *args: typing.Any, _configuration: typing.Optional[Configuration] = None, **kwargs):
+        if not args:
+            if not kwargs:
+                raise ApiTypeError('{} is missing required input data in args or kwargs'.format(cls.__name__))
+            args = (kwargs, )
+        return super().from_openapi_data_oapg(args[0], _configuration=_configuration)
 
-def order_response_types(required_types):
-    """Returns the required types sorted in coercion order
 
-    Args:
-        required_types (list/tuple): collection of classes or instance of
-            list or dict with class information inside it.
+class ListSchema(
+    ListBase,
+    Schema,
+    TupleMixin
+):
 
-    Returns:
-        (list): coercion order sorted collection of classes or instance
-            of list or dict with class information inside it.
-    """
-
-    def index_getter(class_or_instance):
-        if isinstance(class_or_instance, list):
-            return COERCION_INDEX_BY_TYPE[list]
-        elif isinstance(class_or_instance, dict):
-            return COERCION_INDEX_BY_TYPE[dict]
-        elif (inspect.isclass(class_or_instance)
-                and issubclass(class_or_instance, ModelComposed)):
-            return COERCION_INDEX_BY_TYPE[ModelComposed]
-        elif (inspect.isclass(class_or_instance)
-                and issubclass(class_or_instance, ModelNormal)):
-            return COERCION_INDEX_BY_TYPE[ModelNormal]
-        elif (inspect.isclass(class_or_instance)
-                and issubclass(class_or_instance, ModelSimple)):
-            return COERCION_INDEX_BY_TYPE[ModelSimple]
-        elif class_or_instance in COERCION_INDEX_BY_TYPE:
-            return COERCION_INDEX_BY_TYPE[class_or_instance]
-        raise ApiValueError("Unsupported type: %s" % class_or_instance)
-
-    sorted_types = sorted(
-        required_types,
-        key=lambda class_or_instance: index_getter(class_or_instance)
-    )
-    return sorted_types
-
-
-def remove_uncoercible(required_types_classes, current_item, spec_property_naming,
-                       must_convert=True):
-    """Only keeps the type conversions that are possible
+    @classmethod
+    def from_openapi_data_oapg(cls, arg: typing.List[typing.Any], _configuration: typing.Optional[Configuration] = None):
+        return super().from_openapi_data_oapg(arg, _configuration=_configuration)
 
-    Args:
-        required_types_classes (tuple): tuple of classes that are required
-                          these should be ordered by COERCION_INDEX_BY_TYPE
-        spec_property_naming (bool): True if the variable names in the input
-            data are serialized names as specified in the OpenAPI document.
-            False if the variables names in the input data are python
-            variable names in PEP-8 snake case.
-        current_item (any): the current item (input data) to be converted
-
-    Keyword Args:
-        must_convert (bool): if True the item to convert is of the wrong
-                          type and we want a big list of coercibles
-                          if False, we want a limited list of coercibles
-
-    Returns:
-        (list): the remaining coercible required types, classes only
-    """
-    current_type_simple = get_simple_class(current_item)
-
-    results_classes = []
-    for required_type_class in required_types_classes:
-        # convert our models to OpenApiModel
-        required_type_class_simplified = required_type_class
-        if isinstance(required_type_class_simplified, type):
-            if issubclass(required_type_class_simplified, ModelComposed):
-                required_type_class_simplified = ModelComposed
-            elif issubclass(required_type_class_simplified, ModelNormal):
-                required_type_class_simplified = ModelNormal
-            elif issubclass(required_type_class_simplified, ModelSimple):
-                required_type_class_simplified = ModelSimple
-
-        if required_type_class_simplified == current_type_simple:
-            # don't consider converting to one's own class
-            continue
-
-        class_pair = (current_type_simple, required_type_class_simplified)
-        if must_convert and class_pair in COERCIBLE_TYPE_PAIRS[spec_property_naming]:
-            results_classes.append(required_type_class)
-        elif class_pair in UPCONVERSION_TYPE_PAIRS:
-            results_classes.append(required_type_class)
-    return results_classes
-
-
-def get_discriminated_classes(cls):
-    """
-    Returns all the classes that a discriminator converts to
-    TODO: lru_cache this
-    """
-    possible_classes = []
-    key = list(cls.discriminator.keys())[0]
-    if is_type_nullable(cls):
-        possible_classes.append(cls)
-    for discr_cls in cls.discriminator[key].values():
-        if hasattr(discr_cls, 'discriminator') and discr_cls.discriminator is not None:
-            possible_classes.extend(get_discriminated_classes(discr_cls))
-        else:
-            possible_classes.append(discr_cls)
-    return possible_classes
+    def __new__(cls, arg: typing.Union[typing.List[typing.Any], typing.Tuple[typing.Any]], **kwargs: Configuration):
+        return super().__new__(cls, arg, **kwargs)
 
 
-def get_possible_classes(cls, from_server_context):
-    # TODO: lru_cache this
-    possible_classes = [cls]
-    if from_server_context:
-        return possible_classes
-    if hasattr(cls, 'discriminator') and cls.discriminator is not None:
-        possible_classes = []
-        possible_classes.extend(get_discriminated_classes(cls))
-    elif issubclass(cls, ModelComposed):
-        possible_classes.extend(composed_model_input_classes(cls))
-    return possible_classes
-
-
-def get_required_type_classes(required_types_mixed, spec_property_naming):
-    """Converts the tuple required_types into a tuple and a dict described
-    below
+class NoneSchema(
+    NoneBase,
+    Schema,
+    NoneMixin
+):
 
-    Args:
-        required_types_mixed (tuple/list): will contain either classes or
-            instance of list or dict
-        spec_property_naming (bool): if True these values came from the
-            server, and we use the data types in our endpoints.
-            If False, we are client side and we need to include
-            oneOf and discriminator classes inside the data types in our endpoints
-
-    Returns:
-        (valid_classes, dict_valid_class_to_child_types_mixed):
-            valid_classes (tuple): the valid classes that the current item
-                                   should be
-            dict_valid_class_to_child_types_mixed (dict):
-                valid_class (class): this is the key
-                child_types_mixed (list/dict/tuple): describes the valid child
-                    types
-    """
-    valid_classes = []
-    child_req_types_by_current_type = {}
-    for required_type in required_types_mixed:
-        if isinstance(required_type, list):
-            valid_classes.append(list)
-            child_req_types_by_current_type[list] = required_type
-        elif isinstance(required_type, tuple):
-            valid_classes.append(tuple)
-            child_req_types_by_current_type[tuple] = required_type
-        elif isinstance(required_type, dict):
-            valid_classes.append(dict)
-            child_req_types_by_current_type[dict] = required_type[str]
-        else:
-            valid_classes.extend(get_possible_classes(required_type, spec_property_naming))
-    return tuple(valid_classes), child_req_types_by_current_type
+    @classmethod
+    def from_openapi_data_oapg(cls, arg: None, _configuration: typing.Optional[Configuration] = None):
+        return super().from_openapi_data_oapg(arg, _configuration=_configuration)
 
+    def __new__(cls, arg: None, **kwargs: Configuration):
+        return super().__new__(cls, arg, **kwargs)
 
-def change_keys_js_to_python(input_dict, model_class):
+
+class NumberSchema(
+    NumberBase,
+    Schema,
+    NumberMixin
+):
+    """
+    This is used for type: number with no format
+    Both integers AND floats are accepted
     """
-    Converts from javascript_key keys in the input_dict to python_keys in
-    the output dict using the mapping in model_class.
-    If the input_dict contains a key which does not declared in the model_class,
-    the key is added to the output dict as is. The assumption is the model_class
-    may have undeclared properties (additionalProperties attribute in the OAS
-    document).
-    """
-
-    if getattr(model_class, 'attribute_map', None) is None:
-        return input_dict
-    output_dict = {}
-    reversed_attr_map = {value: key for key, value in
-                         model_class.attribute_map.items()}
-    for javascript_key, value in input_dict.items():
-        python_key = reversed_attr_map.get(javascript_key)
-        if python_key is None:
-            # if the key is unknown, it is in error or it is an
-            # additionalProperties variable
-            python_key = javascript_key
-        output_dict[python_key] = value
-    return output_dict
-
-
-def get_type_error(var_value, path_to_item, valid_classes, key_type=False):
-    error_msg = type_error_message(
-        var_name=path_to_item[-1],
-        var_value=var_value,
-        valid_classes=valid_classes,
-        key_type=key_type
-    )
-    return ApiTypeError(
-        error_msg,
-        path_to_item=path_to_item,
-        valid_classes=valid_classes,
-        key_type=key_type
-    )
-
-
-def deserialize_primitive(data, klass, path_to_item):
-    """Deserializes string to primitive type.
-
-    :param data: str/int/float
-    :param klass: str/class the class to convert to
-
-    :return: int, float, str, bool, date, datetime
-    """
-    additional_message = ""
-    try:
-        if klass in {datetime, date}:
-            additional_message = (
-                "If you need your parameter to have a fallback "
-                "string value, please set its type as `type: {}` in your "
-                "spec. That allows the value to be any type. "
-            )
-            if klass == datetime:
-                if len(data) < 8:
-                    raise ValueError("This is not a datetime")
-                # The string should be in iso8601 datetime format.
-                parsed_datetime = parse(data)
-                date_only = (
-                    parsed_datetime.hour == 0 and
-                    parsed_datetime.minute == 0 and
-                    parsed_datetime.second == 0 and
-                    parsed_datetime.tzinfo is None and
-                    8 <= len(data) <= 10
+
+    @classmethod
+    def from_openapi_data_oapg(cls, arg: typing.Union[int, float], _configuration: typing.Optional[Configuration] = None):
+        return super().from_openapi_data_oapg(arg, _configuration=_configuration)
+
+    def __new__(cls, arg: typing.Union[decimal.Decimal, int, float], **kwargs: Configuration):
+        return super().__new__(cls, arg, **kwargs)
+
+
+class IntBase:
+    @property
+    def as_int_oapg(self) -> int:
+        try:
+            return self._as_int
+        except AttributeError:
+            self._as_int = int(self)
+            return self._as_int
+
+    @classmethod
+    def __validate_format(cls, arg: typing.Optional[decimal.Decimal], validation_metadata: ValidationMetadata):
+        if isinstance(arg, decimal.Decimal):
+
+            denominator = arg.as_integer_ratio()[-1]
+            if denominator != 1:
+                raise ApiValueError(
+                    "Invalid value '{}' for type integer at {}".format(arg, validation_metadata.path_to_item)
                 )
-                if date_only:
-                    raise ValueError("This is a date, not a datetime")
-                return parsed_datetime
-            elif klass == date:
-                if len(data) < 8:
-                    raise ValueError("This is not a date")
-                return parse(data).date()
-        else:
-            converted_value = klass(data)
-            if isinstance(data, str) and klass == float:
-                if str(converted_value) != data:
-                    # '7' -> 7.0 -> '7.0' != '7'
-                    raise ValueError('This is not a float')
-            return converted_value
-    except (OverflowError, ValueError) as ex:
-        # parse can raise OverflowError
-        raise ApiValueError(
-            "{0}Failed to parse {1} as {2}".format(
-                additional_message, repr(data), klass.__name__
-            ),
-            path_to_item=path_to_item
-        ) from ex
 
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ):
+        """
+        IntBase _validate_oapg
+        TODO what about types = (int, number) -> IntBase, NumberBase? We could drop int and keep number only
+        """
+        cls.__validate_format(arg, validation_metadata=validation_metadata)
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
 
-def get_discriminator_class(model_class,
-                            discr_name,
-                            discr_value, cls_visited):
-    """Returns the child class specified by the discriminator.
 
-    Args:
-        model_class (OpenApiModel): the model class.
-        discr_name (string): the name of the discriminator property.
-        discr_value (any): the discriminator value.
-        cls_visited (list): list of model classes that have been visited.
-            Used to determine the discriminator class without
-            visiting circular references indefinitely.
-
-    Returns:
-        used_model_class (class/None): the chosen child class that will be used
-            to deserialize the data, for example dog.Dog.
-            If a class is not found, None is returned.
-    """
+class IntSchema(IntBase, NumberBase, Schema, IntMixin):
 
-    if model_class in cls_visited:
-        # The class has already been visited and no suitable class was found.
-        return None
-    cls_visited.append(model_class)
-    used_model_class = None
-    if discr_name in model_class.discriminator:
-        class_name_to_discr_class = model_class.discriminator[discr_name]
-        used_model_class = class_name_to_discr_class.get(discr_value)
-    if used_model_class is None:
-        # We didn't find a discriminated class in class_name_to_discr_class.
-        # So look in the ancestor or descendant discriminators
-        # The discriminator mapping may exist in a descendant (anyOf, oneOf)
-        # or ancestor (allOf).
-        # Ancestor example: in the GrandparentAnimal -> ParentPet -> ChildCat
-        #   hierarchy, the discriminator mappings may be defined at any level
-        #   in the hierarchy.
-        # Descendant example:  mammal -> whale/zebra/Pig -> BasquePig/DanishPig
-        #   if we try to make BasquePig from mammal, we need to travel through
-        #   the oneOf descendant discriminators to find BasquePig
-        descendant_classes = model_class._composed_schemas.get('oneOf', ()) + \
-            model_class._composed_schemas.get('anyOf', ())
-        ancestor_classes = model_class._composed_schemas.get('allOf', ())
-        possible_classes = descendant_classes + ancestor_classes
-        for cls in possible_classes:
-            # Check if the schema has inherited discriminators.
-            if hasattr(cls, 'discriminator') and cls.discriminator is not None:
-                used_model_class = get_discriminator_class(
-                    cls, discr_name, discr_value, cls_visited)
-                if used_model_class is not None:
-                    return used_model_class
-    return used_model_class
-
-
-def deserialize_model(model_data, model_class, path_to_item, check_type,
-                      configuration, spec_property_naming):
-    """Deserializes model_data to model instance.
+    @classmethod
+    def from_openapi_data_oapg(cls, arg: int, _configuration: typing.Optional[Configuration] = None):
+        return super().from_openapi_data_oapg(arg, _configuration=_configuration)
 
-    Args:
-        model_data (int/str/float/bool/none_type/list/dict): data to instantiate the model
-        model_class (OpenApiModel): the model class
-        path_to_item (list): path to the model in the received data
-        check_type (bool): whether to check the data tupe for the values in
-            the model
-        configuration (Configuration): the instance to use to convert files
-        spec_property_naming (bool): True if the variable names in the input
-            data are serialized names as specified in the OpenAPI document.
-            False if the variables names in the input data are python
-            variable names in PEP-8 snake case.
-
-    Returns:
-        model instance
-
-    Raise:
-        ApiTypeError
-        ApiValueError
-        ApiKeyError
-    """
-
-    kw_args = dict(_check_type=check_type,
-                   _path_to_item=path_to_item,
-                   _configuration=configuration,
-                   _spec_property_naming=spec_property_naming)
-
-    if issubclass(model_class, ModelSimple):
-        return model_class._new_from_openapi_data(model_data, **kw_args)
-    elif isinstance(model_data, list):
-        return model_class._new_from_openapi_data(*model_data, **kw_args)
-    if isinstance(model_data, dict):
-        kw_args.update(model_data)
-        return model_class._new_from_openapi_data(**kw_args)
-    elif isinstance(model_data, PRIMITIVE_TYPES):
-        return model_class._new_from_openapi_data(model_data, **kw_args)
+    def __new__(cls, arg: typing.Union[decimal.Decimal, int], **kwargs: Configuration):
+        return super().__new__(cls, arg, **kwargs)
 
 
-def deserialize_file(response_data, configuration, content_disposition=None):
-    """Deserializes body to file
+class Int32Base:
+    __inclusive_minimum = decimal.Decimal(-2147483648)
+    __inclusive_maximum = decimal.Decimal(2147483647)
 
-    Saves response body into a file in a temporary folder,
-    using the filename from the `Content-Disposition` header if provided.
+    @classmethod
+    def __validate_format(cls, arg: typing.Optional[decimal.Decimal], validation_metadata: ValidationMetadata):
+        if isinstance(arg, decimal.Decimal) and arg.as_tuple().exponent == 0:
+            if not cls.__inclusive_minimum <= arg <= cls.__inclusive_maximum:
+                raise ApiValueError(
+                    "Invalid value '{}' for type int32 at {}".format(arg, validation_metadata.path_to_item)
+                )
 
-    Args:
-        param response_data (str):  the file data to write
-        configuration (Configuration): the instance to use to convert files
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ):
+        """
+        Int32Base _validate_oapg
+        """
+        cls.__validate_format(arg, validation_metadata=validation_metadata)
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
 
-    Keyword Args:
-        content_disposition (str):  the value of the Content-Disposition
-            header
-
-    Returns:
-        (file_type): the deserialized file which is open
-            The user is responsible for closing and reading the file
-    """
-    fd, path = tempfile.mkstemp(dir=configuration.temp_folder_path)
-    os.close(fd)
-    os.remove(path)
-
-    if content_disposition:
-        filename = re.search(r'filename=[\'"]?([^\'"\s]+)[\'"]?',
-                             content_disposition,
-                             flags=re.I)
-        if filename is not None:
-            filename = filename.group(1)
-        else:
-            filename = "default_" + str(uuid.uuid4())
 
-        path = os.path.join(os.path.dirname(path), filename)
+class Int32Schema(
+    Int32Base,
+    IntSchema
+):
+    pass
 
-    with open(path, "wb") as f:
-        if isinstance(response_data, str):
-            # change str to bytes so we can write it
-            response_data = response_data.encode('utf-8')
-        f.write(response_data)
 
-    f = open(path, "rb")
-    return f
+class Int64Base:
+    __inclusive_minimum = decimal.Decimal(-9223372036854775808)
+    __inclusive_maximum = decimal.Decimal(9223372036854775807)
 
+    @classmethod
+    def __validate_format(cls, arg: typing.Optional[decimal.Decimal], validation_metadata: ValidationMetadata):
+        if isinstance(arg, decimal.Decimal) and arg.as_tuple().exponent == 0:
+            if not cls.__inclusive_minimum <= arg <= cls.__inclusive_maximum:
+                raise ApiValueError(
+                    "Invalid value '{}' for type int64 at {}".format(arg, validation_metadata.path_to_item)
+                )
 
-def attempt_convert_item(input_value, valid_classes, path_to_item,
-                         configuration, spec_property_naming, key_type=False,
-                         must_convert=False, check_type=True):
-    """
-    Args:
-        input_value (any): the data to convert
-        valid_classes (any): the classes that are valid
-        path_to_item (list): the path to the item to convert
-        configuration (Configuration): the instance to use to convert files
-        spec_property_naming (bool): True if the variable names in the input
-            data are serialized names as specified in the OpenAPI document.
-            False if the variables names in the input data are python
-            variable names in PEP-8 snake case.
-        key_type (bool): if True we need to convert a key type (not supported)
-        must_convert (bool): if True we must convert
-        check_type (bool): if True we check the type or the returned data in
-            ModelComposed/ModelNormal/ModelSimple instances
-
-    Returns:
-        instance (any) the fixed item
-
-    Raises:
-        ApiTypeError
-        ApiValueError
-        ApiKeyError
-    """
-    valid_classes_ordered = order_response_types(valid_classes)
-    valid_classes_coercible = remove_uncoercible(
-        valid_classes_ordered, input_value, spec_property_naming)
-    if not valid_classes_coercible or key_type:
-        # we do not handle keytype errors, json will take care
-        # of this for us
-        if configuration is None or not configuration.discard_unknown_keys:
-            raise get_type_error(input_value, path_to_item, valid_classes,
-                                 key_type=key_type)
-    for valid_class in valid_classes_coercible:
-        try:
-            if issubclass(valid_class, OpenApiModel):
-                return deserialize_model(input_value, valid_class,
-                                         path_to_item, check_type,
-                                         configuration, spec_property_naming)
-            elif valid_class == file_type:
-                return deserialize_file(input_value, configuration)
-            return deserialize_primitive(input_value, valid_class,
-                                         path_to_item)
-        except (ApiTypeError, ApiValueError, ApiKeyError) as conversion_exc:
-            if must_convert:
-                raise conversion_exc
-            # if we have conversion errors when must_convert == False
-            # we ignore the exception and move on to the next class
-            continue
-    # we were unable to convert, must_convert == False
-    return input_value
-
-
-def is_type_nullable(input_type):
-    """
-    Returns true if None is an allowed value for the specified input_type.
-
-    A type is nullable if at least one of the following conditions is true:
-    1. The OAS 'nullable' attribute has been specified,
-    1. The type is the 'null' type,
-    1. The type is a anyOf/oneOf composed schema, and a child schema is
-       the 'null' type.
-    Args:
-        input_type (type): the class of the input_value that we are
-            checking
-    Returns:
-        bool
-    """
-    if input_type is none_type:
-        return True
-    if issubclass(input_type, OpenApiModel) and input_type._nullable:
-        return True
-    if issubclass(input_type, ModelComposed):
-        # If oneOf/anyOf, check if the 'null' type is one of the allowed types.
-        for t in input_type._composed_schemas.get('oneOf', ()):
-            if is_type_nullable(t):
-                return True
-        for t in input_type._composed_schemas.get('anyOf', ()):
-            if is_type_nullable(t):
-                return True
-    return False
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ):
+        """
+        Int64Base _validate_oapg
+        """
+        cls.__validate_format(arg, validation_metadata=validation_metadata)
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
+
+
+class Int64Schema(
+    Int64Base,
+    IntSchema
+):
+    pass
+
+
+class Float32Base:
+    __inclusive_minimum = decimal.Decimal(-3.4028234663852886e+38)
+    __inclusive_maximum = decimal.Decimal(3.4028234663852886e+38)
 
+    @classmethod
+    def __validate_format(cls, arg: typing.Optional[decimal.Decimal], validation_metadata: ValidationMetadata):
+        if isinstance(arg, decimal.Decimal):
+            if not cls.__inclusive_minimum <= arg <= cls.__inclusive_maximum:
+                raise ApiValueError(
+                    "Invalid value '{}' for type float at {}".format(arg, validation_metadata.path_to_item)
+                )
+
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ):
+        """
+        Float32Base _validate_oapg
+        """
+        cls.__validate_format(arg, validation_metadata=validation_metadata)
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
+
+
+class Float32Schema(
+    Float32Base,
+    NumberSchema
+):
+
+    @classmethod
+    def from_openapi_data_oapg(cls, arg: float, _configuration: typing.Optional[Configuration] = None):
+        return super().from_openapi_data_oapg(arg, _configuration=_configuration)
+
+
+class Float64Base:
+    __inclusive_minimum = decimal.Decimal(-1.7976931348623157E+308)
+    __inclusive_maximum = decimal.Decimal(1.7976931348623157E+308)
+
+    @classmethod
+    def __validate_format(cls, arg: typing.Optional[decimal.Decimal], validation_metadata: ValidationMetadata):
+        if isinstance(arg, decimal.Decimal):
+            if not cls.__inclusive_minimum <= arg <= cls.__inclusive_maximum:
+                raise ApiValueError(
+                    "Invalid value '{}' for type double at {}".format(arg, validation_metadata.path_to_item)
+                )
 
-def is_valid_type(input_class_simple, valid_classes):
+    @classmethod
+    def _validate_oapg(
+        cls,
+        arg,
+        validation_metadata: ValidationMetadata,
+    ):
+        """
+        Float64Base _validate_oapg
+        """
+        cls.__validate_format(arg, validation_metadata=validation_metadata)
+        return super()._validate_oapg(arg, validation_metadata=validation_metadata)
+
+class Float64Schema(
+    Float64Base,
+    NumberSchema
+):
+
+    @classmethod
+    def from_openapi_data_oapg(cls, arg: float, _configuration: typing.Optional[Configuration] = None):
+        # todo check format
+        return super().from_openapi_data_oapg(arg, _configuration=_configuration)
+
+
+class StrSchema(
+    StrBase,
+    Schema,
+    StrMixin
+):
+    """
+    date + datetime string types must inherit from this class
+    That is because one can validate a str payload as both:
+    - type: string (format unset)
+    - type: string, format: date
     """
-    Args:
-        input_class_simple (class): the class of the input_value that we are
-            checking
-        valid_classes (tuple): the valid classes that the current item
-            should be
-    Returns:
-        bool
-    """
-    if issubclass(input_class_simple, OpenApiModel) and \
-            valid_classes == (bool, date, datetime, dict, float, int, list, str, none_type,):
-        return True
-    valid_type = input_class_simple in valid_classes
-    if not valid_type and (
-            issubclass(input_class_simple, OpenApiModel) or
-            input_class_simple is none_type):
-        for valid_class in valid_classes:
-            if input_class_simple is none_type and is_type_nullable(valid_class):
-                # Schema is oneOf/anyOf and the 'null' type is one of the allowed types.
-                return True
-            if not (issubclass(valid_class, OpenApiModel) and valid_class.discriminator):
-                continue
-            discr_propertyname_py = list(valid_class.discriminator.keys())[0]
-            discriminator_classes = (
-                valid_class.discriminator[discr_propertyname_py].values()
-            )
-            valid_type = is_valid_type(input_class_simple, discriminator_classes)
-            if valid_type:
-                return True
-    return valid_type
 
+    @classmethod
+    def from_openapi_data_oapg(cls, arg: str, _configuration: typing.Optional[Configuration] = None) -> 'StrSchema':
+        return super().from_openapi_data_oapg(arg, _configuration=_configuration)
+
+    def __new__(cls, arg: typing.Union[str, date, datetime, uuid.UUID], **kwargs: Configuration):
+        return super().__new__(cls, arg, **kwargs)
 
-def validate_and_convert_types(input_value, required_types_mixed, path_to_item,
-                               spec_property_naming, _check_type, configuration=None):
-    """Raises a TypeError is there is a problem, otherwise returns value
 
-    Args:
-        input_value (any): the data to validate/convert
-        required_types_mixed (list/dict/tuple): A list of
-            valid classes, or a list tuples of valid classes, or a dict where
-            the value is a tuple of value classes
-        path_to_item: (list) the path to the data being validated
-            this stores a list of keys or indices to get to the data being
-            validated
-        spec_property_naming (bool): True if the variable names in the input
-            data are serialized names as specified in the OpenAPI document.
-            False if the variables names in the input data are python
-            variable names in PEP-8 snake case.
-        _check_type: (boolean) if true, type will be checked and conversion
-            will be attempted.
-        configuration: (Configuration): the configuration class to use
-            when converting file_type items.
-            If passed, conversion will be attempted when possible
-            If not passed, no conversions will be attempted and
-            exceptions will be raised
-
-    Returns:
-        the correctly typed value
-
-    Raises:
-        ApiTypeError
-    """
-    results = get_required_type_classes(required_types_mixed, spec_property_naming)
-    valid_classes, child_req_types_by_current_type = results
-
-    input_class_simple = get_simple_class(input_value)
-    valid_type = is_valid_type(input_class_simple, valid_classes)
-    if not valid_type:
-        if (configuration
-                or (input_class_simple == dict
-                    and dict not in valid_classes)):
-            # if input_value is not valid_type try to convert it
-            converted_instance = attempt_convert_item(
-                input_value,
-                valid_classes,
-                path_to_item,
-                configuration,
-                spec_property_naming,
-                key_type=False,
-                must_convert=True,
-                check_type=_check_type
-            )
-            return converted_instance
-        else:
-            raise get_type_error(input_value, path_to_item, valid_classes,
-                                 key_type=False)
+class UUIDSchema(UUIDBase, StrSchema):
 
-    # input_value's type is in valid_classes
-    if len(valid_classes) > 1 and configuration:
-        # there are valid classes which are not the current class
-        valid_classes_coercible = remove_uncoercible(
-            valid_classes, input_value, spec_property_naming, must_convert=False)
-        if valid_classes_coercible:
-            converted_instance = attempt_convert_item(
-                input_value,
-                valid_classes_coercible,
-                path_to_item,
-                configuration,
-                spec_property_naming,
-                key_type=False,
-                must_convert=False,
-                check_type=_check_type
-            )
-            return converted_instance
+    def __new__(cls, arg: typing.Union[str, uuid.UUID], **kwargs: Configuration):
+        return super().__new__(cls, arg, **kwargs)
 
-    if child_req_types_by_current_type == {}:
-        # all types are of the required types and there are no more inner
-        # variables left to look at
-        return input_value
-    inner_required_types = child_req_types_by_current_type.get(
-        type(input_value)
-    )
-    if inner_required_types is None:
-        # for this type, there are not more inner variables left to look at
-        return input_value
-    if isinstance(input_value, list):
-        if input_value == []:
-            # allow an empty list
-            return input_value
-        for index, inner_value in enumerate(input_value):
-            inner_path = list(path_to_item)
-            inner_path.append(index)
-            input_value[index] = validate_and_convert_types(
-                inner_value,
-                inner_required_types,
-                inner_path,
-                spec_property_naming,
-                _check_type,
-                configuration=configuration
-            )
-    elif isinstance(input_value, dict):
-        if input_value == {}:
-            # allow an empty dict
-            return input_value
-        for inner_key, inner_val in input_value.items():
-            inner_path = list(path_to_item)
-            inner_path.append(inner_key)
-            if get_simple_class(inner_key) != str:
-                raise get_type_error(inner_key, inner_path, valid_classes,
-                                     key_type=True)
-            input_value[inner_key] = validate_and_convert_types(
-                inner_val,
-                inner_required_types,
-                inner_path,
-                spec_property_naming,
-                _check_type,
-                configuration=configuration
-            )
-    return input_value
 
+class DateSchema(DateBase, StrSchema):
 
-def model_to_dict(model_instance, serialize=True):
-    """Returns the model properties as a dict
+    def __new__(cls, arg: typing.Union[str, date], **kwargs: Configuration):
+        return super().__new__(cls, arg, **kwargs)
 
-    Args:
-        model_instance (one of your model instances): the model instance that
-            will be converted to a dict.
 
-    Keyword Args:
-        serialize (bool): if True, the keys in the dict will be values from
-            attribute_map
-    """
-    result = {}
-
-    def extract_item(item): return (
-        item[0], model_to_dict(
-            item[1], serialize=serialize)) if hasattr(
-        item[1], '_data_store') else item
-
-    model_instances = [model_instance]
-    if model_instance._composed_schemas:
-        model_instances.extend(model_instance._composed_instances)
-    seen_json_attribute_names = set()
-    used_fallback_python_attribute_names = set()
-    py_to_json_map = {}
-    for model_instance in model_instances:
-        for attr, value in model_instance._data_store.items():
-            if serialize:
-                # we use get here because additional property key names do not
-                # exist in attribute_map
-                try:
-                    attr = model_instance.attribute_map[attr]
-                    py_to_json_map.update(model_instance.attribute_map)
-                    seen_json_attribute_names.add(attr)
-                except KeyError:
-                    used_fallback_python_attribute_names.add(attr)
-            if isinstance(value, list):
-                if not value:
-                    # empty list or None
-                    result[attr] = value
-                else:
-                    res = []
-                    for v in value:
-                        if isinstance(v, PRIMITIVE_TYPES) or v is None:
-                            res.append(v)
-                        elif isinstance(v, ModelSimple):
-                            res.append(v.value)
-                        elif isinstance(v, dict):
-                            res.append(dict(map(
-                                extract_item,
-                                v.items()
-                            )))
-                        else:
-                            res.append(model_to_dict(v, serialize=serialize))
-                    result[attr] = res
-            elif isinstance(value, dict):
-                result[attr] = dict(map(
-                    extract_item,
-                    value.items()
-                ))
-            elif isinstance(value, ModelSimple):
-                result[attr] = value.value
-            elif hasattr(value, '_data_store'):
-                result[attr] = model_to_dict(value, serialize=serialize)
-            else:
-                result[attr] = value
-    if serialize:
-        for python_key in used_fallback_python_attribute_names:
-            json_key = py_to_json_map.get(python_key)
-            if json_key is None:
-                continue
-            if python_key == json_key:
-                continue
-            json_key_assigned_no_need_for_python_key = json_key in seen_json_attribute_names
-            if json_key_assigned_no_need_for_python_key:
-                del result[python_key]
-
-    return result
-
-
-def type_error_message(var_value=None, var_name=None, valid_classes=None,
-                       key_type=None):
-    """
-    Keyword Args:
-        var_value (any): the variable which has the type_error
-        var_name (str): the name of the variable which has the typ error
-        valid_classes (tuple): the accepted classes for current_item's
-                                  value
-        key_type (bool): False if our value is a value in a dict
-                         True if it is a key in a dict
-                         False if our item is an item in a list
-    """
-    key_or_value = 'value'
-    if key_type:
-        key_or_value = 'key'
-    valid_classes_phrase = get_valid_classes_phrase(valid_classes)
-    msg = (
-        "Invalid type for variable '{0}'. Required {1} type {2} and "
-        "passed type was {3}".format(
-            var_name,
-            key_or_value,
-            valid_classes_phrase,
-            type(var_value).__name__,
-        )
-    )
-    return msg
+class DateTimeSchema(DateTimeBase, StrSchema):
+
+    def __new__(cls, arg: typing.Union[str, datetime], **kwargs: Configuration):
+        return super().__new__(cls, arg, **kwargs)
+
+
+class DecimalSchema(DecimalBase, StrSchema):
+
+    def __new__(cls, arg: str, **kwargs: Configuration):
+        """
+        Note: Decimals may not be passed in because cast_to_allowed_types is only invoked once for payloads
+        which can be simple (str) or complex (dicts or lists with nested values)
+        Because casting is only done once and recursively casts all values prior to validation then for a potential
+        client side Decimal input if Decimal was accepted as an input in DecimalSchema then one would not know
+        if one was using it for a StrSchema (where it should be cast to str) or one is using it for NumberSchema
+        where it should stay as Decimal.
+        """
+        return super().__new__(cls, arg, **kwargs)
 
 
-def get_valid_classes_phrase(input_classes):
-    """Returns a string phrase describing what types are allowed
+class BytesSchema(
+    Schema,
+    BytesMixin
+):
     """
-    all_classes = list(input_classes)
-    all_classes = sorted(all_classes, key=lambda cls: cls.__name__)
-    all_class_names = [cls.__name__ for cls in all_classes]
-    if len(all_class_names) == 1:
-        return 'is {0}'.format(all_class_names[0])
-    return "is one of [{0}]".format(", ".join(all_class_names))
+    this class will subclass bytes and is immutable
+    """
+    def __new__(cls, arg: bytes, **kwargs: Configuration):
+        return super(Schema, cls).__new__(cls, arg)
 
 
-def get_allof_instances(self, model_args, constant_args):
+class FileSchema(
+    Schema,
+    FileMixin
+):
     """
-    Args:
-        self: the class we are handling
-        model_args (dict): var_name to var_value
-            used to make instances
-        constant_args (dict):
-            metadata arguments:
-            _check_type
-            _path_to_item
-            _spec_property_naming
-            _configuration
-            _visited_composed_classes
+    This class is NOT immutable
+    Dynamic classes are built using it for example when AnyType allows in binary data
+    Al other schema classes ARE immutable
+    If one wanted to make this immutable one could make this a DictSchema with required properties:
+    - data = BytesSchema (which would be an immutable bytes based schema)
+    - file_name = StrSchema
+    and cast_to_allowed_types would convert bytes and file instances into dicts containing data + file_name
+    The downside would be that data would be stored in memory which one may not want to do for very large files
 
-    Returns
-        composed_instances (list)
+    The developer is responsible for closing this file and deleting it
+
+    This class was kept as mutable:
+    - to allow file reading and writing to disk
+    - to be able to preserve file name info
     """
-    composed_instances = []
-    for allof_class in self._composed_schemas['allOf']:
 
-        try:
-            if constant_args.get('_spec_property_naming'):
-                allof_instance = allof_class._from_openapi_data(**model_args, **constant_args)
-            else:
-                allof_instance = allof_class(**model_args, **constant_args)
-            composed_instances.append(allof_instance)
-        except Exception as ex:
-            raise ApiValueError(
-                "Invalid inputs given to generate an instance of '%s'. The "
-                "input data was invalid for the allOf schema '%s' in the composed "
-                "schema '%s'. Error=%s" % (
-                    allof_class.__name__,
-                    allof_class.__name__,
-                    self.__class__.__name__,
-                    str(ex)
-                )
-            ) from ex
-    return composed_instances
+    def __new__(cls, arg: typing.Union[io.FileIO, io.BufferedReader], **kwargs: Configuration):
+        return super(Schema, cls).__new__(cls, arg)
 
 
-def get_oneof_instance(cls, model_kwargs, constant_kwargs, model_arg=None):
-    """
-    Find the oneOf schema that matches the input data (e.g. payload).
-    If exactly one schema matches the input data, an instance of that schema
-    is returned.
-    If zero or more than one schema match the input data, an exception is raised.
-    In OAS 3.x, the payload MUST, by validation, match exactly one of the
-    schemas described by oneOf.
+class BinaryBase:
+    pass
 
-    Args:
-        cls: the class we are handling
-        model_kwargs (dict): var_name to var_value
-            The input data, e.g. the payload that must match a oneOf schema
-            in the OpenAPI document.
-        constant_kwargs (dict): var_name to var_value
-            args that every model requires, including configuration, server
-            and path to item.
-
-    Kwargs:
-        model_arg: (int, float, bool, str, date, datetime, ModelSimple, None):
-            the value to assign to a primitive class or ModelSimple class
-            Notes:
-            - this is only passed in when oneOf includes types which are not object
-            - None is used to suppress handling of model_arg, nullable models are handled in __new__
 
-    Returns
-        oneof_instance (instance)
-    """
-    if len(cls._composed_schemas['oneOf']) == 0:
-        return None
+class BinarySchema(
+    ComposedBase,
+    BinaryBase,
+    Schema,
+    BinaryMixin
+):
+    class MetaOapg:
+        @staticmethod
+        def one_of():
+            return [
+                BytesSchema,
+                FileSchema,
+            ]
 
-    oneof_instances = []
-    # Iterate over each oneOf schema and determine if the input data
-    # matches the oneOf schemas.
-    for oneof_class in cls._composed_schemas['oneOf']:
-        # The composed oneOf schema allows the 'null' type and the input data
-        # is the null value. This is a OAS >= 3.1 feature.
-        if oneof_class is none_type:
-            # skip none_types because we are deserializing dict data.
-            # none_type deserialization is handled in the __new__ method
-            continue
+    def __new__(cls, arg: typing.Union[io.FileIO, io.BufferedReader, bytes], **kwargs: Configuration):
+        return super().__new__(cls, arg)
 
-        single_value_input = allows_single_value_input(oneof_class)
 
-        try:
-            if not single_value_input:
-                if constant_kwargs.get('_spec_property_naming'):
-                    oneof_instance = oneof_class._from_openapi_data(
-                        **model_kwargs, **constant_kwargs)
-                else:
-                    oneof_instance = oneof_class(**model_kwargs, **constant_kwargs)
-            else:
-                if issubclass(oneof_class, ModelSimple):
-                    if constant_kwargs.get('_spec_property_naming'):
-                        oneof_instance = oneof_class._from_openapi_data(
-                            model_arg, **constant_kwargs)
-                    else:
-                        oneof_instance = oneof_class(model_arg, **constant_kwargs)
-                elif oneof_class in PRIMITIVE_TYPES:
-                    oneof_instance = validate_and_convert_types(
-                        model_arg,
-                        (oneof_class,),
-                        constant_kwargs['_path_to_item'],
-                        constant_kwargs['_spec_property_naming'],
-                        constant_kwargs['_check_type'],
-                        configuration=constant_kwargs['_configuration']
-                    )
-            oneof_instances.append(oneof_instance)
-        except Exception:
-            pass
-    if len(oneof_instances) == 0:
-        raise ApiValueError(
-            "Invalid inputs given to generate an instance of %s. None "
-            "of the oneOf schemas matched the input data." %
-            cls.__name__
-        )
-    elif len(oneof_instances) > 1:
-        raise ApiValueError(
-            "Invalid inputs given to generate an instance of %s. Multiple "
-            "oneOf schemas matched the inputs, but a max of one is allowed." %
-            cls.__name__
-        )
-    return oneof_instances[0]
+class BoolSchema(
+    BoolBase,
+    Schema,
+    BoolMixin
+):
 
+    @classmethod
+    def from_openapi_data_oapg(cls, arg: bool, _configuration: typing.Optional[Configuration] = None):
+        return super().from_openapi_data_oapg(arg, _configuration=_configuration)
 
-def get_anyof_instances(self, model_args, constant_args):
-    """
-    Args:
-        self: the class we are handling
-        model_args (dict): var_name to var_value
-            The input data, e.g. the payload that must match at least one
-            anyOf child schema in the OpenAPI document.
-        constant_args (dict): var_name to var_value
-            args that every model requires, including configuration, server
-            and path to item.
-
-    Returns
-        anyof_instances (list)
-    """
-    anyof_instances = []
-    if len(self._composed_schemas['anyOf']) == 0:
-        return anyof_instances
-
-    for anyof_class in self._composed_schemas['anyOf']:
-        # The composed oneOf schema allows the 'null' type and the input data
-        # is the null value. This is a OAS >= 3.1 feature.
-        if anyof_class is none_type:
-            # skip none_types because we are deserializing dict data.
-            # none_type deserialization is handled in the __new__ method
-            continue
+    def __new__(cls, arg: bool, **kwargs: ValidationMetadata):
+        return super().__new__(cls, arg, **kwargs)
 
-        try:
-            if constant_args.get('_spec_property_naming'):
-                anyof_instance = anyof_class._from_openapi_data(**model_args, **constant_args)
-            else:
-                anyof_instance = anyof_class(**model_args, **constant_args)
-            anyof_instances.append(anyof_instance)
-        except Exception:
-            pass
-    if len(anyof_instances) == 0:
-        raise ApiValueError(
-            "Invalid inputs given to generate an instance of %s. None of the "
-            "anyOf schemas matched the inputs." %
-            self.__class__.__name__
+
+class AnyTypeSchema(
+    DictBase,
+    ListBase,
+    NumberBase,
+    StrBase,
+    BoolBase,
+    NoneBase,
+    Schema,
+    NoneFrozenDictTupleStrIntDecimalBoolFileBytesMixin
+):
+    # Python representation of a schema defined as true or {}
+    pass
+
+
+class UnsetAnyTypeSchema(AnyTypeSchema):
+    # Used when additionalProperties/items was not explicitly defined and a defining schema is needed
+    pass
+
+
+class NotAnyTypeSchema(
+    ComposedSchema,
+):
+    """
+    Python representation of a schema defined as false or {'not': {}}
+    Does not allow inputs in of AnyType
+    Note: validations on this class are never run because the code knows that no inputs will ever validate
+    """
+
+    class MetaOapg:
+        not_schema = AnyTypeSchema
+
+    def __new__(
+        cls,
+        *args,
+        _configuration: typing.Optional[Configuration] = None,
+    ) -> 'NotAnyTypeSchema':
+        return super().__new__(
+            cls,
+            *args,
+            _configuration=_configuration,
         )
-    return anyof_instances
 
 
-def get_discarded_args(self, composed_instances, model_args):
+class DictSchema(
+    DictBase,
+    Schema,
+    FrozenDictMixin
+):
+    @classmethod
+    def from_openapi_data_oapg(cls, arg: typing.Dict[str, typing.Any], _configuration: typing.Optional[Configuration] = None):
+        return super().from_openapi_data_oapg(arg, _configuration=_configuration)
+
+    def __new__(cls, *args: typing.Union[dict, frozendict.frozendict], **kwargs: typing.Union[dict, frozendict.frozendict, list, tuple, decimal.Decimal, float, int, str, date, datetime, bool, None, bytes, Schema, Unset, ValidationMetadata]):
+        return super().__new__(cls, *args, **kwargs)
+
+
+schema_type_classes = {NoneSchema, DictSchema, ListSchema, NumberSchema, StrSchema, BoolSchema, AnyTypeSchema}
+
+
+@functools.lru_cache()
+def get_new_class(
+    class_name: str,
+    bases: typing.Tuple[typing.Type[typing.Union[Schema, typing.Any]], ...]
+) -> typing.Type[Schema]:
     """
-    Gathers the args that were discarded by configuration.discard_unknown_keys
+    Returns a new class that is made with the subclass bases
     """
-    model_arg_keys = model_args.keys()
-    discarded_args = set()
-    # arguments passed to self were already converted to python names
-    # before __init__ was called
-    for instance in composed_instances:
-        if instance.__class__ in self._composed_schemas['allOf']:
-            try:
-                keys = instance.to_dict().keys()
-                discarded_keys = model_args - keys
-                discarded_args.update(discarded_keys)
-            except Exception:
-                # allOf integer schema will throw exception
-                pass
-        else:
-            try:
-                all_keys = set(model_to_dict(instance, serialize=False).keys())
-                js_keys = model_to_dict(instance, serialize=True).keys()
-                all_keys.update(js_keys)
-                discarded_keys = model_arg_keys - all_keys
-                discarded_args.update(discarded_keys)
-            except Exception:
-                # allOf integer schema will throw exception
-                pass
-    return discarded_args
+    new_cls: typing.Type[Schema] = type(class_name, bases, {})
+    return new_cls
 
 
-def validate_get_composed_info(constant_args, model_args, self):
-    """
-    For composed schemas, generate schema instances for
-    all schemas in the oneOf/anyOf/allOf definition. If additional
-    properties are allowed, also assign those properties on
-    all matched schemas that contain additionalProperties.
-    Openapi schemas are python classes.
+LOG_CACHE_USAGE = False
 
-    Exceptions are raised if:
-    - 0 or > 1 oneOf schema matches the model_args input data
-    - no anyOf schema matches the model_args input data
-    - any of the allOf schemas do not match the model_args input data
 
-    Args:
-        constant_args (dict): these are the args that every model requires
-        model_args (dict): these are the required and optional spec args that
-            were passed in to make this model
-        self (class): the class that we are instantiating
-            This class contains self._composed_schemas
-
-    Returns:
-        composed_info (list): length three
-            composed_instances (list): the composed instances which are not
-                self
-            var_name_to_model_instances (dict): a dict going from var_name
-                to the model_instance which holds that var_name
-                the model_instance may be self or an instance of one of the
-                classes in self.composed_instances()
-            additional_properties_model_instances (list): a list of the
-                model instances which have the property
-                additional_properties_type. This list can include self
-    """
-    # create composed_instances
-    composed_instances = []
-    allof_instances = get_allof_instances(self, model_args, constant_args)
-    composed_instances.extend(allof_instances)
-    oneof_instance = get_oneof_instance(self.__class__, model_args, constant_args)
-    if oneof_instance is not None:
-        composed_instances.append(oneof_instance)
-    anyof_instances = get_anyof_instances(self, model_args, constant_args)
-    composed_instances.extend(anyof_instances)
-    """
-    set additional_properties_model_instances
-    additional properties must be evaluated at the schema level
-    so self's additional properties are most important
-    If self is a composed schema with:
-    - no properties defined in self
-    - additionalProperties: False
-    Then for object payloads every property is an additional property
-    and they are not allowed, so only empty dict is allowed
-
-    Properties must be set on all matching schemas
-    so when a property is assigned toa composed instance, it must be set on all
-    composed instances regardless of additionalProperties presence
-    keeping it to prevent breaking changes in v5.0.1
-    TODO remove cls._additional_properties_model_instances in 6.0.0
-    """
-    additional_properties_model_instances = []
-    if self.additional_properties_type is not None:
-        additional_properties_model_instances = [self]
-
-    """
-    no need to set properties on self in here, they will be set in __init__
-    By here all composed schema oneOf/anyOf/allOf instances have their properties set using
-    model_args
-    """
-    discarded_args = get_discarded_args(self, composed_instances, model_args)
-
-    # map variable names to composed_instances
-    var_name_to_model_instances = {}
-    for prop_name in model_args:
-        if prop_name not in discarded_args:
-            var_name_to_model_instances[prop_name] = [self] + list(
-                filter(
-                    lambda x: prop_name in x.openapi_types, composed_instances))
-
-    return [
-        composed_instances,
-        var_name_to_model_instances,
-        additional_properties_model_instances,
-        discarded_args
-    ]
+def log_cache_usage(cache_fn):
+    if LOG_CACHE_USAGE:
+        print(cache_fn.__name__, cache_fn.cache_info())
```

### Comparing `dojah-python-sdk-3.0.0/test/test_categorize_transactions_request.py` & `dojah_python_sdk-4.0.0/dojah_client/type/categorize_transactions_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,28 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.categorize_transactions_request import CategorizeTransactionsRequest
-
-
-class TestCategorizeTransactionsRequest(unittest.TestCase):
-    """CategorizeTransactionsRequest unit test stubs"""
-
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
+RequiredCategorizeTransactionsRequest = TypedDict("RequiredCategorizeTransactionsRequest", {
+    })
 
-    def testCategorizeTransactionsRequest(self):
-        """Test CategorizeTransactionsRequest"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = CategorizeTransactionsRequest()  # noqa: E501
-        pass
+OptionalCategorizeTransactionsRequest = TypedDict("OptionalCategorizeTransactionsRequest", {
+    "description": str,
 
+    "trans_type": str,
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class CategorizeTransactionsRequest(RequiredCategorizeTransactionsRequest, OptionalCategorizeTransactionsRequest):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_categorize_transactions_response.py` & `dojah_python_sdk-4.0.0/dojah_client/type/categorize_transactions_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.categorize_transactions_response_entity import CategorizeTransactionsResponseEntity
-globals()['CategorizeTransactionsResponseEntity'] = CategorizeTransactionsResponseEntity
-from dojah_client.model.categorize_transactions_response import CategorizeTransactionsResponse
-
-
-class TestCategorizeTransactionsResponse(unittest.TestCase):
-    """CategorizeTransactionsResponse unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testCategorizeTransactionsResponse(self):
-        """Test CategorizeTransactionsResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = CategorizeTransactionsResponse()  # noqa: E501
-        pass
+RequiredCategorizeTransactionsResponse = TypedDict("RequiredCategorizeTransactionsResponse", {
+    })
 
+OptionalCategorizeTransactionsResponse = TypedDict("OptionalCategorizeTransactionsResponse", {
+    "entity": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class CategorizeTransactionsResponse(RequiredCategorizeTransactionsResponse, OptionalCategorizeTransactionsResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_collect_status_from_pdf_request.py` & `dojah_python_sdk-4.0.0/dojah_client/type/collect_status_from_pdf_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,28 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.collect_status_from_pdf_request import CollectStatusFromPdfRequest
-
-
-class TestCollectStatusFromPdfRequest(unittest.TestCase):
-    """CollectStatusFromPdfRequest unit test stubs"""
-
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
+RequiredCollectStatusFromPdfRequest = TypedDict("RequiredCollectStatusFromPdfRequest", {
+    })
 
-    def testCollectStatusFromPdfRequest(self):
-        """Test CollectStatusFromPdfRequest"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = CollectStatusFromPdfRequest()  # noqa: E501
-        pass
+OptionalCollectStatusFromPdfRequest = TypedDict("OptionalCollectStatusFromPdfRequest", {
+    "statement": typing.IO,
 
+    "bank_code": int,
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class CollectStatusFromPdfRequest(RequiredCollectStatusFromPdfRequest, OptionalCollectStatusFromPdfRequest):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_financial_get_full_bvn_response.py` & `dojah_python_sdk-4.0.0/dojah_client/type/get_full_bvn_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.financial_get_full_bvn_response_entity import FinancialGetFullBvnResponseEntity
-globals()['FinancialGetFullBvnResponseEntity'] = FinancialGetFullBvnResponseEntity
-from dojah_client.model.financial_get_full_bvn_response import FinancialGetFullBvnResponse
-
-
-class TestFinancialGetFullBvnResponse(unittest.TestCase):
-    """FinancialGetFullBvnResponse unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testFinancialGetFullBvnResponse(self):
-        """Test FinancialGetFullBvnResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = FinancialGetFullBvnResponse()  # noqa: E501
-        pass
+RequiredGetFullBvnResponse = TypedDict("RequiredGetFullBvnResponse", {
+    })
 
+OptionalGetFullBvnResponse = TypedDict("OptionalGetFullBvnResponse", {
+    "entity": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class GetFullBvnResponse(RequiredGetFullBvnResponse, OptionalGetFullBvnResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_financial_get_full_bvn_response_entity.py` & `dojah_python_sdk-4.0.0/dojah_client/type/financial_get_full_bvn_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.financial_get_full_bvn_response_entity import FinancialGetFullBvnResponseEntity
-
-
-class TestFinancialGetFullBvnResponseEntity(unittest.TestCase):
-    """FinancialGetFullBvnResponseEntity unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testFinancialGetFullBvnResponseEntity(self):
-        """Test FinancialGetFullBvnResponseEntity"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = FinancialGetFullBvnResponseEntity()  # noqa: E501
-        pass
+RequiredFinancialGetFullBvnResponse = TypedDict("RequiredFinancialGetFullBvnResponse", {
+    })
 
+OptionalFinancialGetFullBvnResponse = TypedDict("OptionalFinancialGetFullBvnResponse", {
+    "entity": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class FinancialGetFullBvnResponse(RequiredFinancialGetFullBvnResponse, OptionalFinancialGetFullBvnResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_get_account_analysis_response_entity_funds_management.py` & `dojah_python_sdk-4.0.0/dojah_client/type/get_account_analysis_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.get_account_analysis_response_entity_funds_management import GetAccountAnalysisResponseEntityFundsManagement
-
-
-class TestGetAccountAnalysisResponseEntityFundsManagement(unittest.TestCase):
-    """GetAccountAnalysisResponseEntityFundsManagement unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testGetAccountAnalysisResponseEntityFundsManagement(self):
-        """Test GetAccountAnalysisResponseEntityFundsManagement"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = GetAccountAnalysisResponseEntityFundsManagement()  # noqa: E501
-        pass
+RequiredGetAccountAnalysisResponse = TypedDict("RequiredGetAccountAnalysisResponse", {
+    })
 
+OptionalGetAccountAnalysisResponse = TypedDict("OptionalGetAccountAnalysisResponse", {
+    "entity": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class GetAccountAnalysisResponse(RequiredGetAccountAnalysisResponse, OptionalGetAccountAnalysisResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_get_banks_response.py` & `dojah_python_sdk-4.0.0/dojah_client/type/get_banks_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.get_banks_response_entity_inner import GetBanksResponseEntityInner
-globals()['GetBanksResponseEntityInner'] = GetBanksResponseEntityInner
-from dojah_client.model.get_banks_response import GetBanksResponse
-
-
-class TestGetBanksResponse(unittest.TestCase):
-    """GetBanksResponse unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testGetBanksResponse(self):
-        """Test GetBanksResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = GetBanksResponse()  # noqa: E501
-        pass
+RequiredGetBanksResponse = TypedDict("RequiredGetBanksResponse", {
+    })
 
+OptionalGetBanksResponse = TypedDict("OptionalGetBanksResponse", {
+    "entity": typing.List[typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class GetBanksResponse(RequiredGetBanksResponse, OptionalGetBanksResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_get_basic_bvn_response.py` & `dojah_python_sdk-4.0.0/dojah_client/type/get_basic_bvn_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.get_basic_bvn_response_entity import GetBasicBvnResponseEntity
-globals()['GetBasicBvnResponseEntity'] = GetBasicBvnResponseEntity
-from dojah_client.model.get_basic_bvn_response import GetBasicBvnResponse
-
-
-class TestGetBasicBvnResponse(unittest.TestCase):
-    """GetBasicBvnResponse unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testGetBasicBvnResponse(self):
-        """Test GetBasicBvnResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = GetBasicBvnResponse()  # noqa: E501
-        pass
+RequiredGetBasicBvnResponse = TypedDict("RequiredGetBasicBvnResponse", {
+    })
 
+OptionalGetBasicBvnResponse = TypedDict("OptionalGetBasicBvnResponse", {
+    "entity": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class GetBasicBvnResponse(RequiredGetBasicBvnResponse, OptionalGetBasicBvnResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_get_bin_response.py` & `dojah_python_sdk-4.0.0/dojah_client/type/get_bin_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.get_bin_response_entity import GetBinResponseEntity
-globals()['GetBinResponseEntity'] = GetBinResponseEntity
-from dojah_client.model.get_bin_response import GetBinResponse
-
-
-class TestGetBinResponse(unittest.TestCase):
-    """GetBinResponse unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testGetBinResponse(self):
-        """Test GetBinResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = GetBinResponse()  # noqa: E501
-        pass
+RequiredGetBinResponse = TypedDict("RequiredGetBinResponse", {
+    })
 
+OptionalGetBinResponse = TypedDict("OptionalGetBinResponse", {
+    "entity": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class GetBinResponse(RequiredGetBinResponse, OptionalGetBinResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_get_cac_response.py` & `dojah_python_sdk-4.0.0/dojah_client/type/get_advanced_cac_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.get_cac_response_entity import GetCacResponseEntity
-globals()['GetCacResponseEntity'] = GetCacResponseEntity
-from dojah_client.model.get_cac_response import GetCacResponse
-
-
-class TestGetCacResponse(unittest.TestCase):
-    """GetCacResponse unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testGetCacResponse(self):
-        """Test GetCacResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = GetCacResponse()  # noqa: E501
-        pass
+RequiredGetAdvancedCacResponse = TypedDict("RequiredGetAdvancedCacResponse", {
+    })
 
+OptionalGetAdvancedCacResponse = TypedDict("OptionalGetAdvancedCacResponse", {
+    "entity": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class GetAdvancedCacResponse(RequiredGetAdvancedCacResponse, OptionalGetAdvancedCacResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_get_earning_structure_response.py` & `dojah_python_sdk-4.0.0/dojah_client/type/get_earning_structure_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.get_earning_structure_response_entity import GetEarningStructureResponseEntity
-globals()['GetEarningStructureResponseEntity'] = GetEarningStructureResponseEntity
-from dojah_client.model.get_earning_structure_response import GetEarningStructureResponse
-
-
-class TestGetEarningStructureResponse(unittest.TestCase):
-    """GetEarningStructureResponse unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testGetEarningStructureResponse(self):
-        """Test GetEarningStructureResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = GetEarningStructureResponse()  # noqa: E501
-        pass
+RequiredGetEarningStructureResponse = TypedDict("RequiredGetEarningStructureResponse", {
+    })
 
+OptionalGetEarningStructureResponse = TypedDict("OptionalGetEarningStructureResponse", {
+    "entity": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class GetEarningStructureResponse(RequiredGetEarningStructureResponse, OptionalGetEarningStructureResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_get_email_reputation_response.py` & `dojah_python_sdk-4.0.0/dojah_client/type/get_email_reputation_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.get_email_reputation_response_entity import GetEmailReputationResponseEntity
-globals()['GetEmailReputationResponseEntity'] = GetEmailReputationResponseEntity
-from dojah_client.model.get_email_reputation_response import GetEmailReputationResponse
-
-
-class TestGetEmailReputationResponse(unittest.TestCase):
-    """GetEmailReputationResponse unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testGetEmailReputationResponse(self):
-        """Test GetEmailReputationResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = GetEmailReputationResponse()  # noqa: E501
-        pass
+RequiredGetEmailReputationResponse = TypedDict("RequiredGetEmailReputationResponse", {
+    })
 
+OptionalGetEmailReputationResponse = TypedDict("OptionalGetEmailReputationResponse", {
+    "entity": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class GetEmailReputationResponse(RequiredGetEmailReputationResponse, OptionalGetEmailReputationResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_get_generic_ocr_text_response.py` & `dojah_python_sdk-4.0.0/dojah_client/type/get_generic_ocr_text_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.get_ocr_text_response_entity import GetOcrTextResponseEntity
-globals()['GetOcrTextResponseEntity'] = GetOcrTextResponseEntity
-from dojah_client.model.get_generic_ocr_text_response import GetGenericOcrTextResponse
-
-
-class TestGetGenericOcrTextResponse(unittest.TestCase):
-    """GetGenericOcrTextResponse unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testGetGenericOcrTextResponse(self):
-        """Test GetGenericOcrTextResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = GetGenericOcrTextResponse()  # noqa: E501
-        pass
+RequiredGetGenericOcrTextResponse = TypedDict("RequiredGetGenericOcrTextResponse", {
+    })
 
+OptionalGetGenericOcrTextResponse = TypedDict("OptionalGetGenericOcrTextResponse", {
+    "entity": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class GetGenericOcrTextResponse(RequiredGetGenericOcrTextResponse, OptionalGetGenericOcrTextResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_get_kyc_drivers_license_response.py` & `dojah_python_sdk-4.0.0/dojah_client/type/get_drivers_license_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.get_kyc_drivers_license_response_entity import GetKycDriversLicenseResponseEntity
-globals()['GetKycDriversLicenseResponseEntity'] = GetKycDriversLicenseResponseEntity
-from dojah_client.model.get_kyc_drivers_license_response import GetKycDriversLicenseResponse
-
-
-class TestGetKycDriversLicenseResponse(unittest.TestCase):
-    """GetKycDriversLicenseResponse unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testGetKycDriversLicenseResponse(self):
-        """Test GetKycDriversLicenseResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = GetKycDriversLicenseResponse()  # noqa: E501
-        pass
+RequiredGetDriversLicenseResponse = TypedDict("RequiredGetDriversLicenseResponse", {
+    })
 
+OptionalGetDriversLicenseResponse = TypedDict("OptionalGetDriversLicenseResponse", {
+    "entity": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class GetDriversLicenseResponse(RequiredGetDriversLicenseResponse, OptionalGetDriversLicenseResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_get_ocr_text_response.py` & `dojah_python_sdk-4.0.0/dojah_client/type/get_ocr_text_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.get_ocr_text_response_entity import GetOcrTextResponseEntity
-globals()['GetOcrTextResponseEntity'] = GetOcrTextResponseEntity
-from dojah_client.model.get_ocr_text_response import GetOcrTextResponse
-
-
-class TestGetOcrTextResponse(unittest.TestCase):
-    """GetOcrTextResponse unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testGetOcrTextResponse(self):
-        """Test GetOcrTextResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = GetOcrTextResponse()  # noqa: E501
-        pass
+RequiredGetOcrTextResponse = TypedDict("RequiredGetOcrTextResponse", {
+    })
 
+OptionalGetOcrTextResponse = TypedDict("OptionalGetOcrTextResponse", {
+    "entity": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class GetOcrTextResponse(RequiredGetOcrTextResponse, OptionalGetOcrTextResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_get_ssnit_response_entity.py` & `dojah_python_sdk-4.0.0/dojah_client/type/get_ssnit_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.get_ssnit_response_entity import GetSsnitResponseEntity
-
-
-class TestGetSsnitResponseEntity(unittest.TestCase):
-    """GetSsnitResponseEntity unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testGetSsnitResponseEntity(self):
-        """Test GetSsnitResponseEntity"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = GetSsnitResponseEntity()  # noqa: E501
-        pass
+RequiredGetSsnitResponse = TypedDict("RequiredGetSsnitResponse", {
+    })
 
+OptionalGetSsnitResponse = TypedDict("OptionalGetSsnitResponse", {
+    "entity": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class GetSsnitResponse(RequiredGetSsnitResponse, OptionalGetSsnitResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_get_transaction_response.py` & `dojah_python_sdk-4.0.0/dojah_client/type/get_transaction_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.get_transaction_response_entity import GetTransactionResponseEntity
-globals()['GetTransactionResponseEntity'] = GetTransactionResponseEntity
-from dojah_client.model.get_transaction_response import GetTransactionResponse
-
-
-class TestGetTransactionResponse(unittest.TestCase):
-    """GetTransactionResponse unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testGetTransactionResponse(self):
-        """Test GetTransactionResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = GetTransactionResponse()  # noqa: E501
-        pass
+RequiredGetTransactionResponse = TypedDict("RequiredGetTransactionResponse", {
+    })
 
+OptionalGetTransactionResponse = TypedDict("OptionalGetTransactionResponse", {
+    "entity": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class GetTransactionResponse(RequiredGetTransactionResponse, OptionalGetTransactionResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_get_vin_response.py` & `dojah_python_sdk-4.0.0/dojah_client/type/get_tin_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.get_vin_response_entity import GetVinResponseEntity
-globals()['GetVinResponseEntity'] = GetVinResponseEntity
-from dojah_client.model.get_vin_response import GetVinResponse
-
-
-class TestGetVinResponse(unittest.TestCase):
-    """GetVinResponse unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testGetVinResponse(self):
-        """Test GetVinResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = GetVinResponse()  # noqa: E501
-        pass
+RequiredGetTinResponse = TypedDict("RequiredGetTinResponse", {
+    })
 
+OptionalGetTinResponse = TypedDict("OptionalGetTinResponse", {
+    "entity": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class GetTinResponse(RequiredGetTinResponse, OptionalGetTinResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_get_voter_response.py` & `dojah_python_sdk-4.0.0/dojah_client/type/get_voter_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.get_voter_response_entity import GetVoterResponseEntity
-globals()['GetVoterResponseEntity'] = GetVoterResponseEntity
-from dojah_client.model.get_voter_response import GetVoterResponse
-
-
-class TestGetVoterResponse(unittest.TestCase):
-    """GetVoterResponse unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testGetVoterResponse(self):
-        """Test GetVoterResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = GetVoterResponse()  # noqa: E501
-        pass
+RequiredGetVoterResponse = TypedDict("RequiredGetVoterResponse", {
+    "entity": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    })
 
+OptionalGetVoterResponse = TypedDict("OptionalGetVoterResponse", {
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class GetVoterResponse(RequiredGetVoterResponse, OptionalGetVoterResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_get_wallet_balance_response.py` & `dojah_python_sdk-4.0.0/dojah_client/type/get_wallet_balance_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.get_wallet_balance_response_entity import GetWalletBalanceResponseEntity
-globals()['GetWalletBalanceResponseEntity'] = GetWalletBalanceResponseEntity
-from dojah_client.model.get_wallet_balance_response import GetWalletBalanceResponse
-
-
-class TestGetWalletBalanceResponse(unittest.TestCase):
-    """GetWalletBalanceResponse unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testGetWalletBalanceResponse(self):
-        """Test GetWalletBalanceResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = GetWalletBalanceResponse()  # noqa: E501
-        pass
+RequiredGetWalletBalanceResponse = TypedDict("RequiredGetWalletBalanceResponse", {
+    })
 
+OptionalGetWalletBalanceResponse = TypedDict("OptionalGetWalletBalanceResponse", {
+    "entity": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class GetWalletBalanceResponse(RequiredGetWalletBalanceResponse, OptionalGetWalletBalanceResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_get_wallets_response.py` & `dojah_python_sdk-4.0.0/dojah_client/type/get_wallets_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.get_wallets_response_entity import GetWalletsResponseEntity
-globals()['GetWalletsResponseEntity'] = GetWalletsResponseEntity
-from dojah_client.model.get_wallets_response import GetWalletsResponse
-
-
-class TestGetWalletsResponse(unittest.TestCase):
-    """GetWalletsResponse unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testGetWalletsResponse(self):
-        """Test GetWalletsResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = GetWalletsResponse()  # noqa: E501
-        pass
+RequiredGetWalletsResponse = TypedDict("RequiredGetWalletsResponse", {
+    })
 
+OptionalGetWalletsResponse = TypedDict("OptionalGetWalletsResponse", {
+    "entity": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class GetWalletsResponse(RequiredGetWalletsResponse, OptionalGetWalletsResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_notify_webhook_request.py` & `dojah_python_sdk-4.0.0/dojah_client/type/notify_webhook_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,28 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.notify_webhook_request_data import NotifyWebhookRequestData
-globals()['NotifyWebhookRequestData'] = NotifyWebhookRequestData
-from dojah_client.model.notify_webhook_request import NotifyWebhookRequest
-
-
-class TestNotifyWebhookRequest(unittest.TestCase):
-    """NotifyWebhookRequest unit test stubs"""
-
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
+RequiredNotifyWebhookRequest = TypedDict("RequiredNotifyWebhookRequest", {
+    })
 
-    def testNotifyWebhookRequest(self):
-        """Test NotifyWebhookRequest"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = NotifyWebhookRequest()  # noqa: E501
-        pass
+OptionalNotifyWebhookRequest = TypedDict("OptionalNotifyWebhookRequest", {
+    "subject": str,
 
+    "data": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class NotifyWebhookRequest(RequiredNotifyWebhookRequest, OptionalNotifyWebhookRequest):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_screen_aml_response_entity.py` & `dojah_python_sdk-4.0.0/dojah_client/type/screen_aml_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.screen_aml_response_entity import ScreenAmlResponseEntity
-
-
-class TestScreenAmlResponseEntity(unittest.TestCase):
-    """ScreenAmlResponseEntity unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testScreenAmlResponseEntity(self):
-        """Test ScreenAmlResponseEntity"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ScreenAmlResponseEntity()  # noqa: E501
-        pass
+RequiredScreenAmlResponse = TypedDict("RequiredScreenAmlResponse", {
+    })
 
+OptionalScreenAmlResponse = TypedDict("OptionalScreenAmlResponse", {
+    "entity": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class ScreenAmlResponse(RequiredScreenAmlResponse, OptionalScreenAmlResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_validate_bvn_response.py` & `dojah_python_sdk-4.0.0/dojah_client/type/validate_bvn_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.validate_bvn_response_entity import ValidateBvnResponseEntity
-globals()['ValidateBvnResponseEntity'] = ValidateBvnResponseEntity
-from dojah_client.model.validate_bvn_response import ValidateBvnResponse
-
-
-class TestValidateBvnResponse(unittest.TestCase):
-    """ValidateBvnResponse unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testValidateBvnResponse(self):
-        """Test ValidateBvnResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ValidateBvnResponse()  # noqa: E501
-        pass
+RequiredValidateBvnResponse = TypedDict("RequiredValidateBvnResponse", {
+    })
 
+OptionalValidateBvnResponse = TypedDict("OptionalValidateBvnResponse", {
+    "entity": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class ValidateBvnResponse(RequiredValidateBvnResponse, OptionalValidateBvnResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_validate_otp_response_entity.py` & `dojah_python_sdk-4.0.0/dojah_client/type/validate_otp_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.validate_otp_response_entity import ValidateOtpResponseEntity
-
-
-class TestValidateOtpResponseEntity(unittest.TestCase):
-    """ValidateOtpResponseEntity unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testValidateOtpResponseEntity(self):
-        """Test ValidateOtpResponseEntity"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = ValidateOtpResponseEntity()  # noqa: E501
-        pass
+RequiredValidateOtpResponse = TypedDict("RequiredValidateOtpResponse", {
+    })
 
+OptionalValidateOtpResponse = TypedDict("OptionalValidateOtpResponse", {
+    "entity": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class ValidateOtpResponse(RequiredValidateOtpResponse, OptionalValidateOtpResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_verify_photo_id_with_selfie_response_entity_selfie.py` & `dojah_python_sdk-4.0.0/dojah_client/type/verify_photo_id_with_selfie_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.verify_photo_id_with_selfie_response_entity_selfie import VerifyPhotoIdWithSelfieResponseEntitySelfie
-
-
-class TestVerifyPhotoIdWithSelfieResponseEntitySelfie(unittest.TestCase):
-    """VerifyPhotoIdWithSelfieResponseEntitySelfie unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testVerifyPhotoIdWithSelfieResponseEntitySelfie(self):
-        """Test VerifyPhotoIdWithSelfieResponseEntitySelfie"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = VerifyPhotoIdWithSelfieResponseEntitySelfie()  # noqa: E501
-        pass
+RequiredVerifyPhotoIdWithSelfieResponse = TypedDict("RequiredVerifyPhotoIdWithSelfieResponse", {
+    })
 
+OptionalVerifyPhotoIdWithSelfieResponse = TypedDict("OptionalVerifyPhotoIdWithSelfieResponse", {
+    "entity": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class VerifyPhotoIdWithSelfieResponse(RequiredVerifyPhotoIdWithSelfieResponse, OptionalVerifyPhotoIdWithSelfieResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_verify_selfie_bvn_request.py` & `dojah_python_sdk-4.0.0/dojah_client/type/verify_selfie_bvn_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,28 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.verify_selfie_bvn_request import VerifySelfieBvnRequest
-
-
-class TestVerifySelfieBvnRequest(unittest.TestCase):
-    """VerifySelfieBvnRequest unit test stubs"""
-
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
+RequiredVerifySelfieBvnRequest = TypedDict("RequiredVerifySelfieBvnRequest", {
+    })
 
-    def testVerifySelfieBvnRequest(self):
-        """Test VerifySelfieBvnRequest"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = VerifySelfieBvnRequest()  # noqa: E501
-        pass
+OptionalVerifySelfieBvnRequest = TypedDict("OptionalVerifySelfieBvnRequest", {
+    "bvn": str,
 
+    "selfie_image": str,
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class VerifySelfieBvnRequest(RequiredVerifySelfieBvnRequest, OptionalVerifySelfieBvnRequest):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_verify_selfie_bvn_response.py` & `dojah_python_sdk-4.0.0/dojah_client/type/verify_selfie_bvn_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,26 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.verify_selfie_bvn_response_entity import VerifySelfieBvnResponseEntity
-globals()['VerifySelfieBvnResponseEntity'] = VerifySelfieBvnResponseEntity
-from dojah_client.model.verify_selfie_bvn_response import VerifySelfieBvnResponse
-
-
-class TestVerifySelfieBvnResponse(unittest.TestCase):
-    """VerifySelfieBvnResponse unit test stubs"""
-
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
 
-    def testVerifySelfieBvnResponse(self):
-        """Test VerifySelfieBvnResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = VerifySelfieBvnResponse()  # noqa: E501
-        pass
+RequiredVerifySelfieBvnResponse = TypedDict("RequiredVerifySelfieBvnResponse", {
+    })
 
+OptionalVerifySelfieBvnResponse = TypedDict("OptionalVerifySelfieBvnResponse", {
+    "entity": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class VerifySelfieBvnResponse(RequiredVerifySelfieBvnResponse, OptionalVerifySelfieBvnResponse):
+    pass
```

### Comparing `dojah-python-sdk-3.0.0/test/test_verify_selfie_nin_request.py` & `dojah_python_sdk-4.0.0/dojah_client/type/verify_selfie_nin_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,28 @@
+# coding: utf-8
+
 """
     DOJAH APIs
 
-    Use Dojah to verify, onboard and manage user identity across Africa!  # noqa: E501
+    Use Dojah to verify, onboard and manage user identity across Africa!
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import sys
-import unittest
-
-import dojah_client
-from dojah_client.model.verify_selfie_nin_request import VerifySelfieNinRequest
-
-
-class TestVerifySelfieNinRequest(unittest.TestCase):
-    """VerifySelfieNinRequest unit test stubs"""
-
-    def setUp(self):
-        pass
 
-    def tearDown(self):
-        pass
+RequiredVerifySelfieNinRequest = TypedDict("RequiredVerifySelfieNinRequest", {
+    })
 
-    def testVerifySelfieNinRequest(self):
-        """Test VerifySelfieNinRequest"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = VerifySelfieNinRequest()  # noqa: E501
-        pass
+OptionalVerifySelfieNinRequest = TypedDict("OptionalVerifySelfieNinRequest", {
+    "nin": str,
 
+    "selfie_image": str,
+    }, total=False)
 
-if __name__ == '__main__':
-    unittest.main()
+class VerifySelfieNinRequest(RequiredVerifySelfieNinRequest, OptionalVerifySelfieNinRequest):
+    pass
```

