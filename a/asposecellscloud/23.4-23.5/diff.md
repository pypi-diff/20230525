# Comparing `tmp/asposecellscloud-23.4.tar.gz` & `tmp/asposecellscloud-23.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\asposecellscloud-23.4.tar", last modified: Fri Apr 21 23:31:27 2023, max compression
+gzip compressed data, was "dist\asposecellscloud-23.5.tar", last modified: Thu May 25 12:58:19 2023, max compression
```

## Comparing `asposecellscloud-23.4.tar` & `asposecellscloud-23.5.tar`

### file list

```diff
@@ -1,322 +1,322 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 23:31:27.826035 asposecellscloud-23.4/
--rw-rw-rw-   0        0        0     1092 2023-04-21 23:29:09.000000 asposecellscloud-23.4/LICENSE
--rw-rw-rw-   0        0        0      898 2023-04-21 23:31:27.826035 asposecellscloud-23.4/PKG-INFO
--rw-rw-rw-   0        0        0     6917 2023-04-21 23:29:09.000000 asposecellscloud-23.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 23:31:23.255767 asposecellscloud-23.4/asposecellscloud/
--rw-rw-rw-   0        0        0    15740 2023-04-21 23:29:09.000000 asposecellscloud-23.4/asposecellscloud/__init__.py
--rw-rw-rw-   0        0        0    30485 2022-12-08 06:28:10.000000 asposecellscloud-23.4/asposecellscloud/api_client.py
-drwxrwxrwx   0        0        0        0 2023-04-21 23:31:23.302646 asposecellscloud-23.4/asposecellscloud/apis/
--rw-rw-rw-   0        0        0      128 2023-04-21 23:29:09.000000 asposecellscloud-23.4/asposecellscloud/apis/__init__.py
--rw-rw-rw-   0        0        0  2588146 2023-04-21 23:29:09.000000 asposecellscloud-23.4/asposecellscloud/apis/cells_api.py
--rw-rw-rw-   0        0        0    98544 2023-04-21 23:29:09.000000 asposecellscloud-23.4/asposecellscloud/apis/light_cells_api.py
--rw-rw-rw-   0        0        0    86342 2022-01-24 09:49:53.000000 asposecellscloud-23.4/asposecellscloud/apis/lite_cells_api.py
--rw-rw-rw-   0        0        0     8706 2023-04-21 23:29:09.000000 asposecellscloud-23.4/asposecellscloud/configuration.py
-drwxrwxrwx   0        0        0        0 2023-04-21 23:31:27.579157 asposecellscloud-23.4/asposecellscloud/models/
--rw-rw-rw-   0        0        0    13630 2023-04-21 23:29:09.000000 asposecellscloud-23.4/asposecellscloud/models/__init__.py
--rw-rw-rw-   0        0        0     7878 2022-01-09 23:56:52.000000 asposecellscloud-23.4/asposecellscloud/models/above_average.py
--rw-rw-rw-   0        0        0    10430 2022-01-09 23:56:52.000000 asposecellscloud-23.4/asposecellscloud/models/access_token_response.py
--rw-rw-rw-   0        0        0     8340 2022-01-09 23:56:52.000000 asposecellscloud-23.4/asposecellscloud/models/area.py
--rw-rw-rw-   0        0        0     6499 2022-01-09 23:56:52.000000 asposecellscloud-23.4/asposecellscloud/models/auto_filter.py
--rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:52.000000 asposecellscloud-23.4/asposecellscloud/models/auto_filter_response.py
--rw-rw-rw-   0        0        0     6636 2022-01-09 23:56:52.000000 asposecellscloud-23.4/asposecellscloud/models/auto_fitter_options.py
--rw-rw-rw-   0        0        0    30150 2022-01-09 23:56:52.000000 asposecellscloud-23.4/asposecellscloud/models/auto_shape.py
--rw-rw-rw-   0        0        0     4648 2022-01-09 23:56:52.000000 asposecellscloud-23.4/asposecellscloud/models/auto_shape_response.py
--rw-rw-rw-   0        0        0     5228 2022-01-09 23:56:52.000000 asposecellscloud-23.4/asposecellscloud/models/auto_shapes.py
--rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:52.000000 asposecellscloud-23.4/asposecellscloud/models/auto_shapes_response.py
--rw-rw-rw-   0        0        0    30674 2022-12-08 06:28:04.000000 asposecellscloud-23.4/asposecellscloud/models/axis.py
--rw-rw-rw-   0        0        0     4464 2022-12-08 06:28:04.000000 asposecellscloud-23.4/asposecellscloud/models/axis_response.py
--rw-rw-rw-   0        0        0     6075 2022-12-08 06:52:13.000000 asposecellscloud-23.4/asposecellscloud/models/barcode_response.py
--rw-rw-rw-   0        0        0     4577 2022-05-26 05:48:42.000000 asposecellscloud-23.4/asposecellscloud/models/barcode_response_list.py
--rw-rw-rw-   0        0        0     9409 2022-01-09 23:56:52.000000 asposecellscloud-23.4/asposecellscloud/models/batch_convert_request.py
--rw-rw-rw-   0        0        0     5784 2022-01-09 23:56:52.000000 asposecellscloud-23.4/asposecellscloud/models/border.py
--rw-rw-rw-   0        0        0     7101 2022-01-09 23:56:52.000000 asposecellscloud-23.4/asposecellscloud/models/calculation_options.py
--rw-rw-rw-   0        0        0    17986 2022-01-09 23:56:53.000000 asposecellscloud-23.4/asposecellscloud/models/cell.py
--rw-rw-rw-   0        0        0     6979 2022-01-09 23:56:53.000000 asposecellscloud-23.4/asposecellscloud/models/cell_area.py
--rw-rw-rw-   0        0        0     4464 2022-01-09 23:56:53.000000 asposecellscloud-23.4/asposecellscloud/models/cell_response.py
--rw-rw-rw-   0        0        0     7712 2022-01-09 23:56:53.000000 asposecellscloud-23.4/asposecellscloud/models/cell_value.py
--rw-rw-rw-   0        0        0     8817 2022-01-09 23:56:53.000000 asposecellscloud-23.4/asposecellscloud/models/cells.py
--rw-rw-rw-   0        0        0     6537 2022-01-09 23:56:53.000000 asposecellscloud-23.4/asposecellscloud/models/cells_cloud_file_info.py
--rw-rw-rw-   0        0        0     5207 2022-01-09 23:56:53.000000 asposecellscloud-23.4/asposecellscloud/models/cells_cloud_response.py
--rw-rw-rw-   0        0        0     7300 2022-01-09 23:56:53.000000 asposecellscloud-23.4/asposecellscloud/models/cells_color.py
--rw-rw-rw-   0        0        0     5567 2022-01-09 23:56:53.000000 asposecellscloud-23.4/asposecellscloud/models/cells_document_properties.py
--rw-rw-rw-   0        0        0     5010 2022-01-09 23:56:53.000000 asposecellscloud-23.4/asposecellscloud/models/cells_document_properties_response.py
--rw-rw-rw-   0        0        0     9807 2022-01-09 23:56:53.000000 asposecellscloud-23.4/asposecellscloud/models/cells_document_property.py
--rw-rw-rw-   0        0        0     4944 2022-01-09 23:56:53.000000 asposecellscloud-23.4/asposecellscloud/models/cells_document_property_response.py
--rw-rw-rw-   0        0        0     6787 2022-01-09 23:56:53.000000 asposecellscloud-23.4/asposecellscloud/models/cells_error.py
--rw-rw-rw-   0        0        0     6872 2022-01-09 23:56:53.000000 asposecellscloud-23.4/asposecellscloud/models/cells_object_operate_task_parameter.py
--rw-rw-rw-   0        0        0     4497 2022-01-09 23:56:53.000000 asposecellscloud-23.4/asposecellscloud/models/cells_response.py
--rw-rw-rw-   0        0        0    42900 2022-01-09 23:56:53.000000 asposecellscloud-23.4/asposecellscloud/models/chart.py
--rw-rw-rw-   0        0        0    13338 2022-01-09 23:56:54.000000 asposecellscloud-23.4/asposecellscloud/models/chart_area.py
--rw-rw-rw-   0        0        0     4648 2022-01-09 23:56:54.000000 asposecellscloud-23.4/asposecellscloud/models/chart_area_response.py
--rw-rw-rw-   0        0        0    13399 2022-01-09 23:56:54.000000 asposecellscloud-23.4/asposecellscloud/models/chart_frame.py
--rw-rw-rw-   0        0        0    11252 2022-01-09 23:56:54.000000 asposecellscloud-23.4/asposecellscloud/models/chart_operate_parameter.py
--rw-rw-rw-   0        0        0     5077 2022-01-09 23:56:54.000000 asposecellscloud-23.4/asposecellscloud/models/charts.py
--rw-rw-rw-   0        0        0     4530 2022-01-09 23:56:54.000000 asposecellscloud-23.4/asposecellscloud/models/charts_response.py
--rw-rw-rw-   0        0        0     6206 2022-01-09 23:56:54.000000 asposecellscloud-23.4/asposecellscloud/models/color.py
--rw-rw-rw-   0        0        0     7856 2022-01-09 23:56:54.000000 asposecellscloud-23.4/asposecellscloud/models/color_filter.py
--rw-rw-rw-   0        0        0     6284 2022-01-09 23:56:54.000000 asposecellscloud-23.4/asposecellscloud/models/color_filter_request.py
--rw-rw-rw-   0        0        0     9488 2022-01-09 23:56:54.000000 asposecellscloud-23.4/asposecellscloud/models/color_scale.py
--rw-rw-rw-   0        0        0     7595 2022-01-09 23:56:54.000000 asposecellscloud-23.4/asposecellscloud/models/column.py
--rw-rw-rw-   0        0        0     4530 2022-01-09 23:56:54.000000 asposecellscloud-23.4/asposecellscloud/models/column_response.py
--rw-rw-rw-   0        0        0     6821 2022-01-09 23:56:54.000000 asposecellscloud-23.4/asposecellscloud/models/columns.py
--rw-rw-rw-   0        0        0     4563 2022-01-09 23:56:54.000000 asposecellscloud-23.4/asposecellscloud/models/columns_response.py
--rw-rw-rw-   0        0        0    12495 2022-01-09 23:56:55.000000 asposecellscloud-23.4/asposecellscloud/models/comment.py
--rw-rw-rw-   0        0        0     4563 2022-01-09 23:56:55.000000 asposecellscloud-23.4/asposecellscloud/models/comment_response.py
--rw-rw-rw-   0        0        0     5143 2022-01-09 23:56:55.000000 asposecellscloud-23.4/asposecellscloud/models/comments.py
--rw-rw-rw-   0        0        0     4596 2022-01-09 23:56:55.000000 asposecellscloud-23.4/asposecellscloud/models/comments_response.py
--rw-rw-rw-   0        0        0     6091 2022-01-09 23:56:55.000000 asposecellscloud-23.4/asposecellscloud/models/conditional_formatting.py
--rw-rw-rw-   0        0        0     6615 2022-01-09 23:56:55.000000 asposecellscloud-23.4/asposecellscloud/models/conditional_formatting_icon.py
--rw-rw-rw-   0        0        0     5044 2022-01-09 23:56:55.000000 asposecellscloud-23.4/asposecellscloud/models/conditional_formatting_response.py
--rw-rw-rw-   0        0        0     7124 2022-01-09 23:56:55.000000 asposecellscloud-23.4/asposecellscloud/models/conditional_formatting_value.py
--rw-rw-rw-   0        0        0     6424 2022-01-09 23:56:55.000000 asposecellscloud-23.4/asposecellscloud/models/conditional_formattings.py
--rw-rw-rw-   0        0        0     5077 2022-01-09 23:56:55.000000 asposecellscloud-23.4/asposecellscloud/models/conditional_formattings_response.py
--rw-rw-rw-   0        0        0     6330 2022-01-09 23:56:55.000000 asposecellscloud-23.4/asposecellscloud/models/convert_task_parameter.py
--rw-rw-rw-   0        0        0    10343 2021-01-25 09:55:40.000000 asposecellscloud-23.4/asposecellscloud/models/convert_worksheet_task_parameter.py
--rw-rw-rw-   0        0        0    10822 2022-01-09 23:56:55.000000 asposecellscloud-23.4/asposecellscloud/models/copy_options.py
--rw-rw-rw-   0        0        0     9904 2022-01-09 23:56:55.000000 asposecellscloud-23.4/asposecellscloud/models/create_pivot_table_request.py
--rw-rw-rw-   0        0        0     5389 2022-01-09 23:56:55.000000 asposecellscloud-23.4/asposecellscloud/models/custom_filter.py
--rw-rw-rw-   0        0        0     6181 2022-01-09 23:56:55.000000 asposecellscloud-23.4/asposecellscloud/models/custom_parser_config.py
--rw-rw-rw-   0        0        0    14799 2022-01-09 23:56:56.000000 asposecellscloud-23.4/asposecellscloud/models/data_bar.py
--rw-rw-rw-   0        0        0     5420 2022-01-09 23:56:56.000000 asposecellscloud-23.4/asposecellscloud/models/data_bar_border.py
--rw-rw-rw-   0        0        0     6904 2022-01-09 23:56:56.000000 asposecellscloud-23.4/asposecellscloud/models/data_sorter.py
--rw-rw-rw-   0        0        0     3856 2022-01-09 23:56:56.000000 asposecellscloud-23.4/asposecellscloud/models/dif_save_options.py
--rw-rw-rw-   0        0        0     5507 2022-01-09 23:56:56.000000 asposecellscloud-23.4/asposecellscloud/models/disc_usage.py
--rw-rw-rw-   0        0        0     3862 2022-07-25 09:20:18.000000 asposecellscloud-23.4/asposecellscloud/models/docx_save_options.py
--rw-rw-rw-   0        0        0     6036 2022-01-09 23:56:56.000000 asposecellscloud-23.4/asposecellscloud/models/dynamic_filter.py
--rw-rw-rw-   0        0        0     5319 2022-01-09 23:56:56.000000 asposecellscloud-23.4/asposecellscloud/models/error_details.py
--rw-rw-rw-   0        0        0     5975 2021-07-06 12:22:32.000000 asposecellscloud-23.4/asposecellscloud/models/file_info.py
--rw-rw-rw-   0        0        0     5302 2022-01-09 23:56:56.000000 asposecellscloud-23.4/asposecellscloud/models/file_source.py
--rw-rw-rw-   0        0        0     5596 2022-01-09 23:56:56.000000 asposecellscloud-23.4/asposecellscloud/models/file_version.py
--rw-rw-rw-   0        0        0     4514 2022-01-09 23:56:56.000000 asposecellscloud-23.4/asposecellscloud/models/file_versions.py
--rw-rw-rw-   0        0        0     4535 2022-01-09 23:56:56.000000 asposecellscloud-23.4/asposecellscloud/models/files_list.py
--rw-rw-rw-   0        0        0     4424 2021-07-06 12:22:32.000000 asposecellscloud-23.4/asposecellscloud/models/files_result.py
--rw-rw-rw-   0        0        0     5357 2022-01-09 23:56:56.000000 asposecellscloud-23.4/asposecellscloud/models/files_upload_result.py
--rw-rw-rw-   0        0        0     8516 2022-01-09 23:56:56.000000 asposecellscloud-23.4/asposecellscloud/models/fill_format.py
--rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:56.000000 asposecellscloud-23.4/asposecellscloud/models/fill_format_response.py
--rw-rw-rw-   0        0        0    11145 2022-01-09 23:56:56.000000 asposecellscloud-23.4/asposecellscloud/models/filter_column.py
--rw-rw-rw-   0        0        0    10480 2022-01-09 23:56:56.000000 asposecellscloud-23.4/asposecellscloud/models/font.py
--rw-rw-rw-   0        0        0     7369 2022-01-09 23:56:56.000000 asposecellscloud-23.4/asposecellscloud/models/font_setting.py
--rw-rw-rw-   0        0        0    15284 2022-01-09 23:56:57.000000 asposecellscloud-23.4/asposecellscloud/models/format_condition.py
--rw-rw-rw-   0        0        0     6793 2022-01-09 23:56:57.000000 asposecellscloud-23.4/asposecellscloud/models/gradient_fill.py
--rw-rw-rw-   0        0        0     6156 2022-01-09 23:56:57.000000 asposecellscloud-23.4/asposecellscloud/models/gradient_fill_stop.py
--rw-rw-rw-   0        0        0     6286 2022-01-09 23:56:57.000000 asposecellscloud-23.4/asposecellscloud/models/horizontal_page_break.py
--rw-rw-rw-   0        0        0     4997 2022-01-09 23:56:57.000000 asposecellscloud-23.4/asposecellscloud/models/horizontal_page_break_response.py
--rw-rw-rw-   0        0        0     5601 2022-01-09 23:56:57.000000 asposecellscloud-23.4/asposecellscloud/models/horizontal_page_breaks.py
--rw-rw-rw-   0        0        0     5030 2022-01-09 23:56:57.000000 asposecellscloud-23.4/asposecellscloud/models/horizontal_page_breaks_response.py
--rw-rw-rw-   0        0        0    35831 2022-01-09 23:56:57.000000 asposecellscloud-23.4/asposecellscloud/models/html_save_options.py
--rw-rw-rw-   0        0        0     7164 2022-01-09 23:56:57.000000 asposecellscloud-23.4/asposecellscloud/models/hyperlink.py
--rw-rw-rw-   0        0        0     4629 2022-01-09 23:56:57.000000 asposecellscloud-23.4/asposecellscloud/models/hyperlink_response.py
--rw-rw-rw-   0        0        0     5931 2022-01-09 23:56:57.000000 asposecellscloud-23.4/asposecellscloud/models/hyperlinks.py
--rw-rw-rw-   0        0        0     4662 2022-01-09 23:56:57.000000 asposecellscloud-23.4/asposecellscloud/models/hyperlinks_response.py
--rw-rw-rw-   0        0        0     5303 2022-01-09 23:56:57.000000 asposecellscloud-23.4/asposecellscloud/models/icon_filter.py
--rw-rw-rw-   0        0        0     9489 2022-01-09 23:56:57.000000 asposecellscloud-23.4/asposecellscloud/models/icon_set.py
--rw-rw-rw-   0        0        0    14318 2022-01-09 23:56:57.000000 asposecellscloud-23.4/asposecellscloud/models/image_save_options.py
--rw-rw-rw-   0        0        0     4682 2022-01-09 23:56:57.000000 asposecellscloud-23.4/asposecellscloud/models/import_batch_data_option.py
--rw-rw-rw-   0        0        0     8921 2022-01-09 23:56:57.000000 asposecellscloud-23.4/asposecellscloud/models/import_csv_data_option.py
--rw-rw-rw-   0        0        0     6508 2022-01-09 23:56:57.000000 asposecellscloud-23.4/asposecellscloud/models/import_data_task_parameter.py
--rw-rw-rw-   0        0        0     6936 2022-01-09 23:56:57.000000 asposecellscloud-23.4/asposecellscloud/models/import_double_array_option.py
--rw-rw-rw-   0        0        0     6864 2022-01-09 23:56:57.000000 asposecellscloud-23.4/asposecellscloud/models/import_int_array_option.py
--rw-rw-rw-   0        0        0     6953 2022-01-09 23:56:58.000000 asposecellscloud-23.4/asposecellscloud/models/import_option.py
--rw-rw-rw-   0        0        0     9052 2022-01-09 23:56:58.000000 asposecellscloud-23.4/asposecellscloud/models/import_picture_option.py
--rw-rw-rw-   0        0        0     5368 2023-04-21 23:29:09.000000 asposecellscloud-23.4/asposecellscloud/models/import_position.py
--rw-rw-rw-   0        0        0     6930 2022-01-09 23:56:58.000000 asposecellscloud-23.4/asposecellscloud/models/import_string_array_option.py
--rw-rw-rw-   0        0        0     5069 2023-04-21 23:29:09.000000 asposecellscloud-23.4/asposecellscloud/models/import_xml_request.py
--rw-rw-rw-   0        0        0     6968 2022-07-25 09:20:20.000000 asposecellscloud-23.4/asposecellscloud/models/json_save_options.py
--rw-rw-rw-   0        0        0    14632 2022-01-09 23:56:58.000000 asposecellscloud-23.4/asposecellscloud/models/legend.py
--rw-rw-rw-   0        0        0     4530 2022-01-09 23:56:58.000000 asposecellscloud-23.4/asposecellscloud/models/legend_response.py
--rw-rw-rw-   0        0        0    17404 2022-01-09 23:56:58.000000 asposecellscloud-23.4/asposecellscloud/models/line.py
--rw-rw-rw-   0        0        0    17619 2022-01-09 23:56:58.000000 asposecellscloud-23.4/asposecellscloud/models/line_format.py
--rw-rw-rw-   0        0        0     4464 2022-01-09 23:56:58.000000 asposecellscloud-23.4/asposecellscloud/models/line_response.py
--rw-rw-rw-   0        0        0     6045 2022-01-09 23:56:58.000000 asposecellscloud-23.4/asposecellscloud/models/link.py
--rw-rw-rw-   0        0        0     4374 2022-01-09 23:56:58.000000 asposecellscloud-23.4/asposecellscloud/models/link_element.py
--rw-rw-rw-   0        0        0     7020 2022-01-09 23:56:58.000000 asposecellscloud-23.4/asposecellscloud/models/list_column.py
--rw-rw-rw-   0        0        0    18926 2022-01-09 23:56:58.000000 asposecellscloud-23.4/asposecellscloud/models/list_object.py
--rw-rw-rw-   0        0        0     4753 2022-01-09 23:56:58.000000 asposecellscloud-23.4/asposecellscloud/models/list_object_operate_parameter.py
--rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:58.000000 asposecellscloud-23.4/asposecellscloud/models/list_object_response.py
--rw-rw-rw-   0        0        0     5261 2022-01-09 23:56:58.000000 asposecellscloud-23.4/asposecellscloud/models/list_objects.py
--rw-rw-rw-   0        0        0     4714 2022-01-09 23:56:58.000000 asposecellscloud-23.4/asposecellscloud/models/list_objects_response.py
--rw-rw-rw-   0        0        0    15529 2022-01-09 23:56:59.000000 asposecellscloud-23.4/asposecellscloud/models/m_html_save_options.py
--rw-rw-rw-   0        0        0     6279 2022-01-09 23:56:58.000000 asposecellscloud-23.4/asposecellscloud/models/markdown_save_options.py
--rw-rw-rw-   0        0        0     5643 2022-01-09 23:56:58.000000 asposecellscloud-23.4/asposecellscloud/models/match_condition_request.py
--rw-rw-rw-   0        0        0     7627 2022-01-09 23:56:58.000000 asposecellscloud-23.4/asposecellscloud/models/merged_cell.py
--rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:59.000000 asposecellscloud-23.4/asposecellscloud/models/merged_cell_response.py
--rw-rw-rw-   0        0        0     5987 2022-01-09 23:56:59.000000 asposecellscloud-23.4/asposecellscloud/models/merged_cells.py
--rw-rw-rw-   0        0        0     4714 2022-01-09 23:56:59.000000 asposecellscloud-23.4/asposecellscloud/models/merged_cells_response.py
--rw-rw-rw-   0        0        0     3801 2022-01-09 23:56:59.000000 asposecellscloud-23.4/asposecellscloud/models/multiple_filter.py
--rw-rw-rw-   0        0        0     5541 2022-01-09 23:56:59.000000 asposecellscloud-23.4/asposecellscloud/models/multiple_filters.py
--rw-rw-rw-   0        0        0     9541 2022-01-09 23:56:59.000000 asposecellscloud-23.4/asposecellscloud/models/name.py
--rw-rw-rw-   0        0        0     4464 2022-01-09 23:56:59.000000 asposecellscloud-23.4/asposecellscloud/models/name_response.py
--rw-rw-rw-   0        0        0     5746 2022-01-09 23:56:59.000000 asposecellscloud-23.4/asposecellscloud/models/names.py
--rw-rw-rw-   0        0        0     4497 2022-01-09 23:56:59.000000 asposecellscloud-23.4/asposecellscloud/models/names_response.py
--rw-rw-rw-   0        0        0     7728 2022-01-09 23:56:59.000000 asposecellscloud-23.4/asposecellscloud/models/negative_bar_format.py
--rw-rw-rw-   0        0        0     5540 2022-01-09 23:56:59.000000 asposecellscloud-23.4/asposecellscloud/models/object_exist.py
--rw-rw-rw-   0        0        0     3856 2022-01-09 23:56:59.000000 asposecellscloud-23.4/asposecellscloud/models/ods_save_options.py
--rw-rw-rw-   0        0        0    35679 2022-01-09 23:56:59.000000 asposecellscloud-23.4/asposecellscloud/models/ole_object.py
--rw-rw-rw-   0        0        0     4648 2022-01-09 23:56:59.000000 asposecellscloud-23.4/asposecellscloud/models/ole_object_response.py
--rw-rw-rw-   0        0        0     5228 2022-01-09 23:56:59.000000 asposecellscloud-23.4/asposecellscloud/models/ole_objects.py
--rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:59.000000 asposecellscloud-23.4/asposecellscloud/models/ole_objects_response.py
--rw-rw-rw-   0        0        0     4714 2022-01-09 23:56:59.000000 asposecellscloud-23.4/asposecellscloud/models/ooxml_save_options.py
--rw-rw-rw-   0        0        0     5436 2022-01-09 23:56:59.000000 asposecellscloud-23.4/asposecellscloud/models/operate_object.py
--rw-rw-rw-   0        0        0     8551 2022-01-09 23:56:59.000000 asposecellscloud-23.4/asposecellscloud/models/operate_object_position.py
--rw-rw-rw-   0        0        0     4575 2022-01-09 23:57:00.000000 asposecellscloud-23.4/asposecellscloud/models/operate_parameter.py
--rw-rw-rw-   0        0        0     8394 2022-01-09 23:57:00.000000 asposecellscloud-23.4/asposecellscloud/models/page_break_operate_parameter.py
--rw-rw-rw-   0        0        0     8214 2022-01-09 23:57:00.000000 asposecellscloud-23.4/asposecellscloud/models/page_section.py
--rw-rw-rw-   0        0        0     4762 2022-01-09 23:57:00.000000 asposecellscloud-23.4/asposecellscloud/models/page_sections_response.py
--rw-rw-rw-   0        0        0    36653 2022-01-09 23:57:00.000000 asposecellscloud-23.4/asposecellscloud/models/page_setup.py
--rw-rw-rw-   0        0        0     4720 2022-01-09 23:57:00.000000 asposecellscloud-23.4/asposecellscloud/models/page_setup_operate_parameter.py
--rw-rw-rw-   0        0        0     4648 2022-01-09 23:57:00.000000 asposecellscloud-23.4/asposecellscloud/models/page_setup_response.py
--rw-rw-rw-   0        0        0     4487 2022-01-09 23:57:00.000000 asposecellscloud-23.4/asposecellscloud/models/password_request.py
--rw-rw-rw-   0        0        0     6858 2022-01-09 23:57:00.000000 asposecellscloud-23.4/asposecellscloud/models/paste_options.py
--rw-rw-rw-   0        0        0     9851 2022-01-09 23:57:00.000000 asposecellscloud-23.4/asposecellscloud/models/pattern_fill.py
--rw-rw-rw-   0        0        0    12225 2022-01-09 23:57:00.000000 asposecellscloud-23.4/asposecellscloud/models/pdf_save_options.py
--rw-rw-rw-   0        0        0    14691 2022-01-09 23:57:00.000000 asposecellscloud-23.4/asposecellscloud/models/pdf_security_options.py
--rw-rw-rw-   0        0        0     7612 2022-01-09 23:57:01.000000 asposecellscloud-23.4/asposecellscloud/models/pic_format_option.py
--rw-rw-rw-   0        0        0    34670 2022-01-09 23:57:01.000000 asposecellscloud-23.4/asposecellscloud/models/picture.py
--rw-rw-rw-   0        0        0     4563 2022-01-09 23:57:01.000000 asposecellscloud-23.4/asposecellscloud/models/picture_response.py
--rw-rw-rw-   0        0        0     5143 2022-01-09 23:57:01.000000 asposecellscloud-23.4/asposecellscloud/models/pictures.py
--rw-rw-rw-   0        0        0     4596 2022-01-09 23:57:01.000000 asposecellscloud-23.4/asposecellscloud/models/pictures_response.py
--rw-rw-rw-   0        0        0    35618 2022-01-09 23:57:01.000000 asposecellscloud-23.4/asposecellscloud/models/pivot_field.py
--rw-rw-rw-   0        0        0     4681 2022-01-09 23:57:01.000000 asposecellscloud-23.4/asposecellscloud/models/pivot_field_response.py
--rw-rw-rw-   0        0        0    11803 2022-01-09 23:57:01.000000 asposecellscloud-23.4/asposecellscloud/models/pivot_filter.py
--rw-rw-rw-   0        0        0     4714 2022-01-09 23:57:01.000000 asposecellscloud-23.4/asposecellscloud/models/pivot_filter_response.py
--rw-rw-rw-   0        0        0     4762 2022-01-09 23:57:01.000000 asposecellscloud-23.4/asposecellscloud/models/pivot_filters_response.py
--rw-rw-rw-   0        0        0     6544 2022-01-09 23:57:01.000000 asposecellscloud-23.4/asposecellscloud/models/pivot_item.py
--rw-rw-rw-   0        0        0    62471 2022-01-09 23:57:01.000000 asposecellscloud-23.4/asposecellscloud/models/pivot_table.py
--rw-rw-rw-   0        0        0     4488 2022-01-09 23:57:02.000000 asposecellscloud-23.4/asposecellscloud/models/pivot_table_field_request.py
--rw-rw-rw-   0        0        0    11025 2022-01-09 23:57:02.000000 asposecellscloud-23.4/asposecellscloud/models/pivot_table_operate_parameter.py
--rw-rw-rw-   0        0        0     4681 2022-01-09 23:57:02.000000 asposecellscloud-23.4/asposecellscloud/models/pivot_table_response.py
--rw-rw-rw-   0        0        0     5261 2022-01-09 23:57:01.000000 asposecellscloud-23.4/asposecellscloud/models/pivot_tables.py
--rw-rw-rw-   0        0        0     4714 2022-01-09 23:57:01.000000 asposecellscloud-23.4/asposecellscloud/models/pivot_tables_response.py
--rw-rw-rw-   0        0        0     3862 2022-07-25 09:20:24.000000 asposecellscloud-23.4/asposecellscloud/models/pptx_save_options.py
--rw-rw-rw-   0        0        0    19154 2022-01-09 23:57:02.000000 asposecellscloud-23.4/asposecellscloud/models/protect_sheet_parameter.py
--rw-rw-rw-   0        0        0    11570 2022-01-09 23:57:02.000000 asposecellscloud-23.4/asposecellscloud/models/range.py
--rw-rw-rw-   0        0        0     6655 2022-01-09 23:57:02.000000 asposecellscloud-23.4/asposecellscloud/models/range_copy_request.py
--rw-rw-rw-   0        0        0     7038 2022-01-09 23:57:02.000000 asposecellscloud-23.4/asposecellscloud/models/range_set_outline_border_request.py
--rw-rw-rw-   0        0        0     5147 2022-01-09 23:57:02.000000 asposecellscloud-23.4/asposecellscloud/models/range_set_style_request.py
--rw-rw-rw-   0        0        0     4661 2022-01-09 23:57:02.000000 asposecellscloud-23.4/asposecellscloud/models/range_value_response.py
--rw-rw-rw-   0        0        0     4469 2022-01-09 23:57:02.000000 asposecellscloud-23.4/asposecellscloud/models/ranges.py
--rw-rw-rw-   0        0        0     4530 2022-01-09 23:57:02.000000 asposecellscloud-23.4/asposecellscloud/models/ranges_response.py
--rw-rw-rw-   0        0        0     6184 2022-01-09 23:57:02.000000 asposecellscloud-23.4/asposecellscloud/models/result_destination.py
--rw-rw-rw-   0        0        0     9021 2022-01-09 23:57:02.000000 asposecellscloud-23.4/asposecellscloud/models/row.py
--rw-rw-rw-   0        0        0     4431 2022-01-09 23:57:02.000000 asposecellscloud-23.4/asposecellscloud/models/row_response.py
--rw-rw-rw-   0        0        0     6572 2022-01-09 23:57:02.000000 asposecellscloud-23.4/asposecellscloud/models/rows.py
--rw-rw-rw-   0        0        0     4464 2022-01-09 23:57:02.000000 asposecellscloud-23.4/asposecellscloud/models/rows_response.py
--rw-rw-rw-   0        0        0    11282 2022-01-09 23:57:02.000000 asposecellscloud-23.4/asposecellscloud/models/save_options.py
--rw-rw-rw-   0        0        0     4621 2022-01-09 23:57:02.000000 asposecellscloud-23.4/asposecellscloud/models/save_response.py
--rw-rw-rw-   0        0        0     4525 2022-01-09 23:57:02.000000 asposecellscloud-23.4/asposecellscloud/models/save_result.py
--rw-rw-rw-   0        0        0     5706 2022-01-09 23:57:02.000000 asposecellscloud-23.4/asposecellscloud/models/save_result_task_parameter.py
--rw-rw-rw-   0        0        0     8516 2022-01-09 23:57:02.000000 asposecellscloud-23.4/asposecellscloud/models/shadow_effect.py
--rw-rw-rw-   0        0        0    29570 2022-01-09 23:57:03.000000 asposecellscloud-23.4/asposecellscloud/models/shape.py
--rw-rw-rw-   0        0        0     4569 2022-01-09 23:57:03.000000 asposecellscloud-23.4/asposecellscloud/models/shape_operate_parameter.py
--rw-rw-rw-   0        0        0     4497 2022-01-09 23:57:03.000000 asposecellscloud-23.4/asposecellscloud/models/shape_response.py
--rw-rw-rw-   0        0        0     5077 2022-01-09 23:57:03.000000 asposecellscloud-23.4/asposecellscloud/models/shapes.py
--rw-rw-rw-   0        0        0     4530 2022-01-09 23:57:03.000000 asposecellscloud-23.4/asposecellscloud/models/shapes_response.py
--rw-rw-rw-   0        0        0     5135 2022-01-09 23:57:03.000000 asposecellscloud-23.4/asposecellscloud/models/single_value.py
--rw-rw-rw-   0        0        0     4575 2022-01-09 23:57:03.000000 asposecellscloud-23.4/asposecellscloud/models/single_value_response.py
--rw-rw-rw-   0        0        0     6559 2022-01-09 23:57:03.000000 asposecellscloud-23.4/asposecellscloud/models/smart_marker_task_parameter.py
--rw-rw-rw-   0        0        0     5903 2022-01-09 23:57:03.000000 asposecellscloud-23.4/asposecellscloud/models/solid_fill.py
--rw-rw-rw-   0        0        0     7683 2022-01-09 23:57:03.000000 asposecellscloud-23.4/asposecellscloud/models/sort_key.py
--rw-rw-rw-   0        0        0     5887 2022-01-09 23:57:03.000000 asposecellscloud-23.4/asposecellscloud/models/sparkline.py
--rw-rw-rw-   0        0        0    27947 2022-01-09 23:57:03.000000 asposecellscloud-23.4/asposecellscloud/models/sparkline_group.py
--rw-rw-rw-   0        0        0     4813 2022-01-09 23:57:03.000000 asposecellscloud-23.4/asposecellscloud/models/sparkline_group_response.py
--rw-rw-rw-   0        0        0     4776 2022-01-09 23:57:03.000000 asposecellscloud-23.4/asposecellscloud/models/sparkline_groups.py
--rw-rw-rw-   0        0        0     4846 2022-01-09 23:57:03.000000 asposecellscloud-23.4/asposecellscloud/models/sparkline_groups_response.py
--rw-rw-rw-   0        0        0     4534 2022-01-09 23:57:03.000000 asposecellscloud-23.4/asposecellscloud/models/split_result.py
--rw-rw-rw-   0        0        0     5141 2022-01-09 23:57:03.000000 asposecellscloud-23.4/asposecellscloud/models/split_result_document.py
--rw-rw-rw-   0        0        0     4683 2022-01-09 23:57:03.000000 asposecellscloud-23.4/asposecellscloud/models/split_result_response.py
--rw-rw-rw-   0        0        0     9690 2022-01-09 23:57:03.000000 asposecellscloud-23.4/asposecellscloud/models/split_workbook_task_parameter.py
--rw-rw-rw-   0        0        0     6924 2022-01-09 23:57:03.000000 asposecellscloud-23.4/asposecellscloud/models/spreadsheet_ml2003_save_options.py
--rw-rw-rw-   0        0        0    14315 2022-07-25 09:20:26.000000 asposecellscloud-23.4/asposecellscloud/models/sql_script_save_options.py
--rw-rw-rw-   0        0        0     4629 2022-01-09 23:57:03.000000 asposecellscloud-23.4/asposecellscloud/models/storage_exist.py
--rw-rw-rw-   0        0        0     7638 2022-01-09 23:57:03.000000 asposecellscloud-23.4/asposecellscloud/models/storage_file.py
--rw-rw-rw-   0        0        0    21950 2022-01-09 23:57:03.000000 asposecellscloud-23.4/asposecellscloud/models/style.py
--rw-rw-rw-   0        0        0     4497 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/style_response.py
--rw-rw-rw-   0        0        0     4592 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/svg_save_options.py
--rw-rw-rw-   0        0        0     6423 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/table_total_request.py
--rw-rw-rw-   0        0        0     4418 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/task_data.py
--rw-rw-rw-   0        0        0     5358 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/task_description.py
--rw-rw-rw-   0        0        0     3796 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/task_parameter.py
--rw-rw-rw-   0        0        0     4942 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/text_item.py
--rw-rw-rw-   0        0        0     5186 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/text_items.py
--rw-rw-rw-   0        0        0     4648 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/text_items_response.py
--rw-rw-rw-   0        0        0    14978 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/text_options.py
--rw-rw-rw-   0        0        0     7524 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/text_water_marker_request.py
--rw-rw-rw-   0        0        0     8184 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/texture_fill.py
--rw-rw-rw-   0        0        0     5090 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/theme_color.py
--rw-rw-rw-   0        0        0    12409 2022-12-08 06:28:10.000000 asposecellscloud-23.4/asposecellscloud/models/tick_labels.py
--rw-rw-rw-   0        0        0     8508 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/tile_pic_option.py
--rw-rw-rw-   0        0        0    18670 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/title.py
--rw-rw-rw-   0        0        0     4497 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/title_response.py
--rw-rw-rw-   0        0        0     6735 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/top10.py
--rw-rw-rw-   0        0        0     6759 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/top10_filter.py
--rw-rw-rw-   0        0        0     6950 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/txt_save_options.py
--rw-rw-rw-   0        0        0    18950 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/validation.py
--rw-rw-rw-   0        0        0     4662 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/validation_response.py
--rw-rw-rw-   0        0        0     5968 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/validations.py
--rw-rw-rw-   0        0        0     4695 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/validations_response.py
--rw-rw-rw-   0        0        0     3776 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/value_type.py
--rw-rw-rw-   0        0        0     6189 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/vertical_page_break.py
--rw-rw-rw-   0        0        0     4931 2022-01-09 23:57:05.000000 asposecellscloud-23.4/asposecellscloud/models/vertical_page_break_response.py
--rw-rw-rw-   0        0        0     5529 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/vertical_page_breaks.py
--rw-rw-rw-   0        0        0     4964 2022-01-09 23:57:04.000000 asposecellscloud-23.4/asposecellscloud/models/vertical_page_breaks_response.py
--rw-rw-rw-   0        0        0    11948 2022-01-09 23:57:05.000000 asposecellscloud-23.4/asposecellscloud/models/workbook.py
--rw-rw-rw-   0        0        0     6539 2022-01-09 23:57:05.000000 asposecellscloud-23.4/asposecellscloud/models/workbook_encryption_request.py
--rw-rw-rw-   0        0        0     3936 2022-01-09 23:57:05.000000 asposecellscloud-23.4/asposecellscloud/models/workbook_operate_parameter.py
--rw-rw-rw-   0        0        0     5709 2022-01-09 23:57:05.000000 asposecellscloud-23.4/asposecellscloud/models/workbook_protection_request.py
--rw-rw-rw-   0        0        0     5491 2022-01-09 23:57:05.000000 asposecellscloud-23.4/asposecellscloud/models/workbook_replace_response.py
--rw-rw-rw-   0        0        0     4596 2022-01-09 23:57:05.000000 asposecellscloud-23.4/asposecellscloud/models/workbook_response.py
--rw-rw-rw-   0        0        0    52420 2022-01-09 23:57:05.000000 asposecellscloud-23.4/asposecellscloud/models/workbook_settings.py
--rw-rw-rw-   0        0        0     4951 2022-01-09 23:57:05.000000 asposecellscloud-23.4/asposecellscloud/models/workbook_settings_operate_parameter.py
--rw-rw-rw-   0        0        0     4700 2022-01-09 23:57:05.000000 asposecellscloud-23.4/asposecellscloud/models/workbook_settings_response.py
--rw-rw-rw-   0        0        0    32067 2022-01-09 23:57:05.000000 asposecellscloud-23.4/asposecellscloud/models/worksheet.py
--rw-rw-rw-   0        0        0     5720 2022-01-09 23:57:05.000000 asposecellscloud-23.4/asposecellscloud/models/worksheet_moving_request.py
--rw-rw-rw-   0        0        0     7026 2021-05-13 06:59:25.000000 asposecellscloud-23.4/asposecellscloud/models/worksheet_operate_parameter.py
--rw-rw-rw-   0        0        0     5525 2022-01-09 23:57:05.000000 asposecellscloud-23.4/asposecellscloud/models/worksheet_replace_response.py
--rw-rw-rw-   0        0        0     4629 2022-01-09 23:57:05.000000 asposecellscloud-23.4/asposecellscloud/models/worksheet_response.py
--rw-rw-rw-   0        0        0     5209 2022-01-09 23:57:05.000000 asposecellscloud-23.4/asposecellscloud/models/worksheets.py
--rw-rw-rw-   0        0        0     4662 2022-01-09 23:57:05.000000 asposecellscloud-23.4/asposecellscloud/models/worksheets_response.py
--rw-rw-rw-   0        0        0     3856 2022-01-09 23:57:05.000000 asposecellscloud-23.4/asposecellscloud/models/xls_save_options.py
--rw-rw-rw-   0        0        0     3862 2022-01-09 23:57:05.000000 asposecellscloud-23.4/asposecellscloud/models/xlsb_save_options.py
--rw-rw-rw-   0        0        0     3856 2022-01-09 23:57:05.000000 asposecellscloud-23.4/asposecellscloud/models/xps_save_options.py
--rw-rw-rw-   0        0        0    14132 2022-01-09 23:57:06.000000 asposecellscloud-23.4/asposecellscloud/rest.py
-drwxrwxrwx   0        0        0        0 2023-04-21 23:31:23.287026 asposecellscloud-23.4/asposecellscloud.egg-info/
--rw-rw-rw-   0        0        0      898 2023-04-21 23:31:22.000000 asposecellscloud-23.4/asposecellscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    13335 2023-04-21 23:31:23.000000 asposecellscloud-23.4/asposecellscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 23:31:22.000000 asposecellscloud-23.4/asposecellscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-21 23:31:22.000000 asposecellscloud-23.4/asposecellscloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-21 23:31:22.000000 asposecellscloud-23.4/asposecellscloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 23:31:27.851889 asposecellscloud-23.4/setup.cfg
--rw-rw-rw-   0        0        0     1422 2023-04-21 23:29:09.000000 asposecellscloud-23.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 23:31:27.826035 asposecellscloud-23.4/test/
--rw-rw-rw-   0        0        0     7256 2022-12-08 07:15:43.000000 asposecellscloud-23.4/test/test_cells_chart_axis_api.py
--rw-rw-rw-   0        0        0     7996 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_auto_filter_controller.py
--rw-rw-rw-   0        0        0     1816 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_batch_controller.py
--rw-rw-rw-   0        0        0     1338 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_cells_barcodes_controller.py
--rw-rw-rw-   0        0        0    21475 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_cells_controller.py
--rw-rw-rw-   0        0        0     1774 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_cells_status_controller.py
--rw-rw-rw-   0        0        0     2297 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_chart_area_controller.py
--rw-rw-rw-   0        0        0     8079 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_charts_controller.py
--rw-rw-rw-   0        0        0     5842 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_conditional_formattings_controller.py
--rw-rw-rw-   0        0        0    70981 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_conversion.py
--rw-rw-rw-   0        0        0    18233 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_conversion_json.py
--rw-rw-rw-   0        0        0    17784 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_conversion_png.py
--rw-rw-rw-   0        0        0     3361 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_file_controller.py
--rw-rw-rw-   0        0        0     3093 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_folder_controller.py
--rw-rw-rw-   0        0        0     3944 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_hypelinks_controller.py
--rw-rw-rw-   0        0        0   120147 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_light_cells.py
--rw-rw-rw-   0        0        0     7608 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_list_objects_controller.py
--rw-rw-rw-   0        0        0     4326 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_ole_objects_controller.py
--rw-rw-rw-   0        0        0     1333 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_one.py
--rw-rw-rw-   0        0        0     5884 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_page_breaks_controller.py
--rw-rw-rw-   0        0        0     4203 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_page_setup_controller.py
--rw-rw-rw-   0        0        0     4186 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_pictures_controller.py
--rw-rw-rw-   0        0        0    12668 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_pivot_tables_controller.py
--rw-rw-rw-   0        0        0     3363 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_properties_controller.py
--rw-rw-rw-   0        0        0     8719 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_ranges_controller.py
--rw-rw-rw-   0        0        0     4970 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_shapes_controller.py
--rw-rw-rw-   0        0        0     4073 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_sparkline_groups_controller.py
--rw-rw-rw-   0        0        0     2573 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_storage_controller.py
--rw-rw-rw-   0        0        0    18939 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_workbook_controller.py
--rw-rw-rw-   0        0        0    21080 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_worksheet_controller.py
--rw-rw-rw-   0        0        0     3912 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_worksheet_validations_controller.py
--rw-rw-rw-   0        0        0     2422 2023-04-21 23:29:10.000000 asposecellscloud-23.4/test/tests_xml_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:58:19.181003 asposecellscloud-23.5/
+-rw-rw-rw-   0        0        0     1092 2023-04-21 23:29:09.000000 asposecellscloud-23.5/LICENSE
+-rw-rw-rw-   0        0        0      898 2023-05-25 12:58:19.175964 asposecellscloud-23.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6827 2023-05-25 12:57:31.000000 asposecellscloud-23.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 12:58:08.197351 asposecellscloud-23.5/asposecellscloud/
+-rw-rw-rw-   0        0        0    15740 2023-04-21 23:29:09.000000 asposecellscloud-23.5/asposecellscloud/__init__.py
+-rw-rw-rw-   0        0        0    30487 2023-05-25 12:57:31.000000 asposecellscloud-23.5/asposecellscloud/api_client.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:58:08.264335 asposecellscloud-23.5/asposecellscloud/apis/
+-rw-rw-rw-   0        0        0      128 2023-04-21 23:29:09.000000 asposecellscloud-23.5/asposecellscloud/apis/__init__.py
+-rw-rw-rw-   0        0        0  2591815 2023-05-25 12:57:31.000000 asposecellscloud-23.5/asposecellscloud/apis/cells_api.py
+-rw-rw-rw-   0        0        0    98544 2023-04-21 23:29:09.000000 asposecellscloud-23.5/asposecellscloud/apis/light_cells_api.py
+-rw-rw-rw-   0        0        0    86342 2022-01-24 09:49:53.000000 asposecellscloud-23.5/asposecellscloud/apis/lite_cells_api.py
+-rw-rw-rw-   0        0        0     8706 2023-04-21 23:29:09.000000 asposecellscloud-23.5/asposecellscloud/configuration.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:58:18.818967 asposecellscloud-23.5/asposecellscloud/models/
+-rw-rw-rw-   0        0        0    13630 2023-04-21 23:29:09.000000 asposecellscloud-23.5/asposecellscloud/models/__init__.py
+-rw-rw-rw-   0        0        0     7878 2022-01-09 23:56:52.000000 asposecellscloud-23.5/asposecellscloud/models/above_average.py
+-rw-rw-rw-   0        0        0    10430 2022-01-09 23:56:52.000000 asposecellscloud-23.5/asposecellscloud/models/access_token_response.py
+-rw-rw-rw-   0        0        0     8340 2022-01-09 23:56:52.000000 asposecellscloud-23.5/asposecellscloud/models/area.py
+-rw-rw-rw-   0        0        0     6499 2022-01-09 23:56:52.000000 asposecellscloud-23.5/asposecellscloud/models/auto_filter.py
+-rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:52.000000 asposecellscloud-23.5/asposecellscloud/models/auto_filter_response.py
+-rw-rw-rw-   0        0        0     6636 2022-01-09 23:56:52.000000 asposecellscloud-23.5/asposecellscloud/models/auto_fitter_options.py
+-rw-rw-rw-   0        0        0    30150 2022-01-09 23:56:52.000000 asposecellscloud-23.5/asposecellscloud/models/auto_shape.py
+-rw-rw-rw-   0        0        0     4648 2022-01-09 23:56:52.000000 asposecellscloud-23.5/asposecellscloud/models/auto_shape_response.py
+-rw-rw-rw-   0        0        0     5228 2022-01-09 23:56:52.000000 asposecellscloud-23.5/asposecellscloud/models/auto_shapes.py
+-rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:52.000000 asposecellscloud-23.5/asposecellscloud/models/auto_shapes_response.py
+-rw-rw-rw-   0        0        0    30674 2022-12-08 06:28:04.000000 asposecellscloud-23.5/asposecellscloud/models/axis.py
+-rw-rw-rw-   0        0        0     4464 2022-12-08 06:28:04.000000 asposecellscloud-23.5/asposecellscloud/models/axis_response.py
+-rw-rw-rw-   0        0        0     6075 2022-12-08 06:52:13.000000 asposecellscloud-23.5/asposecellscloud/models/barcode_response.py
+-rw-rw-rw-   0        0        0     4577 2022-05-26 05:48:42.000000 asposecellscloud-23.5/asposecellscloud/models/barcode_response_list.py
+-rw-rw-rw-   0        0        0     9409 2022-01-09 23:56:52.000000 asposecellscloud-23.5/asposecellscloud/models/batch_convert_request.py
+-rw-rw-rw-   0        0        0     5784 2022-01-09 23:56:52.000000 asposecellscloud-23.5/asposecellscloud/models/border.py
+-rw-rw-rw-   0        0        0     7101 2022-01-09 23:56:52.000000 asposecellscloud-23.5/asposecellscloud/models/calculation_options.py
+-rw-rw-rw-   0        0        0    17986 2022-01-09 23:56:53.000000 asposecellscloud-23.5/asposecellscloud/models/cell.py
+-rw-rw-rw-   0        0        0     6979 2022-01-09 23:56:53.000000 asposecellscloud-23.5/asposecellscloud/models/cell_area.py
+-rw-rw-rw-   0        0        0     4464 2022-01-09 23:56:53.000000 asposecellscloud-23.5/asposecellscloud/models/cell_response.py
+-rw-rw-rw-   0        0        0     7712 2022-01-09 23:56:53.000000 asposecellscloud-23.5/asposecellscloud/models/cell_value.py
+-rw-rw-rw-   0        0        0     8817 2022-01-09 23:56:53.000000 asposecellscloud-23.5/asposecellscloud/models/cells.py
+-rw-rw-rw-   0        0        0     6537 2022-01-09 23:56:53.000000 asposecellscloud-23.5/asposecellscloud/models/cells_cloud_file_info.py
+-rw-rw-rw-   0        0        0     5207 2022-01-09 23:56:53.000000 asposecellscloud-23.5/asposecellscloud/models/cells_cloud_response.py
+-rw-rw-rw-   0        0        0     7300 2022-01-09 23:56:53.000000 asposecellscloud-23.5/asposecellscloud/models/cells_color.py
+-rw-rw-rw-   0        0        0     5567 2022-01-09 23:56:53.000000 asposecellscloud-23.5/asposecellscloud/models/cells_document_properties.py
+-rw-rw-rw-   0        0        0     5010 2022-01-09 23:56:53.000000 asposecellscloud-23.5/asposecellscloud/models/cells_document_properties_response.py
+-rw-rw-rw-   0        0        0     9807 2022-01-09 23:56:53.000000 asposecellscloud-23.5/asposecellscloud/models/cells_document_property.py
+-rw-rw-rw-   0        0        0     4944 2022-01-09 23:56:53.000000 asposecellscloud-23.5/asposecellscloud/models/cells_document_property_response.py
+-rw-rw-rw-   0        0        0     6787 2022-01-09 23:56:53.000000 asposecellscloud-23.5/asposecellscloud/models/cells_error.py
+-rw-rw-rw-   0        0        0     6872 2022-01-09 23:56:53.000000 asposecellscloud-23.5/asposecellscloud/models/cells_object_operate_task_parameter.py
+-rw-rw-rw-   0        0        0     4497 2022-01-09 23:56:53.000000 asposecellscloud-23.5/asposecellscloud/models/cells_response.py
+-rw-rw-rw-   0        0        0    42900 2022-01-09 23:56:53.000000 asposecellscloud-23.5/asposecellscloud/models/chart.py
+-rw-rw-rw-   0        0        0    13338 2022-01-09 23:56:54.000000 asposecellscloud-23.5/asposecellscloud/models/chart_area.py
+-rw-rw-rw-   0        0        0     4648 2022-01-09 23:56:54.000000 asposecellscloud-23.5/asposecellscloud/models/chart_area_response.py
+-rw-rw-rw-   0        0        0    13399 2022-01-09 23:56:54.000000 asposecellscloud-23.5/asposecellscloud/models/chart_frame.py
+-rw-rw-rw-   0        0        0    11252 2022-01-09 23:56:54.000000 asposecellscloud-23.5/asposecellscloud/models/chart_operate_parameter.py
+-rw-rw-rw-   0        0        0     5077 2022-01-09 23:56:54.000000 asposecellscloud-23.5/asposecellscloud/models/charts.py
+-rw-rw-rw-   0        0        0     4530 2022-01-09 23:56:54.000000 asposecellscloud-23.5/asposecellscloud/models/charts_response.py
+-rw-rw-rw-   0        0        0     6206 2022-01-09 23:56:54.000000 asposecellscloud-23.5/asposecellscloud/models/color.py
+-rw-rw-rw-   0        0        0     7856 2022-01-09 23:56:54.000000 asposecellscloud-23.5/asposecellscloud/models/color_filter.py
+-rw-rw-rw-   0        0        0     6284 2022-01-09 23:56:54.000000 asposecellscloud-23.5/asposecellscloud/models/color_filter_request.py
+-rw-rw-rw-   0        0        0     9488 2022-01-09 23:56:54.000000 asposecellscloud-23.5/asposecellscloud/models/color_scale.py
+-rw-rw-rw-   0        0        0     7595 2022-01-09 23:56:54.000000 asposecellscloud-23.5/asposecellscloud/models/column.py
+-rw-rw-rw-   0        0        0     4530 2022-01-09 23:56:54.000000 asposecellscloud-23.5/asposecellscloud/models/column_response.py
+-rw-rw-rw-   0        0        0     6821 2022-01-09 23:56:54.000000 asposecellscloud-23.5/asposecellscloud/models/columns.py
+-rw-rw-rw-   0        0        0     4563 2022-01-09 23:56:54.000000 asposecellscloud-23.5/asposecellscloud/models/columns_response.py
+-rw-rw-rw-   0        0        0    12495 2022-01-09 23:56:55.000000 asposecellscloud-23.5/asposecellscloud/models/comment.py
+-rw-rw-rw-   0        0        0     4563 2022-01-09 23:56:55.000000 asposecellscloud-23.5/asposecellscloud/models/comment_response.py
+-rw-rw-rw-   0        0        0     5143 2022-01-09 23:56:55.000000 asposecellscloud-23.5/asposecellscloud/models/comments.py
+-rw-rw-rw-   0        0        0     4596 2022-01-09 23:56:55.000000 asposecellscloud-23.5/asposecellscloud/models/comments_response.py
+-rw-rw-rw-   0        0        0     6091 2022-01-09 23:56:55.000000 asposecellscloud-23.5/asposecellscloud/models/conditional_formatting.py
+-rw-rw-rw-   0        0        0     6615 2022-01-09 23:56:55.000000 asposecellscloud-23.5/asposecellscloud/models/conditional_formatting_icon.py
+-rw-rw-rw-   0        0        0     5044 2022-01-09 23:56:55.000000 asposecellscloud-23.5/asposecellscloud/models/conditional_formatting_response.py
+-rw-rw-rw-   0        0        0     7124 2022-01-09 23:56:55.000000 asposecellscloud-23.5/asposecellscloud/models/conditional_formatting_value.py
+-rw-rw-rw-   0        0        0     6424 2022-01-09 23:56:55.000000 asposecellscloud-23.5/asposecellscloud/models/conditional_formattings.py
+-rw-rw-rw-   0        0        0     5077 2022-01-09 23:56:55.000000 asposecellscloud-23.5/asposecellscloud/models/conditional_formattings_response.py
+-rw-rw-rw-   0        0        0     6330 2022-01-09 23:56:55.000000 asposecellscloud-23.5/asposecellscloud/models/convert_task_parameter.py
+-rw-rw-rw-   0        0        0    10343 2021-01-25 09:55:40.000000 asposecellscloud-23.5/asposecellscloud/models/convert_worksheet_task_parameter.py
+-rw-rw-rw-   0        0        0    10822 2022-01-09 23:56:55.000000 asposecellscloud-23.5/asposecellscloud/models/copy_options.py
+-rw-rw-rw-   0        0        0     9904 2022-01-09 23:56:55.000000 asposecellscloud-23.5/asposecellscloud/models/create_pivot_table_request.py
+-rw-rw-rw-   0        0        0     5389 2022-01-09 23:56:55.000000 asposecellscloud-23.5/asposecellscloud/models/custom_filter.py
+-rw-rw-rw-   0        0        0     6181 2022-01-09 23:56:55.000000 asposecellscloud-23.5/asposecellscloud/models/custom_parser_config.py
+-rw-rw-rw-   0        0        0    14799 2022-01-09 23:56:56.000000 asposecellscloud-23.5/asposecellscloud/models/data_bar.py
+-rw-rw-rw-   0        0        0     5420 2022-01-09 23:56:56.000000 asposecellscloud-23.5/asposecellscloud/models/data_bar_border.py
+-rw-rw-rw-   0        0        0     6904 2022-01-09 23:56:56.000000 asposecellscloud-23.5/asposecellscloud/models/data_sorter.py
+-rw-rw-rw-   0        0        0     3856 2022-01-09 23:56:56.000000 asposecellscloud-23.5/asposecellscloud/models/dif_save_options.py
+-rw-rw-rw-   0        0        0     5507 2022-01-09 23:56:56.000000 asposecellscloud-23.5/asposecellscloud/models/disc_usage.py
+-rw-rw-rw-   0        0        0     3862 2022-07-25 09:20:18.000000 asposecellscloud-23.5/asposecellscloud/models/docx_save_options.py
+-rw-rw-rw-   0        0        0     6036 2022-01-09 23:56:56.000000 asposecellscloud-23.5/asposecellscloud/models/dynamic_filter.py
+-rw-rw-rw-   0        0        0     5319 2022-01-09 23:56:56.000000 asposecellscloud-23.5/asposecellscloud/models/error_details.py
+-rw-rw-rw-   0        0        0     5975 2021-07-06 12:22:32.000000 asposecellscloud-23.5/asposecellscloud/models/file_info.py
+-rw-rw-rw-   0        0        0     5302 2022-01-09 23:56:56.000000 asposecellscloud-23.5/asposecellscloud/models/file_source.py
+-rw-rw-rw-   0        0        0     5596 2022-01-09 23:56:56.000000 asposecellscloud-23.5/asposecellscloud/models/file_version.py
+-rw-rw-rw-   0        0        0     4514 2022-01-09 23:56:56.000000 asposecellscloud-23.5/asposecellscloud/models/file_versions.py
+-rw-rw-rw-   0        0        0     4535 2022-01-09 23:56:56.000000 asposecellscloud-23.5/asposecellscloud/models/files_list.py
+-rw-rw-rw-   0        0        0     4424 2021-07-06 12:22:32.000000 asposecellscloud-23.5/asposecellscloud/models/files_result.py
+-rw-rw-rw-   0        0        0     5357 2022-01-09 23:56:56.000000 asposecellscloud-23.5/asposecellscloud/models/files_upload_result.py
+-rw-rw-rw-   0        0        0     8516 2022-01-09 23:56:56.000000 asposecellscloud-23.5/asposecellscloud/models/fill_format.py
+-rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:56.000000 asposecellscloud-23.5/asposecellscloud/models/fill_format_response.py
+-rw-rw-rw-   0        0        0    11145 2022-01-09 23:56:56.000000 asposecellscloud-23.5/asposecellscloud/models/filter_column.py
+-rw-rw-rw-   0        0        0    10480 2022-01-09 23:56:56.000000 asposecellscloud-23.5/asposecellscloud/models/font.py
+-rw-rw-rw-   0        0        0     7369 2022-01-09 23:56:56.000000 asposecellscloud-23.5/asposecellscloud/models/font_setting.py
+-rw-rw-rw-   0        0        0    15284 2022-01-09 23:56:57.000000 asposecellscloud-23.5/asposecellscloud/models/format_condition.py
+-rw-rw-rw-   0        0        0     6793 2022-01-09 23:56:57.000000 asposecellscloud-23.5/asposecellscloud/models/gradient_fill.py
+-rw-rw-rw-   0        0        0     6156 2022-01-09 23:56:57.000000 asposecellscloud-23.5/asposecellscloud/models/gradient_fill_stop.py
+-rw-rw-rw-   0        0        0     6286 2022-01-09 23:56:57.000000 asposecellscloud-23.5/asposecellscloud/models/horizontal_page_break.py
+-rw-rw-rw-   0        0        0     4997 2022-01-09 23:56:57.000000 asposecellscloud-23.5/asposecellscloud/models/horizontal_page_break_response.py
+-rw-rw-rw-   0        0        0     5601 2022-01-09 23:56:57.000000 asposecellscloud-23.5/asposecellscloud/models/horizontal_page_breaks.py
+-rw-rw-rw-   0        0        0     5030 2022-01-09 23:56:57.000000 asposecellscloud-23.5/asposecellscloud/models/horizontal_page_breaks_response.py
+-rw-rw-rw-   0        0        0    35831 2022-01-09 23:56:57.000000 asposecellscloud-23.5/asposecellscloud/models/html_save_options.py
+-rw-rw-rw-   0        0        0     7164 2022-01-09 23:56:57.000000 asposecellscloud-23.5/asposecellscloud/models/hyperlink.py
+-rw-rw-rw-   0        0        0     4629 2022-01-09 23:56:57.000000 asposecellscloud-23.5/asposecellscloud/models/hyperlink_response.py
+-rw-rw-rw-   0        0        0     5931 2022-01-09 23:56:57.000000 asposecellscloud-23.5/asposecellscloud/models/hyperlinks.py
+-rw-rw-rw-   0        0        0     4662 2022-01-09 23:56:57.000000 asposecellscloud-23.5/asposecellscloud/models/hyperlinks_response.py
+-rw-rw-rw-   0        0        0     5303 2022-01-09 23:56:57.000000 asposecellscloud-23.5/asposecellscloud/models/icon_filter.py
+-rw-rw-rw-   0        0        0     9489 2022-01-09 23:56:57.000000 asposecellscloud-23.5/asposecellscloud/models/icon_set.py
+-rw-rw-rw-   0        0        0    14318 2022-01-09 23:56:57.000000 asposecellscloud-23.5/asposecellscloud/models/image_save_options.py
+-rw-rw-rw-   0        0        0     4682 2022-01-09 23:56:57.000000 asposecellscloud-23.5/asposecellscloud/models/import_batch_data_option.py
+-rw-rw-rw-   0        0        0     8921 2022-01-09 23:56:57.000000 asposecellscloud-23.5/asposecellscloud/models/import_csv_data_option.py
+-rw-rw-rw-   0        0        0     6508 2022-01-09 23:56:57.000000 asposecellscloud-23.5/asposecellscloud/models/import_data_task_parameter.py
+-rw-rw-rw-   0        0        0     6936 2022-01-09 23:56:57.000000 asposecellscloud-23.5/asposecellscloud/models/import_double_array_option.py
+-rw-rw-rw-   0        0        0     6864 2022-01-09 23:56:57.000000 asposecellscloud-23.5/asposecellscloud/models/import_int_array_option.py
+-rw-rw-rw-   0        0        0     6953 2022-01-09 23:56:58.000000 asposecellscloud-23.5/asposecellscloud/models/import_option.py
+-rw-rw-rw-   0        0        0     9052 2022-01-09 23:56:58.000000 asposecellscloud-23.5/asposecellscloud/models/import_picture_option.py
+-rw-rw-rw-   0        0        0     5368 2023-04-21 23:29:09.000000 asposecellscloud-23.5/asposecellscloud/models/import_position.py
+-rw-rw-rw-   0        0        0     6930 2022-01-09 23:56:58.000000 asposecellscloud-23.5/asposecellscloud/models/import_string_array_option.py
+-rw-rw-rw-   0        0        0     5069 2023-04-21 23:29:09.000000 asposecellscloud-23.5/asposecellscloud/models/import_xml_request.py
+-rw-rw-rw-   0        0        0     6968 2022-07-25 09:20:20.000000 asposecellscloud-23.5/asposecellscloud/models/json_save_options.py
+-rw-rw-rw-   0        0        0    14632 2022-01-09 23:56:58.000000 asposecellscloud-23.5/asposecellscloud/models/legend.py
+-rw-rw-rw-   0        0        0     4530 2022-01-09 23:56:58.000000 asposecellscloud-23.5/asposecellscloud/models/legend_response.py
+-rw-rw-rw-   0        0        0    17404 2022-01-09 23:56:58.000000 asposecellscloud-23.5/asposecellscloud/models/line.py
+-rw-rw-rw-   0        0        0    17619 2022-01-09 23:56:58.000000 asposecellscloud-23.5/asposecellscloud/models/line_format.py
+-rw-rw-rw-   0        0        0     4464 2022-01-09 23:56:58.000000 asposecellscloud-23.5/asposecellscloud/models/line_response.py
+-rw-rw-rw-   0        0        0     6045 2022-01-09 23:56:58.000000 asposecellscloud-23.5/asposecellscloud/models/link.py
+-rw-rw-rw-   0        0        0     4374 2022-01-09 23:56:58.000000 asposecellscloud-23.5/asposecellscloud/models/link_element.py
+-rw-rw-rw-   0        0        0     7020 2022-01-09 23:56:58.000000 asposecellscloud-23.5/asposecellscloud/models/list_column.py
+-rw-rw-rw-   0        0        0    18926 2022-01-09 23:56:58.000000 asposecellscloud-23.5/asposecellscloud/models/list_object.py
+-rw-rw-rw-   0        0        0     4753 2022-01-09 23:56:58.000000 asposecellscloud-23.5/asposecellscloud/models/list_object_operate_parameter.py
+-rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:58.000000 asposecellscloud-23.5/asposecellscloud/models/list_object_response.py
+-rw-rw-rw-   0        0        0     5261 2022-01-09 23:56:58.000000 asposecellscloud-23.5/asposecellscloud/models/list_objects.py
+-rw-rw-rw-   0        0        0     4714 2022-01-09 23:56:58.000000 asposecellscloud-23.5/asposecellscloud/models/list_objects_response.py
+-rw-rw-rw-   0        0        0    15529 2022-01-09 23:56:59.000000 asposecellscloud-23.5/asposecellscloud/models/m_html_save_options.py
+-rw-rw-rw-   0        0        0     6279 2022-01-09 23:56:58.000000 asposecellscloud-23.5/asposecellscloud/models/markdown_save_options.py
+-rw-rw-rw-   0        0        0     5643 2022-01-09 23:56:58.000000 asposecellscloud-23.5/asposecellscloud/models/match_condition_request.py
+-rw-rw-rw-   0        0        0     7627 2022-01-09 23:56:58.000000 asposecellscloud-23.5/asposecellscloud/models/merged_cell.py
+-rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:59.000000 asposecellscloud-23.5/asposecellscloud/models/merged_cell_response.py
+-rw-rw-rw-   0        0        0     5987 2022-01-09 23:56:59.000000 asposecellscloud-23.5/asposecellscloud/models/merged_cells.py
+-rw-rw-rw-   0        0        0     4714 2022-01-09 23:56:59.000000 asposecellscloud-23.5/asposecellscloud/models/merged_cells_response.py
+-rw-rw-rw-   0        0        0     3801 2022-01-09 23:56:59.000000 asposecellscloud-23.5/asposecellscloud/models/multiple_filter.py
+-rw-rw-rw-   0        0        0     5541 2022-01-09 23:56:59.000000 asposecellscloud-23.5/asposecellscloud/models/multiple_filters.py
+-rw-rw-rw-   0        0        0     9541 2022-01-09 23:56:59.000000 asposecellscloud-23.5/asposecellscloud/models/name.py
+-rw-rw-rw-   0        0        0     4464 2022-01-09 23:56:59.000000 asposecellscloud-23.5/asposecellscloud/models/name_response.py
+-rw-rw-rw-   0        0        0     5746 2022-01-09 23:56:59.000000 asposecellscloud-23.5/asposecellscloud/models/names.py
+-rw-rw-rw-   0        0        0     4497 2022-01-09 23:56:59.000000 asposecellscloud-23.5/asposecellscloud/models/names_response.py
+-rw-rw-rw-   0        0        0     7728 2022-01-09 23:56:59.000000 asposecellscloud-23.5/asposecellscloud/models/negative_bar_format.py
+-rw-rw-rw-   0        0        0     5540 2022-01-09 23:56:59.000000 asposecellscloud-23.5/asposecellscloud/models/object_exist.py
+-rw-rw-rw-   0        0        0     3856 2022-01-09 23:56:59.000000 asposecellscloud-23.5/asposecellscloud/models/ods_save_options.py
+-rw-rw-rw-   0        0        0    35679 2022-01-09 23:56:59.000000 asposecellscloud-23.5/asposecellscloud/models/ole_object.py
+-rw-rw-rw-   0        0        0     4648 2022-01-09 23:56:59.000000 asposecellscloud-23.5/asposecellscloud/models/ole_object_response.py
+-rw-rw-rw-   0        0        0     5228 2022-01-09 23:56:59.000000 asposecellscloud-23.5/asposecellscloud/models/ole_objects.py
+-rw-rw-rw-   0        0        0     4681 2022-01-09 23:56:59.000000 asposecellscloud-23.5/asposecellscloud/models/ole_objects_response.py
+-rw-rw-rw-   0        0        0     4714 2022-01-09 23:56:59.000000 asposecellscloud-23.5/asposecellscloud/models/ooxml_save_options.py
+-rw-rw-rw-   0        0        0     5436 2022-01-09 23:56:59.000000 asposecellscloud-23.5/asposecellscloud/models/operate_object.py
+-rw-rw-rw-   0        0        0     8551 2022-01-09 23:56:59.000000 asposecellscloud-23.5/asposecellscloud/models/operate_object_position.py
+-rw-rw-rw-   0        0        0     4575 2022-01-09 23:57:00.000000 asposecellscloud-23.5/asposecellscloud/models/operate_parameter.py
+-rw-rw-rw-   0        0        0     8394 2022-01-09 23:57:00.000000 asposecellscloud-23.5/asposecellscloud/models/page_break_operate_parameter.py
+-rw-rw-rw-   0        0        0     8214 2022-01-09 23:57:00.000000 asposecellscloud-23.5/asposecellscloud/models/page_section.py
+-rw-rw-rw-   0        0        0     4762 2022-01-09 23:57:00.000000 asposecellscloud-23.5/asposecellscloud/models/page_sections_response.py
+-rw-rw-rw-   0        0        0    36653 2022-01-09 23:57:00.000000 asposecellscloud-23.5/asposecellscloud/models/page_setup.py
+-rw-rw-rw-   0        0        0     4720 2022-01-09 23:57:00.000000 asposecellscloud-23.5/asposecellscloud/models/page_setup_operate_parameter.py
+-rw-rw-rw-   0        0        0     4648 2022-01-09 23:57:00.000000 asposecellscloud-23.5/asposecellscloud/models/page_setup_response.py
+-rw-rw-rw-   0        0        0     4487 2022-01-09 23:57:00.000000 asposecellscloud-23.5/asposecellscloud/models/password_request.py
+-rw-rw-rw-   0        0        0     6858 2022-01-09 23:57:00.000000 asposecellscloud-23.5/asposecellscloud/models/paste_options.py
+-rw-rw-rw-   0        0        0     9851 2022-01-09 23:57:00.000000 asposecellscloud-23.5/asposecellscloud/models/pattern_fill.py
+-rw-rw-rw-   0        0        0    12225 2022-01-09 23:57:00.000000 asposecellscloud-23.5/asposecellscloud/models/pdf_save_options.py
+-rw-rw-rw-   0        0        0    14691 2022-01-09 23:57:00.000000 asposecellscloud-23.5/asposecellscloud/models/pdf_security_options.py
+-rw-rw-rw-   0        0        0     7612 2022-01-09 23:57:01.000000 asposecellscloud-23.5/asposecellscloud/models/pic_format_option.py
+-rw-rw-rw-   0        0        0    34670 2022-01-09 23:57:01.000000 asposecellscloud-23.5/asposecellscloud/models/picture.py
+-rw-rw-rw-   0        0        0     4563 2022-01-09 23:57:01.000000 asposecellscloud-23.5/asposecellscloud/models/picture_response.py
+-rw-rw-rw-   0        0        0     5143 2022-01-09 23:57:01.000000 asposecellscloud-23.5/asposecellscloud/models/pictures.py
+-rw-rw-rw-   0        0        0     4596 2022-01-09 23:57:01.000000 asposecellscloud-23.5/asposecellscloud/models/pictures_response.py
+-rw-rw-rw-   0        0        0    35618 2022-01-09 23:57:01.000000 asposecellscloud-23.5/asposecellscloud/models/pivot_field.py
+-rw-rw-rw-   0        0        0     4681 2022-01-09 23:57:01.000000 asposecellscloud-23.5/asposecellscloud/models/pivot_field_response.py
+-rw-rw-rw-   0        0        0    11803 2022-01-09 23:57:01.000000 asposecellscloud-23.5/asposecellscloud/models/pivot_filter.py
+-rw-rw-rw-   0        0        0     4714 2022-01-09 23:57:01.000000 asposecellscloud-23.5/asposecellscloud/models/pivot_filter_response.py
+-rw-rw-rw-   0        0        0     4762 2022-01-09 23:57:01.000000 asposecellscloud-23.5/asposecellscloud/models/pivot_filters_response.py
+-rw-rw-rw-   0        0        0     6544 2022-01-09 23:57:01.000000 asposecellscloud-23.5/asposecellscloud/models/pivot_item.py
+-rw-rw-rw-   0        0        0    62471 2022-01-09 23:57:01.000000 asposecellscloud-23.5/asposecellscloud/models/pivot_table.py
+-rw-rw-rw-   0        0        0     4488 2022-01-09 23:57:02.000000 asposecellscloud-23.5/asposecellscloud/models/pivot_table_field_request.py
+-rw-rw-rw-   0        0        0    11025 2022-01-09 23:57:02.000000 asposecellscloud-23.5/asposecellscloud/models/pivot_table_operate_parameter.py
+-rw-rw-rw-   0        0        0     4681 2022-01-09 23:57:02.000000 asposecellscloud-23.5/asposecellscloud/models/pivot_table_response.py
+-rw-rw-rw-   0        0        0     5261 2022-01-09 23:57:01.000000 asposecellscloud-23.5/asposecellscloud/models/pivot_tables.py
+-rw-rw-rw-   0        0        0     4714 2022-01-09 23:57:01.000000 asposecellscloud-23.5/asposecellscloud/models/pivot_tables_response.py
+-rw-rw-rw-   0        0        0     3862 2022-07-25 09:20:24.000000 asposecellscloud-23.5/asposecellscloud/models/pptx_save_options.py
+-rw-rw-rw-   0        0        0    19154 2022-01-09 23:57:02.000000 asposecellscloud-23.5/asposecellscloud/models/protect_sheet_parameter.py
+-rw-rw-rw-   0        0        0    11570 2022-01-09 23:57:02.000000 asposecellscloud-23.5/asposecellscloud/models/range.py
+-rw-rw-rw-   0        0        0     6655 2022-01-09 23:57:02.000000 asposecellscloud-23.5/asposecellscloud/models/range_copy_request.py
+-rw-rw-rw-   0        0        0     7038 2022-01-09 23:57:02.000000 asposecellscloud-23.5/asposecellscloud/models/range_set_outline_border_request.py
+-rw-rw-rw-   0        0        0     5147 2022-01-09 23:57:02.000000 asposecellscloud-23.5/asposecellscloud/models/range_set_style_request.py
+-rw-rw-rw-   0        0        0     4661 2022-01-09 23:57:02.000000 asposecellscloud-23.5/asposecellscloud/models/range_value_response.py
+-rw-rw-rw-   0        0        0     4469 2022-01-09 23:57:02.000000 asposecellscloud-23.5/asposecellscloud/models/ranges.py
+-rw-rw-rw-   0        0        0     4530 2022-01-09 23:57:02.000000 asposecellscloud-23.5/asposecellscloud/models/ranges_response.py
+-rw-rw-rw-   0        0        0     6184 2022-01-09 23:57:02.000000 asposecellscloud-23.5/asposecellscloud/models/result_destination.py
+-rw-rw-rw-   0        0        0     9021 2022-01-09 23:57:02.000000 asposecellscloud-23.5/asposecellscloud/models/row.py
+-rw-rw-rw-   0        0        0     4431 2022-01-09 23:57:02.000000 asposecellscloud-23.5/asposecellscloud/models/row_response.py
+-rw-rw-rw-   0        0        0     6572 2022-01-09 23:57:02.000000 asposecellscloud-23.5/asposecellscloud/models/rows.py
+-rw-rw-rw-   0        0        0     4464 2022-01-09 23:57:02.000000 asposecellscloud-23.5/asposecellscloud/models/rows_response.py
+-rw-rw-rw-   0        0        0    11282 2022-01-09 23:57:02.000000 asposecellscloud-23.5/asposecellscloud/models/save_options.py
+-rw-rw-rw-   0        0        0     4621 2022-01-09 23:57:02.000000 asposecellscloud-23.5/asposecellscloud/models/save_response.py
+-rw-rw-rw-   0        0        0     4525 2022-01-09 23:57:02.000000 asposecellscloud-23.5/asposecellscloud/models/save_result.py
+-rw-rw-rw-   0        0        0     5706 2022-01-09 23:57:02.000000 asposecellscloud-23.5/asposecellscloud/models/save_result_task_parameter.py
+-rw-rw-rw-   0        0        0     8516 2022-01-09 23:57:02.000000 asposecellscloud-23.5/asposecellscloud/models/shadow_effect.py
+-rw-rw-rw-   0        0        0    29570 2022-01-09 23:57:03.000000 asposecellscloud-23.5/asposecellscloud/models/shape.py
+-rw-rw-rw-   0        0        0     4569 2022-01-09 23:57:03.000000 asposecellscloud-23.5/asposecellscloud/models/shape_operate_parameter.py
+-rw-rw-rw-   0        0        0     4497 2022-01-09 23:57:03.000000 asposecellscloud-23.5/asposecellscloud/models/shape_response.py
+-rw-rw-rw-   0        0        0     5077 2022-01-09 23:57:03.000000 asposecellscloud-23.5/asposecellscloud/models/shapes.py
+-rw-rw-rw-   0        0        0     4530 2022-01-09 23:57:03.000000 asposecellscloud-23.5/asposecellscloud/models/shapes_response.py
+-rw-rw-rw-   0        0        0     5135 2022-01-09 23:57:03.000000 asposecellscloud-23.5/asposecellscloud/models/single_value.py
+-rw-rw-rw-   0        0        0     4575 2022-01-09 23:57:03.000000 asposecellscloud-23.5/asposecellscloud/models/single_value_response.py
+-rw-rw-rw-   0        0        0     6559 2022-01-09 23:57:03.000000 asposecellscloud-23.5/asposecellscloud/models/smart_marker_task_parameter.py
+-rw-rw-rw-   0        0        0     5903 2022-01-09 23:57:03.000000 asposecellscloud-23.5/asposecellscloud/models/solid_fill.py
+-rw-rw-rw-   0        0        0     7683 2022-01-09 23:57:03.000000 asposecellscloud-23.5/asposecellscloud/models/sort_key.py
+-rw-rw-rw-   0        0        0     5887 2022-01-09 23:57:03.000000 asposecellscloud-23.5/asposecellscloud/models/sparkline.py
+-rw-rw-rw-   0        0        0    27947 2022-01-09 23:57:03.000000 asposecellscloud-23.5/asposecellscloud/models/sparkline_group.py
+-rw-rw-rw-   0        0        0     4813 2022-01-09 23:57:03.000000 asposecellscloud-23.5/asposecellscloud/models/sparkline_group_response.py
+-rw-rw-rw-   0        0        0     4776 2022-01-09 23:57:03.000000 asposecellscloud-23.5/asposecellscloud/models/sparkline_groups.py
+-rw-rw-rw-   0        0        0     4846 2022-01-09 23:57:03.000000 asposecellscloud-23.5/asposecellscloud/models/sparkline_groups_response.py
+-rw-rw-rw-   0        0        0     4534 2022-01-09 23:57:03.000000 asposecellscloud-23.5/asposecellscloud/models/split_result.py
+-rw-rw-rw-   0        0        0     5141 2022-01-09 23:57:03.000000 asposecellscloud-23.5/asposecellscloud/models/split_result_document.py
+-rw-rw-rw-   0        0        0     4683 2022-01-09 23:57:03.000000 asposecellscloud-23.5/asposecellscloud/models/split_result_response.py
+-rw-rw-rw-   0        0        0     9690 2022-01-09 23:57:03.000000 asposecellscloud-23.5/asposecellscloud/models/split_workbook_task_parameter.py
+-rw-rw-rw-   0        0        0     6924 2022-01-09 23:57:03.000000 asposecellscloud-23.5/asposecellscloud/models/spreadsheet_ml2003_save_options.py
+-rw-rw-rw-   0        0        0    14315 2022-07-25 09:20:26.000000 asposecellscloud-23.5/asposecellscloud/models/sql_script_save_options.py
+-rw-rw-rw-   0        0        0     4629 2022-01-09 23:57:03.000000 asposecellscloud-23.5/asposecellscloud/models/storage_exist.py
+-rw-rw-rw-   0        0        0     7638 2022-01-09 23:57:03.000000 asposecellscloud-23.5/asposecellscloud/models/storage_file.py
+-rw-rw-rw-   0        0        0    21950 2022-01-09 23:57:03.000000 asposecellscloud-23.5/asposecellscloud/models/style.py
+-rw-rw-rw-   0        0        0     4497 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/style_response.py
+-rw-rw-rw-   0        0        0     4592 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/svg_save_options.py
+-rw-rw-rw-   0        0        0     6423 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/table_total_request.py
+-rw-rw-rw-   0        0        0     4418 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/task_data.py
+-rw-rw-rw-   0        0        0     5358 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/task_description.py
+-rw-rw-rw-   0        0        0     3796 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/task_parameter.py
+-rw-rw-rw-   0        0        0     4942 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/text_item.py
+-rw-rw-rw-   0        0        0     5186 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/text_items.py
+-rw-rw-rw-   0        0        0     4648 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/text_items_response.py
+-rw-rw-rw-   0        0        0    14978 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/text_options.py
+-rw-rw-rw-   0        0        0     7524 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/text_water_marker_request.py
+-rw-rw-rw-   0        0        0     8184 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/texture_fill.py
+-rw-rw-rw-   0        0        0     5090 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/theme_color.py
+-rw-rw-rw-   0        0        0    12409 2022-12-08 06:28:10.000000 asposecellscloud-23.5/asposecellscloud/models/tick_labels.py
+-rw-rw-rw-   0        0        0     8508 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/tile_pic_option.py
+-rw-rw-rw-   0        0        0    18670 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/title.py
+-rw-rw-rw-   0        0        0     4497 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/title_response.py
+-rw-rw-rw-   0        0        0     6735 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/top10.py
+-rw-rw-rw-   0        0        0     6759 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/top10_filter.py
+-rw-rw-rw-   0        0        0     6950 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/txt_save_options.py
+-rw-rw-rw-   0        0        0    18950 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/validation.py
+-rw-rw-rw-   0        0        0     4662 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/validation_response.py
+-rw-rw-rw-   0        0        0     5968 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/validations.py
+-rw-rw-rw-   0        0        0     4695 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/validations_response.py
+-rw-rw-rw-   0        0        0     3776 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/value_type.py
+-rw-rw-rw-   0        0        0     6189 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/vertical_page_break.py
+-rw-rw-rw-   0        0        0     4931 2022-01-09 23:57:05.000000 asposecellscloud-23.5/asposecellscloud/models/vertical_page_break_response.py
+-rw-rw-rw-   0        0        0     5529 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/vertical_page_breaks.py
+-rw-rw-rw-   0        0        0     4964 2022-01-09 23:57:04.000000 asposecellscloud-23.5/asposecellscloud/models/vertical_page_breaks_response.py
+-rw-rw-rw-   0        0        0    11948 2022-01-09 23:57:05.000000 asposecellscloud-23.5/asposecellscloud/models/workbook.py
+-rw-rw-rw-   0        0        0     6539 2022-01-09 23:57:05.000000 asposecellscloud-23.5/asposecellscloud/models/workbook_encryption_request.py
+-rw-rw-rw-   0        0        0     3936 2022-01-09 23:57:05.000000 asposecellscloud-23.5/asposecellscloud/models/workbook_operate_parameter.py
+-rw-rw-rw-   0        0        0     5709 2022-01-09 23:57:05.000000 asposecellscloud-23.5/asposecellscloud/models/workbook_protection_request.py
+-rw-rw-rw-   0        0        0     5491 2022-01-09 23:57:05.000000 asposecellscloud-23.5/asposecellscloud/models/workbook_replace_response.py
+-rw-rw-rw-   0        0        0     4596 2022-01-09 23:57:05.000000 asposecellscloud-23.5/asposecellscloud/models/workbook_response.py
+-rw-rw-rw-   0        0        0    52420 2022-01-09 23:57:05.000000 asposecellscloud-23.5/asposecellscloud/models/workbook_settings.py
+-rw-rw-rw-   0        0        0     4951 2022-01-09 23:57:05.000000 asposecellscloud-23.5/asposecellscloud/models/workbook_settings_operate_parameter.py
+-rw-rw-rw-   0        0        0     4700 2022-01-09 23:57:05.000000 asposecellscloud-23.5/asposecellscloud/models/workbook_settings_response.py
+-rw-rw-rw-   0        0        0    32067 2022-01-09 23:57:05.000000 asposecellscloud-23.5/asposecellscloud/models/worksheet.py
+-rw-rw-rw-   0        0        0     5720 2022-01-09 23:57:05.000000 asposecellscloud-23.5/asposecellscloud/models/worksheet_moving_request.py
+-rw-rw-rw-   0        0        0     7026 2021-05-13 06:59:25.000000 asposecellscloud-23.5/asposecellscloud/models/worksheet_operate_parameter.py
+-rw-rw-rw-   0        0        0     5525 2022-01-09 23:57:05.000000 asposecellscloud-23.5/asposecellscloud/models/worksheet_replace_response.py
+-rw-rw-rw-   0        0        0     4629 2022-01-09 23:57:05.000000 asposecellscloud-23.5/asposecellscloud/models/worksheet_response.py
+-rw-rw-rw-   0        0        0     5209 2022-01-09 23:57:05.000000 asposecellscloud-23.5/asposecellscloud/models/worksheets.py
+-rw-rw-rw-   0        0        0     4662 2022-01-09 23:57:05.000000 asposecellscloud-23.5/asposecellscloud/models/worksheets_response.py
+-rw-rw-rw-   0        0        0     3856 2022-01-09 23:57:05.000000 asposecellscloud-23.5/asposecellscloud/models/xls_save_options.py
+-rw-rw-rw-   0        0        0     3862 2022-01-09 23:57:05.000000 asposecellscloud-23.5/asposecellscloud/models/xlsb_save_options.py
+-rw-rw-rw-   0        0        0     3856 2022-01-09 23:57:05.000000 asposecellscloud-23.5/asposecellscloud/models/xps_save_options.py
+-rw-rw-rw-   0        0        0    14129 2023-05-25 12:57:31.000000 asposecellscloud-23.5/asposecellscloud/rest.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:58:08.230427 asposecellscloud-23.5/asposecellscloud.egg-info/
+-rw-rw-rw-   0        0        0      898 2023-05-25 12:58:07.000000 asposecellscloud-23.5/asposecellscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13335 2023-05-25 12:58:08.000000 asposecellscloud-23.5/asposecellscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 12:58:07.000000 asposecellscloud-23.5/asposecellscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-25 12:58:07.000000 asposecellscloud-23.5/asposecellscloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-25 12:58:07.000000 asposecellscloud-23.5/asposecellscloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 12:58:19.194993 asposecellscloud-23.5/setup.cfg
+-rw-rw-rw-   0        0        0     1422 2023-05-25 12:57:31.000000 asposecellscloud-23.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 12:58:19.168991 asposecellscloud-23.5/test/
+-rw-rw-rw-   0        0        0     7256 2022-12-08 07:15:43.000000 asposecellscloud-23.5/test/test_cells_chart_axis_api.py
+-rw-rw-rw-   0        0        0     7996 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_auto_filter_controller.py
+-rw-rw-rw-   0        0        0     1816 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_batch_controller.py
+-rw-rw-rw-   0        0        0     1338 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_cells_barcodes_controller.py
+-rw-rw-rw-   0        0        0    21475 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_cells_controller.py
+-rw-rw-rw-   0        0        0     1774 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_cells_status_controller.py
+-rw-rw-rw-   0        0        0     2297 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_chart_area_controller.py
+-rw-rw-rw-   0        0        0     8079 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_charts_controller.py
+-rw-rw-rw-   0        0        0     5842 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_conditional_formattings_controller.py
+-rw-rw-rw-   0        0        0    70981 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_conversion.py
+-rw-rw-rw-   0        0        0    18233 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_conversion_json.py
+-rw-rw-rw-   0        0        0    17784 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_conversion_png.py
+-rw-rw-rw-   0        0        0     3361 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_file_controller.py
+-rw-rw-rw-   0        0        0     3093 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_folder_controller.py
+-rw-rw-rw-   0        0        0     3932 2023-05-25 12:57:31.000000 asposecellscloud-23.5/test/tests_hypelinks_controller.py
+-rw-rw-rw-   0        0        0   120147 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_light_cells.py
+-rw-rw-rw-   0        0        0     7608 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_list_objects_controller.py
+-rw-rw-rw-   0        0        0     4326 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_ole_objects_controller.py
+-rw-rw-rw-   0        0        0     1333 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_one.py
+-rw-rw-rw-   0        0        0     5884 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_page_breaks_controller.py
+-rw-rw-rw-   0        0        0     4203 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_page_setup_controller.py
+-rw-rw-rw-   0        0        0     4182 2023-05-25 12:57:31.000000 asposecellscloud-23.5/test/tests_pictures_controller.py
+-rw-rw-rw-   0        0        0    12668 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_pivot_tables_controller.py
+-rw-rw-rw-   0        0        0     3363 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_properties_controller.py
+-rw-rw-rw-   0        0        0     8719 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_ranges_controller.py
+-rw-rw-rw-   0        0        0     4970 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_shapes_controller.py
+-rw-rw-rw-   0        0        0     4073 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_sparkline_groups_controller.py
+-rw-rw-rw-   0        0        0     2573 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_storage_controller.py
+-rw-rw-rw-   0        0        0    18939 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_workbook_controller.py
+-rw-rw-rw-   0        0        0    21080 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_worksheet_controller.py
+-rw-rw-rw-   0        0        0     3912 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_worksheet_validations_controller.py
+-rw-rw-rw-   0        0        0     2422 2023-04-21 23:29:10.000000 asposecellscloud-23.5/test/tests_xml_controller.py
```

### Comparing `asposecellscloud-23.4/LICENSE` & `asposecellscloud-23.5/LICENSE`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/PKG-INFO` & `asposecellscloud-23.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: asposecellscloud
-Version: 23.4
+Version: 23.5
 Summary: Python Cloud SDK wraps Aspose.Cells REST API so you could seamlessly integrate Microsoft Excel® spreadsheet generation, manipulation, conversion & inspection features into your own Python applications.
 Home-page: https://github.com/aspose-cells-cloud/aspose-cells-cloud-python
 Author: Aspose Cloud
 Author-email: aspose.cloud@aspose.com
 License: UNKNOWN
 Description: Python Cloud SDK wraps Aspose.Cells REST API so you could seamlessly integrate Microsoft Excel® spreadsheet generation, manipulation, conversion & inspection features into your own Python applications.
 Keywords: aspose,cells,cloud
```

