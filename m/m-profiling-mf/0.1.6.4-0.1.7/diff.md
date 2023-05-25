# Comparing `tmp/m-profiling-mf-0.1.6.4.tar.gz` & `tmp/m-profiling-mf-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m-profiling-mf-0.1.6.4.tar", last modified: Thu Jan  5 02:33:20 2023, max compression
+gzip compressed data, was "m-profiling-mf-0.1.7.tar", last modified: Thu May 25 09:45:37 2023, max compression
```

## Comparing `m-profiling-mf-0.1.6.4.tar` & `m-profiling-mf-0.1.7.tar`

### file list

```diff
@@ -1,132 +1,135 @@
-drwxrwxr-x   0 giangnth  (1000) giangnth  (1000)        0 2023-01-05 02:33:20.192627 m-profiling-mf-0.1.6.4/
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)     1380 2023-01-05 02:33:20.192627 m-profiling-mf-0.1.6.4/PKG-INFO
--rwxr-xr-x   0 giangnth  (1000) giangnth  (1000)      501 2023-01-05 02:32:22.000000 m-profiling-mf-0.1.6.4/README.md
-drwxrwxr-x   0 giangnth  (1000) giangnth  (1000)        0 2023-01-05 02:33:20.188627 m-profiling-mf-0.1.6.4/m_profiling_mf.egg-info/
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     1380 2023-01-05 02:33:20.000000 m-profiling-mf-0.1.6.4/m_profiling_mf.egg-info/PKG-INFO
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     6678 2023-01-05 02:33:20.000000 m-profiling-mf-0.1.6.4/m_profiling_mf.egg-info/SOURCES.txt
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)        1 2023-01-05 02:33:20.000000 m-profiling-mf-0.1.6.4/m_profiling_mf.egg-info/dependency_links.txt
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      151 2023-01-05 02:33:20.000000 m-profiling-mf-0.1.6.4/m_profiling_mf.egg-info/requires.txt
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      204 2023-01-05 02:33:20.000000 m-profiling-mf-0.1.6.4/m_profiling_mf.egg-info/top_level.txt
-drwxrwxr-x   0 giangnth  (1000) giangnth  (1000)        0 2023-01-05 02:33:20.188627 m-profiling-mf-0.1.6.4/mobio/
-drwxrwxr-x   0 giangnth  (1000) giangnth  (1000)        0 2023-01-05 02:33:20.188627 m-profiling-mf-0.1.6.4/mobio/libs/
-drwxrwxr-x   0 giangnth  (1000) giangnth  (1000)        0 2023-01-05 02:33:20.188627 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     7837 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/__init__.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)    11705 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/common_helper.py
-drwxrwxr-x   0 giangnth  (1000) giangnth  (1000)        0 2023-01-05 02:33:20.192627 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)        0 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/__init__.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     7668 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/base_merge.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     3199 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_address.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      676 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_age.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2199 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_avatar.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2545 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_bank_cards.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      770 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_birth_date.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      771 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_birth_month.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      770 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_birth_year.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2733 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_birthday.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2354 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_budget_high_threshold.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2353 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_budget_low_threshold.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      681 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_card_code.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      679 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_card_id.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      683 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_card_status.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2593 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_cards.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      767 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_childs.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2751 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_cif.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2268 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_clv.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      768 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_company.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      779 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_created_account_type.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2038 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_created_time.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2644 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_customer_created_time.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2382 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_customer_id.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2863 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_degree.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     5669 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_device_types.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     6012 2023-01-05 02:31:21.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_devices.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     3865 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_district_code.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2728 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_driver_license.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     3819 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_dynamic.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2948 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_face_id.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      764 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_fax.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      778 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_frequently_demands.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2279 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_gender.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     5922 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_hobby.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      763 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_id.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2630 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_identify_code.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     1994 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_income_family.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2000 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_income_high_threshold.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2001 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_income_low_threshold.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     1992 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_income_type.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     3192 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_internal_id.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      770 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_is_company.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      773 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_is_non_profile.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      774 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_is_staff_update.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2865 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_isp.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     4160 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_job.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      772 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_last_payment.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     1940 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_lat.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2075 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_lending_limit.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      783 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_list_ignore_social_update.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2016 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_lon.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     4507 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_marital_status.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     3163 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_merchant_id.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2193 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_name.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     4263 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_nation.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      764 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_nth.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      773 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_number_childs.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      691 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_number_transactions.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     4449 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_operation.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     1973 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_partner_point.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2039 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_passport.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     1987 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_password.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      769 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_people_id.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     1986 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_point.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      768 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_predict.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     5158 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_primary_email.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     5195 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_primary_phone.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2640 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_profile_group.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2166 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_profile_id.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     8276 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_profile_identify.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2299 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_profile_owner.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     6756 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_profile_tags.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     3826 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_province_code.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     3070 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_push_id.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     1945 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_rank_point.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      779 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_relation_with_childs.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      777 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_relationship_data.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     4382 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_religiousness.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     1942 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_salary.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     7323 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_secondary_emails.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     7055 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_secondary_phones.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     3688 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_social_name.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      771 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_social_tags.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     5816 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_social_user.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2292 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_source.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      765 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_tags.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      776 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_tags_interactive.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     1935 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_tax_address.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     1932 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_tax_code.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     1956 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_tax_name.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)      779 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_unsub_mobio_email_mkt.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2038 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_updated_time.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2544 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_vib_cards.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     4460 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_ward_code.py
-drwxrwxr-x   0 giangnth  (1000) giangnth  (1000)        0 2023-01-05 02:33:20.192627 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_v2_helpers/
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)        0 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_v2_helpers/__init__.py
-drwxrwxr-x   0 giangnth  (1000) giangnth  (1000)        0 2023-01-05 02:33:20.192627 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_v2_helpers/dynamic_import_module/
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2435 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_v2_helpers/dynamic_import_module/__init__.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     3551 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_common.py
-drwxrwxr-x   0 giangnth  (1000) giangnth  (1000)        0 2023-01-05 02:33:20.192627 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_data/
--rwxr-xr-x   0 giangnth  (1000) giangnth  (1000)        0 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_data/__init__.py
--rwxr-xr-x   0 giangnth  (1000) giangnth  (1000)     1298 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_data/account_type_data.py
--rwxr-xr-x   0 giangnth  (1000) giangnth  (1000)      751 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_data/degree_data.py
--rwxr-xr-x   0 giangnth  (1000) giangnth  (1000)     1171 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_data/frequently_demand_data.py
--rwxr-xr-x   0 giangnth  (1000) giangnth  (1000)      403 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_data/gender_data.py
--rwxr-xr-x   0 giangnth  (1000) giangnth  (1000)    23208 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_data/hobby_data.py
--rwxr-xr-x   0 giangnth  (1000) giangnth  (1000)    11031 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_data/job_data.py
--rwxr-xr-x   0 giangnth  (1000) giangnth  (1000)     1002 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_data/marital_status_data.py
--rwxr-xr-x   0 giangnth  (1000) giangnth  (1000)     4091 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_data/nation_data.py
--rwxr-xr-x   0 giangnth  (1000) giangnth  (1000)     1315 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_data/operation_data.py
--rwxr-xr-x   0 giangnth  (1000) giangnth  (1000)     1873 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_data/question_data.py
--rwxr-xr-x   0 giangnth  (1000) giangnth  (1000)     1874 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_data/religiousness_data.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     8528 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_helper.py
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     3992 2022-10-18 04:43:07.000000 m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_schema.py
--rw-rw-r--   0 giangnth  (1000) giangnth  (1000)       38 2023-01-05 02:33:20.192627 m-profiling-mf-0.1.6.4/setup.cfg
--rw-r--r--   0 giangnth  (1000) giangnth  (1000)     2372 2023-01-05 02:31:40.000000 m-profiling-mf-0.1.6.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 09:45:37.355546 m-profiling-mf-0.1.7/
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-05-25 09:45:37.354546 m-profiling-mf-0.1.7/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)      536 2023-05-25 09:43:55.000000 m-profiling-mf-0.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 09:45:37.192541 m-profiling-mf-0.1.7/m_profiling_mf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-05-25 09:45:36.000000 m-profiling-mf-0.1.7/m_profiling_mf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6763 2023-05-25 09:45:37.000000 m-profiling-mf-0.1.7/m_profiling_mf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 09:45:36.000000 m-profiling-mf-0.1.7/m_profiling_mf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-25 09:45:36.000000 m-profiling-mf-0.1.7/m_profiling_mf.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)      151 2023-05-25 09:45:36.000000 m-profiling-mf-0.1.7/m_profiling_mf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-25 09:45:36.000000 m-profiling-mf-0.1.7/m_profiling_mf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 09:45:37.160541 m-profiling-mf-0.1.7/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 09:45:37.193541 m-profiling-mf-0.1.7/mobio/libs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 09:45:37.198541 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/
+-rw-r--r--   0 root         (0) root         (0)     7837 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11705 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/common_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 09:45:37.337545 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7668 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/base_merge.py
+-rw-r--r--   0 root         (0) root         (0)     3199 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_address.py
+-rw-r--r--   0 root         (0) root         (0)      676 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_age.py
+-rw-r--r--   0 root         (0) root         (0)     2199 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_avatar.py
+-rw-r--r--   0 root         (0) root         (0)     2545 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_bank_cards.py
+-rw-r--r--   0 root         (0) root         (0)      770 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_birth_date.py
+-rw-r--r--   0 root         (0) root         (0)      771 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_birth_month.py
+-rw-r--r--   0 root         (0) root         (0)      770 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_birth_year.py
+-rw-r--r--   0 root         (0) root         (0)     2733 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_birthday.py
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_budget_high_threshold.py
+-rw-r--r--   0 root         (0) root         (0)     2353 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_budget_low_threshold.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_card_code.py
+-rw-r--r--   0 root         (0) root         (0)      679 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_card_id.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_card_status.py
+-rw-r--r--   0 root         (0) root         (0)     2593 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_cards.py
+-rw-r--r--   0 root         (0) root         (0)      767 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_childs.py
+-rw-r--r--   0 root         (0) root         (0)     2751 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_cif.py
+-rw-r--r--   0 root         (0) root         (0)     2268 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_clv.py
+-rw-r--r--   0 root         (0) root         (0)      768 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_company.py
+-rw-r--r--   0 root         (0) root         (0)      779 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_created_account_type.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_created_time.py
+-rw-r--r--   0 root         (0) root         (0)     2644 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_customer_created_time.py
+-rw-r--r--   0 root         (0) root         (0)     2382 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_customer_id.py
+-rw-r--r--   0 root         (0) root         (0)     2863 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_degree.py
+-rw-r--r--   0 root         (0) root         (0)     5669 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_device_types.py
+-rw-r--r--   0 root         (0) root         (0)     6012 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_devices.py
+-rw-r--r--   0 root         (0) root         (0)     3865 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_district_code.py
+-rw-r--r--   0 root         (0) root         (0)     2728 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_driver_license.py
+-rw-r--r--   0 root         (0) root         (0)     3819 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     2948 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_face_id.py
+-rw-r--r--   0 root         (0) root         (0)      764 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_fax.py
+-rw-r--r--   0 root         (0) root         (0)      778 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_frequently_demands.py
+-rw-r--r--   0 root         (0) root         (0)     2279 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_gender.py
+-rw-r--r--   0 root         (0) root         (0)     5922 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_hobby.py
+-rw-r--r--   0 root         (0) root         (0)      763 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_id.py
+-rw-r--r--   0 root         (0) root         (0)     2630 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_identify_code.py
+-rw-r--r--   0 root         (0) root         (0)     1994 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_income_family.py
+-rw-r--r--   0 root         (0) root         (0)     2000 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_income_high_threshold.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_income_low_threshold.py
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_income_type.py
+-rw-r--r--   0 root         (0) root         (0)     3192 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_internal_id.py
+-rw-r--r--   0 root         (0) root         (0)      770 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_is_company.py
+-rw-r--r--   0 root         (0) root         (0)      773 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_is_non_profile.py
+-rw-r--r--   0 root         (0) root         (0)      774 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_is_staff_update.py
+-rw-r--r--   0 root         (0) root         (0)     2865 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_isp.py
+-rw-r--r--   0 root         (0) root         (0)     4160 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_job.py
+-rw-r--r--   0 root         (0) root         (0)      772 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_last_payment.py
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_lat.py
+-rw-r--r--   0 root         (0) root         (0)     2075 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_lending_limit.py
+-rw-r--r--   0 root         (0) root         (0)      783 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_list_ignore_social_update.py
+-rw-r--r--   0 root         (0) root         (0)     2016 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_lon.py
+-rw-r--r--   0 root         (0) root         (0)     4507 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_marital_status.py
+-rw-r--r--   0 root         (0) root         (0)     3163 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_merchant_id.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_name.py
+-rw-r--r--   0 root         (0) root         (0)     4263 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_nation.py
+-rw-r--r--   0 root         (0) root         (0)      764 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_nth.py
+-rw-r--r--   0 root         (0) root         (0)      773 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_number_childs.py
+-rw-r--r--   0 root         (0) root         (0)      691 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_number_transactions.py
+-rw-r--r--   0 root         (0) root         (0)     4449 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_operation.py
+-rw-r--r--   0 root         (0) root         (0)     1973 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_partner_point.py
+-rw-r--r--   0 root         (0) root         (0)     2039 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_passport.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_password.py
+-rw-r--r--   0 root         (0) root         (0)      769 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_people_id.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_point.py
+-rw-r--r--   0 root         (0) root         (0)      768 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_predict.py
+-rw-r--r--   0 root         (0) root         (0)     5158 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_primary_email.py
+-rw-r--r--   0 root         (0) root         (0)     5195 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_primary_phone.py
+-rw-r--r--   0 root         (0) root         (0)     2640 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_profile_group.py
+-rw-r--r--   0 root         (0) root         (0)     2166 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_profile_id.py
+-rw-r--r--   0 root         (0) root         (0)     8276 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_profile_identify.py
+-rw-r--r--   0 root         (0) root         (0)     2299 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_profile_owner.py
+-rw-r--r--   0 root         (0) root         (0)     6756 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_profile_tags.py
+-rw-r--r--   0 root         (0) root         (0)     3826 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_province_code.py
+-rw-r--r--   0 root         (0) root         (0)     3070 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_push_id.py
+-rw-r--r--   0 root         (0) root         (0)     1945 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_rank_point.py
+-rw-r--r--   0 root         (0) root         (0)      779 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_relation_with_childs.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_relationship_data.py
+-rw-r--r--   0 root         (0) root         (0)     4382 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_religiousness.py
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_salary.py
+-rw-r--r--   0 root         (0) root         (0)     7323 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_secondary_emails.py
+-rw-r--r--   0 root         (0) root         (0)     7055 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_secondary_phones.py
+-rw-r--r--   0 root         (0) root         (0)     3688 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_social_name.py
+-rw-r--r--   0 root         (0) root         (0)      771 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_social_tags.py
+-rw-r--r--   0 root         (0) root         (0)     5816 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_social_user.py
+-rw-r--r--   0 root         (0) root         (0)     2292 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_source.py
+-rw-r--r--   0 root         (0) root         (0)      765 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_tags.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_tags_interactive.py
+-rw-r--r--   0 root         (0) root         (0)     1935 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_tax_address.py
+-rw-r--r--   0 root         (0) root         (0)     1932 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_tax_code.py
+-rw-r--r--   0 root         (0) root         (0)     1956 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_tax_name.py
+-rw-r--r--   0 root         (0) root         (0)      779 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_unsub_mobio_email_mkt.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_updated_time.py
+-rw-r--r--   0 root         (0) root         (0)     2544 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_vib_cards.py
+-rw-r--r--   0 root         (0) root         (0)     4460 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_ward_code.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 09:45:37.338545 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_v2_helpers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_v2_helpers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 09:45:37.338545 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_v2_helpers/dynamic_import_module/
+-rw-r--r--   0 root         (0) root         (0)     2435 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_v2_helpers/dynamic_import_module/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3551 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 09:45:37.353546 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_data/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_data/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1298 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_data/account_type_data.py
+-rwxr-xr-x   0 root         (0) root         (0)      751 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_data/degree_data.py
+-rwxr-xr-x   0 root         (0) root         (0)     1171 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_data/frequently_demand_data.py
+-rwxr-xr-x   0 root         (0) root         (0)      403 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_data/gender_data.py
+-rwxr-xr-x   0 root         (0) root         (0)    23208 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_data/hobby_data.py
+-rwxr-xr-x   0 root         (0) root         (0)    11031 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_data/job_data.py
+-rwxr-xr-x   0 root         (0) root         (0)     1002 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_data/marital_status_data.py
+-rwxr-xr-x   0 root         (0) root         (0)     4091 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_data/nation_data.py
+-rwxr-xr-x   0 root         (0) root         (0)     1315 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_data/operation_data.py
+-rwxr-xr-x   0 root         (0) root         (0)     1873 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_data/question_data.py
+-rwxr-xr-x   0 root         (0) root         (0)     1874 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_data/religiousness_data.py
+-rw-r--r--   0 root         (0) root         (0)     8528 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_helper.py
+-rw-r--r--   0 root         (0) root         (0)     3992 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_schema.py
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-25 09:37:37.000000 m-profiling-mf-0.1.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 09:45:37.355546 m-profiling-mf-0.1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9392 2023-05-25 09:45:36.000000 m-profiling-mf-0.1.7/setup.py
```

### Comparing `m-profiling-mf-0.1.6.4/PKG-INFO` & `m-profiling-mf-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: m-profiling-mf
-Version: 0.1.6.4
+Version: 0.1.7
 Summary: Mobio Profiling Management Fields
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
+Project-URL: Source, https://github.com/mobiovn
+Description: - **Thư viện fields của Profiling** :
+          - 0.1.7 upgrade requests library
+          - 0.1.6.4 fix normalized device_id 
+          - 0.1.6.3 upgrade admin_sdk support encrypt data
+          - 0.1.6.1 upgrade admin_sdk
+          - 0.1.6 using admin_sdk
+          - 0.1.5.5 support internal_id
+          - 0.1.5.4 singleton merchant_config
+          - 0.1.5.3 support validate phone_number
+          - 0.1.5.2 update check unification rule
+          - 0.1.5.1 fix profile_tag get update data
+          - 0.1.5 fix marital_status get update data
+          - 0.1.4 fix get UDT support trigger
+          - 0.1.3 remove provinces data
+        
+Keywords: mobio,profiling-mf
 Platform: UNKNOWN
