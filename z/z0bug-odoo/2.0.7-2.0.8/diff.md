# Comparing `tmp/z0bug_odoo-2.0.7.tar.gz` & `tmp/z0bug_odoo-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/z0bug_odoo-2.0.7.tar", last modified: Tue May  9 16:04:15 2023, max compression
+gzip compressed data, was "dist/z0bug_odoo-2.0.8.tar", last modified: Thu May 25 08:55:28 2023, max compression
```

## Comparing `z0bug_odoo-2.0.7.tar` & `z0bug_odoo-2.0.8.tar`

### file list

```diff
@@ -1,161 +1,162 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/__main__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5923 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/asset_category.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6015 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_payment_mode.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    17914 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_21.png
--rw-r--r--   0 odoo      (1000) odoo      (1000)     8512 2023-03-31 16:47:10.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/date_range.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    11354 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/res_partner.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5958 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_9.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    12377 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_12.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6863 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.partner_mycompany.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    28222 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_2.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5311 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_payment_method.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8641 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/res_country_state.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5736 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_payment_term.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    26659 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_5.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5254 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/italy_profile_account.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5649 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_fiscal_position_tax.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6034 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_payment_term_line.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     4933 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/decimal_precision.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5304 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/asset_asset.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6297 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/miscellaneous.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    21273 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_4.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    11254 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_tax.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6230 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_move_line.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     9845 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_24.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6256 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_10.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5320 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/res_bank.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8169 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_5.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    20091 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_6.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    20415 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_10.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5183 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/date_range_type.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    17619 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_3.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    23271 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_11.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    36713 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_account.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     9436 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_18.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6801 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/res_partner_bank.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5806 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/purchase_order.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5098 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_fiscal_year.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    13357 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_26.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    10816 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_19.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    40384 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/base.partner_admin.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5008 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/res_company.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    49021 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_6.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7618 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_14.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5548 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/product_supplierinfo.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6862 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_4.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6619 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/modules.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5485 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/withholding_tax.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7139 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_journal.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    14311 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_22.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7885 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/purchase_order_line.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    37268 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_8.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5063 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/stock_inventory.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5185 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/withholding_tax_rate.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    14221 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_16.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7940 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_15.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5681 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/asset_category_depreciation_type.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5797 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_16.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    15336 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_1.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    14581 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_1.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     3017 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_15.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5420 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_rc_type.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    10897 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_17.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5159 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_banking_mandate.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     4987 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/dichiarazione_intento_yearly_limit.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     9709 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_invoice_line.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8011 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/sale_order_line.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    14993 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_3.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5289 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/dichiarazione_intento.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5496 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/res_currency_rate.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7931 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_11.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6090 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_13.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7940 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_invoice.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5573 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_move.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7118 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_20.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     9911 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_13.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    12143 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_7.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    10429 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_12.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7695 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_8.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5119 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_rc_type_tax.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    15668 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_14.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     9180 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/product_product.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1436 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_7.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8985 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/product_template.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    12852 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_2.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6097 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/sale_order.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5212 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/stock_inventory_line.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6561 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_fiscal_position.xlsx
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo/scripts/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2311 2023-05-01 09:23:43.000000 z0bug_odoo-2.0.7/z0bug_odoo/scripts/setup.info
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6806 2023-05-01 08:26:51.000000 z0bug_odoo-2.0.7/z0bug_odoo/scripts/main.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/scripts/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4491 2023-04-15 07:28:59.000000 z0bug_odoo-2.0.7/z0bug_odoo/z0bug_odoo_lib.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo/testenv/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)   113219 2023-04-26 13:59:11.000000 z0bug_odoo-2.0.7/z0bug_odoo/testenv/testenv.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       46 2022-12-21 12:44:21.000000 z0bug_odoo-2.0.7/z0bug_odoo/testenv/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    12824 2023-04-15 07:28:59.000000 z0bug_odoo-2.0.7/z0bug_odoo/test_common.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    14660 2023-04-15 07:25:23.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/run_pylint.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/pylint_deprecated_modules/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/pylint_deprecated_modules/openerp/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/pylint_deprecated_modules/openerp/osv/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/pylint_deprecated_modules/openerp/osv/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)       68 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/pylint_deprecated_modules/openerp/__init__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      174 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/pylint_deprecated_modules/README.md
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/pylint_deprecated_modules/pudb.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/pylint_deprecated_modules/pdb.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/pylint_deprecated_modules/ipdb.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1515 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/git_run.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     3601 2023-04-15 07:28:59.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/get_test_dependencies.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2084 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/test_pylint
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8580 2023-04-15 07:28:59.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/getaddons.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3134 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/travis_test_dependencies
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6412 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/odoo_connection.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3551 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/apis.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2598 2023-04-15 07:28:59.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/test_flake8
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3843 2023-04-30 14:00:33.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/travis_run_tests
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1863 2023-04-15 07:25:46.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/travis_tnlbot.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     7550 2023-04-15 07:28:59.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/clone_oca_dependencies
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    28570 2023-04-15 07:28:59.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/test_server.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      668 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8__init__MINIMAL.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2005 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_pr.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      593 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8__init__REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      744 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8_REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      775 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      117 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_shellcheck.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8_AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      618 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_70.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1022 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8_NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8__init__AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8__init__.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2575 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2823 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_PYPI.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      619 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_61.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8__init__NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2526 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_beta.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      814 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8_MINIMAL.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3247 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/travis_makepot
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      263 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      120 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/travis_run_flake8
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      833 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/travis_helpers.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      780 2023-04-15 07:28:59.000000 z0bug_odoo-2.0.7/z0bug_odoo/__init__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       11 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo.egg-info/top_level.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-01-07 16:23:41.000000 z0bug_odoo-2.0.7/z0bug_odoo.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       66 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6100 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       44 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1181 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/setup.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2235 2023-05-04 12:56:37.000000 z0bug_odoo-2.0.7/setup.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1181 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    98395 2023-05-09 16:04:14.000000 z0bug_odoo-2.0.7/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/__main__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5923 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/asset_category.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6015 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_payment_mode.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    17914 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_21.png
+-rw-r--r--   0 odoo      (1000) odoo      (1000)     8512 2023-03-31 16:47:10.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/date_range.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    11354 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/res_partner.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5958 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_9.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    12377 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_12.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6863 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.partner_mycompany.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    28222 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_2.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5311 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_payment_method.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8641 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/res_country_state.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5736 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_payment_term.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    26659 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_5.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5254 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/italy_profile_account.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5649 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_fiscal_position_tax.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6034 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_payment_term_line.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4933 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/decimal_precision.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5304 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/asset_asset.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6297 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/miscellaneous.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    21273 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_4.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    11254 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_tax.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6230 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_move_line.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     9845 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_24.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6256 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_10.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5320 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/res_bank.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8169 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_5.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    20091 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_6.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    20415 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_10.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5183 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/date_range_type.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    17619 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_3.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    23271 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_11.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    36713 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_account.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     9436 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_18.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6801 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/res_partner_bank.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5806 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/purchase_order.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5098 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_fiscal_year.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    13357 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_26.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    10816 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_19.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    40384 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/base.partner_admin.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5008 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/res_company.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    49021 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_6.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7618 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_14.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5548 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/product_supplierinfo.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6862 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_4.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6619 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/modules.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5485 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/withholding_tax.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7139 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_journal.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    14311 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_22.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7885 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/purchase_order_line.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    37268 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_8.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5063 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/stock_inventory.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5185 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/withholding_tax_rate.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    14221 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_16.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7940 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_15.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5681 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/asset_category_depreciation_type.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5797 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_16.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    15336 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_1.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    14581 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_1.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3017 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_15.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5420 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_rc_type.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    10897 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_17.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5159 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_banking_mandate.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4987 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/dichiarazione_intento_yearly_limit.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     9709 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_invoice_line.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8011 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/sale_order_line.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    14993 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_3.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5289 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/dichiarazione_intento.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5496 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/res_currency_rate.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7931 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_11.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6090 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_13.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7940 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_invoice.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5573 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_move.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7118 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_20.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     9911 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_13.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    12143 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_7.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    10429 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_12.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7695 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_8.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5119 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_rc_type_tax.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    15668 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_14.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     9180 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/product_product.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1436 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_7.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8985 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/product_template.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    12852 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_2.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6097 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/sale_order.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5212 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/stock_inventory_line.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6561 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_fiscal_position.xlsx
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo/scripts/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2235 2023-05-20 08:36:32.000000 z0bug_odoo-2.0.8/z0bug_odoo/scripts/setup.info
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6806 2023-05-20 07:45:02.000000 z0bug_odoo-2.0.8/z0bug_odoo/scripts/main.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/scripts/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4491 2023-05-20 07:45:02.000000 z0bug_odoo-2.0.8/z0bug_odoo/z0bug_odoo_lib.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo/testenv/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5945 2023-05-24 07:12:36.000000 z0bug_odoo-2.0.8/z0bug_odoo/testenv/_check4deps_.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)   113576 2023-05-23 15:08:50.000000 z0bug_odoo-2.0.8/z0bug_odoo/testenv/testenv.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       73 2023-05-24 07:19:53.000000 z0bug_odoo-2.0.8/z0bug_odoo/testenv/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    12824 2023-05-20 07:45:02.000000 z0bug_odoo-2.0.8/z0bug_odoo/test_common.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    14660 2023-04-15 07:25:23.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/run_pylint.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/pylint_deprecated_modules/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/pylint_deprecated_modules/openerp/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/pylint_deprecated_modules/openerp/osv/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/pylint_deprecated_modules/openerp/osv/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)       68 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/pylint_deprecated_modules/openerp/__init__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      174 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/pylint_deprecated_modules/README.md
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/pylint_deprecated_modules/pudb.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/pylint_deprecated_modules/pdb.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/pylint_deprecated_modules/ipdb.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1515 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/git_run.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3601 2023-05-20 07:45:02.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/get_test_dependencies.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2084 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/test_pylint
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8580 2023-05-20 07:45:02.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/getaddons.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3134 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/travis_test_dependencies
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6412 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/odoo_connection.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3551 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/apis.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2598 2023-05-20 07:45:02.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/test_flake8
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3843 2023-05-20 07:45:02.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/travis_run_tests
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1863 2023-04-15 07:25:46.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/travis_tnlbot.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     7550 2023-05-20 07:45:02.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/clone_oca_dependencies
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    28570 2023-05-20 07:45:02.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/test_server.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      668 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8__init__MINIMAL.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2005 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_pr.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      593 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8__init__REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      744 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8_REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      775 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      117 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_shellcheck.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8_AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      618 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_70.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1022 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8_NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8__init__AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8__init__.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2575 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2823 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_PYPI.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      619 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_61.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8__init__NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2526 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_beta.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      814 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8_MINIMAL.cfg
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3247 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/travis_makepot
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      263 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      120 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/travis_run_flake8
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      833 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/travis_helpers.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      780 2023-05-20 07:45:02.000000 z0bug_odoo-2.0.8/z0bug_odoo/__init__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       11 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-01-07 16:23:41.000000 z0bug_odoo-2.0.8/z0bug_odoo.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       66 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6135 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       44 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1181 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/setup.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2235 2023-05-20 07:45:02.000000 z0bug_odoo-2.0.8/setup.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1181 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    97341 2023-05-21 13:34:13.000000 z0bug_odoo-2.0.8/README.rst
```

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/asset_category.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/asset_category.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/account_payment_mode.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/account_payment_mode.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_21.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_21.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/date_range.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/date_range.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/res_partner.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/res_partner.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_9.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_9.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_12.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_12.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.partner_mycompany.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.partner_mycompany.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_2.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_2.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/account_payment_method.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/account_payment_method.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/res_country_state.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/res_country_state.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/account_payment_term.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/account_payment_term.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_5.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_5.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/italy_profile_account.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/italy_profile_account.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/account_fiscal_position_tax.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/account_fiscal_position_tax.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/account_payment_term_line.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/account_payment_term_line.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/decimal_precision.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/decimal_precision.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/asset_asset.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/asset_asset.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/miscellaneous.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/miscellaneous.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_4.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_4.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/account_tax.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/account_tax.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/account_move_line.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/account_move_line.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_24.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_24.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_10.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_10.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/res_bank.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/res_bank.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_5.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_5.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_6.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_6.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_10.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_10.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/date_range_type.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/date_range_type.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_3.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_3.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_11.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_11.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/account_account.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/account_account.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_18.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_18.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/res_partner_bank.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/res_partner_bank.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/purchase_order.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/purchase_order.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/account_fiscal_year.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/account_fiscal_year.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_26.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_26.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_19.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_19.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/base.partner_admin.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/base.partner_admin.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/res_company.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/res_company.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_6.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_6.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_14.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_14.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/product_supplierinfo.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/product_supplierinfo.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_4.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_4.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/modules.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/modules.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/withholding_tax.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/withholding_tax.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/account_journal.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/account_journal.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_22.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_22.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/purchase_order_line.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/purchase_order_line.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_8.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_8.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/stock_inventory.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/stock_inventory.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/withholding_tax_rate.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/withholding_tax_rate.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_16.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_16.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_15.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_15.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/asset_category_depreciation_type.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/asset_category_depreciation_type.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_16.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_16.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_1.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_1.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_1.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_1.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_15.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_15.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/account_rc_type.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/account_rc_type.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_17.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_17.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/account_banking_mandate.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/account_banking_mandate.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/dichiarazione_intento_yearly_limit.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/dichiarazione_intento_yearly_limit.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/account_invoice_line.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/account_invoice_line.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/sale_order_line.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/sale_order_line.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_3.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_3.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/dichiarazione_intento.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/dichiarazione_intento.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/res_currency_rate.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/res_currency_rate.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_11.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_11.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_13.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_13.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/account_invoice.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/account_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/account_move.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/account_move.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_20.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_20.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_13.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_13.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_7.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_7.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_12.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_12.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_8.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_8.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/account_rc_type_tax.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/account_rc_type_tax.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_14.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_14.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/product_product.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/product_product.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_7.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_7.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/product_template.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/product_template.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_2.png` & `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_2.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/sale_order.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/sale_order.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/stock_inventory_line.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/stock_inventory_line.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/data/account_fiscal_position.xlsx` & `z0bug_odoo-2.0.8/z0bug_odoo/data/account_fiscal_position.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/scripts/setup.info` & `z0bug_odoo-2.0.8/z0bug_odoo/scripts/setup.info`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='z0bug_odoo',
-    version='2.0.7',
+    version='2.0.8',
     description='Odoo testing framework',
     long_description="""
 Zeroincombenze(R) continuous testing framework for Odoo modules.
 
 Make avaiable test functions indipendent by Odoo version.
 """,
     classifiers=[
@@ -28,16 +28,15 @@
     project_urls={
         'Documentation': 'https://zeroincombenze-tools.readthedocs.io',
         'Source': 'https://github.com/zeroincombenze/tools',
     },
     author='Antonio Maria Vigliotti',
     author_email='antoniomaria.vigliotti@gmail.com',
     license='Affero GPL',
-    # install_requires=['future', 'python-magic', 'clodoo', 'zerobug', 'gitPython'],
-    install_requires=['future', 'python-magic', 'zerobug', 'gitPython'],
+    install_requires=['future', 'python-magic', 'zerobug', 'gitPython', 'Click'],
     packages=find_packages(exclude=['docs', 'examples', 'tests', 'egg-info', 'junk']),
     package_data={
         '': [
             'scripts/setup.info',
             'data/*',
             'travis/cfg/*',
             'travis/pylint_deprecated_modules/*',
```

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/scripts/main.py` & `z0bug_odoo-2.0.8/z0bug_odoo/scripts/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
```

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/z0bug_odoo_lib.py` & `z0bug_odoo-2.0.8/z0bug_odoo/z0bug_odoo_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 
 from openpyxl import load_workbook
 
 
 from python_plus import unicodes
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 
 class Z0bugOdoo(object):
     def __init__(self, release=None):
         try:
             import odoo.release as release
```

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/testenv/testenv.py` & `z0bug_odoo-2.0.8/z0bug_odoo/testenv/testenv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-"""Test Environment v2.0.7.1
+"""Test Environment v2.0.8
 
 Copy this file in tests directory of your module.
 Please copy the documentation testenv.rst file too in your module.
 The __init__.py must import testenv.
 Your python test file should have to contain some following example lines:
 
 ::
@@ -1616,15 +1616,20 @@
         Returns:
             None
         """
         self.log_lvl_3("🐜  %s.onchange(%s=%s)" % (wizard, field, value))
         cur_vals = {}
         for name in wizard._fields.keys():
             if name not in SUPERMAGIC_COLUMNS:
-                cur_vals[name] = getattr(wizard, name)
+                try:
+                    cur_vals[name] = getattr(wizard, name)
+                except BaseException:
+                    self.raise_error(
+                        "Wrong compute for %s.%s! Forgot @multi?" % (wizard._name,
+                                                                     name))
         value = self._cast_field(resource, field, value, fmt="cmd")
         if value is not None:
             setattr(wizard, field, value)
         user_act = True
         while user_act:
             user_act = False
             for field in wizard._fields.keys():
@@ -2677,14 +2682,16 @@
         if len(record) > 1 or isinstance(record, (list, tuple)):
             for rec in record:
                 match = self.tmpl_init(
                     template, rec, nr=nr, repr=repr, rec_parent=rec_parent)
             return match
 
         resource = self._get_model_from_records(record)
+        if not resource:
+            self.raise_error("No valid record supplied for comparation!")
         self._load_field_struct(resource)
         childs_name = self.childs_name.get(resource)
         resource_child = self.childs_resource.get(resource)
         if resource_child:
             self._load_field_struct(resource_child)
         key = (rec_parent, record)
         template["_MATCH"] = template.get("_MATCH", {})
```

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/test_common.py` & `z0bug_odoo-2.0.8/z0bug_odoo/test_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     else:
         import odoo.tests.common as test_common
         from odoo.modules.module import get_module_resource  # noqa: F401
 else:
     print('No Odoo environment found!')
     sys.exit(0)
 
-__version__ = '2.0.7'
+__version__ = '2.0.8'
 
 
 class Z0bugBaseCase(test_common.BaseCase):
     def pool_env(self, model):
         """Return model pool_environment"""
         if int(release.major_version.split('.')[0]) < 8:
             return self.registry(model)
```

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/run_pylint.py` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/run_pylint.py`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/git_run.py` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/git_run.py`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/get_test_dependencies.py` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/get_test_dependencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     from test_server import get_test_dependencies
 except ImportError:
     from .getaddons import (get_dependencies, get_dependents, get_modules,
                             get_modules_info)
     from .test_server import get_test_dependencies
 
 
-__version__ = '2.0.7'
+__version__ = '2.0.8'
 
 
 def get_module_list(paths):
     res = []
     for path in paths.split(','):
         r = get_modules(os.path.expanduser(path))
         for m in r:
```

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/test_pylint` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/test_pylint`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/getaddons.py` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/getaddons.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     from git_run import GitRun
 except ImportError:
     try:
         from .git_run import GitRun
     except ImportError:
         from git_run import GitRun
 
-__version__ = '2.0.7'
+__version__ = '2.0.8'
 
 MANIFEST_FILES = ['__manifest__.py', '__odoo__.py', '__openerp__.py', '__terp__.py']
 
 
 def is_module(path):
     """return False if the path doesn't contain an odoo module, and the full
     path to the module manifest otherwise"""
```

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/travis_test_dependencies` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/travis_test_dependencies`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/odoo_connection.py` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/odoo_connection.py`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/apis.py` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/apis.py`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/test_flake8` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/test_flake8`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import subprocess
 import sys
 
 from getaddons import get_modules
 
 
-__version__ = '2.0.7'
+__version__ = '2.0.8'
 
 
 def get_build_dir():
     odoo_version = os.environ.get("VERSION")
     travis_base_dir = os.environ.get("TRAVIS_BUILD_DIR", "../..")
     tested_version = ''
     for ldir in ('./server/openerp', './openerp', './odoo'):
```

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/travis_run_tests` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/travis_run_tests`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 # import subprocess
 # import shutil
 import sys
 from distutils.spawn import find_executable
 from travis_helpers import success_msg, fail_msg
 
-__version__ = '2.0.7'
+__version__ = '2.0.8'
 
 
 def main(test_list):
     """
     Loop through each test and run them, add display results at the end
 
     If the test has a .py extension, import as a list and call main function
```

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/travis_tnlbot.py` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/travis_tnlbot.py`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/clone_oca_dependencies` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/clone_oca_dependencies`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import os.path as osp
 import subprocess
 import logging
 from travis_helpers import print_flush
 from z0lib import z0lib
 
 _logger = logging.getLogger()
-__version__ = '2.0.7'
+__version__ = '2.0.8'
 
 
 def create_deps():
     return {
         'reqfilenames': [],
         'processed': set(),
     }
```

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/test_server.py` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/test_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                             get_modules, get_modules_info)
     from .travis_helpers import fail_msg, print_flush, success_msg
 try:
     import ConfigParser
 except ImportError:
     import configparser as ConfigParser
 
-__version__ = '2.0.7'
+__version__ = '2.0.8'
 
 LDIR = ('server/openerp', 'odoo/odoo', 'openerp', 'odoo')
 
 
 def has_test_errors(fname, dbname, odoo_version, check_loaded=True):
     """
     Check a list of log lines for test errors.
```

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8__init__MINIMAL.cfg` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8__init__MINIMAL.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_pr.cfg` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_pr.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8__init__REDUCED.cfg` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8__init__REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8_REDUCED.cfg` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8_REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_REDUCED.cfg` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8_AVERAGE.cfg` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8_AVERAGE.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_70.cfg` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_70.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8_NEARBY.cfg` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8_NEARBY.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8.cfg` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint.cfg` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_PYPI.cfg` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_PYPI.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_61.cfg` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_61.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_beta.cfg` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_beta.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8_MINIMAL.cfg` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8_MINIMAL.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/travis_makepot` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/travis_makepot`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/travis/travis_helpers.py` & `z0bug_odoo-2.0.8/z0bug_odoo/travis/travis_helpers.py`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo/__init__.py` & `z0bug_odoo-2.0.8/z0bug_odoo/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 except ImportError:
     try:
         import openerp.release as release
         from . import test_common
     except ImportError:
         release = ''
 
-__version__ = '2.0.7'
+__version__ = '2.0.8'
 if eval(os.environ.get('TRAVIS_DEBUG_MODE', '0')) > 2:
     print('DEBUG: z0bug_odoo %s' % __version__)
     print('DEBUG: z0bug_odoo.sys.path=%s' % sys.path)
     if release:
         print('DEBUG: Odoo version detected: %s' % release.version)
     else:
         print('DEBUG: No Odoo environment found!')
```

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo.egg-info/SOURCES.txt` & `z0bug_odoo-2.0.8/z0bug_odoo.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -97,14 +97,15 @@
 z0bug_odoo/data/z0bug.res_partner_6.png
 z0bug_odoo/data/z0bug.res_partner_7.png
 z0bug_odoo/data/z0bug.res_partner_8.png
 z0bug_odoo/scripts/__init__.py
 z0bug_odoo/scripts/main.py
 z0bug_odoo/scripts/setup.info
 z0bug_odoo/testenv/__init__.py
+z0bug_odoo/testenv/_check4deps_.py
 z0bug_odoo/testenv/testenv.py
 z0bug_odoo/travis/__init__.py
 z0bug_odoo/travis/apis.py
 z0bug_odoo/travis/clone_oca_dependencies
 z0bug_odoo/travis/get_test_dependencies.py
 z0bug_odoo/travis/getaddons.py
 z0bug_odoo/travis/git_run.py
```

### Comparing `z0bug_odoo-2.0.7/z0bug_odoo.egg-info/PKG-INFO` & `z0bug_odoo-2.0.8/z0bug_odoo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: z0bug-odoo
-Version: 2.0.7
+Version: 2.0.8
 Summary: Odoo testing framework
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
```

### Comparing `z0bug_odoo-2.0.7/setup.py` & `z0bug_odoo-2.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='z0bug_odoo',
-    version='2.0.7',
+    version='2.0.8',
     description='Odoo testing framework',
     long_description="""
 Zeroincombenze(R) continuous testing framework for Odoo modules.
 
 Make avaiable test functions indipendent by Odoo version.
 """,
     classifiers=[
```

### Comparing `z0bug_odoo-2.0.7/PKG-INFO` & `z0bug_odoo-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: z0bug_odoo
-Version: 2.0.7
+Version: 2.0.8
 Summary: Odoo testing framework
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
```

### Comparing `z0bug_odoo-2.0.7/README.rst` & `z0bug_odoo-2.0.8/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 ================
-z0bug_odoo 2.0.7
+z0bug_odoo 2.0.8
 ================
 
 
 
-|Maturity| |Build Status| |Coverage Status| |license gpl|
+|Maturity| |license gpl|
 
 
 
 
 Overview
 ========
 
@@ -1787,19 +1787,14 @@
 |
 |
 
 Getting started
 ===============
 
 
-|
-
-Installation
-------------
-
 For stable version:
 
 `pip install z0bug_odoo`
 
 For current version:
 
 `cd $HOME`
@@ -1807,50 +1802,40 @@
 `cd $HOME/tools`
 `./install_tools.sh`
 
 
 Upgrade
 -------
 
-Upgrade
--------
-
 Stable version via Python Package
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+::
+
     pip install z0bug_odoo -U
 
 |
 
-Current stable version
-~~~~~~~~~~~~~~~~~~~~~~
+Current version via Git
+~~~~~~~~~~~~~~~~~~~~~~~
 
 ::
 
     cd $HOME
     ./install_tools.sh -U
-    source /opt/odoo/devel/activate_tools
-
-Current development version
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-::
-
-    cd $HOME
-    ./install_tools.sh -Ud
-    source /opt/odoo/devel/activate_tools
+    source $HOME/devel/activate_tools
 
 
 History
 -------
 
-2.0.7.1 (2023-04-26)
-~~~~~~~~~~~~~~~~~~~~
+2.0.8 (2023-04-26)
+~~~~~~~~~~~~~~~~~~
 
-* [FIX] TestEnv: multiple actione on the same records
+* [FIX] TestEnv: multiple action on the same records
 
 2.0.7 (2023-04-08)
 ~~~~~~~~~~~~~~~~~~
 
 * [NEW] TestEnv: assertion counter
 * [IMP] TestEnv: is_xref recognizes dot name, i.e "zobug.external.10"
 * [IMP] TestEnv: the field <description> is not mode key (only acount.tax)
@@ -1939,58 +1924,44 @@
 SHS-AV s.r.l. <https://www.shs-av.com/>
 
 
 Contributors
 ------------
 
 * Antonio M. Vigliotti <info@shs-av.com>
+* Antonio Maria Vigliotti <antoniomaria.vigliotti@gmail.com>
 Contributors
 ------------
 
 
 
 |
 
 This module is part of tools project.
 
-Last Update / Ultimo aggiornamento: 2023-05-01
+Last Update / Ultimo aggiornamento: 2023-05-21
 
 .. |Maturity| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: 
-.. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=master
-    :target: https://travis-ci.com/zeroincombenze/tools
-    :alt: github.com
 .. |license gpl| image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 .. |license opl| image:: https://img.shields.io/badge/licence-OPL-7379c3.svg
     :target: https://www.odoo.com/documentation/user/9.0/legal/licenses/licenses.html
     :alt: License: OPL
-.. |Coverage Status| image:: https://coveralls.io/repos/github/zeroincombenze/tools/badge.svg?branch=master
-    :target: https://coveralls.io/github/zeroincombenze/tools?branch=2.0
-    :alt: Coverage
-.. |Codecov Status| image:: https://codecov.io/gh/zeroincombenze/tools/branch/2.0/graph/badge.svg
-    :target: https://codecov.io/gh/zeroincombenze/tools/branch/2.0
-    :alt: Codecov
 .. |Tech Doc| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-docs-2.svg
     :target: https://wiki.zeroincombenze.org/en/Odoo/2.0/dev
     :alt: Technical Documentation
 .. |Help| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-help-2.svg
     :target: https://wiki.zeroincombenze.org/it/Odoo/2.0/man
     :alt: Technical Documentation
 .. |Try Me| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-try-it-2.svg
     :target: https://erp2.zeroincombenze.it
     :alt: Try Me
-.. |OCA Codecov| image:: https://codecov.io/gh/OCA/tools/branch/2.0/graph/badge.svg
-    :target: https://codecov.io/gh/OCA/tools/branch/2.0
-    :alt: Codecov
-.. |Odoo Italia Associazione| image:: https://www.odoo-italia.org/images/Immagini/Odoo%20Italia%20-%20126x56.png
-   :target: https://odoo-italia.org
-   :alt: Odoo Italia Associazione
 .. |Zeroincombenze| image:: https://avatars0.githubusercontent.com/u/6972555?s=460&v=4
    :target: https://www.zeroincombenze.it/
    :alt: Zeroincombenze
 .. |en| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/flags/en_US.png
    :target: https://www.facebook.com/Zeroincombenze-Software-gestionale-online-249494305219415/
 .. |it| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/flags/it_IT.png
    :target: https://www.facebook.com/Zeroincombenze-Software-gestionale-online-249494305219415/
```