### Comparing `asposecellscloud-23.4/README.md` & `asposecellscloud-23.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![](https://img.shields.io/badge/REST%20API-v3.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/asposecellscloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/asposecellscloud) ![PyPI - Downloads](https://img.shields.io/pypi/dm/asposecellscloud)  [![GitHub license](https://img.shields.io/github/license/aspose-cells-cloud/aspose-cells-cloud-python)](https://github.com/aspose-cells-cloud/aspose-cells-cloud-python/blob/master/LICENSE) ![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/aspose-cells-cloud/aspose-cells-cloud-python/23.4)
+![](https://img.shields.io/badge/REST%20API-v3.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/asposecellscloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/asposecellscloud) ![PyPI - Downloads](https://img.shields.io/pypi/dm/asposecellscloud)  [![GitHub license](https://img.shields.io/github/license/aspose-cells-cloud/aspose-cells-cloud-python)](https://github.com/aspose-cells-cloud/aspose-cells-cloud-python/blob/master/LICENSE) ![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/aspose-cells-cloud/aspose-cells-cloud-python/23.5)
 
 
 # Python SDK for Spreadsheet Processing in Cloud
 
 Python Cloud SDK wraps Aspose.Cells REST API so you could seamlessly integrate Microsoft Excel® spreadsheet generation, manipulation, conversion & inspection features into your own Python applications. 
 
 [Aspose.Cells Cloud SDK for Python](https://products.aspose.cloud/cells/python) offers Excel® file creation, editing, conversion, & rendering. Developers can format worksheets, rows, columns or cells to the most granular level, create & manipulate chart & pivot tables, render worksheets, charts and specific data ranges to PDF & images, add & calculate Excel's built-in and custom formulas and much more.
@@ -17,19 +17,18 @@
 - Set complex formulas & calculate results via API.
 - Set protection on workbook, worksheet, cell, column or row.
 - Create & manipulate named ranges.
 - Populate worksheets through Smart Markers.
 - Convert worksheets to PDF, XPS & SVG formats.
 - Inter-convert files to popular Excel formats.
 
-## Feature & Enhancements in Version 23.4
+## Feature & Enhancements in Version 23.5
+
+- Fix few method names for spelling error.
 
-- Adopt the new model(Conflicting expired function names are appended with _).
-- Add import xml data api.
-- Add export xml data api.
  
 ## Read & Write Spreadsheet Formats
 
 **Microsoft Excel:** XLS, XLSX, XLSB, XLSM, XLT, XLTX, XLTM
 **OpenOffice:** ODS
 **SpreadsheetML:** XML
 **Text:** CSV, TSV, TXT (TabDelimited)
```

### Comparing `asposecellscloud-23.4/asposecellscloud/__init__.py` & `asposecellscloud-23.5/asposecellscloud/__init__.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/api_client.py` & `asposecellscloud-23.5/asposecellscloud/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -549,15 +549,15 @@
         """
         config = Configuration()
 
         fd, path = tempfile.mkstemp(dir=config.temp_folder_path)
         os.close(fd)
         os.remove(path)
 
-        content_disposition = response.getheader("Content-Disposition")
+        content_disposition = response.headers.get("Content-Disposition")
         if content_disposition:
             filename = re.\
                 search(r'filename=[\'"]?([^\'"\s]+)[\'"]?', content_disposition).\
                 group(1)
             path = os.path.join(os.path.dirname(path), filename)
 
         with open(path, "wb") as f:
```

### Comparing `asposecellscloud-23.4/asposecellscloud/apis/cells_api.py` & `asposecellscloud-23.5/asposecellscloud/apis/cells_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -5103,29 +5103,35 @@
                                         callback=params.get('callback'),
                                         _return_http_data_only=params.get('_return_http_data_only'),
                                         _preload_content=params.get('_preload_content', True),
                                         _request_timeout=params.get('_request_timeout'),
                                         collection_formats=http_params['collection_formats'])
 
 
-
+    def get_work_sheet_hyperlinks(self, request, **kwargs):
+        warnings.warn("get_work_sheet_hyperlinks is deprecated", DeprecationWarning)
+        return self.get_worksheet_hyperlinks(request,kwargs)
+    def get_work_sheet_hyperlinks_with_http_info(self, request, **kwargs):
+        warnings.warn("get_work_sheet_hyperlinks_with_http_info is deprecated", DeprecationWarning)
+        return self.get_worksheet_hyperlinks_with_http_info(request,kwargs)
+    
     # <summary>
     # </summary>
-    # <param name="request">Request. <see cref="GetWorkSheetHyperlinksRequest" /></param>
-    def get_work_sheet_hyperlinks(self, request, **kwargs):
+    # <param name="request">Request. <see cref="GetWorkheetHyperlinksRequest" /></param>
+    def get_worksheet_hyperlinks(self, request, **kwargs):
 
         kwargs['_return_http_data_only'] = True
         self.check_access_token()
         if kwargs.get('callback'):
-            return self.get_work_sheet_hyperlinks_with_http_info(request,**kwargs)
+            return self.get_worksheet_hyperlinks_with_http_info(request,**kwargs)
         else:
-            (data) = self.get_work_sheet_hyperlinks_with_http_info(request,**kwargs)
+            (data) = self.get_worksheet_hyperlinks_with_http_info(request,**kwargs)
             return data
 
-    def get_work_sheet_hyperlinks_with_http_info(self, request, **kwargs):
+    def get_worksheet_hyperlinks_with_http_info(self, request, **kwargs):
         all_params = []
         all_params.append('callback')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
         params = locals()
         for key, val in iteritems(params['kwargs']):
@@ -5150,29 +5156,34 @@
                                         callback=params.get('callback'),
                                         _return_http_data_only=params.get('_return_http_data_only'),
                                         _preload_content=params.get('_preload_content', True),
                                         _request_timeout=params.get('_request_timeout'),
                                         collection_formats=http_params['collection_formats'])
 
 
-
+    def get_work_sheet_hyperlink(self, request, **kwargs):
+        warnings.warn("get_work_sheet_hyperlink is deprecated", DeprecationWarning)
+        return self.get_worksheet_hyperlink(request,kwargs)
+    def get_work_sheet_hyperlink_with_http_info(self, request, **kwargs):
+        warnings.warn("get_work_sheet_hyperlink_with_http_info is deprecated", DeprecationWarning)
+        return self.get_worksheet_hyperlink_with_http_info(request,kwargs)    
     # <summary>
     # </summary>
-    # <param name="request">Request. <see cref="GetWorkSheetHyperlinkRequest" /></param>
-    def get_work_sheet_hyperlink(self, request, **kwargs):
+    # <param name="request">Request. <see cref="GetWorksheetHyperlinkRequest" /></param>
+    def get_worksheet_hyperlink(self, request, **kwargs):
 
         kwargs['_return_http_data_only'] = True
         self.check_access_token()
         if kwargs.get('callback'):
-            return self.get_work_sheet_hyperlink_with_http_info(request,**kwargs)
+            return self.get_worksheet_hyperlink_with_http_info(request,**kwargs)
         else:
-            (data) = self.get_work_sheet_hyperlink_with_http_info(request,**kwargs)
+            (data) = self.get_worksheet_hyperlink_with_http_info(request,**kwargs)
             return data
 
-    def get_work_sheet_hyperlink_with_http_info(self, request, **kwargs):
+    def get_worksheet_hyperlink_with_http_info(self, request, **kwargs):
         all_params = []
         all_params.append('callback')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
         params = locals()
         for key, val in iteritems(params['kwargs']):
@@ -5197,29 +5208,34 @@
                                         callback=params.get('callback'),
                                         _return_http_data_only=params.get('_return_http_data_only'),
                                         _preload_content=params.get('_preload_content', True),
                                         _request_timeout=params.get('_request_timeout'),
                                         collection_formats=http_params['collection_formats'])
 
 
-
+    def delete_work_sheet_hyperlink(self, request, **kwargs):
+        warnings.warn("get_work_sheet_hyperlink is deprecated", DeprecationWarning)
+        return self.delete_worksheet_hyperlink(request,kwargs)
+    def delete_work_sheet_hyperlink_with_http_info(self, request, **kwargs):
+        warnings.warn("delete_work_sheet_hyperlink_with_http_info is deprecated", DeprecationWarning)
+        return self.delete_worksheet_hyperlink_with_http_info(request,kwargs)   
     # <summary>
     # </summary>
-    # <param name="request">Request. <see cref="DeleteWorkSheetHyperlinkRequest" /></param>
-    def delete_work_sheet_hyperlink(self, request, **kwargs):
+    # <param name="request">Request. <see cref="DeleteWorksheetHyperlinkRequest" /></param>
+    def delete_worksheet_hyperlink(self, request, **kwargs):
 
         kwargs['_return_http_data_only'] = True
         self.check_access_token()
         if kwargs.get('callback'):
-            return self.delete_work_sheet_hyperlink_with_http_info(request,**kwargs)
+            return self.delete_worksheet_hyperlink_with_http_info(request,**kwargs)
         else:
-            (data) = self.delete_work_sheet_hyperlink_with_http_info(request,**kwargs)
+            (data) = self.delete_worksheet_hyperlink_with_http_info(request,**kwargs)
             return data
 
-    def delete_work_sheet_hyperlink_with_http_info(self, request, **kwargs):
+    def delete_worksheet_hyperlink_with_http_info(self, request, **kwargs):
         all_params = []
         all_params.append('callback')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
         params = locals()
         for key, val in iteritems(params['kwargs']):
@@ -5244,29 +5260,34 @@
                                         callback=params.get('callback'),
                                         _return_http_data_only=params.get('_return_http_data_only'),
                                         _preload_content=params.get('_preload_content', True),
                                         _request_timeout=params.get('_request_timeout'),
                                         collection_formats=http_params['collection_formats'])
 
 
-
+    def post_work_sheet_hyperlink(self, request, **kwargs):
+        warnings.warn("post_work_sheet_hyperlink is deprecated", DeprecationWarning)
+        return self.post_worksheet_hyperlink(request,kwargs)
+    def post_work_sheet_hyperlink_with_http_info(self, request, **kwargs):
+        warnings.warn("post_work_sheet_hyperlink_with_http_info is deprecated", DeprecationWarning)
+        return self.post_worksheet_hyperlink_with_http_info(request,kwargs)  
     # <summary>
     # </summary>
-    # <param name="request">Request. <see cref="PostWorkSheetHyperlinkRequest" /></param>
-    def post_work_sheet_hyperlink(self, request, **kwargs):
+    # <param name="request">Request. <see cref="PostWorksheetHyperlinkRequest" /></param>
+    def post_worksheet_hyperlink(self, request, **kwargs):
 
         kwargs['_return_http_data_only'] = True
         self.check_access_token()
         if kwargs.get('callback'):
-            return self.post_work_sheet_hyperlink_with_http_info(request,**kwargs)
+            return self.post_worksheet_hyperlink_with_http_info(request,**kwargs)
         else:
-            (data) = self.post_work_sheet_hyperlink_with_http_info(request,**kwargs)
+            (data) = self.post_worksheet_hyperlink_with_http_info(request,**kwargs)
             return data
 
-    def post_work_sheet_hyperlink_with_http_info(self, request, **kwargs):
+    def post_worksheet_hyperlink_with_http_info(self, request, **kwargs):
         all_params = []
         all_params.append('callback')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
         params = locals()
         for key, val in iteritems(params['kwargs']):
@@ -5291,29 +5312,34 @@
                                         callback=params.get('callback'),
                                         _return_http_data_only=params.get('_return_http_data_only'),
                                         _preload_content=params.get('_preload_content', True),
                                         _request_timeout=params.get('_request_timeout'),
                                         collection_formats=http_params['collection_formats'])
 
 
-
+    def put_work_sheet_hyperlink(self, request, **kwargs):
+        warnings.warn("put_work_sheet_hyperlink is deprecated", DeprecationWarning)
+        return self.put_worksheet_hyperlink(request,kwargs)
+    def put_work_sheet_hyperlink_with_http_info(self, request, **kwargs):
+        warnings.warn("put_work_sheet_hyperlink_with_http_info is deprecated", DeprecationWarning)
+        return self.put_worksheet_hyperlink_with_http_info(request,kwargs) 
     # <summary>
     # </summary>
-    # <param name="request">Request. <see cref="PutWorkSheetHyperlinkRequest" /></param>
-    def put_work_sheet_hyperlink(self, request, **kwargs):
+    # <param name="request">Request. <see cref="PutWorksheetHyperlinkRequest" /></param>
+    def put_worksheet_hyperlink(self, request, **kwargs):
 
         kwargs['_return_http_data_only'] = True
         self.check_access_token()
         if kwargs.get('callback'):
-            return self.put_work_sheet_hyperlink_with_http_info(request,**kwargs)
+            return self.put_worksheet_hyperlink_with_http_info(request,**kwargs)
         else:
-            (data) = self.put_work_sheet_hyperlink_with_http_info(request,**kwargs)
+            (data) = self.put_worksheet_hyperlink_with_http_info(request,**kwargs)
             return data
 
-    def put_work_sheet_hyperlink_with_http_info(self, request, **kwargs):
+    def put_worksheet_hyperlink_with_http_info(self, request, **kwargs):
         all_params = []
         all_params.append('callback')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
         params = locals()
         for key, val in iteritems(params['kwargs']):
@@ -5338,29 +5364,34 @@
                                         callback=params.get('callback'),
                                         _return_http_data_only=params.get('_return_http_data_only'),
                                         _preload_content=params.get('_preload_content', True),
                                         _request_timeout=params.get('_request_timeout'),
                                         collection_formats=http_params['collection_formats'])
 
 
-
+    def delete_work_sheet_hyperlinks(self, request, **kwargs):
+        warnings.warn("delete_work_sheet_hyperlinks is deprecated", DeprecationWarning)
+        return self.delete_worksheet_hyperlinks(request,kwargs)
+    def delete_work_sheet_hyperlinks_with_http_info(self, request, **kwargs):
+        warnings.warn("delete_work_sheet_hyperlinks_with_http_info is deprecated", DeprecationWarning)
+        return self.delete_worksheet_hyperlinks_with_http_info(request,kwargs) 
     # <summary>
     # </summary>
-    # <param name="request">Request. <see cref="DeleteWorkSheetHyperlinksRequest" /></param>
-    def delete_work_sheet_hyperlinks(self, request, **kwargs):
+    # <param name="request">Request. <see cref="DeleteWorksheetHyperlinksRequest" /></param>
+    def delete_worksheet_hyperlinks(self, request, **kwargs):
 
         kwargs['_return_http_data_only'] = True
         self.check_access_token()
         if kwargs.get('callback'):
-            return self.delete_work_sheet_hyperlinks_with_http_info(request,**kwargs)
+            return self.delete_worksheet_hyperlinks_with_http_info(request,**kwargs)
         else:
-            (data) = self.delete_work_sheet_hyperlinks_with_http_info(request,**kwargs)
+            (data) = self.delete_worksheet_hyperlinks_with_http_info(request,**kwargs)
             return data
 
-    def delete_work_sheet_hyperlinks_with_http_info(self, request, **kwargs):
+    def delete_worksheet_hyperlinks_with_http_info(self, request, **kwargs):
         all_params = []
         all_params.append('callback')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
         params = locals()
         for key, val in iteritems(params['kwargs']):
@@ -7923,29 +7954,34 @@
                                         callback=params.get('callback'),
                                         _return_http_data_only=params.get('_return_http_data_only'),
                                         _preload_content=params.get('_preload_content', True),
                                         _request_timeout=params.get('_request_timeout'),
                                         collection_formats=http_params['collection_formats'])
 
 
-
+    def post_work_sheet_picture(self, request, **kwargs):
+        warnings.warn("post_work_sheet_picture is deprecated", DeprecationWarning)
+        return self.post_worksheet_picture(request,kwargs)
+    def post_work_sheet_picture_with_http_info(self, request, **kwargs):
+        warnings.warn("post_work_sheet_picture_with_http_info is deprecated", DeprecationWarning)
+        return self.post_worksheet_picture_with_http_info(request,kwargs)
     # <summary>
     # </summary>
-    # <param name="request">Request. <see cref="PostWorkSheetPictureRequest" /></param>
-    def post_work_sheet_picture(self, request, **kwargs):
+    # <param name="request">Request. <see cref="PostWorksheetPictureRequest" /></param>
+    def post_worksheet_picture(self, request, **kwargs):
 
         kwargs['_return_http_data_only'] = True
         self.check_access_token()
         if kwargs.get('callback'):
-            return self.post_work_sheet_picture_with_http_info(request,**kwargs)
+            return self.post_worksheet_picture_with_http_info(request,**kwargs)
         else:
-            (data) = self.post_work_sheet_picture_with_http_info(request,**kwargs)
+            (data) = self.post_worksheet_picture_with_http_info(request,**kwargs)
             return data
 
-    def post_work_sheet_picture_with_http_info(self, request, **kwargs):
+    def post_worksheet_picture_with_http_info(self, request, **kwargs):
         all_params = []
         all_params.append('callback')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
         params = locals()
         for key, val in iteritems(params['kwargs']):
@@ -8017,29 +8053,34 @@
                                         callback=params.get('callback'),
                                         _return_http_data_only=params.get('_return_http_data_only'),
                                         _preload_content=params.get('_preload_content', True),
                                         _request_timeout=params.get('_request_timeout'),
                                         collection_formats=http_params['collection_formats'])
 
 
-
+    def post_work_sheet_pictures(self, request, **kwargs):
+        warnings.warn("post_work_sheet_pictures is deprecated", DeprecationWarning)
+        return self.post_worksheet_pictures(request,kwargs)
+    def post_work_sheet_pictures_with_http_info(self, request, **kwargs):
+        warnings.warn("post_work_sheet_pictures_with_http_info is deprecated", DeprecationWarning)
+        return self.post_worksheet_pictures_with_http_info(request,kwargs)
     # <summary>
     # </summary>
-    # <param name="request">Request. <see cref="DeleteWorkSheetPicturesRequest" /></param>
-    def delete_work_sheet_pictures(self, request, **kwargs):
+    # <param name="request">Request. <see cref="DeleteWorksheetPicturesRequest" /></param>
+    def delete_worksheet_pictures(self, request, **kwargs):
 
         kwargs['_return_http_data_only'] = True
         self.check_access_token()
         if kwargs.get('callback'):
-            return self.delete_work_sheet_pictures_with_http_info(request,**kwargs)
+            return self.delete_worksheet_pictures_with_http_info(request,**kwargs)
         else:
-            (data) = self.delete_work_sheet_pictures_with_http_info(request,**kwargs)
+            (data) = self.delete_worksheet_pictures_with_http_info(request,**kwargs)
             return data
 
-    def delete_work_sheet_pictures_with_http_info(self, request, **kwargs):
+    def delete_worksheet_pictures_with_http_info(self, request, **kwargs):
         all_params = []
         all_params.append('callback')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
         params = locals()
         for key, val in iteritems(params['kwargs']):
```

### Comparing `asposecellscloud-23.4/asposecellscloud/apis/light_cells_api.py` & `asposecellscloud-23.5/asposecellscloud/apis/light_cells_api.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/apis/lite_cells_api.py` & `asposecellscloud-23.5/asposecellscloud/apis/lite_cells_api.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/configuration.py` & `asposecellscloud-23.5/asposecellscloud/configuration.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/__init__.py` & `asposecellscloud-23.5/asposecellscloud/models/__init__.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/above_average.py` & `asposecellscloud-23.5/asposecellscloud/models/above_average.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/access_token_response.py` & `asposecellscloud-23.5/asposecellscloud/models/access_token_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/area.py` & `asposecellscloud-23.5/asposecellscloud/models/area.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/auto_filter.py` & `asposecellscloud-23.5/asposecellscloud/models/auto_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/auto_filter_response.py` & `asposecellscloud-23.5/asposecellscloud/models/auto_filter_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/auto_fitter_options.py` & `asposecellscloud-23.5/asposecellscloud/models/auto_fitter_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/auto_shape.py` & `asposecellscloud-23.5/asposecellscloud/models/auto_shape.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/auto_shape_response.py` & `asposecellscloud-23.5/asposecellscloud/models/auto_shape_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/auto_shapes.py` & `asposecellscloud-23.5/asposecellscloud/models/auto_shapes.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/auto_shapes_response.py` & `asposecellscloud-23.5/asposecellscloud/models/auto_shapes_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/axis.py` & `asposecellscloud-23.5/asposecellscloud/models/axis.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/axis_response.py` & `asposecellscloud-23.5/asposecellscloud/models/axis_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/barcode_response.py` & `asposecellscloud-23.5/asposecellscloud/models/barcode_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/barcode_response_list.py` & `asposecellscloud-23.5/asposecellscloud/models/barcode_response_list.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/batch_convert_request.py` & `asposecellscloud-23.5/asposecellscloud/models/batch_convert_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/border.py` & `asposecellscloud-23.5/asposecellscloud/models/border.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/calculation_options.py` & `asposecellscloud-23.5/asposecellscloud/models/calculation_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/cell.py` & `asposecellscloud-23.5/asposecellscloud/models/cell.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/cell_area.py` & `asposecellscloud-23.5/asposecellscloud/models/cell_area.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/cell_response.py` & `asposecellscloud-23.5/asposecellscloud/models/cell_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/cell_value.py` & `asposecellscloud-23.5/asposecellscloud/models/cell_value.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/cells.py` & `asposecellscloud-23.5/asposecellscloud/models/cells.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/cells_cloud_file_info.py` & `asposecellscloud-23.5/asposecellscloud/models/cells_cloud_file_info.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/cells_cloud_response.py` & `asposecellscloud-23.5/asposecellscloud/models/cells_cloud_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/cells_color.py` & `asposecellscloud-23.5/asposecellscloud/models/cells_color.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/cells_document_properties.py` & `asposecellscloud-23.5/asposecellscloud/models/cells_document_properties.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/cells_document_properties_response.py` & `asposecellscloud-23.5/asposecellscloud/models/cells_document_properties_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/cells_document_property.py` & `asposecellscloud-23.5/asposecellscloud/models/cells_document_property.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/cells_document_property_response.py` & `asposecellscloud-23.5/asposecellscloud/models/cells_document_property_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/cells_error.py` & `asposecellscloud-23.5/asposecellscloud/models/cells_error.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/cells_object_operate_task_parameter.py` & `asposecellscloud-23.5/asposecellscloud/models/cells_object_operate_task_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/cells_response.py` & `asposecellscloud-23.5/asposecellscloud/models/cells_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/chart.py` & `asposecellscloud-23.5/asposecellscloud/models/chart.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/chart_area.py` & `asposecellscloud-23.5/asposecellscloud/models/chart_area.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/chart_area_response.py` & `asposecellscloud-23.5/asposecellscloud/models/chart_area_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/chart_frame.py` & `asposecellscloud-23.5/asposecellscloud/models/chart_frame.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/chart_operate_parameter.py` & `asposecellscloud-23.5/asposecellscloud/models/chart_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/charts.py` & `asposecellscloud-23.5/asposecellscloud/models/charts.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/charts_response.py` & `asposecellscloud-23.5/asposecellscloud/models/charts_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/color.py` & `asposecellscloud-23.5/asposecellscloud/models/color.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/color_filter.py` & `asposecellscloud-23.5/asposecellscloud/models/color_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/color_filter_request.py` & `asposecellscloud-23.5/asposecellscloud/models/color_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/color_scale.py` & `asposecellscloud-23.5/asposecellscloud/models/color_scale.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/column.py` & `asposecellscloud-23.5/asposecellscloud/models/column.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/column_response.py` & `asposecellscloud-23.5/asposecellscloud/models/column_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/columns.py` & `asposecellscloud-23.5/asposecellscloud/models/columns.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/columns_response.py` & `asposecellscloud-23.5/asposecellscloud/models/columns_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/comment.py` & `asposecellscloud-23.5/asposecellscloud/models/comment.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/comment_response.py` & `asposecellscloud-23.5/asposecellscloud/models/comment_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/comments.py` & `asposecellscloud-23.5/asposecellscloud/models/comments.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/comments_response.py` & `asposecellscloud-23.5/asposecellscloud/models/comments_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/conditional_formatting.py` & `asposecellscloud-23.5/asposecellscloud/models/conditional_formatting.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/conditional_formatting_icon.py` & `asposecellscloud-23.5/asposecellscloud/models/conditional_formatting_icon.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/conditional_formatting_response.py` & `asposecellscloud-23.5/asposecellscloud/models/conditional_formatting_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/conditional_formatting_value.py` & `asposecellscloud-23.5/asposecellscloud/models/conditional_formatting_value.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/conditional_formattings.py` & `asposecellscloud-23.5/asposecellscloud/models/conditional_formattings.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/conditional_formattings_response.py` & `asposecellscloud-23.5/asposecellscloud/models/conditional_formattings_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/convert_task_parameter.py` & `asposecellscloud-23.5/asposecellscloud/models/convert_task_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/convert_worksheet_task_parameter.py` & `asposecellscloud-23.5/asposecellscloud/models/convert_worksheet_task_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/copy_options.py` & `asposecellscloud-23.5/asposecellscloud/models/copy_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/create_pivot_table_request.py` & `asposecellscloud-23.5/asposecellscloud/models/create_pivot_table_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/custom_filter.py` & `asposecellscloud-23.5/asposecellscloud/models/custom_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/custom_parser_config.py` & `asposecellscloud-23.5/asposecellscloud/models/custom_parser_config.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/data_bar.py` & `asposecellscloud-23.5/asposecellscloud/models/data_bar.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/data_bar_border.py` & `asposecellscloud-23.5/asposecellscloud/models/data_bar_border.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/data_sorter.py` & `asposecellscloud-23.5/asposecellscloud/models/data_sorter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/dif_save_options.py` & `asposecellscloud-23.5/asposecellscloud/models/dif_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/disc_usage.py` & `asposecellscloud-23.5/asposecellscloud/models/disc_usage.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/docx_save_options.py` & `asposecellscloud-23.5/asposecellscloud/models/docx_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/dynamic_filter.py` & `asposecellscloud-23.5/asposecellscloud/models/dynamic_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/error_details.py` & `asposecellscloud-23.5/asposecellscloud/models/error_details.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/file_info.py` & `asposecellscloud-23.5/asposecellscloud/models/file_info.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/file_source.py` & `asposecellscloud-23.5/asposecellscloud/models/file_source.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/file_version.py` & `asposecellscloud-23.5/asposecellscloud/models/file_version.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/file_versions.py` & `asposecellscloud-23.5/asposecellscloud/models/file_versions.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/files_list.py` & `asposecellscloud-23.5/asposecellscloud/models/files_list.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/files_result.py` & `asposecellscloud-23.5/asposecellscloud/models/files_result.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/files_upload_result.py` & `asposecellscloud-23.5/asposecellscloud/models/files_upload_result.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/fill_format.py` & `asposecellscloud-23.5/asposecellscloud/models/fill_format.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/fill_format_response.py` & `asposecellscloud-23.5/asposecellscloud/models/fill_format_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/filter_column.py` & `asposecellscloud-23.5/asposecellscloud/models/filter_column.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/font.py` & `asposecellscloud-23.5/asposecellscloud/models/font.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/font_setting.py` & `asposecellscloud-23.5/asposecellscloud/models/font_setting.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/format_condition.py` & `asposecellscloud-23.5/asposecellscloud/models/format_condition.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/gradient_fill.py` & `asposecellscloud-23.5/asposecellscloud/models/gradient_fill.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/gradient_fill_stop.py` & `asposecellscloud-23.5/asposecellscloud/models/gradient_fill_stop.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/horizontal_page_break.py` & `asposecellscloud-23.5/asposecellscloud/models/horizontal_page_break.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/horizontal_page_break_response.py` & `asposecellscloud-23.5/asposecellscloud/models/horizontal_page_break_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/horizontal_page_breaks.py` & `asposecellscloud-23.5/asposecellscloud/models/horizontal_page_breaks.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/horizontal_page_breaks_response.py` & `asposecellscloud-23.5/asposecellscloud/models/horizontal_page_breaks_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/html_save_options.py` & `asposecellscloud-23.5/asposecellscloud/models/html_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/hyperlink.py` & `asposecellscloud-23.5/asposecellscloud/models/hyperlink.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/hyperlink_response.py` & `asposecellscloud-23.5/asposecellscloud/models/hyperlink_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/hyperlinks.py` & `asposecellscloud-23.5/asposecellscloud/models/hyperlinks.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/hyperlinks_response.py` & `asposecellscloud-23.5/asposecellscloud/models/hyperlinks_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/icon_filter.py` & `asposecellscloud-23.5/asposecellscloud/models/icon_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/icon_set.py` & `asposecellscloud-23.5/asposecellscloud/models/icon_set.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/image_save_options.py` & `asposecellscloud-23.5/asposecellscloud/models/image_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/import_batch_data_option.py` & `asposecellscloud-23.5/asposecellscloud/models/import_batch_data_option.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/import_csv_data_option.py` & `asposecellscloud-23.5/asposecellscloud/models/import_csv_data_option.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/import_data_task_parameter.py` & `asposecellscloud-23.5/asposecellscloud/models/import_data_task_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/import_double_array_option.py` & `asposecellscloud-23.5/asposecellscloud/models/import_double_array_option.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/import_int_array_option.py` & `asposecellscloud-23.5/asposecellscloud/models/import_int_array_option.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/import_option.py` & `asposecellscloud-23.5/asposecellscloud/models/import_option.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/import_picture_option.py` & `asposecellscloud-23.5/asposecellscloud/models/import_picture_option.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/import_position.py` & `asposecellscloud-23.5/asposecellscloud/models/import_position.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/import_string_array_option.py` & `asposecellscloud-23.5/asposecellscloud/models/import_string_array_option.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/import_xml_request.py` & `asposecellscloud-23.5/asposecellscloud/models/import_xml_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/json_save_options.py` & `asposecellscloud-23.5/asposecellscloud/models/json_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/legend.py` & `asposecellscloud-23.5/asposecellscloud/models/legend.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/legend_response.py` & `asposecellscloud-23.5/asposecellscloud/models/legend_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/line.py` & `asposecellscloud-23.5/asposecellscloud/models/line.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/line_format.py` & `asposecellscloud-23.5/asposecellscloud/models/line_format.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/line_response.py` & `asposecellscloud-23.5/asposecellscloud/models/line_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/link.py` & `asposecellscloud-23.5/asposecellscloud/models/link.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/link_element.py` & `asposecellscloud-23.5/asposecellscloud/models/link_element.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/list_column.py` & `asposecellscloud-23.5/asposecellscloud/models/list_column.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/list_object.py` & `asposecellscloud-23.5/asposecellscloud/models/list_object.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/list_object_operate_parameter.py` & `asposecellscloud-23.5/asposecellscloud/models/list_object_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/list_object_response.py` & `asposecellscloud-23.5/asposecellscloud/models/list_object_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/list_objects.py` & `asposecellscloud-23.5/asposecellscloud/models/list_objects.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/list_objects_response.py` & `asposecellscloud-23.5/asposecellscloud/models/list_objects_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/m_html_save_options.py` & `asposecellscloud-23.5/asposecellscloud/models/m_html_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/markdown_save_options.py` & `asposecellscloud-23.5/asposecellscloud/models/markdown_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/match_condition_request.py` & `asposecellscloud-23.5/asposecellscloud/models/match_condition_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/merged_cell.py` & `asposecellscloud-23.5/asposecellscloud/models/merged_cell.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/merged_cell_response.py` & `asposecellscloud-23.5/asposecellscloud/models/merged_cell_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/merged_cells.py` & `asposecellscloud-23.5/asposecellscloud/models/merged_cells.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/merged_cells_response.py` & `asposecellscloud-23.5/asposecellscloud/models/merged_cells_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/multiple_filter.py` & `asposecellscloud-23.5/asposecellscloud/models/multiple_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/multiple_filters.py` & `asposecellscloud-23.5/asposecellscloud/models/multiple_filters.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/name.py` & `asposecellscloud-23.5/asposecellscloud/models/name.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/name_response.py` & `asposecellscloud-23.5/asposecellscloud/models/name_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/names.py` & `asposecellscloud-23.5/asposecellscloud/models/names.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/names_response.py` & `asposecellscloud-23.5/asposecellscloud/models/names_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/negative_bar_format.py` & `asposecellscloud-23.5/asposecellscloud/models/negative_bar_format.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/object_exist.py` & `asposecellscloud-23.5/asposecellscloud/models/object_exist.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/ods_save_options.py` & `asposecellscloud-23.5/asposecellscloud/models/ods_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/ole_object.py` & `asposecellscloud-23.5/asposecellscloud/models/ole_object.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/ole_object_response.py` & `asposecellscloud-23.5/asposecellscloud/models/ole_object_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/ole_objects.py` & `asposecellscloud-23.5/asposecellscloud/models/ole_objects.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/ole_objects_response.py` & `asposecellscloud-23.5/asposecellscloud/models/ole_objects_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/ooxml_save_options.py` & `asposecellscloud-23.5/asposecellscloud/models/ooxml_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/operate_object.py` & `asposecellscloud-23.5/asposecellscloud/models/operate_object.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/operate_object_position.py` & `asposecellscloud-23.5/asposecellscloud/models/operate_object_position.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/operate_parameter.py` & `asposecellscloud-23.5/asposecellscloud/models/operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/page_break_operate_parameter.py` & `asposecellscloud-23.5/asposecellscloud/models/page_break_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/page_section.py` & `asposecellscloud-23.5/asposecellscloud/models/page_section.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/page_sections_response.py` & `asposecellscloud-23.5/asposecellscloud/models/page_sections_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/page_setup.py` & `asposecellscloud-23.5/asposecellscloud/models/page_setup.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/page_setup_operate_parameter.py` & `asposecellscloud-23.5/asposecellscloud/models/page_setup_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/page_setup_response.py` & `asposecellscloud-23.5/asposecellscloud/models/page_setup_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/password_request.py` & `asposecellscloud-23.5/asposecellscloud/models/password_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/paste_options.py` & `asposecellscloud-23.5/asposecellscloud/models/paste_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/pattern_fill.py` & `asposecellscloud-23.5/asposecellscloud/models/pattern_fill.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/pdf_save_options.py` & `asposecellscloud-23.5/asposecellscloud/models/pdf_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/pdf_security_options.py` & `asposecellscloud-23.5/asposecellscloud/models/pdf_security_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/pic_format_option.py` & `asposecellscloud-23.5/asposecellscloud/models/pic_format_option.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/picture.py` & `asposecellscloud-23.5/asposecellscloud/models/picture.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/picture_response.py` & `asposecellscloud-23.5/asposecellscloud/models/picture_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/pictures.py` & `asposecellscloud-23.5/asposecellscloud/models/pictures.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/pictures_response.py` & `asposecellscloud-23.5/asposecellscloud/models/pictures_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/pivot_field.py` & `asposecellscloud-23.5/asposecellscloud/models/pivot_field.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/pivot_field_response.py` & `asposecellscloud-23.5/asposecellscloud/models/pivot_field_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/pivot_filter.py` & `asposecellscloud-23.5/asposecellscloud/models/pivot_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/pivot_filter_response.py` & `asposecellscloud-23.5/asposecellscloud/models/pivot_filter_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/pivot_filters_response.py` & `asposecellscloud-23.5/asposecellscloud/models/pivot_filters_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/pivot_item.py` & `asposecellscloud-23.5/asposecellscloud/models/pivot_item.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/pivot_table.py` & `asposecellscloud-23.5/asposecellscloud/models/pivot_table.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/pivot_table_field_request.py` & `asposecellscloud-23.5/asposecellscloud/models/pivot_table_field_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/pivot_table_operate_parameter.py` & `asposecellscloud-23.5/asposecellscloud/models/pivot_table_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/pivot_table_response.py` & `asposecellscloud-23.5/asposecellscloud/models/pivot_table_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/pivot_tables.py` & `asposecellscloud-23.5/asposecellscloud/models/pivot_tables.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/pivot_tables_response.py` & `asposecellscloud-23.5/asposecellscloud/models/pivot_tables_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/pptx_save_options.py` & `asposecellscloud-23.5/asposecellscloud/models/pptx_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/protect_sheet_parameter.py` & `asposecellscloud-23.5/asposecellscloud/models/protect_sheet_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/range.py` & `asposecellscloud-23.5/asposecellscloud/models/range.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/range_copy_request.py` & `asposecellscloud-23.5/asposecellscloud/models/range_copy_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/range_set_outline_border_request.py` & `asposecellscloud-23.5/asposecellscloud/models/range_set_outline_border_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/range_set_style_request.py` & `asposecellscloud-23.5/asposecellscloud/models/range_set_style_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/range_value_response.py` & `asposecellscloud-23.5/asposecellscloud/models/range_value_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/ranges.py` & `asposecellscloud-23.5/asposecellscloud/models/ranges.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/ranges_response.py` & `asposecellscloud-23.5/asposecellscloud/models/ranges_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/result_destination.py` & `asposecellscloud-23.5/asposecellscloud/models/result_destination.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/row.py` & `asposecellscloud-23.5/asposecellscloud/models/row.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/row_response.py` & `asposecellscloud-23.5/asposecellscloud/models/row_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/rows.py` & `asposecellscloud-23.5/asposecellscloud/models/rows.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/rows_response.py` & `asposecellscloud-23.5/asposecellscloud/models/rows_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/save_options.py` & `asposecellscloud-23.5/asposecellscloud/models/save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/save_response.py` & `asposecellscloud-23.5/asposecellscloud/models/save_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/save_result.py` & `asposecellscloud-23.5/asposecellscloud/models/save_result.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/save_result_task_parameter.py` & `asposecellscloud-23.5/asposecellscloud/models/save_result_task_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/shadow_effect.py` & `asposecellscloud-23.5/asposecellscloud/models/shadow_effect.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/shape.py` & `asposecellscloud-23.5/asposecellscloud/models/shape.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/shape_operate_parameter.py` & `asposecellscloud-23.5/asposecellscloud/models/shape_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/shape_response.py` & `asposecellscloud-23.5/asposecellscloud/models/shape_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/shapes.py` & `asposecellscloud-23.5/asposecellscloud/models/shapes.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/shapes_response.py` & `asposecellscloud-23.5/asposecellscloud/models/shapes_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/single_value.py` & `asposecellscloud-23.5/asposecellscloud/models/single_value.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/single_value_response.py` & `asposecellscloud-23.5/asposecellscloud/models/single_value_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/smart_marker_task_parameter.py` & `asposecellscloud-23.5/asposecellscloud/models/smart_marker_task_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/solid_fill.py` & `asposecellscloud-23.5/asposecellscloud/models/solid_fill.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/sort_key.py` & `asposecellscloud-23.5/asposecellscloud/models/sort_key.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/sparkline.py` & `asposecellscloud-23.5/asposecellscloud/models/sparkline.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/sparkline_group.py` & `asposecellscloud-23.5/asposecellscloud/models/sparkline_group.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/sparkline_group_response.py` & `asposecellscloud-23.5/asposecellscloud/models/sparkline_group_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/sparkline_groups.py` & `asposecellscloud-23.5/asposecellscloud/models/sparkline_groups.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/sparkline_groups_response.py` & `asposecellscloud-23.5/asposecellscloud/models/sparkline_groups_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/split_result.py` & `asposecellscloud-23.5/asposecellscloud/models/split_result.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/split_result_document.py` & `asposecellscloud-23.5/asposecellscloud/models/split_result_document.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/split_result_response.py` & `asposecellscloud-23.5/asposecellscloud/models/split_result_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/split_workbook_task_parameter.py` & `asposecellscloud-23.5/asposecellscloud/models/split_workbook_task_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/spreadsheet_ml2003_save_options.py` & `asposecellscloud-23.5/asposecellscloud/models/spreadsheet_ml2003_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/sql_script_save_options.py` & `asposecellscloud-23.5/asposecellscloud/models/sql_script_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/storage_exist.py` & `asposecellscloud-23.5/asposecellscloud/models/storage_exist.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/storage_file.py` & `asposecellscloud-23.5/asposecellscloud/models/storage_file.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/style.py` & `asposecellscloud-23.5/asposecellscloud/models/style.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/style_response.py` & `asposecellscloud-23.5/asposecellscloud/models/style_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/svg_save_options.py` & `asposecellscloud-23.5/asposecellscloud/models/svg_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/table_total_request.py` & `asposecellscloud-23.5/asposecellscloud/models/table_total_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/task_data.py` & `asposecellscloud-23.5/asposecellscloud/models/task_data.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/task_description.py` & `asposecellscloud-23.5/asposecellscloud/models/task_description.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/task_parameter.py` & `asposecellscloud-23.5/asposecellscloud/models/task_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/text_item.py` & `asposecellscloud-23.5/asposecellscloud/models/text_item.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/text_items.py` & `asposecellscloud-23.5/asposecellscloud/models/text_items.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/text_items_response.py` & `asposecellscloud-23.5/asposecellscloud/models/text_items_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/text_options.py` & `asposecellscloud-23.5/asposecellscloud/models/text_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/text_water_marker_request.py` & `asposecellscloud-23.5/asposecellscloud/models/text_water_marker_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/texture_fill.py` & `asposecellscloud-23.5/asposecellscloud/models/texture_fill.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/theme_color.py` & `asposecellscloud-23.5/asposecellscloud/models/theme_color.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/tick_labels.py` & `asposecellscloud-23.5/asposecellscloud/models/tick_labels.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/tile_pic_option.py` & `asposecellscloud-23.5/asposecellscloud/models/tile_pic_option.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/title.py` & `asposecellscloud-23.5/asposecellscloud/models/title.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/title_response.py` & `asposecellscloud-23.5/asposecellscloud/models/title_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/top10.py` & `asposecellscloud-23.5/asposecellscloud/models/top10.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/top10_filter.py` & `asposecellscloud-23.5/asposecellscloud/models/top10_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/txt_save_options.py` & `asposecellscloud-23.5/asposecellscloud/models/txt_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/validation.py` & `asposecellscloud-23.5/asposecellscloud/models/validation.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/validation_response.py` & `asposecellscloud-23.5/asposecellscloud/models/validation_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/validations.py` & `asposecellscloud-23.5/asposecellscloud/models/validations.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/validations_response.py` & `asposecellscloud-23.5/asposecellscloud/models/validations_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/value_type.py` & `asposecellscloud-23.5/asposecellscloud/models/value_type.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/vertical_page_break.py` & `asposecellscloud-23.5/asposecellscloud/models/vertical_page_break.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/vertical_page_break_response.py` & `asposecellscloud-23.5/asposecellscloud/models/vertical_page_break_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/vertical_page_breaks.py` & `asposecellscloud-23.5/asposecellscloud/models/vertical_page_breaks.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/vertical_page_breaks_response.py` & `asposecellscloud-23.5/asposecellscloud/models/vertical_page_breaks_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/workbook.py` & `asposecellscloud-23.5/asposecellscloud/models/workbook.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/workbook_encryption_request.py` & `asposecellscloud-23.5/asposecellscloud/models/workbook_encryption_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/workbook_operate_parameter.py` & `asposecellscloud-23.5/asposecellscloud/models/workbook_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/workbook_protection_request.py` & `asposecellscloud-23.5/asposecellscloud/models/workbook_protection_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/workbook_replace_response.py` & `asposecellscloud-23.5/asposecellscloud/models/workbook_replace_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/workbook_response.py` & `asposecellscloud-23.5/asposecellscloud/models/workbook_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/workbook_settings.py` & `asposecellscloud-23.5/asposecellscloud/models/workbook_settings.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/workbook_settings_operate_parameter.py` & `asposecellscloud-23.5/asposecellscloud/models/workbook_settings_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/workbook_settings_response.py` & `asposecellscloud-23.5/asposecellscloud/models/workbook_settings_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/worksheet.py` & `asposecellscloud-23.5/asposecellscloud/models/worksheet.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/worksheet_moving_request.py` & `asposecellscloud-23.5/asposecellscloud/models/worksheet_moving_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/worksheet_operate_parameter.py` & `asposecellscloud-23.5/asposecellscloud/models/worksheet_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/worksheet_replace_response.py` & `asposecellscloud-23.5/asposecellscloud/models/worksheet_replace_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/worksheet_response.py` & `asposecellscloud-23.5/asposecellscloud/models/worksheet_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/worksheets.py` & `asposecellscloud-23.5/asposecellscloud/models/worksheets.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/worksheets_response.py` & `asposecellscloud-23.5/asposecellscloud/models/worksheets_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/xls_save_options.py` & `asposecellscloud-23.5/asposecellscloud/models/xls_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/xlsb_save_options.py` & `asposecellscloud-23.5/asposecellscloud/models/xlsb_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/models/xps_save_options.py` & `asposecellscloud-23.5/asposecellscloud/models/xps_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/asposecellscloud/rest.py` & `asposecellscloud-23.5/asposecellscloud/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,21 +53,21 @@
         self.reason = resp.reason
         self.data = resp.data
 
     def getheaders(self):
         """
         Returns a dictionary of the response headers.
         """
-        return self.urllib3_response.getheaders()
+        return self.urllib3_response.headers
 
     def getheader(self, name, default=None):
         """
         Returns a given response header.
         """
-        return self.urllib3_response.getheader(name, default)
+        return self.urllib3_response.headers.get(name, default)
 
 
 class RESTClientObject(object):
 
     def __init__(self, pools_size=4, maxsize=4):
         # urllib3.PoolManager will pass all kw parameters to connectionpool
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/poolmanager.py#L75
```

### Comparing `asposecellscloud-23.4/asposecellscloud.egg-info/PKG-INFO` & `asposecellscloud-23.5/asposecellscloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: asposecellscloud
-Version: 23.4
+Version: 23.5
 Summary: Python Cloud SDK wraps Aspose.Cells REST API so you could seamlessly integrate Microsoft Excel® spreadsheet generation, manipulation, conversion & inspection features into your own Python applications.
 Home-page: https://github.com/aspose-cells-cloud/aspose-cells-cloud-python
 Author: Aspose Cloud
 Author-email: aspose.cloud@aspose.com
 License: UNKNOWN
 Description: Python Cloud SDK wraps Aspose.Cells REST API so you could seamlessly integrate Microsoft Excel® spreadsheet generation, manipulation, conversion & inspection features into your own Python applications.
 Keywords: aspose,cells,cloud
```

### Comparing `asposecellscloud-23.4/asposecellscloud.egg-info/SOURCES.txt` & `asposecellscloud-23.5/asposecellscloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/setup.py` & `asposecellscloud-23.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages
 
 NAME = "asposecellscloud"
-VERSION = "23.4"
+VERSION = "23.5"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `asposecellscloud-23.4/test/test_cells_chart_axis_api.py` & `asposecellscloud-23.5/test/test_cells_chart_axis_api.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_auto_filter_controller.py` & `asposecellscloud-23.5/test/tests_auto_filter_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_batch_controller.py` & `asposecellscloud-23.5/test/tests_batch_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_cells_barcodes_controller.py` & `asposecellscloud-23.5/test/tests_cells_barcodes_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_cells_controller.py` & `asposecellscloud-23.5/test/tests_cells_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_cells_status_controller.py` & `asposecellscloud-23.5/test/tests_cells_status_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_chart_area_controller.py` & `asposecellscloud-23.5/test/tests_chart_area_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_charts_controller.py` & `asposecellscloud-23.5/test/tests_charts_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_conditional_formattings_controller.py` & `asposecellscloud-23.5/test/tests_conditional_formattings_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_conversion.py` & `asposecellscloud-23.5/test/tests_conversion.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_conversion_json.py` & `asposecellscloud-23.5/test/tests_conversion_json.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_conversion_png.py` & `asposecellscloud-23.5/test/tests_conversion_png.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_file_controller.py` & `asposecellscloud-23.5/test/tests_file_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_folder_controller.py` & `asposecellscloud-23.5/test/tests_folder_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_hypelinks_controller.py` & `asposecellscloud-23.5/test/tests_hypelinks_controller.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,88 +25,88 @@
         if global_api is None:
            global_api = CellsApi(AuthUtil.GetClientId(),AuthUtil.GetClientSecret(),"v3.0",AuthUtil.GetBaseUrl())
         self.api = global_api
 
     def tearDown(self):
         pass
 
-    def test_get_work_sheet_hyperlinks(self):
+    def test_get_worksheet_hyperlinks(self):
         remote_folder = 'TestData/In'
 
         local_name = 'Book1.xlsx'
         remote_name = 'Book1.xlsx'
 
         result = AuthUtil.Ready(self.api, local_name, remote_folder + '/' + remote_name ,  '')
         self.assertTrue(len(result.uploaded)>0) 
      
-        request =  GetWorkSheetHyperlinksRequest( remote_name, 'Sheet1',folder= remote_folder,storage_name= '')
-        self.api.get_work_sheet_hyperlinks(request)
+        request =  GetWorksheetHyperlinksRequest( remote_name, 'Sheet1',folder= remote_folder,storage_name= '')
+        self.api.get_worksheet_hyperlinks(request)
 
 
-    def test_get_work_sheet_hyperlink(self):
+    def test_get_worksheet_hyperlink(self):
         remote_folder = 'TestData/In'
 
         local_name = 'Book1.xlsx'
         remote_name = 'Book1.xlsx'
 
         result = AuthUtil.Ready(self.api, local_name, remote_folder + '/' + remote_name ,  '')
         self.assertTrue(len(result.uploaded)>0) 
      
         request =  GetWorkSheetHyperlinkRequest( remote_name, 'Sheet1', 0,folder= remote_folder,storage_name= '')
-        self.api.get_work_sheet_hyperlink(request)
+        self.api.get_worksheet_hyperlink(request)
 
 
-    def test_delete_work_sheet_hyperlink(self):
+    def test_delete_worksheet_hyperlink(self):
         remote_folder = 'TestData/In'
 
         local_name = 'Book1.xlsx'
         remote_name = 'Book1.xlsx'
 
         result = AuthUtil.Ready(self.api, local_name, remote_folder + '/' + remote_name ,  '')
         self.assertTrue(len(result.uploaded)>0) 
      
         request =  DeleteWorkSheetHyperlinkRequest( remote_name, 'Sheet1', 0,folder= remote_folder,storage_name= '')
-        self.api.delete_work_sheet_hyperlink(request)
+        self.api.delete_worksheet_hyperlink(request)
 
 
-    def test_post_work_sheet_hyperlink(self):
+    def test_post_worksheet_hyperlink(self):
         remote_folder = 'TestData/In'
 
         local_name = 'Book1.xlsx'
         remote_name = 'Book1.xlsx'
 
         hyperlink = Hyperlink(address= 'https://products.aspose.cloud/cells/' )
         result = AuthUtil.Ready(self.api, local_name, remote_folder + '/' + remote_name ,  '')
         self.assertTrue(len(result.uploaded)>0) 
      
         request =  PostWorkSheetHyperlinkRequest( remote_name, 'Sheet1', 0, hyperlink,folder= remote_folder,storage_name= '')
-        self.api.post_work_sheet_hyperlink(request)
+        self.api.post_worksheet_hyperlink(request)
 
 
-    def test_put_work_sheet_hyperlink(self):
+    def test_put_worksheet_hyperlink(self):
         remote_folder = 'TestData/In'
 
         local_name = 'Book1.xlsx'
         remote_name = 'Book1.xlsx'
 
         result = AuthUtil.Ready(self.api, local_name, remote_folder + '/' + remote_name ,  '')
         self.assertTrue(len(result.uploaded)>0) 
      
         request =  PutWorkSheetHyperlinkRequest( remote_name, 'Sheet1', 1, 1, 2, 3, 'https://products.aspose.cloud/cells/',folder= remote_folder,storage_name= '')
-        self.api.put_work_sheet_hyperlink(request)
+        self.api.put_worksheet_hyperlink(request)
 
 
-    def test_delete_work_sheet_hyperlinks(self):
+    def test_delete_worksheet_hyperlinks(self):
         remote_folder = 'TestData/In'
 
         local_name = 'Book1.xlsx'
         remote_name = 'Book1.xlsx'
 
         result = AuthUtil.Ready(self.api, local_name, remote_folder + '/' + remote_name ,  '')
         self.assertTrue(len(result.uploaded)>0) 
      
         request =  DeleteWorkSheetHyperlinksRequest( remote_name, 'Sheet1',folder= remote_folder,storage_name= '')
-        self.api.delete_work_sheet_hyperlinks(request)
+        self.api.delete_worksheet_hyperlinks(request)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `asposecellscloud-23.4/test/tests_light_cells.py` & `asposecellscloud-23.5/test/tests_light_cells.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_list_objects_controller.py` & `asposecellscloud-23.5/test/tests_list_objects_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_ole_objects_controller.py` & `asposecellscloud-23.5/test/tests_ole_objects_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_one.py` & `asposecellscloud-23.5/test/tests_one.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_page_breaks_controller.py` & `asposecellscloud-23.5/test/tests_page_breaks_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_page_setup_controller.py` & `asposecellscloud-23.5/test/tests_page_setup_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_pictures_controller.py` & `asposecellscloud-23.5/test/tests_pictures_controller.py`

 * *Files 11% similar despite different names*

```diff
@@ -67,26 +67,26 @@
         result = AuthUtil.Ready(self.api, water_mark_png, remote_folder + '/WaterMark.png' ,  '')
         self.assertTrue(len(result.uploaded)>0) 
      
         request =  PutWorksheetAddPictureRequest( remote_name, 'Sheet6',upper_left_row= 1,upper_left_column= 1,lower_right_row= 10,lower_right_column= 10,picture_path= remote_folder + '/WaterMark.png',folder= remote_folder,storage_name= '')
         self.api.put_worksheet_add_picture(request)
 
 
-    def test_post_work_sheet_picture(self):
+    def test_post_worksheet_picture(self):
         remote_folder = 'TestData/In'
 
         local_name = 'Book1.xlsx'
         remote_name = 'Book1.xlsx'
 
         picture = Picture(left= 10 ,bottom= 10 )
         result = AuthUtil.Ready(self.api, local_name, remote_folder + '/' + remote_name ,  '')
         self.assertTrue(len(result.uploaded)>0) 
      
         request =  PostWorkSheetPictureRequest( remote_name, 'Sheet6', 0, picture,folder= remote_folder,storage_name= '')
-        self.api.post_work_sheet_picture(request)
+        self.api.post_worksheet_picture(request)
 
 
     def test_delete_worksheet_picture(self):
         remote_folder = 'TestData/In'
 
         local_name = 'Book1.xlsx'
         remote_name = 'Book1.xlsx'
@@ -94,22 +94,22 @@
         result = AuthUtil.Ready(self.api, local_name, remote_folder + '/' + remote_name ,  '')
         self.assertTrue(len(result.uploaded)>0) 
      
         request =  DeleteWorksheetPictureRequest( remote_name, 'Sheet6', 0,folder= remote_folder,storage_name= '')
         self.api.delete_worksheet_picture(request)
 
 
-    def test_delete_work_sheet_pictures(self):
+    def test_delete_worksheet_pictures(self):
         remote_folder = 'TestData/In'
 
         local_name = 'Book1.xlsx'
         remote_name = 'Book1.xlsx'
 
         result = AuthUtil.Ready(self.api, local_name, remote_folder + '/' + remote_name ,  '')
         self.assertTrue(len(result.uploaded)>0) 
      
         request =  DeleteWorkSheetPicturesRequest( remote_name, 'Sheet6',folder= remote_folder,storage_name= '')
-        self.api.delete_work_sheet_pictures(request)
+        self.api.delete_worksheet_pictures(request)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `asposecellscloud-23.4/test/tests_pivot_tables_controller.py` & `asposecellscloud-23.5/test/tests_pivot_tables_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_properties_controller.py` & `asposecellscloud-23.5/test/tests_properties_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_ranges_controller.py` & `asposecellscloud-23.5/test/tests_ranges_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_shapes_controller.py` & `asposecellscloud-23.5/test/tests_shapes_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_sparkline_groups_controller.py` & `asposecellscloud-23.5/test/tests_sparkline_groups_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_storage_controller.py` & `asposecellscloud-23.5/test/tests_storage_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_workbook_controller.py` & `asposecellscloud-23.5/test/tests_workbook_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_worksheet_controller.py` & `asposecellscloud-23.5/test/tests_worksheet_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_worksheet_validations_controller.py` & `asposecellscloud-23.5/test/tests_worksheet_validations_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-23.4/test/tests_xml_controller.py` & `asposecellscloud-23.5/test/tests_xml_controller.py`

 * *Files identical despite different names*