-Classifier: Topic :: Software Development
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3
 Description-Content-Type: text/markdown
-
-- **Thư viện fields của Profiling** :
-  - 0.1.6.4 fix normalized device_id 
-  - 0.1.6.3 upgrade admin_sdk support encrypt data
-  - 0.1.6.1 upgrade admin_sdk
-  - 0.1.6 using admin_sdk
-  - 0.1.5.5 support internal_id
-  - 0.1.5.4 singleton merchant_config
-  - 0.1.5.3 support validate phone_number
-  - 0.1.5.2 update check unification rule
-  - 0.1.5.1 fix profile_tag get update data
-  - 0.1.5 fix marital_status get update data
-  - 0.1.4 fix get UDT support trigger
-  - 0.1.3 remove provinces data
-
-
```

### Comparing `m-profiling-mf-0.1.6.4/m_profiling_mf.egg-info/PKG-INFO` & `m-profiling-mf-0.1.7/m_profiling_mf.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: m-profiling-mf
-Version: 0.1.6.4
+Version: 0.1.7
 Summary: Mobio Profiling Management Fields
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
+Project-URL: Source, https://github.com/mobiovn
+Description: - **Thư viện fields của Profiling** :
+          - 0.1.7 upgrade requests library
+          - 0.1.6.4 fix normalized device_id 
+          - 0.1.6.3 upgrade admin_sdk support encrypt data
+          - 0.1.6.1 upgrade admin_sdk
+          - 0.1.6 using admin_sdk
+          - 0.1.5.5 support internal_id
+          - 0.1.5.4 singleton merchant_config
+          - 0.1.5.3 support validate phone_number
+          - 0.1.5.2 update check unification rule
+          - 0.1.5.1 fix profile_tag get update data
+          - 0.1.5 fix marital_status get update data
+          - 0.1.4 fix get UDT support trigger
+          - 0.1.3 remove provinces data
+        
+Keywords: mobio,profiling-mf
 Platform: UNKNOWN
