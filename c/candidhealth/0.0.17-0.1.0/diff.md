# Comparing `tmp/candidhealth-0.0.17.tar.gz` & `tmp/candidhealth-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "candidhealth-0.0.17.tar", max compression
+gzip compressed data, was "candidhealth-0.1.0.tar", max compression
```

## Comparing `candidhealth-0.0.17.tar` & `candidhealth-0.1.0.tar`

### file list

```diff
@@ -1,213 +1,236 @@
--rw-r--r--   0        0        0        0 2023-05-22 20:44:14.093702 candidhealth-0.0.17/README.md
--rw-r--r--   0        0        0      374 2023-05-22 20:44:14.093702 candidhealth-0.0.17/pyproject.toml
--rw-r--r--   0        0        0     5433 2023-05-22 20:44:14.093702 candidhealth-0.0.17/src/candid/__init__.py
--rw-r--r--   0        0        0     1688 2023-05-22 20:44:14.093702 candidhealth-0.0.17/src/candid/client.py
--rw-r--r--   0        0        0      348 2023-05-22 20:44:14.093702 candidhealth-0.0.17/src/candid/core/__init__.py
--rw-r--r--   0        0        0      426 2023-05-22 20:44:14.093702 candidhealth-0.0.17/src/candid/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-05-22 20:44:14.093702 candidhealth-0.0.17/src/candid/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-05-22 20:44:14.093702 candidhealth-0.0.17/src/candid/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-05-22 20:44:14.093702 candidhealth-0.0.17/src/candid/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      227 2023-05-22 20:44:14.093702 candidhealth-0.0.17/src/candid/environment.py
--rw-r--r--   0        0        0        0 2023-05-22 20:44:14.093702 candidhealth-0.0.17/src/candid/py.typed
--rw-r--r--   0        0        0     5585 2023-05-22 20:44:14.093702 candidhealth-0.0.17/src/candid/resources/__init__.py
--rw-r--r--   0        0        0      191 2023-05-22 20:44:14.093702 candidhealth-0.0.17/src/candid/resources/billing_notes/__init__.py
--rw-r--r--   0        0        0     2741 2023-05-22 20:44:14.093702 candidhealth-0.0.17/src/candid/resources/billing_notes/client.py
--rw-r--r--   0        0        0      256 2023-05-22 20:44:14.093702 candidhealth-0.0.17/src/candid/resources/billing_notes/types/__init__.py
--rw-r--r--   0        0        0     1136 2023-05-22 20:44:14.093702 candidhealth-0.0.17/src/candid/resources/billing_notes/types/billing_note.py
--rw-r--r--   0        0        0      813 2023-05-22 20:44:14.093702 candidhealth-0.0.17/src/candid/resources/billing_notes/types/billing_note_base.py
--rw-r--r--   0        0        0      104 2023-05-22 20:44:14.093702 candidhealth-0.0.17/src/candid/resources/billing_notes/types/billing_note_id.py
--rw-r--r--   0        0        0      139 2023-05-22 20:44:14.093702 candidhealth-0.0.17/src/candid/resources/claims/__init__.py
--rw-r--r--   0        0        0      164 2023-05-22 20:44:14.093702 candidhealth-0.0.17/src/candid/resources/claims/types/__init__.py
--rw-r--r--   0        0        0     1151 2023-05-22 20:44:14.093702 candidhealth-0.0.17/src/candid/resources/claims/types/claim.py
--rw-r--r--   0        0        0     2605 2023-05-22 20:44:14.093702 candidhealth-0.0.17/src/candid/resources/claims/types/claim_status.py
--rw-r--r--   0        0        0     1241 2023-05-22 20:44:14.093702 candidhealth-0.0.17/src/candid/resources/commons/__init__.py
--rw-r--r--   0        0        0     1824 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/__init__.py
--rw-r--r--   0        0        0       98 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/claim_id.py
--rw-r--r--   0        0        0       90 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/content_download_url.py
--rw-r--r--   0        0        0       76 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/date.py
--rw-r--r--   0        0        0       91 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/encounter_external_id.py
--rw-r--r--   0        0        0      102 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/encounter_id.py
--rw-r--r--   0        0        0    11148 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/facility_type_code.py
--rw-r--r--   0        0        0    15447 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/insurance_type_code.py
--rw-r--r--   0        0        0       79 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/link_url.py
--rw-r--r--   0        0        0       75 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/npi.py
--rw-r--r--   0        0        0      105 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/organization_id.py
--rw-r--r--   0        0        0       81 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/page_token.py
--rw-r--r--   0        0        0       89 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/patient_external_id.py
--rw-r--r--   0        0        0     4686 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py
--rw-r--r--   0        0        0    79514 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/procedure_modifier.py
--rw-r--r--   0        0        0      735 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/region_national.py
--rw-r--r--   0        0        0      790 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/region_states.py
--rw-r--r--   0        0        0      722 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/regions.py
--rw-r--r--   0        0        0      864 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/resource_page.py
--rw-r--r--   0        0        0      104 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/service_line_id.py
--rw-r--r--   0        0        0      432 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/service_line_units.py
--rw-r--r--   0        0        0     5065 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/source_of_payment_code.py
--rw-r--r--   0        0        0     6264 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/state.py
--rw-r--r--   0        0        0     1037 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/street_address_base.py
--rw-r--r--   0        0        0      985 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/street_address_long_zip.py
--rw-r--r--   0        0        0     1003 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/commons/types/street_address_short_zip.py
--rw-r--r--   0        0        0      251 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/contracts/__init__.py
--rw-r--r--   0        0        0      365 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/contracts/types/__init__.py
--rw-r--r--   0        0        0      940 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/contracts/types/authorized_signatory.py
--rw-r--r--   0        0        0     1430 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/contracts/types/contract.py
--rw-r--r--   0        0        0     1517 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/contracts/types/contract_base.py
--rw-r--r--   0        0        0      101 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/contracts/types/contract_id.py
--rw-r--r--   0        0        0      986 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/contracts/types/contract_status.py
--rw-r--r--   0        0        0     1125 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/credentialing/__init__.py
--rw-r--r--   0        0        0     1472 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/credentialing/types/__init__.py
--rw-r--r--   0        0        0      886 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/credentialing/types/credentialed_encounter_status_result.py
--rw-r--r--   0        0        0      940 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/credentialing/types/credentialing_span_dates.py
--rw-r--r--   0        0        0      977 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/credentialing/types/credentialing_span_status.py
--rw-r--r--   0        0        0      881 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/credentialing/types/encounter_credentialing_status_result.py
--rw-r--r--   0        0        0      864 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/credentialing/types/non_required_credentialing_dates.py
--rw-r--r--   0        0        0     2210 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/credentialing/types/provider_credentialing_span.py
--rw-r--r--   0        0        0      958 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/credentialing/types/provider_credentialing_span_base.py
--rw-r--r--   0        0        0      118 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/credentialing/types/provider_credentialing_span_id.py
--rw-r--r--   0        0        0      827 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/credentialing/types/required_credentialing_dates.py
--rw-r--r--   0        0        0      279 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/diagnoses/__init__.py
--rw-r--r--   0        0        0      409 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/diagnoses/types/__init__.py
--rw-r--r--   0        0        0      958 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/diagnoses/types/diagnosis.py
--rw-r--r--   0        0        0     1904 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/diagnoses/types/diagnosis_create.py
--rw-r--r--   0        0        0      102 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/diagnoses/types/diagnosis_id.py
--rw-r--r--   0        0        0     1974 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/diagnoses/types/diagnosis_type_code.py
--rw-r--r--   0        0        0      903 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py
--rw-r--r--   0        0        0      111 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounter_providers/__init__.py
--rw-r--r--   0        0        0      102 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounter_providers/resources/__init__.py
--rw-r--r--   0        0        0      381 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounter_providers/resources/v_2/__init__.py
--rw-r--r--   0        0        0      516 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0     1988 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py
--rw-r--r--   0        0        0     1092 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py
--rw-r--r--   0        0        0     1284 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py
--rw-r--r--   0        0        0      101 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounter_providers/resources/v_2/types/provider_id.py
--rw-r--r--   0        0        0     1244 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py
--rw-r--r--   0        0        0     1244 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py
--rw-r--r--   0        0        0      111 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/__init__.py
--rw-r--r--   0        0        0      741 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/client.py
--rw-r--r--   0        0        0      102 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/__init__.py
--rw-r--r--   0        0        0     2507 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/__init__.py
--rw-r--r--   0        0        0    30911 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/client.py
--rw-r--r--   0        0        0     3652 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/__init__.py
--rw-r--r--   0        0        0      103 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/attachment_id.py
--rw-r--r--   0        0        0     1314 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/attributable_contracting_status_result.py
--rw-r--r--   0        0        0      944 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/base_attachment.py
--rw-r--r--   0        0        0      874 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/clinical_note.py
--rw-r--r--   0        0        0      944 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/clinical_note_category.py
--rw-r--r--   0        0        0      894 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/clinical_note_category_create.py
--rw-r--r--   0        0        0      659 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/coding_attribution_type.py
--rw-r--r--   0        0        0      713 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/contracting_out_of_of_network_reason.py
--rw-r--r--   0        0        0     2879 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/encounter.py
--rw-r--r--   0        0        0      920 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/encounter_attachment.py
--rw-r--r--   0        0        0      388 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/encounter_attachment_type.py
--rw-r--r--   0        0        0     4498 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/encounter_base.py
--rw-r--r--   0        0        0      885 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/encounter_page.py
--rw-r--r--   0        0        0     1025 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/encounter_sort_options.py
--rw-r--r--   0        0        0      659 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/generate_clinical_notes_pdf_response.py
--rw-r--r--   0        0        0      855 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/in_network_contracting_status_result.py
--rw-r--r--   0        0        0      845 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/intake_follow_up.py
--rw-r--r--   0        0        0       88 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/intake_follow_up_id.py
--rw-r--r--   0        0        0      969 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/intake_question.py
--rw-r--r--   0        0        0       88 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/intake_question_id.py
--rw-r--r--   0        0        0      891 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/intake_response_and_follow_ups.py
--rw-r--r--   0        0        0     1303 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/intervention.py
--rw-r--r--   0        0        0      865 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/intervention_category.py
--rw-r--r--   0        0        0      855 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/lab.py
--rw-r--r--   0        0        0      457 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/lab_code_type.py
--rw-r--r--   0        0        0      834 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/mark_as_not_billable_response.py
--rw-r--r--   0        0        0      953 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/medication.py
--rw-r--r--   0        0        0      880 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/network_status.py
--rw-r--r--   0        0        0     1164 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/network_status_computation_results.py
--rw-r--r--   0        0        0     2615 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/note_category.py
--rw-r--r--   0        0        0      900 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/out_of_network_contracting_status_result.py
--rw-r--r--   0        0        0     1012 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/patient_history_category.py
--rw-r--r--   0        0        0      885 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/patient_history_category_enum.py
--rw-r--r--   0        0        0       96 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/prior_authorization_number.py
--rw-r--r--   0        0        0       77 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/rx_cui.py
--rw-r--r--   0        0        0      898 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/successful_generate_clinical_notes_pdf_response.py
--rw-r--r--   0        0        0      544 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/synchronicity_type.py
--rw-r--r--   0        0        0      893 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/vitals.py
--rw-r--r--   0        0        0      143 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/era/__init__.py
--rw-r--r--   0        0        0      181 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/era/types/__init__.py
--rw-r--r--   0        0        0      817 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/era/types/era.py
--rw-r--r--   0        0        0      811 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/era/types/era_base.py
--rw-r--r--   0        0        0       96 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/era/types/era_id.py
--rw-r--r--   0        0        0      207 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/expected_network_status/__init__.py
--rw-r--r--   0        0        0     5471 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/expected_network_status/client.py
--rw-r--r--   0        0        0      270 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/expected_network_status/types/__init__.py
--rw-r--r--   0        0        0      729 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/expected_network_status/types/expected_network_status.py
--rw-r--r--   0        0        0      981 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/expected_network_status/types/expected_network_status_response.py
--rw-r--r--   0        0        0      399 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/individual/__init__.py
--rw-r--r--   0        0        0      545 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/individual/types/__init__.py
--rw-r--r--   0        0        0      871 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/individual/types/gender.py
--rw-r--r--   0        0        0      821 2023-05-22 20:44:14.097702 candidhealth-0.0.17/src/candid/resources/individual/types/individual_base.py
--rw-r--r--   0        0        0      103 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/individual/types/individual_id.py
--rw-r--r--   0        0        0      867 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/individual/types/patient.py
--rw-r--r--   0        0        0     1515 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/individual/types/patient_create.py
--rw-r--r--   0        0        0      972 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/individual/types/subscriber.py
--rw-r--r--   0        0        0     1200 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/individual/types/subscriber_base.py
--rw-r--r--   0        0        0      925 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/individual/types/subscriber_create.py
--rw-r--r--   0        0        0      247 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/insurance_card/__init__.py
--rw-r--r--   0        0        0      352 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/insurance_card/types/__init__.py
--rw-r--r--   0        0        0     1106 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/insurance_card/types/insurance_card.py
--rw-r--r--   0        0        0     1122 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/insurance_card/types/insurance_card_base.py
--rw-r--r--   0        0        0     1026 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/insurance_card/types/insurance_card_create.py
--rw-r--r--   0        0        0      106 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/insurance_card/types/insurance_card_id.py
--rw-r--r--   0        0        0      199 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/invoices/__init__.py
--rw-r--r--   0        0        0      276 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/invoices/types/__init__.py
--rw-r--r--   0        0        0     1397 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/invoices/types/invoice.py
--rw-r--r--   0        0        0      100 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/invoices/types/invoice_id.py
--rw-r--r--   0        0        0      849 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/invoices/types/invoice_item.py
--rw-r--r--   0        0        0      908 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/invoices/types/invoice_status.py
--rw-r--r--   0        0        0      111 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/organization_providers/__init__.py
--rw-r--r--   0        0        0      102 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/organization_providers/resources/__init__.py
--rw-r--r--   0        0        0      501 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/organization_providers/resources/v_2/__init__.py
--rw-r--r--   0        0        0      704 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/organization_providers/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0      334 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/organization_providers/resources/v_2/types/address_type.py
--rw-r--r--   0        0        0      492 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/organization_providers/resources/v_2/types/employment_status.py
--rw-r--r--   0        0        0     2857 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/organization_providers/resources/v_2/types/license_type.py
--rw-r--r--   0        0        0     1562 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/organization_providers/resources/v_2/types/organization_provider.py
--rw-r--r--   0        0        0     1062 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py
--rw-r--r--   0        0        0     2853 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_base.py
--rw-r--r--   0        0        0      113 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_id.py
--rw-r--r--   0        0        0      510 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/organization_providers/resources/v_2/types/provider_type.py
--rw-r--r--   0        0        0      111 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/patient_payments/__init__.py
--rw-r--r--   0        0        0      102 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/patient_payments/resources/__init__.py
--rw-r--r--   0        0        0      259 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/patient_payments/resources/v_2/__init__.py
--rw-r--r--   0        0        0      370 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/patient_payments/resources/v_2/types/__init__.py
--rw-r--r--   0        0        0     1648 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/patient_payments/resources/v_2/types/patient_payment.py
--rw-r--r--   0        0        0       88 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_id.py
--rw-r--r--   0        0        0     2035 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_source.py
--rw-r--r--   0        0        0     2055 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_status.py
--rw-r--r--   0        0        0      135 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/payers/__init__.py
--rw-r--r--   0        0        0     4633 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/payers/client.py
--rw-r--r--   0        0        0      158 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/payers/types/__init__.py
--rw-r--r--   0        0        0     1043 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/payers/types/payer.py
--rw-r--r--   0        0        0      865 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/payers/types/payer_page.py
--rw-r--r--   0        0        0      251 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/service_facility/__init__.py
--rw-r--r--   0        0        0      348 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/service_facility/types/__init__.py
--rw-r--r--   0        0        0      975 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/service_facility/types/encounter_service_facility.py
--rw-r--r--   0        0        0     1574 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/service_facility/types/encounter_service_facility_base.py
--rw-r--r--   0        0        0      108 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/service_facility/types/service_facility_id.py
--rw-r--r--   0        0        0      671 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/service_lines/__init__.py
--rw-r--r--   0        0        0      978 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/service_lines/types/__init__.py
--rw-r--r--   0        0        0     6559 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/service_lines/types/denial_reason_content.py
--rw-r--r--   0        0        0     1104 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/service_lines/types/drug_identification.py
--rw-r--r--   0        0        0      996 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/service_lines/types/measurement_unit_code.py
--rw-r--r--   0        0        0     1659 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/service_lines/types/service_id_qualifier.py
--rw-r--r--   0        0        0     1144 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/service_lines/types/service_line.py
--rw-r--r--   0        0        0      960 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/service_lines/types/service_line_adjustment.py
--rw-r--r--   0        0        0      866 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/service_lines/types/service_line_base.py
--rw-r--r--   0        0        0     1899 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/service_lines/types/service_line_base_with_optionals.py
--rw-r--r--   0        0        0     1601 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/service_lines/types/service_line_create.py
--rw-r--r--   0        0        0     1099 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/service_lines/types/service_line_denial_reason.py
--rw-r--r--   0        0        0      917 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/service_lines/types/service_line_era_data.py
--rw-r--r--   0        0        0      177 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/tags/__init__.py
--rw-r--r--   0        0        0      244 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/tags/types/__init__.py
--rw-r--r--   0        0        0      799 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/tags/types/tag.py
--rw-r--r--   0        0        0     1527 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/tags/types/tag_color_enum.py
--rw-r--r--   0        0        0      861 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/tags/types/tag_create.py
--rw-r--r--   0        0        0       77 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/tags/types/tag_id.py
--rw-r--r--   0        0        0      113 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/tasks/__init__.py
--rw-r--r--   0        0        0      115 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/tasks/types/__init__.py
--rw-r--r--   0        0        0       97 2023-05-22 20:44:14.101702 candidhealth-0.0.17/src/candid/resources/tasks/types/task_id.py
--rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 candidhealth-0.0.17/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-25 18:31:54.583160 candidhealth-0.1.0/README.md
+-rw-r--r--   0        0        0      373 2023-05-25 18:31:54.583160 candidhealth-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5601 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/__init__.py
+-rw-r--r--   0        0        0     2009 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/client.py
+-rw-r--r--   0        0        0      348 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      227 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/environment.py
+-rw-r--r--   0        0        0        0 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/py.typed
+-rw-r--r--   0        0        0     5767 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/__init__.py
+-rw-r--r--   0        0        0      111 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/auth/__init__.py
+-rw-r--r--   0        0        0      820 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/auth/client.py
+-rw-r--r--   0        0        0      102 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/auth/resources/__init__.py
+-rw-r--r--   0        0        0      304 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/auth/resources/v_2/__init__.py
+-rw-r--r--   0        0        0     3502 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/auth/resources/v_2/client.py
+-rw-r--r--   0        0        0      159 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/auth/resources/v_2/errors/__init__.py
+-rw-r--r--   0        0        0      330 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/auth/resources/v_2/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      333 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/auth/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0      785 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_request.py
+-rw-r--r--   0        0        0      806 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/auth/resources/v_2/types/auth_get_token_response.py
+-rw-r--r--   0        0        0      765 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/auth/resources/v_2/types/too_many_requests_error_type.py
+-rw-r--r--   0        0        0      191 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/billing_notes/__init__.py
+-rw-r--r--   0        0        0     2831 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/billing_notes/client.py
+-rw-r--r--   0        0        0      256 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/billing_notes/types/__init__.py
+-rw-r--r--   0        0        0     1136 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/billing_notes/types/billing_note.py
+-rw-r--r--   0        0        0      813 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/billing_notes/types/billing_note_base.py
+-rw-r--r--   0        0        0      104 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/billing_notes/types/billing_note_id.py
+-rw-r--r--   0        0        0      139 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/claims/__init__.py
+-rw-r--r--   0        0        0      164 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/claims/types/__init__.py
+-rw-r--r--   0        0        0     1151 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/claims/types/claim.py
+-rw-r--r--   0        0        0     2605 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/claims/types/claim_status.py
+-rw-r--r--   0        0        0     1305 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/commons/__init__.py
+-rw-r--r--   0        0        0     1928 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0       79 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/commons/types/auth_0_id.py
+-rw-r--r--   0        0        0       98 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/commons/types/claim_id.py
+-rw-r--r--   0        0        0       90 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/commons/types/content_download_url.py
+-rw-r--r--   0        0        0       76 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/commons/types/date.py
+-rw-r--r--   0        0        0       91 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/commons/types/encounter_external_id.py
+-rw-r--r--   0        0        0      102 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/commons/types/encounter_id.py
+-rw-r--r--   0        0        0    11148 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/commons/types/facility_type_code.py
+-rw-r--r--   0        0        0    15447 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/commons/types/insurance_type_code.py
+-rw-r--r--   0        0        0       79 2023-05-25 18:31:54.583160 candidhealth-0.1.0/src/candid/resources/commons/types/link_url.py
+-rw-r--r--   0        0        0       75 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/npi.py
+-rw-r--r--   0        0        0      105 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/organization_id.py
+-rw-r--r--   0        0        0       81 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/page_token.py
+-rw-r--r--   0        0        0       89 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/patient_external_id.py
+-rw-r--r--   0        0        0     4686 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py
+-rw-r--r--   0        0        0    79514 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/procedure_modifier.py
+-rw-r--r--   0        0        0      735 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/region_national.py
+-rw-r--r--   0        0        0      790 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/region_states.py
+-rw-r--r--   0        0        0      722 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/regions.py
+-rw-r--r--   0        0        0      864 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/resource_page.py
+-rw-r--r--   0        0        0      104 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/service_line_id.py
+-rw-r--r--   0        0        0      432 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/service_line_units.py
+-rw-r--r--   0        0        0     5065 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/source_of_payment_code.py
+-rw-r--r--   0        0        0     6264 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/state.py
+-rw-r--r--   0        0        0     1037 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/street_address_base.py
+-rw-r--r--   0        0        0      985 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/street_address_long_zip.py
+-rw-r--r--   0        0        0     1003 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/street_address_short_zip.py
+-rw-r--r--   0        0        0       83 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/commons/types/work_queue_id.py
+-rw-r--r--   0        0        0      251 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/contracts/__init__.py
+-rw-r--r--   0        0        0      365 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/contracts/types/__init__.py
+-rw-r--r--   0        0        0      940 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/contracts/types/authorized_signatory.py
+-rw-r--r--   0        0        0     1430 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/contracts/types/contract.py
+-rw-r--r--   0        0        0     1517 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/contracts/types/contract_base.py
+-rw-r--r--   0        0        0      101 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/contracts/types/contract_id.py
+-rw-r--r--   0        0        0      986 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/contracts/types/contract_status.py
+-rw-r--r--   0        0        0     1125 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/credentialing/__init__.py
+-rw-r--r--   0        0        0     1472 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/credentialing/types/__init__.py
+-rw-r--r--   0        0        0      886 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/credentialing/types/credentialed_encounter_status_result.py
+-rw-r--r--   0        0        0      940 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/credentialing/types/credentialing_span_dates.py
+-rw-r--r--   0        0        0      977 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/credentialing/types/credentialing_span_status.py
+-rw-r--r--   0        0        0      881 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/credentialing/types/encounter_credentialing_status_result.py
+-rw-r--r--   0        0        0      864 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/credentialing/types/non_required_credentialing_dates.py
+-rw-r--r--   0        0        0     2210 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/credentialing/types/provider_credentialing_span.py
+-rw-r--r--   0        0        0      958 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/credentialing/types/provider_credentialing_span_base.py
+-rw-r--r--   0        0        0      118 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/credentialing/types/provider_credentialing_span_id.py
+-rw-r--r--   0        0        0      827 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/credentialing/types/required_credentialing_dates.py
+-rw-r--r--   0        0        0      279 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/diagnoses/__init__.py
+-rw-r--r--   0        0        0      409 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/diagnoses/types/__init__.py
+-rw-r--r--   0        0        0      958 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/diagnoses/types/diagnosis.py
+-rw-r--r--   0        0        0     1904 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/diagnoses/types/diagnosis_create.py
+-rw-r--r--   0        0        0      102 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/diagnoses/types/diagnosis_id.py
+-rw-r--r--   0        0        0     1974 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/diagnoses/types/diagnosis_type_code.py
+-rw-r--r--   0        0        0      903 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py
+-rw-r--r--   0        0        0      111 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounter_providers/__init__.py
+-rw-r--r--   0        0        0      102 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/__init__.py
+-rw-r--r--   0        0        0      381 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/__init__.py
+-rw-r--r--   0        0        0      516 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0     1988 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py
+-rw-r--r--   0        0        0     1092 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py
+-rw-r--r--   0        0        0     1284 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py
+-rw-r--r--   0        0        0      101 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/provider_id.py
+-rw-r--r--   0        0        0     1244 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py
+-rw-r--r--   0        0        0     1244 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py
+-rw-r--r--   0        0        0      111 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/__init__.py
+-rw-r--r--   0        0        0      832 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/client.py
+-rw-r--r--   0        0        0      102 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/__init__.py
+-rw-r--r--   0        0        0     2507 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/__init__.py
+-rw-r--r--   0        0        0    31263 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/client.py
+-rw-r--r--   0        0        0     3652 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/__init__.py
+-rw-r--r--   0        0        0      103 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/attachment_id.py
+-rw-r--r--   0        0        0     1314 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/attributable_contracting_status_result.py
+-rw-r--r--   0        0        0      944 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/base_attachment.py
+-rw-r--r--   0        0        0      874 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/clinical_note.py
+-rw-r--r--   0        0        0      944 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category.py
+-rw-r--r--   0        0        0      894 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category_create.py
+-rw-r--r--   0        0        0      659 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/coding_attribution_type.py
+-rw-r--r--   0        0        0      713 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/contracting_out_of_of_network_reason.py
+-rw-r--r--   0        0        0     2992 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/encounter.py
+-rw-r--r--   0        0        0      920 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/encounter_attachment.py
+-rw-r--r--   0        0        0      388 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/encounter_attachment_type.py
+-rw-r--r--   0        0        0     4498 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/encounter_base.py
+-rw-r--r--   0        0        0      885 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/encounter_page.py
+-rw-r--r--   0        0        0     1025 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/encounter_sort_options.py
+-rw-r--r--   0        0        0      659 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/generate_clinical_notes_pdf_response.py
+-rw-r--r--   0        0        0      855 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/in_network_contracting_status_result.py
+-rw-r--r--   0        0        0      845 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up.py
+-rw-r--r--   0        0        0       88 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up_id.py
+-rw-r--r--   0        0        0      969 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intake_question.py
+-rw-r--r--   0        0        0       88 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intake_question_id.py
+-rw-r--r--   0        0        0      891 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intake_response_and_follow_ups.py
+-rw-r--r--   0        0        0     1303 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intervention.py
+-rw-r--r--   0        0        0      865 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intervention_category.py
+-rw-r--r--   0        0        0      855 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/lab.py
+-rw-r--r--   0        0        0      457 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/lab_code_type.py
+-rw-r--r--   0        0        0      834 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/mark_as_not_billable_response.py
+-rw-r--r--   0        0        0      953 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/medication.py
+-rw-r--r--   0        0        0      880 2023-05-25 18:31:54.587161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/network_status.py
+-rw-r--r--   0        0        0     1164 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/network_status_computation_results.py
+-rw-r--r--   0        0        0     2615 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/note_category.py
+-rw-r--r--   0        0        0      900 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/out_of_network_contracting_status_result.py
+-rw-r--r--   0        0        0     1012 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category.py
+-rw-r--r--   0        0        0      885 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category_enum.py
+-rw-r--r--   0        0        0       96 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/prior_authorization_number.py
+-rw-r--r--   0        0        0       77 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/rx_cui.py
+-rw-r--r--   0        0        0      898 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/successful_generate_clinical_notes_pdf_response.py
+-rw-r--r--   0        0        0      544 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/synchronicity_type.py
+-rw-r--r--   0        0        0      893 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/vitals.py
+-rw-r--r--   0        0        0      143 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/era/__init__.py
+-rw-r--r--   0        0        0      181 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/era/types/__init__.py
+-rw-r--r--   0        0        0      817 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/era/types/era.py
+-rw-r--r--   0        0        0      811 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/era/types/era_base.py
+-rw-r--r--   0        0        0       96 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/era/types/era_id.py
+-rw-r--r--   0        0        0      207 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/expected_network_status/__init__.py
+-rw-r--r--   0        0        0     5547 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/expected_network_status/client.py
+-rw-r--r--   0        0        0      270 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/expected_network_status/types/__init__.py
+-rw-r--r--   0        0        0      729 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/expected_network_status/types/expected_network_status.py
+-rw-r--r--   0        0        0      981 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/expected_network_status/types/expected_network_status_response.py
+-rw-r--r--   0        0        0      399 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/individual/__init__.py
+-rw-r--r--   0        0        0      545 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/individual/types/__init__.py
+-rw-r--r--   0        0        0      871 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/individual/types/gender.py
+-rw-r--r--   0        0        0      821 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/individual/types/individual_base.py
+-rw-r--r--   0        0        0      103 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/individual/types/individual_id.py
+-rw-r--r--   0        0        0      867 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/individual/types/patient.py
+-rw-r--r--   0        0        0     1515 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/individual/types/patient_create.py
+-rw-r--r--   0        0        0      972 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/individual/types/subscriber.py
+-rw-r--r--   0        0        0     1200 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/individual/types/subscriber_base.py
+-rw-r--r--   0        0        0      925 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/individual/types/subscriber_create.py
+-rw-r--r--   0        0        0      247 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/insurance_card/__init__.py
+-rw-r--r--   0        0        0      352 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/insurance_card/types/__init__.py
+-rw-r--r--   0        0        0     1106 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/insurance_card/types/insurance_card.py
+-rw-r--r--   0        0        0     1122 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/insurance_card/types/insurance_card_base.py
+-rw-r--r--   0        0        0     1026 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/insurance_card/types/insurance_card_create.py
+-rw-r--r--   0        0        0      106 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/insurance_card/types/insurance_card_id.py
+-rw-r--r--   0        0        0      199 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/invoices/__init__.py
+-rw-r--r--   0        0        0      276 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/invoices/types/__init__.py
+-rw-r--r--   0        0        0     1397 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/invoices/types/invoice.py
+-rw-r--r--   0        0        0      100 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/invoices/types/invoice_id.py
+-rw-r--r--   0        0        0      849 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/invoices/types/invoice_item.py
+-rw-r--r--   0        0        0      908 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/invoices/types/invoice_status.py
+-rw-r--r--   0        0        0      111 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/__init__.py
+-rw-r--r--   0        0        0      102 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/resources/__init__.py
+-rw-r--r--   0        0        0      501 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/__init__.py
+-rw-r--r--   0        0        0      704 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0      334 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/address_type.py
+-rw-r--r--   0        0        0      492 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/employment_status.py
+-rw-r--r--   0        0        0     2857 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/license_type.py
+-rw-r--r--   0        0        0     1562 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider.py
+-rw-r--r--   0        0        0     1062 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py
+-rw-r--r--   0        0        0     2853 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_base.py
+-rw-r--r--   0        0        0      113 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_id.py
+-rw-r--r--   0        0        0      510 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/provider_type.py
+-rw-r--r--   0        0        0      111 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/patient_payments/__init__.py
+-rw-r--r--   0        0        0      102 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/patient_payments/resources/__init__.py
+-rw-r--r--   0        0        0      259 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/patient_payments/resources/v_2/__init__.py
+-rw-r--r--   0        0        0      370 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/patient_payments/resources/v_2/types/__init__.py
+-rw-r--r--   0        0        0     1648 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/patient_payments/resources/v_2/types/patient_payment.py
+-rw-r--r--   0        0        0       88 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_id.py
+-rw-r--r--   0        0        0     2035 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_source.py
+-rw-r--r--   0        0        0     2055 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_status.py
+-rw-r--r--   0        0        0      135 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/payers/__init__.py
+-rw-r--r--   0        0        0     4709 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/payers/client.py
+-rw-r--r--   0        0        0      158 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/payers/types/__init__.py
+-rw-r--r--   0        0        0     1043 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/payers/types/payer.py
+-rw-r--r--   0        0        0      865 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/payers/types/payer_page.py
+-rw-r--r--   0        0        0      251 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_facility/__init__.py
+-rw-r--r--   0        0        0      348 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_facility/types/__init__.py
+-rw-r--r--   0        0        0      975 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_facility/types/encounter_service_facility.py
+-rw-r--r--   0        0        0     1574 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_facility/types/encounter_service_facility_base.py
+-rw-r--r--   0        0        0      108 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_facility/types/service_facility_id.py
+-rw-r--r--   0        0        0      671 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_lines/__init__.py
+-rw-r--r--   0        0        0      978 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_lines/types/__init__.py
+-rw-r--r--   0        0        0     6559 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_lines/types/denial_reason_content.py
+-rw-r--r--   0        0        0     1104 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_lines/types/drug_identification.py
+-rw-r--r--   0        0        0      996 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_lines/types/measurement_unit_code.py
+-rw-r--r--   0        0        0     1659 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_lines/types/service_id_qualifier.py
+-rw-r--r--   0        0        0     1144 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line.py
+-rw-r--r--   0        0        0      960 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_adjustment.py
+-rw-r--r--   0        0        0      866 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_base.py
+-rw-r--r--   0        0        0     1899 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_base_with_optionals.py
+-rw-r--r--   0        0        0     1618 2023-05-25 18:31:54.591161 candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_create.py
+-rw-r--r--   0        0        0     1099 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_denial_reason.py
+-rw-r--r--   0        0        0      917 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_era_data.py
+-rw-r--r--   0        0        0      177 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/tags/__init__.py
+-rw-r--r--   0        0        0      244 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/tags/types/__init__.py
+-rw-r--r--   0        0        0      799 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/tags/types/tag.py
+-rw-r--r--   0        0        0     1527 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/tags/types/tag_color_enum.py
+-rw-r--r--   0        0        0      861 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/tags/types/tag_create.py
+-rw-r--r--   0        0        0       77 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/tags/types/tag_id.py
+-rw-r--r--   0        0        0      113 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/tasks/__init__.py
+-rw-r--r--   0        0        0      115 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/tasks/types/__init__.py
+-rw-r--r--   0        0        0       97 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/tasks/types/task_id.py
+-rw-r--r--   0        0        0      109 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/users/__init__.py
+-rw-r--r--   0        0        0      108 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/users/types/__init__.py
+-rw-r--r--   0        0        0      916 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/users/types/user.py
+-rw-r--r--   0        0        0      111 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/work_queues/__init__.py
+-rw-r--r--   0        0        0      102 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/work_queues/resources/__init__.py
+-rw-r--r--   0        0        0      207 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/work_queues/resources/v_1/__init__.py
+-rw-r--r--   0        0        0      281 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/work_queues/resources/v_1/types/__init__.py
+-rw-r--r--   0        0        0     1052 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/work_queues/resources/v_1/types/work_queue.py
+-rw-r--r--   0        0        0      893 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/work_queues/resources/v_1/types/work_queue_category.py
+-rw-r--r--   0        0        0     1242 2023-05-25 18:31:54.595161 candidhealth-0.1.0/src/candid/resources/work_queues/resources/v_1/types/work_queue_category_type.py
+-rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 candidhealth-0.1.0/PKG-INFO
```

### Comparing `candidhealth-0.0.17/src/candid/__init__.py` & `candidhealth-0.1.0/src/candid/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .environment import CandidApiEnvironment
 from .resources import (
+    Auth0Id,
     AuthorizedSignatory,
     BillingNote,
     BillingNoteBase,
     BillingNoteId,
     Claim,
     ClaimId,
     ClaimStatus,
@@ -95,14 +96,17 @@
     SubscriberBase,
     SubscriberCreate,
     Tag,
     TagColorEnum,
     TagCreate,
     TagId,
     TaskId,
+    User,
+    WorkQueueId,
+    auth,
     billing_notes,
     claims,
     commons,
     contracts,
     credentialing,
     diagnoses,
     encounter_providers,
@@ -115,17 +119,20 @@
     organization_providers,
     patient_payments,
     payers,
     service_facility,
     service_lines,
     tags,
     tasks,
+    users,
+    work_queues,
 )
 
 __all__ = [
+    "Auth0Id",
     "AuthorizedSignatory",
     "BillingNote",
     "BillingNoteBase",
     "BillingNoteId",
     "CandidApiEnvironment",
     "Claim",
     "ClaimId",
@@ -216,14 +223,17 @@
     "SubscriberBase",
     "SubscriberCreate",
     "Tag",
     "TagColorEnum",
     "TagCreate",
     "TagId",
     "TaskId",
+    "User",
+    "WorkQueueId",
+    "auth",
     "billing_notes",
     "claims",
     "commons",
     "contracts",
     "credentialing",
     "diagnoses",
     "encounter_providers",
@@ -236,8 +246,10 @@
     "organization_providers",
     "patient_payments",
     "payers",
     "service_facility",
     "service_lines",
     "tags",
     "tasks",
+    "users",
+    "work_queues",
 ]
