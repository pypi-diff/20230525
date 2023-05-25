# Comparing `tmp/mercoa-0.0.8.tar.gz` & `tmp/mercoa-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercoa-0.0.8.tar", max compression
+gzip compressed data, was "mercoa-0.0.9.tar", max compression
```

## Comparing `mercoa-0.0.8.tar` & `mercoa-0.0.9.tar`

### file list

```diff
@@ -1,144 +1,149 @@
--rw-r--r--   0        0        0      410 2023-05-11 04:26:07.369902 mercoa-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4995 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/__init__.py
--rw-r--r--   0        0        0     5019 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/client.py
--rw-r--r--   0        0        0      348 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/core/__init__.py
--rw-r--r--   0        0        0      326 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/core/datetime_utils.py
--rw-r--r--   0        0        0     3507 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      157 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/environment.py
--rw-r--r--   0        0        0        0 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/py.typed
--rw-r--r--   0        0        0     5125 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/__init__.py
--rw-r--r--   0        0        0      165 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/bank_lookup/__init__.py
--rw-r--r--   0        0        0     2582 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/bank_lookup/client.py
--rw-r--r--   0        0        0      205 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/bank_lookup/types/__init__.py
--rw-r--r--   0        0        0      960 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/bank_lookup/types/bank_address.py
--rw-r--r--   0        0        0      946 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
--rw-r--r--   0        0        0      359 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/commons/__init__.py
--rw-r--r--   0        0        0      148 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/commons/errors/__init__.py
--rw-r--r--   0        0        0      216 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/commons/errors/unauthorized_error.py
--rw-r--r--   0        0        0      407 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/commons/types/__init__.py
--rw-r--r--   0        0        0     1093 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/commons/types/address.py
--rw-r--r--   0        0        0      824 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/commons/types/birth_date.py
--rw-r--r--   0        0        0      994 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/commons/types/full_name.py
--rw-r--r--   0        0        0      850 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/commons/types/individual_government_id.py
--rw-r--r--   0        0        0      857 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/commons/types/itin.py
--rw-r--r--   0        0        0      855 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/commons/types/phone_number.py
--rw-r--r--   0        0        0      856 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/commons/types/ssn.py
--rw-r--r--   0        0        0      199 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/counterparty/__init__.py
--rw-r--r--   0        0        0     4513 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/counterparty/client.py
--rw-r--r--   0        0        0      256 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/counterparty/types/__init__.py
--rw-r--r--   0        0        0     1022 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/counterparty/types/counterparty_response.py
--rw-r--r--   0        0        0     1446 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/counterparty/types/find_counterparties_response.py
--rw-r--r--   0        0        0      811 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/__init__.py
--rw-r--r--   0        0        0    21970 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/client.py
--rw-r--r--   0        0        0     1195 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/__init__.py
--rw-r--r--   0        0        0      487 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/account_type.py
--rw-r--r--   0        0        0     1535 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/business_profile_request.py
--rw-r--r--   0        0        0     1492 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/business_profile_response.py
--rw-r--r--   0        0        0     1917 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/business_type.py
--rw-r--r--   0        0        0      741 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/ein.py
--rw-r--r--   0        0        0       80 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/entity_id.py
--rw-r--r--   0        0        0     1546 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/entity_request.py
--rw-r--r--   0        0        0     1590 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/entity_response.py
--rw-r--r--   0        0        0     1084 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/entity_status.py
--rw-r--r--   0        0        0     1586 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/entity_update_request.py
--rw-r--r--   0        0        0     1372 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/individual_profile_request.py
--rw-r--r--   0        0        0     1206 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/individual_profile_response.py
--rw-r--r--   0        0        0     1059 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/invoice_metrics_response.py
--rw-r--r--   0        0        0      974 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/profile_request.py
--rw-r--r--   0        0        0      981 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/profile_response.py
--rw-r--r--   0        0        0      761 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity/types/tax_id.py
--rw-r--r--   0        0        0      207 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity_users/__init__.py
--rw-r--r--   0        0        0     9662 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity_users/client.py
--rw-r--r--   0        0        0      281 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity_users/types/__init__.py
--rw-r--r--   0        0        0       84 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity_users/types/entity_user_id.py
--rw-r--r--   0        0        0     1100 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity_users/types/entity_user_request.py
--rw-r--r--   0        0        0     1224 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/entity_users/types/entity_user_response.py
--rw-r--r--   0        0        0      633 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/__init__.py
--rw-r--r--   0        0        0    19563 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/client.py
--rw-r--r--   0        0        0      916 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/__init__.py
--rw-r--r--   0        0        0       81 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/comment_id.py
--rw-r--r--   0        0        0      750 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/comment_request.py
--rw-r--r--   0        0        0      937 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/comment_response.py
--rw-r--r--   0        0        0     1048 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/create_vendor_request.py
--rw-r--r--   0        0        0    22179 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/currency_code.py
--rw-r--r--   0        0        0      955 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/document_response.py
--rw-r--r--   0        0        0       81 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/invoice_id.py
--rw-r--r--   0        0        0     1302 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/invoice_line_item_request.py
--rw-r--r--   0        0        0     1229 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/invoice_line_item_response.py
--rw-r--r--   0        0        0     3437 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/invoice_request.py
--rw-r--r--   0        0        0     3144 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/invoice_response.py
--rw-r--r--   0        0        0     1332 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/invoice/types/invoice_status.py
--rw-r--r--   0        0        0      213 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/ocr/__init__.py
--rw-r--r--   0        0        0     4443 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/ocr/client.py
--rw-r--r--   0        0        0      298 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/ocr/types/__init__.py
--rw-r--r--   0        0        0     1068 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/ocr/types/attachments.py
--rw-r--r--   0        0        0     1969 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/ocr/types/email_ocr_request.py
--rw-r--r--   0        0        0      891 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/ocr/types/ocr_mailbox.py
--rw-r--r--   0        0        0     1234 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/ocr/types/ocr_response.py
--rw-r--r--   0        0        0      983 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/__init__.py
--rw-r--r--   0        0        0     7449 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/client.py
--rw-r--r--   0        0        0     1466 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/__init__.py
--rw-r--r--   0        0        0      948 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/color_scheme_request.py
--rw-r--r--   0        0        0      949 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/color_scheme_response.py
--rw-r--r--   0        0        0      981 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/email_log_response.py
--rw-r--r--   0        0        0      932 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/email_provider_request.py
--rw-r--r--   0        0        0      936 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/email_provider_response.py
--rw-r--r--   0        0        0      656 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/email_sender_provider.py
--rw-r--r--   0        0        0     1052 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/email_sender_request.py
--rw-r--r--   0        0        0     1044 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/email_sender_response.py
--rw-r--r--   0        0        0       86 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/organization_id.py
--rw-r--r--   0        0        0     1463 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/organization_request.py
--rw-r--r--   0        0        0     1579 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/organization_response.py
--rw-r--r--   0        0        0     1142 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/payment_methods_request.py
--rw-r--r--   0        0        0     1148 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/payment_methods_response.py
--rw-r--r--   0        0        0      849 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/payment_rail_markup.py
--rw-r--r--   0        0        0      482 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/payment_rail_markup_type.py
--rw-r--r--   0        0        0     1145 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/payment_rail_request.py
--rw-r--r--   0        0        0      797 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/organization/types/payment_rail_response.py
--rw-r--r--   0        0        0      943 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/__init__.py
--rw-r--r--   0        0        0    12242 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/client.py
--rw-r--r--   0        0        0     1411 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/__init__.py
--rw-r--r--   0        0        0       85 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/bank_account_id.py
--rw-r--r--   0        0        0     1297 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/bank_account_request.py
--rw-r--r--   0        0        0     1318 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/bank_account_response.py
--rw-r--r--   0        0        0      960 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/bank_status.py
--rw-r--r--   0        0        0      632 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/bank_type.py
--rw-r--r--   0        0        0      819 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/card_brand.py
--rw-r--r--   0        0        0       78 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/card_id.py
--rw-r--r--   0        0        0     1120 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/card_request.py
--rw-r--r--   0        0        0     1217 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/card_response.py
--rw-r--r--   0        0        0      750 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/card_type.py
--rw-r--r--   0        0        0       79 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/check_id.py
--rw-r--r--   0        0        0     1152 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/check_request.py
--rw-r--r--   0        0        0     1327 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/check_response.py
--rw-r--r--   0        0        0       80 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/custom_id.py
--rw-r--r--   0        0        0     1568 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/custom_payment_method_request.py
--rw-r--r--   0        0        0     1922 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/custom_payment_method_response.py
--rw-r--r--   0        0        0       87 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/payment_method_id.py
--rw-r--r--   0        0        0     1296 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/payment_method_request.py
--rw-r--r--   0        0        0     1508 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/payment_method_response.py
--rw-r--r--   0        0        0     1229 2023-05-11 04:26:07.369902 mercoa-0.0.8/src/mercoa/resources/payment_method/types/payment_method_type.py
--rw-r--r--   0        0        0      425 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/payment_method_schema/__init__.py
--rw-r--r--   0        0        0     7794 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/payment_method_schema/client.py
--rw-r--r--   0        0        0      589 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/payment_method_schema/types/__init__.py
--rw-r--r--   0        0        0     1984 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py
--rw-r--r--   0        0        0      682 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py
--rw-r--r--   0        0        0       93 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/payment_method_schema/types/payment_method_schema_id.py
--rw-r--r--   0        0        0     1249 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py
--rw-r--r--   0        0        0     1468 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py
--rw-r--r--   0        0        0      269 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/representative/__init__.py
--rw-r--r--   0        0        0     8182 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/representative/client.py
--rw-r--r--   0        0        0      381 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/representative/types/__init__.py
--rw-r--r--   0        0        0       88 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/representative/types/representative_id.py
--rw-r--r--   0        0        0     1370 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/representative/types/representative_request.py
--rw-r--r--   0        0        0     1539 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/representative/types/representative_response.py
--rw-r--r--   0        0        0     1100 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/representative/types/responsibilities.py
--rw-r--r--   0        0        0      211 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/transaction/__init__.py
--rw-r--r--   0        0        0     4206 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/transaction/client.py
--rw-r--r--   0        0        0      284 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/transaction/types/__init__.py
--rw-r--r--   0        0        0       85 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/transaction/types/transaction_id.py
--rw-r--r--   0        0        0     1125 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/transaction/types/transaction_response.py
--rw-r--r--   0        0        0     1261 2023-05-11 04:26:07.373902 mercoa-0.0.8/src/mercoa/resources/transaction/types/transaction_status.py
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 mercoa-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      410 2023-05-19 14:42:27.516931 mercoa-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5163 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/__init__.py
+-rw-r--r--   0        0        0     5449 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/client.py
+-rw-r--r--   0        0        0      348 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/core/__init__.py
+-rw-r--r--   0        0        0      326 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/core/datetime_utils.py
+-rw-r--r--   0        0        0     3507 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      157 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/environment.py
+-rw-r--r--   0        0        0        0 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/py.typed
+-rw-r--r--   0        0        0     5313 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/__init__.py
+-rw-r--r--   0        0        0      165 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/bank_lookup/__init__.py
+-rw-r--r--   0        0        0     2582 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/bank_lookup/client.py
+-rw-r--r--   0        0        0      205 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/bank_lookup/types/__init__.py
+-rw-r--r--   0        0        0      960 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/bank_lookup/types/bank_address.py
+-rw-r--r--   0        0        0      946 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
+-rw-r--r--   0        0        0      359 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/commons/__init__.py
+-rw-r--r--   0        0        0      148 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/commons/errors/__init__.py
+-rw-r--r--   0        0        0      216 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/commons/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      407 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0     1093 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/commons/types/address.py
+-rw-r--r--   0        0        0      824 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/commons/types/birth_date.py
+-rw-r--r--   0        0        0      994 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/commons/types/full_name.py
+-rw-r--r--   0        0        0      850 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/commons/types/individual_government_id.py
+-rw-r--r--   0        0        0      857 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/commons/types/itin.py
+-rw-r--r--   0        0        0      855 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/commons/types/phone_number.py
+-rw-r--r--   0        0        0      856 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/commons/types/ssn.py
+-rw-r--r--   0        0        0      199 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/counterparty/__init__.py
+-rw-r--r--   0        0        0     4513 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/counterparty/client.py
+-rw-r--r--   0        0        0      256 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/counterparty/types/__init__.py
+-rw-r--r--   0        0        0     1022 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/counterparty/types/counterparty_response.py
+-rw-r--r--   0        0        0     1446 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/counterparty/types/find_counterparties_response.py
+-rw-r--r--   0        0        0      811 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/__init__.py
+-rw-r--r--   0        0        0    21970 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/client.py
+-rw-r--r--   0        0        0     1195 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/__init__.py
+-rw-r--r--   0        0        0      487 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/account_type.py
+-rw-r--r--   0        0        0     1535 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/business_profile_request.py
+-rw-r--r--   0        0        0     1492 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/business_profile_response.py
+-rw-r--r--   0        0        0     1917 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/business_type.py
+-rw-r--r--   0        0        0      741 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/ein.py
+-rw-r--r--   0        0        0       80 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/entity_id.py
+-rw-r--r--   0        0        0     2432 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/entity_request.py
+-rw-r--r--   0        0        0     1814 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/entity_response.py
+-rw-r--r--   0        0        0     1084 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/entity_status.py
+-rw-r--r--   0        0        0     2084 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/entity_update_request.py
+-rw-r--r--   0        0        0     1372 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/individual_profile_request.py
+-rw-r--r--   0        0        0     1206 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/individual_profile_response.py
+-rw-r--r--   0        0        0     1059 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/invoice_metrics_response.py
+-rw-r--r--   0        0        0      974 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/profile_request.py
+-rw-r--r--   0        0        0      981 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/profile_response.py
+-rw-r--r--   0        0        0      761 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity/types/tax_id.py
+-rw-r--r--   0        0        0      207 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity_users/__init__.py
+-rw-r--r--   0        0        0     9662 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity_users/client.py
+-rw-r--r--   0        0        0      281 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity_users/types/__init__.py
+-rw-r--r--   0        0        0       84 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity_users/types/entity_user_id.py
+-rw-r--r--   0        0        0     1100 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity_users/types/entity_user_request.py
+-rw-r--r--   0        0        0     1224 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/entity_users/types/entity_user_response.py
+-rw-r--r--   0        0        0      633 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/invoice/__init__.py
+-rw-r--r--   0        0        0    19563 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/invoice/client.py
+-rw-r--r--   0        0        0      916 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/invoice/types/__init__.py
+-rw-r--r--   0        0        0       81 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/invoice/types/comment_id.py
+-rw-r--r--   0        0        0      750 2023-05-19 14:42:27.516931 mercoa-0.0.9/src/mercoa/resources/invoice/types/comment_request.py
+-rw-r--r--   0        0        0      937 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/invoice/types/comment_response.py
+-rw-r--r--   0        0        0     1048 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/invoice/types/create_vendor_request.py
+-rw-r--r--   0        0        0    22179 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/invoice/types/currency_code.py
+-rw-r--r--   0        0        0      955 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/invoice/types/document_response.py
+-rw-r--r--   0        0        0       81 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/invoice/types/invoice_id.py
+-rw-r--r--   0        0        0     1302 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/invoice/types/invoice_line_item_request.py
+-rw-r--r--   0        0        0     1229 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/invoice/types/invoice_line_item_response.py
+-rw-r--r--   0        0        0     3437 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/invoice/types/invoice_request.py
+-rw-r--r--   0        0        0     3144 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/invoice/types/invoice_response.py
+-rw-r--r--   0        0        0     1485 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/invoice/types/invoice_status.py
+-rw-r--r--   0        0        0      213 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/ocr/__init__.py
+-rw-r--r--   0        0        0     4443 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/ocr/client.py
+-rw-r--r--   0        0        0      298 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/ocr/types/__init__.py
+-rw-r--r--   0        0        0     1068 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/ocr/types/attachments.py
+-rw-r--r--   0        0        0     1969 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/ocr/types/email_ocr_request.py
+-rw-r--r--   0        0        0      891 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/ocr/types/ocr_mailbox.py
+-rw-r--r--   0        0        0     1234 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/ocr/types/ocr_response.py
+-rw-r--r--   0        0        0      983 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/__init__.py
+-rw-r--r--   0        0        0     7449 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/client.py
+-rw-r--r--   0        0        0     1466 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/__init__.py
+-rw-r--r--   0        0        0      948 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/color_scheme_request.py
+-rw-r--r--   0        0        0      949 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/color_scheme_response.py
+-rw-r--r--   0        0        0      981 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/email_log_response.py
+-rw-r--r--   0        0        0      932 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/email_provider_request.py
+-rw-r--r--   0        0        0      936 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/email_provider_response.py
+-rw-r--r--   0        0        0      656 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/email_sender_provider.py
+-rw-r--r--   0        0        0     1052 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/email_sender_request.py
+-rw-r--r--   0        0        0     1044 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/email_sender_response.py
+-rw-r--r--   0        0        0       86 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/organization_id.py
+-rw-r--r--   0        0        0     1463 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/organization_request.py
+-rw-r--r--   0        0        0     1579 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/organization_response.py
+-rw-r--r--   0        0        0     1142 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/payment_methods_request.py
+-rw-r--r--   0        0        0     1148 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/payment_methods_response.py
+-rw-r--r--   0        0        0      849 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/payment_rail_markup.py
+-rw-r--r--   0        0        0      482 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/payment_rail_markup_type.py
+-rw-r--r--   0        0        0     1145 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/payment_rail_request.py
+-rw-r--r--   0        0        0      797 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/organization/types/payment_rail_response.py
+-rw-r--r--   0        0        0      943 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/__init__.py
+-rw-r--r--   0        0        0    12242 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/client.py
+-rw-r--r--   0        0        0     1411 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/__init__.py
+-rw-r--r--   0        0        0       85 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/bank_account_id.py
+-rw-r--r--   0        0        0     1297 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/bank_account_request.py
+-rw-r--r--   0        0        0     1318 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/bank_account_response.py
+-rw-r--r--   0        0        0      960 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/bank_status.py
+-rw-r--r--   0        0        0      632 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/bank_type.py
+-rw-r--r--   0        0        0      819 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/card_brand.py
+-rw-r--r--   0        0        0       78 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/card_id.py
+-rw-r--r--   0        0        0     1120 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/card_request.py
+-rw-r--r--   0        0        0     1217 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/card_response.py
+-rw-r--r--   0        0        0      750 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/card_type.py
+-rw-r--r--   0        0        0       79 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/check_id.py
+-rw-r--r--   0        0        0     1152 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/check_request.py
+-rw-r--r--   0        0        0     1327 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/check_response.py
+-rw-r--r--   0        0        0       80 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/custom_id.py
+-rw-r--r--   0        0        0     1568 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/custom_payment_method_request.py
+-rw-r--r--   0        0        0     1922 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/custom_payment_method_response.py
+-rw-r--r--   0        0        0       87 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/payment_method_id.py
+-rw-r--r--   0        0        0     1296 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/payment_method_request.py
+-rw-r--r--   0        0        0     1662 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/payment_method_response.py
+-rw-r--r--   0        0        0     1229 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method/types/payment_method_type.py
+-rw-r--r--   0        0        0      425 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method_schema/__init__.py
+-rw-r--r--   0        0        0     7794 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method_schema/client.py
+-rw-r--r--   0        0        0      589 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method_schema/types/__init__.py
+-rw-r--r--   0        0        0     1984 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py
+-rw-r--r--   0        0        0      682 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py
+-rw-r--r--   0        0        0       93 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method_schema/types/payment_method_schema_id.py
+-rw-r--r--   0        0        0     1597 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py
+-rw-r--r--   0        0        0     1709 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py
+-rw-r--r--   0        0        0      143 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/process_invoice/__init__.py
+-rw-r--r--   0        0        0     2498 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/process_invoice/client.py
+-rw-r--r--   0        0        0      161 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/process_invoice/types/__init__.py
+-rw-r--r--   0        0        0      916 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/process_invoice/types/process_invoice_request.py
+-rw-r--r--   0        0        0      269 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/representative/__init__.py
+-rw-r--r--   0        0        0     8182 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/representative/client.py
+-rw-r--r--   0        0        0      381 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/representative/types/__init__.py
+-rw-r--r--   0        0        0       88 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/representative/types/representative_id.py
+-rw-r--r--   0        0        0     1370 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/representative/types/representative_request.py
+-rw-r--r--   0        0        0     1539 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/representative/types/representative_response.py
+-rw-r--r--   0        0        0     1100 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/representative/types/responsibilities.py
+-rw-r--r--   0        0        0      271 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/transaction/__init__.py
+-rw-r--r--   0        0        0     4315 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/transaction/client.py
+-rw-r--r--   0        0        0      386 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/transaction/types/__init__.py
+-rw-r--r--   0        0        0       85 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/transaction/types/transaction_id.py
+-rw-r--r--   0        0        0     1125 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/transaction/types/transaction_response.py
+-rw-r--r--   0        0        0     1564 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/transaction/types/transaction_response_expanded.py
+-rw-r--r--   0        0        0     1261 2023-05-19 14:42:27.520931 mercoa-0.0.9/src/mercoa/resources/transaction/types/transaction_status.py
+-rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 mercoa-0.0.9/PKG-INFO
```

### Comparing `mercoa-0.0.8/src/mercoa/__init__.py` & `mercoa-0.0.9/src/mercoa/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,35 +83,38 @@
     PaymentMethodsResponse,
     PaymentMethodType,
     PaymentRailMarkup,
     PaymentRailMarkupType,
     PaymentRailRequest,
     PaymentRailResponse,
     PhoneNumber,