-Classifier: Topic :: Software Development
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3
 Description-Content-Type: text/markdown
-
-- **Thư viện fields của Profiling** :
-  - 0.1.6.4 fix normalized device_id 
-  - 0.1.6.3 upgrade admin_sdk support encrypt data
-  - 0.1.6.1 upgrade admin_sdk
-  - 0.1.6 using admin_sdk
-  - 0.1.5.5 support internal_id
-  - 0.1.5.4 singleton merchant_config
-  - 0.1.5.3 support validate phone_number
-  - 0.1.5.2 update check unification rule
-  - 0.1.5.1 fix profile_tag get update data
-  - 0.1.5 fix marital_status get update data
-  - 0.1.4 fix get UDT support trigger
-  - 0.1.3 remove provinces data
-
-
```

### Comparing `m-profiling-mf-0.1.6.4/m_profiling_mf.egg-info/SOURCES.txt` & `m-profiling-mf-0.1.7/m_profiling_mf.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 README.md
+pyproject.toml
 setup.py
 m_profiling_mf.egg-info/PKG-INFO
 m_profiling_mf.egg-info/SOURCES.txt
 m_profiling_mf.egg-info/dependency_links.txt
+m_profiling_mf.egg-info/namespace_packages.txt
 m_profiling_mf.egg-info/requires.txt
 m_profiling_mf.egg-info/top_level.txt