```

### Comparing `candidhealth-0.0.17/src/candid/client.py` & `candidhealth-0.1.0/src/candid/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
+import typing
+
 from .environment import CandidApiEnvironment
+from .resources.auth.client import AsyncAuthClient, AuthClient
 from .resources.billing_notes.client import AsyncBillingNotesClient, BillingNotesClient
 from .resources.encounters.client import AsyncEncountersClient, EncountersClient
 from .resources.expected_network_status.client import AsyncExpectedNetworkStatusClient, ExpectedNetworkStatusClient
 from .resources.payers.client import AsyncPayersClient, PayersClient
 
 
 class CandidApi:
-    def __init__(self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: str):
+    def __init__(
+        self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
+    ):
         self._environment = environment
         self._token = token
+        self.auth = AuthClient(environment=self._environment, token=self._token)
         self.encounters = EncountersClient(environment=self._environment, token=self._token)
         self.billing_notes = BillingNotesClient(environment=self._environment, token=self._token)
         self.expected_network_status = ExpectedNetworkStatusClient(environment=self._environment, token=self._token)
         self.payers = PayersClient(environment=self._environment, token=self._token)
 
 
 class AsyncCandidApi:
-    def __init__(self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: str):
+    def __init__(
+        self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
+    ):
         self._environment = environment
         self._token = token