+    ProcessInvoiceRequest,
     ProfileRequest,
     ProfileResponse,
     RepresentativeId,
     RepresentativeRequest,
     RepresentativeResponse,
     Responsibilities,
     TaxID,
     TransactionId,
     TransactionResponse,
+    TransactionResponseExpanded,
     TransactionStatus,
     UnauthorizedError,
     bank_lookup,
     commons,
     counterparty,
     entity,
     entity_users,
     invoice,
     ocr,
     organization,
     payment_method,
     payment_method_schema,
+    process_invoice,
     representative,
     transaction,
 )
 
 __all__ = [
     "AccountType",
     "Address",
@@ -194,32 +197,35 @@
     "PaymentMethodsRequest",
     "PaymentMethodsResponse",
     "PaymentRailMarkup",
     "PaymentRailMarkupType",
     "PaymentRailRequest",
     "PaymentRailResponse",
     "PhoneNumber",
+    "ProcessInvoiceRequest",
     "ProfileRequest",
     "ProfileResponse",
     "RepresentativeId",
     "RepresentativeRequest",
     "RepresentativeResponse",
     "Responsibilities",
     "SSN",
     "TaxID",
     "TransactionId",
     "TransactionResponse",
+    "TransactionResponseExpanded",
     "TransactionStatus",
     "UnauthorizedError",
     "bank_lookup",
     "commons",
     "counterparty",
     "entity",
     "entity_users",
     "invoice",
     "ocr",
     "organization",
     "payment_method",
     "payment_method_schema",
+    "process_invoice",
     "representative",
     "transaction",
 ]