+mobio/libs/__init__.py
 mobio/libs/profiling_mf/__init__.py
 mobio/libs/profiling_mf/common_helper.py
 mobio/libs/profiling_mf/profiling_common.py
 mobio/libs/profiling_mf/profiling_helper.py
 mobio/libs/profiling_mf/profiling_schema.py
 mobio/libs/profiling_mf/merge_fields/__init__.py
 mobio/libs/profiling_mf/merge_fields/base_merge.py
```

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/__init__.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/__init__.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/common_helper.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/common_helper.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/base_merge.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/base_merge.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_address.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_address.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_age.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_age.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_avatar.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_avatar.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_bank_cards.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_bank_cards.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_birth_date.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_birth_date.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_birth_month.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_birth_month.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_birth_year.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_birth_year.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_birthday.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_birthday.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_budget_high_threshold.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_budget_high_threshold.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_budget_low_threshold.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_budget_low_threshold.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_card_code.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_card_code.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_card_id.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_card_id.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_card_status.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_card_status.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_cards.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_cards.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_childs.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_childs.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_cif.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_cif.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_clv.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_clv.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_company.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_company.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_created_account_type.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_created_account_type.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_created_time.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_created_time.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_customer_created_time.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_customer_created_time.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_customer_id.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_customer_id.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_degree.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_degree.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_device_types.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_device_types.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_devices.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_devices.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_district_code.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_district_code.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_driver_license.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_driver_license.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_dynamic.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_dynamic.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_face_id.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_face_id.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_fax.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_fax.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_frequently_demands.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_frequently_demands.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_gender.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_gender.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_hobby.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_hobby.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_id.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_id.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_identify_code.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_identify_code.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_income_family.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_income_family.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_income_high_threshold.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_income_high_threshold.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_income_low_threshold.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_income_low_threshold.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_income_type.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_income_type.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_internal_id.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_internal_id.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_is_company.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_is_company.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_is_non_profile.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_is_non_profile.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_is_staff_update.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_is_staff_update.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_isp.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_isp.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_job.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_job.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_last_payment.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_last_payment.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_lat.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_lat.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_lending_limit.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_lending_limit.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_list_ignore_social_update.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_list_ignore_social_update.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_lon.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_lon.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_marital_status.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_marital_status.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_merchant_id.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_merchant_id.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_name.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_name.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_nation.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_nation.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_nth.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_nth.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_number_childs.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_number_childs.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_number_transactions.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_number_transactions.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_operation.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_operation.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_partner_point.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_partner_point.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_passport.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_passport.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_password.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_password.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_people_id.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_people_id.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_point.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_point.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_predict.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_predict.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_primary_email.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_primary_email.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_primary_phone.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_primary_phone.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_profile_group.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_profile_group.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_profile_id.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_profile_id.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_profile_identify.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_profile_identify.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_profile_owner.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_profile_owner.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_profile_tags.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_profile_tags.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_province_code.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_province_code.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_push_id.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_push_id.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_rank_point.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_rank_point.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_relation_with_childs.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_relation_with_childs.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_relationship_data.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_relationship_data.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_religiousness.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_religiousness.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_salary.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_salary.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_secondary_emails.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_secondary_emails.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_secondary_phones.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_secondary_phones.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_social_name.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_social_name.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_social_tags.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_social_tags.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_social_user.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_social_user.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_source.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_source.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_tags.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_tags.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_tags_interactive.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_tags_interactive.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_tax_address.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_tax_address.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_tax_code.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_tax_code.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_tax_name.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_tax_name.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_unsub_mobio_email_mkt.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_unsub_mobio_email_mkt.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_updated_time.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_updated_time.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_vib_cards.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_vib_cards.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_fields/merge_ward_code.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_fields/merge_ward_code.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/merge_v2_helpers/dynamic_import_module/__init__.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/merge_v2_helpers/dynamic_import_module/__init__.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_common.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_common.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_data/account_type_data.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_data/account_type_data.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_data/degree_data.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_data/degree_data.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_data/frequently_demand_data.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_data/frequently_demand_data.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_data/hobby_data.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_data/hobby_data.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_data/job_data.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_data/job_data.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_data/marital_status_data.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_data/marital_status_data.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_data/nation_data.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_data/nation_data.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_data/operation_data.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_data/operation_data.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_data/question_data.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_data/question_data.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_data/religiousness_data.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_data/religiousness_data.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_helper.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_helper.py`

 * *Files identical despite different names*

### Comparing `m-profiling-mf-0.1.6.4/mobio/libs/profiling_mf/profiling_schema.py` & `m-profiling-mf-0.1.7/mobio/libs/profiling_mf/profiling_schema.py`

 * *Files identical despite different names*