+        self.auth = AsyncAuthClient(environment=self._environment, token=self._token)
         self.encounters = AsyncEncountersClient(environment=self._environment, token=self._token)
         self.billing_notes = AsyncBillingNotesClient(environment=self._environment, token=self._token)
         self.expected_network_status = AsyncExpectedNetworkStatusClient(
             environment=self._environment, token=self._token
         )
         self.payers = AsyncPayersClient(environment=self._environment, token=self._token)
```

### Comparing `candidhealth-0.0.17/src/candid/core/datetime_utils.py` & `candidhealth-0.1.0/src/candid/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/core/jsonable_encoder.py` & `candidhealth-0.1.0/src/candid/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/__init__.py` & `candidhealth-0.1.0/src/candid/resources/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from . import (
+    auth,
     billing_notes,
     claims,
     commons,
     contracts,
     credentialing,
     diagnoses,
     encounter_providers,
@@ -17,18 +18,21 @@
     organization_providers,
     patient_payments,
     payers,
     service_facility,
     service_lines,
     tags,
     tasks,
+    users,
+    work_queues,
 )
 from .billing_notes import BillingNote, BillingNoteBase, BillingNoteId
 from .claims import Claim, ClaimStatus
 from .commons import (
+    Auth0Id,
     ClaimId,
     ContentDownloadUrl,
     Date,
     EncounterExternalId,
     EncounterId,
     FacilityTypeCode,
     InsuranceTypeCode,
@@ -48,14 +52,15 @@
     ServiceLineId,
     ServiceLineUnits,
     SourceOfPaymentCode,
     State,
     StreetAddressBase,
     StreetAddressLongZip,
     StreetAddressShortZip,
+    WorkQueueId,
 )
 from .contracts import AuthorizedSignatory, Contract, ContractBase, ContractId, ContractStatus
 from .credentialing import (
     CredentialedEncounterStatusResult,
     CredentialingSpanDates,
     CredentialingSpanDates_NonRequiredDates,
     CredentialingSpanDates_RequiredDates,
@@ -97,16 +102,18 @@
     ServiceLineBaseWithOptionals,
     ServiceLineCreate,
     ServiceLineDenialReason,
     ServiceLineEraData,
 )
 from .tags import Tag, TagColorEnum, TagCreate, TagId
 from .tasks import TaskId