```

### Comparing `mercoa-0.0.8/src/mercoa/client.py` & `mercoa-0.0.9/src/mercoa/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .resources.entity.client import AsyncEntityClient, EntityClient
 from .resources.entity_users.client import AsyncEntityUsersClient, EntityUsersClient
 from .resources.invoice.client import AsyncInvoiceClient, InvoiceClient
 from .resources.ocr.client import AsyncOcrClient, OcrClient
 from .resources.organization.client import AsyncOrganizationClient, OrganizationClient
 from .resources.payment_method.client import AsyncPaymentMethodClient, PaymentMethodClient
 from .resources.payment_method_schema.client import AsyncPaymentMethodSchemaClient, PaymentMethodSchemaClient
+from .resources.process_invoice.client import AsyncProcessInvoiceClient, ProcessInvoiceClient
 from .resources.representative.client import AsyncRepresentativeClient, RepresentativeClient
 from .resources.transaction.client import AsyncTransactionClient, TransactionClient
 
 
 class Mercoa:
     def __init__(
         self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
@@ -58,14 +59,18 @@
         return PaymentMethodSchemaClient(environment=self._environment, token=self._token)
 
     @cached_property
     def payment_method(self) -> PaymentMethodClient:
         return PaymentMethodClient(environment=self._environment, token=self._token)
 
     @cached_property
+    def process_invoice(self) -> ProcessInvoiceClient:
+        return ProcessInvoiceClient(environment=self._environment, token=self._token)
+
+    @cached_property
     def representative(self) -> RepresentativeClient:
         return RepresentativeClient(environment=self._environment, token=self._token)
 
     @cached_property
     def transaction(self) -> TransactionClient:
         return TransactionClient(environment=self._environment, token=self._token)
 
@@ -110,13 +115,17 @@
         return AsyncPaymentMethodSchemaClient(environment=self._environment, token=self._token)
 
     @cached_property
     def payment_method(self) -> AsyncPaymentMethodClient:
         return AsyncPaymentMethodClient(environment=self._environment, token=self._token)
 
     @cached_property
+    def process_invoice(self) -> AsyncProcessInvoiceClient:
+        return AsyncProcessInvoiceClient(environment=self._environment, token=self._token)
+
+    @cached_property
     def representative(self) -> AsyncRepresentativeClient:
         return AsyncRepresentativeClient(environment=self._environment, token=self._token)
 
     @cached_property
     def transaction(self) -> AsyncTransactionClient:
         return AsyncTransactionClient(environment=self._environment, token=self._token)
```

### Comparing `mercoa-0.0.8/src/mercoa/core/datetime_utils.py` & `mercoa-0.0.9/src/mercoa/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/core/jsonable_encoder.py` & `mercoa-0.0.9/src/mercoa/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/__init__.py` & `mercoa-0.0.9/src/mercoa/resources/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     entity,
     entity_users,
     invoice,
     ocr,
     organization,
     payment_method,
     payment_method_schema,
+    process_invoice,
     representative,
     transaction,
 )
 from .bank_lookup import BankAddress, BankLookupResponse
 from .commons import ITIN, SSN, Address, BirthDate, FullName, IndividualGovernmentID, PhoneNumber, UnauthorizedError
 from .counterparty import CounterpartyResponse, FindCounterpartiesResponse
 from .entity import (
@@ -95,16 +96,17 @@
 from .payment_method_schema import (
     PaymentMethodSchemaField,
     PaymentMethodSchemaFieldType,
     PaymentMethodSchemaId,
     PaymentMethodSchemaRequest,
     PaymentMethodSchemaResponse,
 )
+from .process_invoice import ProcessInvoiceRequest
 from .representative import RepresentativeId, RepresentativeRequest, RepresentativeResponse, Responsibilities
-from .transaction import TransactionId, TransactionResponse, TransactionStatus
+from .transaction import TransactionId, TransactionResponse, TransactionResponseExpanded, TransactionStatus
 
 __all__ = [
     "AccountType",
     "Address",
     "Attachments",
     "BankAccountId",
     "BankAccountRequest",
@@ -183,32 +185,35 @@
     "PaymentMethodsRequest",
     "PaymentMethodsResponse",
     "PaymentRailMarkup",
     "PaymentRailMarkupType",
     "PaymentRailRequest",
     "PaymentRailResponse",
     "PhoneNumber",
+    "ProcessInvoiceRequest",
     "ProfileRequest",
     "ProfileResponse",
     "RepresentativeId",
     "RepresentativeRequest",
     "RepresentativeResponse",
     "Responsibilities",
     "SSN",
     "TaxID",
     "TransactionId",
     "TransactionResponse",
+    "TransactionResponseExpanded",
     "TransactionStatus",
     "UnauthorizedError",
     "bank_lookup",
     "commons",
     "counterparty",
     "entity",
     "entity_users",
     "invoice",
     "ocr",
     "organization",
     "payment_method",
     "payment_method_schema",
+    "process_invoice",
     "representative",
     "transaction",
 ]
```

### Comparing `mercoa-0.0.8/src/mercoa/resources/bank_lookup/client.py` & `mercoa-0.0.9/src/mercoa/resources/bank_lookup/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/bank_lookup/types/bank_address.py` & `mercoa-0.0.9/src/mercoa/resources/bank_lookup/types/bank_address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py` & `mercoa-0.0.9/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/commons/types/address.py` & `mercoa-0.0.9/src/mercoa/resources/commons/types/address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/commons/types/birth_date.py` & `mercoa-0.0.9/src/mercoa/resources/commons/types/birth_date.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/commons/types/full_name.py` & `mercoa-0.0.9/src/mercoa/resources/commons/types/full_name.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/commons/types/individual_government_id.py` & `mercoa-0.0.9/src/mercoa/resources/commons/types/individual_government_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/commons/types/itin.py` & `mercoa-0.0.9/src/mercoa/resources/commons/types/itin.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/commons/types/phone_number.py` & `mercoa-0.0.9/src/mercoa/resources/commons/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/commons/types/ssn.py` & `mercoa-0.0.9/src/mercoa/resources/commons/types/ssn.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/counterparty/client.py` & `mercoa-0.0.9/src/mercoa/resources/counterparty/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/counterparty/types/counterparty_response.py` & `mercoa-0.0.9/src/mercoa/resources/counterparty/types/counterparty_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/counterparty/types/find_counterparties_response.py` & `mercoa-0.0.9/src/mercoa/resources/counterparty/types/find_counterparties_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/entity/__init__.py` & `mercoa-0.0.9/src/mercoa/resources/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/entity/client.py` & `mercoa-0.0.9/src/mercoa/resources/entity/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/entity/types/__init__.py` & `mercoa-0.0.9/src/mercoa/resources/entity/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/entity/types/business_profile_request.py` & `mercoa-0.0.9/src/mercoa/resources/entity/types/business_profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/entity/types/business_profile_response.py` & `mercoa-0.0.9/src/mercoa/resources/entity/types/business_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/entity/types/business_type.py` & `mercoa-0.0.9/src/mercoa/resources/entity/types/business_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/entity/types/ein.py` & `mercoa-0.0.9/src/mercoa/resources/entity/types/ein.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/entity/types/entity_request.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method/types/check_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,32 +2,24 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .account_type import AccountType
-from .profile_request import ProfileRequest
 
 
-class EntityRequest(pydantic.BaseModel):
-    foreign_id: typing.Optional[str] = pydantic.Field(alias="foreignId")
-    email_to: typing.Optional[str] = pydantic.Field(
-        alias="emailTo", description=("Email inbox address. Do not inclue the @domain.com\n")
-    )
-    email_to_alias: typing.Optional[typing.List[str]] = pydantic.Field(
-        alias="emailToAlias",
-        description=(
-            "Email inbox alias addresses. Used when forwarding emails to the emailTo address from an alias. Include the full email address.\n"
-        ),
-    )
-    owned_by_org: typing.Optional[bool] = pydantic.Field(alias="ownedByOrg")
-    account_type: AccountType = pydantic.Field(alias="accountType")
-    profile: ProfileRequest
+class CheckRequest(pydantic.BaseModel):
+    pay_to_the_order_of: str = pydantic.Field(alias="payToTheOrderOf")
+    address_line_1: str = pydantic.Field(alias="addressLine1")
+    address_line_2: typing.Optional[str] = pydantic.Field(alias="addressLine2")
+    city: str
+    state_or_province: str = pydantic.Field(alias="stateOrProvince")
+    postal_code: str = pydantic.Field(alias="postalCode")
+    country: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.8/src/mercoa/resources/entity/types/entity_response.py` & `mercoa-0.0.9/src/mercoa/resources/entity/types/entity_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     owned_by_org: bool = pydantic.Field(alias="ownedByOrg")
     account_type: AccountType = pydantic.Field(alias="accountType")
     name: str
     email: str
     profile: ProfileResponse
     status: EntityStatus
     accepted_tos: bool = pydantic.Field(alias="acceptedTos")
+    is_payor: bool = pydantic.Field(alias="isPayor", description=("True if this entity can pay invoices.\n"))
+    is_payee: bool = pydantic.Field(alias="isPayee", description=("True if this entity can receive payments.\n"))
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
     updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mercoa-0.0.8/src/mercoa/resources/entity/types/entity_status.py` & `mercoa-0.0.9/src/mercoa/resources/entity/types/entity_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/entity/types/entity_update_request.py` & `mercoa-0.0.9/src/mercoa/resources/organization/types/organization_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,32 +2,27 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .account_type import AccountType
-from .profile_request import ProfileRequest
+from .color_scheme_request import ColorSchemeRequest
+from .email_provider_request import EmailProviderRequest
+from .payment_methods_request import PaymentMethodsRequest
 
 
-class EntityUpdateRequest(pydantic.BaseModel):
-    foreign_id: typing.Optional[str] = pydantic.Field(alias="foreignId")
-    email_to: typing.Optional[str] = pydantic.Field(
-        alias="emailTo", description=("Email inbox address. Do not inclue the @domain.com\n")
-    )
-    email_to_alias: typing.Optional[typing.List[str]] = pydantic.Field(
-        alias="emailToAlias",
-        description=(
-            "Email inbox alias addresses. Used when forwarding emails to the emailTo address from an alias. Include the full email address.\n"
-        ),
-    )
-    owned_by_org: typing.Optional[bool] = pydantic.Field(alias="ownedByOrg")
-    account_type: typing.Optional[AccountType] = pydantic.Field(alias="accountType")
-    profile: typing.Optional[ProfileRequest]
+class OrganizationRequest(pydantic.BaseModel):
+    name: typing.Optional[str]
+    logo: typing.Optional[str]
+    website_url: typing.Optional[str] = pydantic.Field(alias="websiteUrl")
+    support_email: typing.Optional[str] = pydantic.Field(alias="supportEmail")
+    payment_methods: typing.Optional[PaymentMethodsRequest] = pydantic.Field(alias="paymentMethods")
+    email_provider: typing.Optional[EmailProviderRequest] = pydantic.Field(alias="emailProvider")
+    color_scheme: typing.Optional[ColorSchemeRequest] = pydantic.Field(alias="colorScheme")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.8/src/mercoa/resources/entity/types/individual_profile_request.py` & `mercoa-0.0.9/src/mercoa/resources/entity/types/individual_profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/entity/types/individual_profile_response.py` & `mercoa-0.0.9/src/mercoa/resources/entity/types/individual_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/entity/types/invoice_metrics_response.py` & `mercoa-0.0.9/src/mercoa/resources/entity/types/invoice_metrics_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/entity/types/profile_request.py` & `mercoa-0.0.9/src/mercoa/resources/entity/types/profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/entity/types/profile_response.py` & `mercoa-0.0.9/src/mercoa/resources/entity/types/profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/entity/types/tax_id.py` & `mercoa-0.0.9/src/mercoa/resources/entity/types/tax_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/entity_users/client.py` & `mercoa-0.0.9/src/mercoa/resources/entity_users/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/entity_users/types/entity_user_request.py` & `mercoa-0.0.9/src/mercoa/resources/entity_users/types/entity_user_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/entity_users/types/entity_user_response.py` & `mercoa-0.0.9/src/mercoa/resources/entity_users/types/entity_user_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/invoice/__init__.py` & `mercoa-0.0.9/src/mercoa/resources/invoice/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/invoice/client.py` & `mercoa-0.0.9/src/mercoa/resources/invoice/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/invoice/types/__init__.py` & `mercoa-0.0.9/src/mercoa/resources/invoice/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/invoice/types/comment_request.py` & `mercoa-0.0.9/src/mercoa/resources/invoice/types/comment_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/invoice/types/comment_response.py` & `mercoa-0.0.9/src/mercoa/resources/invoice/types/comment_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/invoice/types/create_vendor_request.py` & `mercoa-0.0.9/src/mercoa/resources/invoice/types/create_vendor_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/invoice/types/currency_code.py` & `mercoa-0.0.9/src/mercoa/resources/invoice/types/currency_code.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/invoice/types/document_response.py` & `mercoa-0.0.9/src/mercoa/resources/invoice/types/document_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/invoice/types/invoice_line_item_request.py` & `mercoa-0.0.9/src/mercoa/resources/invoice/types/invoice_line_item_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/invoice/types/invoice_line_item_response.py` & `mercoa-0.0.9/src/mercoa/resources/invoice/types/invoice_line_item_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/invoice/types/invoice_request.py` & `mercoa-0.0.9/src/mercoa/resources/invoice/types/invoice_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/invoice/types/invoice_response.py` & `mercoa-0.0.9/src/mercoa/resources/invoice/types/invoice_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/invoice/types/invoice_status.py` & `mercoa-0.0.9/src/mercoa/resources/invoice/types/invoice_status.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,25 +11,27 @@
     NEW = "NEW"
     PENDING = "PENDING"
     PAID = "PAID"
     CANCELED = "CANCELED"
     REFUSED = "REFUSED"
     APPROVED = "APPROVED"
     ARCHIVED = "ARCHIVED"
+    SCHEDULED = "SCHEDULED"
 
     def visit(
         self,
         draft: typing.Callable[[], T_Result],
         new: typing.Callable[[], T_Result],
         pending: typing.Callable[[], T_Result],
         paid: typing.Callable[[], T_Result],
         canceled: typing.Callable[[], T_Result],
         refused: typing.Callable[[], T_Result],
         approved: typing.Callable[[], T_Result],
         archived: typing.Callable[[], T_Result],
+        scheduled: typing.Callable[[], T_Result],
     ) -> T_Result:
         if self is InvoiceStatus.DRAFT:
             return draft()
         if self is InvoiceStatus.NEW:
             return new()
         if self is InvoiceStatus.PENDING:
             return pending()
@@ -39,7 +41,9 @@
             return canceled()
         if self is InvoiceStatus.REFUSED:
             return refused()
         if self is InvoiceStatus.APPROVED:
             return approved()
         if self is InvoiceStatus.ARCHIVED:
             return archived()
+        if self is InvoiceStatus.SCHEDULED:
+            return scheduled()
```

### Comparing `mercoa-0.0.8/src/mercoa/resources/ocr/client.py` & `mercoa-0.0.9/src/mercoa/resources/ocr/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/ocr/types/attachments.py` & `mercoa-0.0.9/src/mercoa/resources/ocr/types/attachments.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/ocr/types/email_ocr_request.py` & `mercoa-0.0.9/src/mercoa/resources/ocr/types/email_ocr_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/ocr/types/ocr_mailbox.py` & `mercoa-0.0.9/src/mercoa/resources/ocr/types/ocr_mailbox.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/ocr/types/ocr_response.py` & `mercoa-0.0.9/src/mercoa/resources/ocr/types/ocr_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/organization/__init__.py` & `mercoa-0.0.9/src/mercoa/resources/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/organization/client.py` & `mercoa-0.0.9/src/mercoa/resources/organization/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/organization/types/__init__.py` & `mercoa-0.0.9/src/mercoa/resources/organization/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/organization/types/color_scheme_request.py` & `mercoa-0.0.9/src/mercoa/resources/organization/types/color_scheme_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/organization/types/color_scheme_response.py` & `mercoa-0.0.9/src/mercoa/resources/organization/types/color_scheme_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/organization/types/email_log_response.py` & `mercoa-0.0.9/src/mercoa/resources/organization/types/email_log_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/organization/types/email_provider_request.py` & `mercoa-0.0.9/src/mercoa/resources/organization/types/email_provider_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/organization/types/email_provider_response.py` & `mercoa-0.0.9/src/mercoa/resources/organization/types/email_provider_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/organization/types/email_sender_provider.py` & `mercoa-0.0.9/src/mercoa/resources/organization/types/email_sender_provider.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/organization/types/email_sender_request.py` & `mercoa-0.0.9/src/mercoa/resources/organization/types/email_sender_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/organization/types/email_sender_response.py` & `mercoa-0.0.9/src/mercoa/resources/organization/types/email_sender_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/organization/types/organization_request.py` & `mercoa-0.0.9/src/mercoa/resources/organization/types/organization_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,27 +2,30 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .color_scheme_request import ColorSchemeRequest
-from .email_provider_request import EmailProviderRequest
-from .payment_methods_request import PaymentMethodsRequest
+from .color_scheme_response import ColorSchemeResponse
+from .email_provider_response import EmailProviderResponse
+from .organization_id import OrganizationId
+from .payment_methods_response import PaymentMethodsResponse
 
 
-class OrganizationRequest(pydantic.BaseModel):
-    name: typing.Optional[str]
-    logo: typing.Optional[str]
+class OrganizationResponse(pydantic.BaseModel):
+    id: OrganizationId
+    sandbox: bool
+    name: str
+    logo_url: typing.Optional[str] = pydantic.Field(alias="logoUrl")
     website_url: typing.Optional[str] = pydantic.Field(alias="websiteUrl")
     support_email: typing.Optional[str] = pydantic.Field(alias="supportEmail")
-    payment_methods: typing.Optional[PaymentMethodsRequest] = pydantic.Field(alias="paymentMethods")
-    email_provider: typing.Optional[EmailProviderRequest] = pydantic.Field(alias="emailProvider")
-    color_scheme: typing.Optional[ColorSchemeRequest] = pydantic.Field(alias="colorScheme")
+    payment_methods: typing.Optional[PaymentMethodsResponse] = pydantic.Field(alias="paymentMethods")
+    email_provider: typing.Optional[EmailProviderResponse] = pydantic.Field(alias="emailProvider")
+    color_scheme: typing.Optional[ColorSchemeResponse] = pydantic.Field(alias="colorScheme")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.8/src/mercoa/resources/organization/types/organization_response.py` & `mercoa-0.0.9/src/mercoa/resources/transaction/types/transaction_response_expanded.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,30 +2,28 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .color_scheme_response import ColorSchemeResponse
-from .email_provider_response import EmailProviderResponse
-from .organization_id import OrganizationId
-from .payment_methods_response import PaymentMethodsResponse
-
-
-class OrganizationResponse(pydantic.BaseModel):
-    id: OrganizationId
-    sandbox: bool
-    name: str
-    logo_url: typing.Optional[str] = pydantic.Field(alias="logoUrl")
-    website_url: typing.Optional[str] = pydantic.Field(alias="websiteUrl")
-    support_email: typing.Optional[str] = pydantic.Field(alias="supportEmail")
-    payment_methods: typing.Optional[PaymentMethodsResponse] = pydantic.Field(alias="paymentMethods")
-    email_provider: typing.Optional[EmailProviderResponse] = pydantic.Field(alias="emailProvider")
-    color_scheme: typing.Optional[ColorSchemeResponse] = pydantic.Field(alias="colorScheme")
+from ...entity.types.entity_response import EntityResponse
+from ...invoice.types.invoice_id import InvoiceId
+from ...payment_method.types.payment_method_response import PaymentMethodResponse
+from .transaction_response import TransactionResponse
+
+
+class TransactionResponseExpanded(TransactionResponse):
+    invoice_id: InvoiceId = pydantic.Field(alias="invoiceId")
+    deduction_date: typing.Optional[dt.datetime] = pydantic.Field(alias="deductionDate")
+    due_date: typing.Optional[dt.datetime] = pydantic.Field(alias="dueDate")
+    payer: typing.Optional[EntityResponse]
+    vendor: typing.Optional[EntityResponse]
+    payment_source: typing.Optional[PaymentMethodResponse] = pydantic.Field(alias="paymentSource")
+    payment_destination: typing.Optional[PaymentMethodResponse] = pydantic.Field(alias="paymentDestination")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.8/src/mercoa/resources/organization/types/payment_methods_request.py` & `mercoa-0.0.9/src/mercoa/resources/organization/types/payment_methods_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/organization/types/payment_methods_response.py` & `mercoa-0.0.9/src/mercoa/resources/organization/types/payment_methods_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/organization/types/payment_rail_markup.py` & `mercoa-0.0.9/src/mercoa/resources/organization/types/payment_rail_markup.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/organization/types/payment_rail_request.py` & `mercoa-0.0.9/src/mercoa/resources/organization/types/payment_rail_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/organization/types/payment_rail_response.py` & `mercoa-0.0.9/src/mercoa/resources/organization/types/payment_rail_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method/__init__.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method/client.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method/types/__init__.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method/types/bank_account_request.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method/types/bank_account_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method/types/bank_account_response.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method/types/bank_account_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method/types/bank_status.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method/types/bank_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method/types/bank_type.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method/types/bank_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method/types/card_brand.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method/types/card_brand.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method/types/card_request.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method/types/card_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method/types/card_response.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method/types/card_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method/types/card_type.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method/types/card_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method/types/check_request.py` & `mercoa-0.0.9/src/mercoa/resources/representative/types/responsibilities.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,22 +4,19 @@
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 
 
-class CheckRequest(pydantic.BaseModel):
-    pay_to_the_order_of: str = pydantic.Field(alias="payToTheOrderOf")
-    address_line_1: str = pydantic.Field(alias="addressLine1")
-    address_line_2: typing.Optional[str] = pydantic.Field(alias="addressLine2")
-    city: str
-    state_or_province: str = pydantic.Field(alias="stateOrProvince")
-    postal_code: str = pydantic.Field(alias="postalCode")
-    country: str
+class Responsibilities(pydantic.BaseModel):
+    job_title: typing.Optional[str] = pydantic.Field(alias="jobTitle")
+    is_controller: typing.Optional[bool] = pydantic.Field(alias="isController")
+    is_owner: typing.Optional[bool] = pydantic.Field(alias="isOwner")
+    ownership_percentage: typing.Optional[float] = pydantic.Field(alias="ownershipPercentage")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method/types/check_response.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method/types/check_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method/types/custom_payment_method_request.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method/types/custom_payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method/types/custom_payment_method_response.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method/types/custom_payment_method_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method/types/payment_method_request.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method/types/payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method/types/payment_method_response.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method/types/payment_method_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from ...invoice.types.currency_code import CurrencyCode
 from .bank_account_response import BankAccountResponse
 from .card_response import CardResponse
 from .check_response import CheckResponse
 from .custom_payment_method_response import CustomPaymentMethodResponse
 from .payment_method_id import PaymentMethodId
 from .payment_method_type import PaymentMethodType
 
@@ -17,14 +18,15 @@
 class PaymentMethodResponse(pydantic.BaseModel):
     id: PaymentMethodId
     type: PaymentMethodType
     bank_account: typing.Optional[BankAccountResponse] = pydantic.Field(alias="bankAccount")
     check: typing.Optional[CheckResponse]
     card: typing.Optional[CardResponse]
     custom: typing.Optional[CustomPaymentMethodResponse]
+    supported_currencies: typing.List[CurrencyCode] = pydantic.Field(alias="supportedCurrencies")
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
     updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method/types/payment_method_type.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method/types/payment_method_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method_schema/client.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method_schema/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method_schema/types/__init__.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method_schema/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,26 +2,34 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from ...invoice.types.currency_code import CurrencyCode
 from .payment_method_schema_field import PaymentMethodSchemaField
+from .payment_method_schema_id import PaymentMethodSchemaId
 
 
-class PaymentMethodSchemaRequest(pydantic.BaseModel):
+class PaymentMethodSchemaResponse(pydantic.BaseModel):
+    id: PaymentMethodSchemaId
     name: str
     is_source: bool = pydantic.Field(
         alias="isSource", description=("This payment method can be used as a payment source for an invoice\n")
     )
     is_destination: bool = pydantic.Field(
         alias="isDestination", description=("This payment method can be used as a payment destination for an invoice\n")
     )
+    supported_currencies: typing.List[CurrencyCode] = pydantic.Field(
+        alias="supportedCurrencies", description=("List of currencies that this payment method supports.\n")
+    )
     fields: typing.List[PaymentMethodSchemaField]
+    created_at: dt.datetime = pydantic.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.8/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py` & `mercoa-0.0.9/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,30 +2,33 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from ...invoice.types.currency_code import CurrencyCode
 from .payment_method_schema_field import PaymentMethodSchemaField
-from .payment_method_schema_id import PaymentMethodSchemaId
 
 
-class PaymentMethodSchemaResponse(pydantic.BaseModel):
-    id: PaymentMethodSchemaId
+class PaymentMethodSchemaRequest(pydantic.BaseModel):
     name: str
     is_source: bool = pydantic.Field(
         alias="isSource", description=("This payment method can be used as a payment source for an invoice\n")
     )
     is_destination: bool = pydantic.Field(
         alias="isDestination", description=("This payment method can be used as a payment destination for an invoice\n")
     )
+    supported_currencies: typing.Optional[typing.List[CurrencyCode]] = pydantic.Field(
+        alias="supportedCurrencies",
+        description=(
+            "List of currencies that this payment method supports. If not provided, the payment method will support only USD.\n"
+        ),
+    )
     fields: typing.List[PaymentMethodSchemaField]
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.0.8/src/mercoa/resources/representative/client.py` & `mercoa-0.0.9/src/mercoa/resources/representative/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/representative/types/representative_request.py` & `mercoa-0.0.9/src/mercoa/resources/representative/types/representative_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/representative/types/representative_response.py` & `mercoa-0.0.9/src/mercoa/resources/representative/types/representative_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/transaction/client.py` & `mercoa-0.0.9/src/mercoa/resources/transaction/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import MercoaEnvironment
 from .types.transaction_id import TransactionId
 from .types.transaction_response import TransactionResponse
+from .types.transaction_response_expanded import TransactionResponseExpanded
 
 
 class TransactionClient:
     def __init__(
         self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
@@ -33,28 +34,28 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TransactionResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_all(self) -> typing.List[TransactionResponse]:
+    def get_all(self) -> typing.List[TransactionResponseExpanded]:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "transactions"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[TransactionResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(typing.List[TransactionResponseExpanded], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncTransactionClient:
     def __init__(
         self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
@@ -74,23 +75,23 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(TransactionResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_all(self) -> typing.List[TransactionResponse]:
+    async def get_all(self) -> typing.List[TransactionResponseExpanded]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", "transactions"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[TransactionResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(typing.List[TransactionResponseExpanded], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `mercoa-0.0.8/src/mercoa/resources/transaction/types/transaction_response.py` & `mercoa-0.0.9/src/mercoa/resources/transaction/types/transaction_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/src/mercoa/resources/transaction/types/transaction_status.py` & `mercoa-0.0.9/src/mercoa/resources/transaction/types/transaction_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.0.8/PKG-INFO` & `mercoa-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercoa
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