+from .users import User
 
 __all__ = [
+    "Auth0Id",
     "AuthorizedSignatory",
     "BillingNote",
     "BillingNoteBase",
     "BillingNoteId",
     "Claim",
     "ClaimId",
     "ClaimStatus",
@@ -196,14 +203,17 @@
     "SubscriberBase",
     "SubscriberCreate",
     "Tag",
     "TagColorEnum",
     "TagCreate",
     "TagId",
     "TaskId",
+    "User",
+    "WorkQueueId",
+    "auth",
     "billing_notes",
     "claims",
     "commons",
     "contracts",
     "credentialing",
     "diagnoses",
     "encounter_providers",
@@ -216,8 +226,10 @@
     "organization_providers",
     "patient_payments",
     "payers",
     "service_facility",
     "service_lines",
     "tags",
     "tasks",
+    "users",
+    "work_queues",
 ]
```

### Comparing `candidhealth-0.0.17/src/candid/resources/billing_notes/client.py` & `candidhealth-0.1.0/src/candid/resources/billing_notes/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # This file was auto-generated by Fern from our API Definition.
 
+import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
@@ -11,15 +12,17 @@
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import CandidApiEnvironment
 from ..commons.types.encounter_id import EncounterId
 from .types.billing_note import BillingNote
 
 
 class BillingNotesClient:
-    def __init__(self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: str):
+    def __init__(
+        self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
+    ):
         self._environment = environment
         self._token = token
 
     def create(self, *, encounter_id: EncounterId, text: str) -> BillingNote:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/billing_notes/v2"),
@@ -35,15 +38,17 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(BillingNote, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncBillingNotesClient:
-    def __init__(self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: str):
+    def __init__(
+        self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
+    ):
         self._environment = environment
         self._token = token
 
     async def create(self, *, encounter_id: EncounterId, text: str) -> BillingNote:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
```

### Comparing `candidhealth-0.0.17/src/candid/resources/billing_notes/types/billing_note.py` & `candidhealth-0.1.0/src/candid/resources/billing_notes/types/billing_note.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/billing_notes/types/billing_note_base.py` & `candidhealth-0.1.0/src/candid/resources/billing_notes/types/billing_note_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/claims/types/claim.py` & `candidhealth-0.1.0/src/candid/resources/claims/types/claim.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/claims/types/claim_status.py` & `candidhealth-0.1.0/src/candid/resources/claims/types/claim_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/commons/__init__.py` & `candidhealth-0.1.0/src/candid/resources/commons/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
+    Auth0Id,
     ClaimId,
     ContentDownloadUrl,
     Date,
     EncounterExternalId,
     EncounterId,
     FacilityTypeCode,
     InsuranceTypeCode,
@@ -24,17 +25,19 @@
     ServiceLineId,
     ServiceLineUnits,
     SourceOfPaymentCode,
     State,
     StreetAddressBase,
     StreetAddressLongZip,
     StreetAddressShortZip,
+    WorkQueueId,
 )
 
 __all__ = [
+    "Auth0Id",
     "ClaimId",
     "ContentDownloadUrl",
     "Date",
     "EncounterExternalId",
     "EncounterId",
     "FacilityTypeCode",
     "InsuranceTypeCode",
@@ -54,8 +57,9 @@
     "ServiceLineId",
     "ServiceLineUnits",
     "SourceOfPaymentCode",
     "State",
     "StreetAddressBase",
     "StreetAddressLongZip",
     "StreetAddressShortZip",
+    "WorkQueueId",
 ]
```

### Comparing `candidhealth-0.0.17/src/candid/resources/commons/types/__init__.py` & `candidhealth-0.1.0/src/candid/resources/commons/types/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # This file was auto-generated by Fern from our API Definition.
 
+from .auth_0_id import Auth0Id
 from .claim_id import ClaimId
 from .content_download_url import ContentDownloadUrl
 from .date import Date
 from .encounter_external_id import EncounterExternalId
 from .encounter_id import EncounterId
 from .facility_type_code import FacilityTypeCode
 from .insurance_type_code import InsuranceTypeCode
@@ -21,16 +22,18 @@
 from .service_line_id import ServiceLineId
 from .service_line_units import ServiceLineUnits
 from .source_of_payment_code import SourceOfPaymentCode
 from .state import State
 from .street_address_base import StreetAddressBase
 from .street_address_long_zip import StreetAddressLongZip
 from .street_address_short_zip import StreetAddressShortZip
+from .work_queue_id import WorkQueueId
 
 __all__ = [
+    "Auth0Id",
     "ClaimId",
     "ContentDownloadUrl",
     "Date",
     "EncounterExternalId",
     "EncounterId",
     "FacilityTypeCode",
     "InsuranceTypeCode",
@@ -50,8 +53,9 @@
     "ServiceLineId",
     "ServiceLineUnits",
     "SourceOfPaymentCode",
     "State",
     "StreetAddressBase",
     "StreetAddressLongZip",
     "StreetAddressShortZip",
+    "WorkQueueId",
 ]
```

### Comparing `candidhealth-0.0.17/src/candid/resources/commons/types/facility_type_code.py` & `candidhealth-0.1.0/src/candid/resources/commons/types/facility_type_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/commons/types/insurance_type_code.py` & `candidhealth-0.1.0/src/candid/resources/commons/types/insurance_type_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py` & `candidhealth-0.1.0/src/candid/resources/commons/types/patient_relationship_to_insured_code_all.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/commons/types/procedure_modifier.py` & `candidhealth-0.1.0/src/candid/resources/commons/types/procedure_modifier.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/commons/types/region_national.py` & `candidhealth-0.1.0/src/candid/resources/commons/types/region_national.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/commons/types/region_states.py` & `candidhealth-0.1.0/src/candid/resources/commons/types/region_states.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/commons/types/regions.py` & `candidhealth-0.1.0/src/candid/resources/commons/types/regions.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/commons/types/resource_page.py` & `candidhealth-0.1.0/src/candid/resources/commons/types/resource_page.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/commons/types/source_of_payment_code.py` & `candidhealth-0.1.0/src/candid/resources/commons/types/source_of_payment_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/commons/types/state.py` & `candidhealth-0.1.0/src/candid/resources/commons/types/state.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/commons/types/street_address_base.py` & `candidhealth-0.1.0/src/candid/resources/commons/types/street_address_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/commons/types/street_address_long_zip.py` & `candidhealth-0.1.0/src/candid/resources/commons/types/street_address_long_zip.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/commons/types/street_address_short_zip.py` & `candidhealth-0.1.0/src/candid/resources/commons/types/street_address_short_zip.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/contracts/types/authorized_signatory.py` & `candidhealth-0.1.0/src/candid/resources/contracts/types/authorized_signatory.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/contracts/types/contract.py` & `candidhealth-0.1.0/src/candid/resources/contracts/types/contract.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/contracts/types/contract_base.py` & `candidhealth-0.1.0/src/candid/resources/contracts/types/contract_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/contracts/types/contract_status.py` & `candidhealth-0.1.0/src/candid/resources/contracts/types/contract_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/credentialing/__init__.py` & `candidhealth-0.1.0/src/candid/resources/credentialing/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/credentialing/types/__init__.py` & `candidhealth-0.1.0/src/candid/resources/credentialing/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/credentialing/types/credentialed_encounter_status_result.py` & `candidhealth-0.1.0/src/candid/resources/credentialing/types/credentialed_encounter_status_result.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/credentialing/types/credentialing_span_dates.py` & `candidhealth-0.1.0/src/candid/resources/credentialing/types/credentialing_span_dates.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/credentialing/types/credentialing_span_status.py` & `candidhealth-0.1.0/src/candid/resources/credentialing/types/credentialing_span_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/credentialing/types/encounter_credentialing_status_result.py` & `candidhealth-0.1.0/src/candid/resources/credentialing/types/encounter_credentialing_status_result.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/credentialing/types/non_required_credentialing_dates.py` & `candidhealth-0.1.0/src/candid/resources/credentialing/types/non_required_credentialing_dates.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/credentialing/types/provider_credentialing_span.py` & `candidhealth-0.1.0/src/candid/resources/credentialing/types/provider_credentialing_span.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/credentialing/types/provider_credentialing_span_base.py` & `candidhealth-0.1.0/src/candid/resources/credentialing/types/provider_credentialing_span_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/credentialing/types/required_credentialing_dates.py` & `candidhealth-0.1.0/src/candid/resources/credentialing/types/required_credentialing_dates.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/diagnoses/types/diagnosis.py` & `candidhealth-0.1.0/src/candid/resources/diagnoses/types/diagnosis.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/diagnoses/types/diagnosis_create.py` & `candidhealth-0.1.0/src/candid/resources/diagnoses/types/diagnosis_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/diagnoses/types/diagnosis_type_code.py` & `candidhealth-0.1.0/src/candid/resources/diagnoses/types/diagnosis_type_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py` & `candidhealth-0.1.0/src/candid/resources/diagnoses/types/standalone_diagnosis_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py` & `candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py` & `candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/billing_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py` & `candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py` & `candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/encounter_provider_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py` & `candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/referring_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py` & `candidhealth-0.1.0/src/candid/resources/encounter_providers/resources/v_2/types/rendering_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/client.py` & `candidhealth-0.1.0/src/candid/resources/encounters/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
+import typing
+
 from ...environment import CandidApiEnvironment
-from .resources.v_3.client import AsyncV3Client, V3Client
+from .resources.v_4.client import AsyncV4Client, V4Client
 
 
 class EncountersClient:
-    def __init__(self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: str):
+    def __init__(
+        self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
+    ):
         self._environment = environment
         self._token = token
-        self.v_3 = V3Client(environment=self._environment, token=self._token)
+        self.v_4 = V4Client(environment=self._environment, token=self._token)
 
 
 class AsyncEncountersClient:
-    def __init__(self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: str):
+    def __init__(
+        self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
+    ):
         self._environment = environment
         self._token = token
-        self.v_3 = AsyncV3Client(environment=self._environment, token=self._token)
+        self.v_4 = AsyncV4Client(environment=self._environment, token=self._token)
```

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/__init__.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/client.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from ....claims.types.claim_status import ClaimStatus
 from ....commons.types.date import Date
 from ....commons.types.encounter_external_id import EncounterExternalId
 from ....commons.types.encounter_id import EncounterId
 from ....commons.types.facility_type_code import FacilityTypeCode
 from ....commons.types.page_token import PageToken
 from ....commons.types.street_address_long_zip import StreetAddressLongZip
+from ....commons.types.work_queue_id import WorkQueueId
 from ....diagnoses.types.diagnosis_create import DiagnosisCreate
 from ....diagnoses.types.diagnosis_id import DiagnosisId
 from ....encounter_providers.resources.v_2.types.billing_provider import BillingProvider
 from ....encounter_providers.resources.v_2.types.referring_provider import ReferringProvider
 from ....encounter_providers.resources.v_2.types.rendering_provider import RenderingProvider
 from ....individual.types.patient_create import PatientCreate
 from ....individual.types.subscriber_create import SubscriberCreate
@@ -46,16 +47,18 @@
 from .types.synchronicity_type import SynchronicityType
 from .types.vitals import Vitals
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class V3Client:
-    def __init__(self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: str):
+class V4Client:
+    def __init__(
+        self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
+    ):
         self._environment = environment
         self._token = token
 
     def get_all(
         self,
         *,
         limit: typing.Optional[int] = None,
@@ -66,18 +69,19 @@
         date_of_service_max: typing.Optional[Date] = None,
         primary_payer_names: typing.Optional[str] = None,
         search_term: typing.Optional[str] = None,
         external_id: typing.Optional[EncounterExternalId] = None,
         diagnoses_updated_since: typing.Optional[dt.datetime] = None,
         tag_ids: typing.Union[typing.Optional[TagId], typing.List[TagId]],
         do_not_bill: typing.Optional[bool] = None,
+        work_queue_id: typing.Optional[WorkQueueId] = None,
     ) -> EncounterPage:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/encounters/v3"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/encounters/v4"),
             params={
                 "limit": limit,
                 "claim_status": claim_status,
                 "sort": sort,
                 "page_token": page_token,
                 "date_of_service_min": date_of_service_min,
                 "date_of_service_max": date_of_service_max,
@@ -85,14 +89,15 @@
                 "search_term": search_term,
                 "external_id": external_id,
                 "diagnoses_updated_since": serialize_datetime(diagnoses_updated_since)
                 if diagnoses_updated_since is not None
                 else None,
                 "tag_ids": tag_ids,
                 "do_not_bill": do_not_bill,
+                "work_queue_id": work_queue_id,
             },
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
@@ -102,15 +107,15 @@
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(EncounterPage, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, encounter_id: EncounterId) -> Encounter:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/encounters/v3/{encounter_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/encounters/v4/{encounter_id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
             _response_json = _response.json()
@@ -196,15 +201,15 @@
             _request["interventions"] = interventions
         if pay_to_address is not OMIT:
             _request["pay_to_address"] = pay_to_address
         if synchronicity is not OMIT:
             _request["synchronicity"] = synchronicity
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "api/encounters/v3"),
+            urllib.parse.urljoin(f"{self._environment.value}/", "api/encounters/v4"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
@@ -240,15 +245,15 @@
             _request["tag_ids"] = tag_ids
         if clinical_notes is not OMIT:
             _request["clinical_notes"] = clinical_notes
         if pay_to_address is not OMIT:
             _request["pay_to_address"] = pay_to_address
         _response = httpx.request(
             "PATCH",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/encounters/v3/{encounter_id}"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/encounters/v4/{encounter_id}"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
@@ -258,15 +263,15 @@
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(Encounter, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_attachments(self, encounter_id: EncounterId) -> typing.List[EncounterAttachment]:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment.value}/", f"api/encounters/v3/{encounter_id}/attachments"),
+            urllib.parse.urljoin(f"{self._environment.value}/", f"api/encounters/v4/{encounter_id}/attachments"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
             _response_json = _response.json()
@@ -276,15 +281,15 @@
             return pydantic.parse_obj_as(typing.List[EncounterAttachment], _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def generate_clinical_notes_pdf(self, encounter_id: EncounterId) -> GenerateClinicalNotesPdfResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(
-                f"{self._environment.value}/", f"api/encounters/v3/{encounter_id}/clinical-notes-pdf/generate"
+                f"{self._environment.value}/", f"api/encounters/v4/{encounter_id}/clinical-notes-pdf/generate"
             ),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
@@ -295,15 +300,15 @@
             return pydantic.parse_obj_as(GenerateClinicalNotesPdfResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def recompute_network_status_results(self, encounter_id: EncounterId) -> NetworkStatusComputationResults:
         _response = httpx.request(
             "PUT",
             urllib.parse.urljoin(
-                f"{self._environment.value}/", f"api/encounters/v3/{encounter_id}/network-status-results"
+                f"{self._environment.value}/", f"api/encounters/v4/{encounter_id}/network-status-results"
             ),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
@@ -314,15 +319,15 @@
             return pydantic.parse_obj_as(NetworkStatusComputationResults, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def mark_as_not_billable(self, encounter_id: EncounterId) -> MarkAsNotBillableResponse:
         _response = httpx.request(
             "PUT",
             urllib.parse.urljoin(
-                f"{self._environment.value}/", f"api/encounters/v3/{encounter_id}/mark-as-not-billable"
+                f"{self._environment.value}/", f"api/encounters/v4/{encounter_id}/mark-as-not-billable"
             ),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
@@ -330,16 +335,18 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(MarkAsNotBillableResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncV3Client:
-    def __init__(self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: str):
+class AsyncV4Client:
+    def __init__(
+        self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
+    ):
         self._environment = environment
         self._token = token
 
     async def get_all(
         self,
         *,
         limit: typing.Optional[int] = None,
@@ -350,19 +357,20 @@
         date_of_service_max: typing.Optional[Date] = None,
         primary_payer_names: typing.Optional[str] = None,
         search_term: typing.Optional[str] = None,
         external_id: typing.Optional[EncounterExternalId] = None,
         diagnoses_updated_since: typing.Optional[dt.datetime] = None,
         tag_ids: typing.Union[typing.Optional[TagId], typing.List[TagId]],
         do_not_bill: typing.Optional[bool] = None,
+        work_queue_id: typing.Optional[WorkQueueId] = None,
     ) -> EncounterPage:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", "api/encounters/v3"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "api/encounters/v4"),
                 params={
                     "limit": limit,
                     "claim_status": claim_status,
                     "sort": sort,
                     "page_token": page_token,
                     "date_of_service_min": date_of_service_min,
                     "date_of_service_max": date_of_service_max,
@@ -370,14 +378,15 @@
                     "search_term": search_term,
                     "external_id": external_id,
                     "diagnoses_updated_since": serialize_datetime(diagnoses_updated_since)
                     if diagnoses_updated_since is not None
                     else None,
                     "tag_ids": tag_ids,
                     "do_not_bill": do_not_bill,
+                    "work_queue_id": work_queue_id,
                 },
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
@@ -388,15 +397,15 @@
             return pydantic.parse_obj_as(EncounterPage, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(self, encounter_id: EncounterId) -> Encounter:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"api/encounters/v3/{encounter_id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"api/encounters/v4/{encounter_id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
             _response_json = _response.json()
@@ -483,15 +492,15 @@
         if pay_to_address is not OMIT:
             _request["pay_to_address"] = pay_to_address
         if synchronicity is not OMIT:
             _request["synchronicity"] = synchronicity
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "api/encounters/v3"),
+                urllib.parse.urljoin(f"{self._environment.value}/", "api/encounters/v4"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
@@ -528,15 +537,15 @@
         if clinical_notes is not OMIT:
             _request["clinical_notes"] = clinical_notes
         if pay_to_address is not OMIT:
             _request["pay_to_address"] = pay_to_address
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"api/encounters/v3/{encounter_id}"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"api/encounters/v4/{encounter_id}"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
@@ -547,15 +556,15 @@
             return pydantic.parse_obj_as(Encounter, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_attachments(self, encounter_id: EncounterId) -> typing.List[EncounterAttachment]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment.value}/", f"api/encounters/v3/{encounter_id}/attachments"),
+                urllib.parse.urljoin(f"{self._environment.value}/", f"api/encounters/v4/{encounter_id}/attachments"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
             _response_json = _response.json()
@@ -566,15 +575,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def generate_clinical_notes_pdf(self, encounter_id: EncounterId) -> GenerateClinicalNotesPdfResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(
-                    f"{self._environment.value}/", f"api/encounters/v3/{encounter_id}/clinical-notes-pdf/generate"
+                    f"{self._environment.value}/", f"api/encounters/v4/{encounter_id}/clinical-notes-pdf/generate"
                 ),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
@@ -586,15 +595,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def recompute_network_status_results(self, encounter_id: EncounterId) -> NetworkStatusComputationResults:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PUT",
                 urllib.parse.urljoin(
-                    f"{self._environment.value}/", f"api/encounters/v3/{encounter_id}/network-status-results"
+                    f"{self._environment.value}/", f"api/encounters/v4/{encounter_id}/network-status-results"
                 ),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
@@ -606,15 +615,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def mark_as_not_billable(self, encounter_id: EncounterId) -> MarkAsNotBillableResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PUT",
                 urllib.parse.urljoin(
-                    f"{self._environment.value}/", f"api/encounters/v3/{encounter_id}/mark-as-not-billable"
+                    f"{self._environment.value}/", f"api/encounters/v4/{encounter_id}/mark-as-not-billable"
                 ),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
```

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/__init__.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/attributable_contracting_status_result.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/attributable_contracting_status_result.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/base_attachment.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/base_attachment.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/clinical_note.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/clinical_note.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/clinical_note_category.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/clinical_note_category_create.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/clinical_note_category_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/coding_attribution_type.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/coding_attribution_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/contracting_out_of_of_network_reason.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/contracting_out_of_of_network_reason.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/encounter.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/encounter.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from .....diagnoses.types.diagnosis import Diagnosis
 from .....encounter_providers.resources.v_2.types.encounter_provider import EncounterProvider
 from .....individual.types.patient import Patient
 from .....individual.types.subscriber import Subscriber
 from .....patient_payments.resources.v_2.types.patient_payment import PatientPayment
 from .....service_facility.types.encounter_service_facility import EncounterServiceFacility
 from .....tags.types.tag import Tag
+from .....work_queues.resources.v_1.types.work_queue import WorkQueue
 from .clinical_note_category import ClinicalNoteCategory
 from .coding_attribution_type import CodingAttributionType
 from .encounter_base import EncounterBase
 from .patient_history_category import PatientHistoryCategory
 
 
 class Encounter(EncounterBase):
@@ -44,14 +45,15 @@
     )
     place_of_service_code: typing.Optional[FacilityTypeCode]
     place_of_service_code_as_submitted: typing.Optional[FacilityTypeCode]
     patient_histories: typing.List[PatientHistoryCategory]
     patient_payments: typing.List[PatientPayment]
     tags: typing.List[Tag]
     coding_attribution: typing.Optional[CodingAttributionType]
+    work_queue: typing.Optional[WorkQueue]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/encounter_attachment.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/encounter_attachment.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/encounter_base.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/encounter_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/encounter_page.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/encounter_page.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/encounter_sort_options.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/encounter_sort_options.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/generate_clinical_notes_pdf_response.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/generate_clinical_notes_pdf_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/in_network_contracting_status_result.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/in_network_contracting_status_result.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/intake_follow_up.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intake_follow_up.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/intake_question.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intake_question.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/intake_response_and_follow_ups.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intake_response_and_follow_ups.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/intervention.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intervention.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/intervention_category.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/intervention_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/lab.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/lab.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/mark_as_not_billable_response.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/mark_as_not_billable_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/medication.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/medication.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/network_status.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/network_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/network_status_computation_results.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/network_status_computation_results.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/note_category.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/note_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/out_of_network_contracting_status_result.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/out_of_network_contracting_status_result.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/patient_history_category.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/patient_history_category_enum.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/patient_history_category_enum.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/successful_generate_clinical_notes_pdf_response.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/successful_generate_clinical_notes_pdf_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/synchronicity_type.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/synchronicity_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/encounters/resources/v_3/types/vitals.py` & `candidhealth-0.1.0/src/candid/resources/encounters/resources/v_4/types/vitals.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/era/types/era.py` & `candidhealth-0.1.0/src/candid/resources/era/types/era.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/era/types/era_base.py` & `candidhealth-0.1.0/src/candid/resources/era/types/era_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/expected_network_status/client.py` & `candidhealth-0.1.0/src/candid/resources/expected_network_status/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 from .types.expected_network_status_response import ExpectedNetworkStatusResponse
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class ExpectedNetworkStatusClient:
-    def __init__(self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: str):
+    def __init__(
+        self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
+    ):
         self._environment = environment
         self._token = token
 
     def compute(
         self,
         *,
         external_patient_id: typing.Optional[str] = OMIT,
@@ -69,15 +71,17 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ExpectedNetworkStatusResponse, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncExpectedNetworkStatusClient:
-    def __init__(self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: str):
+    def __init__(
+        self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
+    ):
         self._environment = environment
         self._token = token
 
     async def compute(
         self,
         *,
         external_patient_id: typing.Optional[str] = OMIT,
```

### Comparing `candidhealth-0.0.17/src/candid/resources/expected_network_status/types/expected_network_status.py` & `candidhealth-0.1.0/src/candid/resources/expected_network_status/types/expected_network_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/expected_network_status/types/expected_network_status_response.py` & `candidhealth-0.1.0/src/candid/resources/expected_network_status/types/expected_network_status_response.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/individual/types/__init__.py` & `candidhealth-0.1.0/src/candid/resources/individual/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/individual/types/gender.py` & `candidhealth-0.1.0/src/candid/resources/individual/types/gender.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/individual/types/individual_base.py` & `candidhealth-0.1.0/src/candid/resources/individual/types/individual_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/individual/types/patient.py` & `candidhealth-0.1.0/src/candid/resources/individual/types/patient.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/individual/types/patient_create.py` & `candidhealth-0.1.0/src/candid/resources/individual/types/patient_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/individual/types/subscriber.py` & `candidhealth-0.1.0/src/candid/resources/individual/types/subscriber.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/individual/types/subscriber_base.py` & `candidhealth-0.1.0/src/candid/resources/individual/types/subscriber_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/individual/types/subscriber_create.py` & `candidhealth-0.1.0/src/candid/resources/individual/types/subscriber_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/insurance_card/types/insurance_card.py` & `candidhealth-0.1.0/src/candid/resources/insurance_card/types/insurance_card.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/insurance_card/types/insurance_card_base.py` & `candidhealth-0.1.0/src/candid/resources/insurance_card/types/insurance_card_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/insurance_card/types/insurance_card_create.py` & `candidhealth-0.1.0/src/candid/resources/insurance_card/types/insurance_card_create.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/invoices/types/invoice.py` & `candidhealth-0.1.0/src/candid/resources/invoices/types/invoice.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/invoices/types/invoice_item.py` & `candidhealth-0.1.0/src/candid/resources/invoices/types/invoice_item.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/invoices/types/invoice_status.py` & `candidhealth-0.1.0/src/candid/resources/invoices/types/invoice_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/organization_providers/resources/v_2/types/__init__.py` & `candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/organization_providers/resources/v_2/types/license_type.py` & `candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/license_type.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/organization_providers/resources/v_2/types/organization_provider.py` & `candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py` & `candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_address.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_base.py` & `candidhealth-0.1.0/src/candid/resources/organization_providers/resources/v_2/types/organization_provider_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/patient_payments/resources/v_2/types/patient_payment.py` & `candidhealth-0.1.0/src/candid/resources/patient_payments/resources/v_2/types/patient_payment.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_source.py` & `candidhealth-0.1.0/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_source.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_status.py` & `candidhealth-0.1.0/src/candid/resources/patient_payments/resources/v_2/types/patient_payment_status.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/payers/client.py` & `candidhealth-0.1.0/src/candid/resources/payers/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 from ...environment import CandidApiEnvironment
 from ..commons.types.page_token import PageToken
 from .types.payer import Payer
 from .types.payer_page import PayerPage
 
 
 class PayersClient:
-    def __init__(self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: str):
+    def __init__(
+        self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
+    ):
         self._environment = environment
         self._token = token
 
     def get(self, payer_uuid: uuid.UUID) -> Payer:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/payers/v3/{payer_uuid}"),
@@ -60,15 +62,17 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PayerPage, _response_json)  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncPayersClient:
-    def __init__(self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: str):
+    def __init__(
+        self, *, environment: CandidApiEnvironment = CandidApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
+    ):
         self._environment = environment
         self._token = token
 
     async def get(self, payer_uuid: uuid.UUID) -> Payer:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
```

### Comparing `candidhealth-0.0.17/src/candid/resources/payers/types/payer.py` & `candidhealth-0.1.0/src/candid/resources/payers/types/payer.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/payers/types/payer_page.py` & `candidhealth-0.1.0/src/candid/resources/payers/types/payer_page.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/service_facility/types/encounter_service_facility.py` & `candidhealth-0.1.0/src/candid/resources/service_facility/types/encounter_service_facility.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/service_facility/types/encounter_service_facility_base.py` & `candidhealth-0.1.0/src/candid/resources/service_facility/types/encounter_service_facility_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/service_lines/__init__.py` & `candidhealth-0.1.0/src/candid/resources/service_lines/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/service_lines/types/__init__.py` & `candidhealth-0.1.0/src/candid/resources/service_lines/types/__init__.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/service_lines/types/denial_reason_content.py` & `candidhealth-0.1.0/src/candid/resources/service_lines/types/denial_reason_content.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/service_lines/types/drug_identification.py` & `candidhealth-0.1.0/src/candid/resources/service_lines/types/drug_identification.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/service_lines/types/measurement_unit_code.py` & `candidhealth-0.1.0/src/candid/resources/service_lines/types/measurement_unit_code.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/service_lines/types/service_id_qualifier.py` & `candidhealth-0.1.0/src/candid/resources/service_lines/types/service_id_qualifier.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/service_lines/types/service_line.py` & `candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/service_lines/types/service_line_adjustment.py` & `candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_adjustment.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/service_lines/types/service_line_base.py` & `candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_base.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/service_lines/types/service_line_base_with_optionals.py` & `candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_base_with_optionals.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/service_lines/types/service_line_create.py` & `candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_create.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .service_line_base import ServiceLineBase
 
 
 class ServiceLineCreate(ServiceLineBase):
     procedure_code: str
     quantity: str
     units: ServiceLineUnits
-    charge_amount_cents: int = pydantic.Field(
+    charge_amount_cents: typing.Optional[int] = pydantic.Field(
         description=(
             "The total amount charged for this service line taking quantity into account. For example, if a single unit\n"
             "costs 100 cents and 2 units were rendered, the charge_amount_cents should be 200. Should be greater than or\n"
             "equal to 0.\n"
         )
     )
     diagnosis_pointers: typing.List[int] = pydantic.Field(
```

### Comparing `candidhealth-0.0.17/src/candid/resources/service_lines/types/service_line_denial_reason.py` & `candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_denial_reason.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/service_lines/types/service_line_era_data.py` & `candidhealth-0.1.0/src/candid/resources/service_lines/types/service_line_era_data.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/tags/types/tag.py` & `candidhealth-0.1.0/src/candid/resources/tags/types/tag.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/tags/types/tag_color_enum.py` & `candidhealth-0.1.0/src/candid/resources/tags/types/tag_color_enum.py`

 * *Files identical despite different names*

### Comparing `candidhealth-0.0.17/src/candid/resources/tags/types/tag_create.py` & `candidhealth-0.1.0/src/candid/resources/tags/types/tag_create.py`

 * *Files identical despite different names*

